# UFO-Sighting-JS-Challenge-11

Purpose: A UFO enthusiast has compiled a database of UFO sightings around the globe in January of 2010.  This code was written to filter and display the database on a web page built on HTML with CSS elements with a javascript back end that will take user inputted search criteria and update the table in real time.  Users are allowed to search the database on date, city, state, country, and shape of UFO sighted.



Results: 

The database can be searched and filtered based on any combination of the following criteria: date, city, state, country, and shape. Users can enter the values on the left in the filter search section, then press enter.  The table will automatically apply all filters containing an entry.  Clearing the entries in the filter search would reset the search and display the entire database.

Fig 1:
![1](https://user-images.githubusercontent.com/108313294/190218923-904b52c6-0ebf-45cd-8631-6b5b84a2c309.png)

Some users may look at the complete data table ahead of time and see how search filter entries must be entered.  all entries are case sensitive, and state or country must be entered in their 2 letter abbreviations. The following is a summary of the correct search filter formatting.

date: M/DD/YYYY -  Date must be in this format, for dates with single digit days, format M/D/YYYY
City: cityname - City names must be in lower case.  Spaces are allowed. Some cities may have additional data in brackets under this filter.  That must also be entered
State: ny - State must be lowercase 2 letter abbreviation
Country: us - Country must be 2 letter lowercase abbreviation
shape: circle - Shape must be one of: circle, light, triangle, unknown, fireball, formation, other, sphere, disk, cheveron, rectangle, cross, flash, changing, oval, cigar, teardrop, or cylinder.



Summary:
This website is fairly intuitive if the user already knows all the data that is stored in the database.  This design cannot be scaled to big data where the database can get messy.  In order for users to effectively use the filter function, they would need to know every unique element of each column.  This would require a legend.  New users may also type a valid filter incorrectly or in the incorrect format (eg. State: Oregon instead of "or").  

Recommended changes to the code include select dropdown menues instead of manual typing to ensure that all filters are valid filter entries.  

For scalability reasons, instead of displaying the entire database and removing invalid entries based on the filter criteria, it may be better have an empty table that queries and displays the based on the filter results.  This would allow the website to work on any sized database without encountering memory related issues.  A clear all fitlers button, and a button for starting the search may work better with this method instead of live updates to reduce how often the database gets queried. 

      
