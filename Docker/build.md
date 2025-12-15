
### Dockerfile

* Dockerfile (instructions set that starts the application) -> Image -> Container

```dockerfile
FROM (base image)
RUN (commands to configure OS)
COPY (copy files from local dir to container image)
ENV (inject environment variable on image)
CMD (commands to execute when uses docker run)
```

* **docker build Dockerfile**: builds the image
* Generally, this process is automated on CI pipeline

### Cache
