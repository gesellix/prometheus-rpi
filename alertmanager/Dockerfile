FROM hypriot/rpi-alpine-scratch
RUN apk add -U curl tar && curl -sSL -o /tmp/alertmgr-arm.tgz https://github.com/prometheus/alertmanager/releases/download/v0.5.1/alertmanager-0.5.1.linux-armv7.tar.gz && mkdir /alertmanager && tar xfz /tmp/alertmgr-arm.tgz -C /alertmanager --strip-components=1
WORKDIR /alertmanager
CMD [ "./alertmanager" ]

