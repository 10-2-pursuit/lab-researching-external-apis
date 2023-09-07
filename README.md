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

> 

Write 3 - 5 user stories for your application. Include each below.

> 1. As a user I am a tourist looking for a specific egyptian exhibit (or exhibits).

> 1. As a user I would like to search for a specific department. 

> 1. As a user I would like to look up art by the artist.

What data is needed to complete your application? Describe the data below and provide a link in the documentation showing where to get this data.

> A list of museum exhibits, a list of muesum departments and a list of Artists currently showing in the building.
  https://metmuseum.github.io/
Determine the number of free requests you can make to the API. Include a link in the documentation showing where you found this limit, if possible.

> 80 Requests per Second 
https://metmuseum.github.io/

Would the number of free requests you can make to the API be sufficient for you to develop a basic version of the application within a week? Why or why not?

> Most definitely 

Does working with the API require the use of a credit card? If possible, include a link in the documentation showing where you found this requirement.

> This API is free to use but has a request rate limit

Write one GET request to your chosen API with Postman. This may involve requesting an API key or other steps. If you requested an API Key, **don't include it.** Instead, replace that part of the URL WITH `<MY API KEY>.`

> https://collectionapi.metmuseum.org/public/collection/v1/objects?departmentIds=1


Include a snippet of the data you received from the above request.

```
{
    "total": 18548,
    "objectIDs": [
        1,
        2,
        3,
        4,
        5,
        6,
        7,
        8,
        9,
        10,]
}
```

> **Note**: If you could not get an API key for any reason (like it required a credit card or took too long for an API key to be delivered), just leave a note here and do your best to answer the questions anyway.

What file do you need to store an API key safely?

We would store the API key in an .env and .env/development file 

Why do you want to place that file within the `.gitignore` file?

>  using version control systems like Git, they keep a history of changes to your code. pushing an API to a git will grant unauthrized access to users that may misuse you API key.
