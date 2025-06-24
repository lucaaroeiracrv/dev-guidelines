# 🚀 Boas Práticas de Commits e Branches

![Git](https://img.shields.io/badge/Git-Essentials-blue?logo=git&logoColor=white)
![Commits](https://img.shields.io/badge/Commits-Convention-green)
![Branches](https://img.shields.io/badge/Branches-Naming-orange)

---

## ✉️ Most Common Prefixes (Commits)

Use prefixes to make the repository history easier to read and understand.  
**Always write commit messages in English.**

- **Add:** Add new feature, file, or dependency.
- **Update:** Update existing feature, improve code, or make small changes.
- **Fix:** Fix bugs.
- **Remove:** Remove code, files, or dependencies.
- **Refactor:** Refactor code (internal improvement, no behavior change).
- **Docs:** Documentation changes.
- **Test:** Add or update automated tests.
- **Chore:** Maintenance tasks, tooling, or chores (no direct impact on source code).
- **Style:** Code formatting, indentation, whitespace (no logic changes).
- **Build:** Changes to build scripts, CI/CD, or external tools.
- **Perf:** Performance improvements.
- **Revert:** Revert a previous commit.
- **Hotfix:** Urgent fix (typically in production).
- **Merge:** Merge branches.

### 💡 Examples

```text
Add: user registration page
Update: adjust header layout
Fix: error when saving user
Remove: obsolete files
Refactor: simplify authentication logic
Docs: update README
Test: add integration test
Chore: update dependencies
Style: standardize spacing
Build: update webpack config
Perf: optimize search filter
Revert: change X due to bug Y
Hotfix: fix memory leak
Merge: develop into main
```

---

## 🌿 Branch Naming Best Practices

Use branch naming conventions to organize work and facilitate collaboration.

- **feature/** or **feat/**: New features
- **bugfix/** or **fix/**: Bug fixes
- **hotfix/**: Urgent production fixes
- **refactor/**: Code refactoring
- **chore/**: Maintenance tasks
- **test/**: Test related
- **docs/**: Documentation

### 💡 Examples

```text
feature/user-registration-page
update/header-layout-adjustment
fix/save-user-error
remove/obsolete-files
refactor/authentication-logic-simplification
docs/update-readme
test/integration-test-addition
chore/dependency-update
style/spacing-standardization
build/webpack-config-update
perf/search-filter-optimization
revert/change-x-bug-y
hotfix/memory-leak-fix
merge/develop-into-main
```

> **Tip:**  
> Use `/` to separate the prefix from the description and `-` to separate words in the description.  
> Be clear and concise: avoid generic names like `dev` or `work`.  
> You may include issue/ticket numbers:  
> `feature/1234-user-profile-page`

---

## 🛠️ Git Commands for Commits

### 1. Stage files

```shell
git add .                     # Stage all changes
git add path/to/file.ext      # Stage a specific file
```

### 2. Create a simple commit

```shell
git commit -m "Update: improve menu responsiveness"
```

### 3. Create a commit with a description (body)

```shell
git commit -m "Update: improve menu responsiveness" -m "Fixes issues on small screens"
```
Or, use an editor for a multi-line message:
```shell
git commit
```
Then in the editor:
```
Update: improve menu responsiveness

Fixes issues on small screens
Improves accessibility for screen readers
```

### 4. Commit all tracked changes quickly

```shell
git commit -am "Update: update dependencies"
```
*(The `-a` flag stages modifications to tracked files. New files must be added with `git add` first.)*

### 5. Commit on a specific branch

The commit is always made on the current branch. To switch branches:
```shell
git checkout branch-name
git commit -m "your message"
```

---

## 💡 Tips

- Use short, objective phrases in the commit title.
- Always use the imperative form in English: "Add", "Update", "Fix", etc.
- Use the commit body for details if necessary.
- Prefer small, focused commits over large, generic ones.
- Follow the language and conventions adopted by your team/project.

---

## 🏷️ Prefix Reference Table

| Prefix    | Main Purpose                          |
|-----------|---------------------------------------|
| Add       | Add new features                      |
| Update    | Updates/improvements                  |
| Fix       | Bug fixes                             |
| Remove    | Remove code/files                     |
| Refactor  | Code refactoring                      |
| Docs      | Documentation                         |
| Test      | Tests                                 |
| Chore     | Maintenance/tasks                     |
| Style     | Formatting/style changes              |
| Build     | Build/configuration                   |
| Perf      | Performance                           |
| Revert    | Revert commits                        |
| Hotfix    | Urgent fixes                          |
| Merge     | Branch merges                         |

---

## 📚 References

- [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)
- [Git Commit Message Guidelines (Angular)](https://github.com/angular/angular/blob/main/CONTRIBUTING.md#commit)
- [GitHub Docs: About branches](https://docs.github.com/en/get-started/quickstart/github-glossary#branch)
