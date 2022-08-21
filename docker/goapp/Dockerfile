FROM golang:1.19.0-alpine

RUN apk update && apk add git
RUN go install github.com/cosmtrek/air@latest

WORKDIR /go/src


# air -c [tomlファイル名] // 設定ファイルを指定してair実行(WORKDIRに.air.tomlを配置しておくこと)
CMD ["air", "-c", ".air.toml"]

# CMD ["go", "run", "server.go"]