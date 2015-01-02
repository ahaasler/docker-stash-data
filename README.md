# docker-stash-data

Builds a data-only container ready to be used with [docker-stash](https://github.com/ahaasler/docker-stash "docker-stash repo").

## Usage

1. Create and name the data-only container:

	```bash
docker run --name stash-data ahaasler/stash-data
	```

2. Use it in the stash container:

	```bash
docker run --name stash --volumes-from stash-data -d -p 7990:7990 -p 7999:7999 ahaasler/stash
	```

> See [docker-stash](https://github.com/ahaasler/docker-stash "docker-stash repo") for more information on the stash container.

## Thanks

* [Docker](https://www.docker.com/ "Docker") for this amazing container engine.
* [Atlassian](https://www.atlassian.com/ "Atlassian") for making great products. Also for their work on [atlassian-docker](https://bitbucket.org/atlassianlabs/atlassian-docker "atlassian-docker repo") which inspired this.
* [Azul Systems](http://www.azulsystems.com/ "Azul Systems") for their *OpenJDK* docker base image.
* And specially to you and the entire community.

## License

This image is licensed under the Apache License, Version 2.0. See [LICENSE](LICENSE) for the full license text.
