FROM registry.access.redhat.com/ubi9/go-toolset:1.23.6-1747059472

COPY . .
RUN go mod download

RUN go build -o ./main

ENV PORT 8081
EXPOSE 8081

CMD [ "./main" ]
