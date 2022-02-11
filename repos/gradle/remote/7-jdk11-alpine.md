## `gradle:7-jdk11-alpine`

```console
$ docker pull gradle@sha256:68687b98f21076602e14ee6d227f150f1d115a64741da69a3503cef8e42daf57
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gradle:7-jdk11-alpine` - linux; amd64

```console
$ docker pull gradle@sha256:88bf652f9e19429ea690d24c0d5f56b96d67ecac1b052389f83e0d6124b05de3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **347.4 MB (347406409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4dbc22d8f38dccfe85064b5708aa96f63afea97934994044ebdb8c0fb2c9ec6`
-	Default Command: `["gradle"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Thu, 13 Jan 2022 17:19:44 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 13 Jan 2022 17:19:46 GMT
RUN apk add --no-cache tzdata musl-locales musl-locales-lang     && rm -rf /var/cache/apk/*
# Tue, 01 Feb 2022 22:21:40 GMT
ENV JAVA_VERSION=jdk-11.0.14+9
# Tue, 01 Feb 2022 22:21:55 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='f94a01258a5496eda9e3de6807e6ecfe08a5ad4a2d42e4332a77f74174706f5c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14%2B9/OpenJDK11U-jdk_x64_alpine-linux_hotspot_11.0.14_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p /opt/java/openjdk; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory /opt/java/openjdk 	      --strip-components 1 	      --no-same-owner 	  ;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 01 Feb 2022 22:21:56 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Feb 2022 22:21:57 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 01 Feb 2022 22:21:57 GMT
CMD ["jshell"]
# Tue, 01 Feb 2022 23:02:57 GMT
CMD ["gradle"]
# Tue, 01 Feb 2022 23:02:57 GMT
ENV GRADLE_HOME=/opt/gradle
# Tue, 01 Feb 2022 23:02:58 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && addgroup --system --gid 1000 gradle     && adduser --system --ingroup gradle --uid 1000 --shell /bin/ash gradle     && mkdir /home/gradle/.gradle     && chown -R gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Tue, 01 Feb 2022 23:02:58 GMT
VOLUME [/home/gradle/.gradle]
# Tue, 01 Feb 2022 23:02:58 GMT
WORKDIR /home/gradle
# Tue, 01 Feb 2022 23:03:02 GMT
RUN set -o errexit -o nounset     && echo "Installing VCSes"     && apk add --no-cache       git       git-lfs       mercurial       subversion         && echo "Testing VCSes"     && which git     && which git-lfs     && which hg     && which svn
# Fri, 11 Feb 2022 01:19:50 GMT
ENV GRADLE_VERSION=7.4
# Fri, 11 Feb 2022 01:19:50 GMT
ARG GRADLE_DOWNLOAD_SHA256=8cc27038d5dbd815759851ba53e70cf62e481b87494cc97cfd97982ada5ba634
# Fri, 11 Feb 2022 01:19:55 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=8cc27038d5dbd815759851ba53e70cf62e481b87494cc97cfd97982ada5ba634
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum -c -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln -s "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7418fdfb53d3b677d087a50df49ad12829a9eab2f0b2c8c19b162589387891`  
		Last Modified: Thu, 13 Jan 2022 17:22:44 GMT  
		Size: 430.3 KB (430278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce0d973b8a34293ba4230b845d4a5f0726a1f2af09f1078b765bf8874db49ca`  
		Last Modified: Tue, 01 Feb 2022 22:26:54 GMT  
		Size: 192.9 MB (192892914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:510eb7edaa97518f5ffadf64ce784eab2e0da839a76d8e140855a446482d6d87`  
		Last Modified: Tue, 01 Feb 2022 22:26:40 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f66883a4187f8e1499816ba2a4a778f7e8b05f24024e85016beeb1ac5979137`  
		Last Modified: Tue, 01 Feb 2022 23:06:34 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c123da932984a255f2bc13e9e4920e18e41b087f98c53c041b8c256a9a1b5721`  
		Last Modified: Tue, 01 Feb 2022 23:06:40 GMT  
		Size: 35.4 MB (35398466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1f4681534013f84b61931fd843dcf89036a08ee4f3e21cac5bfd369038135a`  
		Last Modified: Fri, 11 Feb 2022 01:22:13 GMT  
		Size: 115.9 MB (115864855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
