# FOSSA Snippet Demo

The purpose of this repository is to demonstrate FOSSA's snippet scanning capability. At the time of this typing, Millhone (the original name of FOSSA's snippet scanning capability) is in early preview stages and is currently separated from the CLI. 
🟢 [v3.8.16](https://github.com/fossas/fossa-cli/releases/tag/v3.8.16) is the latest update to snippet scanning.

Run `fossa snippets analyze --help` to learn more on how to use it. This repository shares an example result of snippets detected from [opencv](https://github.com/opencv/opencv/blob/4.x/apps/annotation/opencv_annotation.cpp).

### Useful commands

```
fossa snippets analyze --overwrite-output -o snippets
```

Review results via `jq`
```
cat snippets/main.c.json | jq
```

### References

- https://github.com/fossas/fossa-cli/blob/master/docs/references/subcommands/snippets.md
- FOSSA C++ Demo Example: https://github.com/fossas/cpp-vsi-demo
