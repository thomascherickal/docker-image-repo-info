## `maven:3-openjdk-18-slim`

```console
$ docker pull maven@sha256:1dd46b4633c833bb4e58d1b18bec91da42a4927e63dff6df877fe2a444ec866f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-openjdk-18-slim` - linux; amd64

```console
$ docker pull maven@sha256:0c9dab1f2d1b130c5533f22ef5d353cae3145a652b7e6d46f7759f65cfbb349e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.3 MB (233286284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:977e98e8b569e92c5072aaf94bba81e5cc237b9747e88e19c0060c97889fb570`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:29:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 04:32:33 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Tue, 23 Aug 2022 04:32:33 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 04:32:33 GMT
ENV LANG=C.UTF-8
# Tue, 23 Aug 2022 04:32:33 GMT
ENV JAVA_VERSION=18.0.2.1
# Tue, 23 Aug 2022 04:32:47 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2.1/db379da656dc47308e138f21b33976fa/1/GPL/openjdk-18.0.2.1_linux-x64_bin.tar.gz'; 			downloadSha256='3bfdb59fc38884672677cebca9a216902d87fe867563182ae8bc3373a65a2ebd'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2.1/db379da656dc47308e138f21b33976fa/1/GPL/openjdk-18.0.2.1_linux-aarch64_bin.tar.gz'; 			downloadSha256='79900237a5912045f8c9f1065b5204a474803cbbb4d075ab9620650fb75dfc1b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 23 Aug 2022 04:32:47 GMT
CMD ["jshell"]
# Tue, 23 Aug 2022 21:00:37 GMT
RUN apt-get update   && apt-get install -y curl procps   && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 21:00:37 GMT
ARG MAVEN_VERSION=3.8.6
# Tue, 23 Aug 2022 21:00:37 GMT
ARG USER_HOME_DIR=/root
# Tue, 23 Aug 2022 21:00:37 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Tue, 23 Aug 2022 21:00:37 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Tue, 23 Aug 2022 21:00:43 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 23 Aug 2022 21:00:44 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 23 Aug 2022 21:00:44 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 23 Aug 2022 21:00:44 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 23 Aug 2022 21:00:44 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Tue, 23 Aug 2022 21:00:44 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 23 Aug 2022 21:00:44 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b1c853f5d1e2529f16cddde75874e53c112a9bee4b0954afb1bb8a2a29044b`  
		Last Modified: Tue, 23 Aug 2022 04:36:30 GMT  
		Size: 1.6 MB (1582289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe3d678d285f0faa4f4082af3b35458563df55b5090e41db13b0407a3a5cfe7`  
		Last Modified: Tue, 23 Aug 2022 04:41:47 GMT  
		Size: 189.1 MB (189120359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342e86082e6b4fa5c3adc78fd77c0d3a5083a86283f6904e2c345b8f9dc0a0c0`  
		Last Modified: Tue, 23 Aug 2022 21:03:14 GMT  
		Size: 2.5 MB (2461437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b28e294eec008c279993d37102264499ca8ca7b45b8fc3211995a837616745`  
		Last Modified: Tue, 23 Aug 2022 21:03:14 GMT  
		Size: 8.7 MB (8739500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb4e03a80c92c79e15d6c73333970abc15211b68ba8a44ff515edff98bbd2f2`  
		Last Modified: Tue, 23 Aug 2022 21:03:13 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:081241495a31a965b0392fce66ec87c00ac858e359903abcf2888e5153622604`  
		Last Modified: Tue, 23 Aug 2022 21:03:13 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-openjdk-18-slim` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:f5c5b2bc34190e7f1ddaf7cef3fdfc2c90754021882b0a28f67b55b72d45afc6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.3 MB (230255031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b65c8c556c16d16c1b0c486a3e66e421f3fe24b6a3a8cd08a56c062b95c3ddd0`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 05:16:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 05:20:41 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Tue, 23 Aug 2022 05:20:42 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 05:20:43 GMT
ENV LANG=C.UTF-8
# Tue, 23 Aug 2022 05:20:44 GMT
ENV JAVA_VERSION=18.0.2.1
# Tue, 23 Aug 2022 05:20:57 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2.1/db379da656dc47308e138f21b33976fa/1/GPL/openjdk-18.0.2.1_linux-x64_bin.tar.gz'; 			downloadSha256='3bfdb59fc38884672677cebca9a216902d87fe867563182ae8bc3373a65a2ebd'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2.1/db379da656dc47308e138f21b33976fa/1/GPL/openjdk-18.0.2.1_linux-aarch64_bin.tar.gz'; 			downloadSha256='79900237a5912045f8c9f1065b5204a474803cbbb4d075ab9620650fb75dfc1b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 23 Aug 2022 05:20:58 GMT
CMD ["jshell"]
# Tue, 23 Aug 2022 22:34:10 GMT
RUN apt-get update   && apt-get install -y curl procps   && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 22:34:10 GMT
ARG MAVEN_VERSION=3.8.6
# Tue, 23 Aug 2022 22:34:11 GMT
ARG USER_HOME_DIR=/root
# Tue, 23 Aug 2022 22:34:12 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Tue, 23 Aug 2022 22:34:13 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Tue, 23 Aug 2022 22:34:17 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 23 Aug 2022 22:34:18 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 23 Aug 2022 22:34:19 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 23 Aug 2022 22:34:21 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 23 Aug 2022 22:34:22 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Tue, 23 Aug 2022 22:34:22 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 23 Aug 2022 22:34:23 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a336c8a0edb35428a570e25d2023ce4e03a37c1c31638892cc2c38fca7cf3c91`  
		Last Modified: Tue, 23 Aug 2022 05:27:39 GMT  
		Size: 1.4 MB (1361214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ea9e6bfea9a7640362cdcf466fab21b18ffda897aebfa7a000ea19c1f1f8877`  
		Last Modified: Tue, 23 Aug 2022 05:34:17 GMT  
		Size: 187.8 MB (187822309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19273cb6ce472e19361589da914508bf656835139fe244229482986784df20c7`  
		Last Modified: Tue, 23 Aug 2022 22:38:10 GMT  
		Size: 2.3 MB (2267038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e7f4ec5f17cc45f3733d65a3f4de5ceab4dd2f304a97cf1540d793d2fc8f57f`  
		Last Modified: Tue, 23 Aug 2022 22:38:10 GMT  
		Size: 8.7 MB (8739466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef626b5c8e29c2a509050edba84992fc18b8282d3e7d56080189790f2b59a0f8`  
		Last Modified: Tue, 23 Aug 2022 22:38:09 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8700bd3e39fd1456ee63422d932b3a88b035474a670e514c0a2ca2a67c86239`  
		Last Modified: Tue, 23 Aug 2022 22:38:09 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
