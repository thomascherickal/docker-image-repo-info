## `openjdk:14-ea-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:682e668a56f4a929feb196dd997ccf01d11f90a8cf4bd9f4b15163d88fbbbb4f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `openjdk:14-ea-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:e95696594318726b72796449687f63a7bb5cdaf4bc44236701a52abc6bbb7114
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.2 MB (256197349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:416dfe8334696357332b9a0db2faea15af85b576af1ebebdb708c0c6dfbdb0ff`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 30 Aug 2018 21:49:27 GMT
MAINTAINER Oracle Linux Product Team <ol-ovm-info_ww@oracle.com>
# Mon, 18 Nov 2019 23:05:29 GMT
ADD file:c8bbabb7270612c9e26467e961293f9b6550a7a7ad2bb07d08c08e14c8ea2961 in / 
# Mon, 18 Nov 2019 23:05:30 GMT
CMD ["/bin/bash"]
# Tue, 19 Nov 2019 04:23:39 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Tue, 19 Nov 2019 04:23:39 GMT
ENV LANG=en_US.UTF-8
# Tue, 19 Nov 2019 04:23:39 GMT
ENV JAVA_HOME=/usr/java/openjdk-14
# Tue, 19 Nov 2019 04:23:39 GMT
ENV PATH=/usr/java/openjdk-14/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Dec 2019 00:33:53 GMT
ENV JAVA_VERSION=14-ea+27
# Tue, 17 Dec 2019 00:33:53 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk14/27/GPL/openjdk-14-ea+27_linux-x64_bin.tar.gz
# Tue, 17 Dec 2019 00:33:53 GMT
ENV JAVA_SHA256=44db5f0f8c5a97ee00751fdcaf16926d045b15d8b116c5198503ed20c1f5a00d
# Tue, 17 Dec 2019 00:35:29 GMT
RUN set -eux; 		curl -fL -o /openjdk.tgz "$JAVA_URL"; 	echo "$JAVA_SHA256 */openjdk.tgz" | sha256sum -c -; 	mkdir -p "$JAVA_HOME"; 	tar --extract --file /openjdk.tgz --directory "$JAVA_HOME" --strip-components 1; 	rm /openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		java --version; 	javac --version
# Tue, 17 Dec 2019 00:35:29 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:977461c903012ec41b22a4c1bf975a3199570bd92ccc75a70f5a1119bca6d402`  
		Last Modified: Mon, 18 Nov 2019 23:06:50 GMT  
		Size: 42.7 MB (42712648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b03bc4978d77c248161b19b002c5b1814492890df489738fda21ebfadf7867e`  
		Last Modified: Tue, 19 Nov 2019 04:26:37 GMT  
		Size: 14.8 MB (14789460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:954790b6c589951d95892e09520c07c681ac6115b563a65a896d8aac35cb257a`  
		Last Modified: Tue, 17 Dec 2019 00:38:04 GMT  
		Size: 198.7 MB (198695241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
