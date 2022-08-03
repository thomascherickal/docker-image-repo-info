## `maven:3-openjdk-18-slim`

```console
$ docker pull maven@sha256:41b724903fa72146b4871539d8d5cae72b6da9fd901dcddad521c8845ce01889
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-openjdk-18-slim` - linux; amd64

```console
$ docker pull maven@sha256:de19430638d58b9ee73a5b5f523b8f6312dd9f3afe0858dd982561e6e9049bd4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.3 MB (233266787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d68190f0892901211c5f03cc3a7d9246f132196bcc27c99e8741cd48caabc6ed`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 01:55:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 01:58:39 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Tue, 12 Jul 2022 01:58:39 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 01:58:39 GMT
ENV LANG=C.UTF-8
# Thu, 21 Jul 2022 00:40:56 GMT
ENV JAVA_VERSION=18.0.2
# Thu, 21 Jul 2022 00:41:10 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2/f6ad4b4450fd4d298113270ec84f30ee/9/GPL/openjdk-18.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='cf06f41a3952038df0550e8cbc2baf0aa877c3ba00cca0dd26f73134f8baf0e6'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2/f6ad4b4450fd4d298113270ec84f30ee/9/GPL/openjdk-18.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='99d994dab3c5ad0e87a3d72dc3be33d5b2f045f0ddda0cb7853dfbf6b5d5d3b0'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 21 Jul 2022 00:41:11 GMT
CMD ["jshell"]
# Thu, 21 Jul 2022 01:20:49 GMT
RUN apt-get update   && apt-get install -y curl procps   && rm -rf /var/lib/apt/lists/*
# Thu, 21 Jul 2022 01:20:49 GMT
ARG MAVEN_VERSION=3.8.6
# Thu, 21 Jul 2022 01:20:49 GMT
ARG USER_HOME_DIR=/root
# Thu, 21 Jul 2022 01:20:50 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Thu, 21 Jul 2022 01:20:50 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Thu, 21 Jul 2022 01:20:52 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Thu, 21 Jul 2022 01:20:52 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 21 Jul 2022 01:20:52 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 21 Jul 2022 01:20:52 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 21 Jul 2022 01:20:52 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Thu, 21 Jul 2022 01:20:52 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 21 Jul 2022 01:20:52 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e693ef00b582081dff0c396dca2fc62b2050dc4220400c6964508f017e45f0d1`  
		Last Modified: Tue, 12 Jul 2022 02:09:05 GMT  
		Size: 1.6 MB (1582273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6318e70d288454c6661cd0956c4a76175227c53c8a8eb54bce0067e784c486`  
		Last Modified: Thu, 21 Jul 2022 00:49:48 GMT  
		Size: 189.1 MB (189117960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c881edea346b62385736d2a768132db8cfab4bef535c00867e49d7c563ab46`  
		Last Modified: Thu, 21 Jul 2022 01:23:37 GMT  
		Size: 2.5 MB (2459235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4699b89b49dcf9d95f151c8ccec046add0751b93e3853fa3b5e5708a2c1f9a76`  
		Last Modified: Thu, 21 Jul 2022 01:23:38 GMT  
		Size: 8.7 MB (8739496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3bc3d6c6881297784ed1410cc9e2cba0d7d433fd8a39b3a4b0cacf21df828f`  
		Last Modified: Thu, 21 Jul 2022 01:23:37 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70f244c59465eb2f005d90a7917350104b8bff2b65a36f55d9c62e985816552`  
		Last Modified: Thu, 21 Jul 2022 01:23:37 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-openjdk-18-slim` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:d6496a13f0d5b8f6b518cd2967da26402cbfa4a9cba4d67c3d26bc8ce394c2a8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.5 MB (230450526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4226cb61de255ccaabc868548a023762f6c69aed4177ecf7358b1689440190d1`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:38 GMT
ADD file:6039adfbca55ed34a719c37672c664e3524130a0e2a3b8663629b8120b81b790 in / 
# Tue, 02 Aug 2022 00:40:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:41:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:46:01 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Tue, 02 Aug 2022 04:46:02 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 04:46:03 GMT
ENV LANG=C.UTF-8
# Tue, 02 Aug 2022 04:46:04 GMT
ENV JAVA_VERSION=18.0.2
# Tue, 02 Aug 2022 04:46:19 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2/f6ad4b4450fd4d298113270ec84f30ee/9/GPL/openjdk-18.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='cf06f41a3952038df0550e8cbc2baf0aa877c3ba00cca0dd26f73134f8baf0e6'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2/f6ad4b4450fd4d298113270ec84f30ee/9/GPL/openjdk-18.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='99d994dab3c5ad0e87a3d72dc3be33d5b2f045f0ddda0cb7853dfbf6b5d5d3b0'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 02 Aug 2022 04:46:19 GMT
CMD ["jshell"]
# Wed, 03 Aug 2022 01:02:06 GMT
RUN apt-get update   && apt-get install -y curl procps   && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 01:02:06 GMT
ARG MAVEN_VERSION=3.8.6
# Wed, 03 Aug 2022 01:02:07 GMT
ARG USER_HOME_DIR=/root
# Wed, 03 Aug 2022 01:02:08 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Wed, 03 Aug 2022 01:02:09 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Wed, 03 Aug 2022 01:02:19 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 03 Aug 2022 01:02:20 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 03 Aug 2022 01:02:21 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 03 Aug 2022 01:02:23 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 03 Aug 2022 01:02:24 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 03 Aug 2022 01:02:24 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 03 Aug 2022 01:02:25 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:a9fe95647e78b5516c7e2327355b6996e2ea295cd76ae242cbfe87f016b4e760`  
		Last Modified: Tue, 02 Aug 2022 00:46:05 GMT  
		Size: 30.1 MB (30054304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4015b6e8cc8db11af172df5c0369552bc2a74cd69094b0756d21fc6b0b2a5393`  
		Last Modified: Tue, 02 Aug 2022 05:03:25 GMT  
		Size: 1.6 MB (1565954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94b52de585ebcb5f5cc17675a97f2c82821b3d647781eb8bc053cb757e207c7`  
		Last Modified: Tue, 02 Aug 2022 05:10:28 GMT  
		Size: 187.8 MB (187822580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db7170ff6cb25f02ba4c4f4f921e7f4e8b3d6d818a69103b9abe5d4e4bab1fcf`  
		Last Modified: Wed, 03 Aug 2022 01:13:57 GMT  
		Size: 2.3 MB (2267001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb05214f3cd9952238fcb211fd771fb1e3544f45c26f259c1b4f712a18262db`  
		Last Modified: Wed, 03 Aug 2022 01:13:58 GMT  
		Size: 8.7 MB (8739471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4e1b1b9d4718a62db0254ca13346a9db87212b36c0fe34031b49779042eeee`  
		Last Modified: Wed, 03 Aug 2022 01:13:57 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d319ced30f51bf023254b8c1c06631cc0c8217fa9d785b79dd7a9e159d3ac6b2`  
		Last Modified: Wed, 03 Aug 2022 01:13:57 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
