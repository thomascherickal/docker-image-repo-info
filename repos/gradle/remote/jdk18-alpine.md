## `gradle:jdk18-alpine`

```console
$ docker pull gradle@sha256:30b5409963189cf6a1d75895afd6f020e5679582f5064a73f85c8086eab908dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gradle:jdk18-alpine` - linux; amd64

```console
$ docker pull gradle@sha256:07697a019bfbd66aab68b50397fe4913da13f033cae6e6899862cd88a640078f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **353.8 MB (353843338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd5f7c5db68c82b9bf901132658630c824241c9f2048c9b8a4aa26039c8e4094`
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
# Mon, 18 Jul 2022 22:22:12 GMT
ENV JAVA_VERSION=jdk-18.0.1+10
# Mon, 18 Jul 2022 22:22:51 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='ab72b28e1ce896e6b11e2b362c12c36007ebe9963d8954bc11e637be1f024dfe';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jdk_x64_alpine-linux_hotspot_18.0.1_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p /opt/java/openjdk; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory /opt/java/openjdk 	      --strip-components 1 	      --no-same-owner 	  ;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 18 Jul 2022 22:22:52 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 22:22:53 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Mon, 18 Jul 2022 22:22:53 GMT
CMD ["jshell"]
# Tue, 19 Jul 2022 05:00:41 GMT
CMD ["gradle"]
# Tue, 19 Jul 2022 05:00:41 GMT
ENV GRADLE_HOME=/opt/gradle
# Tue, 19 Jul 2022 05:00:42 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && addgroup --system --gid 1000 gradle     && adduser --system --ingroup gradle --uid 1000 --shell /bin/ash gradle     && mkdir /home/gradle/.gradle     && chown -R gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Tue, 19 Jul 2022 05:00:42 GMT
VOLUME [/home/gradle/.gradle]
# Tue, 19 Jul 2022 05:00:42 GMT
WORKDIR /home/gradle
# Tue, 19 Jul 2022 05:00:46 GMT
RUN set -o errexit -o nounset     && echo "Installing VCSes"     && apk add --no-cache       git       git-lfs       mercurial       subversion         && echo "Testing VCSes"     && which git     && which git-lfs     && which hg     && which svn
# Tue, 19 Jul 2022 05:00:46 GMT
ENV GRADLE_VERSION=7.5
# Tue, 19 Jul 2022 05:00:46 GMT
ARG GRADLE_DOWNLOAD_SHA256=cb87f222c5585bd46838ad4db78463a5c5f3d336e5e2b98dc7c0c586527351c2
# Tue, 19 Jul 2022 05:00:52 GMT
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
	-	`sha256:1692a66f228637064c28c12822caa558cc227d8c55be05dcd9c13f23afe1c3f6`  
		Last Modified: Mon, 18 Jul 2022 22:27:37 GMT  
		Size: 192.9 MB (192862448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae49683e5b028ebf7144f182d99885f81d7393f9ff9fe771a3b2a84e652cc1a4`  
		Last Modified: Mon, 18 Jul 2022 22:27:22 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8c88e83276cbd4526104ac20746fa6c6bb26617126dd7d43eca9fbed506704`  
		Last Modified: Tue, 19 Jul 2022 05:05:09 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f68ad3b8c5b81a32469db5a783a97d288bbcfa03ba07077d53d0d1f6023eda`  
		Last Modified: Tue, 19 Jul 2022 05:05:15 GMT  
		Size: 37.0 MB (37046521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b8a0917ec509dee268267f866e5f5ee5cb39676d5c3d8556dfb8da679b5719a`  
		Last Modified: Tue, 19 Jul 2022 05:05:20 GMT  
		Size: 120.7 MB (120656310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
