## `gradle:jdk-graal`

```console
$ docker pull gradle@sha256:1021dbecd0940d97a9d1d7badf9a5af14e4e760ee0d1d19030ae302d11c0b830
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gradle:jdk-graal` - linux; amd64

```console
$ docker pull gradle@sha256:20c9c9555890ce27ff8e0a0d1fe8eb440097f29183567e74a110ea0624c24087
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **576.5 MB (576485002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5e4eed24da7249831894b6ca8e2ef78aae1dfe1fa0a881e81543b14e17af759`
-	Default Command: `["gradle"]`

```dockerfile
# Fri, 04 Aug 2023 04:52:57 GMT
ARG RELEASE
# Fri, 04 Aug 2023 04:52:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 04:52:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 04:52:58 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 04:52:59 GMT
ADD file:bb1fa1d9d012ae826908afdce8c9fa2feebf221b2ab032e1535255905144411a in / 
# Fri, 04 Aug 2023 04:53:00 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 15:31:46 GMT
CMD ["gradle"]
# Wed, 16 Aug 2023 15:31:46 GMT
ENV GRADLE_HOME=/opt/gradle
# Wed, 16 Aug 2023 15:31:46 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Wed, 16 Aug 2023 15:31:47 GMT
VOLUME [/home/gradle/.gradle]
# Wed, 16 Aug 2023 15:31:47 GMT
WORKDIR /home/gradle
# Wed, 16 Aug 2023 15:33:15 GMT
RUN set -o errexit -o nounset     && export DEBIAN_FRONTEND=noninteractive     && apt-get update     && apt-get install --yes --no-install-recommends         binutils         ca-certificates         curl         fontconfig         locales         p11-kit         tzdata         unzip         wget                 gcc         libc-dev         libz-dev         zlib1g-dev                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Wed, 16 Aug 2023 15:33:16 GMT
ENV JAVA_HOME=/opt/java/graalvm
# Wed, 16 Aug 2023 15:33:32 GMT
RUN set -o errexit -o nounset     && mkdir /opt/java         && echo "Downloading GraalVM"     && JDK_VERSION=17.0.8     && GRAALVM_DOWNLOAD_SHA256=1dffdf5c7cc5bf38558e9f093eef6a14072a6dff0be3a9906208b37b53ecc009     && ARCHITECTURE=$(dpkg --print-architecture)     && if [ "${ARCHITECTURE}" = "amd64" ]; then GRAALVM_ARCHITECTURE=linux-x64; fi     && if [ "${ARCHITECTURE}" = "arm64" ]; then GRAALVM_ARCHITECTURE=linux-aarch64; fi     && GRAALVM_PKG=https://github.com/graalvm/graalvm-ce-builds/releases/download/jdk-${JDK_VERSION}/graalvm-community-jdk-${JDK_VERSION}_${GRAALVM_ARCHITECTURE}_bin.tar.gz     && wget --no-verbose --output-document=graalvm.tar.gz "${GRAALVM_PKG}"         && echo "Checking GraalVM download hash"     && echo "${GRAALVM_DOWNLOAD_SHA256} *graalvm.tar.gz" | sha256sum --check -         && echo "Installing GraalVM"     && tar --extract --gunzip --file graalvm.tar.gz     && rm graalvm.tar.gz     && mv graalvm-* "${JAVA_HOME}"     && for bin in "$JAVA_HOME/bin/"*; do         base="$(basename "$bin")";         [ ! -e "/usr/bin/$base" ];         update-alternatives --install "/usr/bin/${base}" "${base}" "${bin}" 1;     done         && echo "Testing GraalVM installation"     && java --version     && javac --version     && gu --version     && native-image --version
# Wed, 16 Aug 2023 15:33:33 GMT
ENV GRADLE_VERSION=8.2.1
# Wed, 16 Aug 2023 15:33:33 GMT
ARG GRADLE_DOWNLOAD_SHA256=03ec176d388f2aa99defcadc3ac6adf8dd2bce5145a129659537c0874dea5ad1
# Wed, 16 Aug 2023 15:33:38 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=03ec176d388f2aa99defcadc3ac6adf8dd2bce5145a129659537c0874dea5ad1
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking Gradle download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version         && chown --recursive gradle:gradle /home/gradle
```

-	Layers:
	-	`sha256:99de9192b4afd13ed65aeae58d55b38e5231eb97a743921357b7d5b4c0c903c4`  
		Last Modified: Fri, 04 Aug 2023 09:25:19 GMT  
		Size: 30.4 MB (30437960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c266d75c0657390803a4e616451dbd059334958f1f3f58c33477ffa3d875aefd`  
		Last Modified: Wed, 16 Aug 2023 15:36:32 GMT  
		Size: 4.4 KB (4360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc945d064d32f0b3de9767a573cfb9d14847950543d9424ea3984105fd82617`  
		Last Modified: Wed, 16 Aug 2023 15:36:50 GMT  
		Size: 126.4 MB (126413835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b772fb201a7d065541ca4037090eb24e1d0a3a3b13e6e7b664d710466f1c658a`  
		Last Modified: Wed, 16 Aug 2023 15:37:02 GMT  
		Size: 290.9 MB (290900303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9108aa526a4e9d1310eaecf21da4f5bdfbb3eb2591b46ec92e2f479267fc235`  
		Last Modified: Wed, 16 Aug 2023 15:36:39 GMT  
		Size: 128.7 MB (128728544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
