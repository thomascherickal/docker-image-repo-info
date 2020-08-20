## `groovy:jdk14`

```console
$ docker pull groovy@sha256:b330112b55eae799ea9117d244a10da488da6d351f28262b80cf87070674d783
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `groovy:jdk14` - linux; amd64

```console
$ docker pull groovy@sha256:77f848ceac2834386567b2ce18652f334a02de3b4b6638cceebeaafd9f876dd2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.6 MB (301614922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae8fd4db0d9ab6a679c071069d68a2655fcb0ae837b6042c1dbac3585cd84250`
-	Default Command: `["groovysh"]`

```dockerfile
# Fri, 24 Jul 2020 14:38:19 GMT
ADD file:7d9bbf45a5b2510d44d3206a028cf6502757884d49e46d3d2e6356c3a92c4309 in / 
# Fri, 24 Jul 2020 14:38:20 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:22 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:16:41 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 24 Jul 2020 15:17:03 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:19:11 GMT
ENV JAVA_VERSION=jdk-14.0.2+12
# Fri, 24 Jul 2020 15:19:27 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='ee87e9f03b1fbe6f328429b78fe1a9f44900026d220c90dfd747fe0bcd62d904';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.2%2B12/OpenJDK14U-jdk_aarch64_linux_hotspot_14.0.2_12.tar.gz';          ;;        armhf|armv7l)          ESUM='65f193496c6977ba7aed1563edc4b5be091b5ff03e3d790074bb4e389a034b36';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.2%2B12/OpenJDK14U-jdk_arm_linux_hotspot_14.0.2_12.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='465a3b8e931896b8d95e452d479615c4bf543535c05b6ea246323ae114e67d7d';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.2%2B12/OpenJDK14U-jdk_ppc64le_linux_hotspot_14.0.2_12.tar.gz';          ;;        s390x)          ESUM='7d27aea30e359cf0bb561f8dcca6f4591dbc3ae831981f8a19aa367d31a9709b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.2%2B12/OpenJDK14U-jdk_s390x_linux_hotspot_14.0.2_12.tar.gz';          ;;        amd64|x86_64)          ESUM='7d5ee7e06909b8a99c0d029f512f67b092597aa5b0e78c109bd59405bbfa74fe';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.2%2B12/OpenJDK14U-jdk_x64_linux_hotspot_14.0.2_12.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 24 Jul 2020 15:19:27 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Jul 2020 15:19:28 GMT
CMD ["jshell"]
# Fri, 24 Jul 2020 20:03:30 GMT
CMD ["groovysh"]
# Fri, 24 Jul 2020 20:03:30 GMT
ENV GROOVY_HOME=/opt/groovy
# Fri, 24 Jul 2020 20:03:31 GMT
RUN set -o errexit -o nounset     && echo "Adding groovy user and group"     && groupadd --system --gid 1000 groovy     && useradd --system --gid groovy --uid 1000 --shell /bin/bash --create-home groovy     && mkdir --parents /home/groovy/.groovy/grapes     && chown --recursive groovy:groovy /home/groovy     && chmod --recursive 1777 /home/groovy         && echo "Symlinking root .groovy to groovy .groovy"     && ln --symbolic /home/groovy/.groovy /root/.groovy
# Fri, 24 Jul 2020 20:03:31 GMT
VOLUME [/home/groovy/.groovy/grapes]
# Fri, 24 Jul 2020 20:03:31 GMT
WORKDIR /home/groovy
# Fri, 24 Jul 2020 20:03:37 GMT
RUN apt-get update     && echo "Installing build dependencies"     && apt-get install --yes --no-install-recommends         dirmngr         fontconfig         gnupg         unzip         wget     && rm --recursive --force /var/lib/apt/lists/*
# Fri, 24 Jul 2020 20:03:37 GMT
ENV GROOVY_VERSION=3.0.5
# Fri, 24 Jul 2020 20:03:42 GMT
RUN set -o errexit -o nounset     && echo "Downloading Groovy"     && wget --no-verbose --output-document=groovy.zip "https://archive.apache.org/dist/groovy/${GROOVY_VERSION}/distribution/apache-groovy-binary-${GROOVY_VERSION}.zip"         && echo "Importing keys listed in http://www.apache.org/dist/groovy/KEYS from key server"     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --no-tty --keyserver ha.pool.sks-keyservers.net --recv-keys         7FAA0F2206DE228F0DB01AD741321490758AAD6F         331224E1D7BE883D16E8A685825C06C827AF6B66         34441E504A937F43EB0DAEF96A65176A0FB1CD0B         9A810E3B766E089FFB27C70F11B595CEDC4AEBB5         81CABC23EECA0790E8989B361FF96E10F0E13706         && echo "Checking download signature"     && wget --no-verbose --output-document=groovy.zip.asc "https://archive.apache.org/dist/groovy/${GROOVY_VERSION}/distribution/apache-groovy-binary-${GROOVY_VERSION}.zip.asc"     && gpg --batch --no-tty --verify groovy.zip.asc groovy.zip     && rm --recursive --force "${GNUPGHOME}"     && rm groovy.zip.asc         && echo "Installing Groovy"     && unzip groovy.zip     && rm groovy.zip     && mv "groovy-${GROOVY_VERSION}" "${GROOVY_HOME}/"     && ln --symbolic "${GROOVY_HOME}/bin/grape" /usr/bin/grape     && ln --symbolic "${GROOVY_HOME}/bin/groovy" /usr/bin/groovy     && ln --symbolic "${GROOVY_HOME}/bin/groovyc" /usr/bin/groovyc     && ln --symbolic "${GROOVY_HOME}/bin/groovyConsole" /usr/bin/groovyConsole     && ln --symbolic "${GROOVY_HOME}/bin/groovydoc" /usr/bin/groovydoc     && ln --symbolic "${GROOVY_HOME}/bin/groovysh" /usr/bin/groovysh     && ln --symbolic "${GROOVY_HOME}/bin/java2groovy" /usr/bin/java2groovy         && echo "Editing startGroovy to include java.xml.bind module"     && sed --in-place 's|startGroovy ( ) {|startGroovy ( ) {\n    JAVA_OPTS="$JAVA_OPTS --add-modules=ALL-SYSTEM"|' "${GROOVY_HOME}/bin/startGroovy"
# Fri, 24 Jul 2020 20:03:42 GMT
USER groovy
# Fri, 24 Jul 2020 20:03:45 GMT
RUN set -o errexit -o nounset     && echo "Testing Groovy installation"     && groovy --version
```

-	Layers:
	-	`sha256:7595c8c21622ea8a8b9778972e26dbbe063f7a1c4b0a28a80a34ebb3d343b586`  
		Last Modified: Mon, 13 Jul 2020 15:46:50 GMT  
		Size: 26.7 MB (26697127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13af8ca898f36af68711cb67c345f65046a78ccd802453f4b129adf9205b1f8`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70799171ddba93a611490ba3557d782714b3f4da8963d49ac8726786ba8274a5`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c12202c5ef07dc9eb8f9d9e71407064684ed70f8c4040b62679b7d30200840`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54d424eaa66f20b7926dbaa13c37d1c7c27c0e3113239f5608b4a57c157c399`  
		Last Modified: Fri, 24 Jul 2020 15:22:49 GMT  
		Size: 13.9 MB (13875512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe07aff1f5e556204e5b5eda4864b74aa299759cef1049375507a90298cfaf75`  
		Last Modified: Fri, 24 Jul 2020 15:25:14 GMT  
		Size: 211.8 MB (211807007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd714656905877269275cbef4797bea07892e6d89b4d2ee11d12e2ac1bcdaa5`  
		Last Modified: Fri, 24 Jul 2020 20:05:07 GMT  
		Size: 4.5 KB (4521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb2a711d5f2694d645c6e03de1ffdf8edc0611b871b27266d31377147e7baf9e`  
		Last Modified: Fri, 24 Jul 2020 20:05:08 GMT  
		Size: 3.5 MB (3502818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb7024e0e5d79a9d96cf7413573c9c084622daa135215783d3b54f0df985628`  
		Last Modified: Fri, 24 Jul 2020 20:05:11 GMT  
		Size: 45.7 MB (45691424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab87bac253c70278437c9ebafeee9c22cb9e1a5e3b650449dd09e27326387b32`  
		Last Modified: Fri, 24 Jul 2020 20:05:07 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `groovy:jdk14` - linux; arm variant v7

```console
$ docker pull groovy@sha256:2a855fad35f75a48c497ca29a7eba975d84751a2054f1f57a320087d0037d59d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.8 MB (281845181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b71affac3d41e41b77acfffb1edbf7e9a0150ded05bfe0b9223640fd3b36265e`
-	Default Command: `["groovysh"]`

```dockerfile
# Wed, 19 Aug 2020 21:45:03 GMT
ADD file:8369fef9339cb0f1b2b9660d860a6cbf4a5cd6c5e173fbb8cdf8b9485e56aaf4 in / 
# Wed, 19 Aug 2020 21:45:08 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:45:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:45:12 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:45:12 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:12:08 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 19 Aug 2020 22:12:37 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:15:18 GMT
ENV JAVA_VERSION=jdk-14.0.2+12
# Wed, 19 Aug 2020 22:15:40 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='ee87e9f03b1fbe6f328429b78fe1a9f44900026d220c90dfd747fe0bcd62d904';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.2%2B12/OpenJDK14U-jdk_aarch64_linux_hotspot_14.0.2_12.tar.gz';          ;;        armhf|armv7l)          ESUM='65f193496c6977ba7aed1563edc4b5be091b5ff03e3d790074bb4e389a034b36';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.2%2B12/OpenJDK14U-jdk_arm_linux_hotspot_14.0.2_12.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='465a3b8e931896b8d95e452d479615c4bf543535c05b6ea246323ae114e67d7d';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.2%2B12/OpenJDK14U-jdk_ppc64le_linux_hotspot_14.0.2_12.tar.gz';          ;;        s390x)          ESUM='7d27aea30e359cf0bb561f8dcca6f4591dbc3ae831981f8a19aa367d31a9709b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.2%2B12/OpenJDK14U-jdk_s390x_linux_hotspot_14.0.2_12.tar.gz';          ;;        amd64|x86_64)          ESUM='7d5ee7e06909b8a99c0d029f512f67b092597aa5b0e78c109bd59405bbfa74fe';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.2%2B12/OpenJDK14U-jdk_x64_linux_hotspot_14.0.2_12.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 22:15:42 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 22:15:43 GMT
CMD ["jshell"]
# Thu, 20 Aug 2020 00:03:16 GMT
CMD ["groovysh"]
# Thu, 20 Aug 2020 00:03:25 GMT
ENV GROOVY_HOME=/opt/groovy
# Thu, 20 Aug 2020 00:03:51 GMT
RUN set -o errexit -o nounset     && echo "Adding groovy user and group"     && groupadd --system --gid 1000 groovy     && useradd --system --gid groovy --uid 1000 --shell /bin/bash --create-home groovy     && mkdir --parents /home/groovy/.groovy/grapes     && chown --recursive groovy:groovy /home/groovy     && chmod --recursive 1777 /home/groovy         && echo "Symlinking root .groovy to groovy .groovy"     && ln --symbolic /home/groovy/.groovy /root/.groovy
# Thu, 20 Aug 2020 00:03:57 GMT
VOLUME [/home/groovy/.groovy/grapes]
# Thu, 20 Aug 2020 00:04:04 GMT
WORKDIR /home/groovy
# Thu, 20 Aug 2020 00:04:45 GMT
RUN apt-get update     && echo "Installing build dependencies"     && apt-get install --yes --no-install-recommends         dirmngr         fontconfig         gnupg         unzip         wget     && rm --recursive --force /var/lib/apt/lists/*
# Thu, 20 Aug 2020 00:04:51 GMT
ENV GROOVY_VERSION=3.0.5
# Thu, 20 Aug 2020 00:06:19 GMT
RUN set -o errexit -o nounset     && echo "Downloading Groovy"     && wget --no-verbose --output-document=groovy.zip "https://archive.apache.org/dist/groovy/${GROOVY_VERSION}/distribution/apache-groovy-binary-${GROOVY_VERSION}.zip"         && echo "Importing keys listed in http://www.apache.org/dist/groovy/KEYS from key server"     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --no-tty --keyserver ha.pool.sks-keyservers.net --recv-keys         7FAA0F2206DE228F0DB01AD741321490758AAD6F         331224E1D7BE883D16E8A685825C06C827AF6B66         34441E504A937F43EB0DAEF96A65176A0FB1CD0B         9A810E3B766E089FFB27C70F11B595CEDC4AEBB5         81CABC23EECA0790E8989B361FF96E10F0E13706         && echo "Checking download signature"     && wget --no-verbose --output-document=groovy.zip.asc "https://archive.apache.org/dist/groovy/${GROOVY_VERSION}/distribution/apache-groovy-binary-${GROOVY_VERSION}.zip.asc"     && gpg --batch --no-tty --verify groovy.zip.asc groovy.zip     && rm --recursive --force "${GNUPGHOME}"     && rm groovy.zip.asc         && echo "Installing Groovy"     && unzip groovy.zip     && rm groovy.zip     && mv "groovy-${GROOVY_VERSION}" "${GROOVY_HOME}/"     && ln --symbolic "${GROOVY_HOME}/bin/grape" /usr/bin/grape     && ln --symbolic "${GROOVY_HOME}/bin/groovy" /usr/bin/groovy     && ln --symbolic "${GROOVY_HOME}/bin/groovyc" /usr/bin/groovyc     && ln --symbolic "${GROOVY_HOME}/bin/groovyConsole" /usr/bin/groovyConsole     && ln --symbolic "${GROOVY_HOME}/bin/groovydoc" /usr/bin/groovydoc     && ln --symbolic "${GROOVY_HOME}/bin/groovysh" /usr/bin/groovysh     && ln --symbolic "${GROOVY_HOME}/bin/java2groovy" /usr/bin/java2groovy         && echo "Editing startGroovy to include java.xml.bind module"     && sed --in-place 's|startGroovy ( ) {|startGroovy ( ) {\n    JAVA_OPTS="$JAVA_OPTS --add-modules=ALL-SYSTEM"|' "${GROOVY_HOME}/bin/startGroovy"
# Thu, 20 Aug 2020 00:06:28 GMT
USER groovy
# Thu, 20 Aug 2020 00:06:59 GMT
RUN set -o errexit -o nounset     && echo "Testing Groovy installation"     && groovy --version
```

-	Layers:
	-	`sha256:854ab59e811f2c269687884c4899a5de08a5f65b6489dffdb58754086f21e5fc`  
		Last Modified: Mon, 10 Aug 2020 14:29:24 GMT  
		Size: 22.3 MB (22278969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996b7ca18b137080bed3caae4f18c24a2ae9b41a0bd9279d21fe013600e6dbf6`  
		Last Modified: Wed, 19 Aug 2020 21:47:13 GMT  
		Size: 35.5 KB (35458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a08dcf8afcac65e6356d202299b593954a299f9ebdb2db237496025225c8f2`  
		Last Modified: Wed, 19 Aug 2020 21:47:13 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34a2e7cb38ebbe96765deedfead50764f5a482a67ca440de7e9e660db464be7`  
		Last Modified: Wed, 19 Aug 2020 21:47:13 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c28a13f2c101b3996378f0c6d3848c55be63363f19fe99971b36de537e7d8b`  
		Last Modified: Wed, 19 Aug 2020 22:16:32 GMT  
		Size: 12.8 MB (12817129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03be241e4924eb9dc045924c213258aa2773bcb9a8e1a3d153f24810e75ae3f7`  
		Last Modified: Wed, 19 Aug 2020 22:19:38 GMT  
		Size: 198.0 MB (198004349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf10d8549b4b8ef40df74b11eba361bbb883a1d2cb52fb4b44022093da1e05bc`  
		Last Modified: Thu, 20 Aug 2020 00:07:41 GMT  
		Size: 4.5 KB (4534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71d8473969e19b5e2375ad35d0f1d9020573e9d9e2ef53bcff78c1fea4a7ec8`  
		Last Modified: Thu, 20 Aug 2020 00:07:42 GMT  
		Size: 3.0 MB (3012054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab1232cb4c4e6f43b76d31607b07672d9307bb0bd233fb1e21b339153c1ee9d2`  
		Last Modified: Thu, 20 Aug 2020 00:07:48 GMT  
		Size: 45.7 MB (45691476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12eba645a9f1140b4725f78abb27115c0cb4b8f996cbe4a0e817b8bd9ed87df1`  
		Last Modified: Thu, 20 Aug 2020 00:07:41 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `groovy:jdk14` - linux; arm64 variant v8

```console
$ docker pull groovy@sha256:6f8c36b853e07391e4b06ec26cf63b475b65dd504a366e0212d8c3a6bf2311c8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.2 MB (295201828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e5e20984316e2f2c1a0e9418076af152bf5c5eff790beb4ea23d6614c6c4618`
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
# Wed, 19 Aug 2020 22:52:54 GMT
ENV JAVA_VERSION=jdk-14.0.2+12
# Wed, 19 Aug 2020 22:53:13 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='ee87e9f03b1fbe6f328429b78fe1a9f44900026d220c90dfd747fe0bcd62d904';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.2%2B12/OpenJDK14U-jdk_aarch64_linux_hotspot_14.0.2_12.tar.gz';          ;;        armhf|armv7l)          ESUM='65f193496c6977ba7aed1563edc4b5be091b5ff03e3d790074bb4e389a034b36';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.2%2B12/OpenJDK14U-jdk_arm_linux_hotspot_14.0.2_12.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='465a3b8e931896b8d95e452d479615c4bf543535c05b6ea246323ae114e67d7d';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.2%2B12/OpenJDK14U-jdk_ppc64le_linux_hotspot_14.0.2_12.tar.gz';          ;;        s390x)          ESUM='7d27aea30e359cf0bb561f8dcca6f4591dbc3ae831981f8a19aa367d31a9709b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.2%2B12/OpenJDK14U-jdk_s390x_linux_hotspot_14.0.2_12.tar.gz';          ;;        amd64|x86_64)          ESUM='7d5ee7e06909b8a99c0d029f512f67b092597aa5b0e78c109bd59405bbfa74fe';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.2%2B12/OpenJDK14U-jdk_x64_linux_hotspot_14.0.2_12.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 22:53:15 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 22:53:16 GMT
CMD ["jshell"]
# Thu, 20 Aug 2020 01:09:53 GMT
CMD ["groovysh"]
# Thu, 20 Aug 2020 01:09:55 GMT
ENV GROOVY_HOME=/opt/groovy
# Thu, 20 Aug 2020 01:09:57 GMT
RUN set -o errexit -o nounset     && echo "Adding groovy user and group"     && groupadd --system --gid 1000 groovy     && useradd --system --gid groovy --uid 1000 --shell /bin/bash --create-home groovy     && mkdir --parents /home/groovy/.groovy/grapes     && chown --recursive groovy:groovy /home/groovy     && chmod --recursive 1777 /home/groovy         && echo "Symlinking root .groovy to groovy .groovy"     && ln --symbolic /home/groovy/.groovy /root/.groovy
# Thu, 20 Aug 2020 01:09:58 GMT
VOLUME [/home/groovy/.groovy/grapes]
# Thu, 20 Aug 2020 01:09:59 GMT
WORKDIR /home/groovy
# Thu, 20 Aug 2020 01:10:12 GMT
RUN apt-get update     && echo "Installing build dependencies"     && apt-get install --yes --no-install-recommends         dirmngr         fontconfig         gnupg         unzip         wget     && rm --recursive --force /var/lib/apt/lists/*
# Thu, 20 Aug 2020 01:10:13 GMT
ENV GROOVY_VERSION=3.0.5
# Thu, 20 Aug 2020 01:10:19 GMT
RUN set -o errexit -o nounset     && echo "Downloading Groovy"     && wget --no-verbose --output-document=groovy.zip "https://archive.apache.org/dist/groovy/${GROOVY_VERSION}/distribution/apache-groovy-binary-${GROOVY_VERSION}.zip"         && echo "Importing keys listed in http://www.apache.org/dist/groovy/KEYS from key server"     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --no-tty --keyserver ha.pool.sks-keyservers.net --recv-keys         7FAA0F2206DE228F0DB01AD741321490758AAD6F         331224E1D7BE883D16E8A685825C06C827AF6B66         34441E504A937F43EB0DAEF96A65176A0FB1CD0B         9A810E3B766E089FFB27C70F11B595CEDC4AEBB5         81CABC23EECA0790E8989B361FF96E10F0E13706         && echo "Checking download signature"     && wget --no-verbose --output-document=groovy.zip.asc "https://archive.apache.org/dist/groovy/${GROOVY_VERSION}/distribution/apache-groovy-binary-${GROOVY_VERSION}.zip.asc"     && gpg --batch --no-tty --verify groovy.zip.asc groovy.zip     && rm --recursive --force "${GNUPGHOME}"     && rm groovy.zip.asc         && echo "Installing Groovy"     && unzip groovy.zip     && rm groovy.zip     && mv "groovy-${GROOVY_VERSION}" "${GROOVY_HOME}/"     && ln --symbolic "${GROOVY_HOME}/bin/grape" /usr/bin/grape     && ln --symbolic "${GROOVY_HOME}/bin/groovy" /usr/bin/groovy     && ln --symbolic "${GROOVY_HOME}/bin/groovyc" /usr/bin/groovyc     && ln --symbolic "${GROOVY_HOME}/bin/groovyConsole" /usr/bin/groovyConsole     && ln --symbolic "${GROOVY_HOME}/bin/groovydoc" /usr/bin/groovydoc     && ln --symbolic "${GROOVY_HOME}/bin/groovysh" /usr/bin/groovysh     && ln --symbolic "${GROOVY_HOME}/bin/java2groovy" /usr/bin/java2groovy         && echo "Editing startGroovy to include java.xml.bind module"     && sed --in-place 's|startGroovy ( ) {|startGroovy ( ) {\n    JAVA_OPTS="$JAVA_OPTS --add-modules=ALL-SYSTEM"|' "${GROOVY_HOME}/bin/startGroovy"
# Thu, 20 Aug 2020 01:10:20 GMT
USER groovy
# Thu, 20 Aug 2020 01:10:24 GMT
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
	-	`sha256:35a26dad2b0b8a712da1c41fe72cba4c9958bf30ddde045c50a89c9aee3d5c5a`  
		Last Modified: Wed, 19 Aug 2020 22:57:29 GMT  
		Size: 209.2 MB (209228799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f45ebfe58b42660ee4dc52b85db4ee562ad0cb729f5ed02c9b4fb5db18b7d6b`  
		Last Modified: Thu, 20 Aug 2020 01:11:38 GMT  
		Size: 4.6 KB (4555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1a14f78a2d540af8464923ca86cae8c545bd8d7ce45c87865c5d6c2ec8cced`  
		Last Modified: Thu, 20 Aug 2020 01:11:39 GMT  
		Size: 3.2 MB (3233723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85ac62a8ecee3ade675d5134739f4a7a1a6330784609376dd9e9ad5aa0d355e`  
		Last Modified: Thu, 20 Aug 2020 01:11:44 GMT  
		Size: 45.7 MB (45691492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:668a58e5f6ec892347d8b2335933759cb02fe6a715c1104673aa253293b407f2`  
		Last Modified: Thu, 20 Aug 2020 01:11:38 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `groovy:jdk14` - linux; ppc64le

```console
$ docker pull groovy@sha256:31fec1020233fbdb9fe82dbb262f3dd525b6b7057aff89f6b712217734ee83a1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.5 MB (288489731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca579011e171a124475f3741596e6e025f132089f9aa9d094629452d3290da76`
-	Default Command: `["groovysh"]`

```dockerfile
# Fri, 24 Jul 2020 14:33:42 GMT
ADD file:d8c73324b090ba968a3efc4afc8af7d913766bd7787fc4cd6e4436895a4e564a in / 
# Fri, 24 Jul 2020 14:34:10 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:34:45 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:35:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:35:08 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:38:52 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 24 Jul 2020 15:45:16 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 16:01:15 GMT
ENV JAVA_VERSION=jdk-14.0.2+12
# Fri, 24 Jul 2020 16:02:03 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='ee87e9f03b1fbe6f328429b78fe1a9f44900026d220c90dfd747fe0bcd62d904';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.2%2B12/OpenJDK14U-jdk_aarch64_linux_hotspot_14.0.2_12.tar.gz';          ;;        armhf|armv7l)          ESUM='65f193496c6977ba7aed1563edc4b5be091b5ff03e3d790074bb4e389a034b36';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.2%2B12/OpenJDK14U-jdk_arm_linux_hotspot_14.0.2_12.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='465a3b8e931896b8d95e452d479615c4bf543535c05b6ea246323ae114e67d7d';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.2%2B12/OpenJDK14U-jdk_ppc64le_linux_hotspot_14.0.2_12.tar.gz';          ;;        s390x)          ESUM='7d27aea30e359cf0bb561f8dcca6f4591dbc3ae831981f8a19aa367d31a9709b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.2%2B12/OpenJDK14U-jdk_s390x_linux_hotspot_14.0.2_12.tar.gz';          ;;        amd64|x86_64)          ESUM='7d5ee7e06909b8a99c0d029f512f67b092597aa5b0e78c109bd59405bbfa74fe';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.2%2B12/OpenJDK14U-jdk_x64_linux_hotspot_14.0.2_12.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 24 Jul 2020 16:02:25 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Jul 2020 16:02:50 GMT
CMD ["jshell"]
# Fri, 24 Jul 2020 23:32:02 GMT
CMD ["groovysh"]
# Fri, 24 Jul 2020 23:32:09 GMT
ENV GROOVY_HOME=/opt/groovy
# Fri, 24 Jul 2020 23:32:24 GMT
RUN set -o errexit -o nounset     && echo "Adding groovy user and group"     && groupadd --system --gid 1000 groovy     && useradd --system --gid groovy --uid 1000 --shell /bin/bash --create-home groovy     && mkdir --parents /home/groovy/.groovy/grapes     && chown --recursive groovy:groovy /home/groovy     && chmod --recursive 1777 /home/groovy         && echo "Symlinking root .groovy to groovy .groovy"     && ln --symbolic /home/groovy/.groovy /root/.groovy
# Fri, 24 Jul 2020 23:32:27 GMT
VOLUME [/home/groovy/.groovy/grapes]
# Fri, 24 Jul 2020 23:32:35 GMT
WORKDIR /home/groovy
# Fri, 24 Jul 2020 23:33:17 GMT
RUN apt-get update     && echo "Installing build dependencies"     && apt-get install --yes --no-install-recommends         dirmngr         fontconfig         gnupg         unzip         wget     && rm --recursive --force /var/lib/apt/lists/*
# Fri, 24 Jul 2020 23:33:23 GMT
ENV GROOVY_VERSION=3.0.5
# Fri, 24 Jul 2020 23:33:55 GMT
RUN set -o errexit -o nounset     && echo "Downloading Groovy"     && wget --no-verbose --output-document=groovy.zip "https://archive.apache.org/dist/groovy/${GROOVY_VERSION}/distribution/apache-groovy-binary-${GROOVY_VERSION}.zip"         && echo "Importing keys listed in http://www.apache.org/dist/groovy/KEYS from key server"     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --no-tty --keyserver ha.pool.sks-keyservers.net --recv-keys         7FAA0F2206DE228F0DB01AD741321490758AAD6F         331224E1D7BE883D16E8A685825C06C827AF6B66         34441E504A937F43EB0DAEF96A65176A0FB1CD0B         9A810E3B766E089FFB27C70F11B595CEDC4AEBB5         81CABC23EECA0790E8989B361FF96E10F0E13706         && echo "Checking download signature"     && wget --no-verbose --output-document=groovy.zip.asc "https://archive.apache.org/dist/groovy/${GROOVY_VERSION}/distribution/apache-groovy-binary-${GROOVY_VERSION}.zip.asc"     && gpg --batch --no-tty --verify groovy.zip.asc groovy.zip     && rm --recursive --force "${GNUPGHOME}"     && rm groovy.zip.asc         && echo "Installing Groovy"     && unzip groovy.zip     && rm groovy.zip     && mv "groovy-${GROOVY_VERSION}" "${GROOVY_HOME}/"     && ln --symbolic "${GROOVY_HOME}/bin/grape" /usr/bin/grape     && ln --symbolic "${GROOVY_HOME}/bin/groovy" /usr/bin/groovy     && ln --symbolic "${GROOVY_HOME}/bin/groovyc" /usr/bin/groovyc     && ln --symbolic "${GROOVY_HOME}/bin/groovyConsole" /usr/bin/groovyConsole     && ln --symbolic "${GROOVY_HOME}/bin/groovydoc" /usr/bin/groovydoc     && ln --symbolic "${GROOVY_HOME}/bin/groovysh" /usr/bin/groovysh     && ln --symbolic "${GROOVY_HOME}/bin/java2groovy" /usr/bin/java2groovy         && echo "Editing startGroovy to include java.xml.bind module"     && sed --in-place 's|startGroovy ( ) {|startGroovy ( ) {\n    JAVA_OPTS="$JAVA_OPTS --add-modules=ALL-SYSTEM"|' "${GROOVY_HOME}/bin/startGroovy"
# Fri, 24 Jul 2020 23:33:59 GMT
USER groovy
# Fri, 24 Jul 2020 23:34:34 GMT
RUN set -o errexit -o nounset     && echo "Testing Groovy installation"     && groovy --version
```

-	Layers:
	-	`sha256:453712c8810fcce792c21167e028047a35328679a3bd4429b8837301315e9103`  
		Last Modified: Mon, 13 Jul 2020 15:47:10 GMT  
		Size: 30.4 MB (30404926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbb4638d99213e93a32d6945492539426ee3616d7ba413462a8b936268a56af`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 35.2 KB (35224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b0bd277b733224c67d835643aa13dd8a9b86bcc10023a393302b3861e9a7b8`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270c2b729d72bf4931bb8d6ccbd100e124e01bac9628380f36c2d0f13bdcc109`  
		Last Modified: Fri, 24 Jul 2020 14:41:31 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dd6970a3a6adb0cbcb037b053a7c0ea9480e9f5edf524c197aea5374c2cf495`  
		Last Modified: Fri, 24 Jul 2020 16:19:35 GMT  
		Size: 14.5 MB (14519278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b3b7e6c86cce5cd0b8efa457ddf2ae57278c70bc4b2b8e0f4050924c9833e2`  
		Last Modified: Fri, 24 Jul 2020 16:25:24 GMT  
		Size: 193.6 MB (193561543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a49a9cc535b448e5040428059a834c0f3fe1f140109dd33c832de074cd94d07`  
		Last Modified: Fri, 24 Jul 2020 23:39:48 GMT  
		Size: 4.6 KB (4566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c6797c39838a4af2a2915d5e4566489d0eb766244aa533c6db9e3b88472e17`  
		Last Modified: Fri, 24 Jul 2020 23:39:49 GMT  
		Size: 4.3 MB (4271505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09df9634af369950f8c100e12d087d0b820414c27d159ddd78065c53d9055bb6`  
		Last Modified: Fri, 24 Jul 2020 23:39:54 GMT  
		Size: 45.7 MB (45691476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47cd534615a12c07448f13323fc65a7c734024e7e0510a37cea5a7ed43e0c14e`  
		Last Modified: Fri, 24 Jul 2020 23:39:48 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `groovy:jdk14` - linux; s390x

```console
$ docker pull groovy@sha256:828a1b46369be50e653938408af73299ae36309e10afff964effbd5483a64a42
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.7 MB (272686812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8510a5cdacc0d495ba75f2641f1ff269ece715ce739da475dec769ad21aadefc`
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
# Wed, 19 Aug 2020 21:58:50 GMT
ENV JAVA_VERSION=jdk-14.0.2+12
# Wed, 19 Aug 2020 21:59:01 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='ee87e9f03b1fbe6f328429b78fe1a9f44900026d220c90dfd747fe0bcd62d904';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.2%2B12/OpenJDK14U-jdk_aarch64_linux_hotspot_14.0.2_12.tar.gz';          ;;        armhf|armv7l)          ESUM='65f193496c6977ba7aed1563edc4b5be091b5ff03e3d790074bb4e389a034b36';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.2%2B12/OpenJDK14U-jdk_arm_linux_hotspot_14.0.2_12.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='465a3b8e931896b8d95e452d479615c4bf543535c05b6ea246323ae114e67d7d';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.2%2B12/OpenJDK14U-jdk_ppc64le_linux_hotspot_14.0.2_12.tar.gz';          ;;        s390x)          ESUM='7d27aea30e359cf0bb561f8dcca6f4591dbc3ae831981f8a19aa367d31a9709b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.2%2B12/OpenJDK14U-jdk_s390x_linux_hotspot_14.0.2_12.tar.gz';          ;;        amd64|x86_64)          ESUM='7d5ee7e06909b8a99c0d029f512f67b092597aa5b0e78c109bd59405bbfa74fe';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.2%2B12/OpenJDK14U-jdk_x64_linux_hotspot_14.0.2_12.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 21:59:05 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 21:59:05 GMT
CMD ["jshell"]
# Wed, 19 Aug 2020 22:37:28 GMT
CMD ["groovysh"]
# Wed, 19 Aug 2020 22:37:28 GMT
ENV GROOVY_HOME=/opt/groovy
# Wed, 19 Aug 2020 22:37:29 GMT
RUN set -o errexit -o nounset     && echo "Adding groovy user and group"     && groupadd --system --gid 1000 groovy     && useradd --system --gid groovy --uid 1000 --shell /bin/bash --create-home groovy     && mkdir --parents /home/groovy/.groovy/grapes     && chown --recursive groovy:groovy /home/groovy     && chmod --recursive 1777 /home/groovy         && echo "Symlinking root .groovy to groovy .groovy"     && ln --symbolic /home/groovy/.groovy /root/.groovy
# Wed, 19 Aug 2020 22:37:29 GMT
VOLUME [/home/groovy/.groovy/grapes]
# Wed, 19 Aug 2020 22:37:30 GMT
WORKDIR /home/groovy
# Wed, 19 Aug 2020 22:37:37 GMT
RUN apt-get update     && echo "Installing build dependencies"     && apt-get install --yes --no-install-recommends         dirmngr         fontconfig         gnupg         unzip         wget     && rm --recursive --force /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:37:37 GMT
ENV GROOVY_VERSION=3.0.5
# Wed, 19 Aug 2020 22:37:43 GMT
RUN set -o errexit -o nounset     && echo "Downloading Groovy"     && wget --no-verbose --output-document=groovy.zip "https://archive.apache.org/dist/groovy/${GROOVY_VERSION}/distribution/apache-groovy-binary-${GROOVY_VERSION}.zip"         && echo "Importing keys listed in http://www.apache.org/dist/groovy/KEYS from key server"     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --no-tty --keyserver ha.pool.sks-keyservers.net --recv-keys         7FAA0F2206DE228F0DB01AD741321490758AAD6F         331224E1D7BE883D16E8A685825C06C827AF6B66         34441E504A937F43EB0DAEF96A65176A0FB1CD0B         9A810E3B766E089FFB27C70F11B595CEDC4AEBB5         81CABC23EECA0790E8989B361FF96E10F0E13706         && echo "Checking download signature"     && wget --no-verbose --output-document=groovy.zip.asc "https://archive.apache.org/dist/groovy/${GROOVY_VERSION}/distribution/apache-groovy-binary-${GROOVY_VERSION}.zip.asc"     && gpg --batch --no-tty --verify groovy.zip.asc groovy.zip     && rm --recursive --force "${GNUPGHOME}"     && rm groovy.zip.asc         && echo "Installing Groovy"     && unzip groovy.zip     && rm groovy.zip     && mv "groovy-${GROOVY_VERSION}" "${GROOVY_HOME}/"     && ln --symbolic "${GROOVY_HOME}/bin/grape" /usr/bin/grape     && ln --symbolic "${GROOVY_HOME}/bin/groovy" /usr/bin/groovy     && ln --symbolic "${GROOVY_HOME}/bin/groovyc" /usr/bin/groovyc     && ln --symbolic "${GROOVY_HOME}/bin/groovyConsole" /usr/bin/groovyConsole     && ln --symbolic "${GROOVY_HOME}/bin/groovydoc" /usr/bin/groovydoc     && ln --symbolic "${GROOVY_HOME}/bin/groovysh" /usr/bin/groovysh     && ln --symbolic "${GROOVY_HOME}/bin/java2groovy" /usr/bin/java2groovy         && echo "Editing startGroovy to include java.xml.bind module"     && sed --in-place 's|startGroovy ( ) {|startGroovy ( ) {\n    JAVA_OPTS="$JAVA_OPTS --add-modules=ALL-SYSTEM"|' "${GROOVY_HOME}/bin/startGroovy"
# Wed, 19 Aug 2020 22:37:45 GMT
USER groovy
# Wed, 19 Aug 2020 22:37:48 GMT
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
	-	`sha256:f52313f9402c6fe9f9db744d6d0aa6d68b49c286ac80ca5e84cefa3a54e6e420`  
		Last Modified: Wed, 19 Aug 2020 22:04:49 GMT  
		Size: 184.5 MB (184530610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5caf6216c6fe263c5e21f28b9d9fe66037b244704ac7abbfe907b808e1bb08eb`  
		Last Modified: Wed, 19 Aug 2020 22:39:27 GMT  
		Size: 4.5 KB (4550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713b2bf8569d5ec6a04d2c6d390d9be9a3ac42e58b95462a9838f50c08ab6314`  
		Last Modified: Wed, 19 Aug 2020 22:39:28 GMT  
		Size: 3.5 MB (3456019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd3d6d9142b8a8b225f53549176f597ea2dab460030b5865fb1280dfbc142c6`  
		Last Modified: Wed, 19 Aug 2020 22:39:30 GMT  
		Size: 45.7 MB (45691479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74fa775c0a4c778321fae40c35ff46533bd9721bff53c7039646d30b1208472`  
		Last Modified: Wed, 19 Aug 2020 22:39:27 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
