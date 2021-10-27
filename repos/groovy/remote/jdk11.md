## `groovy:jdk11`

```console
$ docker pull groovy@sha256:e406b67f0ad83a36399acffeb37527e1799e82df228b87b7121a632f2dd19c77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `groovy:jdk11` - linux; amd64

```console
$ docker pull groovy@sha256:f399be7499f181c83dae9912b14442ac5b4c969171cdde5d198d144070669fea
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.7 MB (286667451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1643adae5df7eb5434d8884f7154d341d093e806ef915cb09d5599b89d21830c`
-	Default Command: `["groovysh"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:44:06 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 16 Oct 2021 02:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Oct 2021 00:21:28 GMT
ENV JAVA_VERSION=jdk-11.0.13+8
# Wed, 27 Oct 2021 00:21:38 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='a77013bff10a5e9c59159231dd5c4bd071fc4c24beed42bd49b82803ba9506ef';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.13_8.tar.gz';          ;;        armhf|arm)          ESUM='61ee45c4ef21a85a116a87e1bca2e2a420b3af432be8d801bd52c660ffebaa9f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_arm_linux_hotspot_11.0.13_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='82f14cda71cff99c878bf8400598a87235adb6c81b0337f7077c27e5cac1190c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.13_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='9d280d86fdf6a7d9e5cbf54dc37f1d6d09dfe676ff5c684802fdfa3932eee63e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.13_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='3b1c0c34be4c894e64135a454f2d5aaa4bd10aea04ec2fa0c0efe6bb26528e30';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_hotspot_11.0.13_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 27 Oct 2021 00:21:39 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 27 Oct 2021 00:21:40 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 27 Oct 2021 00:21:40 GMT
CMD ["jshell"]
# Wed, 27 Oct 2021 00:54:08 GMT
CMD ["groovysh"]
# Wed, 27 Oct 2021 00:54:08 GMT
ENV GROOVY_HOME=/opt/groovy
# Wed, 27 Oct 2021 00:54:09 GMT
RUN set -o errexit -o nounset     && echo "Adding groovy user and group"     && groupadd --system --gid 1000 groovy     && useradd --system --gid groovy --uid 1000 --shell /bin/bash --create-home groovy     && mkdir --parents /home/groovy/.groovy/grapes     && chown --recursive groovy:groovy /home/groovy     && chmod --recursive 1777 /home/groovy         && echo "Symlinking root .groovy to groovy .groovy"     && ln --symbolic /home/groovy/.groovy /root/.groovy
# Wed, 27 Oct 2021 00:54:09 GMT
VOLUME [/home/groovy/.groovy/grapes]
# Wed, 27 Oct 2021 00:54:09 GMT
WORKDIR /home/groovy
# Wed, 27 Oct 2021 00:54:28 GMT
RUN apt-get update     && echo "Installing build dependencies"     && apt-get install --yes --no-install-recommends         dirmngr         fontconfig         gnupg         unzip         wget     && rm --recursive --force /var/lib/apt/lists/*
# Wed, 27 Oct 2021 00:54:29 GMT
ENV GROOVY_VERSION=3.0.9
# Wed, 27 Oct 2021 00:55:00 GMT
RUN set -o errexit -o nounset     && echo "Downloading Groovy"     && wget --no-verbose --output-document=groovy.zip "https://archive.apache.org/dist/groovy/${GROOVY_VERSION}/distribution/apache-groovy-binary-${GROOVY_VERSION}.zip"         && echo "Importing keys listed in http://www.apache.org/dist/groovy/KEYS from key server"     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --no-tty --keyserver keyserver.ubuntu.com --recv-keys         7FAA0F2206DE228F0DB01AD741321490758AAD6F         331224E1D7BE883D16E8A685825C06C827AF6B66         34441E504A937F43EB0DAEF96A65176A0FB1CD0B         9A810E3B766E089FFB27C70F11B595CEDC4AEBB5         81CABC23EECA0790E8989B361FF96E10F0E13706         && echo "Checking download signature"     && wget --no-verbose --output-document=groovy.zip.asc "https://archive.apache.org/dist/groovy/${GROOVY_VERSION}/distribution/apache-groovy-binary-${GROOVY_VERSION}.zip.asc"     && gpg --batch --no-tty --verify groovy.zip.asc groovy.zip     && rm --recursive --force "${GNUPGHOME}"     && rm groovy.zip.asc         && echo "Installing Groovy"     && unzip groovy.zip     && rm groovy.zip     && mv "groovy-${GROOVY_VERSION}" "${GROOVY_HOME}/"     && ln --symbolic "${GROOVY_HOME}/bin/grape" /usr/bin/grape     && ln --symbolic "${GROOVY_HOME}/bin/groovy" /usr/bin/groovy     && ln --symbolic "${GROOVY_HOME}/bin/groovyc" /usr/bin/groovyc     && ln --symbolic "${GROOVY_HOME}/bin/groovyConsole" /usr/bin/groovyConsole     && ln --symbolic "${GROOVY_HOME}/bin/groovydoc" /usr/bin/groovydoc     && ln --symbolic "${GROOVY_HOME}/bin/groovysh" /usr/bin/groovysh     && ln --symbolic "${GROOVY_HOME}/bin/java2groovy" /usr/bin/java2groovy         && echo "Editing startGroovy to include java.xml.bind module"     && sed --in-place 's|startGroovy ( ) {|startGroovy ( ) {\n    JAVA_OPTS="$JAVA_OPTS --add-modules=ALL-SYSTEM"|' "${GROOVY_HOME}/bin/startGroovy"
# Wed, 27 Oct 2021 00:55:00 GMT
USER groovy
# Wed, 27 Oct 2021 00:55:02 GMT
RUN set -o errexit -o nounset     && echo "Testing Groovy installation"     && groovy --version
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237daeb1ae282fe20092079ef6d5de7924746d0f2e9ad88797d08524a4d842fd`  
		Last Modified: Sat, 16 Oct 2021 02:47:20 GMT  
		Size: 16.0 MB (16036029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be95eabe2b75bbc37fb08d630d608002fba6a0887d04c57831e64037f792b5ec`  
		Last Modified: Wed, 27 Oct 2021 00:24:19 GMT  
		Size: 193.8 MB (193801873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147350fde7b86d0cd855faaeb68057169caa1eb122dcaefd9e9ad8ded307e693`  
		Last Modified: Wed, 27 Oct 2021 00:23:59 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6bdb638ee3a0f7732be04ad7b294bff4999ed49e93dcbb9f10a2123b140018a`  
		Last Modified: Wed, 27 Oct 2021 00:56:29 GMT  
		Size: 4.4 KB (4396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc9d127b5690b9dea9c9321197a4ff7455218934d4cf6a283b88b4f1b1adb6d`  
		Last Modified: Wed, 27 Oct 2021 00:56:31 GMT  
		Size: 4.2 MB (4150601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c1d83ee3999a53540467cd2d68043fc5918078ec202f5144d7a42c59cfe6fb`  
		Last Modified: Wed, 27 Oct 2021 00:56:33 GMT  
		Size: 44.1 MB (44107117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6016e5063e56b526ea9932001931f5b8682a5a628305850ffeef370f7c5c2a60`  
		Last Modified: Wed, 27 Oct 2021 00:56:30 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `groovy:jdk11` - linux; arm variant v7

```console
$ docker pull groovy@sha256:084e768f6c7dc08e28ac62691f556d24e119b8bf2011ad92a7404f7d48f20f4a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.4 MB (268362037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c4e1f7bd19425253e7ff898fa67228cc566af767ee03ebde4ba61715ee919de`
-	Default Command: `["groovysh"]`

```dockerfile
# Sat, 16 Oct 2021 01:12:00 GMT
ADD file:625e3906181f4bd86e59a0e9748f67fcb1391a2e65e36c729e71353381a49757 in / 
# Sat, 16 Oct 2021 01:12:00 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:38:37 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 16 Oct 2021 02:39:17 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:39:59 GMT
ENV JAVA_VERSION=jdk-11.0.12+7
# Sat, 16 Oct 2021 02:40:21 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='105bdc12fcd54c551e8e8ac96bc82412467244c32063689c41cee29ceb7452a2';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.12_7.tar.gz';          ;;        armhf|arm)          ESUM='85929246a9d60ed90e2385ea3f4857798c77019c5100f00189c1dd0a093abea7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_arm_linux_hotspot_11.0.12_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='234a9bafe029ea6cab5d46f9617b5d016a29faa187a42081d0e066f23647b7e5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.12_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='99c1c61e9d67b01a649687189e5a00f89a2371dc1bfed06bb078d127edfa7995';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.12_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='8770f600fc3b89bf331213c7aa21f8eedd9ca5d96036d1cd48cb2748a3dbefd2';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_x64_linux_hotspot_11.0.12_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 16 Oct 2021 02:40:23 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 16 Oct 2021 02:40:25 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Sat, 16 Oct 2021 02:40:25 GMT
CMD ["jshell"]
# Sat, 16 Oct 2021 04:43:42 GMT
CMD ["groovysh"]
# Sat, 16 Oct 2021 04:43:43 GMT
ENV GROOVY_HOME=/opt/groovy
# Sat, 16 Oct 2021 04:43:44 GMT
RUN set -o errexit -o nounset     && echo "Adding groovy user and group"     && groupadd --system --gid 1000 groovy     && useradd --system --gid groovy --uid 1000 --shell /bin/bash --create-home groovy     && mkdir --parents /home/groovy/.groovy/grapes     && chown --recursive groovy:groovy /home/groovy     && chmod --recursive 1777 /home/groovy         && echo "Symlinking root .groovy to groovy .groovy"     && ln --symbolic /home/groovy/.groovy /root/.groovy
# Sat, 16 Oct 2021 04:43:45 GMT
VOLUME [/home/groovy/.groovy/grapes]
# Sat, 16 Oct 2021 04:43:45 GMT
WORKDIR /home/groovy
# Sat, 16 Oct 2021 04:43:59 GMT
RUN apt-get update     && echo "Installing build dependencies"     && apt-get install --yes --no-install-recommends         dirmngr         fontconfig         gnupg         unzip         wget     && rm --recursive --force /var/lib/apt/lists/*
# Sat, 16 Oct 2021 04:43:59 GMT
ENV GROOVY_VERSION=3.0.9
# Sat, 16 Oct 2021 04:44:10 GMT
RUN set -o errexit -o nounset     && echo "Downloading Groovy"     && wget --no-verbose --output-document=groovy.zip "https://archive.apache.org/dist/groovy/${GROOVY_VERSION}/distribution/apache-groovy-binary-${GROOVY_VERSION}.zip"         && echo "Importing keys listed in http://www.apache.org/dist/groovy/KEYS from key server"     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --no-tty --keyserver keyserver.ubuntu.com --recv-keys         7FAA0F2206DE228F0DB01AD741321490758AAD6F         331224E1D7BE883D16E8A685825C06C827AF6B66         34441E504A937F43EB0DAEF96A65176A0FB1CD0B         9A810E3B766E089FFB27C70F11B595CEDC4AEBB5         81CABC23EECA0790E8989B361FF96E10F0E13706         && echo "Checking download signature"     && wget --no-verbose --output-document=groovy.zip.asc "https://archive.apache.org/dist/groovy/${GROOVY_VERSION}/distribution/apache-groovy-binary-${GROOVY_VERSION}.zip.asc"     && gpg --batch --no-tty --verify groovy.zip.asc groovy.zip     && rm --recursive --force "${GNUPGHOME}"     && rm groovy.zip.asc         && echo "Installing Groovy"     && unzip groovy.zip     && rm groovy.zip     && mv "groovy-${GROOVY_VERSION}" "${GROOVY_HOME}/"     && ln --symbolic "${GROOVY_HOME}/bin/grape" /usr/bin/grape     && ln --symbolic "${GROOVY_HOME}/bin/groovy" /usr/bin/groovy     && ln --symbolic "${GROOVY_HOME}/bin/groovyc" /usr/bin/groovyc     && ln --symbolic "${GROOVY_HOME}/bin/groovyConsole" /usr/bin/groovyConsole     && ln --symbolic "${GROOVY_HOME}/bin/groovydoc" /usr/bin/groovydoc     && ln --symbolic "${GROOVY_HOME}/bin/groovysh" /usr/bin/groovysh     && ln --symbolic "${GROOVY_HOME}/bin/java2groovy" /usr/bin/java2groovy         && echo "Editing startGroovy to include java.xml.bind module"     && sed --in-place 's|startGroovy ( ) {|startGroovy ( ) {\n    JAVA_OPTS="$JAVA_OPTS --add-modules=ALL-SYSTEM"|' "${GROOVY_HOME}/bin/startGroovy"
# Sat, 16 Oct 2021 04:44:10 GMT
USER groovy
# Sat, 16 Oct 2021 04:44:15 GMT
RUN set -o errexit -o nounset     && echo "Testing Groovy installation"     && groovy --version
```

-	Layers:
	-	`sha256:8795d4da4abd6abcafe7285749aa85d3a164999e84720a3845f764e56e306771`  
		Last Modified: Sat, 16 Oct 2021 01:15:01 GMT  
		Size: 24.1 MB (24064451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437a7367762ea761c5abbcde550ac6e83ab2fd882f50cc7c0b8a3ef2bcc5505b`  
		Last Modified: Sat, 16 Oct 2021 02:44:07 GMT  
		Size: 14.9 MB (14902308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3667f5a6bc892b9880cf4caac9de64baf32bcf66cabf8364980a650920776d`  
		Last Modified: Sat, 16 Oct 2021 02:46:03 GMT  
		Size: 181.7 MB (181705375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448b05efffeb432678bd6fded7691dcd3944db0a9c669046f18cc3f027ec2503`  
		Last Modified: Sat, 16 Oct 2021 02:44:54 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1988269c65603b2c4cefd1b72703164400676b826f75658ebd788be144d913bf`  
		Last Modified: Sat, 16 Oct 2021 04:49:29 GMT  
		Size: 4.4 KB (4374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f7f116049cdc4ecbde97a748d1ac965816d47409d395e268c5374a5d9a1aad`  
		Last Modified: Sat, 16 Oct 2021 04:49:31 GMT  
		Size: 3.6 MB (3578098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de9a8b4aa97172d2fd8c193aa25860ff531a070ec6cd9712b4f32e843f616a30`  
		Last Modified: Sat, 16 Oct 2021 04:49:42 GMT  
		Size: 44.1 MB (44107098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501c876323f9f789d38da919ca320db38ead022bceb0bd91b5ec7e9360512cb3`  
		Last Modified: Sat, 16 Oct 2021 04:49:29 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `groovy:jdk11` - linux; arm64 variant v8

```console
$ docker pull groovy@sha256:c4042fd49568da5b765c1eff00c4d36e3ed4df6c8d212b52b49e1d528ed97a6d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.6 MB (281573592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c5e415db040f8b2638fc1914197c8e981557eb078a0786a972ac17f0d459b6b`
-	Default Command: `["groovysh"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:25:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 16 Oct 2021 03:25:37 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Oct 2021 00:59:23 GMT
ENV JAVA_VERSION=jdk-11.0.13+8
# Wed, 27 Oct 2021 00:59:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='a77013bff10a5e9c59159231dd5c4bd071fc4c24beed42bd49b82803ba9506ef';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.13_8.tar.gz';          ;;        armhf|arm)          ESUM='61ee45c4ef21a85a116a87e1bca2e2a420b3af432be8d801bd52c660ffebaa9f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_arm_linux_hotspot_11.0.13_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='82f14cda71cff99c878bf8400598a87235adb6c81b0337f7077c27e5cac1190c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.13_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='9d280d86fdf6a7d9e5cbf54dc37f1d6d09dfe676ff5c684802fdfa3932eee63e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.13_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='3b1c0c34be4c894e64135a454f2d5aaa4bd10aea04ec2fa0c0efe6bb26528e30';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_hotspot_11.0.13_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 27 Oct 2021 00:59:32 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 27 Oct 2021 00:59:34 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 27 Oct 2021 00:59:34 GMT
CMD ["jshell"]
# Wed, 27 Oct 2021 01:55:00 GMT
CMD ["groovysh"]
# Wed, 27 Oct 2021 01:55:00 GMT
ENV GROOVY_HOME=/opt/groovy
# Wed, 27 Oct 2021 01:55:01 GMT
RUN set -o errexit -o nounset     && echo "Adding groovy user and group"     && groupadd --system --gid 1000 groovy     && useradd --system --gid groovy --uid 1000 --shell /bin/bash --create-home groovy     && mkdir --parents /home/groovy/.groovy/grapes     && chown --recursive groovy:groovy /home/groovy     && chmod --recursive 1777 /home/groovy         && echo "Symlinking root .groovy to groovy .groovy"     && ln --symbolic /home/groovy/.groovy /root/.groovy
# Wed, 27 Oct 2021 01:55:02 GMT
VOLUME [/home/groovy/.groovy/grapes]
# Wed, 27 Oct 2021 01:55:03 GMT
WORKDIR /home/groovy
# Wed, 27 Oct 2021 01:55:11 GMT
RUN apt-get update     && echo "Installing build dependencies"     && apt-get install --yes --no-install-recommends         dirmngr         fontconfig         gnupg         unzip         wget     && rm --recursive --force /var/lib/apt/lists/*
# Wed, 27 Oct 2021 01:55:11 GMT
ENV GROOVY_VERSION=3.0.9
# Wed, 27 Oct 2021 01:55:41 GMT
RUN set -o errexit -o nounset     && echo "Downloading Groovy"     && wget --no-verbose --output-document=groovy.zip "https://archive.apache.org/dist/groovy/${GROOVY_VERSION}/distribution/apache-groovy-binary-${GROOVY_VERSION}.zip"         && echo "Importing keys listed in http://www.apache.org/dist/groovy/KEYS from key server"     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --no-tty --keyserver keyserver.ubuntu.com --recv-keys         7FAA0F2206DE228F0DB01AD741321490758AAD6F         331224E1D7BE883D16E8A685825C06C827AF6B66         34441E504A937F43EB0DAEF96A65176A0FB1CD0B         9A810E3B766E089FFB27C70F11B595CEDC4AEBB5         81CABC23EECA0790E8989B361FF96E10F0E13706         && echo "Checking download signature"     && wget --no-verbose --output-document=groovy.zip.asc "https://archive.apache.org/dist/groovy/${GROOVY_VERSION}/distribution/apache-groovy-binary-${GROOVY_VERSION}.zip.asc"     && gpg --batch --no-tty --verify groovy.zip.asc groovy.zip     && rm --recursive --force "${GNUPGHOME}"     && rm groovy.zip.asc         && echo "Installing Groovy"     && unzip groovy.zip     && rm groovy.zip     && mv "groovy-${GROOVY_VERSION}" "${GROOVY_HOME}/"     && ln --symbolic "${GROOVY_HOME}/bin/grape" /usr/bin/grape     && ln --symbolic "${GROOVY_HOME}/bin/groovy" /usr/bin/groovy     && ln --symbolic "${GROOVY_HOME}/bin/groovyc" /usr/bin/groovyc     && ln --symbolic "${GROOVY_HOME}/bin/groovyConsole" /usr/bin/groovyConsole     && ln --symbolic "${GROOVY_HOME}/bin/groovydoc" /usr/bin/groovydoc     && ln --symbolic "${GROOVY_HOME}/bin/groovysh" /usr/bin/groovysh     && ln --symbolic "${GROOVY_HOME}/bin/java2groovy" /usr/bin/java2groovy         && echo "Editing startGroovy to include java.xml.bind module"     && sed --in-place 's|startGroovy ( ) {|startGroovy ( ) {\n    JAVA_OPTS="$JAVA_OPTS --add-modules=ALL-SYSTEM"|' "${GROOVY_HOME}/bin/startGroovy"
# Wed, 27 Oct 2021 01:55:42 GMT
USER groovy
# Wed, 27 Oct 2021 01:55:44 GMT
RUN set -o errexit -o nounset     && echo "Testing Groovy installation"     && groovy --version
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de699fc152b0c7a1bb0178ab0b7c6d0d2299c9f200d69a1e73d96ce334f2996d`  
		Last Modified: Sat, 16 Oct 2021 03:31:46 GMT  
		Size: 15.9 MB (15896303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ddd416e2999cff7c29865a2781196528d9a4ddedf4560e63c6ebc95d4d51e50`  
		Last Modified: Wed, 27 Oct 2021 01:02:24 GMT  
		Size: 190.5 MB (190512962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714ab4309f806f0e9c936d6e6608020dfc2faf8167cc933fe4157f8cbd3f6a6b`  
		Last Modified: Wed, 27 Oct 2021 01:02:05 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:737cc3dfaa9fe018d6901b46ec46316bfba5dbe254d95c12d57403d20f0bffc2`  
		Last Modified: Wed, 27 Oct 2021 01:57:34 GMT  
		Size: 4.3 KB (4345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e6f9f898a93d003f6d428310817381eade61f2d40ecc35410dc80fe85903147`  
		Last Modified: Wed, 27 Oct 2021 01:57:35 GMT  
		Size: 3.9 MB (3881747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607553d496fd81a8a8c2143f2a3a798832b6a6caa682c71a95e4acc9203cb909`  
		Last Modified: Wed, 27 Oct 2021 01:57:40 GMT  
		Size: 44.1 MB (44107068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd96c5bd1c502fef35fa4c591fe94d66e39ac3f1122af4c260c056d50729d5bf`  
		Last Modified: Wed, 27 Oct 2021 01:57:34 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `groovy:jdk11` - linux; ppc64le

```console
$ docker pull groovy@sha256:15eece6bfd89ebe479c3d0d71e887d6c2c6752a14b11bbff29d123e2c002368b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.4 MB (275363932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58752970745af9858b687708921f5e19ee0650245c829328ae1f25245119f7aa`
-	Default Command: `["groovysh"]`

```dockerfile
# Sat, 16 Oct 2021 00:36:38 GMT
ADD file:9246bf887411af1b286de95d779c11581dcef3c0d5a29e434162f0c085a7ce85 in / 
# Sat, 16 Oct 2021 00:36:44 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 00:54:47 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 16 Oct 2021 00:55:56 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 00:57:23 GMT
ENV JAVA_VERSION=jdk-11.0.12+7
# Sat, 16 Oct 2021 00:57:40 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='105bdc12fcd54c551e8e8ac96bc82412467244c32063689c41cee29ceb7452a2';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.12_7.tar.gz';          ;;        armhf|arm)          ESUM='85929246a9d60ed90e2385ea3f4857798c77019c5100f00189c1dd0a093abea7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_arm_linux_hotspot_11.0.12_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='234a9bafe029ea6cab5d46f9617b5d016a29faa187a42081d0e066f23647b7e5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.12_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='99c1c61e9d67b01a649687189e5a00f89a2371dc1bfed06bb078d127edfa7995';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.12_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='8770f600fc3b89bf331213c7aa21f8eedd9ca5d96036d1cd48cb2748a3dbefd2';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_x64_linux_hotspot_11.0.12_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 16 Oct 2021 00:57:44 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 16 Oct 2021 00:57:51 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Sat, 16 Oct 2021 00:57:53 GMT
CMD ["jshell"]
# Sat, 16 Oct 2021 02:42:52 GMT
CMD ["groovysh"]
# Sat, 16 Oct 2021 02:42:55 GMT
ENV GROOVY_HOME=/opt/groovy
# Sat, 16 Oct 2021 02:43:09 GMT
RUN set -o errexit -o nounset     && echo "Adding groovy user and group"     && groupadd --system --gid 1000 groovy     && useradd --system --gid groovy --uid 1000 --shell /bin/bash --create-home groovy     && mkdir --parents /home/groovy/.groovy/grapes     && chown --recursive groovy:groovy /home/groovy     && chmod --recursive 1777 /home/groovy         && echo "Symlinking root .groovy to groovy .groovy"     && ln --symbolic /home/groovy/.groovy /root/.groovy
# Sat, 16 Oct 2021 02:43:14 GMT
VOLUME [/home/groovy/.groovy/grapes]
# Sat, 16 Oct 2021 02:43:22 GMT
WORKDIR /home/groovy
# Sat, 16 Oct 2021 02:44:02 GMT
RUN apt-get update     && echo "Installing build dependencies"     && apt-get install --yes --no-install-recommends         dirmngr         fontconfig         gnupg         unzip         wget     && rm --recursive --force /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:44:17 GMT
ENV GROOVY_VERSION=3.0.9
# Sat, 16 Oct 2021 02:44:43 GMT
RUN set -o errexit -o nounset     && echo "Downloading Groovy"     && wget --no-verbose --output-document=groovy.zip "https://archive.apache.org/dist/groovy/${GROOVY_VERSION}/distribution/apache-groovy-binary-${GROOVY_VERSION}.zip"         && echo "Importing keys listed in http://www.apache.org/dist/groovy/KEYS from key server"     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --no-tty --keyserver keyserver.ubuntu.com --recv-keys         7FAA0F2206DE228F0DB01AD741321490758AAD6F         331224E1D7BE883D16E8A685825C06C827AF6B66         34441E504A937F43EB0DAEF96A65176A0FB1CD0B         9A810E3B766E089FFB27C70F11B595CEDC4AEBB5         81CABC23EECA0790E8989B361FF96E10F0E13706         && echo "Checking download signature"     && wget --no-verbose --output-document=groovy.zip.asc "https://archive.apache.org/dist/groovy/${GROOVY_VERSION}/distribution/apache-groovy-binary-${GROOVY_VERSION}.zip.asc"     && gpg --batch --no-tty --verify groovy.zip.asc groovy.zip     && rm --recursive --force "${GNUPGHOME}"     && rm groovy.zip.asc         && echo "Installing Groovy"     && unzip groovy.zip     && rm groovy.zip     && mv "groovy-${GROOVY_VERSION}" "${GROOVY_HOME}/"     && ln --symbolic "${GROOVY_HOME}/bin/grape" /usr/bin/grape     && ln --symbolic "${GROOVY_HOME}/bin/groovy" /usr/bin/groovy     && ln --symbolic "${GROOVY_HOME}/bin/groovyc" /usr/bin/groovyc     && ln --symbolic "${GROOVY_HOME}/bin/groovyConsole" /usr/bin/groovyConsole     && ln --symbolic "${GROOVY_HOME}/bin/groovydoc" /usr/bin/groovydoc     && ln --symbolic "${GROOVY_HOME}/bin/groovysh" /usr/bin/groovysh     && ln --symbolic "${GROOVY_HOME}/bin/java2groovy" /usr/bin/java2groovy         && echo "Editing startGroovy to include java.xml.bind module"     && sed --in-place 's|startGroovy ( ) {|startGroovy ( ) {\n    JAVA_OPTS="$JAVA_OPTS --add-modules=ALL-SYSTEM"|' "${GROOVY_HOME}/bin/startGroovy"
# Sat, 16 Oct 2021 02:44:48 GMT
USER groovy
# Sat, 16 Oct 2021 02:45:12 GMT
RUN set -o errexit -o nounset     && echo "Testing Groovy installation"     && groovy --version
```

-	Layers:
	-	`sha256:77ba7971d651af68e20e7cbb6603a3f7acd8ef2893066767a93db104723556f2`  
		Last Modified: Sat, 16 Oct 2021 00:38:38 GMT  
		Size: 33.3 MB (33287238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c930749dacf55e37561edab7967f5a2f51660034fee0da501c2d71cb783301`  
		Last Modified: Sat, 16 Oct 2021 01:03:26 GMT  
		Size: 17.2 MB (17210510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaca7a459d94934b461957e71559ffcb47511f54848b2fa0a18b62c831c007ad`  
		Last Modified: Sat, 16 Oct 2021 01:04:27 GMT  
		Size: 175.7 MB (175686484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd31127949029231226b0a1198fbf0e913dd0e80d2715727fc19386fd48b6b34`  
		Last Modified: Sat, 16 Oct 2021 01:04:08 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc2dae468ff5edc6b29798b93655d3afd8799ee062f1962adb60f40f38cf76a6`  
		Last Modified: Sat, 16 Oct 2021 02:53:39 GMT  
		Size: 4.4 KB (4401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e15d625e337b4db3934ab7c1b0c5085933f7eb74b777776124307654ba1a6a`  
		Last Modified: Sat, 16 Oct 2021 02:53:40 GMT  
		Size: 5.1 MB (5067845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f718eb2077b33573b554c83addc1f181cae78515a13ab9067365183be2e6cd4`  
		Last Modified: Sat, 16 Oct 2021 02:53:44 GMT  
		Size: 44.1 MB (44107118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4889738f9b0ba763fafc7ad4ececa9124c6a2dbad9c2ea09e9fb07a2f352cf05`  
		Last Modified: Sat, 16 Oct 2021 02:53:39 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `groovy:jdk11` - linux; s390x

```console
$ docker pull groovy@sha256:c240aae52e5395de929c83d7ca6f7de5214b8a4a7ac6edfc6f4fba6bf9898a8a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.3 MB (259252388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3598f4d4cbbd48cf4670c0d7b0e10b81fb27767e497565b35c4ef4d64e7c5c8c`
-	Default Command: `["groovysh"]`

```dockerfile
# Sat, 16 Oct 2021 00:41:46 GMT
ADD file:cf3b6f9c395392eaf2c629969f59c48cde60ae1c74c3dbb13886481999a7a4d5 in / 
# Sat, 16 Oct 2021 00:41:48 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 00:58:42 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 16 Oct 2021 00:58:53 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Oct 2021 00:29:53 GMT
ENV JAVA_VERSION=jdk-11.0.13+8
# Wed, 27 Oct 2021 00:30:08 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='a77013bff10a5e9c59159231dd5c4bd071fc4c24beed42bd49b82803ba9506ef';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.13_8.tar.gz';          ;;        armhf|arm)          ESUM='61ee45c4ef21a85a116a87e1bca2e2a420b3af432be8d801bd52c660ffebaa9f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_arm_linux_hotspot_11.0.13_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='82f14cda71cff99c878bf8400598a87235adb6c81b0337f7077c27e5cac1190c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.13_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='9d280d86fdf6a7d9e5cbf54dc37f1d6d09dfe676ff5c684802fdfa3932eee63e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.13_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='3b1c0c34be4c894e64135a454f2d5aaa4bd10aea04ec2fa0c0efe6bb26528e30';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_hotspot_11.0.13_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 27 Oct 2021 00:30:11 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 27 Oct 2021 00:30:12 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 27 Oct 2021 00:30:12 GMT
CMD ["jshell"]
# Wed, 27 Oct 2021 01:13:59 GMT
CMD ["groovysh"]
# Wed, 27 Oct 2021 01:13:59 GMT
ENV GROOVY_HOME=/opt/groovy
# Wed, 27 Oct 2021 01:14:00 GMT
RUN set -o errexit -o nounset     && echo "Adding groovy user and group"     && groupadd --system --gid 1000 groovy     && useradd --system --gid groovy --uid 1000 --shell /bin/bash --create-home groovy     && mkdir --parents /home/groovy/.groovy/grapes     && chown --recursive groovy:groovy /home/groovy     && chmod --recursive 1777 /home/groovy         && echo "Symlinking root .groovy to groovy .groovy"     && ln --symbolic /home/groovy/.groovy /root/.groovy
# Wed, 27 Oct 2021 01:14:00 GMT
VOLUME [/home/groovy/.groovy/grapes]
# Wed, 27 Oct 2021 01:14:00 GMT
WORKDIR /home/groovy
# Wed, 27 Oct 2021 01:14:04 GMT
RUN apt-get update     && echo "Installing build dependencies"     && apt-get install --yes --no-install-recommends         dirmngr         fontconfig         gnupg         unzip         wget     && rm --recursive --force /var/lib/apt/lists/*
# Wed, 27 Oct 2021 01:14:04 GMT
ENV GROOVY_VERSION=3.0.9
# Wed, 27 Oct 2021 01:14:20 GMT
RUN set -o errexit -o nounset     && echo "Downloading Groovy"     && wget --no-verbose --output-document=groovy.zip "https://archive.apache.org/dist/groovy/${GROOVY_VERSION}/distribution/apache-groovy-binary-${GROOVY_VERSION}.zip"         && echo "Importing keys listed in http://www.apache.org/dist/groovy/KEYS from key server"     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --no-tty --keyserver keyserver.ubuntu.com --recv-keys         7FAA0F2206DE228F0DB01AD741321490758AAD6F         331224E1D7BE883D16E8A685825C06C827AF6B66         34441E504A937F43EB0DAEF96A65176A0FB1CD0B         9A810E3B766E089FFB27C70F11B595CEDC4AEBB5         81CABC23EECA0790E8989B361FF96E10F0E13706         && echo "Checking download signature"     && wget --no-verbose --output-document=groovy.zip.asc "https://archive.apache.org/dist/groovy/${GROOVY_VERSION}/distribution/apache-groovy-binary-${GROOVY_VERSION}.zip.asc"     && gpg --batch --no-tty --verify groovy.zip.asc groovy.zip     && rm --recursive --force "${GNUPGHOME}"     && rm groovy.zip.asc         && echo "Installing Groovy"     && unzip groovy.zip     && rm groovy.zip     && mv "groovy-${GROOVY_VERSION}" "${GROOVY_HOME}/"     && ln --symbolic "${GROOVY_HOME}/bin/grape" /usr/bin/grape     && ln --symbolic "${GROOVY_HOME}/bin/groovy" /usr/bin/groovy     && ln --symbolic "${GROOVY_HOME}/bin/groovyc" /usr/bin/groovyc     && ln --symbolic "${GROOVY_HOME}/bin/groovyConsole" /usr/bin/groovyConsole     && ln --symbolic "${GROOVY_HOME}/bin/groovydoc" /usr/bin/groovydoc     && ln --symbolic "${GROOVY_HOME}/bin/groovysh" /usr/bin/groovysh     && ln --symbolic "${GROOVY_HOME}/bin/java2groovy" /usr/bin/java2groovy         && echo "Editing startGroovy to include java.xml.bind module"     && sed --in-place 's|startGroovy ( ) {|startGroovy ( ) {\n    JAVA_OPTS="$JAVA_OPTS --add-modules=ALL-SYSTEM"|' "${GROOVY_HOME}/bin/startGroovy"
# Wed, 27 Oct 2021 01:14:21 GMT
USER groovy
# Wed, 27 Oct 2021 01:14:22 GMT
RUN set -o errexit -o nounset     && echo "Testing Groovy installation"     && groovy --version
```

-	Layers:
	-	`sha256:1f0267805ccac7499fadaabf65e52d4564add2bc20ed25bcf77df24d8debb103`  
		Last Modified: Sat, 16 Oct 2021 00:42:57 GMT  
		Size: 27.1 MB (27120856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276dbe4459a060d2c186c43e5e92d98fa6f181617c55cce69da393b9d5dd6200`  
		Last Modified: Sat, 16 Oct 2021 01:01:03 GMT  
		Size: 15.7 MB (15742080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f997daed2ec37c813b127371f0d935eede6a53b2e0a56882d215ee24d19e5bb`  
		Last Modified: Wed, 27 Oct 2021 00:31:33 GMT  
		Size: 168.2 MB (168218183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843ae0a80f2edb722ece7d0c771313f6eea63d30403b826e0fd6ddc01c530fdc`  
		Last Modified: Wed, 27 Oct 2021 00:31:23 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6deb771d3040970acd5b4d1d29347c0e1ec552c8f47b8e47595cd613d99d6079`  
		Last Modified: Wed, 27 Oct 2021 01:15:48 GMT  
		Size: 4.4 KB (4397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c88903c12ba2e827103a64f547933e51dc523c01241725ff3caf4e1e6883b306`  
		Last Modified: Wed, 27 Oct 2021 01:15:48 GMT  
		Size: 4.1 MB (4059426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5327a0bdad07aa9de51f1bcc7a912ac73da548f1a1a9e01b8f3c08cd66bfe1c5`  
		Last Modified: Wed, 27 Oct 2021 01:15:51 GMT  
		Size: 44.1 MB (44107115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4062a6d167649292bc8876215874ca476b9aad489b3f6b3d71f9b1cd4848cd76`  
		Last Modified: Wed, 27 Oct 2021 01:15:48 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
