FROM --platform=$BUILDPLATFORM caddy:2.11.7-builder AS builder
ARG TARGETOS TARGETARCH
RUN GOOS=$TARGETOS GOARCH=$TARGETARCH xcaddy build \
    --with github.com/jonaharagon/caddy-umami

FROM caddy:2.11.7
COPY --from=builder /usr/bin/caddy /usr/bin/caddy
