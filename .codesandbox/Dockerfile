FROM node:18-bullseye

# Vite wants to open the browser using `open`, so we
# need to install those utils.
RUN apt update -y && apt install -y xdg-utils \
&& apt clean

RUN addgroup -S nonroot \
    && adduser -S nonroot -G nonroot

USER nonroot
