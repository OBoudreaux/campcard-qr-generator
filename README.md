# QR Code Generator for the Meclenburg County Council Camp Card Sale

Generates QR codes to the online sales page with scout name and unit fields of the form prefilled.

Entirely based on the [work](https://github.com/bizzycola/qrcode-generator) of [bizzycola](https://github.com/bizzycola)


# QR Code Generator UI
[![Docker](https://img.shields.io/badge/Docker-Hub-blue)](https://hub.docker.com/r/bizzycolah/qrcode-generator)

Basic docker container with a HTML/CSS/JS UI to generate a QR Code from a provided URL.
Uses tailwind CSS and qrcode.js


Usage:
```
docker build -t webserver .
docker run -it --rm -d -p 8080:80 --name web webserver
```

I've also included a Docker Compose file so if you've got Docker Compose, you may also use these commands:
```bash
# Run in current shell
docker-compose up

# Run as a background process
docker-compose up -d

# Stop background process
docker-compose down
```

Libraries:

QRCode-SVG: https://github.com/papnkukn/qrcode-svg

TailwindCSS: https://github.com/tailwindlabs/tailwindcss

CanvG: https://github.com/canvg/canvg

