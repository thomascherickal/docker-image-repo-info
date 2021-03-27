## `adoptopenjdk:16_36-jre-hotspot-focal`

```console
$ docker pull adoptopenjdk@sha256:1d6cd8166de2b9bcc7964d1972c33d69298afdd6819f1eda2ec3136ac3782dfc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `adoptopenjdk:16_36-jre-hotspot-focal` - linux; amd64

```console
$ docker pull adoptopenjdk@sha256:241fe57bd2570661f0a27a6b579669693014a92449c4b94c5b80345e342c1e06
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.2 MB (94220762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:395f16b7a082f009e73ef8c08a35e28f50d0d2de5a9b66e0decc4dc704d254cd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 25 Mar 2021 22:33:08 GMT
ADD file:a8d2f02fbaddf8cec8e4da320cd03c06435f395e9d454f69954efe422eb6e1ba in / 
# Thu, 25 Mar 2021 22:33:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:10 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:11 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 09:57:14 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 26 Mar 2021 09:58:10 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 09:59:28 GMT
ENV JAVA_VERSION=jdk-16+36
# Fri, 26 Mar 2021 09:59:49 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='947b02342513b085946b2e7c376cc1f1cfe89600bc3d30455160f88d41da3509';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16%2B36/OpenJDK16-jre_aarch64_linux_hotspot_16_36.tar.gz';          ;;        armhf|armv7l)          ESUM='4d3f351a161792779417ee2730413a976258c4cc5f323526f1fbc0cca82aca6e';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16%2B36/OpenJDK16-jre_arm_linux_hotspot_16_36.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='1e5b54ad65a072d924273cade535b1e5da823cebf72b3645a34c32fb141a2401';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16%2B36/OpenJDK16-jre_ppc64le_linux_hotspot_16_36.tar.gz';          ;;        s390x)          ESUM='2033fee36e83c7f9d37455b29c5f49c5ed0ece7c5b05d52bab8e3cdb3e524a77';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16%2B36/OpenJDK16-jre_s390x_linux_hotspot_16_36.tar.gz';          ;;        amd64|x86_64)          ESUM='4aa99cbe5a6838c3ed29fa7aa7bee95c39ddd41e3f7544178dcd257b15a9359e';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16%2B36/OpenJDK16-jre_x64_linux_hotspot_16_36.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 26 Mar 2021 09:59:49 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
```

-	Layers:
	-	`sha256:04a5f4cda3eea2313a61a2f72208342a57ea36a9326dff54f4f26ed47d145c7c`  
		Last Modified: Thu, 25 Mar 2021 22:34:46 GMT  
		Size: 28.6 MB (28569428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff496a88c8ed9b745dab2f00bfbd9013c6d1db198442a6a8683998a29a85458a`  
		Last Modified: Thu, 25 Mar 2021 22:34:37 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce83f459fe7e0bf459d0c222ef3b2ca4d9911f6b0f9aae02c2120561b54ca18`  
		Last Modified: Thu, 25 Mar 2021 22:34:37 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6315e58a4fe1441064bfd504990b519f51bf9e2c0318a7b2f7f18c6dc8c0812`  
		Last Modified: Fri, 26 Mar 2021 10:09:22 GMT  
		Size: 16.0 MB (16033051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1cd5bc82216979477258beb7630648585fa6232204083aadf375be85b8adba9`  
		Last Modified: Fri, 26 Mar 2021 10:12:45 GMT  
		Size: 49.6 MB (49617248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:16_36-jre-hotspot-focal` - linux; arm variant v7

```console
$ docker pull adoptopenjdk@sha256:813828fdbccf3b0cfae85fe3acdd496b92c79f97bfb23ae73d3daa27a80a0d38
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.6 MB (83609801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:167241f03108731c2fcdc2a95eb66e8d0b023c6866819ca721f9fa65535a07fd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 26 Mar 2021 09:13:57 GMT
ADD file:25837d016ed8e3cc502b297c3a904ffacc471c2f9d4ee2cd1131bd652ea28faf in / 
# Fri, 26 Mar 2021 09:14:13 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 26 Mar 2021 09:14:18 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 26 Mar 2021 09:14:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 26 Mar 2021 09:14:24 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 10:00:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 26 Mar 2021 10:01:40 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 10:03:34 GMT
ENV JAVA_VERSION=jdk-16+36
# Fri, 26 Mar 2021 10:04:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='947b02342513b085946b2e7c376cc1f1cfe89600bc3d30455160f88d41da3509';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16%2B36/OpenJDK16-jre_aarch64_linux_hotspot_16_36.tar.gz';          ;;        armhf|armv7l)          ESUM='4d3f351a161792779417ee2730413a976258c4cc5f323526f1fbc0cca82aca6e';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16%2B36/OpenJDK16-jre_arm_linux_hotspot_16_36.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='1e5b54ad65a072d924273cade535b1e5da823cebf72b3645a34c32fb141a2401';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16%2B36/OpenJDK16-jre_ppc64le_linux_hotspot_16_36.tar.gz';          ;;        s390x)          ESUM='2033fee36e83c7f9d37455b29c5f49c5ed0ece7c5b05d52bab8e3cdb3e524a77';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16%2B36/OpenJDK16-jre_s390x_linux_hotspot_16_36.tar.gz';          ;;        amd64|x86_64)          ESUM='4aa99cbe5a6838c3ed29fa7aa7bee95c39ddd41e3f7544178dcd257b15a9359e';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16%2B36/OpenJDK16-jre_x64_linux_hotspot_16_36.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 26 Mar 2021 10:04:20 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
```

-	Layers:
	-	`sha256:c694f656c1b09a697b76142fc22d737f2aa522515c6c1361bf3ccca7ce42f17f`  
		Last Modified: Fri, 26 Mar 2021 09:16:41 GMT  
		Size: 24.0 MB (24047936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb044b09d0cc8ed58817ae0ce7784aafe41640dd7e214d6700b162b10629353`  
		Last Modified: Fri, 26 Mar 2021 09:16:34 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58af11d697841141a01eee137c7fe4870f077615c2691bf041ba9b331e3de7fc`  
		Last Modified: Fri, 26 Mar 2021 09:16:34 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:948a917fe5641fe838416523c30d9d45a09cd56c91dcadd32d7059104e8c0e76`  
		Last Modified: Fri, 26 Mar 2021 10:05:06 GMT  
		Size: 14.9 MB (14898442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b4113c6d3d652b1bd038fffecf9a6e8bdcc8dfc053b45fb7ef703d0cf45af6`  
		Last Modified: Fri, 26 Mar 2021 10:08:34 GMT  
		Size: 44.7 MB (44662388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:16_36-jre-hotspot-focal` - linux; arm64 variant v8

```console
$ docker pull adoptopenjdk@sha256:bac2989215debd1cfdcdfe1ad78d4c49d037c396b936d7c4e76b0c1300a8f59f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.5 MB (91493353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e6218bf63ed460ee9f9ea1b82d1818dab965732bb04506b0cc0a9236a879a1e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 25 Mar 2021 23:22:32 GMT
ADD file:ee49f9e75d7f5923826cf089f2ac0100a27ef7051f10c31b310b573f9c26d91f in / 
# Thu, 25 Mar 2021 23:22:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 23:22:59 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 23:23:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 23:23:13 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 12:52:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 26 Mar 2021 12:53:08 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 12:54:49 GMT
ENV JAVA_VERSION=jdk-16+36
# Fri, 26 Mar 2021 12:55:29 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='947b02342513b085946b2e7c376cc1f1cfe89600bc3d30455160f88d41da3509';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16%2B36/OpenJDK16-jre_aarch64_linux_hotspot_16_36.tar.gz';          ;;        armhf|armv7l)          ESUM='4d3f351a161792779417ee2730413a976258c4cc5f323526f1fbc0cca82aca6e';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16%2B36/OpenJDK16-jre_arm_linux_hotspot_16_36.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='1e5b54ad65a072d924273cade535b1e5da823cebf72b3645a34c32fb141a2401';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16%2B36/OpenJDK16-jre_ppc64le_linux_hotspot_16_36.tar.gz';          ;;        s390x)          ESUM='2033fee36e83c7f9d37455b29c5f49c5ed0ece7c5b05d52bab8e3cdb3e524a77';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16%2B36/OpenJDK16-jre_s390x_linux_hotspot_16_36.tar.gz';          ;;        amd64|x86_64)          ESUM='4aa99cbe5a6838c3ed29fa7aa7bee95c39ddd41e3f7544178dcd257b15a9359e';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16%2B36/OpenJDK16-jre_x64_linux_hotspot_16_36.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 26 Mar 2021 12:55:31 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
```

-	Layers:
	-	`sha256:c5b23ab54a1c0bb81bfc8f1ef83601638d672cc89e3bd3d49290ecfe0834ea2f`  
		Last Modified: Thu, 25 Mar 2021 23:28:04 GMT  
		Size: 27.2 MB (27176798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de628c73ef9a73e299e0e05bce39612341c12b0907fb5a1f8e9a569631ad20c`  
		Last Modified: Thu, 25 Mar 2021 23:27:58 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d61ee5c846071ed2213196ef64402731d6ed75cca1bb954645d89b53db8d2266`  
		Last Modified: Thu, 25 Mar 2021 23:27:58 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109b32077db9d1441f14a783be1bd2c9fc5a8e09d0bb5b1800876186455527c5`  
		Last Modified: Fri, 26 Mar 2021 13:06:09 GMT  
		Size: 15.9 MB (15894704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea99440041fab732cac1f3652a6c89e2a83df40cf0deb754ac086f5eec703734`  
		Last Modified: Fri, 26 Mar 2021 13:09:29 GMT  
		Size: 48.4 MB (48420814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:16_36-jre-hotspot-focal` - linux; ppc64le

```console
$ docker pull adoptopenjdk@sha256:ea116c1ec363cc0bc84a1f6bf4e0e13117aa7228bd9e138747eb34008b25da43
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 MB (95334650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca487dca7c5942122f21cd41971bfea0b1c0a7dc66e25804f2fa2cd03bea47cd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 25 Mar 2021 23:00:23 GMT
ADD file:894e9e1bf10e5da68eb0c51c8d8e6ba7c362e373d183c283393743652f2d4539 in / 
# Thu, 25 Mar 2021 23:01:14 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 23:03:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 23:03:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 23:05:08 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 15:26:41 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 26 Mar 2021 15:30:51 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 15:37:27 GMT
ENV JAVA_VERSION=jdk-16+36
# Fri, 26 Mar 2021 15:38:44 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='947b02342513b085946b2e7c376cc1f1cfe89600bc3d30455160f88d41da3509';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16%2B36/OpenJDK16-jre_aarch64_linux_hotspot_16_36.tar.gz';          ;;        armhf|armv7l)          ESUM='4d3f351a161792779417ee2730413a976258c4cc5f323526f1fbc0cca82aca6e';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16%2B36/OpenJDK16-jre_arm_linux_hotspot_16_36.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='1e5b54ad65a072d924273cade535b1e5da823cebf72b3645a34c32fb141a2401';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16%2B36/OpenJDK16-jre_ppc64le_linux_hotspot_16_36.tar.gz';          ;;        s390x)          ESUM='2033fee36e83c7f9d37455b29c5f49c5ed0ece7c5b05d52bab8e3cdb3e524a77';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16%2B36/OpenJDK16-jre_s390x_linux_hotspot_16_36.tar.gz';          ;;        amd64|x86_64)          ESUM='4aa99cbe5a6838c3ed29fa7aa7bee95c39ddd41e3f7544178dcd257b15a9359e';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16%2B36/OpenJDK16-jre_x64_linux_hotspot_16_36.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 26 Mar 2021 15:38:52 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
```

-	Layers:
	-	`sha256:ec1ca361e0fa55dece5e1f9f35d7a83e9391705d7b279c587fb410dbe4a66d53`  
		Last Modified: Thu, 25 Mar 2021 23:16:25 GMT  
		Size: 33.3 MB (33280097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41281689db31942710bfa208661f2ad79ffd1e6d1a50fc3c3e1648852e93ab8a`  
		Last Modified: Thu, 25 Mar 2021 23:16:14 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c262f70025c1fc7acb1ee7c01b8f5f042df5ac7f313517b64a61cd0978387a1`  
		Last Modified: Thu, 25 Mar 2021 23:16:13 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f1a9fc7248a10c6cb6d831c4f2a71a8d7fd995e60d321a5729f2ba191304cb3`  
		Last Modified: Fri, 26 Mar 2021 15:58:27 GMT  
		Size: 17.2 MB (17208452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceb67ad8287066ee63cf34272b35f60305dba25576e1329954207f12c69606af`  
		Last Modified: Fri, 26 Mar 2021 16:02:20 GMT  
		Size: 44.8 MB (44845063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:16_36-jre-hotspot-focal` - linux; s390x

```console
$ docker pull adoptopenjdk@sha256:2e45db29b7139da631aa1331023024777b700fa68e1a4ca0a64d03e477dc03b1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.0 MB (86956762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dab8c76ea8cc7eae1e7200a5743bce2dde9050e369d6b97fcd85123031760980`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 25 Mar 2021 22:53:41 GMT
ADD file:567b8e3019b11a3d6256710e3fb87d495b2bdfb38831558f40d2f0c77c2ecac6 in / 
# Thu, 25 Mar 2021 22:53:43 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:53:44 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:53:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:53:44 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 08:37:22 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 26 Mar 2021 08:37:54 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 08:40:15 GMT
ENV JAVA_VERSION=jdk-16+36
# Fri, 26 Mar 2021 08:40:52 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='947b02342513b085946b2e7c376cc1f1cfe89600bc3d30455160f88d41da3509';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16%2B36/OpenJDK16-jre_aarch64_linux_hotspot_16_36.tar.gz';          ;;        armhf|armv7l)          ESUM='4d3f351a161792779417ee2730413a976258c4cc5f323526f1fbc0cca82aca6e';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16%2B36/OpenJDK16-jre_arm_linux_hotspot_16_36.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='1e5b54ad65a072d924273cade535b1e5da823cebf72b3645a34c32fb141a2401';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16%2B36/OpenJDK16-jre_ppc64le_linux_hotspot_16_36.tar.gz';          ;;        s390x)          ESUM='2033fee36e83c7f9d37455b29c5f49c5ed0ece7c5b05d52bab8e3cdb3e524a77';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16%2B36/OpenJDK16-jre_s390x_linux_hotspot_16_36.tar.gz';          ;;        amd64|x86_64)          ESUM='4aa99cbe5a6838c3ed29fa7aa7bee95c39ddd41e3f7544178dcd257b15a9359e';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16%2B36/OpenJDK16-jre_x64_linux_hotspot_16_36.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 26 Mar 2021 08:40:57 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
```

-	Layers:
	-	`sha256:cdd1c56b21eb367736255d72ff30100d00f88c340b7b827aa4f7828492f1227a`  
		Last Modified: Thu, 25 Mar 2021 22:54:38 GMT  
		Size: 27.2 MB (27185728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2824c9898d4aa185efc2aa8c843658691335001ff866986cac63fd447bd2c0e0`  
		Last Modified: Thu, 25 Mar 2021 22:54:35 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173cf7c4cdb0bf4d97ba02de2a30dfc5d54c95f0ddcb5d08e1a4d7519432990b`  
		Last Modified: Thu, 25 Mar 2021 22:54:35 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:046d2694f466c6cac7c1c4a3640a0d270a0a9497da294902365018c1e95412bc`  
		Last Modified: Fri, 26 Mar 2021 08:51:13 GMT  
		Size: 15.7 MB (15741382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58831964fe74ac6f0e3f9ac0dc0039a7e34628901c9a83b3e5fe50ba514296e7`  
		Last Modified: Fri, 26 Mar 2021 08:53:24 GMT  
		Size: 44.0 MB (44028617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
