# Registry Index

---

## `packages.json`

The file `packages.json` at the root of the registry lists all available packages.

---

## Format

```json
{
  "packages": {
    "json": {
      "description": "JSON parser and generator",
      "versions": ["1.0.0", "1.0.1"],
      "latest": "1.0.1"
    },
    "http": {
      "description": "HTTP client",
      "versions": ["0.2.1"],
      "latest": "0.2.1"
    }
  }
}
```

---

Fields

Field Description
description Short summary of the package
versions List of all available versions
latest The most recent stable version

---

Updating

When you publish a new package or version, update packages.json manually.
