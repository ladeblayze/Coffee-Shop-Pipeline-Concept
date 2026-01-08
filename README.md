# GitHub Actions Learning Repository

This repository contains hands-on lessons for learning GitHub Actions using a coffee shop example.

## 🎯 Learning Objectives

By working through these lessons, you'll learn:
- How to create GitHub Actions workflows
- How to use manual triggers (`workflow_dispatch`)
- How to chain jobs with dependencies
- How to save and share data between jobs (artifacts)
- How to create reusable workflows

## 📚 Lessons

### Lesson 1: Basic Workflow Structure
**File:** `.github/workflows/lesson-1-basic.yml`

Learn about:
- Workflow triggers
- Input parameters
- Conditional jobs (`if:` statements)
- Basic shell commands

**Try it:** Go to Actions → Lesson 1 → Run workflow

---

### Lesson 2: Job Dependencies
**File:** `.github/workflows/lesson-2-dependencies.yml`

Learn about:
- The `needs:` keyword
- Running jobs in sequence
- Creating a pipeline of jobs

**Try it:** Go to Actions → Lesson 2 → Run workflow

---

### Lesson 3: Artifacts (Saving Data)
**File:** `.github/workflows/lesson-3-artifacts.yml`

Learn about:
- Uploading artifacts
- Downloading artifacts in later jobs
- Comparing data from different stages

**Try it:** Go to Actions → Lesson 3 → Run workflow

---

### Lesson 4: Reusable Workflows
**Files:** 
- `.github/workflows/_reusable-make-coffee.yml` (the reusable part)
- `.github/workflows/lesson-4-reusable-demo.yml` (how to use it)

Learn about:
- Creating reusable workflows with `workflow_call`
- Calling workflows from other workflows
- Running multiple instances in parallel

**Try it:** Go to Actions → Lesson 4 → Run workflow

---

## 🚀 How to Run These Workflows

1. Go to the **Actions** tab in this repository
2. Select a lesson from the left sidebar
3. Click **"Run workflow"** button
4. Fill in the inputs (location, shift, orders, etc.)
5. Click **"Run workflow"** to start
6. Watch the jobs run in real-time!

## 📖 Reading the Output

Each job will show:
- ✅ Green checkmark = Success
- ❌ Red X = Failed
- 🟡 Yellow dot = Running

Click on any job to see detailed logs of what happened.

## 🎓 Next Steps

After completing these lessons, you'll be ready to understand real deployment pipelines like the one in your SRE work!

The concepts here map directly to deployment workflows:
- **Lesson 1** → Understanding workflow structure
- **Lesson 2** → Pre-deploy → Deploy → Post-deploy chains
- **Lesson 3** → Saving baseline snapshots and comparing them
- **Lesson 4** → Calling Pulumi workflows repeatedly

## 💡 Practice Exercises

1. **Modify Lesson 1:** Add a new shift called "training" that runs different steps
2. **Modify Lesson 2:** Add a new job that runs in parallel with `morning-rush`
3. **Modify Lesson 3:** Create a new artifact that tracks customer complaints
4. **Modify Lesson 4:** Add a third order to the reusable workflow example

## 🔗 Resources

- [GitHub Actions Documentation](https://docs.github.com/en/actions)
- [Workflow Syntax Reference](https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions)
