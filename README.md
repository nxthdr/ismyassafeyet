# Route Origin Validation Check

Simple tool to check if your AS (ISP, own AS, etc.) is correctly implementing RPKI ROV.
Basically [isbgpsafeyet](https://isbgpsafeyet.com/) but as a CLI tool.

```
Usage: rovcheck [OPTIONS]

Options:
      --valid-url <VALID_URL>      The URL to use for valid requests [default: https://valid.rpki.isbgpsafeyet.com]
      --invalid-url <INVALID_URL>  The URL to use for invalid requests [default: https://invalid.rpki.isbgpsafeyet.com]
      --alphabet <ALPHABET>        Alphabet to use for generating the ID [default: 1234567890abcdef]
  -t, --timeout <TIMEOUT>          Requests timeout [default: 3]
  -v, --verbose...                 Increase logging verbosity
  -q, --quiet...                   Decrease logging verbosity
  -h, --help                       Print help
  -V, --version                    Print version
```

## Acknowledgements

This tool is by default relying on Cloudflare's [isbgpsafeyet](https://isbgpsafeyet.com/) infrastructure to work. Thanks to Cloudflare for providing this service.
