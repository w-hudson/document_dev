# Alerts

<!--- Adapted from ZTAP UI Overview on Confluence -->

The **Alerts** screen is where most of the work in ZTAP is done. The main view lists the currently open alerts, based on any default search filtering criteria you have selected. For information on working in an individual alert, see [Working with individual Alerts](#working-with-individual-alerts).

## Alerts interface
![Alerts main screen](https://github.com/w-hudson/document_dev/blob/master/media/Alerts_1.png)

1. **Incident count**: The total number of incidents that match the current filter in the search bar. If the filter is blank, this will show the total number of Alerts across all organizations where the current user is a member.
2. **Bulk Actions**: This feature allows a user to take bulk actions on all of the Alerts displayed based on the current search filter settings. The available bulk actions are **CLOSE** and **ASSIGN TO ME**. If you use the bulk close action, you will be prompted to confirm before the incidents are closed.

   **IMPORTANT**: If no search filter options are designated, the selected action will apply to **all** Alerts. Ensure that your search filters are correct before you perform any bulk actions.
   
3. **Alert details page**: Open the individual Alert and show all related events in a detailed format. See [Working with individual Alerts](#working-with-individual-alerts). You can also click the icon to copy a link to the alert to your system's clipboard.
4. **Created/Updated date and status**: Shows the status of the incident (Open, Assigned, Reviewing, Closed) and when the incident was created and last updated.
5. **Organization & Assignment**: Shows the organization associated with the incident and the assigned group or user.
6. **Trigger event details**: A high-level look at the specific event that triggered the Alert.
7. **Comments**: This shows the total number of comments on an Alert. The most recent comment is usually shown at the bottom of the Alert.  
8. **Event details**: Shows how many total events are part of a particular incident and what products generated those events.
9. **TAP (Threat Analytics Plugin) Actions**: TAPs provide actions that can be taken during the investigation of an Alert, such as downloading the binary, retrieving hash analysis information, or isolating a host. The actions available in this section will differ based on the security products in your environment.
10. **Action bar**: Allows you to take action on an incident without needing to navigate into the incident itself: 
    - Escalate: Escalates an incident to another user or group.
    - Close: Closes the incident. You will be prompted to enter a reason and specify whether or not the incident was resolved. 
    - Assign to me: Assigns an incident to the current user.

## Working with individual Alerts
Click the title of an individual alert to open the Alert details screen.   

![Alert_Details](https://github.com/w-hudson/document_dev/blob/master/media/Alert_Detail_1.png)

1. **Incident number and Categories**:
2. **Created date and status**:
3. **Alert name**:
4. **Product and Assignment**:
5. **Event Information**: The information on these tabs can be useful for obtaining additional background information when you are investigating an Alert.
   - **Trigger Events**: These are events that caused the incident to be created and are considered to be "high-value" from an investigation perspective.
   - **Oberservations**: These are events that do not create an incident, but are instead designed to be helpful events that provide additional context. These types of events have been explicitly filtered by a senior analyst
   - **Whitelisted Events**: Events that have been explicitly whitelisted via the "Whitelist Trigger", the "Whitelist" button from within an incident, or a matching filter set to recategorize to Tier 3 will go into this section. These events may have been whitelisted from the incident they created, or they were whitelisted from another incident entirely
   - **Alert Timeline**: This view shows the specific details around events being added to the incident, groups / users being assigned, and other information with regards to the timeline of the incident
   - **Comments**: This view shows all comments pertaining to this incident with visibility to both analyst and client.
   - **Audit Log**: This page shows the historical timeline of actions and who performed them.
6. **Additional Actions**: 



:

   - Trigger Events: These are events that caused the incident to be created and are considered to be "high-value" from an investigation perspective. An event with the crosshair symbol (  ) indicates that this was the original event that created the incident and is the "main" event displayed in the ZTAP UI
   - Observations: These are events that do not create an incident, but are instead designed to be helpful events that provide additional context. These types of events have been explicitly filtered by a senior analyst
   - Whitelisted Events: Events that have been explicitly whitelisted via the "Whitelist Trigger", the "Whitelist" button from within an incident, or a matching filter set to recategorize to Tier 3 will go into this section. These events may have been whitelisted from the incident they created, or they were whitelisted from another incident entirely
   - Incident Timeline: This view shows the specific details around events being added to the incident, groups / users being assigned, and other information with regards to the timeline of the incident
   - Comments: This view shows all comments pertaining to this incident with visibility to both analyst and client. It is possible for private comments to be made so the other party can't see them. This is an option to provide advice/opinions so all shifts can be on the same page. 
   - Audit Log: This page shows the historical timeline of actions and who performed them. 

   You can edit the Alert title from this screen or the general ZTAP UI by clicking on "Edit:"
