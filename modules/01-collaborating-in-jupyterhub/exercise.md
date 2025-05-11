---
title: "💪 Exercise"
---

## Step 0: Log in to the JupyterHub

1. Visit <https://hub.cryointhecloud.com>.
   You may want to bookmark this page!
1. **Select the last option, "Bring your own image"**.
    * Copy/paste `ghcr.io/geojupyter/geojupyter:latest` into the "custom image" field.
    * Leave "Resource Allocation" as default (1.9GB RAM).
1. **Click "Start"**!
    * It may take a moment for the server to start.
      When it's done, **place a green sticky on the corner of your laptop screen** so
      instructors know you're ready!
    * If startup takes longer than a couple of minutes, put up a red sticky and we'll
      take a look!


## Step 1: Create and clone a new repository for this workshop's exercises

1. Create a new repository in GitHub from our
  [workshop template repository](https://github.com/geojupyter/workshop-csdms2025-template).

    :::{figure} ../../assets/images/github-use-template.png
    Click the green "Use template" button in the upper-right, then select "create a new
    repository".
    :::

1. Leave most of the settings as default: your username should be the "owner", and the
   repo should be public. **Set the "Repository name" to
   `workshop-csdms2025-exercises`** -- this will make it easier for us to find it!

1. **In JupyterHub**, clone the new repository you just created from the template.
   We'll be working here from now on! **Run the command below, replacing `MY-USERNAME`
   with your GitHub account username**.

    ```bash
    git clone https://github.com/MY-USERNAME/workshop-csdms2025-exercises
    ```


## Step 2: Explore the example data

1. Navigate to the newly cloned repository in the JupyterLab file browser on the left
   panel.
   If the left panel isn't open, click the topmost icon in the far left column.
1. Navigate to the `exercises/module-1` directory.
1. Double-click the GeoJSON file `seec.json` to view it with the JupyterLab viewer.


## Step 3: Open our example Notebook and create some new data (WIP)

1. Open `example-1.ipynb` by double-clicking it in the file browser in the left panel.
1. This notebook is pre-populated with some code.
   **Run all the cells** by pressing `SHIFT+ENTER` repeatedly until you reach the end.
1. Add a new cell which adds more data into the GeoDataFrame (_TODO_: Prompt and empty
   space in notebook).
   Start with the address of a location that is meaningful to you:
   Your favorite coffee shop?
   The shelter where you adopted your pet?
   The town where you grew up?
1. Add another new cell which saves the GeoDataFrame with a new filename.


## Step 4: Set up GitHub authentication in JupyterHub (WIP)

In order to push changes from the JupyterHub, you need credentials.
Since the JupyterHub is a shared cloud service, saving credentials there can be
dangerous.
Therefore, we use a special tool,
[`gh-scoped-creds`](https://github.com/jupyterhub/gh-scoped-creds),
to limit this risk.

1. Grant access to the app (_TODO: Details_)
1. Configure your exercises repository to work with `gh-scoped-creds` (_TODO: Details_)

This configuration is valid for 8 hours.
If you need to refresh your access, please re-do the final step in the list above.


## Step 5: Push to GitHub (WIP)

1. `git add .`
1. `git commit --message="Add new data to GeoJSON"`
   This step may fail.
   If it does, you need to tell Git your name and e-mail, then try again.
   Git will print out the commands you need to execute to fix this problem.
1. `git push --set-upstream origin main`
