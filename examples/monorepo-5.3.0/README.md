Does not work

`bazel build //ui:bundle`

```
INFO: Invocation ID: 437fc0ea-e77c-45ea-8163-1c7dac53511e
DEBUG: /data/home/eric/.cache/bazel/_bazel_eric/39f14e9dac564798c1d9f3f2910b9f71/external/build_bazel_rules_nodejs/index.bzl:65:14: node_repository attribute not set and no repository named 'nodejs_toolchains' exists; installing default node
DEBUG: /data/home/eric/.cache/bazel/_bazel_eric/39f14e9dac564798c1d9f3f2910b9f71/external/build_bazel_rules_nodejs/index.bzl:73:14: yarn_install#yarn attribute not set and no repository named 'yarn' exists; installing default yarn
INFO: Analyzed target //ui:bundle (0 packages loaded, 0 targets configured).
INFO: Found 1 target...
ERROR: /data/home/eric/code/rules_nodejs/examples/monorepo-5.3.0/ui/BUILD.bazel:16:11: Compiling TypeScript project //ui:ts [tsc -p ui/tsconfig.json] failed: (Exit 2): tsc.sh failed: error executing command bazel-out/k8-opt-exec-2B5CBBC6/bin/external/npm/typescript/bin/tsc.sh --project ui/tsconfig.json --outDir bazel-out/k8-fastbuild/bin/ui --rootDir ui ... (remaining 1 argument skipped)

Use --sandbox_debug to see verbose messages from the sandbox
ui/index.tsx(1,24): error TS2307: Cannot find module 'react'.
ui/index.tsx(2,27): error TS2307: Cannot find module 'react-dom'.
Target //ui:bundle failed to build
Use --verbose_failures to see the command lines of failed build steps.
INFO: Elapsed time: 4.864s, Critical Path: 3.17s
INFO: 2 processes: 2 internal.
FAILED: Build did NOT complete successfully
```
