# API Project: URL Shortener Microservice for freeCodeCamp
[You can check the app by clicking here](https://cooked-kindhearted-seeder.glitch.me)

#### Usage:
If the user inserts for example "https://www.freecodecamp.org" this will generate a number.

[this_project_url]/api/shorturl/[generated_number]

#### Will redirect to:

https://www.freecodecamp.org


### User Stories

1. I can POST a URL to `[project_url]/api/shorturl/new` and I will receive a shortened URL in the JSON response. Example : `{"original_url":"www.google.com","short_url":1}`
2. If I pass an invalid URL that doesn't follow the valid `http(s)://www.example.com(/more/routes)` format, the JSON response will contain an error like `{"error":"invalid URL"}`. *HINT*: to be sure that the submitted url points to a valid site you can use the function `dns.lookup(host, cb)` from the `dns` core module.
3. When I visit the shortened URL, it will redirect me to my original link.
