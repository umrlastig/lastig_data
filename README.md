# lastig_data
a repository to store data that can be edited by any member of the organization (people, news, job offers).


## How to add offers in recruiting.csv (if category exist, otherwise modify js/recruiting.js)
The recruiting.csv file contains the job offered by the lab (PhD, Post-docs, internships) and the content of the file is used to generate html tables in the pages of the lab website. To work properly, here is how the file should be filled:

For an "EC" offer:
> EC;title;link;team;false

For an internship offer:
> Internship;Geolocalization of photographs using a database of georeferenced images;Geolocalization of photographs using a database of georeferenced images;http://recherche.ign.fr/labos/matis/pdf/stages/2019/sujet_stage_Loc_ALEGORIA-2019.pdf; ACTE;false

For a PhD offer:
> PhD;Généralisation cartographique multi-échelles par apprentissage profond;Multi-scale cartographic generalisation with deep learning techniques;https://raw.githubusercontent.com/umrlastig/lastig_data/master/pdf/sujet-these-2019_touya.pdf; GEOVIS;true

For a Post-doc offer:
> postdoc,titre,title,url_fr,url_en,MEIG,false

## How to add news in news.csv
The news.csv file contains nesw related to Lastig and the content of the file is used to generate html tables in the pages of the lab and team websites. To work properly, here is how the file should be filled:

Insert a new line at the proper place in the file (you are responsible for keeping the news sorted from newest to oldest)
Fill in the following fields: date,team,only,perso,texten,textfr
date: the date or time span of the news
team: the team to which the news is connected (ACTE, MEIG, STRUDEL, GEOVIS). For LASTIG wide news, type LASTIG.
only: type "only" if the news should only appear on the team webpage but not Lastig webpage (accepted paper, participation to a conference,...) Leave this field empty for more important news that should appear on the Lastig webpage (arrivals, Phd defenses, events organized, distinctions,...).
perso: If you want the news to appear on a personal webpage, you can put a person name here. The personal page must have a news.js inspired by /bruno-vallet/js/news.js in order for the news to appear. 
texten: the message of the news in english. May have hyperlinks with the <a href=""https://www.example.ref.org""> Example text </a> syntax
textfr: the message of the news in french
