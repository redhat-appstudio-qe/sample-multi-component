FROM registry.access.redhat.com/ubi9/go-toolset:1.24.4-1752083840

COPY . .
RUN go mod download

RUN go build -o ./main

ENV PORT 8081
EXPOSE 8081

CMD [ "./main" ]
