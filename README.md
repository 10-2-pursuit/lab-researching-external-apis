# Researching External APIs Lab

## Getting Started

1. Fork and clone this repository.

1. Answer the questions below by editing this readme. Leave the questions and prompts, and answer in between them. Take the time to read back the work, and edit what you've written so that your answers are clear and anyone reading it can easily understand what you've written.

1. When it is applicable, please add screenshots, photos, and links.

## Instructions

You will be planning a new application to develop that uses a third-party API. The app should be a simple idea, as the goal is to research and determine if an API is appropriate for your API.

Choose one of the following categories and APIs:

- Music: [Spotify API](https://developer.spotify.com/documentation/web-api)
- Movies: [OMDB API](https://www.omdbapi.com)
- Text Translator: [Rapid Translate](https://rapidapi.com/auth/sign-up?referral=/sibaridev/api/rapid-translate-multi-traduction)
- Sports: [Sports Score](https://rapidapi.com/tipsters/api/sportscore1)
- City Info: [311 Call Aggregator](https://data.cityofnewyork.us/browse?Dataset-Information_Agency=311)
- Art : [Metropolitan Museum of Art ](https://metmuseum.github.io)

Next, describe your application idea. Your application idea should be simple and make use of the data received by the API. It can make use of other data if necessary.

> Your application idea.
Our Application idea is to use the OMDB Api to develop a basic app that allows us to sell posters of movies to people that want to buy them. (Helps current poster store stay in business without paying rent for a store!)

Write 3 - 5 user stories for your application. Include each below.

> 1. As a user ...
we will be able to access a homepage that displays images of various movies 

> 1. As a user ...
we will be able to navigate to a page that displays details regarding the selected movie/image

> 1. As a user ...
we will be able to view and buy a poster of that movie aftyer clicking a particular movie

What data is needed to complete your application? Describe the data below and provide a link in the documentation showing where to get this data.


> The data I need for my app is
We need movie titles, image of posters, and brief description of the movie

Determine the number of free requests you can make to the API. Include a link in the documentation showing where you found this limit, if possible.

> The number of free requests I can make is...
1000

Would the number of free requests you can make to the API be sufficient for you to develop a basic version of the application within a week? Why or why not?

> Your explanation here.
We believe the 1000 free requests provided by the ombdapi would be sufficient for us to develop a basic version of our app within a week. Because it gives us the data we need as long as we provide the URL with the right parameters.

Does working with the API require the use of a credit card? If possible, include a link in the documentation showing where you found this requirement.

> A credit card is...
not required for use of the ombdapi. Please naviagte to the bottom of the page using the following link to see the following "FREE KEYS! The "open" API is finally open again!"  https://www.omdbapi.com/

Write one GET request to your chosen API with Postman. This may involve requesting an API key or other steps. If you requested an API Key, **don't include it.** Instead, replace that part of the URL WITH `<MY API KEY>.`

> Requested URL

Include a snippet of the data you received from the above request.

```
{
    "Search": [
        {
            "Title": "Game of Thrones",
            "Year": "2011–2019",
            "imdbID": "tt0944947",
            "Type": "series",
            "Poster": "https://m.media-amazon.com/images/M/MV5BN2IzYzBiOTQtNGZmMi00NDI5LTgxMzMtN2EzZjA1NjhlOGMxXkEyXkFqcGdeQXVyNjAwNDUxODI@._V1_SX300.jpg"
        },
        {
            "Title": "The Imitation Game",
            "Year": "2014",
            "imdbID": "tt2084970",
            "Type": "movie",
            "Poster": "https://m.media-amazon.com/images/M/MV5BNjI3NjY1Mjg3MV5BMl5BanBnXkFtZTgwMzk5MDQ3MjE@._V1_SX300.jpg"
        },
        {
            "Title": "Squid Game",
            "Year": "2021–",
            "imdbID": "tt10919420",
            "Type": "series",
            "Poster": "https://m.media-amazon.com/images/M/MV5BYWE3MDVkN2EtNjQ5MS00ZDQ4LTliNzYtMjc2YWMzMDEwMTA3XkEyXkFqcGdeQXVyMTEzMTI1Mjk3._V1_SX300.jpg"
        },
        {
            "Title": "Sherlock Holmes: A Game of Shadows",
            "Year": "2011",
            "imdbID": "tt1515091",
            "Type": "movie",
            "Poster": "https://m.media-amazon.com/images/M/MV5BMTQwMzQ5Njk1MF5BMl5BanBnXkFtZTcwNjIxNzIxNw@@._V1_SX300.jpg"
        },
        
    ],
```

> **Note**: If you could not get an API key for any reason (like it required a credit card or took too long for an API key to be delivered), just leave a note here and do your best to answer the questions anyway.

What file do you need to store an API key safely?


> The filename is typically ...
.env and .env.development files

Why do you want to place that file within the `.gitignore` file?

> Your answer here...
we don't want the files that store our API key to ever reach github. Hence the gitignore.
