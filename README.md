# WebpackRailsGlue

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'webpack_rails_glue'
```

## Configure

In `app/controllers/application_controller.rb`

```ruby
helper WebpackRailsGlue::Helper
```

In `config/environments/development.rb`

```ruby
config.dev_server_host = '0.0.0.0:3035'
config.middleware.use WebpackRailsGlue::DevServerProxy, ssl_verify_none: true
```

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/[USERNAME]/webpack_rails_glue. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](http://contributor-covenant.org) code of conduct.

## License

The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).

## Code of Conduct

Everyone interacting in the WebpackRailsGlue project’s codebases, issue trackers, chat rooms and mailing lists is expected to follow the [code of conduct](https://github.com/[USERNAME]/webpack_rails_glue/blob/master/CODE_OF_CONDUCT.md).
