# Image Finder
This repository contains a barebone project that is used as a Java coding interview exercise for the Together With team.


## Brief
You are required to build a server side application, it should expose an endpoint that allows other to find images by a search term. Internally It should query an external image searching API, transform the response(whatever it maybe be), and return **at least** a collection of image URLs as the result.

For the purpose of this exercise, the external API will be NASA's media searching API, here is an example of the API call:

> `https://images-api.nasa.gov/search?q=moon`

Feel free to explore this API via your browser or Postman(or other equivalent tools). You are allow to use Google or Stack Overflow during the exercise, if you need to.


## Usage

#### Gradle build
`git clone --single-branch -b build/gradle https://github.com/jayfeng-sainy/image-finder.git`

#### Maven build
`git clone --single-branch -b build/maven https://github.com/jayfeng-sainy/image-finder.git`


Both builds come with `spring-boot-starter-web` as a dependency, we would prefer you to use spring but you are definitely free to choose other frameworks/libraries if you see fit.


## Assessment
We will be assessing you on these aspects: 
1. Code structure
2. API design
3. Production readiness
4. Functionality
5. Thought process
