ARG TEKU_VERSION
FROM consensys/teku:${TEKU_VERSION}

USER root 

ENV JAVA_OPTS="-Xmx5g"

COPY /security/validator-api-bearer /opt/teku/data/validator/key-manager/validator-api-bearer 
COPY /security/cert /cert
COPY entrypoint.sh /usr/bin/entrypoint.sh

ENTRYPOINT  ["entrypoint.sh"]