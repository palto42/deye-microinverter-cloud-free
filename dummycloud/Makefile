VERSION = $(shell grep -oP '(?<="version": ")[^"]*' package.json)

docker-build:
	@docker buildx build \
		--platform linux/amd64 \
		--output type=docker \
		-t deye-dummycloud:$(VERSION) \
		-t deye-dummycloud:latest \
		.
