## `gradle:jdk11-alpine`

```console
$ docker pull gradle@sha256:f9cd98182b2d0a8c1e00e55859e9bbc9068b9faca33df9f46f0ad28a4d81fee7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gradle:jdk11-alpine` - linux; amd64

```console
$ docker pull gradle@sha256:d71bc2aaee215cb83feaa9dc5006a9ea7b0d1e4b07c753c2e4ed8c028a25fc8b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **367.0 MB (367036030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95331094cf5acac5191f8c516a131574bed6c7814f4ad48a450cd5a0b8f165e6`
-	Default Command: `["gradle"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:48:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 29 Mar 2023 19:48:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Mar 2023 19:48:56 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 29 Mar 2023 19:48:58 GMT
RUN apk add --no-cache fontconfig libretls musl-locales musl-locales-lang ttf-dejavu tzdata zlib     && rm -rf /var/cache/apk/*
# Wed, 29 Mar 2023 19:49:29 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Wed, 29 Mar 2023 19:49:39 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='42722bdbee99ad1430d6e88f17608909f26b57ab7761fb6b87ff4dbf6a8928bc';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_x64_alpine-linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;
# Wed, 29 Mar 2023 19:49:42 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 29 Mar 2023 19:49:42 GMT
CMD ["jshell"]
# Thu, 30 Mar 2023 03:10:37 GMT
CMD ["gradle"]
# Thu, 30 Mar 2023 03:10:37 GMT
ENV GRADLE_HOME=/opt/gradle
# Thu, 30 Mar 2023 03:10:37 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && addgroup --system --gid 1000 gradle     && adduser --system --ingroup gradle --uid 1000 --shell /bin/ash gradle     && mkdir /home/gradle/.gradle     && chown -R gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Thu, 30 Mar 2023 03:10:37 GMT
VOLUME [/home/gradle/.gradle]
# Thu, 30 Mar 2023 03:10:38 GMT
WORKDIR /home/gradle
# Thu, 30 Mar 2023 03:10:41 GMT
RUN set -o errexit -o nounset     && echo "Installing VCSes"     && apk add --no-cache       git       git-lfs       mercurial       subversion         && echo "Testing VCSes"     && which git     && which git-lfs     && which hg     && which svn
# Thu, 13 Apr 2023 21:20:10 GMT
ENV GRADLE_VERSION=8.1
# Thu, 13 Apr 2023 21:20:10 GMT
ARG GRADLE_DOWNLOAD_SHA256=a62c5f99585dd9e1f95dab7b9415a0e698fa9dd1e6c38537faa81ac078f4d23e
# Thu, 13 Apr 2023 21:20:15 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=a62c5f99585dd9e1f95dab7b9415a0e698fa9dd1e6c38537faa81ac078f4d23e
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum -c -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln -s "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ed194273be4d4d02a2158c3e7c9ea96095ed70f65939d53f4968b0f225c628`  
		Last Modified: Wed, 29 Mar 2023 19:52:03 GMT  
		Size: 12.0 MB (12019605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfeea393a4f62a17d4c9c493fee278eb9d53be05eefa3c6bdd7ac1fe7fb3e86c`  
		Last Modified: Wed, 29 Mar 2023 19:52:50 GMT  
		Size: 193.8 MB (193847595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b5d734cfcf3c5d5f8e58118c2fd9f8c6211942c045b3764a28b2b1904963720`  
		Last Modified: Wed, 29 Mar 2023 19:52:38 GMT  
		Size: 179.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8f0024bfef69ba9eeef0016cb61abcc061f45376637be15ac2ea70dfc6395a9`  
		Last Modified: Thu, 30 Mar 2023 03:13:07 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb1a319a87884d828898e38c439be28a4aafa2cf4c43bbb1649fac6ad6d3d3d`  
		Last Modified: Thu, 30 Mar 2023 03:13:12 GMT  
		Size: 33.1 MB (33128112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a31a21b7aa2975193964683621796c70e9a9a10c2d2a752a78e6bc9575352c9`  
		Last Modified: Thu, 13 Apr 2023 21:23:58 GMT  
		Size: 124.7 MB (124664648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
