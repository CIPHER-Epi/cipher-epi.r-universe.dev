# cipher-epi.r-universe.dev

The registry for [cipher-epi.r-universe.dev](https://cipher-epi.r-universe.dev), which builds jheem2 and the
packages it needs from GitHub as binaries for Windows, macOS and Linux.

- **jheem2** is built from its latest release (`*release`): each release cut by jheem2's release workflow.
- **bayesian.simulations, distributions, locations** are built from their default branches.

To install:

```r
options(repos = c(cipher = "https://cipher-epi.r-universe.dev", CRAN = "https://cloud.r-project.org"))
install.packages("jheem2")
```

To add a package, add an entry to `packages.json` (`package` must match the Package field of its DESCRIPTION).
See the [r-universe documentation](https://docs.r-universe.dev/publish/set-up.html).
