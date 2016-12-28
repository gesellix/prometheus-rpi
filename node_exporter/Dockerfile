FROM hypriot/rpi-alpine-scratch
RUN apk add -U curl libc6-compat tar && curl -sSL -o /tmp/node_exporter-arm.tgz https://github.com/prometheus/node_exporter/releases/download/v0.13.0/node_exporter-0.13.0.linux-armv7.tar.gz && mkdir /node_exporter && tar xfz /tmp/node_exporter-arm.tgz -C /node_exporter --strip-components=1
WORKDIR /node_exporter
CMD [ "./node_exporter" ]

