# Linode autodiscovery plugin for Automatron

This plugin provides the ability to auto discover Linode instances for Automatron

## Installation

Simply copy the `linode/` directory to Automatron's `plugins/discovery/` directory.

```shell
$ cp -r linode plugins/discovery/
```

Install python required modules

```shell
$ pip install -r requirements.txt
```

## Configuration

This plugin does require some configuration in Automatron's master configuration file `config.yml`.

```yaml
discovery:
  plugins:
    linode:
      url: http://example.com
      api_key: example
      interval: 60
```

The `linode` plugin requires three configuration items.

* `url` - This is the URL to Linode's API
* `api_key` - This is the Linode API key
* `interval` - This is the frequency to query Linode's API
