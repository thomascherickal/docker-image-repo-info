## `gradle:jdk8`

```console
$ docker pull gradle@sha256:0ab754b6ec11e7e579940b5a9e000fd81e1f181bc42573e4bc21b2bc24067f1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `gradle:jdk8` - linux; amd64

```console
$ docker pull gradle@sha256:9b001f9a7072329da66c132a5b9c2a257c9d8a6a3407b1bddf0860aff43557b9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.2 MB (293169523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:980a31b74fcf2518e37bbb67e377ecef5045da7a93e52414bb89b3c2509d868e`
-	Default Command: `["gradle"]`

```dockerfile
# Fri, 20 Mar 2020 19:20:20 GMT
ADD file:594fa35cf803361e69d817fc867b6a4069c064ffd20ed50caf42ad9bb11ca999 in / 
# Fri, 20 Mar 2020 19:20:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:20:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:20:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:20:22 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:37:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 20 Mar 2020 19:37:33 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 20 Apr 2020 17:21:50 GMT
ENV JAVA_VERSION=jdk8u252-b09
# Mon, 20 Apr 2020 17:21:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='536bf397d98174b376da9ed49d2f659d65c7310318d8211444f4b7ba7c15e453';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jdk_aarch64_linux_hotspot_8u252b09.tar.gz';          ;;        armhf|armv7l)          ESUM='5b401ad3c9b246281bd6df34b1abaf75e10e5cad9c6b26b55232b016e90e411a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jdk_arm_linux_hotspot_8u252b09.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='55f0453b1d28812154138cf52b17b7acd93b9e55263f1f508f559795d31b2671';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u252b09.tar.gz';          ;;        s390x)          ESUM='db39932666c37718b1c3c62a1adb4f8e9c33258cf15a85ddf9b4d71199edfb1d';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jdk_s390x_linux_hotspot_8u252b09.tar.gz';          ;;        amd64|x86_64)          ESUM='2b59b5282ff32bce7abba8ad6b9fde34c15a98f949ad8ae43e789bbd78fc8862';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jdk_x64_linux_hotspot_8u252b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 20 Apr 2020 17:21:58 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 20 Apr 2020 18:49:57 GMT
CMD ["gradle"]
# Mon, 20 Apr 2020 18:49:58 GMT
ENV GRADLE_HOME=/opt/gradle
# Mon, 20 Apr 2020 18:49:59 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Mon, 20 Apr 2020 18:49:59 GMT
VOLUME [/home/gradle/.gradle]
# Mon, 20 Apr 2020 18:49:59 GMT
WORKDIR /home/gradle
# Mon, 20 Apr 2020 18:50:37 GMT
RUN apt-get update     && apt-get install --yes --no-install-recommends         fontconfig         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm -rf /var/lib/apt/lists/*
# Mon, 20 Apr 2020 18:50:37 GMT
ENV GRADLE_VERSION=6.3
# Mon, 20 Apr 2020 18:50:37 GMT
ARG GRADLE_DOWNLOAD_SHA256=038794feef1f4745c6347107b6726279d1c824f3fc634b60f86ace1e9fbd1768
# Mon, 20 Apr 2020 18:50:43 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=038794feef1f4745c6347107b6726279d1c824f3fc634b60f86ace1e9fbd1768
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:5bed26d33875e6da1d9ff9a1054c5fef3bbeb22ee979e14b72acf72528de007b`  
		Last Modified: Thu, 12 Mar 2020 13:21:29 GMT  
		Size: 26.7 MB (26690587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11b29a9c7306674a9479158c1b4259938af11b97359d9ac02030cc1095e9ed1`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 35.4 KB (35372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930bda195c84cf132344bf38edcad255317382f910503fef234a9ce3bff0f4dd`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78bf9a5ad49e4ae42a83f4995ade4efc096f78fd38299cf05bc041e8cdda2a36`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf7abfeb06800729d4f24d971e8017c537c4fa86368ae0bca66a7b36ca2b4189`  
		Last Modified: Fri, 20 Mar 2020 19:40:17 GMT  
		Size: 13.3 MB (13325178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbe63f973d02241570da79f1a12b4da28d87375688924c8933d1f2ee4551be59`  
		Last Modified: Mon, 20 Apr 2020 17:24:49 GMT  
		Size: 102.7 MB (102690072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eadaa5e9bba87b8f7444828c7fbf09f58629493c3da1c82f260ed9758bd97f07`  
		Last Modified: Mon, 20 Apr 2020 18:53:07 GMT  
		Size: 4.5 KB (4493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66d3dcbb18f80436458e603a0ef7196a40320fa1d06143186ee60efee3ba16cc`  
		Last Modified: Mon, 20 Apr 2020 18:53:20 GMT  
		Size: 48.7 MB (48651932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1149aab4e89d3a9ec778913c01703146ae2fee6d26821c77d7b2c4a17654bc4f`  
		Last Modified: Mon, 20 Apr 2020 18:53:15 GMT  
		Size: 101.8 MB (101770879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jdk8` - linux; ppc64le

```console
$ docker pull gradle@sha256:98825175521566dc8a1cb5f41c31348dfb153e34a61f36f67a4ea30691f9bb32
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.2 MB (305152169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d40bf6a018619acdf3670e5b911376b8bb46f212a087d5fbdcc56172c2a4a1e`
-	Default Command: `["gradle"]`

```dockerfile
# Fri, 20 Mar 2020 19:22:18 GMT
ADD file:226ecdf321a0fde3bea0d6e88db018b3d077f676a1f1e06942217ebb26a02301 in / 
# Fri, 20 Mar 2020 19:22:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:22:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:22:40 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:22:44 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:41:38 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 20 Mar 2020 19:44:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:44:07 GMT
ENV JAVA_VERSION=jdk8u242-b08
# Thu, 26 Mar 2020 18:16:50 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='a2314de7f0120c9bdc69aec2198428a2deeb9ad977fc6801f89d0ec8382d65a5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08/OpenJDK8U-jdk_aarch64_linux_hotspot_jdk8u242-b08.tar.gz';          ;;        armhf|armv7l)          ESUM='ea5f784e70f7c07713dd06214e3c993763857bd31f6de3904971e3032d77388e';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08/OpenJDK8U-jdk_arm_linux_hotspot_8u242b08.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='72f42c2014cb29a2fcd71b1a678af3ed148358a8f9b7d741a5da88cb178d9c53';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u242b08.tar.gz';          ;;        s390x)          ESUM='98f7217dc4acc6bc8b474a2009922b51767d84c045f95a16ee0b9216467ba2de';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08/OpenJDK8U-jdk_s390x_linux_hotspot_8u242b08.tar.gz';          ;;        amd64|x86_64)          ESUM='f39b523c724d0e0047d238eb2bb17a9565a60574cf651206c867ee5fc000ab43';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08/OpenJDK8U-jdk_x64_linux_hotspot_8u242b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 26 Mar 2020 18:16:55 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Mar 2020 18:59:11 GMT
CMD ["gradle"]
# Thu, 26 Mar 2020 18:59:18 GMT
ENV GRADLE_HOME=/opt/gradle
# Thu, 26 Mar 2020 18:59:35 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Thu, 26 Mar 2020 18:59:39 GMT
VOLUME [/home/gradle/.gradle]
# Thu, 26 Mar 2020 18:59:45 GMT
WORKDIR /home/gradle
# Thu, 26 Mar 2020 19:02:07 GMT
RUN apt-get update     && apt-get install --yes --no-install-recommends         fontconfig         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm -rf /var/lib/apt/lists/*
# Thu, 26 Mar 2020 19:02:19 GMT
ENV GRADLE_VERSION=6.3
# Thu, 26 Mar 2020 19:02:24 GMT
ARG GRADLE_DOWNLOAD_SHA256=038794feef1f4745c6347107b6726279d1c824f3fc634b60f86ace1e9fbd1768
# Thu, 26 Mar 2020 19:02:40 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=038794feef1f4745c6347107b6726279d1c824f3fc634b60f86ace1e9fbd1768
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:044eae4257f9584af1a24a5cdb9754c96aea36080e68260ddbabab04827bac00`  
		Last Modified: Mon, 16 Mar 2020 15:38:59 GMT  
		Size: 30.4 MB (30399915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf63a142f3acf0fc36d344bc173f2e1990e692aff0c1237ed6dc96cf38cfb2e`  
		Last Modified: Fri, 20 Mar 2020 19:25:02 GMT  
		Size: 35.2 KB (35212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64d9f5f16809d964026266c73b1c06d3cc0dc517437a91d8639758b80958679`  
		Last Modified: Fri, 20 Mar 2020 19:25:01 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c34444f41441c2f598f5dda94ec1b47ee527ce6e5025d70e5eea41a400d16b1`  
		Last Modified: Fri, 20 Mar 2020 19:25:02 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbaa3d39187779cfab3b684c0f6e3d861528565e584fbb8dc2e72d633644f21c`  
		Last Modified: Fri, 20 Mar 2020 19:52:26 GMT  
		Size: 14.0 MB (13970663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ca215f7ddabebf6e696619a7d88288c6bd262aaeb7cb1d8758242095ff1fc6`  
		Last Modified: Thu, 26 Mar 2020 18:23:01 GMT  
		Size: 102.3 MB (102271834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52840df0377d9c23746d8446eaf2241d272213c260909c8e1e8fd622063915c9`  
		Last Modified: Thu, 26 Mar 2020 19:15:31 GMT  
		Size: 4.5 KB (4539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa5b601c1aa5c218e1d949a2c2832ebae7bbd602731d8570fef589a99bee37bd`  
		Last Modified: Thu, 26 Mar 2020 19:15:46 GMT  
		Size: 56.7 MB (56697973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ec7e475f17e4b70be4bbae3eb1839baff6dc013d823da22bcf597ec4cdfe63`  
		Last Modified: Thu, 26 Mar 2020 19:15:46 GMT  
		Size: 101.8 MB (101770996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jdk8` - linux; s390x

```console
$ docker pull gradle@sha256:81c084a9194b646b891439f9e69b2cb3684f67b1ba55a8c31cd4bdbcef4fcc92
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.2 MB (289151937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23d0ee1628618d21bd6d28b261eb396caec9971165d585088e701651407bd238`
-	Default Command: `["gradle"]`

```dockerfile
# Fri, 20 Mar 2020 18:42:06 GMT
ADD file:9a9f44c69cdb84f93d495237619b0c7b6d02c3a86cac5ff3c3150d1f46fdba17 in / 
# Fri, 20 Mar 2020 18:42:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 18:42:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 18:42:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 18:42:11 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:38:36 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 20 Mar 2020 19:38:50 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:38:51 GMT
ENV JAVA_VERSION=jdk8u242-b08
# Thu, 26 Mar 2020 18:41:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='a2314de7f0120c9bdc69aec2198428a2deeb9ad977fc6801f89d0ec8382d65a5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08/OpenJDK8U-jdk_aarch64_linux_hotspot_jdk8u242-b08.tar.gz';          ;;        armhf|armv7l)          ESUM='ea5f784e70f7c07713dd06214e3c993763857bd31f6de3904971e3032d77388e';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08/OpenJDK8U-jdk_arm_linux_hotspot_8u242b08.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='72f42c2014cb29a2fcd71b1a678af3ed148358a8f9b7d741a5da88cb178d9c53';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u242b08.tar.gz';          ;;        s390x)          ESUM='98f7217dc4acc6bc8b474a2009922b51767d84c045f95a16ee0b9216467ba2de';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08/OpenJDK8U-jdk_s390x_linux_hotspot_8u242b08.tar.gz';          ;;        amd64|x86_64)          ESUM='f39b523c724d0e0047d238eb2bb17a9565a60574cf651206c867ee5fc000ab43';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u242-b08/OpenJDK8U-jdk_x64_linux_hotspot_8u242b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 26 Mar 2020 18:41:49 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Mar 2020 19:44:20 GMT
CMD ["gradle"]
# Thu, 26 Mar 2020 19:44:20 GMT
ENV GRADLE_HOME=/opt/gradle
# Thu, 26 Mar 2020 19:44:22 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Thu, 26 Mar 2020 19:44:23 GMT
VOLUME [/home/gradle/.gradle]
# Thu, 26 Mar 2020 19:44:23 GMT
WORKDIR /home/gradle
# Thu, 26 Mar 2020 19:44:59 GMT
RUN apt-get update     && apt-get install --yes --no-install-recommends         fontconfig         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm -rf /var/lib/apt/lists/*
# Thu, 26 Mar 2020 19:45:07 GMT
ENV GRADLE_VERSION=6.3
# Thu, 26 Mar 2020 19:45:08 GMT
ARG GRADLE_DOWNLOAD_SHA256=038794feef1f4745c6347107b6726279d1c824f3fc634b60f86ace1e9fbd1768
# Thu, 26 Mar 2020 19:45:16 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=038794feef1f4745c6347107b6726279d1c824f3fc634b60f86ace1e9fbd1768
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:345ee2b1c666cad4104ddd5596e148e5c29087184128bb6099412591c696a492`  
		Last Modified: Mon, 16 Mar 2020 15:40:41 GMT  
		Size: 25.4 MB (25364606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6259e081be079eda34010ff7e7c4be7d6d6d927b64ddaa77f8a7f09e30a69229`  
		Last Modified: Fri, 20 Mar 2020 18:42:50 GMT  
		Size: 36.2 KB (36183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d110c40c78a87ebc1e1430d0fb68dd1aec06706c6b2d6d7c82a661f8b74f89a`  
		Last Modified: Fri, 20 Mar 2020 18:42:49 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7af2dd09f8eef8efc3d1215ffd89f820bc87f6dc5cd490b3322258ab8e2466e`  
		Last Modified: Fri, 20 Mar 2020 18:42:55 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46c87faf3e6b36db60f122e065a6d270147409d2b806f06443b02248d6187ad`  
		Last Modified: Fri, 20 Mar 2020 19:42:19 GMT  
		Size: 13.0 MB (13043890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf4c4e765532358f457811cd3ec4ea3e705f927e52adaef337f56e4b1d12908`  
		Last Modified: Thu, 26 Mar 2020 18:46:55 GMT  
		Size: 100.8 MB (100808357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b994cb33d863a45d7f10259de1669dfff1f8b0ab2d5a5f9051a59e33b5394db`  
		Last Modified: Thu, 26 Mar 2020 19:47:55 GMT  
		Size: 4.5 KB (4522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb34e92987c3a7c9cb06df4086dae61a65c69d3fb9a77a4629575bbb1872d11`  
		Last Modified: Thu, 26 Mar 2020 19:48:09 GMT  
		Size: 48.1 MB (48122410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebadaed28b9f1a36bc5fb644644ff046962a9c68343b62c7cb09a9f02f491c47`  
		Last Modified: Thu, 26 Mar 2020 19:48:09 GMT  
		Size: 101.8 MB (101770933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
