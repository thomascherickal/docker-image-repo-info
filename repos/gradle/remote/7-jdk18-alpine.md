## `gradle:7-jdk18-alpine`

```console
$ docker pull gradle@sha256:65c340ffccabe114bdd018123f0f1fdd947c0e262ada8c2b2b927ee630123306
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gradle:7-jdk18-alpine` - linux; amd64

```console
$ docker pull gradle@sha256:1575a0b7c009d37496e738134c3567809fb295ec6d409f694e0b03eb56f51b8f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **365.1 MB (365061005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81d79e4b140627d81161f790ddf78dc5e48527ed752139b018ce806701ef6d28`
-	Default Command: `["gradle"]`

```dockerfile
# Mon, 18 Jul 2022 21:00:15 GMT
ADD file:a2648378045615c3785c752423b1afc8dc1c2b213393344f4d0ca17e7255c1cb in / 
# Mon, 18 Jul 2022 21:00:15 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:20:07 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 28 Jul 2022 16:20:06 GMT
RUN apk add --no-cache fontconfig libretls musl-locales musl-locales-lang ttf-dejavu tzdata zlib     && rm -rf /var/cache/apk/*
# Tue, 02 Aug 2022 19:09:34 GMT
ENV JAVA_VERSION=jdk-18.0.2+9
# Tue, 02 Aug 2022 19:09:54 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='045670342a036fff98b2ee90279ed923dc8c92bebe6227a2a60f64ca84f4f7c8';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.2%2B9/OpenJDK18U-jdk_x64_alpine-linux_hotspot_18.0.2_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p /opt/java/openjdk; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory /opt/java/openjdk 	      --strip-components 1 	      --no-same-owner 	  ;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 02 Aug 2022 19:09:54 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 19:09:55 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 02 Aug 2022 19:09:55 GMT
CMD ["jshell"]
# Wed, 03 Aug 2022 12:36:20 GMT
CMD ["gradle"]
# Wed, 03 Aug 2022 12:36:20 GMT
ENV GRADLE_HOME=/opt/gradle
# Wed, 03 Aug 2022 12:36:21 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && addgroup --system --gid 1000 gradle     && adduser --system --ingroup gradle --uid 1000 --shell /bin/ash gradle     && mkdir /home/gradle/.gradle     && chown -R gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Wed, 03 Aug 2022 12:36:21 GMT
VOLUME [/home/gradle/.gradle]
# Wed, 03 Aug 2022 12:36:21 GMT
WORKDIR /home/gradle
# Wed, 03 Aug 2022 12:36:24 GMT
RUN set -o errexit -o nounset     && echo "Installing VCSes"     && apk add --no-cache       git       git-lfs       mercurial       subversion         && echo "Testing VCSes"     && which git     && which git-lfs     && which hg     && which svn
# Mon, 08 Aug 2022 19:28:35 GMT
ENV GRADLE_VERSION=7.5.1
# Mon, 08 Aug 2022 19:28:35 GMT
ARG GRADLE_DOWNLOAD_SHA256=f6b8596b10cce501591e92f229816aa4046424f3b24d771751b06779d58c8ec4
# Mon, 08 Aug 2022 19:28:41 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=f6b8596b10cce501591e92f229816aa4046424f3b24d771751b06779d58c8ec4
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum -c -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln -s "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:530afca65e2ea04227630ae746e0c85b2bd1a179379cbf2b6501b49c4cab2ccc`  
		Last Modified: Mon, 18 Jul 2022 19:09:35 GMT  
		Size: 2.8 MB (2798806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2b3b9d0d1a1f972083dde62c850175d26be845971e3c96ff06c8145fbe2fd0`  
		Last Modified: Thu, 28 Jul 2022 16:25:19 GMT  
		Size: 12.1 MB (12050034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63767b55bc166472c10e5963b6ad0046b42e404d6b8d5486f7a8ac826d179660`  
		Last Modified: Tue, 02 Aug 2022 19:18:32 GMT  
		Size: 192.9 MB (192897541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc4105de4129bcb708e2f690c2ac2d9e5a9d6704e5d998ca95a2ce3087cb9e4`  
		Last Modified: Tue, 02 Aug 2022 19:18:17 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe99f68614c73652073b023dd6bbbffb8f0f3ef832c34111650d8510b5bd3f20`  
		Last Modified: Wed, 03 Aug 2022 12:44:51 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843e0219564e947e015e16d0f55cc6f6bd5fe885cf0ba06b55b54b9476ef56c2`  
		Last Modified: Wed, 03 Aug 2022 12:44:57 GMT  
		Size: 36.7 MB (36655130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67ee3e634c94ccd8657d57f2d2203ee03dd0c32df223d7c8e2b4a128b59f285f`  
		Last Modified: Mon, 08 Aug 2022 19:36:58 GMT  
		Size: 120.7 MB (120658003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
