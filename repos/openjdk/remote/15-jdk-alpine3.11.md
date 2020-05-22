## `openjdk:15-jdk-alpine3.11`

```console
$ docker pull openjdk@sha256:a2d0a9280a56be7217fd7e3ab6a1bc3bfb5b25ba9b69ec2c745918dd777a7616
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `openjdk:15-jdk-alpine3.11` - linux; amd64

```console
$ docker pull openjdk@sha256:628555b203e1cef4f57130ee47d7283bf7985c933da82071e7ef5af78ad986cb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.7 MB (202690807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3712e79ade7548861a907fe1abdba21819c44e9181a7aa67fa2f8665679ab4b`
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
# Fri, 22 May 2020 01:23:07 GMT
RUN set -eux; 		wget -O /openjdk.tgz "$JAVA_URL"; 	echo "$JAVA_SHA256 */openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract --file /openjdk.tgz --directory "$JAVA_HOME" --strip-components 1; 	rm /openjdk.tgz; 		java -Xshare:dump; 		java --version; 	javac --version
# Fri, 22 May 2020 01:23:07 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f63f940b2b97f71dd63758ea307855eda42b2ad6ad589e300590ccbc4d456b2`  
		Last Modified: Fri, 22 May 2020 01:27:30 GMT  
		Size: 199.9 MB (199877491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
