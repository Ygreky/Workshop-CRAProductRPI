This repository contains materials for the Workshop "CRA Conformance and Raspberry Pi: A Collaborative Analysis of Compliance Dos and Don’ts"

- core-image-base-raspberrypi2.rootfs.spdx.json - SPDX 3.0.1 SBOM for an example image with meta-raspberrypi
- 2026-04-13-raspios-trixie-armhf-lite.sbom.xz - SPDX 2.3 SBOM for the Raspios image based on Debian

Uncompress with:
```
xz -dk 2026-04-13-raspios-trixie-armhf-lite.sbom.xz
```
The file is JSON, some tools may require the .json extension, so you can rename:
```
mv 2026-04-13-raspios-trixie-armhf-lite.sbom 2026-04-13-raspios-trixie-armhf-lite.sbom.json
```

For SPDX 2 to 3 conversion use https://github.com/spdx/tools-java

For reviewing (manually) JSON-formatted SBOMs, use ''jq'' (easy available in your system), for example:
```
jq <2026-04-13-raspios-trixie-armhf-lite.sbom.json |less
```

Online tools:
-------------
- SPDX 3 visualiser https://tools.spdx.org/app/spdx3_viz/
- Bomlens demo (with fixed source SBOMs - one is an RPI image) https://sktelecom.github.io/bomlens/demo/#/
