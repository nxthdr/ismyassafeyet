# Is my AS safe yet?

Simple CLI tool to check if the AS (ISP, own AS, etc.) is correctly implementing RPKI ROV.
It's basically [isbgpsafeyet](https://isbgpsafeyet.com/) but in a CLI tool.

```
Usage: ismyassafeyet [OPTIONS]

Options:
      --valid-url <VALID_URL>      The URL to use for valid requests [default: https://valid.rpki.isbgpsafeyet.com]
      --invalid-url <INVALID_URL>  The URL to use for invalid requests [default: https://invalid.rpki.isbgpsafeyet.com]
  -t, --timeout <TIMEOUT>          Request timeout [default: 3]
  -v, --verbose...                 Increase logging verbosity
  -q, --quiet...                   Decrease logging verbosity
  -h, --help                       Print help
  -V, --version                    Print version
```

## Acknowledgements

This tool is by default relying on Cloudflare's [isbgpsafeyet](https://isbgpsafeyet.com/) infrastructure to work. Thanks to Cloudflare for providing this service.