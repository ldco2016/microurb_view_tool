# MicrourbViewTool

> Various view specific methods for applications.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'microurb_view_tool'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install microurb_view_tool

## Usage

```ruby
class ApplicationController < ActionController::Base
  protect_from_forgery with: :exception

  before_action :set_copyright

  def set_copyright
    @copyright = MicrourbViewTool::Renderer.copyright '[Your Name]', 'All rights reserved'
  end
end
```

## Development

After checking out the repo, run `bin/setup` to install dependencies. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/[USERNAME]/microurb_view_tool.

## License

The gem is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).
