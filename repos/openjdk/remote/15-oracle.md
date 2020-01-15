## `openjdk:15-oracle`

```console
$ docker pull openjdk@sha256:aed8b6b6b433666e868e79c5fc9a91d2f3069d1e5e11e9b81a07f3cb553b990a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `openjdk:15-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:0fd8bdc36bc70e062632846e38e7a0f228f35b213a193d3acda6dca424c23210
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.6 MB (256565370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d9cd2c0bceaa9cff1510170416139befda920abe5f1e82a7e23d16a4239e63c`
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
# Wed, 15 Jan 2020 21:24:35 GMT
ENV JAVA_VERSION=15-ea+5
# Wed, 15 Jan 2020 21:24:35 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk15/5/GPL/openjdk-15-ea+5_linux-x64_bin.tar.gz
# Wed, 15 Jan 2020 21:24:36 GMT
ENV JAVA_SHA256=eb1dd42481ccc92d843f4e421e9b101d2c2c86336b963f89823c754b7ef3cd29
# Wed, 15 Jan 2020 21:25:19 GMT
RUN set -eux; 		curl -fL -o /openjdk.tgz "$JAVA_URL"; 	echo "$JAVA_SHA256 */openjdk.tgz" | sha256sum -c -; 	mkdir -p "$JAVA_HOME"; 	tar --extract --file /openjdk.tgz --directory "$JAVA_HOME" --strip-components 1; 	rm /openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		java --version; 	javac --version
# Wed, 15 Jan 2020 21:25:19 GMT
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
	-	`sha256:9be0b3555be0433183383eb59538e496956c70855d4f29d0dfd1cde9a627f974`  
		Last Modified: Wed, 15 Jan 2020 21:31:09 GMT  
		Size: 199.0 MB (199046960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
