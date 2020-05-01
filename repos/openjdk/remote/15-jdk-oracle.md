## `openjdk:15-jdk-oracle`

```console
$ docker pull openjdk@sha256:54a23b960914e33edbb0e9819cd1637bbc7257d6e932190792139473006dcb49
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `openjdk:15-jdk-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:512d214a0d560a25cb8a18e9505090fb162fae2af5dd24e282d0368b55915157
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.3 MB (250283719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56438f061fd85019dbece89d6302dd1a1636c79d3946b927fdd64717ddbc88c7`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 30 Aug 2018 21:49:27 GMT
MAINTAINER Oracle Linux Product Team <ol-ovm-info_ww@oracle.com>
# Fri, 10 Apr 2020 20:26:28 GMT
ADD file:53599f8bbed1dcb68d6fd6418597c9692c328f49a3a3864871c5237c64e00375 in / 
# Fri, 10 Apr 2020 20:26:28 GMT
CMD ["/bin/bash"]
# Fri, 10 Apr 2020 20:43:19 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Fri, 10 Apr 2020 20:43:19 GMT
ENV LANG=en_US.UTF-8
# Fri, 10 Apr 2020 20:43:19 GMT
ENV JAVA_HOME=/usr/java/openjdk-15
# Fri, 10 Apr 2020 20:43:19 GMT
ENV PATH=/usr/java/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 May 2020 00:20:09 GMT
ENV JAVA_VERSION=15-ea+21
# Fri, 01 May 2020 00:20:09 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk15/21/GPL/openjdk-15-ea+21_linux-x64_bin.tar.gz
# Fri, 01 May 2020 00:20:10 GMT
ENV JAVA_SHA256=c8ff25779035a045f1a74f21b51a7383eb5f5d78d06973d722ea259886d9da62
# Fri, 01 May 2020 00:20:23 GMT
RUN set -eux; 		curl -fL -o /openjdk.tgz "$JAVA_URL"; 	echo "$JAVA_SHA256 */openjdk.tgz" | sha256sum -c -; 	mkdir -p "$JAVA_HOME"; 	tar --extract --file /openjdk.tgz --directory "$JAVA_HOME" --strip-components 1; 	rm /openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		java --version; 	javac --version
# Fri, 01 May 2020 00:20:23 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:79ccf0f4e30fb9e8aa16b93e5123f4ebd2ebe8e0f8d21cc01956016f867ab3bf`  
		Last Modified: Fri, 10 Apr 2020 20:27:25 GMT  
		Size: 43.5 MB (43457734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ceb08e4244f41a1398e621d60c54d89e7f76991ffec77188bc98bb07e60001`  
		Last Modified: Fri, 10 Apr 2020 20:45:52 GMT  
		Size: 14.8 MB (14762210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22f41babd737499261d79cc72f80852553241a5f39aaf83ba40cae2ef3167a2a`  
		Last Modified: Fri, 01 May 2020 00:22:59 GMT  
		Size: 192.1 MB (192063775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
