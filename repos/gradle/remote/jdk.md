## `gradle:jdk`

```console
$ docker pull gradle@sha256:cafa4002a7a8ae18281a60cb9ee038bc289e70dd39d057b56b4444f498e5c8fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `gradle:jdk` - linux; amd64

```console
$ docker pull gradle@sha256:7023e406fd9c6f8251614275ae3abfe7d999a6d6113b67ee1b651b8597daa6fc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.8 MB (295783397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea7f6562fd875b1c312aa38872fa5d2ab73b4ad606adf15bb12ff63e6cff74d9`
-	Default Command: `["gradle"]`

```dockerfile
# Wed, 16 Sep 2020 22:20:02 GMT
ADD file:84f8ddc4d76e1e867ab084f300cf4c2397bb9e4628d83dc22f4f5e2f6ec670b4 in / 
# Wed, 16 Sep 2020 22:20:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:20:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 22:20:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:20:05 GMT
CMD ["/bin/bash"]
# Wed, 16 Sep 2020 23:34:43 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 16 Sep 2020 23:35:09 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Sep 2020 23:35:10 GMT
ENV JAVA_VERSION=jdk8u262-b10
# Wed, 16 Sep 2020 23:35:22 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7be0b2a4c749a277302a54b456624c076b3a5b990ad502e2a72d803ab31aecab';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10/OpenJDK8U-jdk_aarch64_linux_hotspot_8u262b10.tar.gz';          ;;        armhf|armv7l)          ESUM='dd85ebb9a64916b4b621a23729e3360adb363d430bf1e99e98f25397834d74bd';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10/OpenJDK8U-jdk_arm_linux_hotspot_8u262b10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='d2a16915fb85ba851145c91cda5666cb78f06bf4713a2b3bdce813779ff972c2';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u262b10.tar.gz';          ;;        s390x)          ESUM='a504af6924a095cfb6c392653dccd7299925048c91b399d05efa95a094820120';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10/OpenJDK8U-jdk_s390x_linux_hotspot_8u262b10.tar.gz';          ;;        amd64|x86_64)          ESUM='733755fd649fad6ae91fc083f7e5a5a0b56410fb6ac1815cff29f744b128b1b1';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10/OpenJDK8U-jdk_x64_linux_hotspot_8u262b10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 16 Sep 2020 23:35:22 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 22 Sep 2020 18:26:50 GMT
CMD ["gradle"]
# Tue, 22 Sep 2020 18:26:50 GMT
ENV GRADLE_HOME=/opt/gradle
# Tue, 22 Sep 2020 18:26:51 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Tue, 22 Sep 2020 18:26:51 GMT
VOLUME [/home/gradle/.gradle]
# Tue, 22 Sep 2020 18:26:51 GMT
WORKDIR /home/gradle
# Tue, 22 Sep 2020 18:27:28 GMT
RUN apt-get update     && apt-get install --yes --no-install-recommends         fontconfig         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm -rf /var/lib/apt/lists/*
# Tue, 22 Sep 2020 18:27:29 GMT
ENV GRADLE_VERSION=6.6.1
# Tue, 22 Sep 2020 18:27:29 GMT
ARG GRADLE_DOWNLOAD_SHA256=7873ed5287f47ca03549ab8dcb6dc877ac7f0e3d7b1eb12685161d10080910ac
# Tue, 22 Sep 2020 18:27:34 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=7873ed5287f47ca03549ab8dcb6dc877ac7f0e3d7b1eb12685161d10080910ac
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:5d9821c948472065b3c166b4abc08367160961c9ac4639eb0023670ab4845a6a`  
		Last Modified: Fri, 04 Sep 2020 12:21:34 GMT  
		Size: 26.7 MB (26699608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a610eae58dfceafc0725cb0472249020f75bcc796468615798ee394cbaf86120`  
		Last Modified: Wed, 16 Sep 2020 22:23:01 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a40e0eb9f1408cd0bee02979b33f05689110bc9caba370388d94f73b46a6379a`  
		Last Modified: Wed, 16 Sep 2020 22:23:01 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1854bb447e96b1e5e1051bef627b6167e587e689da45e38caada1a12fd195061`  
		Last Modified: Wed, 16 Sep 2020 23:41:46 GMT  
		Size: 13.9 MB (13875245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:931ccde4bcb384eecd9c1bda798cdc80afd606cfe3a3b75167b09f7a76c818e1`  
		Last Modified: Wed, 16 Sep 2020 23:41:57 GMT  
		Size: 103.7 MB (103736369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be113acf00cba7e53d0623152a99530b5fea8992a39ee1d956d3f67d30c413ed`  
		Last Modified: Tue, 22 Sep 2020 18:30:23 GMT  
		Size: 4.5 KB (4491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd990911746c51e3c983e2ad036101344b60a1087c26ac4f847793d9a163701`  
		Last Modified: Tue, 22 Sep 2020 18:30:34 GMT  
		Size: 48.8 MB (48781183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f8310f6df2ad23604a3c6ffa728700af74a75f6fbf7da0c234dd12fa7c14cf`  
		Last Modified: Tue, 22 Sep 2020 18:30:31 GMT  
		Size: 102.7 MB (102685487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jdk` - linux; arm variant v7

```console
$ docker pull gradle@sha256:75cf002384c19a25cdd5453960a5d8fbcf3a3a398f55e67d60123a26871996a8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.7 MB (279704198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:682ae3c528c9dadf762db46191ccc51b14f3eeddafdd5f89f0981c2d53580fbe`
-	Default Command: `["gradle"]`

```dockerfile
# Wed, 16 Sep 2020 22:28:20 GMT
ADD file:f239c31583452916dd5a653985cbb35d0acb5e97723cb8bcb089ab6dbc009543 in / 
# Wed, 16 Sep 2020 22:28:25 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:28:27 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 22:28:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:28:29 GMT
CMD ["/bin/bash"]
# Wed, 16 Sep 2020 23:21:47 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 16 Sep 2020 23:22:17 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Sep 2020 23:22:19 GMT
ENV JAVA_VERSION=jdk8u262-b10
# Wed, 16 Sep 2020 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7be0b2a4c749a277302a54b456624c076b3a5b990ad502e2a72d803ab31aecab';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10/OpenJDK8U-jdk_aarch64_linux_hotspot_8u262b10.tar.gz';          ;;        armhf|armv7l)          ESUM='dd85ebb9a64916b4b621a23729e3360adb363d430bf1e99e98f25397834d74bd';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10/OpenJDK8U-jdk_arm_linux_hotspot_8u262b10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='d2a16915fb85ba851145c91cda5666cb78f06bf4713a2b3bdce813779ff972c2';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u262b10.tar.gz';          ;;        s390x)          ESUM='a504af6924a095cfb6c392653dccd7299925048c91b399d05efa95a094820120';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10/OpenJDK8U-jdk_s390x_linux_hotspot_8u262b10.tar.gz';          ;;        amd64|x86_64)          ESUM='733755fd649fad6ae91fc083f7e5a5a0b56410fb6ac1815cff29f744b128b1b1';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10/OpenJDK8U-jdk_x64_linux_hotspot_8u262b10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 16 Sep 2020 23:22:32 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 22 Sep 2020 18:06:43 GMT
CMD ["gradle"]
# Tue, 22 Sep 2020 18:06:59 GMT
ENV GRADLE_HOME=/opt/gradle
# Tue, 22 Sep 2020 18:07:55 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Tue, 22 Sep 2020 18:08:04 GMT
VOLUME [/home/gradle/.gradle]
# Tue, 22 Sep 2020 18:08:16 GMT
WORKDIR /home/gradle
# Tue, 22 Sep 2020 18:09:36 GMT
RUN apt-get update     && apt-get install --yes --no-install-recommends         fontconfig         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm -rf /var/lib/apt/lists/*
# Tue, 22 Sep 2020 18:09:53 GMT
ENV GRADLE_VERSION=6.6.1
# Tue, 22 Sep 2020 18:10:01 GMT
ARG GRADLE_DOWNLOAD_SHA256=7873ed5287f47ca03549ab8dcb6dc877ac7f0e3d7b1eb12685161d10080910ac
# Tue, 22 Sep 2020 18:10:46 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=7873ed5287f47ca03549ab8dcb6dc877ac7f0e3d7b1eb12685161d10080910ac
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:46d8d5151783740c4f70c11c624110a72d6b7d8493331685c23eb44a666f962c`  
		Last Modified: Mon, 07 Sep 2020 15:50:39 GMT  
		Size: 22.3 MB (22279228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb0959cf6d665929dbf2838b855f0075660add7f1c3faf5448a40700196e90b0`  
		Last Modified: Wed, 16 Sep 2020 22:30:31 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1764331539d248c00080a27564305167245f13addfdedad6507d51963b39257c`  
		Last Modified: Wed, 16 Sep 2020 22:30:31 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ed116b49dce41fa6cbbd3367cdb4663c98e07b7ec576f5a34f22773eb4b1fe`  
		Last Modified: Wed, 16 Sep 2020 23:25:56 GMT  
		Size: 12.8 MB (12817152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa20d14114d4afa08e723d58461dcbe16cd11ceb0508c5914a2d0a6689738572`  
		Last Modified: Wed, 16 Sep 2020 23:26:11 GMT  
		Size: 98.2 MB (98179068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab64e96634635be9dd3bd83f899554cc4083c4d0da01144846ed3bd4aeb2043e`  
		Last Modified: Tue, 22 Sep 2020 18:28:44 GMT  
		Size: 4.5 KB (4507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2ec73fc6c74349e3ce280b897a402f0f6f33e86cd47e2687e9f23d0ee6c14ca`  
		Last Modified: Tue, 22 Sep 2020 18:28:59 GMT  
		Size: 43.7 MB (43737579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa492b6a79df887340515c8ce77a49fad2346ddf1442e51bd4dd5e2bd61ef875`  
		Last Modified: Tue, 22 Sep 2020 18:29:01 GMT  
		Size: 102.7 MB (102685622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jdk` - linux; arm64 variant v8

```console
$ docker pull gradle@sha256:b415b666c650ba58cb1bcac7d8ea6799f8a894e85bb51e8cb9ca4b44417c079b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.9 MB (289887920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a705a061db05bf67417f09e4fe48d260afa6b2b84186a59b99a43feeb8bbc4e`
-	Default Command: `["gradle"]`

```dockerfile
# Wed, 16 Sep 2020 23:16:37 GMT
ADD file:9eedc88c2028d53a81210b52c98121dddea7e30ecfbd4d11d2a1b2bdc94a0102 in / 
# Wed, 16 Sep 2020 23:16:39 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 23:16:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 23:16:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 23:16:44 GMT
CMD ["/bin/bash"]
# Wed, 16 Sep 2020 23:25:40 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 16 Sep 2020 23:26:07 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Sep 2020 23:26:08 GMT
ENV JAVA_VERSION=jdk8u262-b10
# Wed, 16 Sep 2020 23:26:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7be0b2a4c749a277302a54b456624c076b3a5b990ad502e2a72d803ab31aecab';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10/OpenJDK8U-jdk_aarch64_linux_hotspot_8u262b10.tar.gz';          ;;        armhf|armv7l)          ESUM='dd85ebb9a64916b4b621a23729e3360adb363d430bf1e99e98f25397834d74bd';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10/OpenJDK8U-jdk_arm_linux_hotspot_8u262b10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='d2a16915fb85ba851145c91cda5666cb78f06bf4713a2b3bdce813779ff972c2';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u262b10.tar.gz';          ;;        s390x)          ESUM='a504af6924a095cfb6c392653dccd7299925048c91b399d05efa95a094820120';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10/OpenJDK8U-jdk_s390x_linux_hotspot_8u262b10.tar.gz';          ;;        amd64|x86_64)          ESUM='733755fd649fad6ae91fc083f7e5a5a0b56410fb6ac1815cff29f744b128b1b1';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10/OpenJDK8U-jdk_x64_linux_hotspot_8u262b10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 16 Sep 2020 23:26:18 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 22 Sep 2020 18:51:25 GMT
CMD ["gradle"]
# Tue, 22 Sep 2020 18:51:28 GMT
ENV GRADLE_HOME=/opt/gradle
# Tue, 22 Sep 2020 18:51:32 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Tue, 22 Sep 2020 18:51:37 GMT
VOLUME [/home/gradle/.gradle]
# Tue, 22 Sep 2020 18:51:38 GMT
WORKDIR /home/gradle
# Tue, 22 Sep 2020 18:52:33 GMT
RUN apt-get update     && apt-get install --yes --no-install-recommends         fontconfig         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm -rf /var/lib/apt/lists/*
# Tue, 22 Sep 2020 18:52:39 GMT
ENV GRADLE_VERSION=6.6.1
# Tue, 22 Sep 2020 18:52:40 GMT
ARG GRADLE_DOWNLOAD_SHA256=7873ed5287f47ca03549ab8dcb6dc877ac7f0e3d7b1eb12685161d10080910ac
# Tue, 22 Sep 2020 18:52:59 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=7873ed5287f47ca03549ab8dcb6dc877ac7f0e3d7b1eb12685161d10080910ac
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:e2d8ee3976bc7c15c8a5279cdf0249b7e41b2a489771330d0f7affb26dd7acfb`  
		Last Modified: Fri, 04 Sep 2020 00:25:25 GMT  
		Size: 23.7 MB (23722305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5007857f7b9b52d6efdfea9e086e6eaf35519130ff97bfe89970353f0ae53f13`  
		Last Modified: Wed, 16 Sep 2020 23:18:23 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43927e60f12d8b877ded6af5048b2ac5753fe78caba77a6bbbece4f98559b672`  
		Last Modified: Wed, 16 Sep 2020 23:18:22 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349d5fbbdf46d60d5864e631278bb555a928a5b16e534b20cd8b72e4671fce7b`  
		Last Modified: Wed, 16 Sep 2020 23:29:27 GMT  
		Size: 13.3 MB (13284762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc2d15824d04ec922152daee45ff5b735fbb11f34788055ed48eb14983ea888`  
		Last Modified: Wed, 16 Sep 2020 23:29:41 GMT  
		Size: 103.9 MB (103874639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6388dabf94cf27d0dda2bf38b2f3397d02013374e8d0e12dd12a9f3d3467b2f2`  
		Last Modified: Tue, 22 Sep 2020 19:01:48 GMT  
		Size: 4.5 KB (4525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad4c2fd0a651825a785296b28a4badb5c05fa52a96a799edbdc5621613d97f8`  
		Last Modified: Tue, 22 Sep 2020 19:02:04 GMT  
		Size: 46.3 MB (46314976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4253dbe0f6af4ee6b1359d6afdeb3d48ecd9533991965ee3579cd8094e06c11f`  
		Last Modified: Tue, 22 Sep 2020 19:02:20 GMT  
		Size: 102.7 MB (102685679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jdk` - linux; ppc64le

```console
$ docker pull gradle@sha256:155431179857105f81de8c969eee2824d3725450a2a5f22872e2bc98c4a15e66
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.3 MB (305349413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a82e7fb953abc05f300086199b407f10ddaa4e43356f62a9f6b8923596172834`
-	Default Command: `["gradle"]`

```dockerfile
# Wed, 19 Aug 2020 21:14:04 GMT
ADD file:4954b2b03fa4bd48fabecbc1facd6d05808f55a143012aca45648ab2f767042a in / 
# Wed, 19 Aug 2020 21:14:14 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:14:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:14:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:14:32 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:22:13 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 19 Aug 2020 22:25:23 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:25:28 GMT
ENV JAVA_VERSION=jdk8u262-b10
# Wed, 19 Aug 2020 22:25:52 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7be0b2a4c749a277302a54b456624c076b3a5b990ad502e2a72d803ab31aecab';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10/OpenJDK8U-jdk_aarch64_linux_hotspot_8u262b10.tar.gz';          ;;        armhf|armv7l)          ESUM='dd85ebb9a64916b4b621a23729e3360adb363d430bf1e99e98f25397834d74bd';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10/OpenJDK8U-jdk_arm_linux_hotspot_8u262b10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='d2a16915fb85ba851145c91cda5666cb78f06bf4713a2b3bdce813779ff972c2';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u262b10.tar.gz';          ;;        s390x)          ESUM='a504af6924a095cfb6c392653dccd7299925048c91b399d05efa95a094820120';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10/OpenJDK8U-jdk_s390x_linux_hotspot_8u262b10.tar.gz';          ;;        amd64|x86_64)          ESUM='733755fd649fad6ae91fc083f7e5a5a0b56410fb6ac1815cff29f744b128b1b1';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10/OpenJDK8U-jdk_x64_linux_hotspot_8u262b10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 22:25:58 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 20 Aug 2020 02:52:58 GMT
CMD ["gradle"]
# Thu, 20 Aug 2020 02:53:01 GMT
ENV GRADLE_HOME=/opt/gradle
# Thu, 20 Aug 2020 02:53:08 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Thu, 20 Aug 2020 02:53:12 GMT
VOLUME [/home/gradle/.gradle]
# Thu, 20 Aug 2020 02:53:15 GMT
WORKDIR /home/gradle
# Thu, 20 Aug 2020 02:54:35 GMT
RUN apt-get update     && apt-get install --yes --no-install-recommends         fontconfig         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Aug 2020 19:18:46 GMT
ENV GRADLE_VERSION=6.6.1
# Wed, 26 Aug 2020 19:18:57 GMT
ARG GRADLE_DOWNLOAD_SHA256=7873ed5287f47ca03549ab8dcb6dc877ac7f0e3d7b1eb12685161d10080910ac
# Wed, 26 Aug 2020 19:19:34 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=7873ed5287f47ca03549ab8dcb6dc877ac7f0e3d7b1eb12685161d10080910ac
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:23e4ce51557a90638716607f36b99292ea21b3e246ef66f83934e1eadb095632`  
		Last Modified: Mon, 10 Aug 2020 15:49:13 GMT  
		Size: 30.4 MB (30408877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b20479dd2a1972abd69e09a781025590f55fcbe8bef98a35b1067dceff85d60`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 35.2 KB (35223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3107678818d326669afdd9fcce37d6b61613c2103e889ff7e019515b97ade1d`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a571510b31b5805e20c811dcbb2413f66118e4be6a44a54c430826d8be670e7`  
		Last Modified: Wed, 19 Aug 2020 21:18:49 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a656bb9c393e26fb309b29304e7708385080d6380485fd32eca79e8dc60234`  
		Last Modified: Wed, 19 Aug 2020 22:41:31 GMT  
		Size: 14.5 MB (14518782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbfbce2dbd7216e3709727a63a96718f8af9c5c63810cb683f2628090f8b48a`  
		Last Modified: Wed, 19 Aug 2020 22:41:41 GMT  
		Size: 100.9 MB (100889828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e45606cf9db90d649a532a985c3d4ddc78ccde9ed604a5566cc7f3a29e561088`  
		Last Modified: Thu, 20 Aug 2020 03:09:57 GMT  
		Size: 4.5 KB (4524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d88e3f7f6b7510cb359188b9da12c1ce0201964db1b5fdadb3a0de4f9f62d8a4`  
		Last Modified: Thu, 20 Aug 2020 03:10:12 GMT  
		Size: 56.8 MB (56805417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c424d24962cd01495d0763698fe73caa1960aa41931a4e34eecdbf2bedc0011`  
		Last Modified: Wed, 26 Aug 2020 19:25:48 GMT  
		Size: 102.7 MB (102685717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jdk` - linux; s390x

```console
$ docker pull gradle@sha256:3c2209e8a57dfeb4184f077a8d32266e0b4cab3b942cb45f419b1257cca37da9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.6 MB (288649645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d6770a3807aa4947d6260291e193a150531ee596e3c64e288f64c120ae14937`
-	Default Command: `["gradle"]`

```dockerfile
# Wed, 16 Sep 2020 22:51:22 GMT
ADD file:835d62b9e8aa5985cb778cef4129baec4d3688713202ad55a1fa54bb9daf136e in / 
# Wed, 16 Sep 2020 22:51:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:51:25 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 22:51:26 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:51:26 GMT
CMD ["/bin/bash"]
# Wed, 16 Sep 2020 23:13:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 16 Sep 2020 23:13:32 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Sep 2020 23:13:33 GMT
ENV JAVA_VERSION=jdk8u262-b10
# Wed, 16 Sep 2020 23:13:40 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7be0b2a4c749a277302a54b456624c076b3a5b990ad502e2a72d803ab31aecab';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10/OpenJDK8U-jdk_aarch64_linux_hotspot_8u262b10.tar.gz';          ;;        armhf|armv7l)          ESUM='dd85ebb9a64916b4b621a23729e3360adb363d430bf1e99e98f25397834d74bd';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10/OpenJDK8U-jdk_arm_linux_hotspot_8u262b10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='d2a16915fb85ba851145c91cda5666cb78f06bf4713a2b3bdce813779ff972c2';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u262b10.tar.gz';          ;;        s390x)          ESUM='a504af6924a095cfb6c392653dccd7299925048c91b399d05efa95a094820120';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10/OpenJDK8U-jdk_s390x_linux_hotspot_8u262b10.tar.gz';          ;;        amd64|x86_64)          ESUM='733755fd649fad6ae91fc083f7e5a5a0b56410fb6ac1815cff29f744b128b1b1';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10/OpenJDK8U-jdk_x64_linux_hotspot_8u262b10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 16 Sep 2020 23:13:43 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 22 Sep 2020 17:44:36 GMT
CMD ["gradle"]
# Tue, 22 Sep 2020 17:44:36 GMT
ENV GRADLE_HOME=/opt/gradle
# Tue, 22 Sep 2020 17:44:37 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Tue, 22 Sep 2020 17:44:37 GMT
VOLUME [/home/gradle/.gradle]
# Tue, 22 Sep 2020 17:44:38 GMT
WORKDIR /home/gradle
# Tue, 22 Sep 2020 17:44:54 GMT
RUN apt-get update     && apt-get install --yes --no-install-recommends         fontconfig         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm -rf /var/lib/apt/lists/*
# Tue, 22 Sep 2020 17:44:57 GMT
ENV GRADLE_VERSION=6.6.1
# Tue, 22 Sep 2020 17:44:57 GMT
ARG GRADLE_DOWNLOAD_SHA256=7873ed5287f47ca03549ab8dcb6dc877ac7f0e3d7b1eb12685161d10080910ac
# Tue, 22 Sep 2020 17:45:04 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=7873ed5287f47ca03549ab8dcb6dc877ac7f0e3d7b1eb12685161d10080910ac
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:cedb15d27487fa2e085bee049ff12636f8ba01e63c3bbdc094088e8bb7d8b641`  
		Last Modified: Mon, 07 Sep 2020 15:51:50 GMT  
		Size: 25.4 MB (25370945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc4002d8c6f20fd20eb7aa7e91bfa01443724872a214bb07ad9cf86a810c86ed`  
		Last Modified: Wed, 16 Sep 2020 22:52:22 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a4b15c73b5f07d5d69927632e5a59fb80805da20bc1fabc30f973b5b2ff5805`  
		Last Modified: Wed, 16 Sep 2020 22:52:22 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e9b0ab5887bff45bcb68bdc19ff28f198af83c3c03d9e85a75ae6214c8dade`  
		Last Modified: Wed, 16 Sep 2020 23:18:16 GMT  
		Size: 13.6 MB (13595571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e223b1ef5f81f678719d6cf055699b113be3ac0877c9c01f42bfb9f78c75662`  
		Last Modified: Wed, 16 Sep 2020 23:18:22 GMT  
		Size: 98.8 MB (98755041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d717d89d784b126f306ae47bf7befcc9a52794070f3f9fa9b58ce2a36cb5248`  
		Last Modified: Tue, 22 Sep 2020 17:48:22 GMT  
		Size: 4.5 KB (4524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78eb03797f936eec42991fd8ce524b36bf41a239d6919e21959d55d678ca2a8c`  
		Last Modified: Tue, 22 Sep 2020 17:48:30 GMT  
		Size: 48.2 MB (48236858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f341a22d2a0b0a78a3c3cbd0b0fb11fa15897561a1a293683e7a3ea06e140e0`  
		Last Modified: Tue, 22 Sep 2020 17:48:27 GMT  
		Size: 102.7 MB (102685669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
