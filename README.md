# Zigrb

Small experiments for integrating in Zig with Ruby via some helpful Rakefile tasks.

## TODO

- [ ] Better zig-build integration

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'zigrb'
```

And then execute:

    $ bundle install

Or install it yourself as:

    $ gem install zigrb

## Usage

Update your `Rakefile` like so:

```ruby
require 'bundler/setup'
require 'zigrb/build_task'

Zigrb::BuildTask.new('hello')

task default: :build
```

See new rake tasks defined for you project:

    rake -vT
    ...
    build

Building the Zig shared library as defined in your Rakefile:

    rake build


## Examples

* [hello](examples/hello/) - Minimal example of project structure

## Development

After checking out the repo, run `bin/setup` to install dependencies. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/[USERNAME]/zigrb. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [code of conduct](https://github.com/[USERNAME]/zigrb/blob/master/CODE_OF_CONDUCT.md).


## License

The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).

## Code of Conduct

Everyone interacting in the Zigrb project's codebases, issue trackers, chat rooms and mailing lists is expected to follow the [code of conduct](https://github.com/[USERNAME]/zigrb/blob/master/CODE_OF_CONDUCT.md).
