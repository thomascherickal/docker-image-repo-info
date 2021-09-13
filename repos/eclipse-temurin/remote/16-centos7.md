## `eclipse-temurin:16-centos7`

```console
$ docker pull eclipse-temurin@sha256:47c484e51b90442bf97ddfb055b87a5e9e64e5ce8c47c27a774d16659d982752
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `eclipse-temurin:16-centos7` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:715a41d8fd9416fdb91039200cd882faffa85b28c473fcb6421aff59bd1f44ac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.3 MB (295268509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f858de989d4b61b5b7db684c4606c48c54c9503820945a1b4d7893b7e872af4`
-	Default Command: `["jshell"]`

```dockerfile
# Sat, 14 Nov 2020 00:20:04 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Sat, 14 Nov 2020 00:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Sat, 14 Nov 2020 00:20:04 GMT
CMD ["/bin/bash"]
# Fri, 13 Aug 2021 21:32:11 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 13 Sep 2021 18:22:03 GMT
RUN yum install -y tzdata openssl curl ca-certificates fontconfig gzip tar binutils     && yum clean all
# Mon, 13 Sep 2021 18:22:04 GMT
ENV JAVA_VERSION=jdk-16.0.2+7
# Mon, 13 Sep 2021 18:22:12 GMT
RUN set -eux;     ARCH="$(uname -m)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cb77d9d126f97898dfdc8b5fb694d1e0e5d93d13a0a6cb2aeda76f8635384340';          BINARY_URL='https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_aarch64_linux_hotspot_16.0.2_7.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='36ebe6c72f2fc19b8b17371f731390e15fa3aab08c28b55b9a8b71d0a578adc9';          BINARY_URL='https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_ppc64le_linux_hotspot_16.0.2_7.tar.gz';          ;;        amd64|x86_64)          ESUM='323d6d7474a359a28eff7ddd0df8e65bd61554a8ed12ef42fd9365349e573c2c';          BINARY_URL='https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_x64_linux_hotspot_16.0.2_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 13 Sep 2021 18:22:13 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 13 Sep 2021 18:22:14 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Mon, 13 Sep 2021 18:22:14 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4d1e2eefb2ba7f44fd4e580bad325e6f5fb0c970c7c7c28105774c2d81ee98`  
		Last Modified: Mon, 13 Sep 2021 18:25:23 GMT  
		Size: 12.7 MB (12704135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f487fb4b28e0a865c505c855b96c7fee1ccac3ce6c5168161d8c439053a493fe`  
		Last Modified: Mon, 13 Sep 2021 18:25:36 GMT  
		Size: 206.5 MB (206467055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a9df459a574e80fad4009d389ef3a69809e0dd0b20712657930bd5cfc0bb82`  
		Last Modified: Mon, 13 Sep 2021 18:25:21 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:16-centos7` - linux; arm64 variant v8

```console
$ docker pull eclipse-temurin@sha256:13061b615fff61f631064bfb021d08234210182ce1a88c3b9a90a3d191001ff4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.8 MB (324763203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63a05450d117f8d89d500c1d3d103499564287c1c0a7ac4c890fd474255ca2c4`
-	Default Command: `["jshell"]`

```dockerfile
# Sat, 14 Nov 2020 00:40:26 GMT
ADD file:5b1e63a3cb041177b802b501dedcd71a86f1773ea0f69f048f2eb3901097711d in / 
# Sat, 14 Nov 2020 00:40:31 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Sat, 14 Nov 2020 00:40:32 GMT
CMD ["/bin/bash"]
# Fri, 13 Aug 2021 21:31:50 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 13 Sep 2021 17:42:09 GMT
RUN yum install -y tzdata openssl curl ca-certificates fontconfig gzip tar binutils     && yum clean all
# Mon, 13 Sep 2021 17:42:09 GMT
ENV JAVA_VERSION=jdk-16.0.2+7
# Mon, 13 Sep 2021 17:42:24 GMT
RUN set -eux;     ARCH="$(uname -m)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cb77d9d126f97898dfdc8b5fb694d1e0e5d93d13a0a6cb2aeda76f8635384340';          BINARY_URL='https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_aarch64_linux_hotspot_16.0.2_7.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='36ebe6c72f2fc19b8b17371f731390e15fa3aab08c28b55b9a8b71d0a578adc9';          BINARY_URL='https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_ppc64le_linux_hotspot_16.0.2_7.tar.gz';          ;;        amd64|x86_64)          ESUM='323d6d7474a359a28eff7ddd0df8e65bd61554a8ed12ef42fd9365349e573c2c';          BINARY_URL='https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_x64_linux_hotspot_16.0.2_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 13 Sep 2021 17:42:25 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 13 Sep 2021 17:42:26 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Mon, 13 Sep 2021 17:42:26 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:6717b8ec66cd6add0272c6391165585613c31314a43ff77d9751b53010e531ec`  
		Last Modified: Sat, 14 Nov 2020 00:41:36 GMT  
		Size: 108.4 MB (108374945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:701e9b18b2f4a3e251a5e9c11db4e8ec4640685804530077f2b501bde1260fcd`  
		Last Modified: Mon, 13 Sep 2021 17:46:52 GMT  
		Size: 12.3 MB (12261603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f824ce155a4687d95aa374b94b16203bd51dcd0c917beedc654dd30ce03c16e5`  
		Last Modified: Mon, 13 Sep 2021 17:47:13 GMT  
		Size: 204.1 MB (204126494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18575f1d580b25fc22beddc407e85eed8fdab4bc817481aaef86ed252cc58e93`  
		Last Modified: Mon, 13 Sep 2021 17:46:50 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:16-centos7` - linux; ppc64le

```console
$ docker pull eclipse-temurin@sha256:5eac6cea57099cfc52d56ff5c0bd51f45513f3a69df5b27f4d61d96f76d3bea7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.1 MB (280076639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c6ad76aa01768fb9b56ce4a23ff2ff8a6c4f4cc3252d94559c70db55b94cb53`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 17 Nov 2020 04:05:22 GMT
ADD file:7f21ae7d20a8e347d8b678bcf26be83abb1ee27d3b567c9cddd993e45ce8ac34 in / 
# Tue, 17 Nov 2020 04:05:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Tue, 17 Nov 2020 04:05:38 GMT
CMD ["/bin/bash"]
# Fri, 13 Aug 2021 21:36:15 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 13 Aug 2021 21:37:18 GMT
RUN yum install -y tzdata openssl curl binutils ca-certificates fontconfig gzip tar     && yum clean all
# Fri, 13 Aug 2021 21:41:53 GMT
ENV JAVA_VERSION=jdk-16.0.2+7
# Fri, 13 Aug 2021 21:42:23 GMT
RUN set -eux;     ARCH="$(uname -m)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cb77d9d126f97898dfdc8b5fb694d1e0e5d93d13a0a6cb2aeda76f8635384340';          BINARY_URL='https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_aarch64_linux_hotspot_16.0.2_7.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='36ebe6c72f2fc19b8b17371f731390e15fa3aab08c28b55b9a8b71d0a578adc9';          BINARY_URL='https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_ppc64le_linux_hotspot_16.0.2_7.tar.gz';          ;;        amd64|x86_64)          ESUM='323d6d7474a359a28eff7ddd0df8e65bd61554a8ed12ef42fd9365349e573c2c';          BINARY_URL='https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_x64_linux_hotspot_16.0.2_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 13 Aug 2021 21:42:31 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Aug 2021 21:42:53 GMT
RUN echo Verifying install ...     && echo   javac --version && javac --version     && echo   java --version && java --version     && echo Complete.
# Fri, 13 Aug 2021 21:42:59 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3fe478aaff9b8f3ba958253e7339e9016ec07c075b805ebfc8cd372ddd01ee64`  
		Last Modified: Tue, 17 Nov 2020 04:06:20 GMT  
		Size: 80.5 MB (80516460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57fd707ce2425491dddf0cd7edd4e7a25914f30619f20dd2b97fc2bb6bb35972`  
		Last Modified: Fri, 13 Aug 2021 21:45:01 GMT  
		Size: 12.6 MB (12610989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c219c6a79b3b1f1751cfda84face10afba1507b937eb25c885189f5770a5ea7c`  
		Last Modified: Fri, 13 Aug 2021 21:47:32 GMT  
		Size: 186.9 MB (186949030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056bb61a5535417d5c3aa3174eed3305f75ece3ae1167498a35f00f4ac52b4c6`  
		Last Modified: Fri, 13 Aug 2021 21:47:11 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
