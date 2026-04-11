# CongruentC
I love C, but I sometimes find C does not come with things that I need.
That is what CongruentC (Congruency) is for. A suite of tools I actually use, organized so I stop losing them.
---
## Philosophy
C is small and honest about what it is and I want to keep it that way. But there are gaps that every C programmer fills alone, slightly and differently each time. CongruentC is my attempt to fill them once and move on.
The goal is that every tool here feels like it came from the same place. Same conventions, same naming, same memory model. You learn one and the next one already feels familiar. That is what congruent means and that is what I am going for.
---
## Tools
Nothing gets added here until I have built it, used it in a real project, and decided it is worth keeping.
| Tool | Description | Status |
|------|-------------|--------|
| `cg_sv` | String view, a pointer and a length | Complete |
| `cg_da` | Dynamic array, growable and generic | Complete |
| `cg_sb` | String builder, append without managing memory manually | Functional |
| `cg_hm` | Hash map, string keys and arbitrary values | Ongoing |
| `cheaders` | Auto-generate header files from your source files | Planned |
Each tool lives in its own repository. Some tools depend on others — dependencies are always minimal and clearly stated.
---
## Conventions
Every tool follows these rules so they all feel consistent:
- **stb-style** — one header file, define `CG_TOOLNAME_IMPLEMENTATION` in one translation unit and include everywhere else
- **File and repo names** — use the `cg_` prefix, e.g. `cg_sv.h`, `cg_da.h`
- **Types and functions** — use the `cg` prefix without underscore, e.g. `cgsv`, `cgda`, `cgsv_from_cstr`
- **Dependencies** — tools declare their dependencies explicitly. If a tool requires another, it will say so.
---
## Contributing
Open an issue before writing any code. Talk it through first. If something fits, I am happy to work with you on it. If you find a bug please say so.
---
## Status
Early days. I am building this as I go.
