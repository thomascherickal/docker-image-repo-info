## `openjdk:15-ea-7-jdk-oracle`

```console
$ docker pull openjdk@sha256:d69b9f91e944ced02c0b1eb72706621556b68b2695b79fdf5dc83ea4fcb8d939
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `openjdk:15-ea-7-jdk-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:bb28ad0c7f1a4b8663838b45a44a043443fee244dc1f32733c7fd59a6a576f4b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.6 MB (256613315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc1ebe4e601febf183d4a635305ef268853e7f03106bb367c18b6a43c5461a47`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 30 Aug 2018 21:49:27 GMT
MAINTAINER Oracle Linux Product Team <ol-ovm-info_ww@oracle.com>
# Fri, 20 Dec 2019 01:46:43 GMT
ADD file:e662b0d428c91ed028fec1db2cccbeddea848eb36b32c8bfad324619b8e57d9f in / 
# Fri, 20 Dec 2019 01:46:44 GMT
CMD ["/bin/bash"]
# Fri, 20 Dec 2019 02:05:13 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Fri, 20 Dec 2019 02:05:13 GMT
ENV LANG=en_US.UTF-8
# Fri, 20 Dec 2019 02:05:13 GMT
ENV JAVA_HOME=/usr/java/openjdk-15
# Fri, 20 Dec 2019 02:05:13 GMT
ENV PATH=/usr/java/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 25 Jan 2020 02:32:56 GMT
ENV JAVA_VERSION=15-ea+7
# Sat, 25 Jan 2020 02:32:56 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk15/7/GPL/openjdk-15-ea+7_linux-x64_bin.tar.gz
# Sat, 25 Jan 2020 02:32:56 GMT
ENV JAVA_SHA256=1e6dce68fd46f21334f33ab68804f7fe4d89180b03dbf4151f61af4d50674e85
# Sat, 25 Jan 2020 02:34:34 GMT
RUN set -eux; 		curl -fL -o /openjdk.tgz "$JAVA_URL"; 	echo "$JAVA_SHA256 */openjdk.tgz" | sha256sum -c -; 	mkdir -p "$JAVA_HOME"; 	tar --extract --file /openjdk.tgz --directory "$JAVA_HOME" --strip-components 1; 	rm /openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		java --version; 	javac --version
# Sat, 25 Jan 2020 02:34:35 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:822ace0353cbeeb23baa4e10b00916d8aae76c005023f5807d16cd97e6339b9b`  
		Last Modified: Fri, 20 Dec 2019 01:48:50 GMT  
		Size: 42.7 MB (42725372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf4d0631bf4e4c98ff5629cdf7958d9db134bbabd5a323f89f8fd783ca4c524`  
		Last Modified: Fri, 20 Dec 2019 02:10:52 GMT  
		Size: 14.8 MB (14793038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f76feb357590a4280781afeacf7c757904fabd2bb53c14ee6c51c9a607cbbcf6`  
		Last Modified: Sat, 25 Jan 2020 02:40:25 GMT  
		Size: 199.1 MB (199094905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
