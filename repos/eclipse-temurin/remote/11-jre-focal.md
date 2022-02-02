## `eclipse-temurin:11-jre-focal`

```console
$ docker pull eclipse-temurin@sha256:b8ec17fa7c914fb96fa7cc90f5556b505508a1d652465c10b713e516cc5783d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `eclipse-temurin:11-jre-focal` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:1d82ba6e81d9b0c14d0cadbad278e688f2c01dff79bd6911b7610340e3d2b146
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.6 MB (96609283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4520f806b3be105b7067621abf3090340174417f13ca1ad011feb50f18f9482c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:57:26 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 02:58:19 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:58:52 GMT
ENV JAVA_VERSION=jdk-11.0.14+9
# Wed, 02 Feb 2022 02:59:21 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f20bcf8c29057b7275876b1d9e68c13dca03789750ddfabdb213a69f3aa3fcf5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.14_9.tar.gz';          ;;        armhf|arm)          ESUM='675fb486e99060e097d194178f6bd387585c06647eeac27109145a0f03ec3b92';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.14_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='fc94df3676ebae655a4a1c07767535f12d72b3d913d5111f5f21ac9e1a009572';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.14_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='d2a631aa367d9ef37082e0b1f5d21d18cffddbe24045f4b2fb318d4ba841c3fd';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.14_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='f9c0b0c5f379f57424a1cb9fb304003aeb827817d8b12164388792e145011480';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.14_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 02:59:21 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 02:59:22 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd22f8f9007b7341ddccd906a9f476337b871592380b8c0c2cc5f7c8e4b16928`  
		Last Modified: Wed, 02 Feb 2022 03:02:00 GMT  
		Size: 24.8 MB (24814660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a585a8f8fd99d708129717ae5fdac2d9fe803a5fee3291ff479f8dc04db42494`  
		Last Modified: Wed, 02 Feb 2022 03:03:11 GMT  
		Size: 43.2 MB (43230362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:965f03a4fb8d3d6c8106ee5f1bef091485bf8ae217d5c0a0b0e09f5c0e1a442f`  
		Last Modified: Wed, 02 Feb 2022 03:03:04 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:11-jre-focal` - linux; arm variant v7

```console
$ docker pull eclipse-temurin@sha256:6ca411d1053509813c5a9cedb0068cdb76f555b106a57e31d4f09c14ac59c5c9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.0 MB (88985698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07aa80834208a8a492997d80b4c21752658c73e1ef86362d798777e11b93aeae`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 02 Feb 2022 02:25:11 GMT
ADD file:0adc3f597b5ba8c31a9a4d67126166cf067749754e269fe2c3ed43f03457b53c in / 
# Wed, 02 Feb 2022 02:25:12 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:47:09 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 02:48:03 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:48:04 GMT
ENV JAVA_VERSION=jdk-11.0.14+9
# Wed, 02 Feb 2022 02:49:02 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f20bcf8c29057b7275876b1d9e68c13dca03789750ddfabdb213a69f3aa3fcf5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.14_9.tar.gz';          ;;        armhf|arm)          ESUM='675fb486e99060e097d194178f6bd387585c06647eeac27109145a0f03ec3b92';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.14_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='fc94df3676ebae655a4a1c07767535f12d72b3d913d5111f5f21ac9e1a009572';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.14_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='d2a631aa367d9ef37082e0b1f5d21d18cffddbe24045f4b2fb318d4ba841c3fd';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.14_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='f9c0b0c5f379f57424a1cb9fb304003aeb827817d8b12164388792e145011480';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.14_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 02:49:03 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 02:49:05 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:42bcffb5d2901aadaedc35f036cf725a537494a5869ae378ec427d313ff41fa6`  
		Last Modified: Wed, 02 Feb 2022 02:29:41 GMT  
		Size: 24.1 MB (24062751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca45b223849013a5db7d5850e0832f4aac669b33c69f09d9d74f6d6ae56a91d8`  
		Last Modified: Wed, 02 Feb 2022 02:54:22 GMT  
		Size: 23.1 MB (23072061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605123915fece369da5778c9391348661f9ac3f37a8d4e3663c9c282ef486789`  
		Last Modified: Wed, 02 Feb 2022 02:55:57 GMT  
		Size: 41.9 MB (41850725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2b512710f7691986f4b2e05d64e27b40ab28ad601c130c9d986ca42d03dcb2`  
		Last Modified: Wed, 02 Feb 2022 02:55:31 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:11-jre-focal` - linux; arm64 variant v8

```console
$ docker pull eclipse-temurin@sha256:b20cf09a608085da06eba74ff2cee55089b6ba42e7b15884be28ea1403a9f0d3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.5 MB (93504680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8e63584fcdf1016a8dfe3d08e3e72e9e5529de866b7e4e10b491d9b3101d7e4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 02 Feb 2022 03:19:27 GMT
ADD file:3acc741be29b0b58e44d7302ab5ce65bf65ea1b35922be58a2cee9cb708d006a in / 
# Wed, 02 Feb 2022 03:19:27 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 05:01:31 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 05:01:53 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 05:02:34 GMT
ENV JAVA_VERSION=jdk-11.0.14+9
# Wed, 02 Feb 2022 05:03:05 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f20bcf8c29057b7275876b1d9e68c13dca03789750ddfabdb213a69f3aa3fcf5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.14_9.tar.gz';          ;;        armhf|arm)          ESUM='675fb486e99060e097d194178f6bd387585c06647eeac27109145a0f03ec3b92';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.14_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='fc94df3676ebae655a4a1c07767535f12d72b3d913d5111f5f21ac9e1a009572';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.14_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='d2a631aa367d9ef37082e0b1f5d21d18cffddbe24045f4b2fb318d4ba841c3fd';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.14_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='f9c0b0c5f379f57424a1cb9fb304003aeb827817d8b12164388792e145011480';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.14_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 05:03:05 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 05:03:07 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:bbf2fb66fa6e06dd46eb26f518f93171ee7c48be68aafb213aa7c2c12f4018ca`  
		Last Modified: Wed, 02 Feb 2022 03:21:24 GMT  
		Size: 27.2 MB (27169640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20305b79e1520f1abaac4873914620f971be40e552579ba5d7dae3be52dd4f68`  
		Last Modified: Wed, 02 Feb 2022 05:06:28 GMT  
		Size: 24.8 MB (24762728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47f6151ca955d4b7fb01dfd3c4470cc07f8484a7de594e6028377da2392b0b9d`  
		Last Modified: Wed, 02 Feb 2022 05:07:49 GMT  
		Size: 41.6 MB (41572184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d5b05b981cfd36cda3c95e6c1b623132675dfd8e918bc928fb89bffc419f28`  
		Last Modified: Wed, 02 Feb 2022 05:07:42 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:11-jre-focal` - linux; ppc64le

```console
$ docker pull eclipse-temurin@sha256:80910b001b6f36dec34fa5b716d0e46c55d45235c4c6d14a80a1b4d7aaa74283
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.6 MB (98569221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5933c199b5af293d01d347517af634cde22e812e849ec1a3f73c836a06a0228e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 02 Feb 2022 03:50:21 GMT
ADD file:e27da75ca1655de0ac82ef9879f868863388ea992e031aeace61195495bc21bc in / 
# Wed, 02 Feb 2022 03:50:25 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 05:45:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 05:48:39 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 05:50:12 GMT
ENV JAVA_VERSION=jdk-11.0.14+9
# Wed, 02 Feb 2022 05:51:15 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f20bcf8c29057b7275876b1d9e68c13dca03789750ddfabdb213a69f3aa3fcf5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.14_9.tar.gz';          ;;        armhf|arm)          ESUM='675fb486e99060e097d194178f6bd387585c06647eeac27109145a0f03ec3b92';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.14_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='fc94df3676ebae655a4a1c07767535f12d72b3d913d5111f5f21ac9e1a009572';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.14_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='d2a631aa367d9ef37082e0b1f5d21d18cffddbe24045f4b2fb318d4ba841c3fd';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.14_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='f9c0b0c5f379f57424a1cb9fb304003aeb827817d8b12164388792e145011480';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.14_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 05:51:19 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 05:51:26 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:e4ad98202983f0b602991305f807e9b8460bb3fdb617889c276ccbd4b92c69b4`  
		Last Modified: Wed, 02 Feb 2022 03:53:11 GMT  
		Size: 33.3 MB (33284717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b628b171f10e336a4f91bbf963a6d636a2d90773ed7eef1ecafde5d9939c3c11`  
		Last Modified: Wed, 02 Feb 2022 05:57:19 GMT  
		Size: 26.6 MB (26643271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0ac27cb36bb8dd24defb16aca611d9a310ff50291b151fb1179fbb18e234e7`  
		Last Modified: Wed, 02 Feb 2022 05:58:45 GMT  
		Size: 38.6 MB (38641073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68febafb066e63efbfcc3c94c15fa0fdf31cc82e9682488ffc94ebe35434214a`  
		Last Modified: Wed, 02 Feb 2022 05:58:38 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:11-jre-focal` - linux; s390x

```console
$ docker pull eclipse-temurin@sha256:998347ad7ea8339c591a019d210c352987dc1541a7774d31e9df1c0d03f93fec
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.9 MB (88894531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:002505ed3acb3332a4466914e10897f040e7a8a9c45a427658e4144c61f43db3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:22:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 02:23:15 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:23:16 GMT
ENV JAVA_VERSION=jdk-11.0.14+9
# Wed, 02 Feb 2022 02:23:45 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f20bcf8c29057b7275876b1d9e68c13dca03789750ddfabdb213a69f3aa3fcf5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.14_9.tar.gz';          ;;        armhf|arm)          ESUM='675fb486e99060e097d194178f6bd387585c06647eeac27109145a0f03ec3b92';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.14_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='fc94df3676ebae655a4a1c07767535f12d72b3d913d5111f5f21ac9e1a009572';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.14_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='d2a631aa367d9ef37082e0b1f5d21d18cffddbe24045f4b2fb318d4ba841c3fd';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.14_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='f9c0b0c5f379f57424a1cb9fb304003aeb827817d8b12164388792e145011480';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.14_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 02 Feb 2022 02:23:47 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Feb 2022 02:23:48 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e6f03368f8ab26f1db664cfc3332680df5d0a5a30115c89be2b6a6a1205c806`  
		Last Modified: Wed, 02 Feb 2022 02:26:22 GMT  
		Size: 24.4 MB (24446542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25ce1e4dbe7bbc1660306e1a6590ef71dca05ea74e4830731b98fd380333338a`  
		Last Modified: Wed, 02 Feb 2022 02:26:44 GMT  
		Size: 37.3 MB (37329092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5c4b1e6c9a96f163f0bd7dbb802fb56046a3a19914592fce4a242ee037ad5f`  
		Last Modified: Wed, 02 Feb 2022 02:26:39 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
