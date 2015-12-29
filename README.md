# Luhn algorithm in Elixir

[![Build Status](https://travis-ci.org/my-flow/luhnatex.svg?branch=master)](https://travis-ci.org/my-flow/luhnatex)
[![Hex.pm](https://img.shields.io/hexpm/v/luhnatex.svg)](https://hex.pm/packages/luhnatex)

Validate Luhn number.

## Installation

```
# mix.exs
defp deps do
  [
    {:luhn, "~> 0.5.0"}
  ]
end

# and fetch
$ mix deps.get
```

## How to use

```
# validate number
Luhn.valid? "378282246310005"
# => true

# Integer type number
Luhn.valid? 378282246310005
# => true

# Luhn base 16 mod 10
Luhn.valid? "0F04871513130338972614312C30307", 16, 10
# => true
```

## Benchmarking

```
$ mix archive.install https://github.com/alco/benchfella/releases/download/v0.2.1/benchfella-0.2.1.ez
$ mix bench
```

## LICENSE

MIT
