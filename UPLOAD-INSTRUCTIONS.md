# How to Upload This to GitHub

## Option 1: GitHub Web Interface (No Git Required)

### Step 1: Create the Repository
1. Go to [github.com/new](https://github.com/new)
2. Repository name: `claude-skills`
3. Description: `Custom Claude AI skills — Resume Analyser & Strategy Toolkit`
4. Set to **Public**
5. Check **Add a README file**
6. License: **MIT License**
7. Click **Create repository**

### Step 2: Upload Files
1. In your new repo, click **Add file** → **Upload files**
2. Drag and drop ALL files from this folder
3. Since GitHub web does not support folders, you will need to create folders first:

**Create folders by creating files with paths:**
1. Click **Add file** → **Create new file**
2. Type `resume-analyser/README.md` (this creates the folder)
3. Paste the content from `resume-analyser/README.md`
4. Click **Commit new file**
5. Repeat for each file in each folder

### Step 3: Upload .skill Files
1. Navigate to the `resume-analyser` folder in your repo
2. Click **Add file** → **Upload files**
3. Drag `resume-analyser.skill` and drop
4. Commit
5. Repeat for `strategy-toolkit/strategy-toolkit.skill`

---

## Option 2: Git Command Line (Faster)

```bash
# 1. Create repo on GitHub first (github.com/new → "claude-skills")

# 2. Clone it locally
git clone https://github.com/YOUR-USERNAME/claude-skills.git
cd claude-skills

# 3. Copy all files from this folder into the cloned repo
# (replace /path/to/ with actual path where you saved the files)
cp -r /path/to/github-repo/* .

# 4. Add, commit, push
git add .
git commit -m "Add Resume Analyser and Strategy Toolkit skills"
git push origin main
```

---

## Option 3: GitHub Desktop (Easiest)

1. Download [GitHub Desktop](https://desktop.github.com/)
2. Create a new repository called `claude-skills`
3. Copy all files from this folder into the repository folder
4. In GitHub Desktop: write commit message → **Commit to main** → **Push origin**

---

## After Upload: Add Repository Topics

Go to your repo → click the gear icon next to "About" → add these topics:

```
claude, claude-ai, claude-skills, ai-tools, strategy, resume, 
career, business-strategy, competitive-analysis, five-forces,
blue-ocean-strategy, balanced-scorecard, resume-review
```

This helps people find your skills when searching GitHub.

## Recommended Repository Settings

- **About description:** `Custom Claude AI skills — Resume Analyser & Strategy Toolkit. Install in Claude.ai for expert-level resume review and business strategy analysis.`
- **Website:** `https://claude.ai`
- **Topics:** See list above
