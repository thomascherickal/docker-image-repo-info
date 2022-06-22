## `gradle:7-jdk11-alpine`

```console
$ docker pull gradle@sha256:d30ab7cceebb1ee763da49911dd95bdac839d696900f4f46b727c3a463192a91
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gradle:7-jdk11-alpine` - linux; amd64

```console
$ docker pull gradle@sha256:1c1341f5e927d5c6eeb328486e7be68d5938b3e17c451b447e0c7c86c353e94d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **350.0 MB (350001919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78bb5bba236af096364a05823f884a4237e9bc67d827f36ee237816b38f7f4c0`
-	Default Command: `["gradle"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Tue, 21 Jun 2022 20:21:34 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 21 Jun 2022 20:21:36 GMT
RUN apk add --no-cache libretls musl-locales musl-locales-lang tzdata zlib     && rm -rf /var/cache/apk/*
# Tue, 21 Jun 2022 20:22:14 GMT
ENV JAVA_VERSION=jdk-11.0.15+10
# Tue, 21 Jun 2022 20:22:29 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='b7409adf3b6d61324d734218be29b796089c1df0c994f128700c7a7fde728d1f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jdk_x64_alpine-linux_hotspot_11.0.15_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p /opt/java/openjdk; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory /opt/java/openjdk 	      --strip-components 1 	      --no-same-owner 	  ;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 21 Jun 2022 20:22:30 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Jun 2022 20:22:31 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 21 Jun 2022 20:22:31 GMT
CMD ["jshell"]
# Tue, 21 Jun 2022 20:52:04 GMT
CMD ["gradle"]
# Tue, 21 Jun 2022 20:52:04 GMT
ENV GRADLE_HOME=/opt/gradle
# Tue, 21 Jun 2022 20:52:05 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && addgroup --system --gid 1000 gradle     && adduser --system --ingroup gradle --uid 1000 --shell /bin/ash gradle     && mkdir /home/gradle/.gradle     && chown -R gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Tue, 21 Jun 2022 20:52:05 GMT
VOLUME [/home/gradle/.gradle]
# Tue, 21 Jun 2022 20:52:05 GMT
WORKDIR /home/gradle
# Tue, 21 Jun 2022 20:52:09 GMT
RUN set -o errexit -o nounset     && echo "Installing VCSes"     && apk add --no-cache       git       git-lfs       mercurial       subversion         && echo "Testing VCSes"     && which git     && which git-lfs     && which hg     && which svn
# Tue, 21 Jun 2022 20:52:10 GMT
ENV GRADLE_VERSION=7.4.2
# Tue, 21 Jun 2022 20:52:10 GMT
ARG GRADLE_DOWNLOAD_SHA256=29e49b10984e585d8118b7d0bc452f944e386458df27371b49b4ac1dec4b7fda
# Tue, 21 Jun 2022 20:52:15 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=29e49b10984e585d8118b7d0bc452f944e386458df27371b49b4ac1dec4b7fda
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum -c -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln -s "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4177d2591259bff2bae6f43f12721dbe4ed5aac24fb0991377a3d27cdd534e`  
		Last Modified: Tue, 21 Jun 2022 20:26:07 GMT  
		Size: 477.8 KB (477755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bdac5116b14573daf99d69d438779b5d5454b39e70a193bae15ca66a3a73fe0`  
		Last Modified: Tue, 21 Jun 2022 20:27:06 GMT  
		Size: 193.8 MB (193812426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9756f75b68ccb43fb81533a877105b3a90ab68c72dbde8959e9bd7a779551bb9`  
		Last Modified: Tue, 21 Jun 2022 20:26:52 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c48d5ea225420989d524be6402d77f85662e76877f61bba51a7001b1a572b4db`  
		Last Modified: Tue, 21 Jun 2022 20:55:52 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5a8493749a65ee30ef9e0554e9f36810073cf2cd7183518f38927ae8656d84`  
		Last Modified: Tue, 21 Jun 2022 20:55:58 GMT  
		Size: 37.0 MB (37044390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c74f7e5fdff3fed652f5148120665d781ad7be4a0641e0ddb82a3db00f7365`  
		Last Modified: Tue, 21 Jun 2022 20:55:58 GMT  
		Size: 115.9 MB (115866967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
