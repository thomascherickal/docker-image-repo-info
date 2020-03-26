## `maven:3-openjdk-15`

```console
$ docker pull maven@sha256:641a193b85bd75c5f1b42a2cf596c90aec729b8cc2e90818b2101902f2af0275
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `maven:3-openjdk-15` - linux; amd64

```console
$ docker pull maven@sha256:e9b0be93fe37770a62d8a68fe8cd794860cbef68a3e4900990d8e89e070b43fe
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.5 MB (265525869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f64bc165a7ee6908ef280a90d926c65506ad95918f79239288b40bac2056358e`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 30 Aug 2018 21:49:27 GMT
MAINTAINER Oracle Linux Product Team <ol-ovm-info_ww@oracle.com>
# Tue, 10 Mar 2020 02:20:39 GMT
ADD file:ca821d696bf87ff0b7ed9d85b5b0acc4656fc6498d2f5bd2c051bb16a99bfcbf in / 
# Tue, 10 Mar 2020 02:20:40 GMT
CMD ["/bin/bash"]
# Tue, 10 Mar 2020 02:37:57 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Tue, 10 Mar 2020 02:37:57 GMT
ENV LANG=en_US.UTF-8
# Tue, 10 Mar 2020 02:37:57 GMT
ENV JAVA_HOME=/usr/java/openjdk-15
# Tue, 10 Mar 2020 02:37:58 GMT
ENV PATH=/usr/java/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 23 Mar 2020 20:20:44 GMT
ENV JAVA_VERSION=15-ea+15
# Mon, 23 Mar 2020 20:20:45 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk15/15/GPL/openjdk-15-ea+15_linux-x64_bin.tar.gz
# Mon, 23 Mar 2020 20:20:45 GMT
ENV JAVA_SHA256=5ac08aae3a6533ef6d6284230f30ec060ca70dc53fa94358f4b16fe1209fa557
# Mon, 23 Mar 2020 20:21:31 GMT
RUN set -eux; 		curl -fL -o /openjdk.tgz "$JAVA_URL"; 	echo "$JAVA_SHA256 */openjdk.tgz" | sha256sum -c -; 	mkdir -p "$JAVA_HOME"; 	tar --extract --file /openjdk.tgz --directory "$JAVA_HOME" --strip-components 1; 	rm /openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		java --version; 	javac --version
# Mon, 23 Mar 2020 20:21:31 GMT
CMD ["jshell"]
# Thu, 26 Mar 2020 18:51:50 GMT
ARG MAVEN_VERSION=3.6.3
# Thu, 26 Mar 2020 18:51:50 GMT
ARG USER_HOME_DIR=/root
# Thu, 26 Mar 2020 18:51:50 GMT
ARG SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0
# Thu, 26 Mar 2020 18:51:50 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries
# Thu, 26 Mar 2020 18:52:00 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Thu, 26 Mar 2020 18:52:00 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 26 Mar 2020 18:52:00 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 26 Mar 2020 18:52:00 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 26 Mar 2020 18:52:00 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Thu, 26 Mar 2020 18:52:00 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 26 Mar 2020 18:52:01 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:cd17e56c322c9601c98f41573bb47bd4cd68ff386d7d07538f156a7c0ef6c650`  
		Last Modified: Tue, 10 Mar 2020 02:22:01 GMT  
		Size: 42.7 MB (42725735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecdd73bb99224b1c73d7d3d8eea56a91f5e7fc73628dcfa3b5432cca23c7373d`  
		Last Modified: Tue, 10 Mar 2020 02:42:14 GMT  
		Size: 14.8 MB (14770095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a260e7ef0586f8567cbc6e0c71b15918f5c14d178e26ac5d28d0133b3a30da8c`  
		Last Modified: Mon, 23 Mar 2020 20:24:08 GMT  
		Size: 198.4 MB (198447140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfad9aa21f180d7d5f73f1c7523afa2272f7391e43fe3d587875ddbbd437bfe8`  
		Last Modified: Thu, 26 Mar 2020 18:52:37 GMT  
		Size: 9.6 MB (9581681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:586a16c493c48b75c4c16c7eeada3c2144365f58a5b1cd5169b48548a75a7ad6`  
		Last Modified: Thu, 26 Mar 2020 18:52:36 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d4a7fa2924eb4af472127142c0e6564c6133581299618291394fb26cd41412`  
		Last Modified: Thu, 26 Mar 2020 18:52:36 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
