IMAGE := ml-notebook
CONTAINER := ml-notebook

build:
	docker build -t $(IMAGE) .

run:
	docker run --rm -it \
		-p 8888:8888 \
		-v $(PWD):/workspace \
		--name $(CONTAINER) \
		$(IMAGE)

exec:
	docker exec -it $(CONTAINER) bash

rm:
	docker rm -f $(CONTAINER)

rmi:
	docker rmi -f $(IMAGE)