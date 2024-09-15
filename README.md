# Logicer's Reusable GitHub Actions Workflows

A useful set of reusable workflows common to many projects.

## Usage

```yaml
jobs:
  <workflow>:
    uses: "logicer16/workflows/.github/workflows/<reusable_workflow>.yml@main"
    with:
      <input>: <value>
    secrets:
      <secret>: <value>
    # or 
    secrets: inherit
```

## Workflows

* [`docker.yml`](https://github.com/Logicer16/workflows/blob/main/.github/workflows/docker.yml) build and publish a docker image
* [`dockerhub-description.yml`](https://github.com/Logicer16/workflows/blob/main/.github/workflows/dockerhub-description.yml) update description of an image on Docker Hub to make the repo's `README.md` and short description.
* [`update-repo.yml`](https://github.com/Logicer16/workflows/blob/main/.github/workflows/update-repo.yml) update a repo by merging upstream and updating submodules
