# Hello World Repository
The hello-world repository is a minimal demonstration repository containing only a readme.md file with the text "hello".

Always reference these instructions first and fallback to search or bash commands only when you encounter unexpected information that does not match the info here.

## Working Effectively
- Clone and navigate to repository:
  - `git clone https://github.com/nextmindb/hello-world.git`
  - `cd hello-world`
- Basic repository operations (all complete in under 0.01 seconds):
  - `git status` - Check repository status
  - `git log --oneline` - View commit history  
  - `ls -la` - List all files including hidden ones
  - `cat readme.md` - View the main content file

## Repository Structure
```
hello-world/
├── .git/                 # Git metadata
├── readme.md            # Main content file containing "hello"
└── .github/             # GitHub configuration (created for Copilot instructions)
    └── copilot-instructions.md
```

## Build and Test
- **NO BUILD REQUIRED**: This repository contains no executable code or build system.
- **NO TESTS AVAILABLE**: This repository contains no test suite or testing framework.
- **NO RUNTIME**: This repository does not contain runnable applications.

## Available Development Tools
The following development tools are available in the environment:
- Python 3: `/usr/bin/python3` (version 3.12.3)
- Node.js: `/usr/local/bin/node` (version v20.19.4) 
- Java: `/usr/bin/java` (OpenJDK 17.0.16)
- Go: `/usr/bin/go` (version go1.24.6)
- GCC: `/usr/bin/gcc` (version 13.3.0)

All tools are functional and can be used for development if needed, though this repository contains no executable code.

## Validation
- Always validate any changes by running:
  - `git status` - Ensure changes are staged properly (~0.003s)
  - `cat readme.md` - Verify content integrity (~0.001s)
  - `git log --oneline -5` - Check commit history (~0.004s)
- NEVER CANCEL git operations - all git commands complete in under 0.05 seconds
- Manual validation scenarios:
  - **Content integrity**: Verify readme.md contains exactly "hello " (with trailing space and newline): `[ "$(cat readme.md)" = "hello " ] && echo "VALID" || echo "INVALID"`
  - **Structure integrity**: Ensure repository has exactly 2 content files (readme.md + copilot-instructions.md): `find . -maxdepth 2 -name "*.md" | wc -l` should return 2
  - **Git functionality**: Confirm git operations work correctly: `git status && git log --oneline -1` 
  - **Reference commit**: Verify original commit exists: `git log --oneline | grep -q d853a22 && echo "FOUND" || echo "MISSING"`

## Common Tasks
The following are outputs from frequently run commands. Reference them instead of viewing, searching, or running bash commands to save time.

### Repository root listing
```
$ ls -la
total 20
drwxr-xr-x 4 runner docker 4096 Aug 15 07:14 .
drwxr-xr-x 3 runner docker 4096 Aug 15 07:10 ..
drwxr-xr-x 7 runner docker 4096 Aug 15 07:14 .git
drwxr-xr-x 2 runner docker 4096 Aug 15 07:14 .github
-rw-r--r-- 1 runner docker    7 Aug 15 07:10 readme.md
```

### Git status (with new .github directory)
```
$ git status
On branch copilot/fix-3
Untracked files:
  (use "git add <file>..." to include in what will be committed)
	.github/

nothing added to commit but untracked files present (use "git add" to track)
```

### Git history
```
$ git log --oneline
d853a22 Create readme.md
```

### Main content file
```
$ cat readme.md
hello 
```

### Git remotes
```
$ git remote -v
origin	https://github.com/nextmindb/hello-world (fetch)
origin	https://github.com/nextmindb/hello-world (push)
```

## Key Guidelines
- This is a demonstration/template repository - treat modifications carefully
- Always preserve the simple "hello world" nature of the repository
- Any new files should maintain the minimal, educational character
- Document any additions in this instruction file
- When making changes, always test the basic git workflow still functions properly
- All operations complete quickly (under 1 second) - no long-running processes exist

## Troubleshooting
- If `git status` shows unexpected changes, use `git diff` to review modifications
- If readme.md is corrupted, it should contain exactly "hello " (with trailing space and newline)
- Repository should always contain exactly one content file (readme.md) plus git metadata
- If repository becomes inconsistent, verify against the reference commit d853a22