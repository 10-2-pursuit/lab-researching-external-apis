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

> Simple translation app using Rapid Translate API.

Write 3 - 5 user stories for your application. Include each below.

> 1. As a user ...i can translate simple phrases.

> 1. As a user ...i can translate a word to multiple languages.

> 1. As a user ...i want to know a language has some words in their dictionaries?

What data is needed to complete your application? Describe the data below and provide a link in the documentation showing where to get this data.

> The data I need for my app is ...A word that translated.
> https://rapidapi.com/sibaridev/api/rapid-translate-multi-traduction

Determine the number of free requests you can make to the API. Include a link in the documentation showing where you found this limit, if possible.

> The number of free requests I can make is...50 per day

Would the number of free requests you can make to the API be sufficient for you to develop a basic version of the application within a week? Why or why not?

> For test purpose, 50 per day is enough. However, if we want to update the app to public, we must purchase more quotas.

Does working with the API require the use of a credit card? If possible, include a link in the documentation showing where you found this requirement.

> It gives 50 free requests per day.
> https://rapidapi.com/sibaridev/api/rapid-translate-multi-traduction/pricing

Write one GET request to your chosen API with Postman. This may involve requesting an API key or other steps. If you requested an API Key, **don't include it.** Instead, replace that part of the URL WITH `<MY API KEY>.`

```
const options = {
  method: 'POST',
  url: 'https://rapid-translate-multi-traduction.p.rapidapi.com/t',
  headers: {
    'content-type': 'application/json',
    'X-RapidAPI-Key': (API key),
    'X-RapidAPI-Host': 'rapid-translate-multi-traduction.p.rapidapi.com'
  },
  data: {
    from: 'en',
    to: 'ar',
    q: 'Hello world'
  }
};
```

Include a snippet of the data you received from the above request.

```
[
    "مرحبا بالعالم"
]
```

> **Note**: If you could not get an API key for any reason (like it required a credit card or took too long for an API key to be delivered), just leave a note here and do your best to answer the questions anyway.

What file do you need to store an API key safely?

> .env or some configuration files.

Why do you want to place that file within the `.gitignore` file?

> Publicly exposing API key can result in the account being compromised, which could lead to unexpected charges.
