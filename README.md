## TwitchBotEx

This is an example project that utilizes the [`twitchbot`](https://github.com/foresthoffman/twitchbot) package. You can read my [walkthrough of `twitchbot`](https://foresthoffman.com/building-a-twitch-tv-chat-bot-with-go-part-1/) and/or grab it with `go get`...

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
