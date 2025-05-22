---
title: "Excel - Document management and Dashboard for IVO Rechtspraak"
excerpt: "To streamline the annual review of internal manuals at IVO Rechtspraak, I designed and implemented this worksheet which includes a dynamic dashboard <br/><img src='/images/Kennisitems-Dashboard.png' width='400'>"
paperurl: 'http://wouterbonhof.github.io/files/KennisitemsOverzicht.xlsx'
collection: portfolio
---

## Situation
IVO Rechtspraak (the IT serviceprovider for the judicial system in The Netherlands) is responsible for over 300 different software applications, each with their own unique challenges. Because it is impossible to train IT support to have intimate knowledge of each application, the support team has created a digital library in TOPdesk and filled it with nearly 1.000 manuals known as 'Kennisitems'. A dedicated team is responsible for the maintenance and upkeep of these manuals, but in recent years these responsibilities have largely been replaced by other time-consuming activities, such as creationg new manuals and processing user feedback. This has led to an overabundance of manuals, some of which have become and have not been revisited for several years.
As part of the Contentmanagement team, I took the responsibility to create a new process for the annual revision of all manuals. Besides setting up a new process with a purposeful flowchart, I also wanted to create a document in which all progress can be documented and reported. The available software was limited due to application constraints set by the IT security team and management wanted the software to be userfriendly. The solution thus needed to be 1) userfriendly, 2) allow controlled data input and editing, 3) give detailed information on each manual, and 4) provide an overview of the current status. With these requirements in mind I decided to create an Excel Worksheet. Nearly everyone is familiar with the basic functionalities of Excel or can quickyl learn it, data input can be constrained and Excel has some excellent native visuals.

The document consists of four tabs, each with a seperate purpose:

1 - **Dashboard** The dashboard tab shows aggregated data. In a heartbeat the managers can here see the total number of manuals the Contentmanagement team is responsible for, how many of these are over date, the prospects for the coming weeks and months and the progress that is being made for the manuals that are over date.

2 - **Data** This tab will be used most heavily by the Contentmanagement team. The tab gives detailed informaton on the manual numbers, manual titles, the domain they are part of, when they have last been checked, who is currently responsible for the manual and what the status is of the check-up. This is also the tab where the Contentmanagement team can enter new manuals as they are created.

3 - **Stats** Information from the Data tab is largely also present on the Stats tab. The Stats tab, however, is the source for the visualisations on the Dashboard tab to prevent data issues as the Contentmanagement team adds and removes data on the Data tab. Additionally, the Stats tab includes several derived tables necessary for the time function visualisations on the Dashboard tab.

4 - **References** All tables used as references for the Data validation on the Data tab are present in the References tab.

<br/><img src='/images/Kennisitems-Data.png' width='500'>

## The Data input
TOPdesk, unfortunately, has no option to connect a live feed to Excel. The list with all relevant manuals was therefore exported to Excel, where the data was cleaned. I then set up a few data tables that would be used as references for Data validation (present in the 'References' tab). For columns such as 'Behandelaar' (the person processing the manual) and 'Sectie' (domain), the Data validation ensures that only the options from the drop-down list are entered and thereby prevents user errors. The colum 'Laatst_bekeken' (most recent inspection) was assigned Conditional formatting, visualising when a manual has not been revisited for over one year (365 days), would soon need to be revisited within the next three months or when a manual did not require inspection. The status of the manual was also made clear in calculated column F.

## The Stats tab
The Stats tab is in part a direct copy of the Data tab. This duplication of data is necessary to prevent issues as the members of the Contentmanagement team add and remove manuals from the worksheet; it was found that when rows were added in the middel of the tab, these were excluded from calculations and the visualisations. Using a column containing the numbers 1 to 200 and the INDEX function, data from the Data tab was copied into the Stats tab and enabled the insertion of rows at random locations. 
Aggregation tables were created in the Stats tab to be used in the Dashboard. Additionally, two time function tables were created to give an indication of the workload that is going to come in the coming weeks and months. These tables show the number of manuals set to expired per month for the next 12 months and per week for the next 5 weeks (current week inclusive).

## The Dashboard tab
The Dashboard gives a quick overview of the status of the manuals. The total number of manuals overseen by the Contentmanagement team can be seen here, as well as the percentage of manuals that are over date and other KPI's. A column chart shows the number of manuals that are set to expire this week as well as in the next four weeks, whilst a waterfall chart shows the number of manuals overdate, how many are set to expire each month in the coming 12 months and the total number of manuals. A line chart finally shows how many expired manuals are not yet being processed, the status of those that are being processed and how many have manuals have been fully revised, but need to have a new expiration date set.

<br/><img src='/images/Kennisitems-Dashboard.png' width='500'>

## Reception
During the creation of the Excel worksheet I have met with both management and the members of the Contemtmanagement team to ask for their requirements and feedback on regular iterations. Feedback was overwhelmingly positive during each meeting and the final product was received with great enthousiasm. Management was impressed by the aesethetics and intuitive design of the dashboard, whilst the Contentmanagemnt team were pleased with the eas-of-use of the Data tab and the inclusion of Data validation to prevent inconsistencies. Two supporting manuals accompanied the Worksheet; one with instructions on the new process of annual revision of the TOPdesk manuals and the other with the design details of the worksheet and instructions on how to make adjustments to the Worksheet.
As a result of the newly set-up process and the overview document, the Contentmanagement team felt they had a better grip on the situation and the number of outdated TOPdesk manuals decreased rapidly. Of the approximately 800 manuals, nearly 50 were deemed irrelevant and archived. A further 100 required substantial redactions, which were quickly implemented, leading to a noticable improvent in the service of IT support.

A reproduction of the Excel worksheet (with fictionalised data) can be downloaded on the previous page.
