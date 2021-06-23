## `maven:3-openjdk-17-slim`

```console
$ docker pull maven@sha256:cfc54738b1dae39dcf2d0b907a363dfc200eb34c1c3704db4a00a336a283559a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-openjdk-17-slim` - linux; amd64

```console
$ docker pull maven@sha256:05a05536f1d3c4d140ef88c784ae3bebc239c7820210d179e6fc7d814ee934c2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.2 MB (230190804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b83d94c8b6062ecb60df99f1c14c9288db220652cb57b6e84bd47d7e3df5440e`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 06:48:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:48:04 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Wed, 12 May 2021 06:48:04 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:48:04 GMT
ENV LANG=C.UTF-8
# Tue, 22 Jun 2021 21:40:35 GMT
ENV JAVA_VERSION=17-ea+27
# Tue, 22 Jun 2021 21:40:50 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/27/GPL/openjdk-17-ea+27_linux-x64_bin.tar.gz'; 			downloadSha256='7e1042e3daf741aad75ebda0ea38650111475a810be8fedf38f554732d7750f4'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/27/GPL/openjdk-17-ea+27_linux-aarch64_bin.tar.gz'; 			downloadSha256='88bdeb49442e85c19e126b720bd810bc59007973c6fc06aa6e62b609c1c44d53'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 22 Jun 2021 21:40:50 GMT
CMD ["jshell"]
# Tue, 22 Jun 2021 22:36:36 GMT
ARG MAVEN_VERSION=3.8.1
# Tue, 22 Jun 2021 22:36:36 GMT
ARG USER_HOME_DIR=/root
# Tue, 22 Jun 2021 22:36:37 GMT
ARG SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d
# Tue, 22 Jun 2021 22:36:37 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries
# Tue, 22 Jun 2021 22:36:43 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN apt-get update &&     apt-get install -y       curl procps   && rm -rf /var/lib/apt/lists/*
# Tue, 22 Jun 2021 22:36:52 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 22 Jun 2021 22:36:52 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 22 Jun 2021 22:36:52 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 22 Jun 2021 22:36:52 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 22 Jun 2021 22:36:52 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Tue, 22 Jun 2021 22:36:53 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 22 Jun 2021 22:36:53 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2b89b6081832b112f9483322d4710c661f12135e79279dc3fb1672883ada8d`  
		Last Modified: Wed, 12 May 2021 06:58:18 GMT  
		Size: 3.3 MB (3268772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c0243df2aafe16b1d73b8c656779657c2be7037309e26b26091641ac2587a9c`  
		Last Modified: Tue, 22 Jun 2021 21:51:16 GMT  
		Size: 187.5 MB (187546028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc0cd195d5b7d71b58eeebcdec9d28b5dde8ba23c299e7104fefa99be1e83c7`  
		Last Modified: Tue, 22 Jun 2021 22:40:00 GMT  
		Size: 2.6 MB (2617901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd079ac32cb350fbb07ec7cd0c0ea4053ce18aa79ed0b0bbf259dba1b7f15dc2`  
		Last Modified: Tue, 22 Jun 2021 22:40:00 GMT  
		Size: 9.6 MB (9610971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d257c828e6cbce0b7a2031bc31749a18a7f89aad52f913a38b00347e9e67e5`  
		Last Modified: Tue, 22 Jun 2021 22:39:59 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5764012c6ff044e6c897a6bc0e047dd7c945d10e51b9fa2264d6aab0c5cf8894`  
		Last Modified: Tue, 22 Jun 2021 22:39:59 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-openjdk-17-slim` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:40bcc7f81973e01afe30ab17666f791b4fe76c27b999096385fe65b714adbeee
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.6 MB (227636893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a60b5507203d4ef1d92aef97c04ded83680d785cb18bd357a94ce82cdbc79e20`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 12 May 2021 00:52:19 GMT
ADD file:91ba1791cab3ad29a1469d1e78f21f4c0b5d3d30598683b7104980604c318854 in / 
# Wed, 12 May 2021 00:52:34 GMT
CMD ["bash"]
# Thu, 27 May 2021 08:38:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 08:38:57 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Thu, 27 May 2021 08:38:57 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 27 May 2021 08:38:57 GMT
ENV LANG=C.UTF-8
# Tue, 22 Jun 2021 21:59:36 GMT
ENV JAVA_VERSION=17-ea+27
# Tue, 22 Jun 2021 21:59:49 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/27/GPL/openjdk-17-ea+27_linux-x64_bin.tar.gz'; 			downloadSha256='7e1042e3daf741aad75ebda0ea38650111475a810be8fedf38f554732d7750f4'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/27/GPL/openjdk-17-ea+27_linux-aarch64_bin.tar.gz'; 			downloadSha256='88bdeb49442e85c19e126b720bd810bc59007973c6fc06aa6e62b609c1c44d53'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 22 Jun 2021 21:59:49 GMT
CMD ["jshell"]
# Tue, 22 Jun 2021 23:00:55 GMT
ARG MAVEN_VERSION=3.8.1
# Tue, 22 Jun 2021 23:00:56 GMT
ARG USER_HOME_DIR=/root
# Tue, 22 Jun 2021 23:00:56 GMT
ARG SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d
# Tue, 22 Jun 2021 23:00:56 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries
# Tue, 22 Jun 2021 23:01:02 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN apt-get update &&     apt-get install -y       curl procps   && rm -rf /var/lib/apt/lists/*
# Tue, 22 Jun 2021 23:01:09 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 22 Jun 2021 23:01:09 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 22 Jun 2021 23:01:09 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 22 Jun 2021 23:01:09 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 22 Jun 2021 23:01:09 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Tue, 22 Jun 2021 23:01:10 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 22 Jun 2021 23:01:10 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:fcad0c936ea5c12e1c8c4edb81a97c0cde04ee71e7067ee3b246474cf1854d7a`  
		Last Modified: Wed, 12 May 2021 01:02:02 GMT  
		Size: 25.9 MB (25911250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb067f13654098b66e57229fcd818a7d0f0c73bd34d158e3bedc28ee2a7b821`  
		Last Modified: Thu, 27 May 2021 08:54:42 GMT  
		Size: 3.1 MB (3118848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3296159e0072d7246eaf63aa0c96c5c40a310668a6c75ad926bf2c4d110ecc1`  
		Last Modified: Tue, 22 Jun 2021 22:16:20 GMT  
		Size: 186.4 MB (186357951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10a8353bc9366690ebde5b7d99cdca762e7ecc39b9957bf63d5c615e683a2fa`  
		Last Modified: Tue, 22 Jun 2021 23:06:54 GMT  
		Size: 2.6 MB (2636674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc46ad3ec0f9bb8a29279c4fd638a1cd77ea5559cee1d14d835ded48e5c4a7c2`  
		Last Modified: Tue, 22 Jun 2021 23:06:55 GMT  
		Size: 9.6 MB (9610950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8a74426506cee8520726f311028735539133e5befd12fb2d8cdc8292ffb974`  
		Last Modified: Tue, 22 Jun 2021 23:06:54 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b8a4bc73fbe3bf2185114b51ec1e3fa3e57845c710a5cf7b84fc2d7aff1379`  
		Last Modified: Tue, 22 Jun 2021 23:06:54 GMT  
		Size: 363.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
