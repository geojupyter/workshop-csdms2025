---
title: "💪 Exercise"
---

### Step 1: Set up GitHub Pages

1. Open your repository on GitHub.
1. Click "⚙️ Settings" towards the top of the page.
    ![](../../assets/images/github-pages-settings.png)

All of the other scaffolding you need is already included in this repo in the
`.github/workflows` directory.
When you build your own MyST website, you can reproduce this with `myst init --site` and
`myst init --gh-pages`.


### Step 2: Make a change & push to GitHub

1. Edit any file in `examples/module-3/my-website`.
1. Commit and push:

    ```bash
    git add .
    git commit --message="Edit to trigger GitHub Pages deployment"
    git push origin main
    ```

### Step 3: View your new GitHub Pages deployment!

1. In your repository, view the GitHub Actions progress.
  1. From the repository home page, click the "Actions" tab towards the top.
  1. You should see an action titled "Edit to trigger GitHub Pages deployment", matching
     the commit message from the previous step.
     Is it complete (green check)?
     Or is it still in progress?
     Did it fail (red X)? Let us know if it failed.
1. View your website. Check that the change you made in the previous step is visible!
  * Your website will be available at this URL (replace `MY-USERNAME` with your username
😉):

    ```
    https://MY-USERNAME.github.io/workshop-csdms2025-examples
    ```

### Step 4: Edit your notebook to display some data (WIP)

_TODO_
