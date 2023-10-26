# Create an image
```bash
docker build -t <image-name> .
```
- -t: tag the image

# Run the container
```bash
docker run -d -p 5000:5000 -w /app -v "$(pwd):/app" <image-name>
```
- -d: run in background
- -p: port mapping
- -w: working directory
- -v: volume mapping

The api is now available at http://0.0.0.0:5000
