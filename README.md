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

> The application would be for watching movies, whenever a movie is searched and the API has that title then it shows up. On page render a few movies should load randomly just to give a few random choices.

Write 3 - 5 user stories for your application. Include each below.

> 1. As a user I should be able to search for a movie of my choice.

> 1. As a user I should be able to leave a comment about the movie and my thoughts on it.

> 1. As a user I should be able to see the description of the movie (genre, director, actors)

What data is needed to complete your application? Describe the data below and provide a link in the documentation showing where to get this data.

> The data I need for my app is the movie titles, I would also need a comment section so users can leave comments on the movie they watched. I would also need the details of those movies such as the genre, directors, actors so it can be dispayed in the decription.

Determine the number of free requests you can make to the API. Include a link in the documentation showing where you found this limit, if possible.

> The number of free requests I can make is [1,000](https://www.omdbapi.com/apikey.aspx)

Would the number of free requests you can make to the API be sufficient for you to develop a basic version of the application within a week? Why or why not?

> The number of free requests I can make to teh API would be sufficient for the development process of a basic version of the application since the limit is 1,000 and I would only display about 4 during development.

Does working with the API require the use of a credit card? If possible, include a link in the documentation showing where you found this requirement.

> A credit card is not needed to use this API, but in order to get a specific [feature](http://www.omdbapi.com/) which is the poster of the movie then you would need to pay.

Write one GET request to your chosen API with Postman. This may involve requesting an API key or other steps. If you requested an API Key, **don't include it.** Instead, replace that part of the URL WITH `<MY API KEY>.`

> Requested URL

Include a snippet of the data you received from the above request.

```
http://www.omdbapi.com/?i=tt3896198&apikey=<MY API KEY>
```

> **Note**: If you could not get an API key for any reason (like it required a credit card or took too long for an API key to be delivered), just leave a note here and do your best to answer the questions anyway.

What file do you need to store an API key safely?

> The filename is typically .env and/or .env-development 

Why do you want to place that file within the `.gitignore` file?

> So that it hides the file when its pushed because if it is not hidden the key can be stolen and used by someone else.
