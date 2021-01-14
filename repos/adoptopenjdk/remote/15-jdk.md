## `adoptopenjdk:15-jdk`

```console
$ docker pull adoptopenjdk@sha256:501c2e74419ab19f2575ded8183825ab72991648c4cd9bcb7354454207b7ff00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `adoptopenjdk:15-jdk` - linux; amd64

```console
$ docker pull adoptopenjdk@sha256:3a1ab5daddc7f89b04e3395a858cc0979c41493b4a4e24a295fb39e090f4696d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.3 MB (252326361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9cc83b30927f17a39564586731d1ab654e86b07bd0dbcbdf14bf20b23cc7dea`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:26 GMT
ADD file:4f15c4475fbafb3fe335e415e3ea1ac416c34af911fcdfe273c5759438aa8eb4 in / 
# Wed, 25 Nov 2020 22:25:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:28 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:29 GMT
CMD ["/bin/bash"]
# Thu, 26 Nov 2020 00:39:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 26 Nov 2020 00:39:43 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 00:40:58 GMT
ENV JAVA_VERSION=jdk-15.0.1+9
# Thu, 26 Nov 2020 00:41:09 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='84398a1566d66ee5a88f3326fb7f0b70504eb510190f8f798bdb386481a3900e';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9/OpenJDK15U-jdk_aarch64_linux_hotspot_15.0.1_9.tar.gz';          ;;        armhf|armv7l)          ESUM='bef5e9f4ab8a87645fa2b3d0ffb9f2b97374caa03cd1296597e8c86e8360d5a2';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9/OpenJDK15U-jdk_arm_linux_hotspot_15.0.1_9.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='bc5347c011025f9830a420f943f52b97ebf0fc642ebff9a25bf465d0a6f3f3b9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9/OpenJDK15U-jdk_ppc64le_linux_hotspot_15.0.1_9.tar.gz';          ;;        s390x)          ESUM='d402e322841abc3c5c8b0352f08d54d6b5c25b7d6f81716401da266bcb1d1ff0';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9/OpenJDK15U-jdk_s390x_linux_hotspot_15.0.1_9.tar.gz';          ;;        amd64|x86_64)          ESUM='61045ecb9434e3320dbc2c597715f9884586b7a18a56d29851b4d4a4d48a2a5e';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9/OpenJDK15U-jdk_x64_linux_hotspot_15.0.1_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 26 Nov 2020 00:41:09 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Nov 2020 00:41:09 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:da7391352a9bb76b292a568c066aa4c3cbae8d494e6a3c68e3c596d34f7c75f8`  
		Last Modified: Fri, 06 Nov 2020 15:20:07 GMT  
		Size: 28.6 MB (28563271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14428a6d4bcdba49a64127900a0691fb00a3f329aced25eb77e3b65646638f8d`  
		Last Modified: Wed, 25 Nov 2020 22:26:39 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2d948710f21ad82dce71743b1654b45acb5c059cf5c19da491582cef6f2601`  
		Last Modified: Wed, 25 Nov 2020 22:26:40 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c07f69a5e5c1c84cfd4566011622ffa52b8d00336abda1dd767c51718498628`  
		Last Modified: Thu, 26 Nov 2020 00:56:19 GMT  
		Size: 16.0 MB (16032786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf986e8585d6f45f288eb693a1d4af5a46a687519fc4766a6fc0a0ed73bb479f`  
		Last Modified: Thu, 26 Nov 2020 00:58:20 GMT  
		Size: 207.7 MB (207729295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:15-jdk` - linux; arm variant v7

```console
$ docker pull adoptopenjdk@sha256:58beb086212c3b8e886c964bcdd50ee57cfd691868b0a31b1ed220153c6cbd71
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.3 MB (230262423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50382dd09d1777a26fe175170f4106cf8ffe24fc33a20d58d3f168feb8c57c6a`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 25 Nov 2020 22:59:41 GMT
ADD file:b2c2bab174379d89834d816a7519d4758ea075a1aa00c6fe305c329089a15d3d in / 
# Wed, 25 Nov 2020 22:59:44 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:59:46 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:59:48 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:59:48 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:18:24 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 25 Nov 2020 23:18:53 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:21:15 GMT
ENV JAVA_VERSION=jdk-15.0.1+9
# Wed, 25 Nov 2020 23:21:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='84398a1566d66ee5a88f3326fb7f0b70504eb510190f8f798bdb386481a3900e';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9/OpenJDK15U-jdk_aarch64_linux_hotspot_15.0.1_9.tar.gz';          ;;        armhf|armv7l)          ESUM='bef5e9f4ab8a87645fa2b3d0ffb9f2b97374caa03cd1296597e8c86e8360d5a2';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9/OpenJDK15U-jdk_arm_linux_hotspot_15.0.1_9.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='bc5347c011025f9830a420f943f52b97ebf0fc642ebff9a25bf465d0a6f3f3b9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9/OpenJDK15U-jdk_ppc64le_linux_hotspot_15.0.1_9.tar.gz';          ;;        s390x)          ESUM='d402e322841abc3c5c8b0352f08d54d6b5c25b7d6f81716401da266bcb1d1ff0';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9/OpenJDK15U-jdk_s390x_linux_hotspot_15.0.1_9.tar.gz';          ;;        amd64|x86_64)          ESUM='61045ecb9434e3320dbc2c597715f9884586b7a18a56d29851b4d4a4d48a2a5e';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9/OpenJDK15U-jdk_x64_linux_hotspot_15.0.1_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 25 Nov 2020 23:21:34 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 25 Nov 2020 23:21:35 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a3a20c5d313f7c8b8e8c7633f51e0ecfd29c87d093315961a38a46da87c3b2be`  
		Last Modified: Fri, 06 Nov 2020 19:09:39 GMT  
		Size: 24.0 MB (24041185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67966bd810cedcb4375094e9af4a7197675edc270d8d16004ab58a8daacbe918`  
		Last Modified: Wed, 25 Nov 2020 23:01:51 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8282ed6897607dd46838e55e3fabf03616b42c2275226012a008da3cf081051`  
		Last Modified: Wed, 25 Nov 2020 23:01:51 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac8cbd0a98818487f6f28b732e1df5a291bc778f42a14ac6be7b4d5eab350bb`  
		Last Modified: Wed, 25 Nov 2020 23:22:35 GMT  
		Size: 14.9 MB (14906111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef2a37741ec8c304f67c133959e3a408c9c6ae6747e5287a38427315d1b02df`  
		Last Modified: Wed, 25 Nov 2020 23:26:03 GMT  
		Size: 191.3 MB (191314087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:15-jdk` - linux; arm64 variant v8

```console
$ docker pull adoptopenjdk@sha256:2c895d8af975a709d6db47a15872d5f572a6a58f3ba7b3e0f71c639a9a5e8e8f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.4 MB (248394963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8d1f4f10930eec166bbe2b8ab64b5421185db557f0d28361762acf9e282de34`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 25 Nov 2020 22:43:12 GMT
ADD file:a9ede6466d698f7a9f018b5121f755f98a7322ba320e16ad207aaf3819ea8bc2 in / 
# Wed, 25 Nov 2020 22:43:15 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:43:17 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:43:19 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:43:20 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:31:44 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 25 Nov 2020 23:32:11 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:34:11 GMT
ENV JAVA_VERSION=jdk-15.0.1+9
# Wed, 25 Nov 2020 23:34:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='84398a1566d66ee5a88f3326fb7f0b70504eb510190f8f798bdb386481a3900e';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9/OpenJDK15U-jdk_aarch64_linux_hotspot_15.0.1_9.tar.gz';          ;;        armhf|armv7l)          ESUM='bef5e9f4ab8a87645fa2b3d0ffb9f2b97374caa03cd1296597e8c86e8360d5a2';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9/OpenJDK15U-jdk_arm_linux_hotspot_15.0.1_9.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='bc5347c011025f9830a420f943f52b97ebf0fc642ebff9a25bf465d0a6f3f3b9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9/OpenJDK15U-jdk_ppc64le_linux_hotspot_15.0.1_9.tar.gz';          ;;        s390x)          ESUM='d402e322841abc3c5c8b0352f08d54d6b5c25b7d6f81716401da266bcb1d1ff0';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9/OpenJDK15U-jdk_s390x_linux_hotspot_15.0.1_9.tar.gz';          ;;        amd64|x86_64)          ESUM='61045ecb9434e3320dbc2c597715f9884586b7a18a56d29851b4d4a4d48a2a5e';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9/OpenJDK15U-jdk_x64_linux_hotspot_15.0.1_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 25 Nov 2020 23:34:34 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 25 Nov 2020 23:34:35 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a970164f39c1a46f71b3615bc9d5b6710832766b530d9179db8e36563f705abb`  
		Last Modified: Fri, 06 Nov 2020 16:25:39 GMT  
		Size: 27.2 MB (27168047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9c66f1fb5a2d6587841797a3b0d4c2d0fd0b7ccd867e55a1314cee2e90ad47d`  
		Last Modified: Wed, 25 Nov 2020 22:44:54 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94362ba2c285844f83a1b1e2dac5217b0426427f8bb809af534b5f4d751e298c`  
		Last Modified: Wed, 25 Nov 2020 22:44:54 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a1a7a5d722a57ef6dd66ff3b0675957c298d427e78f7796b4d320c04511018a`  
		Last Modified: Wed, 25 Nov 2020 23:35:31 GMT  
		Size: 15.9 MB (15900377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f493eab2c340d97b3e5b7f94e217fb6d86338b0693f064f424e43d8a8e7737f4`  
		Last Modified: Wed, 25 Nov 2020 23:38:57 GMT  
		Size: 205.3 MB (205325503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:15-jdk` - linux; ppc64le

```console
$ docker pull adoptopenjdk@sha256:25ba6cce6f5d4ec7390f2de42f0a7d97b1e976a31a5d294f05fa1d2df0b63236
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.3 MB (240273634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:901fdd06534c56d78392a5b259eacdfe80f4f501c060ad224a36647a13c1bf4e`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 25 Nov 2020 22:22:45 GMT
ADD file:349669e872fc8d76ff551a3eb05bb336a7d13ef8d99dc4f7604d54fc263a1a40 in / 
# Wed, 25 Nov 2020 22:23:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:23:19 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:23:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:23:34 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 22:44:43 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 25 Nov 2020 22:46:17 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 22:50:23 GMT
ENV JAVA_VERSION=jdk-15.0.1+9
# Wed, 25 Nov 2020 22:50:51 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='84398a1566d66ee5a88f3326fb7f0b70504eb510190f8f798bdb386481a3900e';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9/OpenJDK15U-jdk_aarch64_linux_hotspot_15.0.1_9.tar.gz';          ;;        armhf|armv7l)          ESUM='bef5e9f4ab8a87645fa2b3d0ffb9f2b97374caa03cd1296597e8c86e8360d5a2';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9/OpenJDK15U-jdk_arm_linux_hotspot_15.0.1_9.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='bc5347c011025f9830a420f943f52b97ebf0fc642ebff9a25bf465d0a6f3f3b9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9/OpenJDK15U-jdk_ppc64le_linux_hotspot_15.0.1_9.tar.gz';          ;;        s390x)          ESUM='d402e322841abc3c5c8b0352f08d54d6b5c25b7d6f81716401da266bcb1d1ff0';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9/OpenJDK15U-jdk_s390x_linux_hotspot_15.0.1_9.tar.gz';          ;;        amd64|x86_64)          ESUM='61045ecb9434e3320dbc2c597715f9884586b7a18a56d29851b4d4a4d48a2a5e';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9/OpenJDK15U-jdk_x64_linux_hotspot_15.0.1_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 25 Nov 2020 22:50:59 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 25 Nov 2020 22:51:04 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:0162c086f3047a91e0409b0f80e741887de3c5e5490b9be62d74a5c054c7d6b0`  
		Last Modified: Mon, 09 Nov 2020 19:03:51 GMT  
		Size: 33.3 MB (33278639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61108ece12882b4998d113ea62b7f4d286877fef610d4aae5b2d2f17d68bf8a4`  
		Last Modified: Wed, 25 Nov 2020 22:27:34 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a92bd8a59839464b3f3c73564e77cb7f1868ac3e96fcc07c1a77b85c51ba1b1`  
		Last Modified: Wed, 25 Nov 2020 22:27:34 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0126056f0b80e5735fc6cef6d439c93c998a81a55e09f213e73e6a7ef1f8cca6`  
		Last Modified: Wed, 25 Nov 2020 23:16:22 GMT  
		Size: 17.2 MB (17210167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d03ec18c03d5c4c248149e2bf853eaa60534f531b43e1bad0835e86339b3edc`  
		Last Modified: Wed, 25 Nov 2020 23:19:26 GMT  
		Size: 189.8 MB (189783785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:15-jdk` - linux; s390x

```console
$ docker pull adoptopenjdk@sha256:316b05e4f8732a023d4085f7531b561a6e6b902e7a88d08167eeec5f219f39c8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.4 MB (224368609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c2168d7c2bcbc803bad38f64a75dec38ea2e02281e521c72423ec9d20be50f2`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 25 Nov 2020 22:45:17 GMT
ADD file:38e2a753398ca5c2c204ddc63d4f5ab0bfb573c7808575be86822459e8d1f812 in / 
# Wed, 25 Nov 2020 22:45:25 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:45:27 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:45:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:45:29 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:16:40 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 25 Nov 2020 23:17:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:20:29 GMT
ENV JAVA_VERSION=jdk-15.0.1+9
# Wed, 25 Nov 2020 23:20:51 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='84398a1566d66ee5a88f3326fb7f0b70504eb510190f8f798bdb386481a3900e';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9/OpenJDK15U-jdk_aarch64_linux_hotspot_15.0.1_9.tar.gz';          ;;        armhf|armv7l)          ESUM='bef5e9f4ab8a87645fa2b3d0ffb9f2b97374caa03cd1296597e8c86e8360d5a2';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9/OpenJDK15U-jdk_arm_linux_hotspot_15.0.1_9.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='bc5347c011025f9830a420f943f52b97ebf0fc642ebff9a25bf465d0a6f3f3b9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9/OpenJDK15U-jdk_ppc64le_linux_hotspot_15.0.1_9.tar.gz';          ;;        s390x)          ESUM='d402e322841abc3c5c8b0352f08d54d6b5c25b7d6f81716401da266bcb1d1ff0';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9/OpenJDK15U-jdk_s390x_linux_hotspot_15.0.1_9.tar.gz';          ;;        amd64|x86_64)          ESUM='61045ecb9434e3320dbc2c597715f9884586b7a18a56d29851b4d4a4d48a2a5e';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9/OpenJDK15U-jdk_x64_linux_hotspot_15.0.1_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 25 Nov 2020 23:21:04 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 25 Nov 2020 23:21:04 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:d777bd6e5a8d1fc6019fe013e0f29e35d2de6a93848ec43ec4b7bcabe67c7d1a`  
		Last Modified: Tue, 10 Nov 2020 00:18:43 GMT  
		Size: 27.2 MB (27206899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fc12e4949d381d9eebf1d32c7547d9d4ebaed0142486b9f416d944257c44c3`  
		Last Modified: Wed, 25 Nov 2020 22:47:22 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15ab9f4a460426ab1fe52891f15e15e67d5b2f246f51b1a6db49e628d6b56f4`  
		Last Modified: Wed, 25 Nov 2020 22:47:21 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf8bd7a5605edf44103ebf135d7e4b32b9e7e95042873ec14d7ab398975f1db`  
		Last Modified: Wed, 25 Nov 2020 23:40:00 GMT  
		Size: 15.8 MB (15761480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf3a72cb50c84ce6e118721e8a755fb2148a8816a8965acb52de3c48e6cd878`  
		Last Modified: Wed, 25 Nov 2020 23:42:03 GMT  
		Size: 181.4 MB (181399198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:15-jdk` - windows version 10.0.17763.1697; amd64

```console
$ docker pull adoptopenjdk@sha256:baed14a99c019e4ce8130a8ff8d18024c436523d2cfd330c42cd0faf4dc2ca3e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2813471263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49aa022bb13710831e7bb1030cdda216a96490a6fecb45e068017e974cc6cbd7`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 22:15:35 GMT
ENV JAVA_VERSION=jdk-15.0.1+9
# Wed, 13 Jan 2021 22:18:10 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9/OpenJDK15U-jdk_x64_windows_hotspot_15.0.1_9.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9/OpenJDK15U-jdk_x64_windows_hotspot_15.0.1_9.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (7254fbe32e77a6cb8c6e36fd1da8ee0744fb323addb0bfda4c32a4d6cf9d22ce) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '7254fbe32e77a6cb8c6e36fd1da8ee0744fb323addb0bfda4c32a4d6cf9d22ce') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 13 Jan 2021 22:18:11 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cec778ebc246eda48b3a5b35a72ea65188a248e5ead895ed44e2a5c7ea680bd`  
		Last Modified: Wed, 13 Jan 2021 23:25:48 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39007f8248f19edcbbc9e232efbf4330769fdf59c32e37db9e5d1aa8f97ab098`  
		Last Modified: Wed, 13 Jan 2021 23:26:20 GMT  
		Size: 377.7 MB (377695741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14b0a6b2ae0a28454c85b04e217f5adced81c56c13bd4ae5bcb9ce06146bfe5`  
		Last Modified: Wed, 13 Jan 2021 23:25:47 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:15-jdk` - windows version 10.0.14393.4169; amd64

```console
$ docker pull adoptopenjdk@sha256:d41fe9e623af5642a4bd1a8fd286f95b3209558cf4f6c87481f306747a0637a5
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6172328170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cecc5570c2dda81a109aac90d60b6ebc8ec9e354d6a98825acc144da25f5f307`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 22:18:18 GMT
ENV JAVA_VERSION=jdk-15.0.1+9
# Wed, 13 Jan 2021 22:21:30 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9/OpenJDK15U-jdk_x64_windows_hotspot_15.0.1_9.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9/OpenJDK15U-jdk_x64_windows_hotspot_15.0.1_9.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (7254fbe32e77a6cb8c6e36fd1da8ee0744fb323addb0bfda4c32a4d6cf9d22ce) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '7254fbe32e77a6cb8c6e36fd1da8ee0744fb323addb0bfda4c32a4d6cf9d22ce') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 13 Jan 2021 22:21:31 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f872b275848bfad3e1d392677f28c74848868bf387c5e3e2590b87a142f77b`  
		Last Modified: Wed, 13 Jan 2021 23:26:52 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f46d8785f38a89e48ba89a2a18904615247d99413fe97b739b2fe026d667d44`  
		Last Modified: Wed, 13 Jan 2021 23:27:22 GMT  
		Size: 378.4 MB (378430680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a165c8d09e7e65c343fac0707cd9a0964d4e49722ec4a5d15e4e1bfcb636cae`  
		Last Modified: Wed, 13 Jan 2021 23:26:52 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
