# description of the structure of the cvs files
each of these files contains the header with the information that updates the site by reading from a table.\
note: the pictures are stored on the path img/gallery/SECTION\
where SECTION is the name of the file .csv without the extension

## organizers.csv
the list of organizer names
```bash
name,position,affiliation,email,twitter,website,picture
```
## program_day1.csv
the schedule of the first day
```bash
schedule,session,title,place,speaker
```
## program_day2.csv
the schedule of the second day
```bash
schedule,session,title,place,speaker
```
## program_day3.csv
the schedule of the third day
```bash
schedule,session,title,place,speaker
```
## scientific_committee.csv
list of people involved in the scientific committee
```bash
name,affiliation,location
```
## speakers.csv
list of the invited speaker
```bash
name,affiliation,website,picture,schedule,title,description
```
## sponsors.csv
list of the sponsor\
pay attention to the category section: platinum, gold, silver, bronze
```bash
 name,url,logo,category
```
