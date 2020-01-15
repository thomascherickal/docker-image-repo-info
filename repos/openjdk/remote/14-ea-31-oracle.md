## `openjdk:14-ea-31-oracle`

```console
$ docker pull openjdk@sha256:6788fbf1a46cadd016049296acf935242d3e25516417d8b059179a4df4be546d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `openjdk:14-ea-31-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:ea6dd1d242a73825fbe70de44f970cdad0d885c5d6fe6d0332e7f5a3a8033227
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.5 MB (256545519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:377de9a7b528be70903c9a39b64107260e1fdeb66ef12a055b545982de7e657a`
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
# Fri, 20 Dec 2019 02:06:57 GMT
ENV JAVA_HOME=/usr/java/openjdk-14
# Fri, 20 Dec 2019 02:06:57 GMT
ENV PATH=/usr/java/openjdk-14/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 15 Jan 2020 21:26:32 GMT
ENV JAVA_VERSION=14-ea+31
# Wed, 15 Jan 2020 21:26:32 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk14/31/GPL/openjdk-14-ea+31_linux-x64_bin.tar.gz
# Wed, 15 Jan 2020 21:26:32 GMT
ENV JAVA_SHA256=4c77b7d01ed49aa787df11034df7270ed4bc755a79f0850711db7b5920f9d582
# Wed, 15 Jan 2020 21:27:12 GMT
RUN set -eux; 		curl -fL -o /openjdk.tgz "$JAVA_URL"; 	echo "$JAVA_SHA256 */openjdk.tgz" | sha256sum -c -; 	mkdir -p "$JAVA_HOME"; 	tar --extract --file /openjdk.tgz --directory "$JAVA_HOME" --strip-components 1; 	rm /openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		java --version; 	javac --version
# Wed, 15 Jan 2020 21:27:13 GMT
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
	-	`sha256:97a92770413d2aae4467b5c9ad150349d1108f59dc492c03139c484b57766e77`  
		Last Modified: Wed, 15 Jan 2020 21:32:30 GMT  
		Size: 199.0 MB (199027109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
