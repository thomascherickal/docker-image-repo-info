## `gradle:jdk11-alpine`

```console
$ docker pull gradle@sha256:160c818966e323414fb2e72238507734e5ed0a8ba32d6f20ee77aa59cc669df8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gradle:jdk11-alpine` - linux; amd64

```console
$ docker pull gradle@sha256:dcf95fba92fef6583c34618c234cda9fae2bd340850e0e24aeaaa48f73296a67
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **369.3 MB (369285601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a069d80578c70d6cf3e26c390553fb5acd5e12e974f74c6ffdf7a2f58c678c29`
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
# Thu, 15 Jun 2023 05:12:29 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Thu, 15 Jun 2023 05:12:38 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='45f56d75da2f55b29e7307cc790958e379abbe6b5f160a3824dc26e320c718e5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jdk_x64_alpine-linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;
# Thu, 15 Jun 2023 05:12:40 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Thu, 15 Jun 2023 05:12:40 GMT
CMD ["jshell"]
# Thu, 15 Jun 2023 09:09:41 GMT
CMD ["gradle"]
# Thu, 15 Jun 2023 09:09:41 GMT
ENV GRADLE_HOME=/opt/gradle
# Thu, 15 Jun 2023 09:09:42 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && addgroup --system --gid 1000 gradle     && adduser --system --ingroup gradle --uid 1000 --shell /bin/ash gradle     && mkdir /home/gradle/.gradle     && chown -R gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Thu, 15 Jun 2023 09:09:42 GMT
VOLUME [/home/gradle/.gradle]
# Thu, 15 Jun 2023 09:09:42 GMT
WORKDIR /home/gradle
# Thu, 15 Jun 2023 09:09:45 GMT
RUN set -o errexit -o nounset     && echo "Installing VCSes"     && apk add --no-cache       git       git-lfs       mercurial       subversion         && echo "Testing VCSes"     && which git     && which git-lfs     && which hg     && which svn
# Thu, 13 Jul 2023 20:20:25 GMT
ENV GRADLE_VERSION=8.2.1
# Thu, 13 Jul 2023 20:20:25 GMT
ARG GRADLE_DOWNLOAD_SHA256=03ec176d388f2aa99defcadc3ac6adf8dd2bce5145a129659537c0874dea5ad1
# Thu, 13 Jul 2023 20:20:30 GMT
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
	-	`sha256:ebf3b64fad2172a6b7e1f9e08e50484176b8466485309d1a761c3c64a0e10310`  
		Last Modified: Thu, 15 Jun 2023 05:16:25 GMT  
		Size: 193.9 MB (193911857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73befd8a0f35cd1eeea42516706b92c5629f75f8a1c672f90246adf5bafce6cd`  
		Last Modified: Thu, 15 Jun 2023 05:16:13 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b6cd15d9705b3b84ce63ff33b237c556b5bece37476c47ac1dc4e4ddd6f3ce`  
		Last Modified: Thu, 15 Jun 2023 09:12:42 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf061c6af8961a3ab1d1d0f13f122c0a2e117e96dbd25c774283608ced49782`  
		Last Modified: Thu, 15 Jun 2023 09:12:47 GMT  
		Size: 35.6 MB (35598740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:259bac1337184456745709594bbf79338d181b339763e6607a3e8c2ab7a480f9`  
		Last Modified: Thu, 13 Jul 2023 20:24:44 GMT  
		Size: 128.7 MB (128727248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
