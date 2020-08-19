## `adoptopenjdk:11-jdk-openj9-bionic`

```console
$ docker pull adoptopenjdk@sha256:54a012415e54eec9bd5b4ccd146fc1a2784f98bc45c005dd502a22306d0026d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `adoptopenjdk:11-jdk-openj9-bionic` - linux; amd64

```console
$ docker pull adoptopenjdk@sha256:d28573e37fb123df982decb7b1c023f14e569b16e1ed36ecf5bd428fdc5ee530
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.1 MB (237058899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10e192e3289dfadf7edb6bdf56e91031e5a7dd2e6f3d2bc9e0355296453bacbc`
-	Default Command: `["jshell"]`

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
# Wed, 19 Aug 2020 22:00:58 GMT
ENV JAVA_VERSION=jdk-11.0.8+10_openj9-0.21.0
# Wed, 19 Aug 2020 22:01:08 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4bad13c0d9c2fbb1954fcddae9ccc5a32c609f2b48bf43ecaa5f39915390604';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.8%2B10_openj9-0.21.0/OpenJDK11U-jdk_aarch64_linux_openj9_11.0.8_10_openj9-0.21.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='5bcaa2075ce5bf634b542c04ea79b9ca505407b6f94d2d8350c712da387120d9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.8%2B10_openj9-0.21.0/OpenJDK11U-jdk_ppc64le_linux_openj9_11.0.8_10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='5e89692057fb8dfcb8e215fd3917b721fdb721c1eeea2b14948f4782413846bb';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.8%2B10_openj9-0.21.0/OpenJDK11U-jdk_s390x_linux_openj9_11.0.8_10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9ab79436180d41809f4fca8afe43e778ae2d82c7b50f3653c62d7a2728150836';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.8%2B10_openj9-0.21.0/OpenJDK11U-jdk_x64_linux_openj9_11.0.8_10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 22:01:08 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 22:01:08 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Wed, 19 Aug 2020 22:01:09 GMT
CMD ["jshell"]
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
	-	`sha256:55528b67d471cd4f39151297a2a8e8e687c540f9ea124b11456b48cc0d57e4ba`  
		Last Modified: Wed, 19 Aug 2020 22:06:11 GMT  
		Size: 196.4 MB (196447236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:11-jdk-openj9-bionic` - linux; ppc64le

```console
$ docker pull adoptopenjdk@sha256:58d321c5f4339ee39c9d88329a22c4a85d698006a9e79ed144e526534a9e5c80
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.3 MB (242254179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05e2da7fe46faa97442752121ab6a0b4209f24d5d9080660f5c205196ff56555`
-	Default Command: `["jshell"]`

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
# Wed, 19 Aug 2020 22:33:55 GMT
ENV JAVA_VERSION=jdk-11.0.8+10_openj9-0.21.0
# Wed, 19 Aug 2020 22:34:26 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4bad13c0d9c2fbb1954fcddae9ccc5a32c609f2b48bf43ecaa5f39915390604';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.8%2B10_openj9-0.21.0/OpenJDK11U-jdk_aarch64_linux_openj9_11.0.8_10_openj9-0.21.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='5bcaa2075ce5bf634b542c04ea79b9ca505407b6f94d2d8350c712da387120d9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.8%2B10_openj9-0.21.0/OpenJDK11U-jdk_ppc64le_linux_openj9_11.0.8_10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='5e89692057fb8dfcb8e215fd3917b721fdb721c1eeea2b14948f4782413846bb';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.8%2B10_openj9-0.21.0/OpenJDK11U-jdk_s390x_linux_openj9_11.0.8_10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9ab79436180d41809f4fca8afe43e778ae2d82c7b50f3653c62d7a2728150836';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.8%2B10_openj9-0.21.0/OpenJDK11U-jdk_x64_linux_openj9_11.0.8_10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 22:34:38 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 22:34:46 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Wed, 19 Aug 2020 22:34:52 GMT
CMD ["jshell"]
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
	-	`sha256:ca991f64dfbc044a1134262988ed19378c5a6205ac1a3ab3bfefd7ad09bfcaaf`  
		Last Modified: Wed, 19 Aug 2020 22:46:49 GMT  
		Size: 197.3 MB (197290252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:11-jdk-openj9-bionic` - linux; s390x

```console
$ docker pull adoptopenjdk@sha256:03205be702e053659eb931a4a234fee3ec53a9436fc3295d2ae2b6296aba4566
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.9 MB (233855487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8b904711c3a5bce796eb4582fd409acb1bf73eb3486f15adee790dd9e39ff17`
-	Default Command: `["jshell"]`

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
# Wed, 19 Aug 2020 22:00:03 GMT
ENV JAVA_VERSION=jdk-11.0.8+10_openj9-0.21.0
# Wed, 19 Aug 2020 22:00:15 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b4bad13c0d9c2fbb1954fcddae9ccc5a32c609f2b48bf43ecaa5f39915390604';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.8%2B10_openj9-0.21.0/OpenJDK11U-jdk_aarch64_linux_openj9_11.0.8_10_openj9-0.21.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='5bcaa2075ce5bf634b542c04ea79b9ca505407b6f94d2d8350c712da387120d9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.8%2B10_openj9-0.21.0/OpenJDK11U-jdk_ppc64le_linux_openj9_11.0.8_10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='5e89692057fb8dfcb8e215fd3917b721fdb721c1eeea2b14948f4782413846bb';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.8%2B10_openj9-0.21.0/OpenJDK11U-jdk_s390x_linux_openj9_11.0.8_10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9ab79436180d41809f4fca8afe43e778ae2d82c7b50f3653c62d7a2728150836';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.8%2B10_openj9-0.21.0/OpenJDK11U-jdk_x64_linux_openj9_11.0.8_10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 22:00:19 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 22:00:19 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Wed, 19 Aug 2020 22:00:20 GMT
CMD ["jshell"]
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
	-	`sha256:725960360ad4e74d7b8f437f88a0d1d0161c07a61017c566d35904b06192aaaf`  
		Last Modified: Wed, 19 Aug 2020 22:05:55 GMT  
		Size: 194.9 MB (194851506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
