## `maven:3-openjdk-15`

```console
$ docker pull maven@sha256:45fa8e1061626d3176ef5bda5ea5b2f9b5ab021f9524ad8a83a16813dfed3926
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `maven:3-openjdk-15` - linux; amd64

```console
$ docker pull maven@sha256:6f3a8b673f2019b93cb4f55eb6834d798393f7491e481623f7b6deffc70406c2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.6 MB (265579846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0b5f0794aa7363050efa845c69e7c7790b935ec19b2a1ed0ddbd185f41c287d`
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
# Tue, 31 Mar 2020 00:34:15 GMT
ENV JAVA_VERSION=15-ea+16
# Tue, 31 Mar 2020 00:34:15 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk15/16/GPL/openjdk-15-ea+16_linux-x64_bin.tar.gz
# Tue, 31 Mar 2020 00:34:15 GMT
ENV JAVA_SHA256=9f4ade109eb9ceea18fe3fd3b1a2428eeb8e01b5485d61916f87602b295bef7d
# Tue, 31 Mar 2020 00:34:52 GMT
RUN set -eux; 		curl -fL -o /openjdk.tgz "$JAVA_URL"; 	echo "$JAVA_SHA256 */openjdk.tgz" | sha256sum -c -; 	mkdir -p "$JAVA_HOME"; 	tar --extract --file /openjdk.tgz --directory "$JAVA_HOME" --strip-components 1; 	rm /openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		java --version; 	javac --version
# Tue, 31 Mar 2020 00:34:52 GMT
CMD ["jshell"]
# Wed, 01 Apr 2020 08:57:47 GMT
ARG MAVEN_VERSION=3.6.3
# Wed, 01 Apr 2020 08:57:48 GMT
ARG USER_HOME_DIR=/root
# Wed, 01 Apr 2020 08:57:48 GMT
ARG SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0
# Wed, 01 Apr 2020 08:57:48 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries
# Wed, 01 Apr 2020 08:57:57 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 01 Apr 2020 08:57:58 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 01 Apr 2020 08:57:58 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 01 Apr 2020 08:57:58 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 01 Apr 2020 08:57:58 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 01 Apr 2020 08:57:58 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 01 Apr 2020 08:57:59 GMT
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
	-	`sha256:10547ec3569d29156cae2a5cd1e987c8fef26a4157d2fb8584ee5711d073d86d`  
		Last Modified: Tue, 31 Mar 2020 00:37:13 GMT  
		Size: 198.5 MB (198501126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e10272bd1cace47e9c0e735d9d71c0376ee24f897cf673c39426ec1ec51dba6`  
		Last Modified: Wed, 01 Apr 2020 08:58:59 GMT  
		Size: 9.6 MB (9581669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed2a166302a7a3617c30ede9f5df45bea32103120c2039ef3746d0acfd4c5e2`  
		Last Modified: Wed, 01 Apr 2020 08:58:58 GMT  
		Size: 859.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc58ac90611f810eed4d01002562b6ec1e443f6689c96935905ceac8fc711c9f`  
		Last Modified: Wed, 01 Apr 2020 08:58:58 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
