## `maven:openjdk`

```console
$ docker pull maven@sha256:68af4d9148e5a578e9042c3ec0f6871b861fb4132abf0683967816d6155780e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:openjdk` - linux; amd64

```console
$ docker pull maven@sha256:7e99a89bc266a30b6827df88879f7fac81e658a2044ecef84eec1a5463805807
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **412.1 MB (412105619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:968d394ed243d6ec76212223279fec746138e6cc202ffc991d01602dd6cbd767`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 28 May 2021 18:22:12 GMT
ADD file:9e4bcf8e1c3b7657912e93a0b82bf37752a310fa3041ec461562c85d65529ad3 in / 
# Fri, 28 May 2021 18:22:12 GMT
CMD ["/bin/bash"]
# Fri, 28 May 2021 18:39:11 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 28 May 2021 18:39:51 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Fri, 28 May 2021 18:39:51 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 May 2021 18:39:51 GMT
ENV LANG=C.UTF-8
# Fri, 28 May 2021 18:39:51 GMT
ENV JAVA_VERSION=16.0.1
# Fri, 28 May 2021 18:40:03 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.1/7147401fd7354114ac51ef3e1328291f/9/GPL/openjdk-16.0.1_linux-x64_bin.tar.gz'; 			downloadSha256='b1198ffffb7d26a3fdedc0fa599f60a0d12aa60da1714b56c1defbce95d8b235'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.1/7147401fd7354114ac51ef3e1328291f/9/GPL/openjdk-16.0.1_linux-aarch64_bin.tar.gz'; 			downloadSha256='602b005074777df2a0b4306e20152a6446803edd87ccbab95b2f313c4d9be6ba'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 28 May 2021 18:40:04 GMT
CMD ["jshell"]
# Fri, 28 May 2021 19:09:29 GMT
ARG MAVEN_VERSION=3.8.1
# Fri, 28 May 2021 19:09:29 GMT
ARG USER_HOME_DIR=/root
# Fri, 28 May 2021 19:09:29 GMT
ARG SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d
# Fri, 28 May 2021 19:09:30 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries
# Fri, 28 May 2021 19:09:55 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN microdnf install findutils git
# Fri, 28 May 2021 19:10:04 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 28 May 2021 19:10:04 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 28 May 2021 19:10:05 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 28 May 2021 19:10:05 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 28 May 2021 19:10:05 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 28 May 2021 19:10:05 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 28 May 2021 19:10:05 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:daa797b1cf01195cd47497fc9ddbf3fc4404f3fc012110f206b7fa3dd531e43d`  
		Last Modified: Fri, 28 May 2021 18:23:25 GMT  
		Size: 42.2 MB (42183040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e7f736a217a7dd2e90a8ba647050e6374f7c3f746ad3256682302739a73ee7`  
		Last Modified: Fri, 28 May 2021 18:44:27 GMT  
		Size: 13.4 MB (13401079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d43932aad3f7475408a3fe5973c87ff47f73ef3dd7a90190c9a17944e8f4fef`  
		Last Modified: Fri, 28 May 2021 18:45:57 GMT  
		Size: 184.8 MB (184799513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91082d8df2eef628124a2380120db931227eaf0854431e329c390c5a0fb280e`  
		Last Modified: Fri, 28 May 2021 19:13:34 GMT  
		Size: 162.1 MB (162109791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a5e10f765fc93a70c69139e1e56ab147972830529598f1f11daaee15291ccc`  
		Last Modified: Fri, 28 May 2021 19:13:17 GMT  
		Size: 9.6 MB (9610978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ff428ecbfb539960bcc6f0db460b0c2761df759b42d5da338ef13198dd6eb9`  
		Last Modified: Fri, 28 May 2021 19:13:16 GMT  
		Size: 859.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae7c4834da0606b73a93ec15ca8f5692742ff6b3706117dc663e65ea399f5be`  
		Last Modified: Fri, 28 May 2021 19:13:16 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:openjdk` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:db62874a12346371fe5f0087b26c31cb30ecce7eccfe74bdd631cfefacb616d8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **387.5 MB (387541902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0252a789f486043d8851a5bb784390f4b9cebfd605483b36db091d5d0198e7ad`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 28 May 2021 18:41:46 GMT
ADD file:11d6c70bf365c2598abfb596f813afaa1a3030212b79ad6c9e239dc94fdd932a in / 
# Fri, 28 May 2021 18:41:47 GMT
CMD ["/bin/bash"]
# Fri, 28 May 2021 18:59:41 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 28 May 2021 19:01:28 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Fri, 28 May 2021 19:01:28 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 May 2021 19:01:28 GMT
ENV LANG=C.UTF-8
# Fri, 28 May 2021 19:01:28 GMT
ENV JAVA_VERSION=16.0.1
# Fri, 28 May 2021 19:01:40 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.1/7147401fd7354114ac51ef3e1328291f/9/GPL/openjdk-16.0.1_linux-x64_bin.tar.gz'; 			downloadSha256='b1198ffffb7d26a3fdedc0fa599f60a0d12aa60da1714b56c1defbce95d8b235'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.1/7147401fd7354114ac51ef3e1328291f/9/GPL/openjdk-16.0.1_linux-aarch64_bin.tar.gz'; 			downloadSha256='602b005074777df2a0b4306e20152a6446803edd87ccbab95b2f313c4d9be6ba'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 28 May 2021 19:01:41 GMT
CMD ["jshell"]
# Fri, 28 May 2021 19:43:05 GMT
ARG MAVEN_VERSION=3.8.1
# Fri, 28 May 2021 19:43:05 GMT
ARG USER_HOME_DIR=/root
# Fri, 28 May 2021 19:43:05 GMT
ARG SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d
# Fri, 28 May 2021 19:43:05 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries
# Fri, 28 May 2021 19:43:27 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN microdnf install findutils git
# Fri, 28 May 2021 19:43:30 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 28 May 2021 19:43:30 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 28 May 2021 19:43:30 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 28 May 2021 19:43:30 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 28 May 2021 19:43:31 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 28 May 2021 19:43:31 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 28 May 2021 19:43:31 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:6bb7bddcd571a468c93282c3fa3b0e38fdcf15ee58fec20d63d32da56f3074af`  
		Last Modified: Fri, 28 May 2021 18:43:06 GMT  
		Size: 42.1 MB (42054735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b1363fd6ea5b7069bbb5efb69721e5fbb5c89d4cf037ed7b6b6ed1476fa5ad8`  
		Last Modified: Fri, 28 May 2021 19:11:54 GMT  
		Size: 14.2 MB (14173117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f00a316a7f6c423df0f6c1f0fc2380ddca79ecd6a3ddd98cc4403c0a1d0972`  
		Last Modified: Fri, 28 May 2021 19:14:06 GMT  
		Size: 179.2 MB (179179491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b46ee94437ae5a0f15e419f7e1772a2f59b097f3b6e4b51f0f61a10296c2888`  
		Last Modified: Fri, 28 May 2021 19:48:34 GMT  
		Size: 142.5 MB (142522374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6b02663d184c10b2c55aabc840759314c80a138cde8b044d70721a49b71434`  
		Last Modified: Fri, 28 May 2021 19:48:19 GMT  
		Size: 9.6 MB (9610970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c34c2e521b8eac1a2c7b81cac5cec689cf367bddee00b1497309623524ee3ba5`  
		Last Modified: Fri, 28 May 2021 19:48:17 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e3cc0d0e066a8414edddbbd2bb319289d829b39798011bd616a006efe993c1`  
		Last Modified: Fri, 28 May 2021 19:48:17 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
