## Lab: Data collection policy

#### Data collection policy & Viewing instrumentation statistics

Why does Jira collect usage data?

We're proud that Jira is one of the most advanced and configurable issue trackers on the planet and we will continue to deliver innovative new features as quickly as we can. In order to prioritize the features we deliver, we need to understand how our customers use Jira, what's important, what's not, and what doesn't work well. The collection of usage data allows us to measure the user experience across many thousands of users and deliver features that matter.

What data is collected?
The type of data we collect is covered in our Privacy Policy. Please read it, as we've tried to avoid legal jargon and make it as straightforward as possible.

To view a sample of data that might be collected from your specific installation:

Log in as a user with the Jira Administratorsglobal permission.
Choose Administration () > System > Advanced > Analytics.
Select the Sample Data link.
How is data collected from Data Center installations?
Analytics are collected using the Atlassian Analytics app. The app collects analytics events in a log file which is located in the Jira home directory under the analytics-logs sub directory. The logs are periodically uploaded using an encrypted session and then deleted. If the Jira installation is unable to connect to the Internet, no logs are ever uploaded. 

Enabling/disabling data collection in Jira Data Center
You can switch off analytics collection at any time: 

Log in as a user with the Jira Administrators global permission.
Choose Administration () > System > Advanced > Analytics.
Select Disabled, and Save your change.


## Viewing Jira application instrumentation statistics

Jira provides an Instrumentation page, which displays a variety of statistics on a wide range of internal properties within Jira that have been 'instrumented' (i.e. recorded) for presentation through Jira's administration area.

This page is mostly useful to help Atlassian Support provide assistance with your support queries, especially if they ask you to quote the statistics of one or more properties listed on this page.

Note: For all of the following procedures, you must be logged in as a user with the Jira Administrators global permission.

From the top navigation bar select **Administration** > **System**. 
Select System support > Instrumentation to display the Instrumentation page.
Instrumentation page.
Last modified on Jun 23, 2020