## `adoptopenjdk:15-hotspot-focal`

```console
$ docker pull adoptopenjdk@sha256:573e035e4d08d2e7f7b718e1b33f708f0a1c7e824c413328f504aea17b89e1dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `adoptopenjdk:15-hotspot-focal` - linux; amd64

```console
$ docker pull adoptopenjdk@sha256:bc85cef1232dc39e51df44d9a26ca2dab61ed6d7f1822613f514559647f692bc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.7 MB (251653297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d3ee36536c9484ef500ebcf5d531f35b6b8b391e228c6d102c6ccca37f7edf4`
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
# Fri, 26 Mar 2021 09:58:59 GMT
ENV JAVA_VERSION=jdk-15.0.2+7
# Fri, 26 Mar 2021 09:59:11 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6e8b6b037148cf20a284b5b257ec7bfdf9cc31ccc87778d0dfd95a2fddf228d4';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_aarch64_linux_hotspot_15.0.2_7.tar.gz';          ;;        armhf|armv7l)          ESUM='ff39c0380224e419d940382c4d651cb1e6297a794854e0cc459c1fd4973b3368';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_arm_linux_hotspot_15.0.2_7.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='486f2aad94c5580c0b27c9007beebadfccd4677c0bd9565a77ca5c34af5319f9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_ppc64le_linux_hotspot_15.0.2_7.tar.gz';          ;;        s390x)          ESUM='7dc35a8a4ba1ccf6cfe96fcf26e09ed936f1802ca668ca6bf708e2392c35ab6a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_s390x_linux_hotspot_15.0.2_7.tar.gz';          ;;        amd64|x86_64)          ESUM='94f20ca8ea97773571492e622563883b8869438a015d02df6028180dd9acc24d';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_x64_linux_hotspot_15.0.2_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 26 Mar 2021 09:59:11 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 09:59:12 GMT
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
	-	`sha256:7985f5603ad9655ebdc51fe061fd56fc69c69f0dec3dcee430c452ac50092aed`  
		Last Modified: Fri, 26 Mar 2021 10:11:17 GMT  
		Size: 207.0 MB (207049783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:15-hotspot-focal` - linux; arm variant v7

```console
$ docker pull adoptopenjdk@sha256:c41d5d22ea4559ff27200a978ff34c3ba514ff3e6e932953c9f443316d71436a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.7 MB (229667673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96e4be0ff6876483ce15fd65d6c56b20785ed72fe0e93f52f4b72761538667bf`
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
# Fri, 26 Mar 2021 10:02:35 GMT
ENV JAVA_VERSION=jdk-15.0.2+7
# Fri, 26 Mar 2021 10:02:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6e8b6b037148cf20a284b5b257ec7bfdf9cc31ccc87778d0dfd95a2fddf228d4';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_aarch64_linux_hotspot_15.0.2_7.tar.gz';          ;;        armhf|armv7l)          ESUM='ff39c0380224e419d940382c4d651cb1e6297a794854e0cc459c1fd4973b3368';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_arm_linux_hotspot_15.0.2_7.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='486f2aad94c5580c0b27c9007beebadfccd4677c0bd9565a77ca5c34af5319f9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_ppc64le_linux_hotspot_15.0.2_7.tar.gz';          ;;        s390x)          ESUM='7dc35a8a4ba1ccf6cfe96fcf26e09ed936f1802ca668ca6bf708e2392c35ab6a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_s390x_linux_hotspot_15.0.2_7.tar.gz';          ;;        amd64|x86_64)          ESUM='94f20ca8ea97773571492e622563883b8869438a015d02df6028180dd9acc24d';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_x64_linux_hotspot_15.0.2_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 26 Mar 2021 10:03:01 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 10:03:02 GMT
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
	-	`sha256:8825687eeb3f7cfbea57b7ab50197903badf9c127bb6469cf79a6c6b360a3999`  
		Last Modified: Fri, 26 Mar 2021 10:06:49 GMT  
		Size: 190.7 MB (190720260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:15-hotspot-focal` - linux; arm64 variant v8

```console
$ docker pull adoptopenjdk@sha256:15cc016bef69e76212ecbd1e69f74ccf12c1e2d7e259c63e0990ce17ee626d5b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.8 MB (247770333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72d530873fa90443766d05dcb05180fc66c96d7e9a93bd0bb28e0a794e5f78af`
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
# Fri, 26 Mar 2021 12:53:55 GMT
ENV JAVA_VERSION=jdk-15.0.2+7
# Fri, 26 Mar 2021 12:54:11 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6e8b6b037148cf20a284b5b257ec7bfdf9cc31ccc87778d0dfd95a2fddf228d4';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_aarch64_linux_hotspot_15.0.2_7.tar.gz';          ;;        armhf|armv7l)          ESUM='ff39c0380224e419d940382c4d651cb1e6297a794854e0cc459c1fd4973b3368';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_arm_linux_hotspot_15.0.2_7.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='486f2aad94c5580c0b27c9007beebadfccd4677c0bd9565a77ca5c34af5319f9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_ppc64le_linux_hotspot_15.0.2_7.tar.gz';          ;;        s390x)          ESUM='7dc35a8a4ba1ccf6cfe96fcf26e09ed936f1802ca668ca6bf708e2392c35ab6a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_s390x_linux_hotspot_15.0.2_7.tar.gz';          ;;        amd64|x86_64)          ESUM='94f20ca8ea97773571492e622563883b8869438a015d02df6028180dd9acc24d';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_x64_linux_hotspot_15.0.2_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 26 Mar 2021 12:54:14 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 12:54:16 GMT
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
	-	`sha256:162b026fc8cd3adf30957a5aaa129869f165e39461e0df1f9244f2cb5be92d26`  
		Last Modified: Fri, 26 Mar 2021 13:07:45 GMT  
		Size: 204.7 MB (204697794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:15-hotspot-focal` - linux; ppc64le

```console
$ docker pull adoptopenjdk@sha256:9c8cabbce660a2a8da8d89f22375c29b44598bad96bc08167beffb75aebb1cd1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.6 MB (239574737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41531f61316dba8e4a2abda4d51a0bf8263e2ccc58f3fe1de3e3608dbb2a0392`
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
# Fri, 26 Mar 2021 15:35:17 GMT
ENV JAVA_VERSION=jdk-15.0.2+7
# Fri, 26 Mar 2021 15:35:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6e8b6b037148cf20a284b5b257ec7bfdf9cc31ccc87778d0dfd95a2fddf228d4';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_aarch64_linux_hotspot_15.0.2_7.tar.gz';          ;;        armhf|armv7l)          ESUM='ff39c0380224e419d940382c4d651cb1e6297a794854e0cc459c1fd4973b3368';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_arm_linux_hotspot_15.0.2_7.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='486f2aad94c5580c0b27c9007beebadfccd4677c0bd9565a77ca5c34af5319f9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_ppc64le_linux_hotspot_15.0.2_7.tar.gz';          ;;        s390x)          ESUM='7dc35a8a4ba1ccf6cfe96fcf26e09ed936f1802ca668ca6bf708e2392c35ab6a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_s390x_linux_hotspot_15.0.2_7.tar.gz';          ;;        amd64|x86_64)          ESUM='94f20ca8ea97773571492e622563883b8869438a015d02df6028180dd9acc24d';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_x64_linux_hotspot_15.0.2_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 26 Mar 2021 15:36:13 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 15:36:20 GMT
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
	-	`sha256:053789297d7cda1a6abfd76d318aad445d2f82a3549f0532df74b7766a634d4d`  
		Last Modified: Fri, 26 Mar 2021 16:00:47 GMT  
		Size: 189.1 MB (189085150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:15-hotspot-focal` - linux; s390x

```console
$ docker pull adoptopenjdk@sha256:b9526a36dcb9fb6fc4cf94acaf93dd2cfc5e7b39e24607f2bfa54af155652072
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.6 MB (223629846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92124e7194ca85c3c88387fca58ce4956f8591486e3adba5c350c1f8e8d7811b`
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
# Fri, 26 Mar 2021 08:39:31 GMT
ENV JAVA_VERSION=jdk-15.0.2+7
# Fri, 26 Mar 2021 08:39:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6e8b6b037148cf20a284b5b257ec7bfdf9cc31ccc87778d0dfd95a2fddf228d4';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_aarch64_linux_hotspot_15.0.2_7.tar.gz';          ;;        armhf|armv7l)          ESUM='ff39c0380224e419d940382c4d651cb1e6297a794854e0cc459c1fd4973b3368';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_arm_linux_hotspot_15.0.2_7.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='486f2aad94c5580c0b27c9007beebadfccd4677c0bd9565a77ca5c34af5319f9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_ppc64le_linux_hotspot_15.0.2_7.tar.gz';          ;;        s390x)          ESUM='7dc35a8a4ba1ccf6cfe96fcf26e09ed936f1802ca668ca6bf708e2392c35ab6a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_s390x_linux_hotspot_15.0.2_7.tar.gz';          ;;        amd64|x86_64)          ESUM='94f20ca8ea97773571492e622563883b8869438a015d02df6028180dd9acc24d';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_x64_linux_hotspot_15.0.2_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 26 Mar 2021 08:39:52 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 08:39:52 GMT
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
	-	`sha256:e8d5e04bdda654d8803e757c941c3b1e1cc805b097b89b0f1d1afd3569c00d0f`  
		Last Modified: Fri, 26 Mar 2021 08:52:30 GMT  
		Size: 180.7 MB (180701701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
