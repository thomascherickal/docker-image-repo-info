## `maven:3-eclipse-temurin-11`

```console
$ docker pull maven@sha256:5b7553d0ee0732dd9f0190cb9fc79f09045a26c560072a2712fc9b211403b6f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `maven:3-eclipse-temurin-11` - linux; amd64

```console
$ docker pull maven@sha256:0cf0b32f78eab3adc7885b081f28ad06c324341c412e62454647549770648a35
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **287.5 MB (287473349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7565afcc92d54bb661743a819898ab411f6c3411d0963ea7cbde20f4f3fd7e84`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:44:06 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 29 Nov 2021 20:21:51 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 29 Nov 2021 20:22:21 GMT
ENV JAVA_VERSION=jdk-11.0.13+8
# Mon, 29 Nov 2021 20:22:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='a77013bff10a5e9c59159231dd5c4bd071fc4c24beed42bd49b82803ba9506ef';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.13_8.tar.gz';          ;;        armhf|arm)          ESUM='61ee45c4ef21a85a116a87e1bca2e2a420b3af432be8d801bd52c660ffebaa9f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_arm_linux_hotspot_11.0.13_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='82f14cda71cff99c878bf8400598a87235adb6c81b0337f7077c27e5cac1190c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.13_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='9d280d86fdf6a7d9e5cbf54dc37f1d6d09dfe676ff5c684802fdfa3932eee63e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.13_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='3b1c0c34be4c894e64135a454f2d5aaa4bd10aea04ec2fa0c0efe6bb26528e30';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_hotspot_11.0.13_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 29 Nov 2021 20:22:33 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 29 Nov 2021 20:22:34 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Mon, 29 Nov 2021 20:22:34 GMT
CMD ["jshell"]
# Tue, 30 Nov 2021 01:05:41 GMT
ARG MAVEN_VERSION=3.8.4
# Tue, 30 Nov 2021 01:05:42 GMT
ARG USER_HOME_DIR=/root
# Tue, 30 Nov 2021 01:05:42 GMT
ARG SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8
# Tue, 30 Nov 2021 01:05:42 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries
# Tue, 30 Nov 2021 01:05:56 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Tue, 30 Nov 2021 01:05:59 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 30 Nov 2021 01:05:59 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 30 Nov 2021 01:05:59 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 30 Nov 2021 01:05:59 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 30 Nov 2021 01:06:00 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Tue, 30 Nov 2021 01:06:00 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 30 Nov 2021 01:06:00 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c122ee837fa892e5fdd4f7c857600f80a7b8fa855d2475bb325372d55eaff04`  
		Last Modified: Mon, 29 Nov 2021 20:25:31 GMT  
		Size: 24.8 MB (24814948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df03d17a1d16d4f310f47ff0900289f9beec130c2f7a84d52ba93541c6f8f048`  
		Last Modified: Mon, 29 Nov 2021 20:26:21 GMT  
		Size: 193.8 MB (193801823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d1597bd18adb0195f9d09ada1bc1261137834d5cb3b4ad5ee2cbc4e010261a`  
		Last Modified: Mon, 29 Nov 2021 20:26:07 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d207bc992c18184e4e2365219f28bc895af88ae1866ab7aa49878ef93488fc5`  
		Last Modified: Tue, 30 Nov 2021 01:10:00 GMT  
		Size: 31.2 MB (31178297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd4ff04fbf36a689372fc149f9f77439f65a12e1704bc457a1503e1878a00f5`  
		Last Modified: Tue, 30 Nov 2021 01:09:56 GMT  
		Size: 9.1 MB (9109806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2cc0ee97b7e8f1c360e04b2d699ab59783f99ff049384b8d251ff66d8a38a0`  
		Last Modified: Tue, 30 Nov 2021 01:09:55 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9dcee43da3acfc595f5cea373c721faa23aa5e18c48def01d85168cf814481`  
		Last Modified: Tue, 30 Nov 2021 01:09:55 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-eclipse-temurin-11` - linux; arm variant v7

```console
$ docker pull maven@sha256:b2654b9f001785cccfcc98663e6669b069a77628deb17c78cb417e388d35c2f2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.2 MB (265248446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee354274ef2b6c7bb3f72bb4b72e0c3bfee65d212e10f669d013a6a0f8957321`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Sat, 16 Oct 2021 01:12:00 GMT
ADD file:625e3906181f4bd86e59a0e9748f67fcb1391a2e65e36c729e71353381a49757 in / 
# Sat, 16 Oct 2021 01:12:00 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:38:37 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 29 Nov 2021 19:58:37 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 29 Nov 2021 19:59:57 GMT
ENV JAVA_VERSION=jdk-11.0.13+8
# Mon, 29 Nov 2021 20:00:19 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='a77013bff10a5e9c59159231dd5c4bd071fc4c24beed42bd49b82803ba9506ef';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.13_8.tar.gz';          ;;        armhf|arm)          ESUM='61ee45c4ef21a85a116a87e1bca2e2a420b3af432be8d801bd52c660ffebaa9f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_arm_linux_hotspot_11.0.13_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='82f14cda71cff99c878bf8400598a87235adb6c81b0337f7077c27e5cac1190c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.13_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='9d280d86fdf6a7d9e5cbf54dc37f1d6d09dfe676ff5c684802fdfa3932eee63e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.13_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='3b1c0c34be4c894e64135a454f2d5aaa4bd10aea04ec2fa0c0efe6bb26528e30';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_hotspot_11.0.13_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 29 Nov 2021 20:00:21 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 29 Nov 2021 20:00:23 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Mon, 29 Nov 2021 20:00:24 GMT
CMD ["jshell"]
# Mon, 29 Nov 2021 21:38:58 GMT
ARG MAVEN_VERSION=3.8.4
# Mon, 29 Nov 2021 21:38:58 GMT
ARG USER_HOME_DIR=/root
# Mon, 29 Nov 2021 21:38:58 GMT
ARG SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8
# Mon, 29 Nov 2021 21:38:59 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries
# Mon, 29 Nov 2021 21:39:21 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Mon, 29 Nov 2021 21:39:31 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Mon, 29 Nov 2021 21:39:31 GMT
ENV MAVEN_HOME=/usr/share/maven
# Mon, 29 Nov 2021 21:39:32 GMT
ENV MAVEN_CONFIG=/root/.m2
# Mon, 29 Nov 2021 21:39:32 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Mon, 29 Nov 2021 21:39:33 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Mon, 29 Nov 2021 21:39:33 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Mon, 29 Nov 2021 21:39:34 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:8795d4da4abd6abcafe7285749aa85d3a164999e84720a3845f764e56e306771`  
		Last Modified: Sat, 16 Oct 2021 01:15:01 GMT  
		Size: 24.1 MB (24064451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f49a73fe087725ab5b9956d86afb7a1ca7735fe7eb993e92d61d1d780acba64`  
		Last Modified: Mon, 29 Nov 2021 20:05:51 GMT  
		Size: 23.1 MB (23068723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3fec13e837b2fa6599f353cc5f1a323c81b59bf77d1a637cb6287cf91ca3ac5`  
		Last Modified: Mon, 29 Nov 2021 20:08:16 GMT  
		Size: 181.7 MB (181700342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac5843df8c306ffa38fabf55990521607c9c0b7e00f014639bf00357222b9936`  
		Last Modified: Mon, 29 Nov 2021 20:07:07 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541b7bdaaa27191eacac43ae68ab5a6778a8082012fa33899331e470aaf23143`  
		Last Modified: Mon, 29 Nov 2021 21:43:47 GMT  
		Size: 27.3 MB (27303749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1abb1a6583544ab48d377613e18fbe1d7120fe5c8c740fb476edbc23c702071`  
		Last Modified: Mon, 29 Nov 2021 21:43:33 GMT  
		Size: 9.1 MB (9109805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a5d4d4f39a964d1fb7c5fffa18329e077fefdbd2ca395f1abacb03c5bc6331`  
		Last Modified: Mon, 29 Nov 2021 21:43:30 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f633ed5c44cb697c44d7cfa9d57eca40be6ebdfa765485984ecbe1879d1bdd0`  
		Last Modified: Mon, 29 Nov 2021 21:43:30 GMT  
		Size: 364.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-eclipse-temurin-11` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:37ad183a9f4dff100570b429db2387630131140cf8ce41e701eb424a520f0553
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.5 MB (282530865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e138c3151464c9a7cb5cf911e3afda51fb0e7c657fd4a26214fa37337cdce66f`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:45 GMT
ADD file:521a8ada4ac06e6f7720904486d481d216a8c3e08c0c7db1376c39a33e709668 in / 
# Fri, 07 Jan 2022 01:53:45 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:32:58 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Jan 2022 02:33:21 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 02:34:02 GMT
ENV JAVA_VERSION=jdk-11.0.13+8
# Fri, 07 Jan 2022 02:34:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='a77013bff10a5e9c59159231dd5c4bd071fc4c24beed42bd49b82803ba9506ef';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.13_8.tar.gz';          ;;        armhf|arm)          ESUM='61ee45c4ef21a85a116a87e1bca2e2a420b3af432be8d801bd52c660ffebaa9f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_arm_linux_hotspot_11.0.13_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='82f14cda71cff99c878bf8400598a87235adb6c81b0337f7077c27e5cac1190c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.13_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='9d280d86fdf6a7d9e5cbf54dc37f1d6d09dfe676ff5c684802fdfa3932eee63e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.13_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='3b1c0c34be4c894e64135a454f2d5aaa4bd10aea04ec2fa0c0efe6bb26528e30';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_hotspot_11.0.13_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 07 Jan 2022 02:34:17 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Jan 2022 02:34:19 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 07 Jan 2022 02:34:20 GMT
CMD ["jshell"]
# Fri, 07 Jan 2022 05:02:28 GMT
ARG MAVEN_VERSION=3.8.4
# Fri, 07 Jan 2022 05:02:28 GMT
ARG USER_HOME_DIR=/root
# Fri, 07 Jan 2022 05:02:29 GMT
ARG SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8
# Fri, 07 Jan 2022 05:02:30 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries
# Fri, 07 Jan 2022 05:02:43 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 05:03:02 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 07 Jan 2022 05:03:03 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 07 Jan 2022 05:03:04 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 07 Jan 2022 05:03:06 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 07 Jan 2022 05:03:07 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 07 Jan 2022 05:03:07 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 07 Jan 2022 05:03:08 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:5f3d23ccb99f6c9462a15efcf35aef0863858073a06d56df671d0e791b26222a`  
		Last Modified: Fri, 07 Jan 2022 01:55:32 GMT  
		Size: 27.2 MB (27171074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cabab443fc2997710c1da51cfcf08e2f3d95b70585ea241c5ce42e6291364ec`  
		Last Modified: Fri, 07 Jan 2022 02:37:58 GMT  
		Size: 24.8 MB (24763102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8331ea3f2959c031fc1659290ea740ca490a2cbda82db1fb8ac995b956a75954`  
		Last Modified: Fri, 07 Jan 2022 02:38:55 GMT  
		Size: 190.5 MB (190512935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a7f2bd205c7f3ae6376e9eaf809fc3d4135e5c6897398f92e2dc27d2e725378`  
		Last Modified: Fri, 07 Jan 2022 02:38:38 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0bf5ed83483f3ae5209bbb7eac42899caeefbb2af41e3a464a1f8e7c0dc8453`  
		Last Modified: Fri, 07 Jan 2022 05:07:55 GMT  
		Size: 31.0 MB (30972631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39dd8bddc9cefb8f9f854a921bd45f0728ef1c5a2de991d8046a7804978334f9`  
		Last Modified: Fri, 07 Jan 2022 05:07:51 GMT  
		Size: 9.1 MB (9109779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a818de0b2793b12a0182a58045242edcbca09d87394d71e7b06eb0c7c57b00`  
		Last Modified: Fri, 07 Jan 2022 05:07:50 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7289e84924a6343c3d246cd09468bf15a13dcac4e014c00bee56921a1748851a`  
		Last Modified: Fri, 07 Jan 2022 05:07:49 GMT  
		Size: 364.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-eclipse-temurin-11` - linux; ppc64le

```console
$ docker pull maven@sha256:c71e99f60c0f6913a0f2480a6f7dcb335669fdf66a617175d2e59e5ab7479672
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.1 MB (283103926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ed7d3b6f92fc0db06b291ba21f4cc722f2d692606dc0b96a1953b4c414850d5`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 07 Jan 2022 02:20:15 GMT
ADD file:014236839eaee978894ae0bd6aecc246177a0a2c11af73f86d9cfafe5478ce18 in / 
# Fri, 07 Jan 2022 02:20:19 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:15:29 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Jan 2022 03:16:40 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:17:55 GMT
ENV JAVA_VERSION=jdk-11.0.13+8
# Fri, 07 Jan 2022 03:18:13 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='a77013bff10a5e9c59159231dd5c4bd071fc4c24beed42bd49b82803ba9506ef';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.13_8.tar.gz';          ;;        armhf|arm)          ESUM='61ee45c4ef21a85a116a87e1bca2e2a420b3af432be8d801bd52c660ffebaa9f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_arm_linux_hotspot_11.0.13_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='82f14cda71cff99c878bf8400598a87235adb6c81b0337f7077c27e5cac1190c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.13_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='9d280d86fdf6a7d9e5cbf54dc37f1d6d09dfe676ff5c684802fdfa3932eee63e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.13_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='3b1c0c34be4c894e64135a454f2d5aaa4bd10aea04ec2fa0c0efe6bb26528e30';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_hotspot_11.0.13_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 07 Jan 2022 03:18:17 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Jan 2022 03:18:21 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 07 Jan 2022 03:18:22 GMT
CMD ["jshell"]
# Fri, 07 Jan 2022 05:54:11 GMT
ARG MAVEN_VERSION=3.8.4
# Fri, 07 Jan 2022 05:54:13 GMT
ARG USER_HOME_DIR=/root
# Fri, 07 Jan 2022 05:54:14 GMT
ARG SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8
# Fri, 07 Jan 2022 05:54:15 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries
# Fri, 07 Jan 2022 05:54:53 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 05:55:01 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 07 Jan 2022 05:55:02 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 07 Jan 2022 05:55:03 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 07 Jan 2022 05:55:04 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 07 Jan 2022 05:55:05 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 07 Jan 2022 05:55:06 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 07 Jan 2022 05:55:08 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:e6e6dea5a8cc4bdc9e5e51e2bfa948159b69d5fbc2dca99bc41776fb04dab967`  
		Last Modified: Fri, 07 Jan 2022 02:22:43 GMT  
		Size: 33.3 MB (33286892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e359e3ea7dc58d4487bc585c0d8fcd27011690cd1135560fbab69fb8eb51ca7`  
		Last Modified: Fri, 07 Jan 2022 03:24:37 GMT  
		Size: 26.6 MB (26642914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4de7ca343f34f14e184a11d2f3f4f9a5764df841e5869e368b6123cf5b12dff5`  
		Last Modified: Fri, 07 Jan 2022 03:25:45 GMT  
		Size: 175.7 MB (175680303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:865657c9cf92624c23fa769d7ecfeef1e589872a914cc683bfa00cb3365abe75`  
		Last Modified: Fri, 07 Jan 2022 03:25:26 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f127c07b2a7c273650b872ab4900061ff5129ca43a6a712b244e5c9cba9bbe89`  
		Last Modified: Fri, 07 Jan 2022 06:01:48 GMT  
		Size: 38.4 MB (38382650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bfa2ff80cfeb5502587a0a2cf4dc5763df0e1935438731963f7b8f5fb7c6f4d`  
		Last Modified: Fri, 07 Jan 2022 06:01:43 GMT  
		Size: 9.1 MB (9109798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f5ebd119a6d96d763e90edbe520e6fa7069eb104732200f2c38479660f5066`  
		Last Modified: Fri, 07 Jan 2022 06:01:41 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8ce495a30338b72e401d19f4c64ae17d5b5c01132cbaad18aea211751745fd`  
		Last Modified: Fri, 07 Jan 2022 06:01:41 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-eclipse-temurin-11` - linux; s390x

```console
$ docker pull maven@sha256:3a99e020bec60cd5701a3d683a00c083b177fcd74e59e445523b127afb75bb1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.6 MB (259592228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2173e661e5e9308247bf764935dc3f3049d565ad0e1f8a7be2c8ec9b6d4aa975`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 07 Jan 2022 01:42:20 GMT
ADD file:b6119f4fcd6a113749f515278b315ffd96aecce7006f086acb060f981e5c59db in / 
# Fri, 07 Jan 2022 01:42:22 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 02:15:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 07 Jan 2022 02:15:38 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 02:15:39 GMT
ENV JAVA_VERSION=jdk-11.0.13+8
# Fri, 07 Jan 2022 02:15:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='a77013bff10a5e9c59159231dd5c4bd071fc4c24beed42bd49b82803ba9506ef';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.13_8.tar.gz';          ;;        armhf|arm)          ESUM='61ee45c4ef21a85a116a87e1bca2e2a420b3af432be8d801bd52c660ffebaa9f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_arm_linux_hotspot_11.0.13_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='82f14cda71cff99c878bf8400598a87235adb6c81b0337f7077c27e5cac1190c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.13_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='9d280d86fdf6a7d9e5cbf54dc37f1d6d09dfe676ff5c684802fdfa3932eee63e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.13_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='3b1c0c34be4c894e64135a454f2d5aaa4bd10aea04ec2fa0c0efe6bb26528e30';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_hotspot_11.0.13_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 07 Jan 2022 02:15:50 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Jan 2022 02:15:51 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 07 Jan 2022 02:15:51 GMT
CMD ["jshell"]
# Fri, 07 Jan 2022 03:32:00 GMT
ARG MAVEN_VERSION=3.8.4
# Fri, 07 Jan 2022 03:32:00 GMT
ARG USER_HOME_DIR=/root
# Fri, 07 Jan 2022 03:32:00 GMT
ARG SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8
# Fri, 07 Jan 2022 03:32:01 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries
# Fri, 07 Jan 2022 03:32:10 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN apt-get update     && apt-get install -y git     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 03:32:14 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 07 Jan 2022 03:32:14 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 07 Jan 2022 03:32:15 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 07 Jan 2022 03:32:15 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 07 Jan 2022 03:32:15 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 07 Jan 2022 03:32:15 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 07 Jan 2022 03:32:15 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:6d200361446626b53394c2a1a520a74a1221795562eac9b318c58e0abe147e23`  
		Last Modified: Fri, 07 Jan 2022 01:44:09 GMT  
		Size: 27.1 MB (27120999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f72e3f9d5b463f73df3140cbe7e59d12fed8b7531031e702de787ea477fb99`  
		Last Modified: Fri, 07 Jan 2022 02:18:29 GMT  
		Size: 24.4 MB (24446369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2768fdacf2ae67d3aae426f1151237e3e9575f158964318b26d2fcecedc3b272`  
		Last Modified: Fri, 07 Jan 2022 02:18:36 GMT  
		Size: 168.2 MB (168218184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab02c8bae3bf1893998a1b33bbe91fe81adb4f32d029ac881c36f7f45bc3942a`  
		Last Modified: Fri, 07 Jan 2022 02:18:25 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf96d2863900a6ee54afd3660c7e81ad7fa98314376fd3c09a984061e86c1b92`  
		Last Modified: Fri, 07 Jan 2022 03:34:18 GMT  
		Size: 30.7 MB (30695509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb56a1dafbdc7ee36f1273914fcb0b20016f2ede461666654e59130ccffe615`  
		Last Modified: Fri, 07 Jan 2022 03:34:14 GMT  
		Size: 9.1 MB (9109800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d9637ac0a595d1e4b0d2061df5ffe4a006600a48d2b39601a2b8014c27d25c`  
		Last Modified: Fri, 07 Jan 2022 03:34:14 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aa90418b00c8e784ebb0417ecb0ff63691f7c108b7bc926d66746988096298c`  
		Last Modified: Fri, 07 Jan 2022 03:34:14 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
