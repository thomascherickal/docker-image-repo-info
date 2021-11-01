## `gradle:7-jdk11-alpine`

```console
$ docker pull gradle@sha256:e23873080935d286aa81c4abdcabe223a74bd7a7d389788b6517a598a05bd6cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gradle:7-jdk11-alpine` - linux; amd64

```console
$ docker pull gradle@sha256:6ecf5dc8509cf580b0ccafa6d4673a22c7dd89377279c2896ecc98dd2cc8b70b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **345.8 MB (345815152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10460c2b28cb653a444a992a7fbdd78551395ea1f29d5ff2f3e455133be5fff9`
-	Default Command: `["gradle"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 17 Sep 2021 21:41:38 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 24 Sep 2021 19:20:30 GMT
RUN apk add --no-cache tzdata musl-locales musl-locales-lang     && rm -rf /var/cache/apk/*
# Wed, 27 Oct 2021 00:21:11 GMT
ENV JAVA_VERSION=jdk-11.0.13+8
# Wed, 27 Oct 2021 00:21:23 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='4216543c8eaa4b10475bbacb15bbda41e04ec5c8c57424b3303f60c36b8b362d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_alpine-linux_hotspot_11.0.13_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p /opt/java/openjdk; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory /opt/java/openjdk 	      --strip-components 1 	      --no-same-owner 	  ;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 27 Oct 2021 00:21:23 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 27 Oct 2021 00:21:25 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 27 Oct 2021 00:21:25 GMT
CMD ["jshell"]
# Mon, 01 Nov 2021 22:38:09 GMT
CMD ["gradle"]
# Mon, 01 Nov 2021 22:38:09 GMT
ENV GRADLE_HOME=/opt/gradle
# Mon, 01 Nov 2021 22:38:10 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && addgroup -S -g 1000 gradle     && adduser -D -S -G gradle -u 1000 -s /bin/ash gradle     && mkdir /home/gradle/.gradle     && chown -R gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Mon, 01 Nov 2021 22:38:10 GMT
VOLUME [/home/gradle/.gradle]
# Mon, 01 Nov 2021 22:38:11 GMT
WORKDIR /home/gradle
# Mon, 01 Nov 2021 22:38:14 GMT
RUN set -o errexit -o nounset     && echo "Installing VCSes"     && apk add --no-cache       git       git-lfs       mercurial       subversion         && echo "Testing VCSes"     && which git     && which git-lfs     && which hg     && which svn
# Mon, 01 Nov 2021 22:38:15 GMT
ENV GRADLE_VERSION=7.2
# Mon, 01 Nov 2021 22:38:15 GMT
ARG GRADLE_DOWNLOAD_SHA256=f581709a9c35e9cb92e16f585d2c4bc99b2b1a5f85d2badbd3dc6bff59e1e6dd
# Mon, 01 Nov 2021 22:38:20 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=f581709a9c35e9cb92e16f585d2c4bc99b2b1a5f85d2badbd3dc6bff59e1e6dd
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum -c -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln -s "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5491faa5141cd7b6b8bcb2f0546bc3268ca907c1a0835e91db57c666453bde3d`  
		Last Modified: Fri, 24 Sep 2021 19:23:00 GMT  
		Size: 408.6 KB (408594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec07926210159dd1ea84cd07a169e8979a796564a763df0eab6cf64056626640`  
		Last Modified: Wed, 27 Oct 2021 00:23:46 GMT  
		Size: 192.7 MB (192741950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9de57a165da61917fe0d96f86e9e26626e47871236625e79da24282f177f1c6`  
		Last Modified: Wed, 27 Oct 2021 00:23:26 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:236030f732f726b82158fd6d407391664a913ce1352762bbd99f12ac4ac2a817`  
		Last Modified: Mon, 01 Nov 2021 22:41:44 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9620f41bfd5677866d8316c5c97f398941ecea79164510a1a89043a37d6e1359`  
		Last Modified: Mon, 01 Nov 2021 22:41:51 GMT  
		Size: 35.5 MB (35474437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a055211da7adb6e480eb5e9d67707c8fb62775a80c7c919ee62a1810429df6`  
		Last Modified: Mon, 01 Nov 2021 22:41:52 GMT  
		Size: 114.4 MB (114374237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
