# Alerts

<!--- Adapted from ZTAP UI Overview on Confluence -->

The **Alerts** screen is where most of the work in ZTAP is done. The main view lists the currently open alerts, based on any default filtering criteria you have selected.

## Alerts interface
<!---insert new screencap of Alerts interface -->

1. Incident count: The total number of incidents that match the current filter in the search bar (#7) – if the filter is blank then this number will be the total number of incidents for all organizations the current user is a member of.
2. Incident details: This section shows:
   - How many total events are part of a particular incident, what products generated those events, and how many events are classified as triggers, observations, and whitelists
   - The status of the incident (Open, Assigned, Reviewing, Closed)
   - When the incident was created and last updated
3. Organization & Assignment: The organization associated with the incident and the group or user within that organization which has been assigned to the incident
4. Trigger event details: A high-level look at the event that triggered the incident – this information can often give an analyst enough information to make a decision, especially if there is only one event in the incident details
5. Action bar: Allows an analyst to take action on an incident without needing to navigate into the incident itself
   - Close: Closes the incident – the analyst will be prompted to enter a reason manually and whether or not the incident was resolved:

   - Escalate: Escalates an incident to another user / group – this is used to request assistance from senior analysts on undetermined incidents for further review. See section 2.1 for more information
   - Assign to me: Assigns an incident to the current analyst – an incident should be first assigned to the logged-in analyst in order for them to escalate (this maintains audit integrity)

<!--- Remove Search section from individual pages, create individual help page for search -->

7. Search / filter bar: Allows an analyst to quickly search all current incidents based on a filter / set of filters. The search bar supports tab-complete for partially-typed strings. It is worth noting that the search bar canonly be used to search for trigger events - a search will not return matching whitelisted events or observation events. Examples:
  - A user wants to return a list of all open incidents for the "Critical Start" organization for the "bit9endpointvisiblity" feed. Starting to type "organization" in the filter bar will cause suggestions to appear based on what has been typed thus far:

   - Partially-completed terms can be tabbed to and selected by pressing enter:

   - Once a search term is complete, ZTAP will automatically suggest values for the search term based on user permissions. The user in this example is only a member of the "Critical Start" organization, and thus only sees their organization for suggested values: 

   - Tabbing to the value and pressing enter will select it: 

   - Search terms with multiple values will show up as a list – selecting the search term "Feed Name" with no value typed will return all values that currently match any open incidents with events matching the search criteria: 

   - We want to search for "bit9endpointvisibility" for this example, so typing "bit9en" will yield the value we want - note that the search bar will auto-collapse earlier search criteria for readability - mousing over a previous search criteria briefly will expand it:

   Once selected, we will only get the incidents which have events matching the criteria we have selected:

<!--- End search section to relocate -->

6. Incident details page: Will navigate to an incident and show all events in a detailed format. See "working with individual alerts"

<!--- Move to individual alerts section -->
   There are four different tabs per incident with information in each tab:

   - Trigger Events: These are events that caused the incident to be created and are considered to be "high-value" from an investigation perspective. An event with the crosshair symbol (  ) indicates that this was the original event that created the incident and is the "main" event displayed in the ZTAP UI
   - Observations: These are events that do not create an incident, but are instead designed to be helpful events that provide additional context. These types of events have been explicitly filtered by a senior analyst
   - Whitelisted Events: Events that have been explicitly whitelisted via the "Whitelist Trigger", the "Whitelist" button from within an incident, or a matching filter set to recategorize to Tier 3 will go into this section. These events may have been whitelisted from the incident they created, or they were whitelisted from another incident entirely
   - Incident Timeline: This view shows the specific details around events being added to the incident, groups / users being assigned, and other information with regards to the timeline of the incident
   - Comments: This view shows all comments pertaining to this incident with visibility to both analyst and client. It is possible for private comments to be made so the other party can't see them. This is an option to provide advice/opinions so all shifts can be on the same page. 
   - Audit Log: This page shows the historical timeline of actions and who performed them. 

    You can edit the Alert title from this screen or the general ZTAP UI by clicking on "Edit:"

<!--- end move -->

7. TAP (Threat Analysis Plugin) Actions: This section is semi-automates investigation procedures. An analyst can get information such as VirusTotal hits, binary information pulled from the Carbon Black instance, network connections the binary made (if applicable), and child process information (if applicable) for the binary. The icons look like the following: 

<!--- move to search section -->
8. Manage Saved Searches: This gear icon allows for management of saved searches - the ZTAP allows for users to save particular searches for quick reference later. If there is a search term already in the search bar, an option appears to potentially name or save the current search parameters. Users can also delete or load searches from this screen (as well as type the saved search into the search bar). An example is below:
<!--- end move -->

8. Bulk Actions: This feature allows for a user to bulk close or bulk assign incidents to themselves. This will apply to the currently-displayed search in the search bar. Please note that if there is no search designated, bulk actions will apply to all incidents. Closing incidents will show the "Close Incident" dialogue box with an optional message by the current user which will be applied to all incidents affected, and once "Close Incident" is selected it will prompt for confirmation.

<!--- Remove User Menu and document separately, maybe as part of Dashboard -->

12. User Menu: The user menu allows a user to view / change information about their user profile and organization, access support, and log out.
<!--- End User menu section -->

9. See All Comments: This shows the total number of comments an incident contains and allows the user to pivot into the comments window. The most recent comment is usually shown at the bottom of the incident. 

<!--- Remove the last two items and document separately -->

14. Saved Search: This shows the current saved search being used.

15. Notifications: This window will open up notifications that pertain to incidents commented on by the user. A white number in a red box will appear when new notifications are present. 
<!--- End remove -->
