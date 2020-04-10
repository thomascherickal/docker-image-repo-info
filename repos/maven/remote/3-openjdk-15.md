## `maven:3-openjdk-15`

```console
$ docker pull maven@sha256:70638395ec48d3c1805a3043485c762f370c301cee3a6677c7bee575b59de5ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `maven:3-openjdk-15` - linux; amd64

```console
$ docker pull maven@sha256:4d78fc0bd792b71143b9ece1aa95e065116dc5555e628678d1662fd0750385c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **264.4 MB (264387603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bba12508e82fd808d2896e488e23608be14dc3c48747e22107976e31db13d8e`
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
# Fri, 10 Apr 2020 03:15:07 GMT
ENV JAVA_VERSION=15-ea+18
# Fri, 10 Apr 2020 03:15:07 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk15/18/GPL/openjdk-15-ea+18_linux-x64_bin.tar.gz
# Fri, 10 Apr 2020 03:15:07 GMT
ENV JAVA_SHA256=b5a60c62d325c8808978848fd7e21f2cce765ae97cf8361a7e136b36b6bd73bf
# Fri, 10 Apr 2020 03:15:42 GMT
RUN set -eux; 		curl -fL -o /openjdk.tgz "$JAVA_URL"; 	echo "$JAVA_SHA256 */openjdk.tgz" | sha256sum -c -; 	mkdir -p "$JAVA_HOME"; 	tar --extract --file /openjdk.tgz --directory "$JAVA_HOME" --strip-components 1; 	rm /openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		java --version; 	javac --version
# Fri, 10 Apr 2020 03:15:42 GMT
CMD ["jshell"]
# Fri, 10 Apr 2020 03:50:11 GMT
ARG MAVEN_VERSION=3.6.3
# Fri, 10 Apr 2020 03:50:11 GMT
ARG USER_HOME_DIR=/root
# Fri, 10 Apr 2020 03:50:12 GMT
ARG SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0
# Fri, 10 Apr 2020 03:50:12 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries
# Fri, 10 Apr 2020 03:50:14 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 10 Apr 2020 03:50:14 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 10 Apr 2020 03:50:14 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 10 Apr 2020 03:50:14 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 10 Apr 2020 03:50:14 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 10 Apr 2020 03:50:14 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 10 Apr 2020 03:50:15 GMT
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
	-	`sha256:72a72ea01700a55c53c1d8f34367a53f9d42d3bff09772b0b276bce24e81997f`  
		Last Modified: Fri, 10 Apr 2020 03:18:00 GMT  
		Size: 197.3 MB (197308868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a105455415dadcd3c07f9bfe8af7af6637acf5cd13e05bce64a49e27cd9ac5`  
		Last Modified: Fri, 10 Apr 2020 03:50:50 GMT  
		Size: 9.6 MB (9581685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:769818b6a7dda7f0dcef09d5f246a69a427c9f46623339fe15eb1d492671f8e9`  
		Last Modified: Fri, 10 Apr 2020 03:50:50 GMT  
		Size: 859.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66aba40e1d4c1dd40a3a69d0fcd0dd8f983d1e60bd81eaa75a83057781729712`  
		Last Modified: Fri, 10 Apr 2020 03:50:50 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
