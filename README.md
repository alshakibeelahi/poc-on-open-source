# 🌍 How to Set Up an Open Source GitHub Repository

This guide will help you convert any project into a professional, community-ready open source project on GitHub.

---

## 1. 🆕 Create a GitHub Repository

- Go to [https://github.com/new](https://github.com/new)
- Choose a repository name (e.g., `my-project`)
- Add a short description
- **Do NOT initialize with a README or license** (you’ll add custom ones)
- Create the repository

---

## 2. 📁 Push Local Code to GitHub

In your project directory:

```bash
git init
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/yourusername/your-project.git
git push -u origin main
````

## 3. 📄 Add a License

Choose a license using [choosealicense.com](https://choosealicense.com/). For example, to add the MIT license:

1. Create a `LICENSE` file
2. Paste MIT License content
3. Commit the file:

   ```bash
   git add LICENSE
   git commit -m "Add MIT License"
   git push
   ```

---

## 4. 📝 Create a README.md

Explain your project:

* What it does
* How to install/use it
* How to contribute

Example starter:

```bash
touch README.md
```

Add content like:

```markdown
# My Project

A brief description of what this project does.

## Installation
...

## Usage
...

## Contributing
See [CONTRIBUTING.md](CONTRIBUTING.md)
```

---

## 5. 🤝 Add a CONTRIBUTING.md

Guide contributors on how to contribute:

```bash
mkdir .github
touch .github/CONTRIBUTING.md
```

Include:

* How to fork & clone
* Branch naming
* PR format
* Code style

---

## 6. 🔖 Add a Pull Request Template

Create a file:

```bash
touch .github/PULL_REQUEST_TEMPLATE.md
```

Example content:

```markdown
## Description

What changed and why?

## Checklist

- [ ] Tests added
- [ ] Docs updated
- [ ] Ready to be merged
```

---

## 7. 🔒 Set Branch Protection Rules (Recommended)

1. Go to your repo → **Settings** → **Branches**
2. Click on → **Add Classic Branch Protection Rule**
3. Add rule for `main` branch
4. Check:

   * ✅ Require pull request before merging
   * ✅ Require status checks (CI)
   * ✅ Require approvals

This ensures quality control before code is merged.

---

## 8. 🏷️ Add Topics and Description

From the repo homepage:

* Add a short description (1-liner)
* Add relevant topics (e.g., `open-source`, `typescript`, `api`)

---

## ✅ You're Done!

Your project is now open source and ready for the world to explore and contribute to. 🌐🎉

---

## 📚 Optional Enhancements

* `CODE_OF_CONDUCT.md` – define contributor behavior
* `SECURITY.md` – how to report vulnerabilities
* CI/CD with GitHub Actions
* Wiki or Documentation site
