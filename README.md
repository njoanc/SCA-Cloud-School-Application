# Adonis fullstack application

This is the fullstack boilerplate for AdonisJs, it comes pre-configured with.

1. Bodyparser
2. Session
3. Authentication
4. Web security middleware
5. CORS
6. Edge template engine
7. Lucid ORM
8. Migrations and seeds

## Setup

Use the adonis command to install the blueprint

```bash
adonis new yardstick
```

or manually clone the repo and then run `npm install`.


### Migrations

Run the following command to run startup migrations.

```js
adonis migration:run
```
## Pushing and Pulling to and from Docker Hub
1. Getting an image from Docker Hub
- docker run --rm -p 8787:8787 rocker/verse
- docker pull rocker/verse
* Log in on https://hub.docker.com/
* Click on Create Repository.
* Choose a name (e.g. verse_gapminder) and a description for your repository and click Create.
* Log into the Docker Hub from the command line
docker login --username=yourhubusername --email=youremail@company.com
* Check the image ID using:
docker images
* and tag your image:
docker tag bb38976d03cf yourhubusername/verse_gapminder:firsttry
* Push your image to the repository you created
docker push yourhubusername/verse_gapminder

2. Saving and loading images
docker save verse_gapminder > verse_gapminder.tar
