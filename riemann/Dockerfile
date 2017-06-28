FROM java:8

ENV RIEMANN_VERSION 0.2.13

RUN wget https://github.com/riemann/riemann/releases/download/${RIEMANN_VERSION}/riemann-${RIEMANN_VERSION}.tar.bz2
RUN tar xvfj riemann-${RIEMANN_VERSION}.tar.bz2

RUN mkdir -p /etc/riemann/conf.d

COPY riemann.config /etc/riemann/

CMD /riemann-${RIEMANN_VERSION}/bin/riemann  /etc/riemann/riemann.config

EXPOSE 5555 5556

#CMD ["start"]
#ENTRYPOINT ["/usr/bin/riemann"]
