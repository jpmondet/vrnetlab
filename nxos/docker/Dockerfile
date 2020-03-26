FROM jpmondet/n9k-base:933

ARG IMAGE
COPY $IMAGE* resources/* /

EXPOSE 22 80 443 161/udp 830 5000 10000-10099
HEALTHCHECK CMD ["/healthcheck.py"]
ENTRYPOINT ["/launch.py"]
