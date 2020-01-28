## `gradle:jre11`

```console
$ docker pull gradle@sha256:c5ea9aaea7373cb6bf3a2fb5a20fb5789f6fce8c86bc6b86e93c6a57f42780e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `gradle:jre11` - linux; amd64

```console
$ docker pull gradle@sha256:55767516f10c843780affd7952a70615a9e34da7baf80eb418cd34114c5cb958
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.1 MB (229102864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9af156165d2ec97e6fd4c24ca0487206d33bb18f2a912541796f27f9584d533d`
-	Default Command: `["gradle"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:31 GMT
ADD file:08e718ed0796013f5957a1be7da3bef6225f3d82d8be0a86a7114e5caad50cbc in / 
# Thu, 16 Jan 2020 01:20:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:44:50 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 16 Jan 2020 01:45:08 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 28 Jan 2020 00:19:44 GMT
ENV JAVA_VERSION=jdk-11.0.6+10
# Tue, 28 Jan 2020 00:20:06 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7ed04ed9ed7271528e7f03490f1fd7dfbbc2d391414bd6fe4dd80ec3bad76d30';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='49231f2c36487b53141ade3f7eb291e2855138b14b1129f9acf435ea9cc0e899';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='bcb3f46cbad742b08c81e922e313549c029f436ac7d91ef3c9bed8e4049d67d2';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='c5a4e69e2be0e3e5f5bb7c759960b20650967d0f571baad4a7f15b2c03bda352';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 28 Jan 2020 00:20:06 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Jan 2020 00:34:16 GMT
CMD ["gradle"]
# Tue, 28 Jan 2020 00:34:16 GMT
ENV GRADLE_HOME=/opt/gradle
# Tue, 28 Jan 2020 00:34:17 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Tue, 28 Jan 2020 00:34:17 GMT
VOLUME [/home/gradle/.gradle]
# Tue, 28 Jan 2020 00:34:17 GMT
WORKDIR /home/gradle
# Tue, 28 Jan 2020 00:34:35 GMT
RUN apt-get update     && apt-get install --yes --no-install-recommends         fontconfig         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm -rf /var/lib/apt/lists/*
# Tue, 28 Jan 2020 00:34:35 GMT
ENV GRADLE_VERSION=6.1.1
# Tue, 28 Jan 2020 00:34:35 GMT
ARG GRADLE_DOWNLOAD_SHA256=9d94e6e4a28ad328072ef6e56bce79a810494ae756751fdcedffdeaf27c093b1
# Tue, 28 Jan 2020 00:34:40 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=9d94e6e4a28ad328072ef6e56bce79a810494ae756751fdcedffdeaf27c093b1
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:5c939e3a4d1097af8d3292ad3a41d3caa846f6333b91f2dd22b972bc2d19c5b5`  
		Last Modified: Mon, 13 Jan 2020 13:21:09 GMT  
		Size: 26.7 MB (26690191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63719cdbe7ae254b453dba06fb446f583b503f2a2c15becc83f8c5bc7a705e0`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 35.4 KB (35366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a861ea6baff71b05cd577478984c3e62cf0177bf74468d0aca551f5fcb891c`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651c9d2d6c4f37c56a221259e033e7e2353b698139c2ff950623ca28d64a9837`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e1a6e1ff3c935882f4005a6063541af139f9244769187488ef236e2052ce19`  
		Last Modified: Thu, 16 Jan 2020 01:48:24 GMT  
		Size: 13.3 MB (13323265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a2f0ff9a40fd1319957e0786e94b776a7b5f272b045ebce29c08e53238f5a5`  
		Last Modified: Tue, 28 Jan 2020 00:23:26 GMT  
		Size: 42.9 MB (42918695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a23fa486a9ed5a6e560a3a68133cdd2626644f99cf780e3a32762f6e2cf75468`  
		Last Modified: Tue, 28 Jan 2020 00:36:46 GMT  
		Size: 4.5 KB (4488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2176502f8b63a823a13a9f603e1dddb57cb45d194fb146e4f3ca9433748eb72`  
		Last Modified: Tue, 28 Jan 2020 00:36:56 GMT  
		Size: 48.6 MB (48646445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d620a970d9cc09720b5eee3e024cac0bb759d79e78395110f7eb32cbf8692e9`  
		Last Modified: Tue, 28 Jan 2020 00:36:53 GMT  
		Size: 97.5 MB (97483403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jre11` - linux; arm64 variant v8

```console
$ docker pull gradle@sha256:6a4bfcd0572a7eeb9e3819e9a0d5225dc1a364351efc2679a392cadb8d1c7b5b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.1 MB (222118894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dcd44a42d49cf207ff15b39c5dbd6301d364998ca4a07bd099b09045e893616`
-	Default Command: `["gradle"]`

```dockerfile
# Thu, 16 Jan 2020 00:40:35 GMT
ADD file:868e3a7e9028dcf197b28fa33d45b368b95d6a4e98cceba6bc9cf2c85daa554a in / 
# Thu, 16 Jan 2020 00:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:40:44 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:40:49 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:40:51 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 00:59:58 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 16 Jan 2020 01:01:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 27 Jan 2020 23:40:14 GMT
ENV JAVA_VERSION=jdk-11.0.6+10
# Mon, 27 Jan 2020 23:40:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7ed04ed9ed7271528e7f03490f1fd7dfbbc2d391414bd6fe4dd80ec3bad76d30';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='49231f2c36487b53141ade3f7eb291e2855138b14b1129f9acf435ea9cc0e899';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='bcb3f46cbad742b08c81e922e313549c029f436ac7d91ef3c9bed8e4049d67d2';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='c5a4e69e2be0e3e5f5bb7c759960b20650967d0f571baad4a7f15b2c03bda352';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 27 Jan 2020 23:40:55 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Jan 2020 23:45:45 GMT
CMD ["gradle"]
# Mon, 27 Jan 2020 23:45:45 GMT
ENV GRADLE_HOME=/opt/gradle
# Mon, 27 Jan 2020 23:45:47 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Mon, 27 Jan 2020 23:45:48 GMT
VOLUME [/home/gradle/.gradle]
# Mon, 27 Jan 2020 23:45:48 GMT
WORKDIR /home/gradle
# Mon, 27 Jan 2020 23:46:21 GMT
RUN apt-get update     && apt-get install --yes --no-install-recommends         fontconfig         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm -rf /var/lib/apt/lists/*
# Mon, 27 Jan 2020 23:46:23 GMT
ENV GRADLE_VERSION=6.1.1
# Mon, 27 Jan 2020 23:46:24 GMT
ARG GRADLE_DOWNLOAD_SHA256=9d94e6e4a28ad328072ef6e56bce79a810494ae756751fdcedffdeaf27c093b1
# Mon, 27 Jan 2020 23:46:30 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=9d94e6e4a28ad328072ef6e56bce79a810494ae756751fdcedffdeaf27c093b1
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:fbdcf4a939bd956d7cd2fd21e684e4e3ca5d9ef60886808b0345bbc2c3b6f18a`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 23.7 MB (23719499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3463cc4abcf9c532fc6f5ad6b6780de967e7a0cadf865674d6dbbeefc9eb349`  
		Last Modified: Thu, 16 Jan 2020 00:43:21 GMT  
		Size: 35.2 KB (35201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf5b492942e45d969f49bd9465095c547ddfa152607f6b5ce9d924fe647f8f8`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7799262edbd86d40847575d269f6f03068dba731519911195aa384ec02ae9702`  
		Last Modified: Thu, 16 Jan 2020 00:43:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd789495d7e9a60c135ebd6aebd36b8364d4f22c79d3a42a45be167c49cd2f09`  
		Last Modified: Thu, 16 Jan 2020 01:03:43 GMT  
		Size: 12.7 MB (12732288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0b046687d673bb7f71d04f52e5bee07da47de4b7ec37abfccb5f9626b3858e`  
		Last Modified: Mon, 27 Jan 2020 23:43:47 GMT  
		Size: 41.9 MB (41945397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7d301b2f80a886a1e9c736e1866be847e29c98810258d75e9b27719ae61ccb`  
		Last Modified: Mon, 27 Jan 2020 23:48:35 GMT  
		Size: 4.5 KB (4529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b634ca139fb52e5793b39aec165b32817704b1ebac81d8e45041b9eaa9572d`  
		Last Modified: Mon, 27 Jan 2020 23:48:52 GMT  
		Size: 46.2 MB (46197437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e907f0676a77b126d88fe6429d7dae1d646a266eb7bb1229acda4f1021d42037`  
		Last Modified: Mon, 27 Jan 2020 23:48:49 GMT  
		Size: 97.5 MB (97483506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jre11` - linux; ppc64le

```console
$ docker pull gradle@sha256:ace309d0da74a9a59e4ddc7680c8bed282d1da64dd83552ef5fbcc9f09312e6d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.2 MB (238172626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08bee23634dae4f846943674201d768005387230f975ac7f0bfe34821153ad9d`
-	Default Command: `["gradle"]`

```dockerfile
# Thu, 16 Jan 2020 01:16:57 GMT
ADD file:9a1a27f07b5eac878569b1a3279d14f876400a0bbb293be818f5554662ac82e9 in / 
# Thu, 16 Jan 2020 01:17:05 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:17:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:17:17 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:17:19 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:43:10 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 16 Jan 2020 01:44:08 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 28 Jan 2020 00:20:37 GMT
ENV JAVA_VERSION=jdk-11.0.6+10
# Tue, 28 Jan 2020 00:21:21 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7ed04ed9ed7271528e7f03490f1fd7dfbbc2d391414bd6fe4dd80ec3bad76d30';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='49231f2c36487b53141ade3f7eb291e2855138b14b1129f9acf435ea9cc0e899';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='bcb3f46cbad742b08c81e922e313549c029f436ac7d91ef3c9bed8e4049d67d2';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='c5a4e69e2be0e3e5f5bb7c759960b20650967d0f571baad4a7f15b2c03bda352';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 28 Jan 2020 00:21:24 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Jan 2020 00:38:28 GMT
CMD ["gradle"]
# Tue, 28 Jan 2020 00:38:30 GMT
ENV GRADLE_HOME=/opt/gradle
# Tue, 28 Jan 2020 00:38:34 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Tue, 28 Jan 2020 00:38:36 GMT
VOLUME [/home/gradle/.gradle]
# Tue, 28 Jan 2020 00:38:38 GMT
WORKDIR /home/gradle
# Tue, 28 Jan 2020 00:39:30 GMT
RUN apt-get update     && apt-get install --yes --no-install-recommends         fontconfig         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm -rf /var/lib/apt/lists/*
# Tue, 28 Jan 2020 00:39:35 GMT
ENV GRADLE_VERSION=6.1.1
# Tue, 28 Jan 2020 00:39:38 GMT
ARG GRADLE_DOWNLOAD_SHA256=9d94e6e4a28ad328072ef6e56bce79a810494ae756751fdcedffdeaf27c093b1
# Tue, 28 Jan 2020 00:39:46 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=9d94e6e4a28ad328072ef6e56bce79a810494ae756751fdcedffdeaf27c093b1
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:5592aacf4ac7489bb730c3e5b1799876d68000b7bbf6e9377ca30e16bff059be`  
		Last Modified: Mon, 13 Jan 2020 15:33:24 GMT  
		Size: 30.4 MB (30400610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f7f270f33afb11e2590bebf54c54fcb052048417bc01b24e357117d730d26a`  
		Last Modified: Thu, 16 Jan 2020 01:19:43 GMT  
		Size: 35.2 KB (35217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242585cde72a9805b281397c8fe3b84a8260c6523a4c290da82e6209845c3690`  
		Last Modified: Thu, 16 Jan 2020 01:19:42 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509fc799f2e0e3149ea8c75fb5b36528e147c5e7123e226d9da46be9c3c79f36`  
		Last Modified: Thu, 16 Jan 2020 01:19:42 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5515694a6e8bfc9e87d0ae9d3b2046662f7a29cfbcb1eaa00c8c3d1a2ba211`  
		Last Modified: Thu, 16 Jan 2020 01:50:01 GMT  
		Size: 14.0 MB (13969109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b58e15b85da97568da2cc8e2f916516c9980d617866db250cc642e21d198b4c`  
		Last Modified: Tue, 28 Jan 2020 00:27:57 GMT  
		Size: 39.6 MB (39581837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54221a10c6006aa63b3d78308e188e9c03fc5364f7805b3d3c311c4156424b09`  
		Last Modified: Tue, 28 Jan 2020 00:44:59 GMT  
		Size: 4.5 KB (4521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b3605b983ddc37f966d1fc7ff67a18457cde106fcf9a7aac8257934d25689b`  
		Last Modified: Tue, 28 Jan 2020 00:45:13 GMT  
		Size: 56.7 MB (56696748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ccf49020775be2db8aa1df31c4443bc7ae03b1a218683c56098eff9b0ae87c7`  
		Last Modified: Tue, 28 Jan 2020 00:45:08 GMT  
		Size: 97.5 MB (97483540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jre11` - linux; s390x

```console
$ docker pull gradle@sha256:557803b1e29f40de6843bc474c1d77ef65f580f52faef65b9bd01797ff5c4ac7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.1 MB (223148826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec8e84ac05177474252791245e7b2c133d858ce74a97b7933000bca3fe059796`
-	Default Command: `["gradle"]`

```dockerfile
# Thu, 31 Oct 2019 22:41:56 GMT
ADD file:6e6c5c69d7791dc0b62c8d03fc0c5051c6291e08dfc4e11abbdc333bc6f44359 in / 
# Thu, 31 Oct 2019 22:41:58 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:41:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:42:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:42:01 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:00:01 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 31 Oct 2019 23:00:30 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:01:04 GMT
ENV JAVA_VERSION=jdk-11.0.4+11
# Thu, 31 Oct 2019 23:01:50 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='5f7b5c110fc0f344a549cb11784a6d76838061a2b6f654f7841f60e0cd286c6a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.4%2B11/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.4_11.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='5da5f86f250eeb26719ba06ae1a1133eb75933fad7b9cf1624d743fafd7a7e2b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.4%2B11/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.4_11.tar.gz';          ;;        s390x)          ESUM='274036da66b150050e23dfc87a4c0ab5331fa6f0d0804b8016621aedf8d1a1e1';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.4%2B11/OpenJDK11U-jre_s390x_linux_hotspot_11.0.4_11.tar.gz';          ;;        amd64|x86_64)          ESUM='70d2cc675155476f1d8516a7ae6729d44681e4fad5a6fc8dfa65cab36a67b7e0';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.4%2B11/OpenJDK11U-jre_x64_linux_hotspot_11.0.4_11.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 31 Oct 2019 23:01:51 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 Nov 2019 00:06:03 GMT
CMD ["gradle"]
# Fri, 01 Nov 2019 00:06:04 GMT
ENV GRADLE_HOME=/opt/gradle
# Fri, 01 Nov 2019 00:06:06 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Fri, 01 Nov 2019 00:06:07 GMT
VOLUME [/home/gradle/.gradle]
# Fri, 01 Nov 2019 00:06:12 GMT
WORKDIR /home/gradle
# Fri, 01 Nov 2019 00:07:00 GMT
RUN apt-get update     && apt-get install --yes --no-install-recommends         fontconfig         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm -rf /var/lib/apt/lists/*
# Tue, 28 Jan 2020 00:10:14 GMT
ENV GRADLE_VERSION=6.1.1
# Tue, 28 Jan 2020 00:10:15 GMT
ARG GRADLE_DOWNLOAD_SHA256=9d94e6e4a28ad328072ef6e56bce79a810494ae756751fdcedffdeaf27c093b1
# Tue, 28 Jan 2020 00:10:20 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=9d94e6e4a28ad328072ef6e56bce79a810494ae756751fdcedffdeaf27c093b1
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:617b55fd1ba95b3ed68226101c9b2568ed00a9b7c50959230d2124648f3a47d2`  
		Last Modified: Thu, 31 Oct 2019 22:43:47 GMT  
		Size: 25.4 MB (25364650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee6ed80b799b3b7d7d66e31ba7e61be1f8d02732bccb1a22d1f14c65f9cea21`  
		Last Modified: Thu, 31 Oct 2019 22:43:42 GMT  
		Size: 36.2 KB (36173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc71634b6bba51b68da661aedfd0876ba93b197653cc94323ca050369bef0bc`  
		Last Modified: Thu, 31 Oct 2019 22:43:43 GMT  
		Size: 841.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e017bfda3869ce68902d01d6dfb0fe74964f8c598ea31bc77825772e58a122b`  
		Last Modified: Thu, 31 Oct 2019 22:43:43 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d6516ebe93aefa5d84bd151472231fda34a88c02a0c5b2ebdfa62a362ffdb3`  
		Last Modified: Thu, 31 Oct 2019 23:05:58 GMT  
		Size: 10.6 MB (10552908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37b8346f33b7a78720e7cd5172e7b4f38a024424cb9dc5daba2b93de5544ff30`  
		Last Modified: Thu, 31 Oct 2019 23:07:19 GMT  
		Size: 39.1 MB (39140065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805900cc5865bfc68379f7c6d998a52143a8dfdd4b0fcf1b01bec462b3e10ef7`  
		Last Modified: Fri, 01 Nov 2019 00:11:20 GMT  
		Size: 4.5 KB (4487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc2b2d13feddb7c6fbb064377df74103abbff926f507978ec46e4bf50eaef0e`  
		Last Modified: Fri, 01 Nov 2019 00:11:32 GMT  
		Size: 50.6 MB (50566020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80beafdbd1c6c0b6663b7ae742ba0bc21ef9ed7ff3b5bbc4effe8a03f4eb5cf0`  
		Last Modified: Tue, 28 Jan 2020 00:11:47 GMT  
		Size: 97.5 MB (97483520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
