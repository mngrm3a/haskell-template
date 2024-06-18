# usage

1. to create a new project:  

   `stack new <name> --bare --setup-info-yaml ./tmp/stack-config.yaml`
2. to use `cabal` and `hpack` but keep `stack.yaml`:  

   `gen-hie --cabal`
3. to use a package set from [stackage with cabal](https://cabal.readthedocs.io/en/3.8/nix-local-build.html#how-can-i-have-a-reproducible-set-of-versions-for-my-dependencies):
   ```cabal
   packages: .
   import: https://www.stackage.org/lts-22.26/cabal.config
   ```
4. remove unwanted files:  

   `rm -r .git ./tmp Changelog.md`