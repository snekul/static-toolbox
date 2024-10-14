# static-toolbox

This repository includes prebuild static binaries and build-recipes for various tools like Nmap and OpenSSH.

The Linux versions are compiled with the musl-cross toolchain and the openssl-pm-snapshot fork of OpenSSL in order to support a wide range of SSL/TLS features (Warning: some of them are insecure!).

Compilation is done automatically with GitHub Actions. The binaries are uploaded to the [release section](https://github.com/ernw/static-toolbox/releases). The artifacts are also available in the artifacts of each GitHub Action. However, there are some limitations:

* Downloading of build artifacts in GitHub Ations currently requires a GitHub account
* Blobs in build artifacts are zipped by the GitHub frontend by default, even zip files themselves! Build artifact zips may contain other zip files.
* Build artifacts will expire after some time.

Therefore, it is recommended to download the binaries from the release section.
