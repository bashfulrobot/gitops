# BS

While bootstrapping a cluster can be BS, I just need to bootstrap.

This folder is contains scripts and documentation.

## ToDO

- looking at this video:
    - change repo to use a key vs a PAT
- Secrets for the sysdig agent
- Add sysdig agent values.
- document Cilium bootstrap
- Finish sysdig install and wiring

## Steps

### Cilium

- do this.

### FluxCd

- install the fluxcd & [just](https://github.com/casey/just
) cli tools
- if you do not have a git repo setup, login to GitHub
- create the repo
- go to `profile > settings > developer settings > personal access tokens > Tokens (classic)`
- create a new classic token:
    - expire whenever. This is short term (7 days) for just bootstrapping. We will be adding access keys
    - under `repo` read/write. Click the main `repo` checkbox which will select all the sub settings.
    - Press `generate token` button
- run `just flux [name of cluster]` in this directory
    - example: `just flux spitfire`
    - this cluster name is used to target the proper directory in git (`cluster/cluster-name`)
    - Note that it will ask you for the PAT you created above.


