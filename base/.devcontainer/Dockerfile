ARG VARIANT="jammy"
FROM buildpack-deps:${VARIANT}-curl
ARG VARIANT
RUN if [ "${VARIANT}" = "noble" ]; then userdel -fr ubuntu; fi
