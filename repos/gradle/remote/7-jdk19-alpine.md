## `gradle:7-jdk19-alpine`

```console
$ docker pull gradle@sha256:0ef5c67c2dd923ceeb9cf1bdfe581dee360ed46dd1a0c969f982cc9d3c092bc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gradle:7-jdk19-alpine` - linux; amd64

```console
$ docker pull gradle@sha256:500c0632c37bcfabe324247b63d6fc5c72820756251113e5f07106c8580d2313
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **370.8 MB (370811865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:713bfe6acdc8578032855e8d2ff95a077037b4891c14cc968722b209aa923d35`
-	Default Command: `["gradle"]`

```dockerfile
# Tue, 22 Nov 2022 22:19:28 GMT
ADD file:587cae71969871d3c6456d844a8795df9b64b12c710c275295a1182b46f630e7 in / 
# Tue, 22 Nov 2022 22:19:29 GMT
CMD ["/bin/sh"]
# Tue, 29 Nov 2022 20:19:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 29 Nov 2022 20:19:48 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Nov 2022 20:19:48 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 29 Nov 2022 20:19:50 GMT
RUN apk add --no-cache fontconfig libretls musl-locales musl-locales-lang ttf-dejavu tzdata zlib     && rm -rf /var/cache/apk/*
# Tue, 29 Nov 2022 20:23:03 GMT
ENV JAVA_VERSION=jdk-19.0.1+10
# Tue, 29 Nov 2022 20:23:25 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='76cfcdf47cdf24331b51939fd2840fd387cf62471da99e4718e2e42b486a9270';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.1%2B10/OpenJDK19U-jdk_x64_alpine-linux_hotspot_19.0.1_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;
# Tue, 29 Nov 2022 20:23:27 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 29 Nov 2022 20:23:27 GMT
CMD ["jshell"]
# Thu, 01 Dec 2022 19:42:23 GMT
CMD ["gradle"]
# Thu, 01 Dec 2022 19:42:23 GMT
ENV GRADLE_HOME=/opt/gradle
# Thu, 01 Dec 2022 19:42:24 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && addgroup --system --gid 1000 gradle     && adduser --system --ingroup gradle --uid 1000 --shell /bin/ash gradle     && mkdir /home/gradle/.gradle     && chown -R gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Thu, 01 Dec 2022 19:42:24 GMT
VOLUME [/home/gradle/.gradle]
# Thu, 01 Dec 2022 19:42:24 GMT
WORKDIR /home/gradle
# Thu, 01 Dec 2022 19:42:27 GMT
RUN set -o errexit -o nounset     && echo "Installing VCSes"     && apk add --no-cache       git       git-lfs       mercurial       subversion         && echo "Testing VCSes"     && which git     && which git-lfs     && which hg     && which svn
# Thu, 01 Dec 2022 19:42:27 GMT
ENV GRADLE_VERSION=7.6
# Thu, 01 Dec 2022 19:42:28 GMT
ARG GRADLE_DOWNLOAD_SHA256=7ba68c54029790ab444b39d7e293d3236b2632631fb5f2e012bb28b4ff669e4b
# Thu, 01 Dec 2022 19:42:34 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=7ba68c54029790ab444b39d7e293d3236b2632631fb5f2e012bb28b4ff669e4b
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum -c -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln -s "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:c158987b05517b6f2c5913f3acef1f2182a32345a304fe357e3ace5fadcad715`  
		Last Modified: Tue, 22 Nov 2022 22:19:52 GMT  
		Size: 3.4 MB (3370706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e5acd5897d762b9a83758d4ceae374df7b8b0367a48cc14b8a00e33998b3bf`  
		Last Modified: Tue, 29 Nov 2022 20:26:18 GMT  
		Size: 12.0 MB (12020105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb257bdcbcd975e9e493219f6dd7220ab6e1c8bcce4128755b8ae59018a8707`  
		Last Modified: Tue, 29 Nov 2022 20:30:53 GMT  
		Size: 200.3 MB (200303543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fef00b4aa6e0e9007248b2d1c189b91d9057213910cc481afd6024e001eaeb9`  
		Last Modified: Tue, 29 Nov 2022 20:30:38 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96cf23ca9339d90e4643ac16a1f2e1a6fccaa39e5ab29ee9682af4ed7c8f4e04`  
		Last Modified: Thu, 01 Dec 2022 19:46:20 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fbab1b2f6a5c2499ff4921eba6079364b73cec768fa54d1d4c79cd018290156`  
		Last Modified: Thu, 01 Dec 2022 19:46:25 GMT  
		Size: 33.1 MB (33058989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6879239dd70ce0a6a2a2c0ccb3a68bf4b678a0cdde0867b9f48daeb7a36a63a7`  
		Last Modified: Thu, 01 Dec 2022 19:46:26 GMT  
		Size: 122.1 MB (122057017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
