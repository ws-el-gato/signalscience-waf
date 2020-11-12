# JIRA

Our JIRA issue integration creates an issue when IPs are flagged on Signal Sciences.



# Adding a JIRA issue integration
JIRA issue integrations are configured per project.

1. Within JIRA, go to Settings > Site Administration > User management.

2. Create a user called e.g. “Create Ticket User”.
3. Confirm the user’s account and set a password.
4. Create an API token for that user
5. On Signal Sciences, go to ***Site Manage > Site Integrations.***
6. Click ***Add site integration*** and select the ***Jira Issue*** integration.
7. Enter the host for your JIRA instance and the username of the user and API Token you created.
8. Enter the key for the project you’d like to create the ticket in.
9. Click Add.


# Activity types

| Activity type | Description |
| ------------- | ------------- |
| flag | An IP was flagged |
| agentAlert |	An agent alert was triggered |

