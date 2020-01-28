## `gradle:jre13`

```console
$ docker pull gradle@sha256:9286b1e4e367900956c8fbe70c1c04b6d9311a54217ce3b381fbb8b55ee27bc3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `gradle:jre13` - linux; amd64

```console
$ docker pull gradle@sha256:ad2cc3474de6128623fbd0e1bcbcdda9f1ecb2844d7ab40d0a2ee21c912d5aa4
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.2 MB (233181819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:974ba775cb3cce79ded217a7adfd8b56bcacf9100d61cd870f204a57c5e66e70`
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
# Tue, 28 Jan 2020 00:20:11 GMT
ENV JAVA_VERSION=jdk-13.0.2+8
# Tue, 28 Jan 2020 00:20:37 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6c4b69d1609f4c65c576c80d6aa101de80048f8ce5566f890e8fff5349228bae';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk13-binaries/releases/download/jdk-13.0.2%2B8/OpenJDK13U-jre_aarch64_linux_hotspot_13.0.2_8.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='43d6fb71bdf7b6ad9295087c46dfc9b00bf26db1b5cdcff0c418cbe43b49904a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk13-binaries/releases/download/jdk-13.0.2%2B8/OpenJDK13U-jre_ppc64le_linux_hotspot_13.0.2_8.tar.gz';          ;;        s390x)          ESUM='ac07703f9b9aed0676ae751f2b5b2346285566944ba89d0d8833790f83b00163';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk13-binaries/releases/download/jdk-13.0.2%2B8/OpenJDK13U-jre_s390x_linux_hotspot_13.0.2_8.tar.gz';          ;;        amd64|x86_64)          ESUM='897f16fe8e056395209e35d2384013bd1ff250e717465769079e3f4793628c34';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk13-binaries/releases/download/jdk-13.0.2%2B8/OpenJDK13U-jre_x64_linux_hotspot_13.0.2_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 28 Jan 2020 00:20:37 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Jan 2020 00:35:12 GMT
CMD ["gradle"]
# Tue, 28 Jan 2020 00:35:12 GMT
ENV GRADLE_HOME=/opt/gradle
# Tue, 28 Jan 2020 00:35:13 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Tue, 28 Jan 2020 00:35:13 GMT
VOLUME [/home/gradle/.gradle]
# Tue, 28 Jan 2020 00:35:13 GMT
WORKDIR /home/gradle
# Tue, 28 Jan 2020 00:35:31 GMT
RUN apt-get update     && apt-get install --yes --no-install-recommends         fontconfig         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm -rf /var/lib/apt/lists/*
# Tue, 28 Jan 2020 00:35:31 GMT
ENV GRADLE_VERSION=6.1.1
# Tue, 28 Jan 2020 00:35:31 GMT
ARG GRADLE_DOWNLOAD_SHA256=9d94e6e4a28ad328072ef6e56bce79a810494ae756751fdcedffdeaf27c093b1
# Tue, 28 Jan 2020 00:35:36 GMT
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
	-	`sha256:83d0dbb67c88962c0eaf0c21f6541429f93415fa840ba518f88da1f32c72e2a8`  
		Last Modified: Tue, 28 Jan 2020 00:24:09 GMT  
		Size: 47.0 MB (46997598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b572003c906be80a9f239d4e587c08dc53997974f558f4411868c32a82d065`  
		Last Modified: Tue, 28 Jan 2020 00:37:26 GMT  
		Size: 4.5 KB (4488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5660df6f340734054e28da7708b66ec40cf9cfa9ba1aa95002d2f166b6f18ebb`  
		Last Modified: Tue, 28 Jan 2020 00:37:37 GMT  
		Size: 48.6 MB (48646497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa547a8664dc00fd2fbbdc58727e8ffbcdef3b67b97b1457d1a361a44e9ebbc`  
		Last Modified: Tue, 28 Jan 2020 00:37:34 GMT  
		Size: 97.5 MB (97483403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jre13` - linux; arm64 variant v8

```console
$ docker pull gradle@sha256:460487eaa4fc573ec378a17028adc1738adc618ccd34169c33dc43b07bb0f1d3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.6 MB (225634747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74efc281a2f72230dd2210a73e500d5bf967b589555b13b9e357d0d09810f925`
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
# Mon, 27 Jan 2020 23:41:01 GMT
ENV JAVA_VERSION=jdk-13.0.2+8
# Mon, 27 Jan 2020 23:41:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6c4b69d1609f4c65c576c80d6aa101de80048f8ce5566f890e8fff5349228bae';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk13-binaries/releases/download/jdk-13.0.2%2B8/OpenJDK13U-jre_aarch64_linux_hotspot_13.0.2_8.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='43d6fb71bdf7b6ad9295087c46dfc9b00bf26db1b5cdcff0c418cbe43b49904a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk13-binaries/releases/download/jdk-13.0.2%2B8/OpenJDK13U-jre_ppc64le_linux_hotspot_13.0.2_8.tar.gz';          ;;        s390x)          ESUM='ac07703f9b9aed0676ae751f2b5b2346285566944ba89d0d8833790f83b00163';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk13-binaries/releases/download/jdk-13.0.2%2B8/OpenJDK13U-jre_s390x_linux_hotspot_13.0.2_8.tar.gz';          ;;        amd64|x86_64)          ESUM='897f16fe8e056395209e35d2384013bd1ff250e717465769079e3f4793628c34';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk13-binaries/releases/download/jdk-13.0.2%2B8/OpenJDK13U-jre_x64_linux_hotspot_13.0.2_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 27 Jan 2020 23:41:48 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Jan 2020 23:47:35 GMT
CMD ["gradle"]
# Mon, 27 Jan 2020 23:47:35 GMT
ENV GRADLE_HOME=/opt/gradle
# Mon, 27 Jan 2020 23:47:37 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Mon, 27 Jan 2020 23:47:37 GMT
VOLUME [/home/gradle/.gradle]
# Mon, 27 Jan 2020 23:47:38 GMT
WORKDIR /home/gradle
# Mon, 27 Jan 2020 23:48:10 GMT
RUN apt-get update     && apt-get install --yes --no-install-recommends         fontconfig         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm -rf /var/lib/apt/lists/*
# Mon, 27 Jan 2020 23:48:12 GMT
ENV GRADLE_VERSION=6.1.1
# Mon, 27 Jan 2020 23:48:13 GMT
ARG GRADLE_DOWNLOAD_SHA256=9d94e6e4a28ad328072ef6e56bce79a810494ae756751fdcedffdeaf27c093b1
# Mon, 27 Jan 2020 23:48:19 GMT
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
	-	`sha256:3b038f496fd7b6fa3de9200b5e0a07e3daf9d2a5a6226cd708b1e0e62548daba`  
		Last Modified: Mon, 27 Jan 2020 23:44:52 GMT  
		Size: 45.5 MB (45461332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d92e8ff0734da637be5d8978ab265913df5758d1dc08ad55e6a364dec618bc39`  
		Last Modified: Mon, 27 Jan 2020 23:49:27 GMT  
		Size: 4.5 KB (4524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cafdf768c2b551c019d8aeb538e0849672747bf4c66e7db8f5a1fb664ef0f6e4`  
		Last Modified: Mon, 27 Jan 2020 23:49:43 GMT  
		Size: 46.2 MB (46197373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ffdfdf82be6c62ec811840ef63b4e58ab7cd5f749fc732387b6a6898af6adee`  
		Last Modified: Mon, 27 Jan 2020 23:49:40 GMT  
		Size: 97.5 MB (97483493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jre13` - linux; ppc64le

```console
$ docker pull gradle@sha256:02896e2cc1b72b0824e2b98e85031b14dfb84841f39dfe81d8c356e9ae9c4c04
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.7 MB (240704405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b3b5aa875752cc5091e169e2bd01c16eb149e8ee9122954e69a0efe819b23d2`
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
# Tue, 28 Jan 2020 00:21:33 GMT
ENV JAVA_VERSION=jdk-13.0.2+8
# Tue, 28 Jan 2020 00:22:19 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6c4b69d1609f4c65c576c80d6aa101de80048f8ce5566f890e8fff5349228bae';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk13-binaries/releases/download/jdk-13.0.2%2B8/OpenJDK13U-jre_aarch64_linux_hotspot_13.0.2_8.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='43d6fb71bdf7b6ad9295087c46dfc9b00bf26db1b5cdcff0c418cbe43b49904a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk13-binaries/releases/download/jdk-13.0.2%2B8/OpenJDK13U-jre_ppc64le_linux_hotspot_13.0.2_8.tar.gz';          ;;        s390x)          ESUM='ac07703f9b9aed0676ae751f2b5b2346285566944ba89d0d8833790f83b00163';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk13-binaries/releases/download/jdk-13.0.2%2B8/OpenJDK13U-jre_s390x_linux_hotspot_13.0.2_8.tar.gz';          ;;        amd64|x86_64)          ESUM='897f16fe8e056395209e35d2384013bd1ff250e717465769079e3f4793628c34';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk13-binaries/releases/download/jdk-13.0.2%2B8/OpenJDK13U-jre_x64_linux_hotspot_13.0.2_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 28 Jan 2020 00:22:21 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Jan 2020 00:41:37 GMT
CMD ["gradle"]
# Tue, 28 Jan 2020 00:41:38 GMT
ENV GRADLE_HOME=/opt/gradle
# Tue, 28 Jan 2020 00:41:43 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Tue, 28 Jan 2020 00:41:46 GMT
VOLUME [/home/gradle/.gradle]
# Tue, 28 Jan 2020 00:41:47 GMT
WORKDIR /home/gradle
# Tue, 28 Jan 2020 00:42:33 GMT
RUN apt-get update     && apt-get install --yes --no-install-recommends         fontconfig         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm -rf /var/lib/apt/lists/*
# Tue, 28 Jan 2020 00:42:37 GMT
ENV GRADLE_VERSION=6.1.1
# Tue, 28 Jan 2020 00:42:38 GMT
ARG GRADLE_DOWNLOAD_SHA256=9d94e6e4a28ad328072ef6e56bce79a810494ae756751fdcedffdeaf27c093b1
# Tue, 28 Jan 2020 00:42:48 GMT
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
	-	`sha256:f6dfa1cbaea79ae71b177315946519dd619747444f18d89f016ffa6ccb1b36db`  
		Last Modified: Tue, 28 Jan 2020 00:28:59 GMT  
		Size: 42.1 MB (42113518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d7c3e5d9bbaf96bdc6d3a5fed5adf953f8f497ff84528c29ae8916f4f9ddd6`  
		Last Modified: Tue, 28 Jan 2020 00:45:53 GMT  
		Size: 4.5 KB (4527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4ffe7cd1b25893fa7e9d4eaf64182e8af63c9cbe59b6cc9aec35bfd20df6e3`  
		Last Modified: Tue, 28 Jan 2020 00:46:08 GMT  
		Size: 56.7 MB (56696850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d73e2d3614dfa9c75c91396417b224429ab818eeb6602c074c7b38eab49b93`  
		Last Modified: Tue, 28 Jan 2020 00:46:03 GMT  
		Size: 97.5 MB (97483530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jre13` - linux; s390x

```console
$ docker pull gradle@sha256:b12fef038a625587387e3efeb5f49b245f92ba6431dcebd5415a9189b7ad1d0d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.9 MB (225942297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b15c30ecc7ea257b48b149e688dbec440ebb81e0f4d0e08e61fd7ed4299dde0b`
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
# Fri, 08 Nov 2019 02:41:48 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 08 Nov 2019 02:42:17 GMT
ENV JAVA_VERSION=jdk-13.0.1+9
# Fri, 08 Nov 2019 02:42:38 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='58e841a26c1b3a0cf15f052797e5a6a91f8b65c78d0eb84e4eb6310b3af5b9ec';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk13-binaries/releases/download/jdk-13.0.1%2B9/OpenJDK13U-jre_aarch64_linux_hotspot_13.0.1_9.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='c6258058557fd0ec6f0426c4671ad78e7b665cf8d487e5d07b690e792121b2f3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk13-binaries/releases/download/jdk-13.0.1%2B9/OpenJDK13U-jre_ppc64le_linux_hotspot_13.0.1_9.tar.gz';          ;;        s390x)          ESUM='e866aa35889358bb134675a079510b0cc279737c3fb26f30e229a69726833f5b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk13-binaries/releases/download/jdk-13.0.1%2B9/OpenJDK13U-jre_s390x_linux_hotspot_13.0.1_9.tar.gz';          ;;        amd64|x86_64)          ESUM='5bd06d9df1f76d953658fbe36812809b43e2d9dd00093e023aded64846f7af5a';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk13-binaries/releases/download/jdk-13.0.1%2B9/OpenJDK13U-jre_x64_linux_hotspot_13.0.1_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 08 Nov 2019 02:42:39 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Nov 2019 00:43:02 GMT
CMD ["gradle"]
# Tue, 12 Nov 2019 00:43:02 GMT
ENV GRADLE_HOME=/opt/gradle
# Tue, 12 Nov 2019 00:43:03 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Tue, 12 Nov 2019 00:43:03 GMT
VOLUME [/home/gradle/.gradle]
# Tue, 12 Nov 2019 00:43:03 GMT
WORKDIR /home/gradle
# Tue, 12 Nov 2019 00:43:27 GMT
RUN apt-get update     && apt-get install --yes --no-install-recommends         fontconfig         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm -rf /var/lib/apt/lists/*
# Tue, 28 Jan 2020 00:10:45 GMT
ENV GRADLE_VERSION=6.1.1
# Tue, 28 Jan 2020 00:10:46 GMT
ARG GRADLE_DOWNLOAD_SHA256=9d94e6e4a28ad328072ef6e56bce79a810494ae756751fdcedffdeaf27c093b1
# Tue, 28 Jan 2020 00:10:51 GMT
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
	-	`sha256:91b19c0383ed91f9b1804ed41cac85c7d675628ede6f1b32b27d54b75a6f40aa`  
		Last Modified: Fri, 08 Nov 2019 02:44:24 GMT  
		Size: 13.0 MB (13040836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1574b9d2915ca440a8df6067210b8b08a83fa5e1b26a947456fe7ce51ac62c79`  
		Last Modified: Fri, 08 Nov 2019 02:45:24 GMT  
		Size: 41.9 MB (41916656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51f59d9f4e9a794f0a5819eb266ba17ab3e031ee74ce4b07f6e0e9f992a9b16`  
		Last Modified: Tue, 12 Nov 2019 00:44:55 GMT  
		Size: 4.5 KB (4499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c9182a8c3317e15fea9b4554a082a526c2c6b2dbe466b8e793e51c1b2ac0c3`  
		Last Modified: Tue, 12 Nov 2019 00:45:06 GMT  
		Size: 48.1 MB (48094976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0930864de6f170219719e178bbffc66b0b655306f3af48253b557e1f986575ce`  
		Last Modified: Tue, 28 Jan 2020 00:12:10 GMT  
		Size: 97.5 MB (97483504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
