# DemoAppWithSPM
[![security status](https://www.meterian.io/badge/gh/MeterianHQ/DemoAppWithSPM/security?branch=main)](https://www.meterian.io/report/gh/MeterianHQ/DemoAppWithSPM)
[![stability status](https://www.meterian.io/badge/gh/MeterianHQ/DemoAppWithSPM/stability?branch=main)](https://www.meterian.io/report/gh/MeterianHQ/DemoAppWithSPM)
[![licensing status](https://www.meterian.io/badge/gh/MeterianHQ/DemoAppWithSPM/licensing?branch=main)](https://www.meterian.io/report/gh/MeterianHQ/DemoAppWithSPM)

This is a demo applicaton using SwiftPM. Here you can see a sample usage of the Meterian Github Action when applied to an opensource project. In order to have Meterian checking your code you case use this simple workflow:

```
# .github/workflows/meterian.yml

name: Meterian Scanner workflow

on: push

jobs:
    meterian_scan:
        name: Meterian client scan
        runs-on: ubuntu-latest
        steps:
          - name: Checkout
            uses: actions/checkout@v3
          - name: Meterian Scanner
            uses: MeterianHQ/meterian-github-action@v1.0.13
            with:
              oss: true
```
You can find more information ad [docs.meterian.io](https://docs.meterian.io), where you can also checkout our [GitHub Action guide](https://docs.meterian.io/guide-your-first-scan/your-first-scan-github-action)

Stay safe!
