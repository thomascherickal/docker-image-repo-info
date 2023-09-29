## `gradle:jdk11-alpine`

```console
$ docker pull gradle@sha256:ca7f3be46cbfb7ab30b0c251918b6afcbaaac5bbe5f82c2c61194444bf176993
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gradle:jdk11-alpine` - linux; amd64

```console
$ docker pull gradle@sha256:c97032b2d26195710c952781f8a801ea7dfd19f741343c8c9b381e1e56aacb52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.5 MB (318538138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e3ed951e1302e25ea47cca81adc316e034f5aaed6dc2c69c40968f29fcf505b`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`
-	Default Command: `["gradle"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 23:24:23 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 28 Sep 2023 23:24:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Sep 2023 23:24:24 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 28 Sep 2023 23:24:25 GMT
RUN apk add --no-cache fontconfig java-cacerts bash libretls musl-locales musl-locales-lang ttf-dejavu tzdata zlib     && rm -rf /var/cache/apk/*
# Thu, 28 Sep 2023 23:25:02 GMT
ENV JAVA_VERSION=jdk-11.0.20.1+1
# Thu, 28 Sep 2023 23:25:10 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='1a94e642bf6cc4124d4f01f43184f9127ef994cbd324e2ee42cc50f715cbaedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_x64_alpine-linux_hotspot_11.0.20.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Thu, 28 Sep 2023 23:25:13 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Thu, 28 Sep 2023 23:25:13 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Thu, 28 Sep 2023 23:25:13 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Thu, 28 Sep 2023 23:25:13 GMT
CMD ["jshell"]
# Fri, 29 Sep 2023 03:51:10 GMT
CMD ["gradle"]
# Fri, 29 Sep 2023 03:51:10 GMT
ENV GRADLE_HOME=/opt/gradle
# Fri, 29 Sep 2023 03:51:10 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && addgroup --system --gid 1000 gradle     && adduser --system --ingroup gradle --uid 1000 --shell /bin/ash gradle     && mkdir /home/gradle/.gradle     && chown -R gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Fri, 29 Sep 2023 03:51:10 GMT
VOLUME [/home/gradle/.gradle]
# Fri, 29 Sep 2023 03:51:10 GMT
WORKDIR /home/gradle
# Fri, 29 Sep 2023 03:51:13 GMT
RUN set -o errexit -o nounset     && echo "Installing VCSes"     && apk add --no-cache       git       git-lfs       mercurial       subversion         && echo "Testing VCSes"     && which git     && which git-lfs     && which hg     && which svn
# Fri, 29 Sep 2023 03:51:14 GMT
ENV GRADLE_VERSION=8.3
# Fri, 29 Sep 2023 03:51:14 GMT
ARG GRADLE_DOWNLOAD_SHA256=591855b517fc635b9e04de1d05d5e76ada3f89f5fc76f87978d1b245b4f69225
# Fri, 29 Sep 2023 03:51:19 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=591855b517fc635b9e04de1d05d5e76ada3f89f5fc76f87978d1b245b4f69225
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking Gradle download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum -c -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln -s "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle
# Fri, 29 Sep 2023 03:51:19 GMT
USER gradle
# Fri, 29 Sep 2023 03:51:20 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=591855b517fc635b9e04de1d05d5e76ada3f89f5fc76f87978d1b245b4f69225
RUN set -o errexit -o nounset     && echo "Testing Gradle installation"     && gradle --version
# Fri, 29 Sep 2023 03:51:20 GMT
USER root
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34e4092d737c5d0c601ddadd8d075b756e55cc717065ae83683571965c2117a9`  
		Last Modified: Thu, 28 Sep 2023 23:28:20 GMT  
		Size: 9.3 MB (9276514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a363adaeeae522cf68572d9f985bdee8d6dd35547169bb62cb4a5e65c6b359e4`  
		Last Modified: Thu, 28 Sep 2023 23:29:11 GMT  
		Size: 140.2 MB (140159189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801ecece587301dd00ac27da98df931840bd4da3eede6ae68ba5f5de6ecc993b`  
		Last Modified: Thu, 28 Sep 2023 23:29:00 GMT  
		Size: 180.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16c1d9a36e7ab385c1d5fca98d54d5e80bb305341468cf266d952b8a5f4b0a8`  
		Last Modified: Thu, 28 Sep 2023 23:29:00 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4031919647cbf45bc1f5a4c6cc6722178f4014420c7afceac2003a96f9dc60`  
		Last Modified: Fri, 29 Sep 2023 03:54:53 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:396745b371575e2461fc186510cbc1917e57aa546fea4283a02fea9b16736d2c`  
		Last Modified: Fri, 29 Sep 2023 03:54:59 GMT  
		Size: 35.0 MB (35031100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c9e4b4259fd5042047022e8300f8b08d63402cb0745b68f136b67521941fcc`  
		Last Modified: Fri, 29 Sep 2023 03:55:08 GMT  
		Size: 130.7 MB (130666952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3b6af08eff809c2ef55c1be695e7fe7e97b7f970ed935c7a107ab3b0d33471`  
		Last Modified: Fri, 29 Sep 2023 03:54:54 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
