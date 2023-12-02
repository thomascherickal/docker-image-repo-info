## `gradle:jdk21-graal-jammy`

```console
$ docker pull gradle@sha256:fa3967eaaf94f5e259c0e0931bd508499ccb1dd0ac7451252e2b17f94f5e747c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gradle:jdk21-graal-jammy` - linux; amd64

```console
$ docker pull gradle@sha256:51fa5fa31e2a0f428b5f3ca174d9198282ce0919e04255c325461453694915a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **578.8 MB (578786706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0479e7fe772d0153bb73d7220829f90ef842c16bd77cb31a7cc63ae5c218967e`
-	Default Command: `["gradle"]`

```dockerfile
# Fri, 01 Dec 2023 07:49:48 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:49:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:49:50 GMT
ADD file:36d444e2cede3abe58191dcf28890b874c0908f5259bf7e8855338555701c4c5 in / 
# Fri, 01 Dec 2023 07:49:50 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:14:19 GMT
CMD ["gradle"]
# Sat, 02 Dec 2023 06:14:19 GMT
ENV GRADLE_HOME=/opt/gradle
# Sat, 02 Dec 2023 06:14:19 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Sat, 02 Dec 2023 06:14:19 GMT
VOLUME [/home/gradle/.gradle]
# Sat, 02 Dec 2023 06:14:20 GMT
WORKDIR /home/gradle
# Sat, 02 Dec 2023 06:14:47 GMT
RUN set -o errexit -o nounset     && export DEBIAN_FRONTEND=noninteractive     && apt-get update     && apt-get install --yes --no-install-recommends         binutils         ca-certificates         curl         fontconfig         locales         p11-kit         tzdata         unzip         wget                 gcc         libc-dev         libz-dev         zlib1g-dev                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Sat, 02 Dec 2023 06:14:48 GMT
ENV JAVA_HOME=/opt/java/graalvm
# Sat, 02 Dec 2023 06:15:48 GMT
ENV JAVA_VERSION=21.0.1
# Sat, 02 Dec 2023 06:16:01 GMT
RUN set -o errexit -o nounset     && mkdir /opt/java         && echo "Downloading GraalVM"     && GRAALVM_DOWNLOAD_SHA256=5283EE48A61633F59A49ECDF0EF0AB4C5A8B006C16CE95209DF740BD2AEE73BF     && ARCHITECTURE=$(dpkg --print-architecture)     && if [ "${ARCHITECTURE}" = "amd64" ]; then GRAALVM_ARCHITECTURE=linux-x64; fi     && if [ "${ARCHITECTURE}" = "arm64" ]; then GRAALVM_ARCHITECTURE=linux-aarch64; fi     && GRAALVM_PKG=https://github.com/graalvm/graalvm-ce-builds/releases/download/jdk-${JAVA_VERSION}/graalvm-community-jdk-${JAVA_VERSION}_${GRAALVM_ARCHITECTURE}_bin.tar.gz     && wget --no-verbose --output-document=graalvm.tar.gz "${GRAALVM_PKG}"         && echo "Checking GraalVM download hash"     && echo "${GRAALVM_DOWNLOAD_SHA256} *graalvm.tar.gz" | sha256sum --check -         && echo "Installing GraalVM"     && tar --extract --gunzip --file graalvm.tar.gz     && rm graalvm.tar.gz     && mv graalvm-* "${JAVA_HOME}"     && for bin in "$JAVA_HOME/bin/"*; do         base="$(basename "$bin")";         [ ! -e "/usr/bin/$base" ];         update-alternatives --install "/usr/bin/${base}" "${base}" "${bin}" 1;     done         && echo "Testing GraalVM installation"     && java --version     && javac --version     && native-image --version
# Sat, 02 Dec 2023 06:16:02 GMT
ENV GRADLE_VERSION=8.5
# Sat, 02 Dec 2023 06:16:03 GMT
ARG GRADLE_DOWNLOAD_SHA256=9d926787066a081739e8200858338b4a69e837c3a821a33aca9db09dd4a41026
# Sat, 02 Dec 2023 06:16:07 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=9d926787066a081739e8200858338b4a69e837c3a821a33aca9db09dd4a41026
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking Gradle download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle
# Sat, 02 Dec 2023 06:16:07 GMT
USER gradle
# Sat, 02 Dec 2023 06:16:08 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=9d926787066a081739e8200858338b4a69e837c3a821a33aca9db09dd4a41026
RUN set -o errexit -o nounset     && echo "Testing Gradle installation"     && gradle --version
# Sat, 02 Dec 2023 06:16:08 GMT
USER root
```

-	Layers:
	-	`sha256:cbe3537751ce03ea42788c2fbe2d5d336180dc2e20472c8cdba8b3224191d101`  
		Last Modified: Wed, 29 Nov 2023 19:24:54 GMT  
		Size: 30.4 MB (30446322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eda49c1924a0297521fa09b961e050daa00fc1ac3133d31a361e8fea492354e`  
		Last Modified: Sat, 02 Dec 2023 06:23:01 GMT  
		Size: 4.4 KB (4360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1015220c27d7cebf6fad6f5692c7c9614907f50dbac4c54b4aa1e9a9e6009c3f`  
		Last Modified: Sat, 02 Dec 2023 06:23:18 GMT  
		Size: 126.4 MB (126406534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce9be579fe2fa93cfa66a906751489cfacd4a294194f7850036c6a633d4853e`  
		Last Modified: Sat, 02 Dec 2023 06:25:58 GMT  
		Size: 289.4 MB (289384630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef3296545efc41368675daf06dcef04d7fa8d493742d3068c90cd8a61265547`  
		Last Modified: Sat, 02 Dec 2023 06:25:42 GMT  
		Size: 132.5 MB (132544692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7918bf07aa0c7160251be5a42bef1b8de047d3f2c4535929a5c07f060803213`  
		Last Modified: Sat, 02 Dec 2023 06:25:36 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
