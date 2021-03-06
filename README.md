## TwitchBotEx

This is an example project that utilizes the [`bot`](https://github.com/foresthoffman/bot) package. You can read my [walkthrough of `bot`](https://dev.to/foresthoffman/building-a-twitchtv-chat-bot-with-go---part-1-i3k) and/or grab it with `go get`...

```bash
$ go get github.com/foresthoffman/twitchbotex
```

## TL;DR

Add a `private/oauth.json` file next to `main.go`, and put the OAuth token you receive from [Twitch's OAuth Generator](http://twitchapps.com/tmi/) into the `private/oauth.json` file with the key "password".

e.g.

```json
{
	"password": "oauth:secretsecretsecretsecretsecret"
}
```

Then, open `main.go` and replace the `Channel` and `Name` values with your own. `Channel` must be lowercase.

Build and run:

```bash
$ go fmt ./... && go build && ./twitchbotex
```

_That's all, enjoy!_
