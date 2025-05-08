---
title: "Module 1: Collaborating in JupyterHub"
---

:::{note} Objectives
:class: dropdown

* Jupyter is much more than Notebooks
* Interact with geospatial data in JupyterLab
* Interact with GitHub
:::


## Presentation

<iframe
  src="https://docs.google.com/presentation/d/e/2PACX-1vSX1BAt5-Dzd1VtXttMqSFRI-HhhCI3lQx8-tfmHQvsXabBrnDxsYYBMLNQgMhYZfTiFLV0vuxTnd3W/pubembed?start=false&loop=false&delayms=60000"
  frameborder="0" width="960" height="569" allowfullscreen="true"
  mozallowfullscreen="true" webkitallowfullscreen="true">
</iframe>


## 💪 Exercise

### Step 0: Create and clone a new repository for this workshop's exercises

1. Create a new repository in GitHub from our
  [workshop template repository](https://github.com/geojupyter/workshop-csdms2025-template).

  :::{figure} ../assets/images/github-use-template.png
  Click the green "Use template" button in the upper-right, then select "create a new
  repository".
  :::

1. Leave all the settings as default: your username should be the "owner", and the repo
   should be public. Set the "Repository name" to `workshop-csdms2025-exercises` -- this
   will make it easier for us to find it!

1. In JupyterHub, clone the new repository you just created from the template.
   We'll be working here from now on! **Run the command below, replacing `MY-USERNAME`
   with your GitHub account username**.

  ```bash
  git clone https://github.com/MY-USERNAME/workshop-csdms2025-exercises
  ```


### Step 1: Set up GitHub authentication in JupyterHub (WIP)

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


### Step 2: Explore the example data (WIP)

1. Navigate to the newly cloned repository in the JupyterLab file browser.
1. Enter the `exercises/module-1` directory.
1. Double-click the GeoJSON file to view it with the JupyterLab viewer.


### Step 2: Open our example Notebook and create some new data (WIP)

This Notebook is pre-populated with some code.

1. Run all the cells (_TODO: Details_).
1. Add a new cell which adds more data into the GeoDataFrame.
1. Add another new cell which saves the GeoDataFrame with a new filename.


### Step 3: Push to GitHub (WIP)

_TODO_
