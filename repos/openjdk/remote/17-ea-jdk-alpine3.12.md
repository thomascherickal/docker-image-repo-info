## `openjdk:17-ea-jdk-alpine3.12`

```console
$ docker pull openjdk@sha256:eb2d901b9cad5ae5a31f2872bd682b35c6a64c045ebeeafc8019ca6feb216afb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `openjdk:17-ea-jdk-alpine3.12` - linux; amd64

```console
$ docker pull openjdk@sha256:b1048d1265541864987443c0e699eae6c60e4e84180b52aee9fe4b9c29291e2c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.6 MB (190616210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f73edea05605f05eca203e1a15fc42d395cbcccc0a69847b86b65a16d3119e62`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 00:00:30 GMT
RUN apk add --no-cache java-cacerts
# Thu, 25 Feb 2021 00:00:30 GMT
ENV JAVA_HOME=/opt/openjdk-17
# Thu, 25 Feb 2021 00:00:30 GMT
ENV PATH=/opt/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 25 Feb 2021 00:00:31 GMT
ENV JAVA_VERSION=17-ea+10
# Thu, 25 Feb 2021 00:01:25 GMT
RUN set -eux; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			downloadUrl='https://download.java.net/java/early_access/alpine/10/binaries/openjdk-17-ea+10_linux-x64-musl_bin.tar.gz'; 			downloadSha256='fc3ea4225030a5df6191b6027051e705e6c34b72115dfdb36d170d735cb409d5'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/ssl/certs/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 25 Feb 2021 00:01:25 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b74035ed8858e7784e115e0cd6a9fbe24c0c1548320c2642c0ab15c3a9ab0d4`  
		Last Modified: Thu, 25 Feb 2021 00:07:58 GMT  
		Size: 927.2 KB (927225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe76a89d040a4b31c007a73d58b798ff3f5c14cb7c5ce1bb1971559098cf165`  
		Last Modified: Thu, 25 Feb 2021 00:08:15 GMT  
		Size: 186.9 MB (186889492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
