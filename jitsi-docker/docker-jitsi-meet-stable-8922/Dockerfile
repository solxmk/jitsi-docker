# Use the stable version of the Jitsi web image
FROM jitsi/web:stable-8922

# Copy images for rebranding
#docker cp docker-jitsi-meet-stable-8922-web-1:/usr/share/jitsi-meet/images ./theme/
COPY ./theme/images /usr/share/jitsi-meet/images

# Copy CSS variables for styling
#  docker cp docker-jitsi-meet-stable-8922-web-1:/usr/share/jitsi-meet/css/ ./theme/

COPY ./theme/css /usr/share/jitsi-meet/css

# Copy language files for localization
# docker cp docker-jitsi-meet-stable-8922-web-1:/usr/share/jitsi-meet/lang/ ./theme/
COPY ./theme/lang /usr/share/jitsi-meet/lang

# Copy custom favicon
COPY ./theme/images/favicon.ico /usr/share/jitsi-meet/static/favicon.ico

# Copy custom watermark
COPY ./theme/images/watermark.svg /usr/share/jitsi-meet/images/watermark.svg

# Copy custom sounds
# docker cp docker-jitsi-meet-stable-8922-web-1:/usr/share/jitsi-meet/sounds ./theme/
COPY ./theme/sounds /usr/share/jitsi-meet/sounds

# Copy custom fonts
# docker cp docker-jitsi-meet-stable-8922-web-1:/usr/share/jitsi-meet/fonts ./theme/
COPY ./theme/fonts /usr/share/jitsi-meet/fonts

# docker build -t alkaloid-jitsi-stable-8922 . && docker compose down && docker compose up -d
