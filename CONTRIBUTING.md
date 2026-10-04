# Contributing to Aero Linux Project

Thank you for your interest in contributing to the **Aero Linux Project**! We are building the ultra-lean AI & developer operating system suite from first principles.

---

## 🚀 Guiding Engineering Principles

1. **Zero Runtime Bloat:** Every CLI tool, script, and GTK3 app must be self-contained and execute instantaneously with minimal memory footprint (<350MB idle target).
2. **First-Principles Depth:** Prefer native Linux kernel interfaces (`sysfs`, `procfs`, `systemd`, `zram`, `bpf`) over heavy wrappers or electron/web-view bloat.
3. **Verified Quality:** 100% test coverage with zero regressions (`make test`).

---

## 🛠️ Development Setup & Workflow

### 1. Clone & Set Up Workspace
```bash
git clone https://github.com/aero-linux/aero-linux.git
cd aero-linux
```

### 2. Run Test Suite
```bash
make test
```
All unit tests in `tests/` must pass before opening a PR.

### 3. Build & Verify Debian Package
```bash
make deb
```
Ensures package structure, dependencies, and file paths are valid.

---

## 🤝 Submitting a Pull Request

1. **Fork the repo** and create your branch from `main`:
   ```bash
   git checkout -b feat/your-feature-name
   ```
2. **Commit your changes:** Follow conventional commits (`feat: ...`, `fix: ...`, `docs: ...`, `perf: ...`).
3. **Open a PR:** Ensure your PR description adheres to `.github/PULL_REQUEST_TEMPLATE.md` with verification steps.

---

## 💡 Architectural RFCs & Proposals

For major features (e.g. eBPF socket tracing, Rust compositor integration, new GTK3 developer applications), please open an issue using the **Feature Request / RFC** template or start a thread in **Discussions**.
