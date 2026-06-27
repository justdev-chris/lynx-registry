# Package Structure

---

## Tarball Contents

```

package.tar.gz
├── src/
│   └── main.lnx
└── lynx.toml

```

---

## `lynx.toml` Example

```toml
[package]
name = "json"
version = "1.0.0"
authors = ["Your Name"]
description = "JSON parser"

[dependencies]
```

---

Entry Point

src/main.lnx is the main file. Sub‑files can be loaded via Stalk_Pack:

```lynx
Stalk_Pack "libs/json/parser.lnx"
```