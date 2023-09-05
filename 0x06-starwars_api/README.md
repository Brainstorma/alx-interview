# 0x06. Star Wars API

## Description
This project is about using the [Star Wars API](https://github.com/Brainstorma/alx-interview/blob/master/0x06-starwars_api/README.md) to get information about the characters in the Star Wars universe. The API provides a RESTful interface to query various resources, such as people, planets, films, species, vehicles, and starships.

The main objective of this project is to write a script that prints all characters of a Star Wars movie in the same order as they appear in the film. The script takes one argument, which is the episode number of the movie. For example, `./0-starwars_characters.js 3` should print the characters of the movie "Return of the Jedi".

The script uses the request module to make HTTP requests to the API. The script also handles pagination, since the API returns a maximum of 10 results per page.

## Requirements
- Node.js 14.x
- request module

## Tasks To Complete

+ [x] 0. **Star Wars Characters**<br/>[0-starwars_characters.js](0-starwars_characters.js) contains a script that prints all characters of a Star Wars movie with the following requirements:
  + The first positional argument passed is the Movie ID - example: `3` = “Return of the Jedi”.
  + Display one character name per line **in the same order as the “characters” list in the `/films/` endpoint**.
  + You must use the [Star wars API](https://swapi-api.hbtn.io/).
  + You must use the `request` module.

