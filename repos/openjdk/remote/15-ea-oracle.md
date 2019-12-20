## `openjdk:15-ea-oracle`

```console
$ docker pull openjdk@sha256:ff049aa389c1163a1e403f3f7090ffa7d83828b68f25ce8bf32bfa9555ee639d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `openjdk:15-ea-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:33fc4ffc084e628bde818d5a1de488ba0a76bc3924e0f622a38a4f182bd988c3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.5 MB (256520066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c82b4a8b70abbb92758dee0f20c1f29d81a1e09538a00e3dd974e27d4379b32d`
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
# Fri, 20 Dec 2019 02:05:14 GMT
ENV JAVA_VERSION=15-ea+2
# Fri, 20 Dec 2019 02:05:14 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk15/2/GPL/openjdk-15-ea+2_linux-x64_bin.tar.gz
# Fri, 20 Dec 2019 02:05:14 GMT
ENV JAVA_SHA256=a329c96e555819bfd005a9fbf11e75cd180c2c4331b1d2637c071ff9276e9f69
# Fri, 20 Dec 2019 02:06:44 GMT
RUN set -eux; 		curl -fL -o /openjdk.tgz "$JAVA_URL"; 	echo "$JAVA_SHA256 */openjdk.tgz" | sha256sum -c -; 	mkdir -p "$JAVA_HOME"; 	tar --extract --file /openjdk.tgz --directory "$JAVA_HOME" --strip-components 1; 	rm /openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		java --version; 	javac --version
# Fri, 20 Dec 2019 02:06:44 GMT
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
	-	`sha256:42b352a7481516c77f482f69dcb7544d0f071d1d827675872cbf5a9bc95f0375`  
		Last Modified: Fri, 20 Dec 2019 02:11:10 GMT  
		Size: 199.0 MB (199001656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
