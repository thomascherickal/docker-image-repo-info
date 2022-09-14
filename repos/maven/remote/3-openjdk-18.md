## `maven:3-openjdk-18`

```console
$ docker pull maven@sha256:cd783a872e863d002a93977ac363952853713c8e90d96c97603d783ee830ba7c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-openjdk-18` - linux; amd64

```console
$ docker pull maven@sha256:0078bb754b3019b630a2fb97de107c5e08e69a29546a0e1ee825249bd6f78955
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **442.0 MB (442016388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf72b8e447904f0f4566121ac5225738f95ff41338c143e138d2201cba3a9164`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 14 Sep 2022 21:20:28 GMT
ADD file:e00d9d8d8f616feec8c064f2250e4836ea3b533ead0611d1af2245974abb4e88 in / 
# Wed, 14 Sep 2022 21:20:28 GMT
CMD ["/bin/bash"]
# Wed, 14 Sep 2022 21:37:14 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 14 Sep 2022 21:38:15 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Wed, 14 Sep 2022 21:38:15 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Sep 2022 21:38:15 GMT
ENV LANG=C.UTF-8
# Wed, 14 Sep 2022 21:38:15 GMT
ENV JAVA_VERSION=18.0.2.1
# Wed, 14 Sep 2022 21:38:25 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2.1/db379da656dc47308e138f21b33976fa/1/GPL/openjdk-18.0.2.1_linux-x64_bin.tar.gz'; 			downloadSha256='3bfdb59fc38884672677cebca9a216902d87fe867563182ae8bc3373a65a2ebd'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2.1/db379da656dc47308e138f21b33976fa/1/GPL/openjdk-18.0.2.1_linux-aarch64_bin.tar.gz'; 			downloadSha256='79900237a5912045f8c9f1065b5204a474803cbbb4d075ab9620650fb75dfc1b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 14 Sep 2022 21:38:25 GMT
CMD ["jshell"]
# Wed, 14 Sep 2022 22:01:10 GMT
RUN microdnf install findutils git
# Wed, 14 Sep 2022 22:01:10 GMT
ARG MAVEN_VERSION=3.8.6
# Wed, 14 Sep 2022 22:01:11 GMT
ARG USER_HOME_DIR=/root
# Wed, 14 Sep 2022 22:01:11 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Wed, 14 Sep 2022 22:01:11 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Wed, 14 Sep 2022 22:01:19 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 14 Sep 2022 22:01:19 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 14 Sep 2022 22:01:19 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 14 Sep 2022 22:01:19 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 14 Sep 2022 22:01:19 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 14 Sep 2022 22:01:20 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 14 Sep 2022 22:01:20 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:051f419db9dd9462e8995886d24f592c26cef792cc915dfbc7548e0b19aa55fe`  
		Last Modified: Wed, 14 Sep 2022 21:21:25 GMT  
		Size: 40.6 MB (40590248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa51c6010a14c1984cbdea1332a5d2f77bf6e0141bc497b44dca611e21f9b391`  
		Last Modified: Wed, 14 Sep 2022 21:41:16 GMT  
		Size: 12.2 MB (12232427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb80f8e66e0b5f7d3dd891238b14c1b12e75a3353f59a4bdca5c8477f3333fee`  
		Last Modified: Wed, 14 Sep 2022 21:43:22 GMT  
		Size: 188.7 MB (188744873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db69af356b86ff58c1dbcbc62028adef2b5e2c3c048f1e38c8396de2767e37b`  
		Last Modified: Wed, 14 Sep 2022 22:04:13 GMT  
		Size: 191.7 MB (191708130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c8e9c04d6a5c26d6f8a97eea128c01ccf9d17c01bada147c1a1e5a499ee484`  
		Last Modified: Wed, 14 Sep 2022 22:03:58 GMT  
		Size: 8.7 MB (8739502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78529be6a32d0ccfd0407368ef82b5e98e24cf9f0c3a8bf5f042148f3fe4cdb3`  
		Last Modified: Wed, 14 Sep 2022 22:03:57 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7209ad5568771d87f02a991d4c6e8ec0a6b4f02e86ab9afdc9ce72608456caab`  
		Last Modified: Wed, 14 Sep 2022 22:03:57 GMT  
		Size: 353.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-openjdk-18` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:48d69baf382a917b635f01c59df04f143228cf7db6d3352862a5346c91db396a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **447.4 MB (447412997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd290775e33b80ab5c27a78b3ef67d90283717909c07076cc9bd7b624867656f`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 30 Aug 2022 20:47:49 GMT
ADD file:4f53d93ae4bccd786d6beda6f0ec4a450fd23a8fff2786d9e5b024a64aad6bb1 in / 
# Tue, 30 Aug 2022 20:47:50 GMT
CMD ["/bin/bash"]
# Tue, 30 Aug 2022 21:08:02 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Tue, 30 Aug 2022 21:10:25 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Tue, 30 Aug 2022 21:10:26 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Aug 2022 21:10:27 GMT
ENV LANG=C.UTF-8
# Tue, 30 Aug 2022 21:10:28 GMT
ENV JAVA_VERSION=18.0.2.1
# Tue, 30 Aug 2022 21:10:39 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2.1/db379da656dc47308e138f21b33976fa/1/GPL/openjdk-18.0.2.1_linux-x64_bin.tar.gz'; 			downloadSha256='3bfdb59fc38884672677cebca9a216902d87fe867563182ae8bc3373a65a2ebd'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2.1/db379da656dc47308e138f21b33976fa/1/GPL/openjdk-18.0.2.1_linux-aarch64_bin.tar.gz'; 			downloadSha256='79900237a5912045f8c9f1065b5204a474803cbbb4d075ab9620650fb75dfc1b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 30 Aug 2022 21:10:40 GMT
CMD ["jshell"]
# Tue, 30 Aug 2022 21:37:51 GMT
RUN microdnf install findutils git
# Tue, 30 Aug 2022 21:37:52 GMT
ARG MAVEN_VERSION=3.8.6
# Tue, 30 Aug 2022 21:37:52 GMT
ARG USER_HOME_DIR=/root
# Tue, 30 Aug 2022 21:37:53 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Tue, 30 Aug 2022 21:37:54 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Tue, 30 Aug 2022 21:38:05 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 30 Aug 2022 21:38:05 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 30 Aug 2022 21:38:06 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 30 Aug 2022 21:38:08 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 30 Aug 2022 21:38:09 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Tue, 30 Aug 2022 21:38:09 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 30 Aug 2022 21:38:10 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:fe1dbcd3b09e2c1e850118728988d6907b2f43969fe81443f422984829c640ce`  
		Last Modified: Tue, 30 Aug 2022 20:48:58 GMT  
		Size: 38.3 MB (38321155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43dbff7ac899e8f3413a3849ac2dcb6c61d52e9763a3cf5bc4c38d1e823fa3a`  
		Last Modified: Tue, 30 Aug 2022 21:16:28 GMT  
		Size: 13.0 MB (13042009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9919019213e036b87bb11d56e6172446367d4b2d6e013b7453758070cffc209`  
		Last Modified: Tue, 30 Aug 2022 21:19:07 GMT  
		Size: 187.7 MB (187659381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7133ef91773572de0d0614c9f1938b89ba580992d458033ed5c6d97b1d72e11a`  
		Last Modified: Tue, 30 Aug 2022 21:42:18 GMT  
		Size: 199.6 MB (199649765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac79d335ccab51f4fc7df806a7d998ec08a62b01fe0367b47b262cdfbfef7d7f`  
		Last Modified: Tue, 30 Aug 2022 21:42:00 GMT  
		Size: 8.7 MB (8739468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07bc739acd40680a21f45c372f4949fb6d06f9049ca73f0d1a46fb3d5638f605`  
		Last Modified: Tue, 30 Aug 2022 21:41:59 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b617227eee0349065703d19a16f8004243b83d8bb354d717c6de0cc496c4deb`  
		Last Modified: Tue, 30 Aug 2022 21:41:59 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
