## `maven:3-eclipse-temurin-11-alpine`

```console
$ docker pull maven@sha256:5f756e0d31238f82768c5c7b46d0b995cd844f637ac60fd016fcbf4517dcd84f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `maven:3-eclipse-temurin-11-alpine` - linux; amd64

```console
$ docker pull maven@sha256:5b8c99a7773f90a194cdeede5573578f60d958b6a72f9f086caf661aa13e3eef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.6 MB (207630715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba94c172f5eecc9b02f42f7df5912c40452b45a02ce4f462c114564c1bda0a5f`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Thu, 13 Jan 2022 17:19:44 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 13 Jan 2022 17:19:46 GMT
RUN apk add --no-cache tzdata musl-locales musl-locales-lang     && rm -rf /var/cache/apk/*
# Mon, 07 Mar 2022 19:26:29 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1
# Mon, 07 Mar 2022 19:26:54 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='99e13a167ac27fac3dbfcc394a024fd9f4d84d24734ad5c250f97215d496ee36';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_alpine-linux_hotspot_11.0.14.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p /opt/java/openjdk; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory /opt/java/openjdk 	      --strip-components 1 	      --no-same-owner 	  ;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 07 Mar 2022 19:26:55 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Mar 2022 19:26:56 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Mon, 07 Mar 2022 19:26:56 GMT
CMD ["jshell"]
# Mon, 07 Mar 2022 20:14:03 GMT
RUN apk add --no-cache curl tar bash procps
# Mon, 07 Mar 2022 20:14:03 GMT
ARG MAVEN_VERSION=3.8.4
# Mon, 07 Mar 2022 20:14:03 GMT
ARG USER_HOME_DIR=/root
# Mon, 07 Mar 2022 20:14:03 GMT
ARG SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8
# Mon, 07 Mar 2022 20:14:03 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries
# Mon, 07 Mar 2022 20:14:05 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Mon, 07 Mar 2022 20:14:05 GMT
ENV MAVEN_HOME=/usr/share/maven
# Mon, 07 Mar 2022 20:14:05 GMT
ENV MAVEN_CONFIG=/root/.m2
# Mon, 07 Mar 2022 20:14:05 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Mon, 07 Mar 2022 20:14:06 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Mon, 07 Mar 2022 20:14:06 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Mon, 07 Mar 2022 20:14:06 GMT
CMD ["mvn"]
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
	-	`sha256:eae7b8c461b80a787226dfdd0673e9fe7036388862ea32248d15f6a14916f8be`  
		Last Modified: Mon, 07 Mar 2022 19:30:49 GMT  
		Size: 192.9 MB (192891714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f337ae9f87446e991566625212477c2cb66e4e5e3d653165ea9727e1c66bace`  
		Last Modified: Mon, 07 Mar 2022 19:30:36 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e43b2fad6e995e8a542de0f22869d5c5adca141ffb24bf9e66b319d68a883536`  
		Last Modified: Mon, 07 Mar 2022 20:17:17 GMT  
		Size: 2.4 MB (2379128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5178defc2325a4d30c961ab844b81c07701b897b887876f2f06c3a74b7cf4a2`  
		Last Modified: Mon, 07 Mar 2022 20:17:18 GMT  
		Size: 9.1 MB (9109813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3420067d4371728c9846bf9d60f0ea3222535c36f936cf9032e0ae1b88ed7d12`  
		Last Modified: Mon, 07 Mar 2022 20:17:17 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb3c11a68139205288fd1709e439cf818d4fb2c6f0ecc4015419b3bb2cdd451`  
		Last Modified: Mon, 07 Mar 2022 20:17:17 GMT  
		Size: 355.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
