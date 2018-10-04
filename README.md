# dxw::utils

This gem is for common code accross dxw's Ruby/Rails projects.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'dxw-utils', git: 'https://github.com/dxw/dxw-utils'
```

And then execute:

```bash
    $ bundle
```

## Components

### Rubocop

To use the shared Rubocop rules in your dxw project, install the gem in your project and add the following lines to your `.rubocop.yml`:

```yml
inherit_gem:
  dxw-utils:
    - dxw-rubocop.yml
```

If you wish to have project-specific Rubocop rules (cops), you can add them to your project's `.rubocop.yml` after the `inherit_gem` declaration, as normal.

Note that you do not need to include Rubocop in your project's Gem file. Using `spec.add_dependency` in dxw-utils' Gemspec means Rubocop will automatically be available to the including project.

## License

The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
