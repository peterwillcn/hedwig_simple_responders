# Hedwig Simple Responders

[![CircleCI](https://circleci.com/gh/labzero/hedwig_simple_responders.svg?style=shield)](https://circleci.com/gh/labzero/hedwig_simple_responders)
[![Hex.pm](https://img.shields.io/hexpm/v/hedwig_simple_responders.svg)](https://hex.pm/packages/hedwig_simple_responders)
[![Hex.pm](https://img.shields.io/hexpm/dt/hedwig_simple_responders.svg)](https://hex.pm/packages/hedwig_simple_responders)

A collection of simple responders for use with a [Hedwig](https://github.com/hedwig-im/hedwig) chat bot. Heavily inspired by the *hubot-scripts* package for Hubot.

#### Responders

| Responder       | Module                           |
|-----------------|----------------------------------|
| Beer Me         | HedwigSimpleResponders.BeerMe    |
| Calming Manatee | HedwigSimpleResponders.Manatee   |
| Echo            | HedwigSimpleResponders.Echo      |
| Fish Pun        | HedwigSimpleResponders.Fishpun   |
| Flip            | HedwigSimpleResponders.Flip      |
| Pug Me          | HedwigSimpleResponders.PugMe     |
| Shingy          | HedwigSimpleResponders.Shingy    |
| Ship it!        | HedwigSimpleResponders.ShipIt    |
| Slime           | HedwigSimpleResponders.Slime     |
| Slogan          | HedwigSimpleResponders.Slogan    |
| Stallman        | HedwigSimpleResponders.Stallman  |
| Time            | HedwigSimpleResponders.Time      |
| Toot!           | HedwigSimpleResponders.Toot      |
| Trout Slap      | HedwigSimpleResponders.TroutSlap |
| Uptime          | HedwigSimpleResponders.Uptime    |


## Installation

Add `hedwig_simple_responders` to your list of dependencies in `mix.exs`:

```elixir
def deps do
  [
    {:hedwig, "~> 1.0"},
    {:hedwig_simple_responders, "~> 0.1.2"}
  ]
end
```

## Usage

Enable some or all the included responders by adding them to your list of `responders` in `config/config.exs`

```elixir
config :my_hedwig_robot, MyHedwigRobot.Robot,
  adapter: Hedwig.Adapters.Console,
  responders: [
    {HedwigSimpleResponders.Slogan, []},
    {HedwigSimpleResponders.ShipIt, %{ extra_squirrels: false }},
    {HedwigSimpleResponders.Stallman, []},
    # ...
  ]
```

## Contributing

1. [Fork it!](http://github.com/labzero/hedwig_simple_responders/fork)
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

## License

The MIT License (MIT)

Copyright (c) 2016 Lab Zero

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
