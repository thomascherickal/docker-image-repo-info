## `openjdk:17-ea-14-jdk-alpine`

```console
$ docker pull openjdk@sha256:046614d43907133abe5be3b9ed93c2ca7df32be308e8568d7f20e9579b718497
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `openjdk:17-ea-14-jdk-alpine` - linux; amd64

```console
$ docker pull openjdk@sha256:e87fd08bd720cf95e2ec4e932e6b24779107d9f3ef7da93a6c957fb097a1affe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.5 MB (190538271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:030f5b486428f7e23aba8606fd020a2907ff3d1f7cfdb27c4d29052c66d1428b`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:32 GMT
ADD file:6b081cabb4b256ee07587d249c4989b5b679375529542b81550a65b6f19f274e in / 
# Thu, 25 Mar 2021 22:19:32 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 05:43:36 GMT
RUN apk add --no-cache java-cacerts
# Fri, 26 Mar 2021 05:43:36 GMT
ENV JAVA_HOME=/opt/openjdk-17
# Fri, 26 Mar 2021 05:43:36 GMT
ENV PATH=/opt/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 05:43:37 GMT
ENV JAVA_VERSION=17-ea+14
# Fri, 26 Mar 2021 05:43:50 GMT
RUN set -eux; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			downloadUrl='https://download.java.net/java/early_access/alpine/14/binaries/openjdk-17-ea+14_linux-x64-musl_bin.tar.gz'; 			downloadSha256='f07a1ac921333dafac1cd886ad49600ce143be7efebd32e1a02599a8a0829dd4'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/ssl/certs/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 26 Mar 2021 05:43:51 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:9aae54b2144e5b2b00c610f8805128f4f86822e1e52d3714c463744a431f0f4a`  
		Last Modified: Thu, 25 Mar 2021 22:20:18 GMT  
		Size: 2.8 MB (2811681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24dcb53f37ee333acb4da15f3a4b5ffb66f4b09ce5572a4289f76c2812b07695`  
		Last Modified: Fri, 26 Mar 2021 05:51:31 GMT  
		Size: 928.4 KB (928432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2be41bd5e99b388651a581c5d5b7bd81fcdab12764553d7e30e126e19d6b5bc`  
		Last Modified: Fri, 26 Mar 2021 05:51:50 GMT  
		Size: 186.8 MB (186798158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
