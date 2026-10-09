# Git Repository

If you already have **Git** installed and you're using **VSCodium**, the simplest workflow is:

## First-time Git setup

If you haven't configured Git yet:

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

Check it:

```bash
git config --list
```

## Classic push (if Git is installed)

### 1. Open your project folder in VSCodium

```bash
cd /path/to/your/project
codium .
```

### 2. Initialize Git (only once per project)

```bash
git init
```

### 3. Add your GitHub repository as the remote (only once)

Replace the URL with your repository's URL:

```bash
git remote add origin https://github.com/USERNAME/REPOSITORY.git
```

Or, if you use SSH:

```bash
git remote add origin git@github.com:USERNAME/REPOSITORY.git
```

### 4. Add your files

```bash
git add .
```

### 5. Commit your changes

```bash
git commit -m "Initial commit"
```

### 6. Push to GitHub

If this is your first push:

```bash
git branch -M main
git push -u origin main
```

For future pushes, you only need:

```bash
git add .
git commit -m "Describe your changes"
git push
```

## Check your status anytime

```bash
git status
```

The basic workflow you'll use most often is:

```bash
git add .
git commit -m "Your message"
git push
```

If you tell me:

* whether you're using **HTTPS** or **SSH**, and
* whether the GitHub repository already exists,

I can give you the exact commands for your setup.

## Using VSCodium instead

You can also do it from the Source Control panel:

1. Open your project in VSCodium.
2. Click the **Source Control** icon (branch icon).
3. Click **Initialize Repository** (if needed).
4. Stage files with the **+** button.
5. Enter a commit message.
6. Click **Commit**.
7. Click **Publish Branch** or **Push**.