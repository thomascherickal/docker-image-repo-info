## `gradle:alpine`

```console
$ docker pull gradle@sha256:769db4d30a935c368cdd42757fd8dae06aebaf8998c28dc1583d55d1cb495986
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gradle:alpine` - linux; amd64

```console
$ docker pull gradle@sha256:4c402bf4c0b4c33accc87aa2a3a4a33a7ac4b05ecfc202539bb5673b70c00695
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **345.0 MB (344963028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eb6f8808028380d114ca5f6cac22ec9ff5bcd885b59756d1fae9afa61fd3d7b`
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
# Fri, 24 Sep 2021 19:20:30 GMT
ENV JAVA_VERSION=jdk-17+35
# Fri, 24 Sep 2021 19:20:42 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='03321e009cc5955d7dbabc9219434d63a5b390c223c8ecc303eb1741eb9036ef';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17%2B35/OpenJDK17-jdk_x64_alpine-linux_hotspot_17_35.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p /opt/java/openjdk; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory /opt/java/openjdk 	      --strip-components 1 	      --no-same-owner 	  ;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 24 Sep 2021 19:20:42 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Sep 2021 19:20:43 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 24 Sep 2021 19:20:43 GMT
CMD ["jshell"]
# Mon, 01 Nov 2021 22:38:56 GMT
CMD ["gradle"]
# Mon, 01 Nov 2021 22:38:57 GMT
ENV GRADLE_HOME=/opt/gradle
# Mon, 01 Nov 2021 22:38:57 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && addgroup -S -g 1000 gradle     && adduser -D -S -G gradle -u 1000 -s /bin/ash gradle     && mkdir /home/gradle/.gradle     && chown -R gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Mon, 01 Nov 2021 22:38:57 GMT
VOLUME [/home/gradle/.gradle]
# Mon, 01 Nov 2021 22:38:58 GMT
WORKDIR /home/gradle
# Mon, 01 Nov 2021 22:39:01 GMT
RUN set -o errexit -o nounset     && echo "Installing VCSes"     && apk add --no-cache       git       git-lfs       mercurial       subversion         && echo "Testing VCSes"     && which git     && which git-lfs     && which hg     && which svn
# Mon, 01 Nov 2021 22:39:02 GMT
ENV GRADLE_VERSION=7.2
# Mon, 01 Nov 2021 22:39:02 GMT
ARG GRADLE_DOWNLOAD_SHA256=f581709a9c35e9cb92e16f585d2c4bc99b2b1a5f85d2badbd3dc6bff59e1e6dd
# Mon, 01 Nov 2021 22:39:07 GMT
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
	-	`sha256:07d8ba3cf6cc5919b2690d102b82a8a714e02f24905d150825a35da2f5068f0d`  
		Last Modified: Fri, 24 Sep 2021 19:23:14 GMT  
		Size: 191.9 MB (191889819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff8ea996eda8bbfee06fdcbf6fe234e9b5f703caa6662ce40bc7ef309df521e`  
		Last Modified: Fri, 24 Sep 2021 19:23:00 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ebf18e155516d1d5a57af44c2d31edd035f854122984bf6030aa982b624db7`  
		Last Modified: Mon, 01 Nov 2021 22:42:55 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d70cbc98fd7c0db5e975beeaf064bb14e8de01e412c881dc0f934d990ac59b3`  
		Last Modified: Mon, 01 Nov 2021 22:43:01 GMT  
		Size: 35.5 MB (35474431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:282e1e0766d23e47da5503a5d8fe22107d5f0c85e78873519ffd8d1e629327a9`  
		Last Modified: Mon, 01 Nov 2021 22:43:01 GMT  
		Size: 114.4 MB (114374250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
