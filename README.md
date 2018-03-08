# angularCLIScriptsOnlyStatSize

This project was created in reference to https://github.com/webpack-contrib/webpack-bundle-analyzer/issues/147#issuecomment-371045968.

The Anguluar CLI project when creating the scripts bundle only concatonates the scripts and is not wrapped in a webpack funciton. This results in the webpack-bundle-analyzer defaulting to the stats.json information rather than showing gzip information and parse size.

To reproduce:

1) Download the repo
2) Yarn install
3) Yarn run build
4) Yarn run bundle-report
