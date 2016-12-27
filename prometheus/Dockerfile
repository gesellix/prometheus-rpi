FROM hypriot/rpi-alpine-scratch
RUN apk add -U curl tar  && curl -sSL -o /tmp/prom-arm.tgz https://s3-eu-west-1.amazonaws.com/downloads.robustperception.io/prometheus/prometheus-linux-arm-nightly.tar.gz && mkdir /prometheus && tar xfz /tmp/prom-arm.tgz -C /prometheus --strip-components=1
WORKDIR /prometheus
CMD [ "./prometheus" ]

