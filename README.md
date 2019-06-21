# Wrap

Build, Publish & Deploy Elixir Infrastructure to the Cloud.

`wrap` is a set of `mix` tasks that use [Distillery](https://github.com/bitwalker/distillery) to 
build an OTP release within [Docker](https://www.docker.com/), publish the container to a registry and 
deploy to cloud infrastructure via [Terraform](https://www.terraform.io/).

## Installation

Add `wrap` to your list of dependencies in `mix.exs`

```elixir
def deps do
  [
    {:wrap, "~> 0.0.3"}
  ]
end
```

## Usage

```
mix wrap.list          # List packages
mix wrap.build         # Build docker images from distillery releases
mix wrap.publish       # Publish latest docker images
mix wrap.plan          # Plan terraform definition
mix wrap.apply         # Apply terraform definition
mix wrap.destroy       # Destroy packages
```
