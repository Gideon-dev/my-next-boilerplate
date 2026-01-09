

# 🚀 Getting Started — Choose Your Workflow

This boilerplate supports **two intentional workflows** depending on how you want to use it.

Read this once. It prevents 90% of Git mistakes.

---

## 🟢 Option 1: Clean Clone (Recommended)

**Best if you want a fresh app with no connection to this boilerplate.**

You get the code — **not the history**.

### Steps

```bash
git clone https://github.com/Gideon-dev/my-next-boilerplate.git my-app
cd my-app
rm -rf .git
git init
git branch -M main
git add .
git commit -m "chore: bootstrap project"
```

Create a new GitHub repo, then:

```bash
git remote add origin https://github.com/YOUR_USERNAME/my-app.git
git push -u origin main
```

### What this means

* ✅ Your app is fully yours
* ✅ No accidental pushes to this repo
* ✅ Clean commit history
* ❌ No automatic updates from this boilerplate

This is the **safest default**.

---

## 🟠 Option 2: Advanced Clone (Opt-in Updates)

**Best if you want to receive future improvements intentionally.**

You keep a **read-only connection** to this boilerplate via `upstream`.

### Steps

```bash
git clone https://github.com/Gideon-dev/my-next-boilerplate.git my-app
cd my-app
git remote rename origin upstream
```

Create your own repo, then:

```bash
git remote add origin https://github.com/YOUR_USERNAME/my-app.git
git push -u origin main
```

### Pulling Updates Later

When you *choose* to update:

git fetch upstream
git merge upstream/main



### What this means

* ✅ You own your app
* ✅ Upstream is pull-only
* ✅ Updates are opt-in
* ❌ No automatic syncing

---

## 🔑 Important Concept: What is `upstream`?

**`upstream` is the original source of the boilerplate.**

You:

* pull from it
* never push to it
* stay in control

```text
upstream (boilerplate) ──▶ your repo ──▶ production
```

If you didn’t create the repo, it’s **upstream**.

---

## 🚫 Things You Should NOT Do

* Do not push to `upstream`
* Do not expect automatic updates
* Do not treat this as a dependency manager

Git is the contract.

---

## ✅ Recommendation

If you’re unsure, use **Clean Clone**.

You can always reintroduce upstream later —
you cannot easily remove coupling once added.

