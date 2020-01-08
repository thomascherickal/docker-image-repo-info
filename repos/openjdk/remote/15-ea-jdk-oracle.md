## `openjdk:15-ea-jdk-oracle`

```console
$ docker pull openjdk@sha256:63968c6b7161eddc610ece0cf4eff73e407c7e19fc867ec3e7b28b8c595fccc1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `openjdk:15-ea-jdk-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:96710a398cc85e638b771ebc5a2216de4cd1172ae994ed8c7fc869518d8a842f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.5 MB (256527779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a390e725540ca77d6b1a235cfb0f419e6ce672557fcda45b773710d4b14e05c`
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
# Tue, 07 Jan 2020 23:24:11 GMT
ENV JAVA_VERSION=15-ea+4
# Tue, 07 Jan 2020 23:24:12 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk15/4/GPL/openjdk-15-ea+4_linux-x64_bin.tar.gz
# Tue, 07 Jan 2020 23:24:12 GMT
ENV JAVA_SHA256=0b4b5eafea84ea2dc9892b5a5e0638fc18d8a8ae7085903af86463b8a794b525
# Tue, 07 Jan 2020 23:24:53 GMT
RUN set -eux; 		curl -fL -o /openjdk.tgz "$JAVA_URL"; 	echo "$JAVA_SHA256 */openjdk.tgz" | sha256sum -c -; 	mkdir -p "$JAVA_HOME"; 	tar --extract --file /openjdk.tgz --directory "$JAVA_HOME" --strip-components 1; 	rm /openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		java --version; 	javac --version
# Tue, 07 Jan 2020 23:24:53 GMT
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
	-	`sha256:1239c949a62dc05a4717c5d243a63814f75c9d89e3b4ea90af4dfe30a641f89f`  
		Last Modified: Tue, 07 Jan 2020 23:29:21 GMT  
		Size: 199.0 MB (199009369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
