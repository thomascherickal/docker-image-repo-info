## `adoptopenjdk:8u265-b01-jdk-hotspot-bionic`

```console
$ docker pull adoptopenjdk@sha256:4489ee7abb5421f5fd9045c44f8906012cbe9730cc0ec2cec47c5046fb4d21d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `adoptopenjdk:8u265-b01-jdk-hotspot-bionic` - linux; amd64

```console
$ docker pull adoptopenjdk@sha256:1658ee59dab5b73afdc9f92524b81ac54803125dc5fefe7b70d4ed9e961c756d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.3 MB (148280720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:824ded0a641b54bfa76bf92a1f2e6c97ea25a579d1f99c8c79917e846e4f9258`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 25 Sep 2020 22:34:27 GMT
ADD file:da80f59399481ffc32f84353830dcf598f31a97785222e75d643bfb8a9aa14e7 in / 
# Fri, 25 Sep 2020 22:34:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:34:29 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:34:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:34:30 GMT
CMD ["/bin/bash"]
# Fri, 16 Oct 2020 23:19:36 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Oct 2020 23:20:10 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Oct 2020 23:20:11 GMT
ENV JAVA_VERSION=jdk8u265-b01
# Fri, 16 Oct 2020 23:20:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='87d16dac293d2a9abbb559a277bfaded702f28d1bfdc526f8613bb9cfed84a12';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_aarch64_linux_hotspot_8u265b01.tar.gz';          ;;        armhf|armv7l)          ESUM='dc3405aab81f422b7721f665c76371bd7b03c291eea89cd110a82d8bcf07809a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_arm_linux_hotspot_8u265b01.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7bbb9d76458ee29bc5e2458b32a91b8c032ecffe6cb8500734ca41d2d8f5c9f3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u265b01.tar.gz';          ;;        s390x)          ESUM='aca50f02d59169cb428d54501846b518edc9fff6a6f428459c72b4faa2b4abb0';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_s390x_linux_hotspot_8u265b01.tar.gz';          ;;        amd64|x86_64)          ESUM='1285da6278f2d38a790a21148d7e683f20de0799c44b937043830ef6b57f58c4';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_x64_linux_hotspot_8u265b01.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 16 Oct 2020 23:20:18 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
```

-	Layers:
	-	`sha256:d72e567cc804d0b637182ba23f8b9ffe101e753a39bf52cd4db6b89eb089f13b`  
		Last Modified: Fri, 25 Sep 2020 15:20:50 GMT  
		Size: 28.6 MB (28558050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3630e5ff08d73b6ec0e22736a5c8d2d666e7b568c16f6a4ffadf8c21b9b1ad`  
		Last Modified: Fri, 25 Sep 2020 22:36:58 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a83d81d1f4f942d37e1f17195d9c519969ed3040fc3e444740b884e44dec33`  
		Last Modified: Fri, 25 Sep 2020 22:36:58 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f0c44dfceb587e1c4449c1d73f2490d56882599242350221d746e21daa3c8d0`  
		Last Modified: Fri, 16 Oct 2020 23:38:04 GMT  
		Size: 16.0 MB (16020270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e748d58c9712265174a39f827e5e32bc0f89ae58044997160ac1997f9ebfdaaf`  
		Last Modified: Fri, 16 Oct 2020 23:38:14 GMT  
		Size: 103.7 MB (103701390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:8u265-b01-jdk-hotspot-bionic` - linux; arm variant v7

```console
$ docker pull adoptopenjdk@sha256:2d7a43ee66c515e935b1afbaa7c68bc90771713dce1238468aea1a30f00ffd99
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.1 MB (137105501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30994e276af6a59ec1a0efae593022d5610becd62c63a6926f20b943d28fed38`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 25 Sep 2020 23:05:07 GMT
ADD file:545bf1be9048265e6c534b9b28f9f47c4a67fe2fe7331c7652187f3b43999005 in / 
# Fri, 25 Sep 2020 23:05:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 23:05:11 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 23:05:13 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 23:05:14 GMT
CMD ["/bin/bash"]
# Fri, 16 Oct 2020 23:58:17 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Oct 2020 23:58:49 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Oct 2020 23:58:51 GMT
ENV JAVA_VERSION=jdk8u265-b01
# Fri, 16 Oct 2020 23:59:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='87d16dac293d2a9abbb559a277bfaded702f28d1bfdc526f8613bb9cfed84a12';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_aarch64_linux_hotspot_8u265b01.tar.gz';          ;;        armhf|armv7l)          ESUM='dc3405aab81f422b7721f665c76371bd7b03c291eea89cd110a82d8bcf07809a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_arm_linux_hotspot_8u265b01.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7bbb9d76458ee29bc5e2458b32a91b8c032ecffe6cb8500734ca41d2d8f5c9f3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u265b01.tar.gz';          ;;        s390x)          ESUM='aca50f02d59169cb428d54501846b518edc9fff6a6f428459c72b4faa2b4abb0';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_s390x_linux_hotspot_8u265b01.tar.gz';          ;;        amd64|x86_64)          ESUM='1285da6278f2d38a790a21148d7e683f20de0799c44b937043830ef6b57f58c4';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_x64_linux_hotspot_8u265b01.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 16 Oct 2020 23:59:05 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
```

-	Layers:
	-	`sha256:39f6a73f1e6a145d93dd5878cc833f3930759e9c59f35905b5ebbcfba8669f0d`  
		Last Modified: Fri, 25 Sep 2020 23:06:54 GMT  
		Size: 24.0 MB (24038486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde417f16107c5260abc78817e22ed7d1fa0eab20e58929e4265b9b782fbc020`  
		Last Modified: Fri, 25 Sep 2020 23:06:47 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b336701abcacc2258baaa4f6e1714b011d5ca0ddbc5231e18f2b7b050b9bfb3`  
		Last Modified: Fri, 25 Sep 2020 23:06:48 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d2fa166473b86127a7a1a3e24278880570e62451d0004e81ad6fdc5a12cd0c7`  
		Last Modified: Sat, 17 Oct 2020 00:02:54 GMT  
		Size: 14.9 MB (14886649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf24153714eb41cc0ed07762d5a16d7cadc5bf93664809de7cf0da93ceeec183`  
		Last Modified: Sat, 17 Oct 2020 00:03:08 GMT  
		Size: 98.2 MB (98179330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:8u265-b01-jdk-hotspot-bionic` - linux; arm64 variant v8

```console
$ docker pull adoptopenjdk@sha256:16bb60cff8a9601b33dc057a0605f4053bddb6f4b41f2fa66e57d4981d6bfa3d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.9 MB (146886477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4322851d46ff070cab716d063278df593e4fc88e854071c8d3118bb8b45022a4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:59 GMT
ADD file:e1079b8987ad959c6a83dae1ea4446405953ab16899c693d57c6214ff888e688 in / 
# Fri, 25 Sep 2020 22:48:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:48:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:48:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:48:06 GMT
CMD ["/bin/bash"]
# Fri, 16 Oct 2020 23:39:44 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Oct 2020 23:40:17 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Oct 2020 23:40:18 GMT
ENV JAVA_VERSION=jdk8u265-b01
# Fri, 16 Oct 2020 23:40:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='87d16dac293d2a9abbb559a277bfaded702f28d1bfdc526f8613bb9cfed84a12';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_aarch64_linux_hotspot_8u265b01.tar.gz';          ;;        armhf|armv7l)          ESUM='dc3405aab81f422b7721f665c76371bd7b03c291eea89cd110a82d8bcf07809a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_arm_linux_hotspot_8u265b01.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7bbb9d76458ee29bc5e2458b32a91b8c032ecffe6cb8500734ca41d2d8f5c9f3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u265b01.tar.gz';          ;;        s390x)          ESUM='aca50f02d59169cb428d54501846b518edc9fff6a6f428459c72b4faa2b4abb0';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_s390x_linux_hotspot_8u265b01.tar.gz';          ;;        amd64|x86_64)          ESUM='1285da6278f2d38a790a21148d7e683f20de0799c44b937043830ef6b57f58c4';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_x64_linux_hotspot_8u265b01.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 16 Oct 2020 23:40:32 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
```

-	Layers:
	-	`sha256:a25fe36305380fa444fa6bd15b622145ff6076e5b6f81168d6cb4c9fee725863`  
		Last Modified: Fri, 25 Sep 2020 08:25:35 GMT  
		Size: 27.2 MB (27160123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326fa3abf0610ea05b9deb392e05c6c86a7afed0c119987a8d920a2a8dceaffc`  
		Last Modified: Fri, 25 Sep 2020 22:49:32 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1b87601e0a324569be2cebc4c0b9981bd53925a9bee894fad57c93f9bd3d01`  
		Last Modified: Fri, 25 Sep 2020 22:49:32 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250393351fede70cb4e53b883fec87230871034c7a674b086131927fb87c1dd0`  
		Last Modified: Fri, 16 Oct 2020 23:48:05 GMT  
		Size: 15.9 MB (15882930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92bfc682ac358b4db32a516bfe980c062f8e03c9df681056f0c29c8a4094761b`  
		Last Modified: Fri, 16 Oct 2020 23:48:21 GMT  
		Size: 103.8 MB (103842390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:8u265-b01-jdk-hotspot-bionic` - linux; ppc64le

```console
$ docker pull adoptopenjdk@sha256:f00d9fe9dd878fdbec5db34e631e90d71e0ab8ac8f1125372e7fae26bc5ad68d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.4 MB (151360158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8a1d9745532a74db42c6ed7fa480742a10a03d5595bd2f33a0cf6e7580f84b8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 25 Sep 2020 23:53:28 GMT
ADD file:5479628763eb7f8cd884270bc1e9bb40ce39f1fb3427e863b086511696fa8107 in / 
# Fri, 25 Sep 2020 23:53:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 23:54:03 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 23:54:24 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 23:54:31 GMT
CMD ["/bin/bash"]
# Sat, 17 Oct 2020 21:53:08 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 17 Oct 2020 21:55:52 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 17 Oct 2020 21:56:02 GMT
ENV JAVA_VERSION=jdk8u265-b01
# Sun, 18 Oct 2020 10:17:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='87d16dac293d2a9abbb559a277bfaded702f28d1bfdc526f8613bb9cfed84a12';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_aarch64_linux_hotspot_8u265b01.tar.gz';          ;;        armhf|armv7l)          ESUM='dc3405aab81f422b7721f665c76371bd7b03c291eea89cd110a82d8bcf07809a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_arm_linux_hotspot_8u265b01.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7bbb9d76458ee29bc5e2458b32a91b8c032ecffe6cb8500734ca41d2d8f5c9f3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u265b01.tar.gz';          ;;        s390x)          ESUM='aca50f02d59169cb428d54501846b518edc9fff6a6f428459c72b4faa2b4abb0';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_s390x_linux_hotspot_8u265b01.tar.gz';          ;;        amd64|x86_64)          ESUM='1285da6278f2d38a790a21148d7e683f20de0799c44b937043830ef6b57f58c4';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_x64_linux_hotspot_8u265b01.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sun, 18 Oct 2020 10:17:47 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
```

-	Layers:
	-	`sha256:af5e190551614a549619ca2cb11a237bf566e7b0942eac80adaf05e21644ad12`  
		Last Modified: Sat, 26 Sep 2020 00:06:58 GMT  
		Size: 33.3 MB (33278058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9dd7d43fa9f545a3f69e66ff00d1a2773213cdfc18d0c99a71bb1c40bbb1f8c`  
		Last Modified: Sat, 26 Sep 2020 00:06:13 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1feb93b9aa176877a7ec845345f281fe28c37605e03363dd0fa489bf0bf10ee`  
		Last Modified: Sat, 26 Sep 2020 00:06:13 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552ff917e16f44b016f2a729c4f39d038bb390da36dbe4f02681940c113b6530`  
		Last Modified: Sat, 17 Oct 2020 22:27:52 GMT  
		Size: 17.2 MB (17189876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b824efe7a8c1961398d14ae2727bc5c61101a60293bf72873546464d67f44ec7`  
		Last Modified: Sun, 18 Oct 2020 10:38:26 GMT  
		Size: 100.9 MB (100891186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:8u265-b01-jdk-hotspot-bionic` - linux; s390x

```console
$ docker pull adoptopenjdk@sha256:297e43e2d704449404ecb8d4ea201bd9ce8148f7586c29ac12094bba6a2fc05e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141787917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9320827176d2cc46d4e7399f9ab9d1bc35293fa02dc1cbf1aab0d14eee10380`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 25 Sep 2020 22:45:02 GMT
ADD file:75a340db285344d2b73beb3a182ed84860806a24c60211a38673223771f3a236 in / 
# Fri, 25 Sep 2020 22:45:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:45:05 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:45:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:45:06 GMT
CMD ["/bin/bash"]
# Fri, 16 Oct 2020 23:41:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Oct 2020 23:41:49 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Oct 2020 23:41:50 GMT
ENV JAVA_VERSION=jdk8u265-b01
# Fri, 16 Oct 2020 23:41:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='87d16dac293d2a9abbb559a277bfaded702f28d1bfdc526f8613bb9cfed84a12';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_aarch64_linux_hotspot_8u265b01.tar.gz';          ;;        armhf|armv7l)          ESUM='dc3405aab81f422b7721f665c76371bd7b03c291eea89cd110a82d8bcf07809a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_arm_linux_hotspot_8u265b01.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7bbb9d76458ee29bc5e2458b32a91b8c032ecffe6cb8500734ca41d2d8f5c9f3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u265b01.tar.gz';          ;;        s390x)          ESUM='aca50f02d59169cb428d54501846b518edc9fff6a6f428459c72b4faa2b4abb0';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_s390x_linux_hotspot_8u265b01.tar.gz';          ;;        amd64|x86_64)          ESUM='1285da6278f2d38a790a21148d7e683f20de0799c44b937043830ef6b57f58c4';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_x64_linux_hotspot_8u265b01.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 16 Oct 2020 23:42:01 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
```

-	Layers:
	-	`sha256:732bed7484b5f127215d82f35831f5772590e5ecc6ed87ef443cc676c98f42d2`  
		Last Modified: Fri, 25 Sep 2020 22:46:01 GMT  
		Size: 27.3 MB (27271534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bb6c28c689be61792f7fa1899196720d036ea4299e73875ca612710dc3559c8`  
		Last Modified: Fri, 25 Sep 2020 22:45:58 GMT  
		Size: 842.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dfea11aa8b7ef661ad1c7d3cd0c8bdcbd6e60a57793e9e29ab227546c8dd150`  
		Last Modified: Fri, 25 Sep 2020 22:45:58 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8118856a9c0f89fe93cd7e7a824bb6a455059ec68963a679a9ba35ce62e5043f`  
		Last Modified: Sat, 17 Oct 2020 00:01:43 GMT  
		Size: 15.8 MB (15759355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00c76c8055fce9a244040cbcd62ed89218d153ec921603762c7b1811555e0c06`  
		Last Modified: Sat, 17 Oct 2020 00:01:47 GMT  
		Size: 98.8 MB (98756000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
