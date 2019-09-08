# WebpackRailsGlue

Welcome to your new gem! In this directory, you'll find the files you need to be able to package up your Ruby library into a gem. Put your Ruby code in the file `lib/webpack_rails_glue`. To experiment with that code, run `bin/console` for an interactive prompt.

TODO: Delete this and the text above, and describe your gem

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'webpack_rails_glue'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install webpack_rails_glue

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

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake spec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/[USERNAME]/webpack_rails_glue. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](http://contributor-covenant.org) code of conduct.

## License

The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).

## Code of Conduct

Everyone interacting in the WebpackRailsGlue project’s codebases, issue trackers, chat rooms and mailing lists is expected to follow the [code of conduct](https://github.com/[USERNAME]/webpack_rails_glue/blob/master/CODE_OF_CONDUCT.md).
