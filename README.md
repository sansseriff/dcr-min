# dcr-min
Code and figures for the paper "Free-space coupled superconducting nanowire single-photon detector with low dark counts"

## Quick install

<!-- QUICK_INSTALL_START -->

Run one of these commands in a terminal to clone and set up the project (requires that git is installed):

⚠️ Warning: Only use single line installers like these if you trust the creator of this repository. 

macOS/Linux (curl):

```zsh
curl -fsSL https://sansseriff.github.io/dcr-min/dl.sh | bash
```

macOS/Linux (wget):

```zsh
wget -qO- https://sansseriff.github.io/dcr-min/dl.sh | bash
```

Windows (PowerShell):

```powershell
powershell -NoProfile -ExecutionPolicy Bypass -Command "iwr -UseBasicParsing https://sansseriff.github.io/dcr-min/dl.ps1 | iex"
```

### Security: Verify before running

To verify the integrity of `dl.sh` before running it:

```zsh
# Download the script without executing
curl -o dl.sh __RAW_BASE_URL__/dl.sh

# Verify SHA256 hash matches the one below
shasum -a 256 dl.sh

# Inspect the script content
cat dl.sh

# Inspect what will be installed
curl -s __RAW_BASE_URL__/dl-util/install_and_sync.sh | less

# If everything looks good, run it
sh dl.sh
```

Integrity (SHA256 of dl.sh):

```text
0b0a1f2094de2fcdc6ac057091c4db1f99661b6f024dfeab3de8fcb86e4450fe
```

<!-- QUICK_INSTALL_END -->


## uv Usage hints

- Add a Python package with `uv add <package-name>`
- Create a local virtual environment `.venv` from the `uv.lock` and `pyproject.toml` files. (already done by install script)
- Run a Python file using the local environment with `uv run <python-file>`
- Run a Jupyter Lab server using the local environment with `uv run --with jupyter jupyter lab`
- Learn more about using uv here: https://docs.astral.sh/uv/guides/projects/#creating-a-new-project
