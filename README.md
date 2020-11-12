# Signal Sciences Project Proposal for WellSky

## Signal Sciences Value Proposition
### 

1. Signal Sciences provides a menu of deployment options to cover diverse environments (modules for IIS, NGINX, node.js, many patterns for Kubernetes, Cloud WAF))
 
2. Signal Sciences uses a proprietary detection method, SmartParse to analyze request parameters to determine whether the code is actually executable and tokenizes the results. The tokenized representation of the request is analyzed, at runtime, to detect attacks such as SQLi, XSS, and other OWASP Top 10 injection attacks. This approach has a much lower false positive rate and is much faster than signature-based detection approaches.
 
  3. Threshold-based approach provides ‘high fidelity’ event summaries to reduce alert fatigue (compared to long lists of requests, etc). We have integrations built for Splunk, Slack, Teams, PagerDuty and more.



## Goals & Objectives of WAF Project 
###

* Easy to implement & maintain. 
* Low management overhead 
* Ability to deploy into pre-production in Blocking mode
Installation & transition to Blocking Mode does not result in performance hits. 
* Provides visibility into Layer 7 attacks and anomalies. 

* Ability to easily understand attack type and what rules have been triggered Accurate, effective detection of OWASP attacks with low false positive rate

* SIEM integration with SPLUNK

* Track False Positives (if any) (what is it, why did it occur, how can we fix it?)
* Latency measures pre/post SigSci implementation

* Simulate tabletop exercise for an incident 

# Project Success Criteria 
###


| Criteria                                                       | How will this be tested/validated?                                                                                                                                                     | Yes/No |
| -------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------ |
| Ease of deployment, implementation & management                | Deploys quickly, doesn’t require tuning of OWASP rulesets, scales across different environments                                                                                        | NA     |
| User friendly                                                  | Easy to configure rules, manage dashboards & look into specific request details                                                                                                        | NA     |
| Actionable visibility & accurate detection                     | Low to no false positives, while able to detect scans run in preprod                                                                                                                   | NA     |
| Low performance impact ***                                     | Determine performance is not impacted pre/post deployment                                                                                                                              | NA     |
| SIEM/Splunk integration                                        | Integrates with Splunk (may have to test this on Sumo)                                                                                                                                 | NA     |
| DevOps friendly (scales with deployments)                      | Integrates into DevOps workflows                                                                                                                                                       | NA     |
| Simulate tabletop exercise for an incident                     | Smaller group determines incident parameters, then operators and SigSci team will observe the incident. Walkthrough entire security event and determine if proper measures were taken. | NA     |
| Protecting public End Points from Business logic style attacks | Advanced features (specifically Rate Limiting) allows for visibility and blocking on those more sophisticated attacks                                                                  | NA     |




# Project Milestones 



| Milestone                                                                          | Target completion date |
| ---------------------------------------------------------------------------------- | ---------------------- |
| Determine preferred deployment method, complete Pre-Deployment Questionnaire       | August 21st            |
| POC Planning: Review POC Plan & Success Criteria, dashboard walkthrough & training | November 6th           |
| POC Kick-off: Install agents, review configuration &  schedule check-in calls      | November 11th          |
| Internal Testing in pre-production environment (dev, QA, staging)                  | November 11-30th       |
| Move to Production                                                                 | December 1st           |
| POC Conclusion: review results & determine if Signal Sciences is technical fit     | December 11th          |
| Solution selected, contracting and security onboarding executed                    | December 31st          |

### Testing Environment & Project Team

Application(s) being used for testing: 
 Deployment Method:

***POC Team:***
- Josh Hull
- Jami Albro-Fisher
- Sean Zehnder
- Jordan Robison
- Suman Shrestha
- David Teague

***Other Key Stakeholders:*** 
- CTO - Joel Dolisy *(will be involved in the entire POC process, and likely will be the ultimate signer)*

- SigSci Account Executive: Austin Hasche
- SigSci Sales Engineers: Aaron Attarzadeh
- SigSci Sales Manager: Jim Rose
- Kudelski Security: Clark Stinson
- Kudelski Security: Chris Haack

### *For more Details on Signal Science's WAF please visit: https://docs.signalsciences.net/*