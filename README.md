# claude-cache-timer workspace

Meta-repository that groups the cache-timer projects as git submodules.

| Path | Repository | What it is |
|---|---|---|
| `claude-cache-timer/` | [suenot/claude-cache-timer](https://github.com/suenot/claude-cache-timer) | The Claude Code plugin: band with the time left on the 1-hour prompt cache, auto-compact, keep warm. Plugin installs come from this repo. |
| `claude-cache-timer-website/` | [suenot/claude-cache-timer-website](https://github.com/suenot/claude-cache-timer-website) | Landing page (static HTML/CSS/JS with GSAP motion design), deployed on Vercel. |

Clone with everything:

```
git clone --recurse-submodules https://github.com/suenot/claude-cache-timer-workspace.git
```

Update the submodules to their latest commits:

```
git submodule update --remote --merge
```

Each submodule is committed and pushed in its own repository first; then the workspace commits the new submodule pointer.
