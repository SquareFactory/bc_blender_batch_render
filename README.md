# Batch Connect - Blender Batch Renderer

![GitHub Release](https://img.shields.io/github/release/csquare-ai/bc_osc_codeserver.svg)

A Batch Connect app designed for OnDemand that launches blender with multi node rendering features within an Reindeer Pizza Cluster batch job.

## Prerequisites

This Batch Connect app requires the following software be installed on the
**compute nodes** that the batch job is intended to run on (**NOT** the
OnDemand node):

- [Lmod] 6.0.1+ or any other `module purge` and `module load <modules>` 
- [blender] 

[blender]: https://www.blender.org/
[lmod]: https://www.tacc.utexas.edu/research-development/tacc-projects/lmod

## Install

1.  Use Git to clone this app and checkout the desired branch/version you want to
    use and place this wherever you store batch connect apps (`/var/www/ood/apps/sys` or `~/ondemand/dev`):

    ```sh
    git clone <repo>
    cd <dir>
    git checkout <tag/branch>
    ```

2.  Deploy code-server on your systems.

3.  Update form.yml to use the correct cluster, and any other changes as necessary to form.yml or submit.yml that is appropriate for your cluster.

## Update

To update the app you would:

```sh
cd <dir>
git fetch
git checkout <tag/branch>
```

Again, you do not need to restart the app as it isn't a Passenger app.

## Known Issues

- None.
