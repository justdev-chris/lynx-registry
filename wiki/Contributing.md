# Contributing to the Registry

---

## Adding a Package

1. Create a Lynx project
2. Write your code
3. Run `lynx publish`
4. Upload tarball to this repo
5. Update `packages.json`
6. Commit and push

---

## Updating a Package

1. Bump version in `lynx.toml`
2. Run `lynx publish`
3. Upload to `<name>/<new-version>/package.tar.gz`
4. Update `packages.json`
5. Commit and push

---

## Removing a Package

- Delete the folder: `<name>/`
- Remove its entry from `packages.json`
- Commit and push

---

## Review Process

- Packages are **not reviewed** — the registry is community-driven
- Use common sense
- Follow naming conventions

---

## License

All packages must use the MIT license (same as Lynx).