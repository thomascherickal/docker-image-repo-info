## `maven:3-openjdk-16`

```console
$ docker pull maven@sha256:181495fc5e12d8be105d4c9f9d212090f786b561707e57b7c59c47a34475c9a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-openjdk-16` - linux; amd64

```console
$ docker pull maven@sha256:a74c553fb9388582050a63f3f37db5dfdf66d51f620b1a8600fa594b7178ca99
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **388.9 MB (388934635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1cba140efcc1b00e00d64f3c536e9c169d3330458bd9519fb3434f54b086b8a`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 15 Sep 2020 21:22:07 GMT
LABEL org.opencontainers.image.authors=Oracle Linux Product Team <ol-ovm-info_ww@oracle.com> org.opencontainers.image.url=https://github.com/oracle/container-images org.opencontainers.image.source=https://github.com/oracle/container-images/tree/dist-amd64/8-slim org.opencontainers.image.vendor=Oracle America, Inc org.opencontainers.image.title=Oracle Linux 8 (slim) org.opencontainers.image.description=Oracle Linux is an open-source       operating system available under the GNU General Public License (GPLv2) and       is suitable for both general purpose or Oracle workloads.
# Wed, 06 Jan 2021 20:21:43 GMT
ADD file:2987f8143a9c4f758731c17e307a6c7ca9e5e1a974df3405a17d2699da7d8351 in / 
# Wed, 06 Jan 2021 20:21:44 GMT
CMD ["/bin/bash"]
# Wed, 06 Jan 2021 20:39:53 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 06 Jan 2021 20:39:53 GMT
ENV LANG=C.UTF-8
# Wed, 06 Jan 2021 20:41:33 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Wed, 06 Jan 2021 20:41:33 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Jan 2021 20:41:33 GMT
ENV JAVA_VERSION=16-ea+30
# Wed, 06 Jan 2021 20:42:07 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/30/GPL/openjdk-16-ea+30_linux-aarch64_bin.tar.gz; 			downloadSha256=82cc271dfc10530a176b89f20ad2bcbc9733b78f39e3997ac54132956ce53ff1; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/30/GPL/openjdk-16-ea+30_linux-x64_bin.tar.gz; 			downloadSha256=01ef449013825308ac144c91fbbbadd9562b084d6e17cd8d428a088386707556; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 06 Jan 2021 20:42:07 GMT
CMD ["jshell"]
# Wed, 06 Jan 2021 21:16:53 GMT
ARG MAVEN_VERSION=3.6.3
# Wed, 06 Jan 2021 21:16:53 GMT
ARG USER_HOME_DIR=/root
# Wed, 06 Jan 2021 21:16:53 GMT
ARG SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0
# Wed, 06 Jan 2021 21:16:53 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries
# Wed, 06 Jan 2021 21:17:20 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN microdnf install findutils git
# Wed, 06 Jan 2021 21:17:23 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 06 Jan 2021 21:17:24 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 06 Jan 2021 21:17:24 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 06 Jan 2021 21:17:24 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 06 Jan 2021 21:17:24 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 06 Jan 2021 21:17:24 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 06 Jan 2021 21:17:25 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:a73adebe9317092fb1f120a1d0d21f460296e9bde7ac683fd452cfc628c528cf`  
		Last Modified: Wed, 06 Jan 2021 20:23:26 GMT  
		Size: 42.1 MB (42069921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01539a440662c3eb557891fa6a645060175a11221504049aa1b23cd50cc3f6fa`  
		Last Modified: Wed, 06 Jan 2021 20:47:24 GMT  
		Size: 13.3 MB (13277651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a362f231ba6e3d4f7192283cb65811335fe5cb82a06caa8a7273182c294f153`  
		Last Modified: Wed, 06 Jan 2021 20:48:41 GMT  
		Size: 184.8 MB (184847441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b3381e5f1938fc1519b7329c8986885906e22502c57b1fd8a6a03f54a62fec3`  
		Last Modified: Wed, 06 Jan 2021 21:20:43 GMT  
		Size: 139.2 MB (139157202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100d07cdce090edb1b28911655b8616c48d6cc3063665d486342f07a599730a6`  
		Last Modified: Wed, 06 Jan 2021 21:20:30 GMT  
		Size: 9.6 MB (9581209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b57381220628fa8f7cc1126365c4c225c9a44bc56f84ebc5e149aa1f43d63ed`  
		Last Modified: Wed, 06 Jan 2021 21:20:29 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58d8e291cb9ce32362bc8a0e8a49a67fa9d9278606e8ff89c3764cb4334a233`  
		Last Modified: Wed, 06 Jan 2021 21:20:29 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-openjdk-16` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:78fbbd4d92d58d3e4af84c9e5504b9824598a521d69b3abdae89157b46d543b6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **361.0 MB (360985606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffb6237f440da3081a5eb06f5140a0a2c0ac27c4bf5e3ae326c08ff4234e7a69`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 15 Sep 2020 20:40:54 GMT
LABEL org.opencontainers.image.authors=Oracle Linux Product Team <ol-ovm-info_ww@oracle.com> org.opencontainers.image.url=https://github.com/oracle/container-images org.opencontainers.image.source=https://github.com/oracle/container-images/tree/dist-arm64v8/8-slim org.opencontainers.image.vendor=Oracle America, Inc org.opencontainers.image.title=Oracle Linux 8 (slim) org.opencontainers.image.description=Oracle Linux is an open-source       operating system available under the GNU General Public License (GPLv2) and       is suitable for both general purpose or Oracle workloads.
# Wed, 06 Jan 2021 20:45:01 GMT
ADD file:ad2b2ddca8e17229cc8d1380ecda32c4b2c04f1e2aed8f493f745c6352b34e60 in / 
# Wed, 06 Jan 2021 20:45:03 GMT
CMD ["/bin/bash"]
# Wed, 06 Jan 2021 21:04:08 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 06 Jan 2021 21:04:09 GMT
ENV LANG=C.UTF-8
# Wed, 06 Jan 2021 21:07:03 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Wed, 06 Jan 2021 21:07:04 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Jan 2021 21:07:04 GMT
ENV JAVA_VERSION=16-ea+30
# Wed, 06 Jan 2021 21:08:12 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/30/GPL/openjdk-16-ea+30_linux-aarch64_bin.tar.gz; 			downloadSha256=82cc271dfc10530a176b89f20ad2bcbc9733b78f39e3997ac54132956ce53ff1; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/30/GPL/openjdk-16-ea+30_linux-x64_bin.tar.gz; 			downloadSha256=01ef449013825308ac144c91fbbbadd9562b084d6e17cd8d428a088386707556; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 06 Jan 2021 21:08:14 GMT
CMD ["jshell"]
# Wed, 06 Jan 2021 21:38:01 GMT
ARG MAVEN_VERSION=3.6.3
# Wed, 06 Jan 2021 21:38:02 GMT
ARG USER_HOME_DIR=/root
# Wed, 06 Jan 2021 21:38:02 GMT
ARG SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0
# Wed, 06 Jan 2021 21:38:03 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries
# Wed, 06 Jan 2021 21:38:37 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN microdnf install findutils git
# Wed, 06 Jan 2021 21:38:45 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 06 Jan 2021 21:38:46 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 06 Jan 2021 21:38:46 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 06 Jan 2021 21:38:47 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 06 Jan 2021 21:38:47 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 06 Jan 2021 21:38:48 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 06 Jan 2021 21:38:48 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:d0eecbd2c3e7306adbf5b4a0d9bebc7d266ebe78bda044d35b0994c1cf655a54`  
		Last Modified: Wed, 06 Jan 2021 20:47:00 GMT  
		Size: 42.0 MB (41996293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d959bac04e84615265b829b8f4c62eddad4d65f7aabc8d560ca8430057b054`  
		Last Modified: Wed, 06 Jan 2021 21:13:39 GMT  
		Size: 14.1 MB (14057340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3603a6118bec8ebbcddc61419dd5fb282a3f72ebd53c626d39d2dee3c82fa78`  
		Last Modified: Wed, 06 Jan 2021 21:15:44 GMT  
		Size: 179.2 MB (179209701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba608783377c16033e3cec105a9da9e4359ce7f9d40430c30b89c72c16be5ae`  
		Last Modified: Wed, 06 Jan 2021 21:42:01 GMT  
		Size: 116.1 MB (116139859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e159e3fa28e03f0dfa0cdf765ba73405f50b27893eadb681e46f2751fbe3ec2`  
		Last Modified: Wed, 06 Jan 2021 21:41:46 GMT  
		Size: 9.6 MB (9581204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67474e6fe992dfedfafc0d2808cf45621053db999655c73584c47c43086ff988`  
		Last Modified: Wed, 06 Jan 2021 21:41:47 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7d4b26b59a5ca9d1a403d556423f1f151fdfd9c5f5a45b7309d960be50bcb5b`  
		Last Modified: Wed, 06 Jan 2021 21:41:46 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
