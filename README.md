# Berri
![License](https://img.shields.io/github/license/macawos/berri) ![Crystal Version](https://img.shields.io/badge/Crystal-0.35.1-000) ![Issues](https://img.shields.io/github/issues/macawos/berri) ![Telegram](https://img.shields.io/badge/chat-t.me%2Fmacawos-blue) ![Discord](https://img.shields.io/discord/758767067196817470)

Berri is a framework for writing fast and efficient Linux webapps in Crystal

## Installation

1. Add the dependency to your `shard.yml`:

   ```yaml
   dependencies:
     berri:
       github: macawos/berri
   ```

2. Run `shards install`

## Usage

*./app.cr*
```crystal
require "berri"
require "./app/*"

app = Berri::App.new
app.title = "DeLorean"
app.color = "#111111"
```
*./app/main.cr*
```crystal
require "berri/main"

post "/" do |context|
   song_dir = env.params.body["song_dir"].as(String)
   puts "Now playing: #{song_dir}"
end

Berri::Main.run
```
*./app/client.cr*
```crystal
require "berri/client"

get "/" do |context|
   render "/src/render/index.ecr"
end

Berri::Client.run
```

## Development

TODO: Write development instructions here

## Contributing

1. Fork it (<https://github.com/macawos/berri/fork>)
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request

## Contributors

- [Bo](https://github.com/acoolstraw) - creator and maintainer
- [Tan](https://github.com/yutyo) - creator and maintainer
