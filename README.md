# rapper command
A Docker image for [Raptor](http://librdf.org/raptor/).

Inspired from

## Build
Build the and publish  Docker image:

    docker build -t linkeddatacenter/rapper:latest .
	docker push linkeddatacenter/rapper:latest
	docker tag linkeddatacenter/rapper:latest linkeddatacenter/rapper:x.x.x
    docker push linkeddatacenter/rapper:x.x.x

## Run
Run the Docker container with the same arguments as the [CLI](http://librdf.org/raptor/rapper.html).

Es:

    cat test.rdf | docker run -i --rm linkeddatacenter/rapper -o turtle -O - - urn:test
