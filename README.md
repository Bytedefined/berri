# berri

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

*app.cr*
```crystal
require "berri"

Berri::Server.run
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
