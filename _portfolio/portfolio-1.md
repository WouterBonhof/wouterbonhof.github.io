---
title: "Power BI Report for WoningNood"
excerpt: "The result of a project for WoningNood, a broker in The Netherlands. <br/><img src='/images/Example-WoningNood.png' width='500'>"
collection: portfolio
projecturl: 'http://academicpages.github.io/files/paper1.pdf'
---

During my Data Traineeship at House of Bèta I worked part-time as a Power BI consultant for the fictional broker WoningNood. Ferdy, an instructor from Data2Benefit, functioned as the contactpoint for WoningNood.

## Situation  
The brokers at WoningNood have informed their managers that the current data system is not sufficient. Every week, the brokers spend at least two hours per person looking for data on the internet for their analyses and visualisations. The board has therefore hired a consultant to investigate the implementation of a Power BI report in which data is extracted through API's. Internal data from WoningNood must be included in the prototype as well, allowing the company to compare themselves against market standards.

## Product
A fully functioning report was produced within the expected time. Included were a homepage, four pages with data and visualisations and a final page listing the sources. Data from the CBS (Centraal Bureau voor Statistic/ Central Bureau for Statistiscs) was connected through API's and subjected to rigorous cleaning. Several new tables had to be made by merging and appending tables and all final tables were connected in a datamodel.  
<p align="center"><img src="/images/Datamodel.png" alt="Datamodel" width="750"></p>

### Homepage and Kerncijfers 2023
The homepage was produced for ease of navigation. Included are five quick links to the other pages of the report.
The first page with data is 'Kerncijfers 2023'. On this page, the 'core numbers' for The Netherlands have been visualised. Six relevant categories were selected for the prototype and through bookmarked pages, the users can switch between each category. Each of the categories included data at the municipal level, but aggregate functions were also used to calculate the numbers at the provincial and national level. For each category, a description was included that becomes visible upon hoover. 
For two categories (Gemiddelde WOZ waarde and Bevolkingsdichtheid), no total or average values were included in the cards, as averages of averages are not appropriate. A little information button was added to the cards in these circumstances to explain this.
Hierarchical filters were added, so that data could be filtered by province and/ or municipality. The map is interactive and automatically zooms in and out.

<img src="/images/Homepage_Page1.gif" alt="Homepage" width="750">

### Page 2
The second page was dedicated to the sales data from WoningNood themselves. Slicers were added to easily switch between data from the different office branches and the types of houses that had been sold. The column graph at the bottom of the page had a drill through function added and an extra page had been created to also show the data on a daily level.

<img src="/images/Page2.gif" alt="Page 2" width="750">

### Page 3 and onwards
Pages 3 and 4 were filled with general information on population and housing market trends over the past decades. Again, data could be filtered by date, province and municipality.
The final page included links to all relevant data sources.

<img src="/images/Page3_onwards.gif" alt="Page 3 and onwards" width="750">

### Reception
The final product was presented to the fictional stakeholders, as represented by the course instructor, fellow course participants and colleages from House of Beta. The report was received very well by all. Observers particularly enjoyed the ease of navigation, consistent theme, well-defined visuals and the many interactive features. 

_With the many details and techniques used, you demonstrate that you not only know very well how Power BI works, but also how to combine all those possibilities into a coherent and usable end product._ - Ferdy Rademaker (course instructor)

### Data sources
The data used in the report had two sources:
 1. Data for WoningNood was created by Ferdy Rademakers for Data2Benefit - https://data2benefit.com/
 2. All other data is publically available at opendata.cbs.nl/statline/#/CBS/nl/
