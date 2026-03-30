# distancefyi

[![crates.io](https://img.shields.io/crates/v/distancefyi.svg)](https://crates.io/crates/distancefyi)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

Haversine distance calculation and travel time estimation — API client for [distancefyi.com](https://distancefyi.com).

> **Try the interactive tools at [distancefyi.com](https://distancefyi.com)**

## Install

`cargo add distancefyi`

## Quick Start

```rust
use distancefyi::Client;

#[tokio::main]
async fn main() -> Result<(), Box<dyn std::error::Error>> {
    let client = Client::new();
    let result = client.search("seoul").await?;
    println!("{} results", result.total);
    Ok(())
}
```

## Also Available

| Platform | Package | Link |
|----------|---------|------|
| **Python** | `pip install distancefyi` | [PyPI](https://pypi.org/project/distancefyi/) |
| **npm** | `npm install distancefyi` | [npm](https://www.npmjs.com/package/distancefyi) |
| **Go** | `go get github.com/fyipedia/distancefyi-go` | [pkg.go.dev](https://pkg.go.dev/github.com/fyipedia/distancefyi-go) |
| **Rust** | `cargo add distancefyi` | [crates.io](https://crates.io/crates/distancefyi) |
| **Ruby** | `gem install distancefyi` | [rubygems](https://rubygems.org/gems/distancefyi) |

## Embed Widget

Embed [DistanceFYI](https://distancefyi.com) widgets on any website with [distancefyi-embed](https://widget.distancefyi.com):

```html
<script src="https://cdn.jsdelivr.net/npm/distancefyi-embed@1/dist/embed.min.js"></script>
<div data-distancefyi="entity" data-slug="seoul"></div>
```

Zero dependencies · Shadow DOM · 4 themes (light/dark/sepia/auto) · [Widget docs](https://widget.distancefyi.com)

## Links

- [DistanceFYI](https://distancefyi.com) — Main site
- [API Documentation](https://distancefyi.com/developers/)
- [OpenAPI Spec](https://distancefyi.com/api/openapi.json)
- [Glossary](https://distancefyi.com/glossary/)

## License

MIT
