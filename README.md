# gowiki
This is an implementation of gowiki from https://golang.org/doc/articles/wiki/ to learn some go.

## Build and run in docker 
Build and start the app, the volume wiki_data is used to save wiki pages.

```sh
docker build -t gowiki .
docker run -d -p 8080:8080 --mount source=wiki_data,target=/root/wiki_data gowiki
```
