## `groovy:jre11`

```console
$ docker pull groovy@sha256:ca21e760a8c58f04b92141e502515e369ed8e8b449dab04947d4dd6f21fae521
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `groovy:jre11` - linux; amd64

```console
$ docker pull groovy@sha256:e7ad4d1c97c95b24c08b90e18670d33352338662645cd397d34ff4d6ec67eeae
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.4 MB (133438034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5be4f95f40d6c2cd4aa53b1572e9c316bd9d959316ff3e96f2f1a3f95e0e184`
-	Default Command: `["groovysh"]`

```dockerfile
# Wed, 19 Aug 2020 21:13:50 GMT
ADD file:5c125b7f411566e9daa738d8cb851098f36197810f06488c2609074296f294b2 in / 
# Wed, 19 Aug 2020 21:13:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:13:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:13:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:13:55 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 21:58:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 19 Aug 2020 21:58:49 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:59:10 GMT
ENV JAVA_VERSION=jdk-11.0.8+10
# Wed, 19 Aug 2020 21:59:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='286c869dbaefda9b470ae71d1250fdecf9f06d8da97c0f7df9021d381d749106';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.8%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.8_10.tar.gz';          ;;        armhf|armv7l)          ESUM='ffa627b2d0c6001448bb8f1f24f7c9921dad37e67637f6ed0a9a479e680a3393';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.8%2B10/OpenJDK11U-jre_arm_linux_hotspot_11.0.8_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='89231e1667d7cc4202d1a401497bb287d4eb12281c90c17e2570211cc4e901a3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.8%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.8_10.tar.gz';          ;;        s390x)          ESUM='dc0e715c17abcb12bedf77c638e58e67d828d3c4bf24a898f0d4b053caaeb25f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.8%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.8_10.tar.gz';          ;;        amd64|x86_64)          ESUM='98615b1b369509965a612232622d39b5cefe117d6189179cbad4dcef2ee2f4e1';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.8%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.8_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 21:59:29 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 20 Aug 2020 02:14:15 GMT
CMD ["groovysh"]
# Thu, 20 Aug 2020 02:14:15 GMT
ENV GROOVY_HOME=/opt/groovy
# Thu, 20 Aug 2020 02:14:16 GMT
RUN set -o errexit -o nounset     && echo "Adding groovy user and group"     && groupadd --system --gid 1000 groovy     && useradd --system --gid groovy --uid 1000 --shell /bin/bash --create-home groovy     && mkdir --parents /home/groovy/.groovy/grapes     && chown --recursive groovy:groovy /home/groovy     && chmod --recursive 1777 /home/groovy         && echo "Symlinking root .groovy to groovy .groovy"     && ln --symbolic /home/groovy/.groovy /root/.groovy
# Thu, 20 Aug 2020 02:14:16 GMT
VOLUME [/home/groovy/.groovy/grapes]
# Thu, 20 Aug 2020 02:14:16 GMT
WORKDIR /home/groovy
# Thu, 20 Aug 2020 02:14:23 GMT
RUN apt-get update     && echo "Installing build dependencies"     && apt-get install --yes --no-install-recommends         dirmngr         fontconfig         gnupg         unzip         wget     && rm --recursive --force /var/lib/apt/lists/*
# Thu, 20 Aug 2020 02:14:23 GMT
ENV GROOVY_VERSION=3.0.5
# Thu, 20 Aug 2020 02:14:28 GMT
RUN set -o errexit -o nounset     && echo "Downloading Groovy"     && wget --no-verbose --output-document=groovy.zip "https://archive.apache.org/dist/groovy/${GROOVY_VERSION}/distribution/apache-groovy-binary-${GROOVY_VERSION}.zip"         && echo "Importing keys listed in http://www.apache.org/dist/groovy/KEYS from key server"     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --no-tty --keyserver ha.pool.sks-keyservers.net --recv-keys         7FAA0F2206DE228F0DB01AD741321490758AAD6F         331224E1D7BE883D16E8A685825C06C827AF6B66         34441E504A937F43EB0DAEF96A65176A0FB1CD0B         9A810E3B766E089FFB27C70F11B595CEDC4AEBB5         81CABC23EECA0790E8989B361FF96E10F0E13706         && echo "Checking download signature"     && wget --no-verbose --output-document=groovy.zip.asc "https://archive.apache.org/dist/groovy/${GROOVY_VERSION}/distribution/apache-groovy-binary-${GROOVY_VERSION}.zip.asc"     && gpg --batch --no-tty --verify groovy.zip.asc groovy.zip     && rm --recursive --force "${GNUPGHOME}"     && rm groovy.zip.asc         && echo "Installing Groovy"     && unzip groovy.zip     && rm groovy.zip     && mv "groovy-${GROOVY_VERSION}" "${GROOVY_HOME}/"     && ln --symbolic "${GROOVY_HOME}/bin/grape" /usr/bin/grape     && ln --symbolic "${GROOVY_HOME}/bin/groovy" /usr/bin/groovy     && ln --symbolic "${GROOVY_HOME}/bin/groovyc" /usr/bin/groovyc     && ln --symbolic "${GROOVY_HOME}/bin/groovyConsole" /usr/bin/groovyConsole     && ln --symbolic "${GROOVY_HOME}/bin/groovydoc" /usr/bin/groovydoc     && ln --symbolic "${GROOVY_HOME}/bin/groovysh" /usr/bin/groovysh     && ln --symbolic "${GROOVY_HOME}/bin/java2groovy" /usr/bin/java2groovy         && echo "Editing startGroovy to include java.xml.bind module"     && sed --in-place 's|startGroovy ( ) {|startGroovy ( ) {\n    JAVA_OPTS="$JAVA_OPTS --add-modules=ALL-SYSTEM"|' "${GROOVY_HOME}/bin/startGroovy"
# Thu, 20 Aug 2020 02:14:28 GMT
USER groovy
# Thu, 20 Aug 2020 02:14:30 GMT
RUN set -o errexit -o nounset     && echo "Testing Groovy installation"     && groovy --version
```

-	Layers:
	-	`sha256:f08d8e2a3ba11bea23cf5c17e8e1c620057412ed05c32d1114640e18d6dd0a43`  
		Last Modified: Sat, 08 Aug 2020 12:21:16 GMT  
		Size: 26.7 MB (26700095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9cb2483bd9c5329a44d9c2fe72535625bbd4308bca95785dd58e72c06365`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e5ff4c0b1526abf77c236655f21c8f67a23313291c8b970fe6b469549d8153`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1860925334f940c3145808527480b4f0cba7f01279087fdb27679e4354fba967`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b7f96c83b992275744136bd8deb3404fb357ee0e75620f46f7db8aed8481d6`  
		Last Modified: Wed, 19 Aug 2020 22:02:55 GMT  
		Size: 13.9 MB (13875193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b6868827e7f0338afd64598978d5fe7dc187d1b6eb86728b81a16c4feba3b1`  
		Last Modified: Wed, 19 Aug 2020 22:03:57 GMT  
		Size: 43.6 MB (43627125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b90714e288487dbd572e7cbc7507c0de27c4a9761b394dbbde9fee10a9a7dff6`  
		Last Modified: Thu, 20 Aug 2020 02:15:52 GMT  
		Size: 4.5 KB (4520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0fbd6819be77af54bbb99a3cfad10075888fc2f1710f007f412eeb25e7d512`  
		Last Modified: Thu, 20 Aug 2020 02:15:52 GMT  
		Size: 3.5 MB (3503180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18feaa7328223b8841979177f0e0686a1d92f41c0c63c02ed2954c6d4c201cf9`  
		Last Modified: Thu, 20 Aug 2020 02:15:55 GMT  
		Size: 45.7 MB (45691406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a4ac53352fff1b9111e3676703085b96d85f8c4266f46b45ee185b5b3eedca`  
		Last Modified: Thu, 20 Aug 2020 02:15:51 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `groovy:jre11` - linux; arm64 variant v8

```console
$ docker pull groovy@sha256:542fdab26a3c11351c7b5118bc08868fcad78ec20e9740bab3ff0dcdad36ac59
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (127951794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f9742ba46710932b77c9327f83518cc30100e5e34229f7a16b3193f60bd3fd3`
-	Default Command: `["groovysh"]`

```dockerfile
# Wed, 19 Aug 2020 21:29:47 GMT
ADD file:b8316fc82a2cf230ce4af7dcf02ec1d7e56b156cf610af8ed23b64509c77c799 in / 
# Wed, 19 Aug 2020 21:29:51 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:29:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:29:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:29:55 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:48:56 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 19 Aug 2020 22:49:31 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:50:07 GMT
ENV JAVA_VERSION=jdk-11.0.8+10
# Wed, 19 Aug 2020 22:51:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='286c869dbaefda9b470ae71d1250fdecf9f06d8da97c0f7df9021d381d749106';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.8%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.8_10.tar.gz';          ;;        armhf|armv7l)          ESUM='ffa627b2d0c6001448bb8f1f24f7c9921dad37e67637f6ed0a9a479e680a3393';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.8%2B10/OpenJDK11U-jre_arm_linux_hotspot_11.0.8_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='89231e1667d7cc4202d1a401497bb287d4eb12281c90c17e2570211cc4e901a3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.8%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.8_10.tar.gz';          ;;        s390x)          ESUM='dc0e715c17abcb12bedf77c638e58e67d828d3c4bf24a898f0d4b053caaeb25f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.8%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.8_10.tar.gz';          ;;        amd64|x86_64)          ESUM='98615b1b369509965a612232622d39b5cefe117d6189179cbad4dcef2ee2f4e1';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.8%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.8_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 22:51:07 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 20 Aug 2020 01:08:19 GMT
CMD ["groovysh"]
# Thu, 20 Aug 2020 01:08:19 GMT
ENV GROOVY_HOME=/opt/groovy
# Thu, 20 Aug 2020 01:08:41 GMT
RUN set -o errexit -o nounset     && echo "Adding groovy user and group"     && groupadd --system --gid 1000 groovy     && useradd --system --gid groovy --uid 1000 --shell /bin/bash --create-home groovy     && mkdir --parents /home/groovy/.groovy/grapes     && chown --recursive groovy:groovy /home/groovy     && chmod --recursive 1777 /home/groovy         && echo "Symlinking root .groovy to groovy .groovy"     && ln --symbolic /home/groovy/.groovy /root/.groovy
# Thu, 20 Aug 2020 01:08:45 GMT
VOLUME [/home/groovy/.groovy/grapes]
# Thu, 20 Aug 2020 01:08:46 GMT
WORKDIR /home/groovy
# Thu, 20 Aug 2020 01:09:08 GMT
RUN apt-get update     && echo "Installing build dependencies"     && apt-get install --yes --no-install-recommends         dirmngr         fontconfig         gnupg         unzip         wget     && rm --recursive --force /var/lib/apt/lists/*
# Thu, 20 Aug 2020 01:09:11 GMT
ENV GROOVY_VERSION=3.0.5
# Thu, 20 Aug 2020 01:09:34 GMT
RUN set -o errexit -o nounset     && echo "Downloading Groovy"     && wget --no-verbose --output-document=groovy.zip "https://archive.apache.org/dist/groovy/${GROOVY_VERSION}/distribution/apache-groovy-binary-${GROOVY_VERSION}.zip"         && echo "Importing keys listed in http://www.apache.org/dist/groovy/KEYS from key server"     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --no-tty --keyserver ha.pool.sks-keyservers.net --recv-keys         7FAA0F2206DE228F0DB01AD741321490758AAD6F         331224E1D7BE883D16E8A685825C06C827AF6B66         34441E504A937F43EB0DAEF96A65176A0FB1CD0B         9A810E3B766E089FFB27C70F11B595CEDC4AEBB5         81CABC23EECA0790E8989B361FF96E10F0E13706         && echo "Checking download signature"     && wget --no-verbose --output-document=groovy.zip.asc "https://archive.apache.org/dist/groovy/${GROOVY_VERSION}/distribution/apache-groovy-binary-${GROOVY_VERSION}.zip.asc"     && gpg --batch --no-tty --verify groovy.zip.asc groovy.zip     && rm --recursive --force "${GNUPGHOME}"     && rm groovy.zip.asc         && echo "Installing Groovy"     && unzip groovy.zip     && rm groovy.zip     && mv "groovy-${GROOVY_VERSION}" "${GROOVY_HOME}/"     && ln --symbolic "${GROOVY_HOME}/bin/grape" /usr/bin/grape     && ln --symbolic "${GROOVY_HOME}/bin/groovy" /usr/bin/groovy     && ln --symbolic "${GROOVY_HOME}/bin/groovyc" /usr/bin/groovyc     && ln --symbolic "${GROOVY_HOME}/bin/groovyConsole" /usr/bin/groovyConsole     && ln --symbolic "${GROOVY_HOME}/bin/groovydoc" /usr/bin/groovydoc     && ln --symbolic "${GROOVY_HOME}/bin/groovysh" /usr/bin/groovysh     && ln --symbolic "${GROOVY_HOME}/bin/java2groovy" /usr/bin/java2groovy         && echo "Editing startGroovy to include java.xml.bind module"     && sed --in-place 's|startGroovy ( ) {|startGroovy ( ) {\n    JAVA_OPTS="$JAVA_OPTS --add-modules=ALL-SYSTEM"|' "${GROOVY_HOME}/bin/startGroovy"
# Thu, 20 Aug 2020 01:09:35 GMT
USER groovy
# Thu, 20 Aug 2020 01:09:39 GMT
RUN set -o errexit -o nounset     && echo "Testing Groovy installation"     && groovy --version
```

-	Layers:
	-	`sha256:237528ba509b2abcdba1ff1344bab27ad56235cdb3c1c131d3587f6fba4d92c9`  
		Last Modified: Sat, 08 Aug 2020 00:25:26 GMT  
		Size: 23.7 MB (23721798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:393b96f31d8b2bf3ce9eb4ac49e6c7411defa4057c1791f02f54c14f2de298ec`  
		Last Modified: Wed, 19 Aug 2020 21:32:13 GMT  
		Size: 35.2 KB (35203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d82b0e39008d2fa246a0dca4cfa5feb15db58591582a839bd69d5000aa2e96d`  
		Last Modified: Wed, 19 Aug 2020 21:32:13 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ca375b8d34c9bc764ae24791184cba22510f0c002815b4f9766dd0463f5f5e`  
		Last Modified: Wed, 19 Aug 2020 21:32:14 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7799af3c6cccc592b3b72623a0d559ec705bec28fdee373ef6675d468a379570`  
		Last Modified: Wed, 19 Aug 2020 22:54:11 GMT  
		Size: 13.3 MB (13285045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be6cfc9b3bd24c956662c74eb6c01624e2074bbb694a4a89f63c5b5d4bf3253`  
		Last Modified: Wed, 19 Aug 2020 22:55:52 GMT  
		Size: 42.0 MB (41978753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b704cfb1712f9f957936e30f3ce0ee6100b2374a71f882ab6ea10a766de5b1e`  
		Last Modified: Thu, 20 Aug 2020 01:11:23 GMT  
		Size: 4.6 KB (4553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ea23fe065bd9a9eef8425c8042c92b9ef9459b6950db80dad028194d2c677e`  
		Last Modified: Thu, 20 Aug 2020 01:11:24 GMT  
		Size: 3.2 MB (3233748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf39ef9133365ffe89893d39908a7ea3b6fe888943db34ffb3b2550915f118e`  
		Last Modified: Thu, 20 Aug 2020 01:11:29 GMT  
		Size: 45.7 MB (45691480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec071670b92cafef394e42f6eeb788df0c0c53c35f05193a6fedae1da8405c19`  
		Last Modified: Thu, 20 Aug 2020 01:11:23 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `groovy:jre11` - linux; ppc64le

```console
$ docker pull groovy@sha256:e4fc07b88f321280724d9e074d18d3adb34a06e83e2a355c4e758d74956f78f0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.6 MB (134555721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ddc261e82d7b22d93e9d875d5dbb6b75150e92fc36049a94f3086e8b0506573`
-	Default Command: `["groovysh"]`

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
# Wed, 19 Aug 2020 22:26:33 GMT
ENV JAVA_VERSION=jdk-11.0.8+10
# Wed, 19 Aug 2020 22:27:37 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='286c869dbaefda9b470ae71d1250fdecf9f06d8da97c0f7df9021d381d749106';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.8%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.8_10.tar.gz';          ;;        armhf|armv7l)          ESUM='ffa627b2d0c6001448bb8f1f24f7c9921dad37e67637f6ed0a9a479e680a3393';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.8%2B10/OpenJDK11U-jre_arm_linux_hotspot_11.0.8_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='89231e1667d7cc4202d1a401497bb287d4eb12281c90c17e2570211cc4e901a3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.8%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.8_10.tar.gz';          ;;        s390x)          ESUM='dc0e715c17abcb12bedf77c638e58e67d828d3c4bf24a898f0d4b053caaeb25f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.8%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.8_10.tar.gz';          ;;        amd64|x86_64)          ESUM='98615b1b369509965a612232622d39b5cefe117d6189179cbad4dcef2ee2f4e1';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.8%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.8_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 22:27:47 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 20 Aug 2020 02:41:57 GMT
CMD ["groovysh"]
# Thu, 20 Aug 2020 02:42:02 GMT
ENV GROOVY_HOME=/opt/groovy
# Thu, 20 Aug 2020 02:42:14 GMT
RUN set -o errexit -o nounset     && echo "Adding groovy user and group"     && groupadd --system --gid 1000 groovy     && useradd --system --gid groovy --uid 1000 --shell /bin/bash --create-home groovy     && mkdir --parents /home/groovy/.groovy/grapes     && chown --recursive groovy:groovy /home/groovy     && chmod --recursive 1777 /home/groovy         && echo "Symlinking root .groovy to groovy .groovy"     && ln --symbolic /home/groovy/.groovy /root/.groovy
# Thu, 20 Aug 2020 02:42:18 GMT
VOLUME [/home/groovy/.groovy/grapes]
# Thu, 20 Aug 2020 02:42:21 GMT
WORKDIR /home/groovy
# Thu, 20 Aug 2020 02:42:56 GMT
RUN apt-get update     && echo "Installing build dependencies"     && apt-get install --yes --no-install-recommends         dirmngr         fontconfig         gnupg         unzip         wget     && rm --recursive --force /var/lib/apt/lists/*
# Thu, 20 Aug 2020 02:43:00 GMT
ENV GROOVY_VERSION=3.0.5
# Thu, 20 Aug 2020 02:43:33 GMT
RUN set -o errexit -o nounset     && echo "Downloading Groovy"     && wget --no-verbose --output-document=groovy.zip "https://archive.apache.org/dist/groovy/${GROOVY_VERSION}/distribution/apache-groovy-binary-${GROOVY_VERSION}.zip"         && echo "Importing keys listed in http://www.apache.org/dist/groovy/KEYS from key server"     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --no-tty --keyserver ha.pool.sks-keyservers.net --recv-keys         7FAA0F2206DE228F0DB01AD741321490758AAD6F         331224E1D7BE883D16E8A685825C06C827AF6B66         34441E504A937F43EB0DAEF96A65176A0FB1CD0B         9A810E3B766E089FFB27C70F11B595CEDC4AEBB5         81CABC23EECA0790E8989B361FF96E10F0E13706         && echo "Checking download signature"     && wget --no-verbose --output-document=groovy.zip.asc "https://archive.apache.org/dist/groovy/${GROOVY_VERSION}/distribution/apache-groovy-binary-${GROOVY_VERSION}.zip.asc"     && gpg --batch --no-tty --verify groovy.zip.asc groovy.zip     && rm --recursive --force "${GNUPGHOME}"     && rm groovy.zip.asc         && echo "Installing Groovy"     && unzip groovy.zip     && rm groovy.zip     && mv "groovy-${GROOVY_VERSION}" "${GROOVY_HOME}/"     && ln --symbolic "${GROOVY_HOME}/bin/grape" /usr/bin/grape     && ln --symbolic "${GROOVY_HOME}/bin/groovy" /usr/bin/groovy     && ln --symbolic "${GROOVY_HOME}/bin/groovyc" /usr/bin/groovyc     && ln --symbolic "${GROOVY_HOME}/bin/groovyConsole" /usr/bin/groovyConsole     && ln --symbolic "${GROOVY_HOME}/bin/groovydoc" /usr/bin/groovydoc     && ln --symbolic "${GROOVY_HOME}/bin/groovysh" /usr/bin/groovysh     && ln --symbolic "${GROOVY_HOME}/bin/java2groovy" /usr/bin/java2groovy         && echo "Editing startGroovy to include java.xml.bind module"     && sed --in-place 's|startGroovy ( ) {|startGroovy ( ) {\n    JAVA_OPTS="$JAVA_OPTS --add-modules=ALL-SYSTEM"|' "${GROOVY_HOME}/bin/startGroovy"
# Thu, 20 Aug 2020 02:43:36 GMT
USER groovy
# Thu, 20 Aug 2020 02:43:58 GMT
RUN set -o errexit -o nounset     && echo "Testing Groovy installation"     && groovy --version
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
	-	`sha256:150ce965860cb5aba883b7e18d76714a54fedde645d2bf6fc5256b1e57f52c48`  
		Last Modified: Wed, 19 Aug 2020 22:42:53 GMT  
		Size: 39.6 MB (39624285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80584f0d2ce4ec8f5e0741d17e4f60a4a206fed276dc8192cec0d26270d4821c`  
		Last Modified: Thu, 20 Aug 2020 02:51:48 GMT  
		Size: 4.6 KB (4561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c09231b8c170e535af228c408718b53faa6f19e3d345b06d6b8f32ff23d9d4dc`  
		Last Modified: Thu, 20 Aug 2020 02:51:49 GMT  
		Size: 4.3 MB (4271314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84b03f563b536b6c87e71f459f321263b1d26d4973abab48cb5160641ed4af5`  
		Last Modified: Thu, 20 Aug 2020 02:51:53 GMT  
		Size: 45.7 MB (45691462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9503b7609ee643d2ccc9ea1dd29646e4002e2477643eb19b09ecaf689633e1`  
		Last Modified: Thu, 20 Aug 2020 02:51:48 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `groovy:jre11` - linux; s390x

```console
$ docker pull groovy@sha256:99bdd2024d468248e56af79dc93dd2bd8b30e6843836b1409227c59b611a00a6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.3 MB (126328621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c954e693bee1e2f81b2685b087eb57eaffec6739af6ca794742954823a6dc4cc`
-	Default Command: `["groovysh"]`

```dockerfile
# Wed, 19 Aug 2020 21:10:03 GMT
ADD file:1343b5ae7d875bd32e4eac552ae10c9631788fd97b99bcdeb9f6a9b85c230ba2 in / 
# Wed, 19 Aug 2020 21:10:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:10:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:10:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:10:06 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 21:55:49 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 19 Aug 2020 21:56:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:56:30 GMT
ENV JAVA_VERSION=jdk-11.0.8+10
# Wed, 19 Aug 2020 21:57:30 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='286c869dbaefda9b470ae71d1250fdecf9f06d8da97c0f7df9021d381d749106';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.8%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.8_10.tar.gz';          ;;        armhf|armv7l)          ESUM='ffa627b2d0c6001448bb8f1f24f7c9921dad37e67637f6ed0a9a479e680a3393';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.8%2B10/OpenJDK11U-jre_arm_linux_hotspot_11.0.8_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='89231e1667d7cc4202d1a401497bb287d4eb12281c90c17e2570211cc4e901a3';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.8%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.8_10.tar.gz';          ;;        s390x)          ESUM='dc0e715c17abcb12bedf77c638e58e67d828d3c4bf24a898f0d4b053caaeb25f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.8%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.8_10.tar.gz';          ;;        amd64|x86_64)          ESUM='98615b1b369509965a612232622d39b5cefe117d6189179cbad4dcef2ee2f4e1';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.8%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.8_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 21:57:36 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 22:37:06 GMT
CMD ["groovysh"]
# Wed, 19 Aug 2020 22:37:06 GMT
ENV GROOVY_HOME=/opt/groovy
# Wed, 19 Aug 2020 22:37:08 GMT
RUN set -o errexit -o nounset     && echo "Adding groovy user and group"     && groupadd --system --gid 1000 groovy     && useradd --system --gid groovy --uid 1000 --shell /bin/bash --create-home groovy     && mkdir --parents /home/groovy/.groovy/grapes     && chown --recursive groovy:groovy /home/groovy     && chmod --recursive 1777 /home/groovy         && echo "Symlinking root .groovy to groovy .groovy"     && ln --symbolic /home/groovy/.groovy /root/.groovy
# Wed, 19 Aug 2020 22:37:08 GMT
VOLUME [/home/groovy/.groovy/grapes]
# Wed, 19 Aug 2020 22:37:08 GMT
WORKDIR /home/groovy
# Wed, 19 Aug 2020 22:37:15 GMT
RUN apt-get update     && echo "Installing build dependencies"     && apt-get install --yes --no-install-recommends         dirmngr         fontconfig         gnupg         unzip         wget     && rm --recursive --force /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:37:15 GMT
ENV GROOVY_VERSION=3.0.5
# Wed, 19 Aug 2020 22:37:21 GMT
RUN set -o errexit -o nounset     && echo "Downloading Groovy"     && wget --no-verbose --output-document=groovy.zip "https://archive.apache.org/dist/groovy/${GROOVY_VERSION}/distribution/apache-groovy-binary-${GROOVY_VERSION}.zip"         && echo "Importing keys listed in http://www.apache.org/dist/groovy/KEYS from key server"     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --no-tty --keyserver ha.pool.sks-keyservers.net --recv-keys         7FAA0F2206DE228F0DB01AD741321490758AAD6F         331224E1D7BE883D16E8A685825C06C827AF6B66         34441E504A937F43EB0DAEF96A65176A0FB1CD0B         9A810E3B766E089FFB27C70F11B595CEDC4AEBB5         81CABC23EECA0790E8989B361FF96E10F0E13706         && echo "Checking download signature"     && wget --no-verbose --output-document=groovy.zip.asc "https://archive.apache.org/dist/groovy/${GROOVY_VERSION}/distribution/apache-groovy-binary-${GROOVY_VERSION}.zip.asc"     && gpg --batch --no-tty --verify groovy.zip.asc groovy.zip     && rm --recursive --force "${GNUPGHOME}"     && rm groovy.zip.asc         && echo "Installing Groovy"     && unzip groovy.zip     && rm groovy.zip     && mv "groovy-${GROOVY_VERSION}" "${GROOVY_HOME}/"     && ln --symbolic "${GROOVY_HOME}/bin/grape" /usr/bin/grape     && ln --symbolic "${GROOVY_HOME}/bin/groovy" /usr/bin/groovy     && ln --symbolic "${GROOVY_HOME}/bin/groovyc" /usr/bin/groovyc     && ln --symbolic "${GROOVY_HOME}/bin/groovyConsole" /usr/bin/groovyConsole     && ln --symbolic "${GROOVY_HOME}/bin/groovydoc" /usr/bin/groovydoc     && ln --symbolic "${GROOVY_HOME}/bin/groovysh" /usr/bin/groovysh     && ln --symbolic "${GROOVY_HOME}/bin/java2groovy" /usr/bin/java2groovy         && echo "Editing startGroovy to include java.xml.bind module"     && sed --in-place 's|startGroovy ( ) {|startGroovy ( ) {\n    JAVA_OPTS="$JAVA_OPTS --add-modules=ALL-SYSTEM"|' "${GROOVY_HOME}/bin/startGroovy"
# Wed, 19 Aug 2020 22:37:21 GMT
USER groovy
# Wed, 19 Aug 2020 22:37:23 GMT
RUN set -o errexit -o nounset     && echo "Testing Groovy installation"     && groovy --version
```

-	Layers:
	-	`sha256:25294e13856fd30261115dbfc6dd49e2d854414d32c9ead824b8183a83620e5c`  
		Last Modified: Mon, 10 Aug 2020 15:49:57 GMT  
		Size: 25.4 MB (25371147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e4b14541a6306ab7ffae9ed980e3ebac039f590869efecf63c6d745e1cde3c`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 36.2 KB (36170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4164a02312fb3bccad51789030500218898a262ff17a962d62bb9849c9103d59`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68677136804619b55f0437044d91d7bfe75e0b8013ca953c0d4db40c4d91d6b`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201a00e3942c21b28b0a9c8923d0cc0469da5d7cb95cd09f08b52650c8a559a2`  
		Last Modified: Wed, 19 Aug 2020 22:03:03 GMT  
		Size: 13.6 MB (13595628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b27ca4bf2bfc98fb4540bce27fd4b077597cfde7fa7aea37e44318c5c020b6da`  
		Last Modified: Wed, 19 Aug 2020 22:03:53 GMT  
		Size: 38.2 MB (38172445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c6714246383257a42065afd26959c4a353885691160a7fe940f6c5cd5a9750c`  
		Last Modified: Wed, 19 Aug 2020 22:39:17 GMT  
		Size: 4.6 KB (4551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5b9e7b5cb0374462c198f16cf77eeae4edb8df02015686b8bc9f10363b3409`  
		Last Modified: Wed, 19 Aug 2020 22:39:17 GMT  
		Size: 3.5 MB (3455993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b54f47a66eebb28734b5697620c0c8952e47a3bd29275fbcf5cb2d4e421140e`  
		Last Modified: Wed, 19 Aug 2020 22:39:20 GMT  
		Size: 45.7 MB (45691480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c05199ee395d9386e02f4da65587eb2a90d7f69cfd8c80dac2ec2f1f8bdc71b`  
		Last Modified: Wed, 19 Aug 2020 22:39:17 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
