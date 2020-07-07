## `groovy:jre`

```console
$ docker pull groovy@sha256:501adeeefb7c3c4bf76e99045bc86d452c099b47e07476a0e5c028d71ee488b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `groovy:jre` - linux; amd64

```console
$ docker pull groovy@sha256:51f22defcc9aebd5a404d629d451edc99274663e5b20dae548c76ddd71e08e66
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128150293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44b66a9242583d2f7c6a6498fc2aa25870bba47757b82793ade4b2fc9bf50869`
-	Default Command: `["groovysh"]`

```dockerfile
# Mon, 06 Jul 2020 21:56:08 GMT
ADD file:0b40d881e3e00d68de1f1df0a565385bb838144b83814df891c994f466e9efa2 in / 
# Mon, 06 Jul 2020 21:56:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 21:56:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:56:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:56:11 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:03:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 06 Jul 2020 23:03:21 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 23:03:21 GMT
ENV JAVA_VERSION=jdk8u252-b09
# Mon, 06 Jul 2020 23:03:37 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='30bba4425497f5b4aabcba7b45db69d582d278fb17357d64c22c9dc6b2d29ca1';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u252b09.tar.gz';          ;;        armhf|armv7l)          ESUM='107699a88f611e0c2d57816be25821ef9b17db860b14402c4e9e5bf0b9cf16fd';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_arm_linux_hotspot_8u252b09.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='fbc559e8f75107f3c2ef92b33938dd48aee5728d471774d04fa3f68ed3b992fe';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u252b09.tar.gz';          ;;        s390x)          ESUM='23daa316ebcd965197e74dff011708a050516cd108a27a40e5b5cfa3c88beaba';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_s390x_linux_hotspot_8u252b09.tar.gz';          ;;        amd64|x86_64)          ESUM='a93be303ed62398dba9acb0376fb3caf8f488fcde80dc62d0a8e46256b3adfb1';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_x64_linux_hotspot_8u252b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 06 Jul 2020 23:03:37 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jul 2020 03:20:26 GMT
CMD ["groovysh"]
# Tue, 07 Jul 2020 03:20:26 GMT
ENV GROOVY_HOME=/opt/groovy
# Tue, 07 Jul 2020 03:20:27 GMT
RUN set -o errexit -o nounset     && echo "Adding groovy user and group"     && groupadd --system --gid 1000 groovy     && useradd --system --gid groovy --uid 1000 --shell /bin/bash --create-home groovy     && mkdir --parents /home/groovy/.groovy/grapes     && chown --recursive groovy:groovy /home/groovy         && echo "Symlinking root .groovy to groovy .groovy"     && ln --symbolic /home/groovy/.groovy /root/.groovy
# Tue, 07 Jul 2020 03:20:27 GMT
VOLUME [/home/groovy/.groovy/grapes]
# Tue, 07 Jul 2020 03:20:27 GMT
WORKDIR /home/groovy
# Tue, 07 Jul 2020 03:20:33 GMT
RUN apt-get update     && echo "Installing build dependencies"     && apt-get install --yes --no-install-recommends         dirmngr         fontconfig         gnupg         unzip         wget     && rm --recursive --force /var/lib/apt/lists/*
# Tue, 07 Jul 2020 03:20:34 GMT
ENV GROOVY_VERSION=3.0.4
# Tue, 07 Jul 2020 03:20:56 GMT
RUN set -o errexit -o nounset     && echo "Downloading Groovy"     && wget --no-verbose --output-document=groovy.zip "https://archive.apache.org/dist/groovy/${GROOVY_VERSION}/distribution/apache-groovy-binary-${GROOVY_VERSION}.zip"         && echo "Importing keys listed in http://www.apache.org/dist/groovy/KEYS from key server"     && export GNUPGHOME="$(mktemp -d)";     for key in         "7FAA0F2206DE228F0DB01AD741321490758AAD6F"         "331224E1D7BE883D16E8A685825C06C827AF6B66"         "34441E504A937F43EB0DAEF96A65176A0FB1CD0B"         "9A810E3B766E089FFB27C70F11B595CEDC4AEBB5"         "81CABC23EECA0790E8989B361FF96E10F0E13706"     ; do         for server in             "ha.pool.sks-keyservers.net"             "hkp://p80.pool.sks-keyservers.net:80"             "pgp.mit.edu"         ; do             echo "  Trying ${server}";             if gpg --batch --no-tty --keyserver "${server}" --recv-keys "${key}"; then                 break;             fi;         done;     done;     if [ $(gpg --batch --no-tty --list-keys | grep --count "pub ") -ne 5 ]; then         echo "ERROR: Failed to fetch GPG keys" >&2;         exit 1;     fi         && echo "Checking download signature"     && wget --no-verbose --output-document=groovy.zip.asc "https://archive.apache.org/dist/groovy/${GROOVY_VERSION}/distribution/apache-groovy-binary-${GROOVY_VERSION}.zip.asc"     && gpg --batch --no-tty --verify groovy.zip.asc groovy.zip     && rm --recursive --force "${GNUPGHOME}"     && rm groovy.zip.asc         && echo "Installing Groovy"     && unzip groovy.zip     && rm groovy.zip     && mv "groovy-${GROOVY_VERSION}" "${GROOVY_HOME}/"     && ln --symbolic "${GROOVY_HOME}/bin/grape" /usr/bin/grape     && ln --symbolic "${GROOVY_HOME}/bin/groovy" /usr/bin/groovy     && ln --symbolic "${GROOVY_HOME}/bin/groovyc" /usr/bin/groovyc     && ln --symbolic "${GROOVY_HOME}/bin/groovyConsole" /usr/bin/groovyConsole     && ln --symbolic "${GROOVY_HOME}/bin/groovydoc" /usr/bin/groovydoc     && ln --symbolic "${GROOVY_HOME}/bin/groovysh" /usr/bin/groovysh     && ln --symbolic "${GROOVY_HOME}/bin/java2groovy" /usr/bin/java2groovy
# Tue, 07 Jul 2020 03:20:56 GMT
USER groovy
# Tue, 07 Jul 2020 03:20:59 GMT
RUN set -o errexit -o nounset     && echo "Testing Groovy installation"     && groovy --version
```

-	Layers:
	-	`sha256:a1125296b23d78a3585a7910d649fbf0cc56284f9d2066e3243e8bc18f90b308`  
		Last Modified: Wed, 01 Jul 2020 12:21:40 GMT  
		Size: 26.7 MB (26696193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c742a4a0f38c95e690ad2dad8909c0cb232911418ac94a73da2a28becc7b734`  
		Last Modified: Mon, 06 Jul 2020 21:57:18 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ea3b329965bf7239f4e4f484915a444ec6d78b532ae12525934d4f6f7ac9a`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4be91ead68299f53759fd80c135e0dde0eb797e91eb8fbc5a708a506e0c433`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cbfb179272dc9aa9a0a4722b2f8ffe1d0cdb83652c091add1d0c091d505468e`  
		Last Modified: Mon, 06 Jul 2020 23:07:26 GMT  
		Size: 13.3 MB (13311646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7092168735a178c86270ca696ef6f3121c32c9fb7431c9472f72806f474d73`  
		Last Modified: Mon, 06 Jul 2020 23:07:46 GMT  
		Size: 41.5 MB (41453839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7f8103c29a500f9fb7c3bffdd47eb3d2a358957b9c5d387850e4d57ffeb9e0`  
		Last Modified: Tue, 07 Jul 2020 03:25:24 GMT  
		Size: 4.5 KB (4511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef562c3ba4fc17f78833c48855f7d632dcab5b3b7d876180bbfa99e41baa274`  
		Last Modified: Tue, 07 Jul 2020 03:25:24 GMT  
		Size: 3.4 MB (3444930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53356763f42413a822241ea42fe8876482ebb43e53a7f8cc58ba22907f0831cc`  
		Last Modified: Tue, 07 Jul 2020 03:25:27 GMT  
		Size: 43.2 MB (43202655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d88b1df638abfd5bfa1be4b0e881b863264e5dac2db7d1490353c4c4aeef5fd`  
		Last Modified: Tue, 07 Jul 2020 03:25:24 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `groovy:jre` - linux; ppc64le

```console
$ docker pull groovy@sha256:d593daead483274192d4f5c2623f11e459bd9ef669081b9b421a92da770c4586
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.3 MB (132343406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:994b3e6df2da10fd40614339bbcc11319ad2a7eaee635827a1ca9086b2c4806a`
-	Default Command: `["groovysh"]`

```dockerfile
# Wed, 17 Jun 2020 01:23:28 GMT
ADD file:3d8a4167931b708419d8f212295ee2e69c2e17523d93de0f36af7c8b7adaf6b0 in / 
# Wed, 17 Jun 2020 01:23:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 17 Jun 2020 01:23:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 17 Jun 2020 01:23:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 17 Jun 2020 01:23:59 GMT
CMD ["/bin/bash"]
# Wed, 17 Jun 2020 03:25:24 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 17 Jun 2020 03:26:55 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Jun 2020 03:27:02 GMT
ENV JAVA_VERSION=jdk8u252-b09
# Wed, 17 Jun 2020 03:28:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='30bba4425497f5b4aabcba7b45db69d582d278fb17357d64c22c9dc6b2d29ca1';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u252b09.tar.gz';          ;;        armhf|armv7l)          ESUM='107699a88f611e0c2d57816be25821ef9b17db860b14402c4e9e5bf0b9cf16fd';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_arm_linux_hotspot_8u252b09.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='fbc559e8f75107f3c2ef92b33938dd48aee5728d471774d04fa3f68ed3b992fe';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u252b09.tar.gz';          ;;        s390x)          ESUM='23daa316ebcd965197e74dff011708a050516cd108a27a40e5b5cfa3c88beaba';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_s390x_linux_hotspot_8u252b09.tar.gz';          ;;        amd64|x86_64)          ESUM='a93be303ed62398dba9acb0376fb3caf8f488fcde80dc62d0a8e46256b3adfb1';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_x64_linux_hotspot_8u252b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 17 Jun 2020 03:28:11 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Jun 2020 06:12:25 GMT
CMD ["groovysh"]
# Wed, 17 Jun 2020 06:12:27 GMT
ENV GROOVY_HOME=/opt/groovy
# Wed, 17 Jun 2020 06:12:40 GMT
RUN set -o errexit -o nounset     && echo "Adding groovy user and group"     && groupadd --system --gid 1000 groovy     && useradd --system --gid groovy --uid 1000 --shell /bin/bash --create-home groovy     && mkdir --parents /home/groovy/.groovy/grapes     && chown --recursive groovy:groovy /home/groovy         && echo "Symlinking root .groovy to groovy .groovy"     && ln --symbolic /home/groovy/.groovy /root/.groovy
# Wed, 17 Jun 2020 06:12:44 GMT
VOLUME [/home/groovy/.groovy/grapes]
# Wed, 17 Jun 2020 06:12:50 GMT
WORKDIR /home/groovy
# Wed, 17 Jun 2020 06:13:37 GMT
RUN apt-get update     && echo "Installing build dependencies"     && apt-get install --yes --no-install-recommends         dirmngr         fontconfig         gnupg         unzip         wget     && rm --recursive --force /var/lib/apt/lists/*
# Wed, 17 Jun 2020 06:13:39 GMT
ENV GROOVY_VERSION=3.0.4
# Wed, 17 Jun 2020 06:14:07 GMT
RUN set -o errexit -o nounset     && echo "Downloading Groovy"     && wget --no-verbose --output-document=groovy.zip "https://archive.apache.org/dist/groovy/${GROOVY_VERSION}/distribution/apache-groovy-binary-${GROOVY_VERSION}.zip"         && echo "Importing keys listed in http://www.apache.org/dist/groovy/KEYS from key server"     && export GNUPGHOME="$(mktemp -d)";     for key in         "7FAA0F2206DE228F0DB01AD741321490758AAD6F"         "331224E1D7BE883D16E8A685825C06C827AF6B66"         "34441E504A937F43EB0DAEF96A65176A0FB1CD0B"         "9A810E3B766E089FFB27C70F11B595CEDC4AEBB5"         "81CABC23EECA0790E8989B361FF96E10F0E13706"     ; do         for server in             "ha.pool.sks-keyservers.net"             "hkp://p80.pool.sks-keyservers.net:80"             "pgp.mit.edu"         ; do             echo "  Trying ${server}";             if gpg --batch --no-tty --keyserver "${server}" --recv-keys "${key}"; then                 break;             fi;         done;     done;     if [ $(gpg --batch --no-tty --list-keys | grep --count "pub ") -ne 5 ]; then         echo "ERROR: Failed to fetch GPG keys" >&2;         exit 1;     fi         && echo "Checking download signature"     && wget --no-verbose --output-document=groovy.zip.asc "https://archive.apache.org/dist/groovy/${GROOVY_VERSION}/distribution/apache-groovy-binary-${GROOVY_VERSION}.zip.asc"     && gpg --batch --no-tty --verify groovy.zip.asc groovy.zip     && rm --recursive --force "${GNUPGHOME}"     && rm groovy.zip.asc         && echo "Installing Groovy"     && unzip groovy.zip     && rm groovy.zip     && mv "groovy-${GROOVY_VERSION}" "${GROOVY_HOME}/"     && ln --symbolic "${GROOVY_HOME}/bin/grape" /usr/bin/grape     && ln --symbolic "${GROOVY_HOME}/bin/groovy" /usr/bin/groovy     && ln --symbolic "${GROOVY_HOME}/bin/groovyc" /usr/bin/groovyc     && ln --symbolic "${GROOVY_HOME}/bin/groovyConsole" /usr/bin/groovyConsole     && ln --symbolic "${GROOVY_HOME}/bin/groovydoc" /usr/bin/groovydoc     && ln --symbolic "${GROOVY_HOME}/bin/groovysh" /usr/bin/groovysh     && ln --symbolic "${GROOVY_HOME}/bin/java2groovy" /usr/bin/java2groovy
# Wed, 17 Jun 2020 06:14:09 GMT
USER groovy
# Wed, 17 Jun 2020 06:14:20 GMT
RUN set -o errexit -o nounset     && echo "Testing Groovy installation"     && groovy --version
```

-	Layers:
	-	`sha256:c82758296165adcddbc1b265a621d9938f9c807decd8469ae7f939d875188bf5`  
		Last Modified: Sat, 30 May 2020 05:26:15 GMT  
		Size: 30.4 MB (30400411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740d34e8b0154512b13d50a28cb641b322092ef53e5681dd77102035104fbffe`  
		Last Modified: Wed, 17 Jun 2020 01:28:15 GMT  
		Size: 35.2 KB (35202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e49637d96cd01435b847808eee898f2f13837bf3034497154962bb88ef0416b`  
		Last Modified: Wed, 17 Jun 2020 01:28:15 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:042abc2d98a7172c5b211cb1f6be22813334814c096e94c8fbf0a7972587d765`  
		Last Modified: Wed, 17 Jun 2020 01:28:15 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a910ee11e6ad058caab92c085018fc0da3bfc7f3d1bb0c650f7aa3eb0c7d7c`  
		Last Modified: Wed, 17 Jun 2020 03:39:07 GMT  
		Size: 14.0 MB (13955963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90739ca271e82feff463d6af0e29086f490f7edbabf11442d42c6716eb1d7793`  
		Last Modified: Wed, 17 Jun 2020 03:39:38 GMT  
		Size: 40.5 MB (40529112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee2faaace448274f4df30411188f8c25a0053e5ba1019312b6eee2ef06fe5a3`  
		Last Modified: Wed, 17 Jun 2020 06:31:43 GMT  
		Size: 4.5 KB (4546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed517b74ea29379356ef2af5683f69771ce45e5e98638adc087018744eac9d8a`  
		Last Modified: Wed, 17 Jun 2020 06:31:44 GMT  
		Size: 4.2 MB (4214339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac87f9893a0784b0c13bbdd6d80f3dec3f4fd7e2b37a7f8292920ecd1f466a78`  
		Last Modified: Wed, 17 Jun 2020 06:31:48 GMT  
		Size: 43.2 MB (43202623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50089389d74a7c72a6f03d45213efec365cfb3ba609c9c61c57959d66ee6395b`  
		Last Modified: Wed, 17 Jun 2020 06:31:43 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `groovy:jre` - linux; s390x

```console
$ docker pull groovy@sha256:86e09428c999671c6f5de47c0ad3df11e4da8e4cdb3b4e0ce2a307a098d9354e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124206401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5eda2b678931075b8b8b53e3940451fa797ef761e59d708eb048e7736ccceb23`
-	Default Command: `["groovysh"]`

```dockerfile
# Mon, 06 Jul 2020 20:20:02 GMT
ADD file:f3c111a69da215610cbc8041a61a2d38e6749f9a4f8d858869f241dfb4387a16 in / 
# Mon, 06 Jul 2020 20:20:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 20:20:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 20:20:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 20:20:06 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 21:07:07 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 06 Jul 2020 21:07:19 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 21:07:20 GMT
ENV JAVA_VERSION=jdk8u252-b09
# Mon, 06 Jul 2020 21:08:00 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='30bba4425497f5b4aabcba7b45db69d582d278fb17357d64c22c9dc6b2d29ca1';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u252b09.tar.gz';          ;;        armhf|armv7l)          ESUM='107699a88f611e0c2d57816be25821ef9b17db860b14402c4e9e5bf0b9cf16fd';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_arm_linux_hotspot_8u252b09.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='fbc559e8f75107f3c2ef92b33938dd48aee5728d471774d04fa3f68ed3b992fe';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u252b09.tar.gz';          ;;        s390x)          ESUM='23daa316ebcd965197e74dff011708a050516cd108a27a40e5b5cfa3c88beaba';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_s390x_linux_hotspot_8u252b09.tar.gz';          ;;        amd64|x86_64)          ESUM='a93be303ed62398dba9acb0376fb3caf8f488fcde80dc62d0a8e46256b3adfb1';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_x64_linux_hotspot_8u252b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 06 Jul 2020 21:08:01 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 06 Jul 2020 21:47:19 GMT
CMD ["groovysh"]
# Mon, 06 Jul 2020 21:47:20 GMT
ENV GROOVY_HOME=/opt/groovy
# Mon, 06 Jul 2020 21:47:20 GMT
RUN set -o errexit -o nounset     && echo "Adding groovy user and group"     && groupadd --system --gid 1000 groovy     && useradd --system --gid groovy --uid 1000 --shell /bin/bash --create-home groovy     && mkdir --parents /home/groovy/.groovy/grapes     && chown --recursive groovy:groovy /home/groovy         && echo "Symlinking root .groovy to groovy .groovy"     && ln --symbolic /home/groovy/.groovy /root/.groovy
# Mon, 06 Jul 2020 21:47:21 GMT
VOLUME [/home/groovy/.groovy/grapes]
# Mon, 06 Jul 2020 21:47:21 GMT
WORKDIR /home/groovy
# Mon, 06 Jul 2020 21:47:40 GMT
RUN apt-get update     && echo "Installing build dependencies"     && apt-get install --yes --no-install-recommends         dirmngr         fontconfig         gnupg         unzip         wget     && rm --recursive --force /var/lib/apt/lists/*
# Mon, 06 Jul 2020 21:47:40 GMT
ENV GROOVY_VERSION=3.0.4
# Mon, 06 Jul 2020 21:47:45 GMT
RUN set -o errexit -o nounset     && echo "Downloading Groovy"     && wget --no-verbose --output-document=groovy.zip "https://archive.apache.org/dist/groovy/${GROOVY_VERSION}/distribution/apache-groovy-binary-${GROOVY_VERSION}.zip"         && echo "Importing keys listed in http://www.apache.org/dist/groovy/KEYS from key server"     && export GNUPGHOME="$(mktemp -d)";     for key in         "7FAA0F2206DE228F0DB01AD741321490758AAD6F"         "331224E1D7BE883D16E8A685825C06C827AF6B66"         "34441E504A937F43EB0DAEF96A65176A0FB1CD0B"         "9A810E3B766E089FFB27C70F11B595CEDC4AEBB5"         "81CABC23EECA0790E8989B361FF96E10F0E13706"     ; do         for server in             "ha.pool.sks-keyservers.net"             "hkp://p80.pool.sks-keyservers.net:80"             "pgp.mit.edu"         ; do             echo "  Trying ${server}";             if gpg --batch --no-tty --keyserver "${server}" --recv-keys "${key}"; then                 break;             fi;         done;     done;     if [ $(gpg --batch --no-tty --list-keys | grep --count "pub ") -ne 5 ]; then         echo "ERROR: Failed to fetch GPG keys" >&2;         exit 1;     fi         && echo "Checking download signature"     && wget --no-verbose --output-document=groovy.zip.asc "https://archive.apache.org/dist/groovy/${GROOVY_VERSION}/distribution/apache-groovy-binary-${GROOVY_VERSION}.zip.asc"     && gpg --batch --no-tty --verify groovy.zip.asc groovy.zip     && rm --recursive --force "${GNUPGHOME}"     && rm groovy.zip.asc         && echo "Installing Groovy"     && unzip groovy.zip     && rm groovy.zip     && mv "groovy-${GROOVY_VERSION}" "${GROOVY_HOME}/"     && ln --symbolic "${GROOVY_HOME}/bin/grape" /usr/bin/grape     && ln --symbolic "${GROOVY_HOME}/bin/groovy" /usr/bin/groovy     && ln --symbolic "${GROOVY_HOME}/bin/groovyc" /usr/bin/groovyc     && ln --symbolic "${GROOVY_HOME}/bin/groovyConsole" /usr/bin/groovyConsole     && ln --symbolic "${GROOVY_HOME}/bin/groovydoc" /usr/bin/groovydoc     && ln --symbolic "${GROOVY_HOME}/bin/groovysh" /usr/bin/groovysh     && ln --symbolic "${GROOVY_HOME}/bin/java2groovy" /usr/bin/java2groovy
# Mon, 06 Jul 2020 21:47:46 GMT
USER groovy
# Mon, 06 Jul 2020 21:47:48 GMT
RUN set -o errexit -o nounset     && echo "Testing Groovy installation"     && groovy --version
```

-	Layers:
	-	`sha256:28e0e3e5309088b077fbb1d0d5bc87312d135f941cc01b88f89cc31fc37c3c20`  
		Last Modified: Mon, 06 Jul 2020 15:47:42 GMT  
		Size: 25.4 MB (25369216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a60d244695bbfbff21ace7be41541efca640a589a81721aaa9fd052adafd948`  
		Last Modified: Mon, 06 Jul 2020 20:21:07 GMT  
		Size: 36.2 KB (36166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8720c5a5362b9307c4ca7b33e250024e9014696310ff5d0c27c28aa3fb7777a1`  
		Last Modified: Mon, 06 Jul 2020 20:21:13 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c97cd7825a55df19db98b48e2ebd8cdf86319af7f0a3afad027e6d19cc03cf8`  
		Last Modified: Mon, 06 Jul 2020 20:21:07 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4752791f924c0ee1b53766356e35e30e455d055f61cca41c86a87d9bea3f57`  
		Last Modified: Mon, 06 Jul 2020 21:12:59 GMT  
		Size: 13.0 MB (13032773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a169e556d34728ba8a44ee0dc13ad7ed6044b7e82886c4d5c30653d6747213`  
		Last Modified: Mon, 06 Jul 2020 21:13:20 GMT  
		Size: 39.2 MB (39161268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9a104ebd3896b69af7af08a32971fd4b5053201aa079a20f495de387768c7c`  
		Last Modified: Mon, 06 Jul 2020 21:49:34 GMT  
		Size: 4.5 KB (4548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa655754f00e6eec5fbe24d98806fd2f3f8b53d35456e14863dd9fea5a6495d2`  
		Last Modified: Mon, 06 Jul 2020 21:49:34 GMT  
		Size: 3.4 MB (3398596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec55f16bf6cd4b599f33ecc3d263fd6dc637f7a7eccc7ba01f9d3ec7b4c12604`  
		Last Modified: Mon, 06 Jul 2020 21:49:41 GMT  
		Size: 43.2 MB (43202626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3426f39edeff2d53ed4f60d2a201d6b427895c99cac6f93a102b2523afb40b`  
		Last Modified: Mon, 06 Jul 2020 21:49:39 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
