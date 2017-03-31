# JIRA Custom UI (JIRACU)
A customizable minimal frontend for JIRA

## Purpose / Usecase
External users need to access a specific set of issues, without ever knowing what is going on behind the scenes. These users might be customers, external developers, your bosses etc.

Think of _JIRACU_ as some sort of firewall, that exposes only the data (and functionality) you'd like to expose.

## Features
- Customization without an additional administrative UI: You can configure _JIRACU_ by using JIRA standard mechanisms.
- No additional services needed: _JIRACU_ doesn't require the installation of any additional services like databases etc. Just start with `npm start` and you are ready to go

## Configuration
### Users

You need to add your users as you would normally do (in JIRA). The credentials required to authenticate in _JIRACU_ are identical to those you use to login to your JIRA instance.

### Issue views
A _JIRACU_ user is only able to see issues that where explicitly shared with him. Issues are shared by creating a filter, defining the visible columns within it, and finally sharing the filter with your external user. The is only able to view issues that are contained in one of the filter results shared with him. Furthermore only the fields you defined in your filter (as columns) will be displayed.
