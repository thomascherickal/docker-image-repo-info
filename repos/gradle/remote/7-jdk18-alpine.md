## `gradle:7-jdk18-alpine`

```console
$ docker pull gradle@sha256:e756976b36cfab185d52e3fee418dad3f429036b88b2c46f30c708e7a108b312
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gradle:7-jdk18-alpine` - linux; amd64

```console
$ docker pull gradle@sha256:75259264492be43e59082e47231af093d36f3bc9867fab5e1e8291b88be5eba1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.1 MB (349051990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:130ee9fc259e468649745d3223e1d5ce6df152d7ab87c5f7c0dd7c74f197e92a`
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
# Tue, 21 Jun 2022 20:23:43 GMT
ENV JAVA_VERSION=jdk-18.0.1+10
# Tue, 21 Jun 2022 20:23:57 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='ab72b28e1ce896e6b11e2b362c12c36007ebe9963d8954bc11e637be1f024dfe';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jdk_x64_alpine-linux_hotspot_18.0.1_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p /opt/java/openjdk; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory /opt/java/openjdk 	      --strip-components 1 	      --no-same-owner 	  ;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 21 Jun 2022 20:23:57 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Jun 2022 20:23:58 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 21 Jun 2022 20:23:58 GMT
CMD ["jshell"]
# Tue, 21 Jun 2022 20:52:47 GMT
CMD ["gradle"]
# Tue, 21 Jun 2022 20:52:48 GMT
ENV GRADLE_HOME=/opt/gradle
# Tue, 21 Jun 2022 20:52:48 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && addgroup --system --gid 1000 gradle     && adduser --system --ingroup gradle --uid 1000 --shell /bin/ash gradle     && mkdir /home/gradle/.gradle     && chown -R gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Tue, 21 Jun 2022 20:52:48 GMT
VOLUME [/home/gradle/.gradle]
# Tue, 21 Jun 2022 20:52:48 GMT
WORKDIR /home/gradle
# Tue, 21 Jun 2022 20:52:52 GMT
RUN set -o errexit -o nounset     && echo "Installing VCSes"     && apk add --no-cache       git       git-lfs       mercurial       subversion         && echo "Testing VCSes"     && which git     && which git-lfs     && which hg     && which svn
# Tue, 21 Jun 2022 20:52:52 GMT
ENV GRADLE_VERSION=7.4.2
# Tue, 21 Jun 2022 20:52:52 GMT
ARG GRADLE_DOWNLOAD_SHA256=29e49b10984e585d8118b7d0bc452f944e386458df27371b49b4ac1dec4b7fda
# Tue, 21 Jun 2022 20:52:58 GMT
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
	-	`sha256:4ce063f20f3f48aa654699a8e40506412bceb1e805998d7959dd66d4b521af4b`  
		Last Modified: Tue, 21 Jun 2022 20:28:44 GMT  
		Size: 192.9 MB (192862501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0092728308d3b3e20f1e4fe1a4d2d7df28e4aaf1cf6c3e284e846452de11b684`  
		Last Modified: Tue, 21 Jun 2022 20:28:29 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a1ab783258e9523564b66f82dc8becd4d3499e366e9209975125573194eb33`  
		Last Modified: Tue, 21 Jun 2022 20:57:35 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51bf842fe7bca7ed0136f4f9d958bcc3ed88d623829c93645f2d38101b8dc67`  
		Last Modified: Tue, 21 Jun 2022 20:57:41 GMT  
		Size: 37.0 MB (37044400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acfaaeb7226822e7434fdcf83aa91181654a8f22f64a1e8b1f0d42c8f3521f55`  
		Last Modified: Tue, 21 Jun 2022 20:57:41 GMT  
		Size: 115.9 MB (115866954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
