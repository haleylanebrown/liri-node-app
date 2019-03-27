# Liri-Node-App

DU Full-Stack Web Development Bootcamp

## Liri

Liri plays off the idea of Siri functionality. It is a node.js command line application that takes in parameters and gives back data. The user must enter 'node liri.js' into the command line followed by a command and then a search parameter.

There are four possible Commands: 'concert-this', 'spotify-this-song', 'movie-this', or 'do-what-it-says'

## 'concert-this'

The 'concert-this' command uses the Bandsintown API to retrive 5 upcoming concerts for an artist/band that is searched. The venue, location and date is provided for each result. Moment.js is used to format the date from the Bandsintown API.

In the following example, the user is looking for the next Billie Eilish Concert: node liri.js concert-this billie eilish

![concert-this](/images/concert-this.gif)

## 'spotify-this-song'

The 'spotify-this-song' command uses the Spotify API to retrieve data about the song entered in the search parameter. The most relevant song title that contains the search parameter or parts of it is returned. The user will receive the artist, song name, a link to preview the song, and the album name.

In this example, the user is looking for the Song "Thriller": node liri.js spotify-this-song thriller

![spotify-this-song](/images/spotify-this-song.gif)

If the user does not enter a search parameter, the 'spotify-this-song' command returns info for the song "The Sign" by Ace of Base.

![spotify-this-song-default](/images/spotify-default.gif)

## 'movie-this'

The 'movie-this' command uses the OMDB API to retreive data about the movie entered in the search parameter. The result will include the title, release year, IMDB rating, Rotten Tomatoes rating, country of production, language, plot, and actors/actresses in the film.

In this example, the user is looking for information about the movie "Elf": node liri.js movie-this elf

![movie-this](/images/movie-this.gif)

If the user does not enter a search parameter, the 'movie-this' command returns info for the movie "Mr. Nobody"

![movie-this-default](/images/movie-default.gif)

## 'do-what-it-says'

The 'do-what-it-says' command reads the random.txt file and executes the parameters inside of it. By default it is set to 'spotify-this-song, I Want It That Way', but this can easily be changed as needed.

![do-what-it-says](/images/do-what-it-says.gif)

## Extra Tidbits

If the user does not enter a valid command, they receive the following message: "Not a valid command. Please try: 'concert-this', 'spotify-this-song', 'movie-this', or 'do-what-it-says'"

![command-message](/images/command-message.gif)

All results are returned in the command line, but also into a separate text file named 'log.txt' as well.

![log-tex](/images/log-text-compressed.gif)

Technologies used: Javascript, Node.js, Moment.js, Bandsintown API, Spotify API, OMDb API