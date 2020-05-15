## `openjdk:15-ea-23-jdk-oracle`

```console
$ docker pull openjdk@sha256:c6a68e3083bc59a07af2f2e526c1328dfe4b70de75f77f0d69a027a920ed5b30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `openjdk:15-ea-23-jdk-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:4d3f25f148cfeb1ecc547a71979310de88df0da5adc2c4bb046f048f0619af81
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.3 MB (250273134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddf5eaf27e749665bcf478dd16bba9ddd019c25111efa5ca1490b80c16857d36`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 30 Aug 2018 21:49:27 GMT
MAINTAINER Oracle Linux Product Team <ol-ovm-info_ww@oracle.com>
# Mon, 04 May 2020 20:20:53 GMT
ADD file:d23891d2372d6aae3d738388c74dacd92f9406083ee0c1ac0e2bfd140f92ec2b in / 
# Mon, 04 May 2020 20:20:53 GMT
CMD ["/bin/bash"]
# Mon, 04 May 2020 20:38:21 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Mon, 04 May 2020 20:38:21 GMT
ENV LANG=en_US.UTF-8
# Mon, 04 May 2020 20:38:21 GMT
ENV JAVA_HOME=/usr/java/openjdk-15
# Mon, 04 May 2020 20:38:21 GMT
ENV PATH=/usr/java/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 May 2020 20:58:26 GMT
ENV JAVA_VERSION=15-ea+23
# Fri, 15 May 2020 20:58:27 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk15/23/GPL/openjdk-15-ea+23_linux-x64_bin.tar.gz
# Fri, 15 May 2020 20:58:27 GMT
ENV JAVA_SHA256=0a3a3f2bb3005d848f9a579c46c1cb581b46d6805faf673a7c1b5a2f158cd1b0
# Fri, 15 May 2020 20:59:08 GMT
RUN set -eux; 		curl -fL -o /openjdk.tgz "$JAVA_URL"; 	echo "$JAVA_SHA256 */openjdk.tgz" | sha256sum -c -; 	mkdir -p "$JAVA_HOME"; 	tar --extract --file /openjdk.tgz --directory "$JAVA_HOME" --strip-components 1; 	rm /openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		java --version; 	javac --version
# Fri, 15 May 2020 20:59:08 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:83755823a002357171a0b229ef5769a60db47a90b624adc45f8c6b7cd1d1394f`  
		Last Modified: Mon, 04 May 2020 20:22:07 GMT  
		Size: 43.5 MB (43455265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e105caaf23acf967db67aa1f683d428603dbb51e12295bfe8f5df6a4cce8bb`  
		Last Modified: Mon, 04 May 2020 20:40:58 GMT  
		Size: 14.8 MB (14758294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d7d7b55b8f2efac94bd12a0cc4194666cee137aa0424fc4cab7ad4b3d2ddfc`  
		Last Modified: Fri, 15 May 2020 21:06:39 GMT  
		Size: 192.1 MB (192059575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
