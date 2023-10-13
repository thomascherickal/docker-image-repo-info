## `gradle:8-jdk11-jammy`

```console
$ docker pull gradle@sha256:6bf96c9c4d51a9901be53ab057841abeec3a4bbbf4416d6844f5a30273022b84
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `gradle:8-jdk11-jammy` - linux; amd64

```console
$ docker pull gradle@sha256:99aff85a100b60552c5a1ef7ccddc9aa38680ab85b0e45a8bb7ecbfc0ec62396
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **370.7 MB (370745492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe0a940809c70d87ccf38440cdfa769f21a5597423b4d3918ff3b19753974d9f`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`
-	Default Command: `["gradle"]`

```dockerfile
# Thu, 05 Oct 2023 07:33:30 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:33:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:33:32 GMT
ADD file:63d5ab3ef0aab308c0e71cb67292c5467f60deafa9b0418cbb220affcd078444 in / 
# Thu, 05 Oct 2023 07:33:32 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 05:51:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 13 Oct 2023 05:51:05 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 05:51:05 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 13 Oct 2023 05:51:27 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 05:52:21 GMT
ENV JAVA_VERSION=jdk-11.0.20.1+1
# Fri, 13 Oct 2023 05:52:30 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='69d39682c4a2fac294a9eaacbf62c26d3c8a2f9123f1b5d287498a5472c6b672';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        armhf|arm)          ESUM='e83674aee238ebb5f359b9395b3c5e3fad5b645846095494662802d2f0fd01c9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_arm_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='b806f4bb526161bf9b2ffb37be4e1b77f56b4e726dc4d52c7902130a79e7d710';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='a7efbe804a4616d38b6ac0def40cd9feacc04aee2bb89132191f4d33fc0a7c1e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='398a64bff002f0e3b0c01ecd24a1a32c83cb72a5255344219e9757d4ddd9f857';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_x64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 13 Oct 2023 05:52:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 13 Oct 2023 05:52:32 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Fri, 13 Oct 2023 05:52:32 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Fri, 13 Oct 2023 05:52:33 GMT
CMD ["jshell"]
# Fri, 13 Oct 2023 06:04:03 GMT
CMD ["gradle"]
# Fri, 13 Oct 2023 06:04:03 GMT
ENV GRADLE_HOME=/opt/gradle
# Fri, 13 Oct 2023 06:04:04 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Fri, 13 Oct 2023 06:04:04 GMT
VOLUME [/home/gradle/.gradle]
# Fri, 13 Oct 2023 06:04:04 GMT
WORKDIR /home/gradle
# Fri, 13 Oct 2023 06:04:19 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Fri, 13 Oct 2023 06:04:20 GMT
ENV GRADLE_VERSION=8.4
# Fri, 13 Oct 2023 06:04:20 GMT
ARG GRADLE_DOWNLOAD_SHA256=3e1af3ae886920c3ac87f7a91f816c0c7c436f276a6eefdb3da152100fef72ae
# Fri, 13 Oct 2023 06:04:24 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=3e1af3ae886920c3ac87f7a91f816c0c7c436f276a6eefdb3da152100fef72ae
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking Gradle download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle
# Fri, 13 Oct 2023 06:04:25 GMT
USER gradle
# Fri, 13 Oct 2023 06:04:26 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=3e1af3ae886920c3ac87f7a91f816c0c7c436f276a6eefdb3da152100fef72ae
RUN set -o errexit -o nounset     && echo "Testing Gradle installation"     && gradle --version
# Fri, 13 Oct 2023 06:04:26 GMT
USER root
```

-	Layers:
	-	`sha256:43f89b94cd7df92a2f7e565b8fb1b7f502eff2cd225508cbd7ea2d36a9a3a601`  
		Last Modified: Thu, 05 Oct 2023 08:42:10 GMT  
		Size: 30.4 MB (30439111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39769250f2be0be25f38285d2996eb4dcbdfaddd7ad6c025b98e2fc2d955a973`  
		Last Modified: Fri, 13 Oct 2023 05:56:41 GMT  
		Size: 12.9 MB (12902386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d78bd96cc6f3e32688badf91f63c46e109ee5d0b1f6089aa9c94cdc502835ac`  
		Last Modified: Fri, 13 Oct 2023 05:58:08 GMT  
		Size: 144.8 MB (144836315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:609b859ad36b156f56ea6def0bc711287fa37701f140011a062fffe1e9f5c076`  
		Last Modified: Fri, 13 Oct 2023 05:57:57 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:442b4ebcd69d88fb1111ee21247fca359f46b4a4c455e6ce4ff6a05974ff72da`  
		Last Modified: Fri, 13 Oct 2023 05:57:57 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782bd958d75285e9f9a945b61f3b9a73d46dba24a06edf4025ca684609880bca`  
		Last Modified: Fri, 13 Oct 2023 06:11:37 GMT  
		Size: 4.4 KB (4361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5882c1e0915bbfdbbdaaeeb1ea20d41b7a198e1bcd3e46117f0c033928ebb205`  
		Last Modified: Fri, 13 Oct 2023 06:11:46 GMT  
		Size: 51.6 MB (51552494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de457cc33c1d2608bce6731165ff82930ef5829bd011fa18c99540d3157f089`  
		Last Modified: Fri, 13 Oct 2023 06:11:45 GMT  
		Size: 131.0 MB (131009746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b6b60d5c49352a1a021788dfdd420c464cd4a9c2f7422932cf25241866997d`  
		Last Modified: Fri, 13 Oct 2023 06:11:37 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:8-jdk11-jammy` - linux; arm variant v7

```console
$ docker pull gradle@sha256:383fef51d87797fcb358b4a308b5d0bfadcdb12d81296af7c0f37830416b88a2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.3 MB (362307522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57f490f9452a5a300737b634d599a662bdae1cfe46bc927b7f5dcf47835b1fab`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`
-	Default Command: `["gradle"]`

```dockerfile
# Thu, 05 Oct 2023 07:34:56 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:34:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:34:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:34:56 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:35:01 GMT
ADD file:4b9d52f97ed5796b14772a84c1e7213402430d32312d15ae04a2dcc9fc485a52 in / 
# Thu, 05 Oct 2023 07:35:02 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 01:15:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 13 Oct 2023 01:15:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 01:15:56 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 13 Oct 2023 01:16:20 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 01:17:22 GMT
ENV JAVA_VERSION=jdk-11.0.20.1+1
# Fri, 13 Oct 2023 01:17:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='69d39682c4a2fac294a9eaacbf62c26d3c8a2f9123f1b5d287498a5472c6b672';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        armhf|arm)          ESUM='e83674aee238ebb5f359b9395b3c5e3fad5b645846095494662802d2f0fd01c9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_arm_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='b806f4bb526161bf9b2ffb37be4e1b77f56b4e726dc4d52c7902130a79e7d710';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='a7efbe804a4616d38b6ac0def40cd9feacc04aee2bb89132191f4d33fc0a7c1e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='398a64bff002f0e3b0c01ecd24a1a32c83cb72a5255344219e9757d4ddd9f857';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_x64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 13 Oct 2023 01:17:36 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 13 Oct 2023 01:17:37 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Fri, 13 Oct 2023 01:17:37 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Fri, 13 Oct 2023 01:17:37 GMT
CMD ["jshell"]
# Fri, 13 Oct 2023 04:05:47 GMT
CMD ["gradle"]
# Fri, 13 Oct 2023 04:05:47 GMT
ENV GRADLE_HOME=/opt/gradle
# Fri, 13 Oct 2023 04:05:47 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Fri, 13 Oct 2023 04:05:47 GMT
VOLUME [/home/gradle/.gradle]
# Fri, 13 Oct 2023 04:05:47 GMT
WORKDIR /home/gradle
# Fri, 13 Oct 2023 04:06:04 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Fri, 13 Oct 2023 04:06:04 GMT
ENV GRADLE_VERSION=8.4
# Fri, 13 Oct 2023 04:06:05 GMT
ARG GRADLE_DOWNLOAD_SHA256=3e1af3ae886920c3ac87f7a91f816c0c7c436f276a6eefdb3da152100fef72ae
# Fri, 13 Oct 2023 04:06:10 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=3e1af3ae886920c3ac87f7a91f816c0c7c436f276a6eefdb3da152100fef72ae
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking Gradle download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle
# Fri, 13 Oct 2023 04:06:11 GMT
USER gradle
# Fri, 13 Oct 2023 04:06:12 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=3e1af3ae886920c3ac87f7a91f816c0c7c436f276a6eefdb3da152100fef72ae
RUN set -o errexit -o nounset     && echo "Testing Gradle installation"     && gradle --version
# Fri, 13 Oct 2023 04:06:12 GMT
USER root
```

-	Layers:
	-	`sha256:c4f28c22de51200ba6a71d2274daa2f71735946524265b3c45752d2cec53dee0`  
		Last Modified: Fri, 06 Oct 2023 02:02:33 GMT  
		Size: 27.5 MB (27513969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d066b62893903fd42aaa8480fcf1a04f9c324fdc1c3818172bd0dc8a51a1b6ed`  
		Last Modified: Fri, 13 Oct 2023 01:20:49 GMT  
		Size: 12.5 MB (12490382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c5c6d8c4b5e5ad3e31ffad35c30a847a6129985fc7e128e90581aa296d13b65`  
		Last Modified: Fri, 13 Oct 2023 01:22:29 GMT  
		Size: 137.4 MB (137402390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2371d4a12d6ba41ec9448eab3684497bc0158dfd5a5dde59d0b7766b6b7741c`  
		Last Modified: Fri, 13 Oct 2023 01:22:12 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0366bf09b6797a15e82fed71dc27332341a92fabc89a64475fedb2ec23aafce6`  
		Last Modified: Fri, 13 Oct 2023 01:22:12 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84dfc54033a4cf08c2faabc3bbd390b420cd719ba06d876e61172733938a7d73`  
		Last Modified: Fri, 13 Oct 2023 04:11:51 GMT  
		Size: 4.4 KB (4351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c595d4413149df5a378a6157cb7825e63a1e323cf535d12834ca0f5cae7635`  
		Last Modified: Fri, 13 Oct 2023 04:12:00 GMT  
		Size: 53.9 MB (53885614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b23359e8f685082a0f24e4f0d07ee80851045aacdea8eeb00c2fa167e4df0d30`  
		Last Modified: Fri, 13 Oct 2023 04:12:00 GMT  
		Size: 131.0 MB (131009738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec203ce11356b3b195c6d792fdaaa0f52b904497f10981e888fcb8cb66f2ea9`  
		Last Modified: Fri, 13 Oct 2023 04:11:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:8-jdk11-jammy` - linux; arm64 variant v8

```console
$ docker pull gradle@sha256:16af67ed5db85372c7ecb896d108216a17fd186d07fc5d21b4c83ed6a618e1ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **365.0 MB (364951329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a26974bbf48afd3ddadc1d039b7f969ac2b5a0f72203bf2300c3ace6320f2c8`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`
-	Default Command: `["gradle"]`

```dockerfile
# Thu, 05 Oct 2023 07:32:20 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:32:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:32:22 GMT
ADD file:f8594e26831508c318e42c8dfd9942041031087b8de1bf3fec11fd75b8b30fd4 in / 
# Thu, 05 Oct 2023 07:32:22 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 02:46:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 13 Oct 2023 02:46:31 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 02:46:31 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 13 Oct 2023 02:46:48 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 02:47:30 GMT
ENV JAVA_VERSION=jdk-11.0.20.1+1
# Fri, 13 Oct 2023 02:47:36 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='69d39682c4a2fac294a9eaacbf62c26d3c8a2f9123f1b5d287498a5472c6b672';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        armhf|arm)          ESUM='e83674aee238ebb5f359b9395b3c5e3fad5b645846095494662802d2f0fd01c9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_arm_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='b806f4bb526161bf9b2ffb37be4e1b77f56b4e726dc4d52c7902130a79e7d710';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='a7efbe804a4616d38b6ac0def40cd9feacc04aee2bb89132191f4d33fc0a7c1e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='398a64bff002f0e3b0c01ecd24a1a32c83cb72a5255344219e9757d4ddd9f857';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_x64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 13 Oct 2023 02:47:39 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 13 Oct 2023 02:47:39 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Fri, 13 Oct 2023 02:47:39 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Fri, 13 Oct 2023 02:47:39 GMT
CMD ["jshell"]
# Fri, 13 Oct 2023 03:37:47 GMT
CMD ["gradle"]
# Fri, 13 Oct 2023 03:37:47 GMT
ENV GRADLE_HOME=/opt/gradle
# Fri, 13 Oct 2023 03:37:48 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Fri, 13 Oct 2023 03:37:48 GMT
VOLUME [/home/gradle/.gradle]
# Fri, 13 Oct 2023 03:37:48 GMT
WORKDIR /home/gradle
# Fri, 13 Oct 2023 03:38:01 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Fri, 13 Oct 2023 03:38:01 GMT
ENV GRADLE_VERSION=8.4
# Fri, 13 Oct 2023 03:38:01 GMT
ARG GRADLE_DOWNLOAD_SHA256=3e1af3ae886920c3ac87f7a91f816c0c7c436f276a6eefdb3da152100fef72ae
# Fri, 13 Oct 2023 03:38:05 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=3e1af3ae886920c3ac87f7a91f816c0c7c436f276a6eefdb3da152100fef72ae
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking Gradle download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle
# Fri, 13 Oct 2023 03:38:06 GMT
USER gradle
# Fri, 13 Oct 2023 03:38:07 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=3e1af3ae886920c3ac87f7a91f816c0c7c436f276a6eefdb3da152100fef72ae
RUN set -o errexit -o nounset     && echo "Testing Gradle installation"     && gradle --version
# Fri, 13 Oct 2023 03:38:07 GMT
USER root
```

-	Layers:
	-	`sha256:895d322e8e5957c04af3ab7b3431f2a562182d34167c6e159e02044150a66967`  
		Last Modified: Thu, 05 Oct 2023 08:57:30 GMT  
		Size: 28.4 MB (28391939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b0137fa974e870bf950b9443cae72cbb22adb398877f52eca3717d3fa96a8d4`  
		Last Modified: Fri, 13 Oct 2023 02:50:57 GMT  
		Size: 12.8 MB (12843553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41290b615d3ecf8c775044af35f17b669d335fcec3839ea8f4461c435efece7d`  
		Last Modified: Fri, 13 Oct 2023 02:52:12 GMT  
		Size: 141.6 MB (141581327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf265af309fb880416333e2dc3ace79f2ce8e56eb48390a0f0cad714e85c23d`  
		Last Modified: Fri, 13 Oct 2023 02:52:03 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cfcedb6f232dce18738a1354fc5768ee3ec392515175c86ecefbd9e3850ef42`  
		Last Modified: Fri, 13 Oct 2023 02:52:03 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26dec10913237db49387cb373b7e41a45cbbb7001e1f2cac362b6320198adbb`  
		Last Modified: Fri, 13 Oct 2023 03:44:05 GMT  
		Size: 4.4 KB (4367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c5485a6819b03dbf7163c5c3aa2e038240ddd2d9dc2bd3685b48137b54bf46`  
		Last Modified: Fri, 13 Oct 2023 03:44:11 GMT  
		Size: 51.1 MB (51119335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f975eda57ebd03b0ae3672fd6786b21fafb4d9d8ce0f3f49a180f353c91c0a4e`  
		Last Modified: Fri, 13 Oct 2023 03:44:11 GMT  
		Size: 131.0 MB (131009728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02577f60969256b8f98dc78c3ec0c17fef79637176fe6980a0af7747558aa257`  
		Last Modified: Fri, 13 Oct 2023 03:44:05 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:8-jdk11-jammy` - linux; ppc64le

```console
$ docker pull gradle@sha256:c1bcf9cc3030a234291e9beebb0d03d4591b77c58145701225b2c916ef768ede
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **368.2 MB (368176329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adcd48d17a0693b388d5ac3cb3c65142cfefc452fd8bb0beb9ddc1eae63c4de0`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`
-	Default Command: `["gradle"]`

```dockerfile
# Mon, 25 Sep 2023 10:20:46 GMT
ARG RELEASE
# Mon, 25 Sep 2023 10:20:46 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 25 Sep 2023 10:20:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 25 Sep 2023 10:20:46 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 25 Sep 2023 10:20:49 GMT
ADD file:4e52928c778d7e98d90ccfcaacd039ae1fdde494dfa310adbe229d7051c30918 in / 
# Mon, 25 Sep 2023 10:20:49 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 08:16:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 03 Oct 2023 08:16:45 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 08:16:46 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 03 Oct 2023 08:17:22 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 08:18:25 GMT
ENV JAVA_VERSION=jdk-11.0.20.1+1
# Tue, 03 Oct 2023 08:18:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='69d39682c4a2fac294a9eaacbf62c26d3c8a2f9123f1b5d287498a5472c6b672';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        armhf|arm)          ESUM='e83674aee238ebb5f359b9395b3c5e3fad5b645846095494662802d2f0fd01c9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_arm_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='b806f4bb526161bf9b2ffb37be4e1b77f56b4e726dc4d52c7902130a79e7d710';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='a7efbe804a4616d38b6ac0def40cd9feacc04aee2bb89132191f4d33fc0a7c1e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='398a64bff002f0e3b0c01ecd24a1a32c83cb72a5255344219e9757d4ddd9f857';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_x64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 03 Oct 2023 08:18:50 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 03 Oct 2023 08:18:50 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Tue, 03 Oct 2023 08:18:50 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Tue, 03 Oct 2023 08:18:51 GMT
CMD ["jshell"]
# Tue, 03 Oct 2023 11:09:51 GMT
CMD ["gradle"]
# Tue, 03 Oct 2023 11:09:51 GMT
ENV GRADLE_HOME=/opt/gradle
# Tue, 03 Oct 2023 11:09:56 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Tue, 03 Oct 2023 11:09:57 GMT
VOLUME [/home/gradle/.gradle]
# Tue, 03 Oct 2023 11:09:58 GMT
WORKDIR /home/gradle
# Tue, 03 Oct 2023 11:11:07 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Fri, 06 Oct 2023 01:29:45 GMT
ENV GRADLE_VERSION=8.4
# Fri, 06 Oct 2023 01:29:45 GMT
ARG GRADLE_DOWNLOAD_SHA256=3e1af3ae886920c3ac87f7a91f816c0c7c436f276a6eefdb3da152100fef72ae
# Fri, 06 Oct 2023 01:29:55 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=3e1af3ae886920c3ac87f7a91f816c0c7c436f276a6eefdb3da152100fef72ae
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking Gradle download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle
# Fri, 06 Oct 2023 01:29:58 GMT
USER gradle
# Fri, 06 Oct 2023 01:30:03 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=3e1af3ae886920c3ac87f7a91f816c0c7c436f276a6eefdb3da152100fef72ae
RUN set -o errexit -o nounset     && echo "Testing Gradle installation"     && gradle --version
# Fri, 06 Oct 2023 01:30:04 GMT
USER root
```

-	Layers:
	-	`sha256:8098558aeb0337452acaa8c74f02401dc8e9bc5a2c048e4c82c013b483a11f11`  
		Last Modified: Tue, 03 Oct 2023 07:57:52 GMT  
		Size: 35.7 MB (35702863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:931c9c8af9e87407323da067bbf3a8b691add055bcd0d602e17cd36b4b0c4cee`  
		Last Modified: Tue, 03 Oct 2023 08:22:20 GMT  
		Size: 13.8 MB (13770245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96bbc961b48057f2617fabf7a8ea5879e914ce27e1c82d52200987b1d285b6cd`  
		Last Modified: Tue, 03 Oct 2023 08:23:13 GMT  
		Size: 132.0 MB (131991917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c8b287cc7cb5b3c9ccdfea6c618e5847be04af6e3605bedb86951851ec1553`  
		Last Modified: Tue, 03 Oct 2023 08:22:54 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9929ad499b81e044b6d5d2e80ef980628f3f872ae43165acb9abf705d14f994f`  
		Last Modified: Tue, 03 Oct 2023 08:22:54 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:301ee492ee5fedd38a39a0c9f3aac9dbdeb9dc841cffa35799130aad8d0ac835`  
		Last Modified: Tue, 03 Oct 2023 11:17:30 GMT  
		Size: 4.4 KB (4365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee3f3ff42147e170fd66f397b24818c5acc1b5be093f65f6da9085fc78cd943`  
		Last Modified: Tue, 03 Oct 2023 11:17:46 GMT  
		Size: 55.7 MB (55696134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4559c3a340883b15a7e35fdde90219e2e3af041600a9f22d4b78465bf2f19d96`  
		Last Modified: Fri, 06 Oct 2023 01:37:05 GMT  
		Size: 131.0 MB (131009726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4645ce32b9ca477c80691ffbf062abdc0787ede9dbe09b10b1ca84e94eeede5`  
		Last Modified: Fri, 06 Oct 2023 01:36:52 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:8-jdk11-jammy` - linux; s390x

```console
$ docker pull gradle@sha256:1aca10261ed6fd3488a10fc1a5a9971579dbd7e8de7580e696f2f67d93cfda61
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.1 MB (349067615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:162b01d0bb99d225430c75fc25c27b4a278f0b73276424c9d08b445925ee4249`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`
-	Default Command: `["gradle"]`

```dockerfile
# Mon, 25 Sep 2023 10:17:26 GMT
ARG RELEASE
# Mon, 25 Sep 2023 10:17:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 25 Sep 2023 10:17:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 25 Sep 2023 10:17:26 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 25 Sep 2023 10:17:28 GMT
ADD file:78683f2464233172a7cd0d6adc4c7d9fb3ef05fa67ca22e6fbaca0325496a536 in / 
# Mon, 25 Sep 2023 10:17:28 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 09:08:41 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 03 Oct 2023 09:08:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 09:08:41 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 03 Oct 2023 09:08:53 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 09:08:55 GMT
ENV JAVA_VERSION=jdk-11.0.20.1+1
# Tue, 03 Oct 2023 09:09:09 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='69d39682c4a2fac294a9eaacbf62c26d3c8a2f9123f1b5d287498a5472c6b672';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        armhf|arm)          ESUM='e83674aee238ebb5f359b9395b3c5e3fad5b645846095494662802d2f0fd01c9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_arm_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='b806f4bb526161bf9b2ffb37be4e1b77f56b4e726dc4d52c7902130a79e7d710';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='a7efbe804a4616d38b6ac0def40cd9feacc04aee2bb89132191f4d33fc0a7c1e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='398a64bff002f0e3b0c01ecd24a1a32c83cb72a5255344219e9757d4ddd9f857';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_x64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 03 Oct 2023 09:09:16 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 03 Oct 2023 09:09:16 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Tue, 03 Oct 2023 09:09:17 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Tue, 03 Oct 2023 09:09:17 GMT
CMD ["jshell"]
# Tue, 03 Oct 2023 11:01:22 GMT
CMD ["gradle"]
# Tue, 03 Oct 2023 11:01:22 GMT
ENV GRADLE_HOME=/opt/gradle
# Tue, 03 Oct 2023 11:01:22 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Tue, 03 Oct 2023 11:01:22 GMT
VOLUME [/home/gradle/.gradle]
# Tue, 03 Oct 2023 11:01:23 GMT
WORKDIR /home/gradle
# Tue, 03 Oct 2023 11:01:55 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Mon, 09 Oct 2023 16:16:15 GMT
ENV GRADLE_VERSION=8.4
# Mon, 09 Oct 2023 16:16:15 GMT
ARG GRADLE_DOWNLOAD_SHA256=3e1af3ae886920c3ac87f7a91f816c0c7c436f276a6eefdb3da152100fef72ae
# Mon, 09 Oct 2023 16:16:25 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=3e1af3ae886920c3ac87f7a91f816c0c7c436f276a6eefdb3da152100fef72ae
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking Gradle download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle
# Mon, 09 Oct 2023 16:16:30 GMT
USER gradle
# Mon, 09 Oct 2023 16:16:32 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=3e1af3ae886920c3ac87f7a91f816c0c7c436f276a6eefdb3da152100fef72ae
RUN set -o errexit -o nounset     && echo "Testing Gradle installation"     && gradle --version
# Mon, 09 Oct 2023 16:16:33 GMT
USER root
```

-	Layers:
	-	`sha256:b6ba488997f9924c9473e547d56b3d4ae74495b1092ca3c613243185ee5d5151`  
		Last Modified: Tue, 03 Oct 2023 08:59:45 GMT  
		Size: 28.7 MB (28651983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6ebbc5199f54e5da3b34aa5983900a17cba52d2381529b95064414261c04f7`  
		Last Modified: Tue, 03 Oct 2023 09:12:09 GMT  
		Size: 13.0 MB (12981189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0520c8e84c9f99925e90d5ca3ddfc084af6a77b6b7bd9d7498a61b0fbe852d01`  
		Last Modified: Tue, 03 Oct 2023 09:12:18 GMT  
		Size: 125.1 MB (125137815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8053a073a19620970b9ea794a222ccbbeab83b011a072c7565f7807fab09a1`  
		Last Modified: Tue, 03 Oct 2023 09:12:07 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426c61158d5f816969ee69ab82556619902f18bd23b4a3f9dabfe1c4f4e7feaf`  
		Last Modified: Tue, 03 Oct 2023 09:12:07 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7c0d27718a12a6f83940811e16c4f471eec674f19831ca4c8243f790052d0e`  
		Last Modified: Tue, 03 Oct 2023 11:07:40 GMT  
		Size: 4.4 KB (4369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:139f6e315d0e178b6445971d782ddead725d476d0d7b41acdd68ab0cf8670f1a`  
		Last Modified: Tue, 03 Oct 2023 11:07:48 GMT  
		Size: 51.3 MB (51281442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252f0002e2032f3d344f0b89fe786aa2b5a915deffd04f53ef15f14a8ccc860f`  
		Last Modified: Mon, 09 Oct 2023 16:21:49 GMT  
		Size: 131.0 MB (131009741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329f72e4a85669432511ce429939d6b016638e18372e92688ffb2078f09a766b`  
		Last Modified: Mon, 09 Oct 2023 16:21:42 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
