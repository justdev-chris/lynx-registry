# Naming Conventions

---

## Package Names

- Lowercase only
- No spaces
- Hyphens allowed for multi-word names

Examples:

```

json
http-client
my-awesome-lib

```

---

## Versioning

Follow [Semantic Versioning](https://semver.org/):

```

<major>.<minor>.<patch>

```

Examples:

```

1.0.0
2.1.3
0.5.0

```

---

## Folder Structure

Each package lives in:

```

/<name>/<version>/package.tar.gz

```

Example:

```

/json/1.0.0/package.tar.gz

```

---

## Reserved Names

- `std` — standard library
- `test` — reserved for testing
- `libs` — reserved for extracted packages