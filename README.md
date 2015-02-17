## Sensu-Plugins-mackerel

[![Build Status](https://travis-ci.org/sensu-plugins/sensu-plugins-mackerel.svg?branch=master)](https://travis-ci.org/sensu-plugins/sensu-plugins-mackerel)
[![Gem Version](https://badge.fury.io/rb/sensu-plugins-mackerel.svg)](http://badge.fury.io/rb/sensu-plugins-mackerel)
[![Code Climate](https://codeclimate.com/github/sensu-plugins/sensu-plugins-mackerel/badges/gpa.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-mackerel)
[![Test Coverage](https://codeclimate.com/github/sensu-plugins/sensu-plugins-mackerel/badges/coverage.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-mackerel)
[![Dependency Status](https://gemnasium.com/sensu-plugins/sensu-plugins-mackerel.svg)](https://gemnasium.com/sensu-plugins/sensu-plugins-mackerel)

## Functionality

## Files
 * bin/metrics-mackerel

## Usage

```
{
  "mackerel": {
    "hostid": "XXXXXXXXXXX",
    "api_key": "XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX"
  }
}
```
## Installation

Add the public key (if you haven’t already) as a trusted certificate

```
gem cert --add <(curl -Ls https://raw.githubusercontent.com/sensu-plugins/sensu-plugins.github.io/master/certs/sensu-plugins.pem)
gem install sensu-plugins-mackerel -P MediumSecurity
```

You can also download the key from /certs/ within each repository.

#### Rubygems

`gem install sensu-plugins-mackerel`

#### Bundler

Add *sensu-plugins-disk-checks* to your Gemfile and run `bundle install` or `bundle update`

#### Chef

Using the Sensu **sensu_gem** LWRP
```
sensu_gem 'sensu-plugins-mackerel' do
  options('--prerelease')
  version '0.0.1'
end
```

Using the Chef **gem_package** resource
```
gem_package 'sensu-plugins-mackerel' do
  options('--prerelease')
  version '0.0.1'
end
```

## Notes
