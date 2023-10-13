## `gradle:8-jdk17-graal`

```console
$ docker pull gradle@sha256:655b7545507658523d47d4877123e5a9ecb36e925d7317b6685fdb9750b4c096
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gradle:8-jdk17-graal` - linux; amd64

```console
$ docker pull gradle@sha256:42fd4f2ab61a82febc10da37bb9c10364ca3ed4936f4e7df38cd6c8a69952ba0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **578.8 MB (578762793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:818ca0e5a1dc1946aec8a19608409f4340f180a92777a71d0efee484319c5233`
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
# Fri, 13 Oct 2023 06:06:03 GMT
CMD ["gradle"]
# Fri, 13 Oct 2023 06:06:03 GMT
ENV GRADLE_HOME=/opt/gradle
# Fri, 13 Oct 2023 06:06:04 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Fri, 13 Oct 2023 06:06:04 GMT
VOLUME [/home/gradle/.gradle]
# Fri, 13 Oct 2023 06:06:04 GMT
WORKDIR /home/gradle
# Fri, 13 Oct 2023 06:06:41 GMT
RUN set -o errexit -o nounset     && export DEBIAN_FRONTEND=noninteractive     && apt-get update     && apt-get install --yes --no-install-recommends         binutils         ca-certificates         curl         fontconfig         locales         p11-kit         tzdata         unzip         wget                 gcc         libc-dev         libz-dev         zlib1g-dev                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Fri, 13 Oct 2023 06:06:42 GMT
ENV JAVA_HOME=/opt/java/graalvm
# Fri, 13 Oct 2023 06:06:43 GMT
ENV JAVA_VERSION=17.0.8
# Fri, 13 Oct 2023 06:06:58 GMT
RUN set -o errexit -o nounset     && mkdir /opt/java         && echo "Downloading GraalVM"     && GRAALVM_DOWNLOAD_SHA256=1dffdf5c7cc5bf38558e9f093eef6a14072a6dff0be3a9906208b37b53ecc009     && ARCHITECTURE=$(dpkg --print-architecture)     && if [ "${ARCHITECTURE}" = "amd64" ]; then GRAALVM_ARCHITECTURE=linux-x64; fi     && if [ "${ARCHITECTURE}" = "arm64" ]; then GRAALVM_ARCHITECTURE=linux-aarch64; fi     && GRAALVM_PKG=https://github.com/graalvm/graalvm-ce-builds/releases/download/jdk-${JAVA_VERSION}/graalvm-community-jdk-${JAVA_VERSION}_${GRAALVM_ARCHITECTURE}_bin.tar.gz     && wget --no-verbose --output-document=graalvm.tar.gz "${GRAALVM_PKG}"         && echo "Checking GraalVM download hash"     && echo "${GRAALVM_DOWNLOAD_SHA256} *graalvm.tar.gz" | sha256sum --check -         && echo "Installing GraalVM"     && tar --extract --gunzip --file graalvm.tar.gz     && rm graalvm.tar.gz     && mv graalvm-* "${JAVA_HOME}"     && for bin in "$JAVA_HOME/bin/"*; do         base="$(basename "$bin")";         [ ! -e "/usr/bin/$base" ];         update-alternatives --install "/usr/bin/${base}" "${base}" "${bin}" 1;     done         && echo "Testing GraalVM installation"     && java --version     && javac --version     && gu --version     && native-image --version
# Fri, 13 Oct 2023 06:07:00 GMT
ENV GRADLE_VERSION=8.4
# Fri, 13 Oct 2023 06:07:00 GMT
ARG GRADLE_DOWNLOAD_SHA256=3e1af3ae886920c3ac87f7a91f816c0c7c436f276a6eefdb3da152100fef72ae
# Fri, 13 Oct 2023 06:07:04 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=3e1af3ae886920c3ac87f7a91f816c0c7c436f276a6eefdb3da152100fef72ae
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking Gradle download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle
# Fri, 13 Oct 2023 06:07:04 GMT
USER gradle
# Fri, 13 Oct 2023 06:07:05 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=3e1af3ae886920c3ac87f7a91f816c0c7c436f276a6eefdb3da152100fef72ae
RUN set -o errexit -o nounset     && echo "Testing Gradle installation"     && gradle --version
# Fri, 13 Oct 2023 06:07:05 GMT
USER root
```

-	Layers:
	-	`sha256:43f89b94cd7df92a2f7e565b8fb1b7f502eff2cd225508cbd7ea2d36a9a3a601`  
		Last Modified: Thu, 05 Oct 2023 08:42:10 GMT  
		Size: 30.4 MB (30439111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b87f8379caa0c66ee56c57c6325cf7ae7cbf937e479e9328734bf67724dc8ad`  
		Last Modified: Fri, 13 Oct 2023 06:14:19 GMT  
		Size: 4.4 KB (4360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b613d28ccd16ad0c8979a793bd2b1e662e8915b6fd5e9fad4bd2933eef7246a1`  
		Last Modified: Fri, 13 Oct 2023 06:14:37 GMT  
		Size: 126.4 MB (126408966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b90abde0c1da3dc8b5b637b9bae844401d38c95b5ec69217bfc78bbfa7744845`  
		Last Modified: Fri, 13 Oct 2023 06:14:43 GMT  
		Size: 290.9 MB (290900461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d653df8601dbfe74848de0e2623f6e9fb6793b3c08e1394ea6c4b113618c65a`  
		Last Modified: Fri, 13 Oct 2023 06:14:27 GMT  
		Size: 131.0 MB (131009728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd8649e85c516c89bde5da39a39a3bf20933ae4cb1ad4e4122938ef71eb7dd7`  
		Last Modified: Fri, 13 Oct 2023 06:14:19 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
