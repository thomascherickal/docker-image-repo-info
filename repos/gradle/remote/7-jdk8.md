## `gradle:7-jdk8`

```console
$ docker pull gradle@sha256:0c212a52264944b457eda128013134d4a70d8839a5f731a8c834f01d43aeb3d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `gradle:7-jdk8` - linux; amd64

```console
$ docker pull gradle@sha256:d0622c7be23fc8c0f214dbb1e4cfcf0a706b7b4bd730ed98ba774b7e39b75996
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.8 MB (325826220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e25f277ee4baa44356fc0791bffed82dbdcdfb49be03c1de29ccbfd031d124b`
-	Default Command: `["gradle"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:34 GMT
ADD file:5c44a80f547b7d68b550b0e64aef898b361666857abf9a5c8f3f8d0567b8e8e4 in / 
# Fri, 23 Apr 2021 22:21:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:37 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:22:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 23 Apr 2021 23:23:01 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 10 May 2021 18:19:20 GMT
ENV JAVA_VERSION=jdk8u292-b10
# Mon, 10 May 2021 18:19:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='a29edaf66221f7a51353d3f28e1ecf4221268848260417bc562d797e514082a8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jdk_aarch64_linux_hotspot_8u292b10.tar.gz';          ;;        armhf|armv7l)          ESUM='0de107b7df38314c1daab78571383b8b39fdc506790aaef5d870b3e70048881b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jdk_arm_linux_hotspot_8u292b10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7ecf00e57033296fd23201477a64dc13a1356b16a635907e104d079ddb544e4b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u292b10.tar.gz';          ;;        s390x)          ESUM='276a431c79b7e94bc1b1b4fd88523383ae2d635ea67114dfc8a6174267f8fb2c';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jdk_s390x_linux_hotspot_8u292b10.tar.gz';          LIBFFI_SUM='05e456a2e8ad9f20db846ccb96c483235c3243e27025c3e8e8e358411fd48be9';          LIBFFI_URL='http://launchpadlibrarian.net/354371408/libffi6_3.2.1-8_s390x.deb';          curl -LfsSo /tmp/libffi6.deb ${LIBFFI_URL};          echo "${LIBFFI_SUM} /tmp/libffi6.deb" | sha256sum -c -;          apt-get install -y --no-install-recommends /tmp/libffi6.deb;          rm -rf /tmp/libffi6.deb;          ;;        amd64|x86_64)          ESUM='0949505fcf42a1765558048451bb2a22e84b3635b1a31dd6191780eeccaa4ada';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jdk_x64_linux_hotspot_8u292b10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 10 May 2021 18:19:28 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 10 May 2021 18:38:02 GMT
CMD ["gradle"]
# Mon, 10 May 2021 18:38:02 GMT
ENV GRADLE_HOME=/opt/gradle
# Mon, 10 May 2021 18:38:03 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Mon, 10 May 2021 18:38:03 GMT
VOLUME [/home/gradle/.gradle]
# Mon, 10 May 2021 18:38:03 GMT
WORKDIR /home/gradle
# Mon, 10 May 2021 18:39:09 GMT
RUN apt-get update     && apt-get install --yes --no-install-recommends         fontconfig         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm -rf /var/lib/apt/lists/*
# Fri, 14 May 2021 18:19:39 GMT
ENV GRADLE_VERSION=7.0.2
# Fri, 14 May 2021 18:19:39 GMT
ARG GRADLE_DOWNLOAD_SHA256=0e46229820205440b48a5501122002842b82886e76af35f0f3a069243dca4b3c
# Fri, 14 May 2021 18:19:44 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=0e46229820205440b48a5501122002842b82886e76af35f0f3a069243dca4b3c
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:345e3491a907bb7c6f1bdddcf4a94284b8b6ddd77eb7d93f09432b17b20f2bbe`  
		Last Modified: Fri, 16 Apr 2021 15:20:19 GMT  
		Size: 28.5 MB (28539626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57671312ef6fdbecf340e5fed0fb0863350cd806c92b1fdd7978adbd02afc5c3`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9250ddb7d0fa6d13302c7c3e6a0aa40390e42424caed1e5289077ee4054709`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592ec2d7c1370aca6ef48ee1d20fbb3a4c148db400adc5dc575778c681f5dba0`  
		Last Modified: Fri, 23 Apr 2021 23:32:39 GMT  
		Size: 16.0 MB (16034099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc70ed4d3c0718f5d97da384d9a7184e3935863b52ce8f7a37d5fcd2d81b922`  
		Last Modified: Mon, 10 May 2021 18:27:45 GMT  
		Size: 103.6 MB (103551888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2646404da5d1a43ff9d216fde18b083d0e883d0ee10446592f703c7979b89f1`  
		Last Modified: Mon, 10 May 2021 18:48:45 GMT  
		Size: 4.4 KB (4362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:936bc560e474fee4c9ad34dcbebfe7a9ee1f05756aee014fbb67801fac1e2992`  
		Last Modified: Mon, 10 May 2021 18:48:57 GMT  
		Size: 65.6 MB (65610672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1bdd5ad6c6061749544746533ac3aed5917560cf291f2e500f9680065b5852`  
		Last Modified: Fri, 14 May 2021 18:24:26 GMT  
		Size: 112.1 MB (112084535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:7-jdk8` - linux; arm64 variant v8

```console
$ docker pull gradle@sha256:134c713c8004abf24abdb243ef4a7a303b343026aa7239931bf7325f83318399
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.4 MB (323402255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59202e6fbd744293088e13931113811cefe624e51b8556fccde575212cece41f`
-	Default Command: `["gradle"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:51 GMT
ADD file:57e6f432b1329c286e596ded8065bebdfc70a87fae91dd79bd805363ef008e5d in / 
# Fri, 23 Apr 2021 22:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:59 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:13:07 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 23 Apr 2021 23:13:41 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 10 May 2021 17:39:41 GMT
ENV JAVA_VERSION=jdk8u292-b10
# Mon, 10 May 2021 17:39:52 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='a29edaf66221f7a51353d3f28e1ecf4221268848260417bc562d797e514082a8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jdk_aarch64_linux_hotspot_8u292b10.tar.gz';          ;;        armhf|armv7l)          ESUM='0de107b7df38314c1daab78571383b8b39fdc506790aaef5d870b3e70048881b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jdk_arm_linux_hotspot_8u292b10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7ecf00e57033296fd23201477a64dc13a1356b16a635907e104d079ddb544e4b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u292b10.tar.gz';          ;;        s390x)          ESUM='276a431c79b7e94bc1b1b4fd88523383ae2d635ea67114dfc8a6174267f8fb2c';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jdk_s390x_linux_hotspot_8u292b10.tar.gz';          LIBFFI_SUM='05e456a2e8ad9f20db846ccb96c483235c3243e27025c3e8e8e358411fd48be9';          LIBFFI_URL='http://launchpadlibrarian.net/354371408/libffi6_3.2.1-8_s390x.deb';          curl -LfsSo /tmp/libffi6.deb ${LIBFFI_URL};          echo "${LIBFFI_SUM} /tmp/libffi6.deb" | sha256sum -c -;          apt-get install -y --no-install-recommends /tmp/libffi6.deb;          rm -rf /tmp/libffi6.deb;          ;;        amd64|x86_64)          ESUM='0949505fcf42a1765558048451bb2a22e84b3635b1a31dd6191780eeccaa4ada';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jdk_x64_linux_hotspot_8u292b10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 10 May 2021 17:39:53 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 10 May 2021 17:46:25 GMT
CMD ["gradle"]
# Mon, 10 May 2021 17:46:25 GMT
ENV GRADLE_HOME=/opt/gradle
# Mon, 10 May 2021 17:46:28 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Mon, 10 May 2021 17:46:28 GMT
VOLUME [/home/gradle/.gradle]
# Mon, 10 May 2021 17:46:29 GMT
WORKDIR /home/gradle
# Mon, 10 May 2021 17:47:12 GMT
RUN apt-get update     && apt-get install --yes --no-install-recommends         fontconfig         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm -rf /var/lib/apt/lists/*
# Fri, 14 May 2021 18:00:42 GMT
ENV GRADLE_VERSION=7.0.2
# Fri, 14 May 2021 18:00:45 GMT
ARG GRADLE_DOWNLOAD_SHA256=0e46229820205440b48a5501122002842b82886e76af35f0f3a069243dca4b3c
# Fri, 14 May 2021 18:01:05 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=0e46229820205440b48a5501122002842b82886e76af35f0f3a069243dca4b3c
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:80bc30679ac1fd798f3241208c14accd6a364cb8a6224d1127dfb1577d10554f`  
		Last Modified: Fri, 16 Apr 2021 08:25:26 GMT  
		Size: 27.1 MB (27144417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf18fab4cfbf479fa9f8409ad47e2702c63241304c2cdd4c33f2a1633c5f85e`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5979309c983a2adeff352538937475cf961d49c34194fa2aab142effe19ed9c1`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6482171366cbde14bd4de2fe7eade385c2d307e224a008056f39e553b9c93d7`  
		Last Modified: Fri, 23 Apr 2021 23:18:01 GMT  
		Size: 15.9 MB (15895133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:576d59285cbc054a53a31f0b00fd160fbb169bf79b7e46f74c76a76e9f075d10`  
		Last Modified: Mon, 10 May 2021 17:42:42 GMT  
		Size: 103.0 MB (102955983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8569d8251a17dea8912aac53e1e736751929f5b9974f3c928511cc7ae30531f8`  
		Last Modified: Mon, 10 May 2021 18:00:31 GMT  
		Size: 4.4 KB (4362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791c076f58ce86c12a4df41c09a959a9ae5e3f06671da9ee3b0dd63051fb8def`  
		Last Modified: Mon, 10 May 2021 18:00:53 GMT  
		Size: 65.3 MB (65316790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54b3feb9100d5285b574d37bbdb421544f8344502f158e4e477fb9714c92be2`  
		Last Modified: Fri, 14 May 2021 18:13:49 GMT  
		Size: 112.1 MB (112084531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:7-jdk8` - linux; ppc64le

```console
$ docker pull gradle@sha256:70f0f074fb10ba72224baa567a5610172638611e52b2d3c493ff960c6c5b9f4d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.6 MB (337576465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37f1c1e5d13b273f767ae2e5d0a0b4f552d40dc7cf519330aaa9a89a284a9942`
-	Default Command: `["gradle"]`

```dockerfile
# Fri, 23 Apr 2021 22:31:45 GMT
ADD file:ec80070ca931734843261734e9ca18cd45a6130030c1a25abac3268e54776be5 in / 
# Fri, 23 Apr 2021 22:32:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:32:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:32:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:32:38 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 01:16:16 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 24 Apr 2021 01:19:33 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 10 May 2021 18:17:15 GMT
ENV JAVA_VERSION=jdk8u292-b10
# Mon, 10 May 2021 18:17:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='a29edaf66221f7a51353d3f28e1ecf4221268848260417bc562d797e514082a8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jdk_aarch64_linux_hotspot_8u292b10.tar.gz';          ;;        armhf|armv7l)          ESUM='0de107b7df38314c1daab78571383b8b39fdc506790aaef5d870b3e70048881b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jdk_arm_linux_hotspot_8u292b10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7ecf00e57033296fd23201477a64dc13a1356b16a635907e104d079ddb544e4b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u292b10.tar.gz';          ;;        s390x)          ESUM='276a431c79b7e94bc1b1b4fd88523383ae2d635ea67114dfc8a6174267f8fb2c';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jdk_s390x_linux_hotspot_8u292b10.tar.gz';          LIBFFI_SUM='05e456a2e8ad9f20db846ccb96c483235c3243e27025c3e8e8e358411fd48be9';          LIBFFI_URL='http://launchpadlibrarian.net/354371408/libffi6_3.2.1-8_s390x.deb';          curl -LfsSo /tmp/libffi6.deb ${LIBFFI_URL};          echo "${LIBFFI_SUM} /tmp/libffi6.deb" | sha256sum -c -;          apt-get install -y --no-install-recommends /tmp/libffi6.deb;          rm -rf /tmp/libffi6.deb;          ;;        amd64|x86_64)          ESUM='0949505fcf42a1765558048451bb2a22e84b3635b1a31dd6191780eeccaa4ada';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jdk_x64_linux_hotspot_8u292b10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 10 May 2021 18:17:40 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 10 May 2021 18:43:01 GMT
CMD ["gradle"]
# Mon, 10 May 2021 18:43:09 GMT
ENV GRADLE_HOME=/opt/gradle
# Mon, 10 May 2021 18:43:36 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Mon, 10 May 2021 18:43:43 GMT
VOLUME [/home/gradle/.gradle]
# Mon, 10 May 2021 18:43:48 GMT
WORKDIR /home/gradle
# Mon, 10 May 2021 18:47:14 GMT
RUN apt-get update     && apt-get install --yes --no-install-recommends         fontconfig         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm -rf /var/lib/apt/lists/*
# Tue, 11 May 2021 01:22:32 GMT
ENV GRADLE_VERSION=7.0.1
# Tue, 11 May 2021 01:22:38 GMT
ARG GRADLE_DOWNLOAD_SHA256=dccda8aa069563c8ba2f6cdfd0777df0e34a5b4d15138ca8b9757e94f4e8a8cb
# Tue, 11 May 2021 01:23:52 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=dccda8aa069563c8ba2f6cdfd0777df0e34a5b4d15138ca8b9757e94f4e8a8cb
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:8cdb522ceff72cef6133f5b26b5f9eac72760a06a86d5d6b7db34a5dde7b156f`  
		Last Modified: Fri, 23 Apr 2021 22:37:11 GMT  
		Size: 33.3 MB (33255388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21136d6107eea0892211e712ba6b20d15f74a37dd1bde1b2f0802e083e85c183`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a03f1456f472e398050e94cf3ac8873969ce172a153bb511be780fe49403c47`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da07529aeac8fe5c90c5bb8c4f516c9d6fd248cc1daa5fecd137c809bce39bb6`  
		Last Modified: Sat, 24 Apr 2021 01:40:58 GMT  
		Size: 17.2 MB (17209103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0237ceeb0026ed78c6a0fd5c4804f8771caa54748976b27ec07f56b6f7a93f5d`  
		Last Modified: Mon, 10 May 2021 18:34:45 GMT  
		Size: 101.0 MB (101047823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d65fb849a5c531b9958cdf0a67c72c42098979475a7c95030444385e7fdaab`  
		Last Modified: Mon, 10 May 2021 20:12:01 GMT  
		Size: 4.4 KB (4383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b989d563dc3bb04235a3d46b65113845f5a5f98edd011a915e903dc6a211a30`  
		Last Modified: Mon, 10 May 2021 20:13:30 GMT  
		Size: 74.0 MB (73974222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac48451113fe88f02b1e223ba2e6531b1b074ace4a6d3317f275a7617843573`  
		Last Modified: Tue, 11 May 2021 01:45:49 GMT  
		Size: 112.1 MB (112084510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:7-jdk8` - linux; s390x

```console
$ docker pull gradle@sha256:b9863b7a784d4e9ea77a8799941b27e85b1b4d569d4142d384bfcbbef8954778
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.4 MB (318426674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6bfe1316256942479fa53fdc9a1d709302baa9f55408abb373b85945812b3cd`
-	Default Command: `["gradle"]`

```dockerfile
# Fri, 23 Apr 2021 21:45:20 GMT
ADD file:282d950116f923276efabd13c7dc17b942821edb14ffac4b89b9a50bcdf99e17 in / 
# Fri, 23 Apr 2021 21:45:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 21:45:27 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 21:45:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 21:45:29 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 22:03:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 23 Apr 2021 22:04:03 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 10 May 2021 17:41:49 GMT
ENV JAVA_VERSION=jdk8u292-b10
# Mon, 10 May 2021 17:42:16 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='a29edaf66221f7a51353d3f28e1ecf4221268848260417bc562d797e514082a8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jdk_aarch64_linux_hotspot_8u292b10.tar.gz';          ;;        armhf|armv7l)          ESUM='0de107b7df38314c1daab78571383b8b39fdc506790aaef5d870b3e70048881b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jdk_arm_linux_hotspot_8u292b10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7ecf00e57033296fd23201477a64dc13a1356b16a635907e104d079ddb544e4b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u292b10.tar.gz';          ;;        s390x)          ESUM='276a431c79b7e94bc1b1b4fd88523383ae2d635ea67114dfc8a6174267f8fb2c';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jdk_s390x_linux_hotspot_8u292b10.tar.gz';          LIBFFI_SUM='05e456a2e8ad9f20db846ccb96c483235c3243e27025c3e8e8e358411fd48be9';          LIBFFI_URL='http://launchpadlibrarian.net/354371408/libffi6_3.2.1-8_s390x.deb';          curl -LfsSo /tmp/libffi6.deb ${LIBFFI_URL};          echo "${LIBFFI_SUM} /tmp/libffi6.deb" | sha256sum -c -;          apt-get install -y --no-install-recommends /tmp/libffi6.deb;          rm -rf /tmp/libffi6.deb;          ;;        amd64|x86_64)          ESUM='0949505fcf42a1765558048451bb2a22e84b3635b1a31dd6191780eeccaa4ada';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jdk_x64_linux_hotspot_8u292b10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 10 May 2021 17:42:25 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 10 May 2021 18:24:43 GMT
CMD ["gradle"]
# Mon, 10 May 2021 18:24:44 GMT
ENV GRADLE_HOME=/opt/gradle
# Mon, 10 May 2021 18:24:46 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Mon, 10 May 2021 18:24:46 GMT
VOLUME [/home/gradle/.gradle]
# Mon, 10 May 2021 18:24:47 GMT
WORKDIR /home/gradle
# Mon, 10 May 2021 18:25:41 GMT
RUN apt-get update     && apt-get install --yes --no-install-recommends         fontconfig         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm -rf /var/lib/apt/lists/*
# Fri, 14 May 2021 17:43:42 GMT
ENV GRADLE_VERSION=7.0.2
# Fri, 14 May 2021 17:43:42 GMT
ARG GRADLE_DOWNLOAD_SHA256=0e46229820205440b48a5501122002842b82886e76af35f0f3a069243dca4b3c
# Fri, 14 May 2021 17:43:50 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=0e46229820205440b48a5501122002842b82886e76af35f0f3a069243dca4b3c
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:de53239ada2db01e7972c3f6eddcf6729f7cf3102be78e0b41363125ce7c2425`  
		Last Modified: Fri, 23 Apr 2021 21:47:14 GMT  
		Size: 27.1 MB (27136362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12932016d0f51acb5c5e5ba5b420a369401a7df47a219f24680bbc05ffde7e11`  
		Last Modified: Fri, 23 Apr 2021 21:47:10 GMT  
		Size: 840.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46997f76c5876e3274170b667463b3d88475cd696ccbc735d2f63965668673ad`  
		Last Modified: Fri, 23 Apr 2021 21:47:10 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bab416938acf6dd045c9fc9097e5768c61b5899b07d110ab3844f447e12b113`  
		Last Modified: Fri, 23 Apr 2021 22:19:05 GMT  
		Size: 15.7 MB (15741779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb930d43f1888410f23786d5db07d59b3f8ed7e8a3d43751ecb211f774ebf5b0`  
		Last Modified: Mon, 10 May 2021 17:55:24 GMT  
		Size: 98.6 MB (98640816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b33d9dbae6b7166854ceb99639458e5cddaf6dcbf5bea9553cdb34d02bf9b8`  
		Last Modified: Mon, 10 May 2021 18:54:18 GMT  
		Size: 4.4 KB (4363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d660cc5571b24d0e67cc69a531fa44001ca3cb9b3361792bcb7e2a381de1042`  
		Last Modified: Mon, 10 May 2021 18:54:28 GMT  
		Size: 64.8 MB (64817817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2fe9044a57661d84a57520cf84531bdab87be12cd07e9f3f18f4469f739fb19`  
		Last Modified: Fri, 14 May 2021 17:49:12 GMT  
		Size: 112.1 MB (112084511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
