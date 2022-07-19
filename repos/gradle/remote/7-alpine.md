## `gradle:7-alpine`

```console
$ docker pull gradle@sha256:fa283fce6e63ffa7516e30e71735c2abc9b59ceacc9a1874b25a325b99910d30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gradle:7-alpine` - linux; amd64

```console
$ docker pull gradle@sha256:f4d41f8216cc32d3dab405af9cf30971901b9fccffef6068ca9b0f560bde8e0e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **352.8 MB (352790244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee775a0f9da5e56beb0985cdee44c1ce636a738b3696036dd5e673545bca20a8`
-	Default Command: `["gradle"]`

```dockerfile
# Mon, 18 Jul 2022 21:00:15 GMT
ADD file:a2648378045615c3785c752423b1afc8dc1c2b213393344f4d0ca17e7255c1cb in / 
# Mon, 18 Jul 2022 21:00:15 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:20:07 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 18 Jul 2022 22:20:08 GMT
RUN apk add --no-cache libretls musl-locales musl-locales-lang tzdata zlib     && rm -rf /var/cache/apk/*
# Mon, 18 Jul 2022 22:21:30 GMT
ENV JAVA_VERSION=jdk-17.0.3+7
# Mon, 18 Jul 2022 22:21:46 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='5cbaece6aec44f6d3911cfa3c5a8659889e85042aff214c944c5fa1b5938a5fc';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jdk_x64_alpine-linux_hotspot_17.0.3_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p /opt/java/openjdk; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory /opt/java/openjdk 	      --strip-components 1 	      --no-same-owner 	  ;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 18 Jul 2022 22:21:47 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 22:21:48 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Mon, 18 Jul 2022 22:21:48 GMT
CMD ["jshell"]
# Tue, 19 Jul 2022 05:00:20 GMT
CMD ["gradle"]
# Tue, 19 Jul 2022 05:00:20 GMT
ENV GRADLE_HOME=/opt/gradle
# Tue, 19 Jul 2022 05:00:21 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && addgroup --system --gid 1000 gradle     && adduser --system --ingroup gradle --uid 1000 --shell /bin/ash gradle     && mkdir /home/gradle/.gradle     && chown -R gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Tue, 19 Jul 2022 05:00:21 GMT
VOLUME [/home/gradle/.gradle]
# Tue, 19 Jul 2022 05:00:21 GMT
WORKDIR /home/gradle
# Tue, 19 Jul 2022 05:00:25 GMT
RUN set -o errexit -o nounset     && echo "Installing VCSes"     && apk add --no-cache       git       git-lfs       mercurial       subversion         && echo "Testing VCSes"     && which git     && which git-lfs     && which hg     && which svn
# Tue, 19 Jul 2022 05:00:26 GMT
ENV GRADLE_VERSION=7.5
# Tue, 19 Jul 2022 05:00:26 GMT
ARG GRADLE_DOWNLOAD_SHA256=cb87f222c5585bd46838ad4db78463a5c5f3d336e5e2b98dc7c0c586527351c2
# Tue, 19 Jul 2022 05:00:31 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=cb87f222c5585bd46838ad4db78463a5c5f3d336e5e2b98dc7c0c586527351c2
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum -c -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln -s "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:530afca65e2ea04227630ae746e0c85b2bd1a179379cbf2b6501b49c4cab2ccc`  
		Last Modified: Mon, 18 Jul 2022 19:09:35 GMT  
		Size: 2.8 MB (2798806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d31e16dc1b50d804a50e80381050a90d4dc55a110eae65cd1cef937d3dc18d3`  
		Last Modified: Mon, 18 Jul 2022 22:24:55 GMT  
		Size: 477.8 KB (477762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ea1633255a1557ec5be0901310988f2a60b65a3ee873350ac747fb18021645`  
		Last Modified: Mon, 18 Jul 2022 22:26:46 GMT  
		Size: 191.8 MB (191809263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:976b645f054d012cff86ab7d955417b543a4db89fdb6c0f85d606fc7a22ed7f5`  
		Last Modified: Mon, 18 Jul 2022 22:26:30 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3eb4e331759b2f460ceaa9966c6831728b6a3dff444a46fa66d62bda96ff569`  
		Last Modified: Tue, 19 Jul 2022 05:04:18 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13651bd84a73c332c3d9f7ef31208fb4c4a8fa07c503eb4fbd7b2053d1412494`  
		Last Modified: Tue, 19 Jul 2022 05:04:25 GMT  
		Size: 37.0 MB (37046551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd76c349bbc0e47f70888b83ff3b3087121f8661a8fb2312e3894ae62a861b5f`  
		Last Modified: Tue, 19 Jul 2022 05:04:25 GMT  
		Size: 120.7 MB (120656374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
