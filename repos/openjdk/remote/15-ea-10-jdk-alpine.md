## `openjdk:15-ea-10-jdk-alpine`

```console
$ docker pull openjdk@sha256:9b90446facf42e5e7f43667196e453a31c0cd72d4414c1eb992708d570686f50
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `openjdk:15-ea-10-jdk-alpine` - linux; amd64

```console
$ docker pull openjdk@sha256:b6a88dae8f4c5f9a0dd8c44f73c792cce361f8016287f670903813f74cd3f476
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.7 MB (202690715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b304e8ae762d7efa124b40d6489738a41b87cbb4e7316968d0ab3ac2cd6c8fd0`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 16:13:45 GMT
ENV JAVA_HOME=/opt/openjdk-15
# Fri, 24 Apr 2020 16:13:45 GMT
ENV PATH=/opt/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Apr 2020 16:13:45 GMT
ENV JAVA_VERSION=15-ea+10
# Fri, 24 Apr 2020 16:13:45 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/alpine/10/binaries/openjdk-15-ea+10_linux-x64-musl_bin.tar.gz
# Fri, 24 Apr 2020 16:13:46 GMT
ENV JAVA_SHA256=15a5e8002e24ed129b82bfe55ffe4bdbf3cfd0a7e5ad3399879cdd44175bfd06
# Fri, 24 Apr 2020 16:15:09 GMT
RUN set -eux; 		wget -O /openjdk.tgz "$JAVA_URL"; 	echo "$JAVA_SHA256 */openjdk.tgz" | sha256sum -c -; 	mkdir -p "$JAVA_HOME"; 	tar --extract --file /openjdk.tgz --directory "$JAVA_HOME" --strip-components 1; 	rm /openjdk.tgz; 		java -Xshare:dump; 		java --version; 	javac --version
# Fri, 24 Apr 2020 16:15:09 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58bb8816b5661a8e5f19bb5fc4b1ee1848b23c8e37642b5f1fc8bdcbfdfbaad`  
		Last Modified: Fri, 24 Apr 2020 16:17:03 GMT  
		Size: 199.9 MB (199877399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
