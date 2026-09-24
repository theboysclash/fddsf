# Fast Ubuntu

Open a working Ubuntu 24.04 system with one command:

```bash
ubuntu
```

The first launch downloads a small Ubuntu base (about 30MB) and installs a few basics. Later launches reuse that system and start in a fraction of a second. Packages you install and files under `/root` stay in `~/.local/share/fast-ubuntu`. This repository is mounted at `/workspace`.

The session runs as root, so `apt install` works without sudo.

From a checkout before the command is on your `PATH`:

```bash
./ubuntu
```

Run a single command instead of a shell:

```bash
ubuntu apt update
ubuntu nano /workspace/README.md
```

Start over with a clean system:

```bash
ubuntu --reset
```

GitHub Codespaces uses the dev container in this repo. After the codespace is created, run `ubuntu` in the terminal. You can also pick the **Ubuntu** terminal profile.
