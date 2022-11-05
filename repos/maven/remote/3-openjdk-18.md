## `maven:3-openjdk-18`

```console
$ docker pull maven@sha256:701fa3a5968ade784226f2619250a0f8b36bb8b1e0118e39cd18fc20134a8680
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-openjdk-18` - linux; amd64

```console
$ docker pull maven@sha256:0260bfa360ca7d2372c86da17c2d84b723dafda5297036a83efbea05de742ab0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **445.5 MB (445461873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f82beb5d3487800cde0e0e911aac9ac6a8e38a79fe48b8a273195bf1b9605dd`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 27 Oct 2022 17:21:44 GMT
ADD file:bb73a6f29d54ad7e2f7ec0aeeb404b06eee41432910aa60dd8f9ec5cdb904455 in / 
# Thu, 27 Oct 2022 17:21:44 GMT
CMD ["/bin/bash"]
# Thu, 27 Oct 2022 17:39:38 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 27 Oct 2022 17:40:08 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Thu, 27 Oct 2022 17:40:08 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 27 Oct 2022 17:40:08 GMT
ENV LANG=C.UTF-8
# Thu, 27 Oct 2022 17:40:08 GMT
ENV JAVA_VERSION=18.0.2.1
# Thu, 27 Oct 2022 17:40:18 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2.1/db379da656dc47308e138f21b33976fa/1/GPL/openjdk-18.0.2.1_linux-x64_bin.tar.gz'; 			downloadSha256='3bfdb59fc38884672677cebca9a216902d87fe867563182ae8bc3373a65a2ebd'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2.1/db379da656dc47308e138f21b33976fa/1/GPL/openjdk-18.0.2.1_linux-aarch64_bin.tar.gz'; 			downloadSha256='79900237a5912045f8c9f1065b5204a474803cbbb4d075ab9620650fb75dfc1b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 27 Oct 2022 17:40:19 GMT
CMD ["jshell"]
# Thu, 27 Oct 2022 18:01:22 GMT
RUN microdnf install findutils git
# Thu, 27 Oct 2022 18:01:23 GMT
ARG MAVEN_VERSION=3.8.6
# Thu, 27 Oct 2022 18:01:24 GMT
ARG USER_HOME_DIR=/root
# Thu, 27 Oct 2022 18:01:24 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Thu, 27 Oct 2022 18:01:24 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Thu, 27 Oct 2022 18:01:26 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Thu, 27 Oct 2022 18:01:26 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 27 Oct 2022 18:01:26 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 27 Oct 2022 18:01:26 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 27 Oct 2022 18:01:26 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Thu, 27 Oct 2022 18:01:26 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 27 Oct 2022 18:01:26 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:d67a603b911ada80815df642621203365c074f4903f50aed87dcf6df07e6e4c6`  
		Last Modified: Thu, 27 Oct 2022 17:23:23 GMT  
		Size: 40.6 MB (40581871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80422febbaefdcc8ba66af30635f777afc7bef13f71ad47f90af2a5da4e8099`  
		Last Modified: Thu, 27 Oct 2022 17:42:41 GMT  
		Size: 12.2 MB (12223871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459f461374cc70f7259f4e2b6307c6f9bf711dba3037540f2254ba873b2d32c6`  
		Last Modified: Thu, 27 Oct 2022 17:43:55 GMT  
		Size: 188.7 MB (188744815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ac1139555c7baad672cb9bbedc66756cd9d8010e9340efaa450f1ec4e58120`  
		Last Modified: Thu, 27 Oct 2022 18:03:57 GMT  
		Size: 195.2 MB (195170603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee1b54b0c42159e30e39fb29e357a76a1a104c66fb7c6dbecdeea7431ccf1e6`  
		Last Modified: Thu, 27 Oct 2022 18:03:41 GMT  
		Size: 8.7 MB (8739495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81773772671bb859603b54aee7b3134cf10ca1665d57db964d5103a58a50323a`  
		Last Modified: Thu, 27 Oct 2022 18:03:40 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b982c8c5559f499813b30c886a4b27b1b17a1e5b33c3f21d6d7a0e3cadc365`  
		Last Modified: Thu, 27 Oct 2022 18:03:40 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-openjdk-18` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:4ffd139c21aba80c63e95ce8b0d02b6ee4ee49e01890d36adf27b37e38c7d279
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **455.2 MB (455249800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b37d00e6fcb72a28f0c2932d83326394a4fb95a9e5ef446961cf24abf0bbd72`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 04 Nov 2022 22:50:08 GMT
ADD file:efa6454225ba5be177493364c69d425968d42231b708b5d492a41f9ab14d64f4 in / 
# Fri, 04 Nov 2022 22:50:08 GMT
CMD ["/bin/bash"]
# Sat, 05 Nov 2022 00:48:43 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Sat, 05 Nov 2022 00:50:48 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Sat, 05 Nov 2022 00:50:48 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 00:50:48 GMT
ENV LANG=C.UTF-8
# Sat, 05 Nov 2022 00:50:48 GMT
ENV JAVA_VERSION=18.0.2.1
# Sat, 05 Nov 2022 00:50:57 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2.1/db379da656dc47308e138f21b33976fa/1/GPL/openjdk-18.0.2.1_linux-x64_bin.tar.gz'; 			downloadSha256='3bfdb59fc38884672677cebca9a216902d87fe867563182ae8bc3373a65a2ebd'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2.1/db379da656dc47308e138f21b33976fa/1/GPL/openjdk-18.0.2.1_linux-aarch64_bin.tar.gz'; 			downloadSha256='79900237a5912045f8c9f1065b5204a474803cbbb4d075ab9620650fb75dfc1b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 05 Nov 2022 00:50:58 GMT
CMD ["jshell"]
# Sat, 05 Nov 2022 02:01:17 GMT
RUN microdnf install findutils git
# Sat, 05 Nov 2022 02:01:19 GMT
ARG MAVEN_VERSION=3.8.6
# Sat, 05 Nov 2022 02:01:19 GMT
ARG USER_HOME_DIR=/root
# Sat, 05 Nov 2022 02:01:19 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Sat, 05 Nov 2022 02:01:20 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Sat, 05 Nov 2022 02:01:25 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Sat, 05 Nov 2022 02:01:25 GMT
ENV MAVEN_HOME=/usr/share/maven
# Sat, 05 Nov 2022 02:01:25 GMT
ENV MAVEN_CONFIG=/root/.m2
# Sat, 05 Nov 2022 02:01:25 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Sat, 05 Nov 2022 02:01:26 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Sat, 05 Nov 2022 02:01:26 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Sat, 05 Nov 2022 02:01:26 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:a13cd8cb50ab4c8c5cb15a9929fa5faf1b7833f87c827551a9a54e84789b1e0b`  
		Last Modified: Fri, 04 Nov 2022 22:51:35 GMT  
		Size: 39.4 MB (39401738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2b575a486b4b7df2602a19466f69783be33126ccdea7a939dbef7ecc85a7c7`  
		Last Modified: Sat, 05 Nov 2022 00:53:50 GMT  
		Size: 13.0 MB (13049666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fedc660ff45bfd209b0ac28ae7621b270c6275e79147e8f130e3a6ee92f8860b`  
		Last Modified: Sat, 05 Nov 2022 00:55:29 GMT  
		Size: 187.7 MB (187659341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2707e5f6c44a48aa9dd1daf8b47c27197441b0258977170c8a0a0864d2ea1b99`  
		Last Modified: Sat, 05 Nov 2022 02:03:10 GMT  
		Size: 206.4 MB (206398343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73c6573464ec3ad1638ddd93e4940e9a78b9577cef586b3bc4fc55a68fea7eb7`  
		Last Modified: Sat, 05 Nov 2022 02:02:59 GMT  
		Size: 8.7 MB (8739500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e07b27c9a3fec33549fe4775075b3b1a5cd621b2fb659f2d5ea05dc9c9e900`  
		Last Modified: Sat, 05 Nov 2022 02:02:58 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078afe35034928f0ed1b46f0febaa58ac1b6d4b1258a96a4d255a93575e8673e`  
		Last Modified: Sat, 05 Nov 2022 02:02:59 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
