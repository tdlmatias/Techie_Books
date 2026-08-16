# Contributing to Techie Books

First off — **thank you!** 🙌 This library exists because people like you share the resources that helped them learn. Every book you add helps the whole community that stars and follows this project.

This guide keeps contributions consistent and easy to review. It's short — please skim it before opening a pull request.

---

## What belongs here

Books, guides, and reference material on:

- Cybersecurity, ethical hacking & penetration testing
- Linux (administration, internals, programming)
- Networking & protocols
- DevOps and the systems/security foundations around it
- Closely related technology topics (make the case in your PR)

Formats we accept: **PDF** (preferred), EPUB, and images for cheat sheets. Large files may be committed compressed (e.g. `.pdf.gz`).

---

## The one rule that matters most: sharing rights ⚖️

Only contribute material that is **free to redistribute**:

- ✅ **Public domain** works
- ✅ **Openly licensed** works (e.g. Creative Commons)
- ✅ Books the **author or publisher has made freely available**

🚫 **Do not upload material you don't have the right to share.** When in doubt, leave it out — or link to the official free download instead of uploading the file.

By opening a pull request, you confirm the material you're adding is free to share. Rights holders can request removal any time via an [issue](https://github.com/tdlmatias/Techie_Books/issues).

---

## How to add a book

### Option A — Web (no git needed)

1. **Fork** the repo (top-right **Fork** button).
2. On your fork, click **Add file → Upload files** and drop your book in the repository root.
3. Edit `README.md` on your fork to add a row for the book in the right section.
4. Commit, then open a **pull request** back to this repo.

### Option B — Git

```bash
# 1. Fork on GitHub, then clone your fork
git clone https://github.com/<your-username>/Techie_Books.git
cd Techie_Books

# 2. Create a branch
git checkout -b add-docker-deep-dive

# 3. Add your file to the repo root
cp ~/Downloads/Docker-Deep-Dive.pdf .

# 4. Add a catalog row in README.md, then commit
git add .
git commit -m "Add Docker Deep Dive to Linux & System Administration"

# 5. Push and open a PR
git push -u origin add-docker-deep-dive
```

---

## Filename conventions

Good filenames make the library searchable and the links reliable:

- Use a **descriptive title**, ideally with author or edition:
  `The-Web-Application-Hackers-Handbook-2nd-Edition.pdf`
- Prefer hyphens over spaces where practical (spaces are OK but must be URL-encoded in links — see below).
- Avoid tracker/junk suffixes like `( PDFDrive.com )` on new uploads.
- Keep the correct extension (`.pdf`, `.epub`, `.pdf.gz`).

---

## Adding your catalog entry

In `README.md`, find the matching section and add a table row:

```markdown
| [Book Title — Author (Edition)](Your-Filename.pdf) |
```

If your filename contains **spaces or special characters**, URL-encode them in the link (the visible title can stay readable):

| Character | Use in link |
| --------- | ----------- |
| space | `%20` |
| `+` | `%2B` |
| `'` | `%27` |
| `(` `)` | `%28` `%29` |
| `@` | `%40` |

Example:

```markdown
| [TCP / UDP](TCP%20UDP.pdf) |
```

Not sure about the category? Add it to the closest one and mention your uncertainty in the PR — a maintainer will help place it.

---

## Pull request checklist

Before you submit, please confirm:

- [ ] The material is **free to redistribute** (public domain, open-licensed, or author/publisher-free).
- [ ] The file is in the **repository root** with a clear, descriptive name.
- [ ] A **catalog row** was added to `README.md` in the right section, with a working (URL-encoded) link.
- [ ] The PR description says **what the book is** and **why it belongs here**.

---

## Other ways to contribute

- 🗂️ Reorganize or clean up categories and filenames.
- 🔗 Fix broken links or mislabeled entries.
- ✍️ Improve book descriptions in the catalog.
- 🐛 [Open an issue](https://github.com/tdlmatias/Techie_Books/issues) for anything that looks wrong.

---

Thanks again for helping keep great learning material free and easy to find. Happy hacking! 🚀
