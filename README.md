# Proof tools

One page for eight small open-source tools that check what really happened:
backups, scheduled jobs, CI and repository security, installed dependencies,
AI coding agents, LLM answers, device traffic and saved reading.

**<https://maximo000.github.io/tools/>**

| Tool | Checks | Install |
|---|---|---|
| [firedrill](https://github.com/MaXiMo000/firedrill) | a database backup restores and is usable | `pip install firedrill` |
| [escrow](https://github.com/MaXiMo000/escrow) | scheduled jobs are still running | `pip install escrow-evidence` |
| [carabiner](https://github.com/MaXiMo000/carabiner) | a repository's security controls exist and fire | `pip install carabiner-sec` |
| [lockstep](https://github.com/MaXiMo000/lockstep) | what's installed matches the lockfile | `pip install lockstep-evidence` |
| [receipt](https://github.com/MaXiMo000/receipt) | what a command or AI agent changed on disk | `pip install receipt-evidence` |
| [sourced](https://github.com/MaXiMo000/sourced) | an LLM answer against its own sources | `pip install sourced-evidence` |
| [drift](https://github.com/MaXiMo000/drift) | a device's traffic against its allow-list | `pip install drift-evidence` |
| [satchel](https://github.com/MaXiMo000/satchel) | a local, searchable archive of what you read | `pip install satchel-reader` |

Every tool reports `pass`, `fail` or `unverified`, and a check that couldn't
run is never reported as a pass.

## This repository

A single static `index.html` with no build step, published with GitHub Pages
from the `main` branch. To preview it locally:

```bash
python -m http.server 8000
```

Then open <http://localhost:8000>.

MIT licensed.
