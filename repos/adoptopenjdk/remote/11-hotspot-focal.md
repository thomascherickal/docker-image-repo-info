## `adoptopenjdk:11-hotspot-focal`

```console
$ docker pull adoptopenjdk@sha256:04686bea3796b204e177080bae38b09f24b23216b5bccf8dfe0f12799f81a226
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `adoptopenjdk:11-hotspot-focal` - linux; amd64

```console
$ docker pull adoptopenjdk@sha256:ae78596739183ba9a47bd181f5384594ed3a492105e8411bdbdbdd680b230c1e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.6 MB (239578802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f19d61596eeef811be31cfa5dd2d673603c0302a8140c4d7faa294ce7a8ecef0`
-	Default Command: `["jshell"]`

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
# Fri, 26 Mar 2021 09:58:33 GMT
ENV JAVA_VERSION=jdk-11.0.10+9
# Fri, 26 Mar 2021 09:58:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='420c5d1e5dc66b2ed7dedd30a7bdf94bfaed10d5e1b07dc579722bf60a8114a9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.10_9.tar.gz';          ;;        armhf|armv7l)          ESUM='34908da9c200f5ef71b8766398b79fd166f8be44d87f97510667698b456c8d44';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jdk_arm_linux_hotspot_11.0.10_9.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='e1d130a284f0881893711f17df83198d320c16f807de823c788407af019b356b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.10_9.tar.gz';          ;;        s390x)          ESUM='b55e5d774bcec96b7e6ffc8178a17914ab151414f7048abab3afe3c2febb9a20';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.10_9.tar.gz';          ;;        amd64|x86_64)          ESUM='ae78aa45f84642545c01e8ef786dfd700d2226f8b12881c844d6a1f71789cb99';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jdk_x64_linux_hotspot_11.0.10_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 26 Mar 2021 09:58:44 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 09:58:44 GMT
CMD ["jshell"]
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
	-	`sha256:5a66377148b2e3d520438a6e7f67f50442ca81b6fad55218600e946d8bacbb40`  
		Last Modified: Fri, 26 Mar 2021 10:10:19 GMT  
		Size: 195.0 MB (194975288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:11-hotspot-focal` - linux; arm variant v7

```console
$ docker pull adoptopenjdk@sha256:09297f1a0b89afc7d66fc52ebd4151d75583eeb503af6cbb8577afd2c62d1855
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.3 MB (222324616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:112c4f88abe4dce768f028c19662738d0b79d678b08567fa4de27fab89426d95`
-	Default Command: `["jshell"]`

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
# Fri, 26 Mar 2021 10:01:42 GMT
ENV JAVA_VERSION=jdk-11.0.10+9
# Fri, 26 Mar 2021 10:02:03 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='420c5d1e5dc66b2ed7dedd30a7bdf94bfaed10d5e1b07dc579722bf60a8114a9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.10_9.tar.gz';          ;;        armhf|armv7l)          ESUM='34908da9c200f5ef71b8766398b79fd166f8be44d87f97510667698b456c8d44';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jdk_arm_linux_hotspot_11.0.10_9.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='e1d130a284f0881893711f17df83198d320c16f807de823c788407af019b356b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.10_9.tar.gz';          ;;        s390x)          ESUM='b55e5d774bcec96b7e6ffc8178a17914ab151414f7048abab3afe3c2febb9a20';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.10_9.tar.gz';          ;;        amd64|x86_64)          ESUM='ae78aa45f84642545c01e8ef786dfd700d2226f8b12881c844d6a1f71789cb99';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jdk_x64_linux_hotspot_11.0.10_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 26 Mar 2021 10:02:06 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 10:02:06 GMT
CMD ["jshell"]
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
	-	`sha256:30960e9cf83df11b16b3a171633a448f76b7e12629782b20f81a3739b282f97b`  
		Last Modified: Fri, 26 Mar 2021 10:05:37 GMT  
		Size: 183.4 MB (183377203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:11-hotspot-focal` - linux; arm64 variant v8

```console
$ docker pull adoptopenjdk@sha256:333f648c7cfede36ba40405df86327c779113392ba87d779026ff979cb86a9d1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.8 MB (234802587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a028640860bb677010e2d124f5f6fd2451b21dd173a6502eb1c5cd86925b7339`
-	Default Command: `["jshell"]`

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
# Fri, 26 Mar 2021 12:53:10 GMT
ENV JAVA_VERSION=jdk-11.0.10+9
# Fri, 26 Mar 2021 12:53:27 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='420c5d1e5dc66b2ed7dedd30a7bdf94bfaed10d5e1b07dc579722bf60a8114a9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.10_9.tar.gz';          ;;        armhf|armv7l)          ESUM='34908da9c200f5ef71b8766398b79fd166f8be44d87f97510667698b456c8d44';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jdk_arm_linux_hotspot_11.0.10_9.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='e1d130a284f0881893711f17df83198d320c16f807de823c788407af019b356b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.10_9.tar.gz';          ;;        s390x)          ESUM='b55e5d774bcec96b7e6ffc8178a17914ab151414f7048abab3afe3c2febb9a20';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.10_9.tar.gz';          ;;        amd64|x86_64)          ESUM='ae78aa45f84642545c01e8ef786dfd700d2226f8b12881c844d6a1f71789cb99';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jdk_x64_linux_hotspot_11.0.10_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 26 Mar 2021 12:53:30 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 12:53:31 GMT
CMD ["jshell"]
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
	-	`sha256:9f6d4b4cc16657927f6e55e4b70ed0e379c7bbc5df3eac117aa31e8c4fd886c6`  
		Last Modified: Fri, 26 Mar 2021 13:06:32 GMT  
		Size: 191.7 MB (191730048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:11-hotspot-focal` - linux; ppc64le

```console
$ docker pull adoptopenjdk@sha256:d7713f318b84c89ebd9f37735b7d0867760ed84a14a4624756c2472dd8e7b5be
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.6 MB (227608591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:329c14aaa7870a38cda1504b64814b34ad85a30dd6567a7c9ffcabe876e67819`
-	Default Command: `["jshell"]`

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
# Fri, 26 Mar 2021 15:33:14 GMT
ENV JAVA_VERSION=jdk-11.0.10+9
# Fri, 26 Mar 2021 15:33:50 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='420c5d1e5dc66b2ed7dedd30a7bdf94bfaed10d5e1b07dc579722bf60a8114a9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.10_9.tar.gz';          ;;        armhf|armv7l)          ESUM='34908da9c200f5ef71b8766398b79fd166f8be44d87f97510667698b456c8d44';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jdk_arm_linux_hotspot_11.0.10_9.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='e1d130a284f0881893711f17df83198d320c16f807de823c788407af019b356b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.10_9.tar.gz';          ;;        s390x)          ESUM='b55e5d774bcec96b7e6ffc8178a17914ab151414f7048abab3afe3c2febb9a20';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.10_9.tar.gz';          ;;        amd64|x86_64)          ESUM='ae78aa45f84642545c01e8ef786dfd700d2226f8b12881c844d6a1f71789cb99';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jdk_x64_linux_hotspot_11.0.10_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 26 Mar 2021 15:34:07 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 15:34:13 GMT
CMD ["jshell"]
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
	-	`sha256:c58983b78e6bf11c2241b63e99ca6b2f6323345e3fe282a2f987922c2a68ccf7`  
		Last Modified: Fri, 26 Mar 2021 15:59:42 GMT  
		Size: 177.1 MB (177119004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:11-hotspot-focal` - linux; s390x

```console
$ docker pull adoptopenjdk@sha256:8f2da8ec2193e510f2ff068644f480c393ce58db3970ad25ca1f4db295d1d42e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.9 MB (212916614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08b2f079e4d7e9b981fd1646ebcb29f8743b863a7537592108e39e8b728d77cf`
-	Default Command: `["jshell"]`

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
# Fri, 26 Mar 2021 08:38:46 GMT
ENV JAVA_VERSION=jdk-11.0.10+9
# Fri, 26 Mar 2021 08:39:01 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='420c5d1e5dc66b2ed7dedd30a7bdf94bfaed10d5e1b07dc579722bf60a8114a9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.10_9.tar.gz';          ;;        armhf|armv7l)          ESUM='34908da9c200f5ef71b8766398b79fd166f8be44d87f97510667698b456c8d44';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jdk_arm_linux_hotspot_11.0.10_9.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='e1d130a284f0881893711f17df83198d320c16f807de823c788407af019b356b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.10_9.tar.gz';          ;;        s390x)          ESUM='b55e5d774bcec96b7e6ffc8178a17914ab151414f7048abab3afe3c2febb9a20';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.10_9.tar.gz';          ;;        amd64|x86_64)          ESUM='ae78aa45f84642545c01e8ef786dfd700d2226f8b12881c844d6a1f71789cb99';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jdk_x64_linux_hotspot_11.0.10_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 26 Mar 2021 08:39:10 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 08:39:10 GMT
CMD ["jshell"]
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
	-	`sha256:be37da2ce4dc3bd0fc3a49c6f71274d0a2d2e06462db6b619e3045e754bf5fc7`  
		Last Modified: Fri, 26 Mar 2021 08:51:54 GMT  
		Size: 170.0 MB (169988469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
