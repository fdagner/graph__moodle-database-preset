# Feedback Targeting

Graph is a preset for the Moodle activity database.

## Description

Representations of relationships in a graph.

<img width="400" alt="list view" src="/screenshots/listenansicht.png">
In this example, the students have entered the countries they have visited. The entries must be separated by commas. There is only one database field, so there is only one category. The larger the bubbles, the more frequently the country is mentioned. 

<img width="400" alt="list view" src="/screenshots/listenansicht2.png">
If you click on a country, you can see who has visited it.

<img width="400" alt="list view" src="/screenshots/listenansicht3.png">
Click on a student to see all other students with the same name. You can then view the countries the student has visited and who else has visited them.

## Getting started

Download the [release file](https://github.com/fdagner/graph__moodle-database-preset/releases). 
Create a "Database" activity in Moodle and then upload the ZIP file.

### Steps

1. Create database fields for the categories (short text or dropdown).
2. Reset the current template for adding entries.
3. Customize the list template:

```
{
name: '##user## ##edit## ##delete##',
Länder: '[[state]]',
},
```
<b>Important: The main category must be named 'name'.</b>

```
{
name: '[[nickname]] ##edit## ##delete##',
Länder: '[[state]]',
},
```
You can also do it this way.

## Language Support

The preset is available in German, but there is not so much to translate. The template can easily be adapted.

