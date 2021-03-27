## `maven:3-openjdk-16-slim`

```console
$ docker pull maven@sha256:eda282c387b1eef822567ee00345706fb8f88d5885fde78a13c4c564ce3b4ed3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-openjdk-16-slim` - linux; amd64

```console
$ docker pull maven@sha256:73d3397bd28ad9b1beaffbc027e9b70ac0f5ce011a214d6f4c3355908b273bff
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.7 MB (227722761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d54ba0e44225e88a4b7350268b150ad4b60bbfa21e503aa70de8ec1c7237d0b`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 12 Mar 2021 02:20:40 GMT
ADD file:3c32f1cd03198e141dd233a7ffd13444157d4150ad917d548f3ee9bf5953ce22 in / 
# Fri, 12 Mar 2021 02:20:41 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 22:10:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 22:11:42 GMT
ENV JAVA_HOME=/usr/local/openjdk-16
# Fri, 12 Mar 2021 22:11:43 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 22:11:43 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 22:11:44 GMT
ENV JAVA_VERSION=16
# Fri, 12 Mar 2021 22:12:04 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk16/7863447f0ab643c585b9bdebf67c69db/36/GPL/openjdk-16_linux-x64_bin.tar.gz'; 			downloadSha256='e952958f16797ad7dc7cd8b724edd69ec7e0e0434537d80d6b5165193e33b931'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk16/7863447f0ab643c585b9bdebf67c69db/36/GPL/openjdk-16_linux-aarch64_bin.tar.gz'; 			downloadSha256='273d3ae0ff14af801c5ffa71fd081f1cc505354f308ce11c77af55302c83d2bf'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 12 Mar 2021 22:12:05 GMT
CMD ["jshell"]
# Sat, 13 Mar 2021 12:39:47 GMT
ARG MAVEN_VERSION=3.6.3
# Sat, 13 Mar 2021 12:39:47 GMT
ARG USER_HOME_DIR=/root
# Sat, 13 Mar 2021 12:39:47 GMT
ARG SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0
# Sat, 13 Mar 2021 12:39:47 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries
# Sat, 13 Mar 2021 12:39:53 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN apt-get update &&     apt-get install -y       curl procps   && rm -rf /var/lib/apt/lists/*
# Sat, 13 Mar 2021 12:39:56 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Sat, 13 Mar 2021 12:39:56 GMT
ENV MAVEN_HOME=/usr/share/maven
# Sat, 13 Mar 2021 12:39:56 GMT
ENV MAVEN_CONFIG=/root/.m2
# Sat, 13 Mar 2021 12:39:56 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Sat, 13 Mar 2021 12:39:56 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Sat, 13 Mar 2021 12:39:57 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Sat, 13 Mar 2021 12:39:57 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:6f28985ad1843afd6fd4fe0b42a30bfab63c27d302362e7341e3316e8ba25ced`  
		Last Modified: Fri, 12 Mar 2021 02:26:11 GMT  
		Size: 27.1 MB (27101001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3555c3885852c38ecf4a297b798053677bc7553f9c7631788ef75e35cb4262c`  
		Last Modified: Fri, 12 Mar 2021 22:22:18 GMT  
		Size: 3.3 MB (3268564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd9c100e068de7dc9d460f49084914b105640e863a2e812ca5c33e068232a808`  
		Last Modified: Fri, 12 Mar 2021 22:24:25 GMT  
		Size: 185.2 MB (185153273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88bf969dd674d780b6af74919a157c4dc9759cc663f45ef6ca9c909c4f525596`  
		Last Modified: Sat, 13 Mar 2021 12:44:20 GMT  
		Size: 2.6 MB (2617504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be16236ef04c519905df1fda7d6f761f218b2a7a1fba3184280162a6e66f5aca`  
		Last Modified: Sat, 13 Mar 2021 12:44:20 GMT  
		Size: 9.6 MB (9581200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cacd102de5d7f471da32d45b71feb49c2bca9972c09673bd23dd486748d0c841`  
		Last Modified: Sat, 13 Mar 2021 12:44:19 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2f190f590f09ab1faa0bf83eca12d65fe530ce2bb3c56ca324e311ff4607f0`  
		Last Modified: Sat, 13 Mar 2021 12:44:19 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-openjdk-16-slim` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:11a17caf0132b83eceb8f1f1a34ac0e3047f94b015fdcc4e514c61ef5d797e04
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.7 MB (220723916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:402c1ab9af8299766d6c02dd9226f9a120b7a2b71c2eaf5a2a6e51b360716211`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 26 Mar 2021 15:41:54 GMT
ADD file:c8c0d923527574a26725e0a1995051870ed169ff6b6ebfe77c50810f5583690b in / 
# Fri, 26 Mar 2021 15:41:56 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 19:43:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 19:44:24 GMT
ENV JAVA_HOME=/usr/local/openjdk-16
# Fri, 26 Mar 2021 19:44:25 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 19:44:25 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 19:44:26 GMT
ENV JAVA_VERSION=16
# Fri, 26 Mar 2021 19:44:57 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk16/7863447f0ab643c585b9bdebf67c69db/36/GPL/openjdk-16_linux-x64_bin.tar.gz'; 			downloadSha256='e952958f16797ad7dc7cd8b724edd69ec7e0e0434537d80d6b5165193e33b931'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk16/7863447f0ab643c585b9bdebf67c69db/36/GPL/openjdk-16_linux-aarch64_bin.tar.gz'; 			downloadSha256='273d3ae0ff14af801c5ffa71fd081f1cc505354f308ce11c77af55302c83d2bf'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 26 Mar 2021 19:44:58 GMT
CMD ["jshell"]
# Fri, 26 Mar 2021 19:58:10 GMT
ARG MAVEN_VERSION=3.6.3
# Fri, 26 Mar 2021 19:58:11 GMT
ARG USER_HOME_DIR=/root
# Fri, 26 Mar 2021 19:58:13 GMT
ARG SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0
# Fri, 26 Mar 2021 19:58:14 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries
# Fri, 26 Mar 2021 19:58:31 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN apt-get update &&     apt-get install -y       curl procps   && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 19:58:45 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 26 Mar 2021 19:58:46 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 26 Mar 2021 19:58:47 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 26 Mar 2021 19:58:48 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 26 Mar 2021 19:58:49 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 26 Mar 2021 19:58:50 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 26 Mar 2021 19:58:51 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:989f98f7e44fde3e2eb49bc6d2bfed15401201d21cd90f42cd9fc4c26eef8bb0`  
		Last Modified: Fri, 26 Mar 2021 15:48:47 GMT  
		Size: 25.9 MB (25856384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:844d8de9377aa4bd4c66d812b6226ebe8ebcb1dbbbdf3be6e3e9d0ea7363e0d3`  
		Last Modified: Fri, 26 Mar 2021 19:50:29 GMT  
		Size: 3.1 MB (3118857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132c603346649d5cfa9bdb9c9b9aeb032dad213434bf6390d60c4c348f0e0cfb`  
		Last Modified: Fri, 26 Mar 2021 19:51:52 GMT  
		Size: 179.5 MB (179529574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6834f5bbaa8b00010c5662b3152207024ec932de2828b76cf2e788567f2d67e5`  
		Last Modified: Fri, 26 Mar 2021 20:06:22 GMT  
		Size: 2.6 MB (2636693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598d66c156d1eae48548a3bd563e6fbf67ce5cbf535786017a0e03faf4d6f969`  
		Last Modified: Fri, 26 Mar 2021 20:06:23 GMT  
		Size: 9.6 MB (9581193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea3866636315bc486a6ebe7da32bb6d463f0fa009ccb12c884bdb6e461a97db`  
		Last Modified: Fri, 26 Mar 2021 20:06:22 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08be3c31bc1b668ba0cb61b4c025ff8d817ded3c9b5318e3e5847d154deeb7ce`  
		Last Modified: Fri, 26 Mar 2021 20:06:22 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
