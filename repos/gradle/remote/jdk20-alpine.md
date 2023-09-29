## `gradle:jdk20-alpine`

```console
$ docker pull gradle@sha256:453b0f125350c26264bd9879b89597a17aa30ba80fa5f6426b6eb9992ab1665f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gradle:jdk20-alpine` - linux; amd64

```console
$ docker pull gradle@sha256:0d2bc774cf69d322613508d94fbdc22d3c1eb0453fc0f62db7fd3739a8552d6d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.3 MB (331309773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06715175b50c8dcbd571a132945aa37454038dc85bebbb9931978c50b8db99c7`
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
# Thu, 28 Sep 2023 23:26:28 GMT
ENV JAVA_VERSION=jdk-20.0.2+9
# Thu, 28 Sep 2023 23:26:39 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='b03aced4b7a1c49bc00297e35e45480fd03818862b93e17e1551a3b721e89306';          BINARY_URL='https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20.0.2%2B9/OpenJDK20U-jdk_x64_alpine-linux_hotspot_20.0.2_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Thu, 28 Sep 2023 23:26:41 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Thu, 28 Sep 2023 23:26:41 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Thu, 28 Sep 2023 23:26:41 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Thu, 28 Sep 2023 23:26:41 GMT
CMD ["jshell"]
# Fri, 29 Sep 2023 03:51:48 GMT
CMD ["gradle"]
# Fri, 29 Sep 2023 03:51:48 GMT
ENV GRADLE_HOME=/opt/gradle
# Fri, 29 Sep 2023 03:51:49 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && addgroup --system --gid 1000 gradle     && adduser --system --ingroup gradle --uid 1000 --shell /bin/ash gradle     && mkdir /home/gradle/.gradle     && chown -R gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Fri, 29 Sep 2023 03:51:49 GMT
VOLUME [/home/gradle/.gradle]
# Fri, 29 Sep 2023 03:51:49 GMT
WORKDIR /home/gradle
# Fri, 29 Sep 2023 03:51:52 GMT
RUN set -o errexit -o nounset     && echo "Installing VCSes"     && apk add --no-cache       git       git-lfs       mercurial       subversion         && echo "Testing VCSes"     && which git     && which git-lfs     && which hg     && which svn
# Fri, 29 Sep 2023 03:51:52 GMT
ENV GRADLE_VERSION=8.3
# Fri, 29 Sep 2023 03:51:52 GMT
ARG GRADLE_DOWNLOAD_SHA256=591855b517fc635b9e04de1d05d5e76ada3f89f5fc76f87978d1b245b4f69225
# Fri, 29 Sep 2023 03:51:57 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=591855b517fc635b9e04de1d05d5e76ada3f89f5fc76f87978d1b245b4f69225
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking Gradle download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum -c -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln -s "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle
# Fri, 29 Sep 2023 03:51:57 GMT
USER gradle
# Fri, 29 Sep 2023 03:51:58 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=591855b517fc635b9e04de1d05d5e76ada3f89f5fc76f87978d1b245b4f69225
RUN set -o errexit -o nounset     && echo "Testing Gradle installation"     && gradle --version
# Fri, 29 Sep 2023 03:51:59 GMT
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
	-	`sha256:2d4780bd88e540ffc3aff06007363d67ee5849f55861ee9c03d071f8878b194e`  
		Last Modified: Thu, 28 Sep 2023 23:30:46 GMT  
		Size: 152.9 MB (152930846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd951bcdd02682030bc58f966174743a3cab42dee968ef682f2166c1f4215de7`  
		Last Modified: Thu, 28 Sep 2023 23:30:31 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e76b0f81ae3a0cca78c8906b0bea646fac04c6b7abfcf3349bca0fb3532c2975`  
		Last Modified: Thu, 28 Sep 2023 23:30:31 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302903d5b5925d30d1c10d248f9a44892da0978cfd43b3e666ec4103e2a39b5e`  
		Last Modified: Fri, 29 Sep 2023 03:56:24 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b92449f2d4c1e2584dcbdc08a27b356d9924e7ea44d90a0d1a1ddf27ab3de4f`  
		Last Modified: Fri, 29 Sep 2023 03:56:29 GMT  
		Size: 35.0 MB (35031121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2ac8db1db45b2aaf5f52517de98841eaf90135c574e03a8be37ce886dcfc5b`  
		Last Modified: Fri, 29 Sep 2023 03:56:31 GMT  
		Size: 130.7 MB (130666921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68cbf9490bfe85a570f12bd94554b7120ef253ffe40daef8e1de0eb6834d836e`  
		Last Modified: Fri, 29 Sep 2023 03:56:24 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
