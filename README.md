# Image Finder

## Brief
We would like to build a Java application which allows others to find images by a search term

A basic service would have the following functionalities:
- Ability to fetch data from an external image searching API
- Transform and filter the data
- Create an endpoint to allow retrieval of the transformed data

We could plan to extend the service by introducing:
- Add test coverage
- Build a frontend to display the images

For the purpose of this exercise, the external API will be NASA's media searching API

    https://images-api.nasa.gov/search?q=moon

Here is an example of the payload:

```
{
  "collection": {
    "href": "https://images-api.nasa.gov/search?q=moon",
    "version": "1.0",
    "items": [
      {
        "href": "https://images-assets.nasa.gov/image/PIA12235/collection.json",
        "data": [ ... ],
        "links": [
          {
            "href": "https://images-assets.nasa.gov/image/PIA12235/PIA12235~thumb.jpg",
            "render": "image",
            "rel": "preview"
          }
        ]
      }
    ]
  }
}
```

Here is what we expect our service to return:

```
[
  "https://images-assets.nasa.gov/image/PIA12235/PIA12235~thumb.jpg",
  "https://images-assets.nasa.gov/image/PIA13517/PIA13517~thumb.jpg",
  ...
]
```

## Usage
Choose one of these builds and clone the project using the following command:


#### Gradle
    git clone --single-branch -b build/gradle https://github.com/JSainsburyPLC/image-finder.git

#### Maven
    git clone --single-branch -b build/maven https://github.com/JSainsburyPLC/image-finder.git


You are free to code and run the application using any IDE/text editor of your choice. Both builds come with `spring-boot-starter-web` as a dependency, we would prefer you to use Spring but you are definitely free to choose other frameworks/libraries if you see fit.
