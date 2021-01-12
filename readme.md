# noembed

> perl backed consistent oEmbed like provider [https://noembed.com/](https://noembed.com/)

## Development

```sh
$ docker build -t noembed .
```

```sh
$ docker run --name=noembed -it --rm -p 8080:8080 -v $(pwd)/lib:/usr/src/myapp/lib noembed
```

Service should now be available at [http://localhost:8080](http://localhost:8080).
