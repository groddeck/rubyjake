<p align="center">
  RubyJake
</p>

----------
[![Gem Version](https://badge.fury.io/rb/rubocop.svg)](https://badge.fury.io/rb/rubocop)
[![CircleCI Status](https://circleci.com/gh/rubocop-hq/rubocop/tree/master.svg?style=svg)](https://circleci.com/gh/rubocop-hq/rubocop/tree/master)
[![Actions Status](https://github.com/rubocop-hq/rubocop/workflows/CI/badge.svg?branch=master)](https://github.com/rubocop-hq/rubocop/actions?query=workflow%3ACI)
[![Coverage Status](https://api.codeclimate.com/v1/badges/ad6e76460499c8c99697/test_coverage)](https://codeclimate.com/github/bbatsov/rubocop)
[![Code Climate](https://codeclimate.com/github/bbatsov/rubocop/badges/gpa.svg)](https://codeclimate.com/github/bbatsov/rubocop)
[![Inline docs](https://inch-ci.org/github/bbatsov/rubocop.svg)](https://inch-ci.org/github/bbatsov/rubocop)
[![SemVer](https://api.dependabot.com/badges/compatibility_score?dependency-name=rubocop&package-manager=bundler&version-scheme=semver)](https://dependabot.com/compatibility-score.html?dependency-name=rubocop&package-manager=bundler&version-scheme=semver)

[![Patreon](https://img.shields.io/badge/patreon-donate-orange.svg)](https://www.patreon.com/bbatsov)
[![OpenCollective](https://opencollective.com/rubocop/backers/badge.svg)](#open-collective-backers)
[![OpenCollective](https://opencollective.com/rubocop/sponsors/badge.svg)](#open-collective-sponsors)
[![Tidelift](https://tidelift.com/badges/package/rubygems/rubocop)](https://tidelift.com/subscription/pkg/rubygems-rubocop?utm_source=rubygems-rubocop&utm_medium=referral&utm_campaign=readme)

**RubyJake** is a Ruby static code analyzer (a.k.a. `linter`) and code formatter forked from this excellent [project](https://docs.rubocop.org/) . Out of the box it
will enforce many of the guidelines outlined in the community [Ruby Style
Guide](https://rubystyle.guide). Apart from reporting the problems discovered in your code,
RubyJake can also automatically fix many of them you.

RubyJake is extremely flexible and most aspects of its behavior can be tweaked via various
[configuration options](https://github.com/rubocop-hq/rubocop/blob/master/config/default.yml).

This fork was created in order to rebrand this tool in honor of "jakes" an affectionate term for firefighters, whose daily, anonymous heroism evokes universal respect for this essential profession and its role in communities.

## Installation

**RubyJake**'s installation is pretty standard:

```sh
$ gem install rubocop
```

If you'd rather install RubyJake using `bundler`, add a line for it in your `Gemfile` (but set the `require` option to `false`, as it is a standalone tool):

```rb
gem 'rubocop', require: false
```

RubyJake's development is moving at a very rapid pace and there are
often backward-incompatible changes between minor releases (since we
haven't reached version 1.0 yet). To prevent an unwanted RubyJake update you
might want to use a conservative version lock in your `Gemfile`:

```rb
gem 'rubocop', '~> 0.85.1', require: false
```

## Quickstart

Just type `rubocop` in a Ruby project's folder and watch the magic happen.

```
$ cd my/cool/ruby/project
$ rubocop
```

## Documentation

You can read a lot more about RubyJake in its [official docs](https://docs.rubocop.org).

## Compatibility

RubyJake supports the following Ruby implementations:

* MRI 2.4+
* JRuby 9.2+

RubyJake has customarily provided support for about a year after EOL of MRI Ruby version.
This is done by RubyJake core to provide the community with a margin of transition.

## Team

Here's a list of RubyJake's core developers:

* [Bozhidar Batsov](https://github.com/bbatsov) (author & head maintainer)
* [Jonas Arvidsson](https://github.com/jonas054)
* [Yuji Nakayama](https://github.com/yujinakayama) (retired)
* [Evgeni Dzhelyov](https://github.com/edzhelyov) (retired)
* [Ted Johansson](https://github.com/drenmi)
* [Masataka Kuwabara](https://github.com/pocke)
* [Koichi Ito](https://github.com/koic)
* [Maxim Krizhanovski](https://github.com/darhazer)
* [Benjamin Quorning](https://github.com/bquorning)
* [Marc-André Lafortune](https://github.com/marcandre)

## Contributors

Here's a [list](https://github.com/rubocop-hq/rubocop/graphs/contributors) of
all the people who have contributed to the development of RubyJake.

I'm extremely grateful to each and every one of them!

If you'd like to contribute to RubyJake, please take the time to go
through our short
[contribution guidelines](CONTRIBUTING.md).

Converting more of the Ruby Style Guide into RubyJake cops is our top
priority right now. Writing a new cop is a great way to dive into RubyJake!

Of course, bug reports and suggestions for improvements are always
welcome. GitHub pull requests are even better! :-)

## Changelog

RubyJake's changelog is available [here](CHANGELOG.md).

## Copyright

Copyright (c) 2012-2020 Bozhidar Batsov. See [LICENSE.txt](LICENSE.txt) for
further details.
