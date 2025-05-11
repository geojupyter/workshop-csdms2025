---
title: "💪 Exercise"
---

## Step 0: Log in to the JupyterHub

1. **Visit <https://hub.cryointhecloud.com>**.
   You may want to bookmark this page!
1. **Select the last option, "Bring your own image"**.
    * Copy/paste `ghcr.io/geojupyter/geojupyter:latest` into the "custom image" field.
    * Leave "Resource Allocation" as default (1.9GB RAM).
1. **Click "Start"**!
    * It may take a moment for the server to start.
      When it's done, **place a 🟩 green sticky on the corner of your laptop screen**
      so instructors know you're ready!
    * If startup takes longer than a couple of minutes, put up a **🟥 red sticky** and we'll
      take a look!


## Step 1: Create and clone a new repository for this workshop's exercises

1. **Create a new repository in GitHub from our
  [workshop template repository](https://github.com/geojupyter/workshop-csdms2025-template)**.

    :::{figure} ../../assets/images/github-use-template.png
    Click the green "Use template" button in the upper-right, then select "create a new
    repository".
    :::

1. Leave most of the settings as default: your username should be the "owner", and the
   repo should be public. **Set the "Repository name" to
   `workshop-csdms2025-exercises`** -- this will make it easier for us to find it!

1. **In JupyterHub, clone the new repository you just created** from the template.
   We'll be working here from now on!
    1. Create a new tab in JupyterHub with the ➕ icon.
    1. Launch a terminal.
    1. In the terminal, **Run the command below, replacing `MY-USERNAME`
       with your GitHub account username**.

    ```bash
    git clone https://github.com/MY-USERNAME/workshop-csdms2025-exercises
    ```


## Step 2: Explore some example data

1. **Navigate to the newly cloned repository in the JupyterLab file browser** on the
   left panel.
    * If the left panel isn't open, click the topmost icon in the far left column.
1. **Navigate to the `exercises/module-1` directory**.
1. **Double-click the GeoJSON file `seec.json`** to view it with the JupyterLab viewer.
1. **Right-click the same GeoJSON file `seec.json`, and select "JSON"** to view the raw
   contents of the file in a structured way.

JupyterLab is about much more than Notebooks!
It's built to be an interactive computational tool that helps us think about problems.
As the Jupyter community grows, so do JupyterLab's capabilities, and it becomes a more
complete solution over time.
We'll explore some of the latest examples of this progress soon.


## Step 3: Open our example Notebook

1. **Open `example-1.ipynb`** by double-clicking it in the file browser in the left panel.
1. This notebook is pre-populated with some code.
   **Run most of the cells** by pressing `SHIFT+ENTER` repeatedly until you reach the
   challenge cells at the end.


## Step 4: Create some new data

1. **Fill in the final cells of the Notebook to add more data to the GeoDataFrame.**
   Start with a location that is meaningful to you:
   Your favorite coffee shop?
   The shelter where you adopted your pet?
   The town where you grew up?
1. Run the final cells.


## Step 5: Push our work to GitHub

### Step 5a: Set up authentication

In order to push changes from the JupyterHub, you need credentials.
Since the JupyterHub is a shared cloud service, saving credentials there can be
dangerous.
Therefore, we use a special tool,
[`gh-scoped-creds`](https://github.com/jupyterhub/gh-scoped-creds),
to limit this risk.

1. **In the terminal, run the command**:

    ```bash
    gh-scoped-creds
    ```

1. This will output a URL and an authorization code.
   **Visit the URL and input the code**.
1. This will output another URL.
    * Visit that URL.
    * Click the "Configure" button.
    * Select your username from the list, and continue.
    * Select "Only select repositories", and then select `workshop-csdms2025-exercises`.
    * Click "Install".

This configuration is valid for 8 hours.
If you need to refresh your access later, please re-do these steps.


### Step 5b: Push!

1. **Run the following commands in the terminal**:

    ```bash
    git add .
    git commit --message="Add new data to GeoJSON"`
    ```

    :::{warning} This step will probably fail!
    If it does, you need to tell Git your name and e-mail, then try again.
    **Git will print out the commands you need to execute to fix this problem**.
    :::

1. **Run the following command in the terminal**:

    ```bash
    git push --set-upstream origin main
    ```
