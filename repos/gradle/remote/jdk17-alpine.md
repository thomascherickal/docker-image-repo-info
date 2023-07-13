## `gradle:jdk17-alpine`

```console
$ docker pull gradle@sha256:4b72942a7054232062ef8651f4fcd6538fb066ad6ac48b01a3999518dc15f6f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gradle:jdk17-alpine` - linux; amd64

```console
$ docker pull gradle@sha256:b6cbedc6082f6d0e9ce76aee2043f568240200e665eb66adf86592b463a95142
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **367.3 MB (367299614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14a54513e2d06b62e13aaa48f48fdeaaf74e1ff9a474a81b59095cbea3452026`
-	Default Command: `["gradle"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 05:11:52 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 15 Jun 2023 05:11:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Jun 2023 05:11:52 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 15 Jun 2023 05:11:54 GMT
RUN apk add --no-cache fontconfig libretls musl-locales musl-locales-lang ttf-dejavu tzdata zlib     && rm -rf /var/cache/apk/*
# Thu, 15 Jun 2023 05:13:09 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Thu, 15 Jun 2023 05:13:19 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='b6edac2fa669876ef16b4895b36b61d01066626e7a69feba2acc19760c8d18cb';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_x64_alpine-linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;
# Thu, 15 Jun 2023 05:13:22 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Thu, 15 Jun 2023 05:13:22 GMT
CMD ["jshell"]
# Thu, 15 Jun 2023 09:10:00 GMT
CMD ["gradle"]
# Thu, 15 Jun 2023 09:10:00 GMT
ENV GRADLE_HOME=/opt/gradle
# Thu, 15 Jun 2023 09:10:01 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && addgroup --system --gid 1000 gradle     && adduser --system --ingroup gradle --uid 1000 --shell /bin/ash gradle     && mkdir /home/gradle/.gradle     && chown -R gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Thu, 15 Jun 2023 09:10:01 GMT
VOLUME [/home/gradle/.gradle]
# Thu, 15 Jun 2023 09:10:01 GMT
WORKDIR /home/gradle
# Thu, 15 Jun 2023 09:10:04 GMT
RUN set -o errexit -o nounset     && echo "Installing VCSes"     && apk add --no-cache       git       git-lfs       mercurial       subversion         && echo "Testing VCSes"     && which git     && which git-lfs     && which hg     && which svn
# Thu, 13 Jul 2023 20:20:51 GMT
ENV GRADLE_VERSION=8.2.1
# Thu, 13 Jul 2023 20:20:51 GMT
ARG GRADLE_DOWNLOAD_SHA256=03ec176d388f2aa99defcadc3ac6adf8dd2bce5145a129659537c0874dea5ad1
# Thu, 13 Jul 2023 20:20:57 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=03ec176d388f2aa99defcadc3ac6adf8dd2bce5145a129659537c0874dea5ad1
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum -c -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln -s "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aadc9aaa732ac5b0edd00545607971071fa1868047a65249e483ba2443982e6`  
		Last Modified: Thu, 15 Jun 2023 05:15:34 GMT  
		Size: 7.6 MB (7648372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc61c42d98a4031b53e224aa8cc9ebeed087bfcaee2312db7bdef6c15b75ace6`  
		Last Modified: Thu, 15 Jun 2023 05:17:11 GMT  
		Size: 191.9 MB (191925872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b872839787b43a160ad35873d407c6ed86e91883cc290c9b0d3eea46d171cb9`  
		Last Modified: Thu, 15 Jun 2023 05:16:58 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b21fa6ead900dea5e9dfb2e82d5038e0a74f9e1d6ad91eb7f812c67a958d73`  
		Last Modified: Thu, 15 Jun 2023 09:13:11 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4bb103d56d449b25a03ae59f30d991e6c17502ab7f81dc69044f5bf9e5dc35`  
		Last Modified: Thu, 15 Jun 2023 09:13:16 GMT  
		Size: 35.6 MB (35598707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb4ce2cc1bfc87301c72e2ec061a012aeb317e94e772ce8df37571f3ccfba56`  
		Last Modified: Thu, 13 Jul 2023 20:26:43 GMT  
		Size: 128.7 MB (128727278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
