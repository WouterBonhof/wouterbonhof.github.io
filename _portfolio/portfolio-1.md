---
title: "Power BI Dashboard for WoningNood"
excerpt: "The result of a project for the WoningNood, a broker in The Netherlands. <br/><img src="/images/Example-WoningNood.png">"
collection: portfolio
---

During my Data Traineeship at House of Bèta I worked part-time as a Power BI consultant for the fictional broker WoningNood. Ferdy, an instructor from Data2Benefit, functioned as the contactpoint for WoningNood.
## Situation  
The brokers at WoningNood have informed their managers that the current data system is not sufficient. Every week, the brokers spend at least two hours per person looking for data on the internet for their analyses and visualisations. The board has therefore hired a consultant to investigate the implementation of a Power BI dashboard in which data is extracted through API's. Internal data from WoningNood must be included in the prototype as well, allowing the company to compare themselves against market standards.

## Product
A fully functioning dashboard was produced within the expected time. Included were a homepage, four pages with data and visualisations and a final page listing the sources. Data from the CBS (Centraal Bureau voor Statistic/ Central Bureau for Statistiscs) was connected through API's and subjected to rigorous cleaning. Several new tables had to be made by merging and appending tables and all final tables were connected in a datamodel.  
<p align="center"><img src="/images/Datamodel.png" alt="Datamodel" width="750"></p>

### Home page and Kerncijfers 2023
The homepage was produced for ease of navigation. Included are five quick links to the other pages of the report.
The first page with data is 'Kerncijfers 2023'. On this page, the most 'core numbers' for The Netherlands are processed. Six relevant categories have been selected for the prototype. These are 'Aantal inwoners/ Number of inhabitants', 'Woningvoorraad/ Availability of houses', 'Gemiddelde WOZ waarde/ Average estimated house worth', 'Bevolkingsdichtheid/ Population density', 'Oppervlakte/ Surface', and 'Aantal huishoudens/ Number of families'. Each of these categories included data at the municipal level, but aggregate functions were also used to calculate these numbers at the provincial and national level. For each category, a description was included that describes the contents of the data and how the numbers were calculated. For two categories (Gemiddelde WOZ waarde and Bevolkingsdichtheid), no total or average values were included in the cards at the top of the page, as averages of averages are not appropriate. This explanation was included through the information buttons at the top-right corners of the cards.
Hierarchical filters were added, so that data could be filtered by province and/ or municipality. The map is interactive and automatically zooms in and out.

<img src="/images/Page2.gif" alt="Datamodel" width="750">
