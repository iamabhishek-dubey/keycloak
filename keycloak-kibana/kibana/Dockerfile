FROM docker.elastic.co/kibana/kibana-oss:6.6.1

USER root

COPY ./kibana.yml config/kibana.yml

ADD https://github.com/novomatic-tech/keycloak-kibana/releases/download/2.0.0-alpha1/keycloak-kibana-2.0.0-alpha1_6.6.1.zip .

RUN ./bin/kibana-plugin install file:./keycloak-kibana-2.0.0-alpha1_6.6.1.zip
