# Liri-Node-App

DU Full-Stack Web Development Bootcamp

## Liri

Liri plays off the idea of Siri functionality. It is a node.js command line application that takes in parameters and gives back data. The user must enter 'node liri.js' into the command line followed by a command and then a search parameter.

There are four possible Commands: 'concert-this', 'spotify-this-song', 'movie-this', or 'do-what-it-says'

## 'concert-this'

The 'concert-this' command uses the Bandsintown API to retrive 5 upcoming concerts for an artist/band that is searched. The venue, location and date is provided for each result. Moment.js is used to format the date from the Bandsintown API.

In the following example the user is looking for the next Billie Eilish Concert: node liri.js concert-this billie eilish

![concert-this](/images/concert-this.gif)

## 'spotify-this-song'

The 'spotify-this-song' command uses the Spotify API to retrieve data about the song entered in the search parameter. The most relevant song title that contains the search parameter or parts of it is returned. The user will receive the artist, song name, a link to preview the song, and the album name.

In this example the user is looking for the Song "Thriller" node liri.js spotify-this-song thriller

![spotify-this-song](/images/spotify-this-song.gif)

If the user does not enter a search parameter, the 'spotify-this-song' command returns info for the song "The Sign" by Ace of Base.

![spotify-this-song-default](/images/spotify-default.gif)

## 'movie-this'

The 'movie-this' command uses the OMDb API to retreive data about the movie entered in the search parameter. The result will include the title, release year, IMDb rating, Rotten Tomatoes rating, country of production, langauge, plot, and actors/actresses in the film.

In this example the user is looking for information about the movie "Elf" node liri.js movie-this elf

![movie-this](/images/movie-this.gif)

If the user does not enter a search parameter, the 'movie-this' command returns info for the movie "Mr. Nobody"

![movie-this-default](/images/movie-default.gif)