# _Wildlife Tracker_

#### _An app for the forest service to track animals for an environmental impact study, July 14, 2017_

#### By _**Mara Timberlake**_

## Description

_The Forest Service is considering a proposal from a timber company to clearcut a nearby forest of Douglas Fir. Before this proposal may be approved, they must complete an environmental impact study. This application was developed to allow Rangers to track wildlife sightings in the area._

## Specifications






## What's included
Within the repository you'll find the following directories and files:

```
java-wildlife-tracker/
├── src/
│    └── main/
│    │    └── java/
|    │    │     └── Animal.java
|    │    │     └── App.java
|    │    │     └── DB.java
|    │    │     └── EndangeredAnimal.java
|    │    │     └── Sighting.java
|    │    │     └── VelocityTemplateEngine.java
|    |    └── resources/
|    |          └──public/
|    |               └──app.css
|    |          └──templates/
|    |               └──animal-form.vtl
|    |               └──animal.vtl
|    |               └──endangered_animals.vtl
|    |               └──error.vtl
|    |               └──index.vtl
|    |               └──layout.vtl
|    |               └──success.vtl
|    └── test/
│         └── java/
|               └── AnimalTest.java
|               └── DatabaseRule.java
|               └── EndangeredAnimalTest.java
|               └── SightingTest.java
├── .gitignore
├── build.gradle
└── README.md
```

## Setup/Installation Requirements
To create the necessary databases:
* _LOCAL: Go to Terminal_
* _Clone this repository:_
```
$ cd ~/Desktop
$ git clone https://github.com/Epicodus-MT/wildlife-tracker.git
$ cd wildlife-tracker
```
* _Run Postgres with terminal command:_
```
$ postgres
```
* _Open a new tab in terminal by pressing [command ⌘] + [T]_
* _In the new tab, create 'sales_tracker' database:_
```
$ psql
* `CREATE DATABASE wildlife_tracker;`
* `\c wildlife_tracker;`
* `CREATE TABLE animals (id serial PRIMARY KEY, name varchar);`
* `CREATE TABLE endangered_animals (id serial PRIMARY KEY, name varchar, health varchar, age varchar);`
* `CREATE TABLE sightings (id serial PRIMARY KEY, animal_id int, location varchar, ranger_name varchar);`
* `CREATE DATABASE wildlife_tracker_test WITH TEMPLATE wildlife_tracker;`
```
* _Return to original tab where repository was cloned and run gradle:_
```
$gradle run
```
* _Open browser window:_
```
localhost:4567
```

## Known Bugs
_No known bugs at this time_

## Support and contact details
_For questions or feedback, please notify Mara Timberlake at maratimberlake@msn.com_

## Technologies Used
_Languages used include Java. IDE used - Atom_

### License
*This software runs under the MIT license*

Copyright (c) 2017 **_MIT License_**
