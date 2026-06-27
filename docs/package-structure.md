# Package Structure

---

## Tarball Contents

A valid package tarball (`package.tar.gz`) contains:

```

package.tar.gz
├── src/
│   └── main.lnx       # Entry point
└── lynx.toml          # Metadata

```

---

## `lynx.toml` Example

```toml
[package]
name = "json"
version = "1.0.0"
authors = ["Your Name"]
description = "JSON parser and generator"

[dependencies]
```

---

Entry Point

src/main.lnx is the main file. It can load sub‑files via Stalk_Pack:

```lynx
Stalk_Pack "libs/json/parser.lnx"
Stalk_Pack "libs/json/utils.lnx"
```

---

Sub‑Files

You can have multiple .lnx files in src/ or a libs/ folder inside the package. Just reference them with Stalk_Pack or KittyPort (if they're separate packages).
