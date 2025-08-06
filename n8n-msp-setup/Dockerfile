FROM docker.n8n.io/n8nio/n8n

USER root

# Install python3, curl and some dependencies yt-dlp might need
RUN apk add --no-cache python3 py3-pip curl && \
    curl -L https://github.com/yt-dlp/yt-dlp/releases/latest/download/yt-dlp -o /usr/local/bin/yt-dlp && \
    chmod a+rx /usr/local/bin/yt-dlp

USER node
