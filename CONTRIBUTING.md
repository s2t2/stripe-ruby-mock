# Contributor's Guide

## Installation

Install package dependencies:

```sh
bundle install
```

## Setup

Run `cp .env.example .env`, then customize `.env` variables using your own Stripe credentials.

## Development

Start a mock server (optionally pass `-p` flag for custom port):

```sh
bin/stripe-mock-server
```

Start a development console:

```sh
bin/console
```

Start developing:

```sh
client = StripeMock.start_client
# etc.
client.get_server_data(:products)
```

## Testing

Run tests:

```sh
bundle exec rspec spec/
```
