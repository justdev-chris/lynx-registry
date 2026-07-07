# 🐾 Lynx Registry

This repository is the **official package registry** for the [Lynx programming language](https://github.com/justdev-chris/Lynx).

It hosts Lynx packages as versioned tarballs that can be installed via `lynx install`.

---

## 📁 Structure

```

/<pkg>/<version>/package.tar.gz

```

Example:

```

/json/1.0.0/package.tar.gz
/http/0.2.1/package.tar.gz

```

---

## 📦 How to Publish

1. Run `lynx publish`
2. This creates `<name>-<version>.tar.gz`
3. Upload it to this repo:
   - Create a folder: `packages/<name>/<version>/`
   - Copy the tarball there and rename it to `package.tar.gz`
   - Commit and push

**Don't know how to use the terminal?** Use GitHub's web interface to upload files, or ask someone to help.

---

📥 How to Install

```
lynx install
```

Packages are downloaded from:

```
https://raw.githubusercontent.com/justdev-chris/lynx-registry/main/<pkg>/<version>/package.tar.gz
```

---

📚 Documentation

Full docs in docs/.

---

📄 License

MIT