FROM hypriot/rpi-alpine-scratch
RUN apk add -U curl tar && curl -sSL -o /tmp/prom-arm.tgz https://github.com/prometheus/prometheus/releases/download/v1.5.2/prometheus-1.5.2.linux-armv7.tar.gz && mkdir /prometheus && tar xfz /tmp/prom-arm.tgz -C /prometheus --strip-components=1
WORKDIR /prometheus
CMD [ "./prometheus" ]

