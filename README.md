# Credits import issue

When importing a project with two dependencies — pondo_protocol and credits — I encounter the error described below. However, if I remove the direct credits import (since it’s already included inside pondo_protocol), I then get an error saying my program cannot read mappings from the credits program.

## Install @doko-js/cli@1.1.1-beta and dependencies

Leo used: leo github repo with tag

[testnet-v3.5.0](https://github.com/ProvableHQ/leo/releases/tag/testnet-v3.5.0)

```npm install -g @doko-js/cli@1.1.1-beta```

```npm i```

## Compile project

`dokojs compile`

### Error we get

```
Error [EPAK0375054]: Conflicting dependency. The existing dependency is 'credits.aleo (on Local) (at /Users/sandeshpokhrel/Workspace/ibriz/cred_imp_issue/imports/credits.aleo)', while the new one is 'credits.aleo (on Network)'.
     |
     = If your project has multiple dependencies on the same program, make sure that they are all network or all local dependencies, with the same editions.
```

### Artifacts of project can be found at artifacts/leo directory after compilation
