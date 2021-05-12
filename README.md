![GitHub Workflow Status](https://img.shields.io/github/workflow/status/jakobht/azurex/Elixir%20CI) ![Hex.pm](https://img.shields.io/hexpm/v/azurex)

# Azurex

Implementation of the Azure Blob Storage [Rest API](https://docs.microsoft.com/en-us/rest/api/storageservices/blob-service-rest-api) for Elixir.

## Supported actions

Currently supports:

1. Downloading blobs
2. Uploading blobs

## Installation

[Available in Hex](https://hex.pm/packages/azurex), the package can be installed
by adding `azurex` to your list of dependencies in `mix.exs` e.g.:

```elixir
def deps do
  [
    {:azurex, "~> 0.1.3"}
  ]
end
```

## Configuration

```elixir
config :azurex, Azurex.Blob.Config,
  api_url: "https://sample.blob.core.windows.net", # Optional
  default_container: "defaultcontainer", # Optional
  storage_account_name: "name",
  storage_account_key: "access key",
  storage_account_connection_string: "Storage=Account;Connection=String" # Required if storage account `name` and `key` not set
```

## Documentation

Documentation can be found at [https://hexdocs.pm/azurex](https://hexdocs.pm/azurex). Or generated using [ExDoc](https://github.com/elixir-lang/ex_doc)

## Development

The goal is to support all actions in the Azure Blob Storage [Rest API](https://docs.microsoft.com/en-us/rest/api/storageservices/blob-service-rest-api) - PRs welcome :)
