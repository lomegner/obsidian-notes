In GitHub, a **Release** is a **tagged snapshot** of your repository, typically with **pre-compiled binaries, release notes, and downloadable assets**.

| Git concept          | GitHub concept                    |
| -------------------- | --------------------------------- |
| Tag (`git tag v1.0`) | **Release** (tag + notes + files) |

## What you can do with releases:

1. **Download** source code (ZIP/tarball)
2. **Attach** compiled binaries (`.exe`, `.apk`, `.dmg`)
3. **Write** release notes/changelog
4. **Mark** as "Latest" or "Pre-release"
5. **Automate** with GitHub Actions (build + upload)
common use cases:
- **Software projects** → distribute compiled versions
- **Libraries** → mark stable versions
- **Documentation** → archive specific versions

for creating a release navigate to code->tags->releases