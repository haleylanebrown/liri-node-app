# Liri-Node-App
======================

DU Full-Stack Web Development Bootcamp

## Liri
======================

Liri plays off the idea of Siri functionality. It is a node.js command line application that takes in parameters and gives back data. The user must enter 'node liri.js' into the command line followed by a command and then a search parameter.

There are four possible Commands: 'concert-this', 'spotify-this-song', 'movie-this', or 'do-what-it-says'

## 'concert-this'
======================
The 'concert-this' command uses the Bandsintown API to retrive 5 upcoming concerts for an artist/band that is searched. The venue, location and date is provided for each result. Moment.js is used to format the date from the Bandsintown API.

In the following example the user is looking for the next Billie Eilish Concert: node liri.js concert-this Billie Eilish

![concert-this](/images/concert-this.gif)