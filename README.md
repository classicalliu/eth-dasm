# EthDasm

[![Build Status](https://travis-ci.org/classicalliu/eth-dasm.svg?branch=master)](https://travis-ci.org/classicalliu/eth-dasm)

EVM disassembler in ruby language.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'eth-dasm', github: 'classicalliu/eth-dasm'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install eth-dasm

## Usage

```ruby
# mode can be :int, :hex or :"int:hex", default is :"int:hex"
EthDasm::Byte2op.decode(code, mode = :"int:hex")
# example
EthDasm::Byte2op.decode("0x...", :"int:hex")
```

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake spec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/classicalliu/eth-dasm. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](http://contributor-covenant.org) code of conduct.

## License

The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).

## Code of Conduct

Everyone interacting in the EthDasm project’s codebases, issue trackers, chat rooms and mailing lists is expected to follow the [code of conduct](https://github.com/classicalliu/eth-dasm/blob/master/CODE_OF_CONDUCT.md).
