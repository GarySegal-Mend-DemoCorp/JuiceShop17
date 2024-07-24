FROM alpine

RUN apk add curl

COPY smoke-test.sh smoke-test.sh

# Mend traceability labels
LABEL io.mend.image.dockerfile.path=main/test/smoke/Dockerfile
LABEL org.opencontainers.image.source=https://github.com/GarySegal-Mend-DemoCorp/JuiceShop17

CMD ["sh", "smoke-test.sh", "http://app:3000"]
