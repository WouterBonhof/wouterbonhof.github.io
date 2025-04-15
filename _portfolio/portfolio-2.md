---
title: "Datamodel for Grafzerken Nederland"
excerpt: "A detailed datamodel created for the non-profit organisation 'Grafzerken Nederland'<br/><img src='/images/LDM_GN.png' width='500'>"
collection: portfolio
paperurl: 'http://wouterbonhof.github.io/files/datamodeleren2025.pdf'
---

# _Page still under construction_

During my Data Traineeship at House of Bèta I took part in the course 'Datamodelleren' by Jan Meeuwsen. 
A key component of the course was the design of a complete datamodel. We were free to pick any topic and I decided to design a datamodel for a fictional non-profit organisation 'Grafzerken Nederland'. 
The resulting model was well received by the instructor and was graded an 8,4 out of 10.

## Situation
Grafzerken Nederland is an finctional, non-profit organization in The Netherlands set up in collaboration with commercial archaeological companies and universities. The goal of Grafzerken Nederland is to document all gravestones that can be found in Dutch churches. The organization wants to be able to analyze this information for research, but it must also be accessible to interested parties from the public sector (for example citizens, researchers and travel guides). The initial focus of the organization is on the gravestones that are located inside churches, but in the long term it should also be possible to add gravestones that are located outside the church to the database.
Before the database is set-up, Grafzerken Nederland has commisioned House of Beta to design a detailed datamodel with full documentation on the design choices.

_Problem statement_
Historic churches in the Netherlands are filled with gravestones. These burials mainly contain the remains of wealthy and influential people. Because the gravestones sometimes completely cover the floor of a church, most gravestones are not protected and are tread on daily. As a result, the information that can be found on the gravestones, such as the names of the buried and their dates of birth and death, is lost. It was therefore decided to set up a database in which the gravestones and the information engraved on them are documented. This information concerns, amongst others, the buried persons and relationships between persons, information about the physical aspect of the gravestone, such as the type of stone and position (lying down or standing).
As part of various projects, relevant information has already been collected for a large part of the Dutch gravestones. These projects were carried out for clients, such as the administrators of the churches (religious communities and the Cultural Heritage Agency of the Netherlands (RCE)), but sometimes also for the companies hired for renovation work, for example. Many scientific articles have been published as a result of these projects, but also as part of research projects by students and researchers.
The database with all the information must be made available to the public. Users from the public can view information about the gravestones via the website and app that are still to be developed. The public also has the opportunity to document gravestones if they are not yet included in the database. By means of this citizen science, GN hopes to have all the gravestones documented at a faster pace. The gravestone information entered by citizens must then be validated by an internal researcher from Grafzerken Nederland or an external affiliated researcher.

## Product
Following from the Problem statement, several use-cases were written out. From these use-cases entities and their attributes were derived, which were in turn used to design a Conceptual Datamodel (CDM) and a Logical Datamodel (LDM). All data was first documented in the 0 normal form and then in gradual steps processed to the 3rd normal form. On top of that, the 1st and 2nd Meeuwsen normal forms were used. The 1st Meeuwsen nf applies generalisation to the entitites. An example of this is the combination of the entities 'User', 'Researcher', and 'Burried person' into a single entity called 'Person'. These originally seperate entities were so-called 'specialised' entities, but by merging these into a single generalised entity, duplicate storage is avoided. Using the dedicated 'Person type' entity, the 'Person' entities can then be differentiated into users, researchers and burried people and even represent multiple types wihtout the need to store personal details in duplicate.
The 2nd Meeuwsen nf implements a mutation history for all relevant entities, which allows an easy recovery of data in case of unwanted changes.


### Design choices
