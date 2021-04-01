## `openjdk:17-alpine3.13`

```console
$ docker pull openjdk@sha256:a5ab5d012d46a26ea887f01a8149fc52034a3b4dc8ee12c15910a9cfdaf78a8a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `openjdk:17-alpine3.13` - linux; amd64

```console
$ docker pull openjdk@sha256:f1fd6bfcd92e97e1e827cbb3d7552b3608198d9ee89ad08a779e7b9eede27db6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.5 MB (190538029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bfbf45a2659af73c4811ec5d60d37636057b1209086db6aa3a97f2219d06649`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 01:15:06 GMT
RUN apk add --no-cache java-cacerts
# Thu, 01 Apr 2021 01:15:07 GMT
ENV JAVA_HOME=/opt/openjdk-17
# Thu, 01 Apr 2021 01:15:07 GMT
ENV PATH=/opt/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 01:15:07 GMT
ENV JAVA_VERSION=17-ea+14
# Thu, 01 Apr 2021 01:15:19 GMT
RUN set -eux; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			downloadUrl='https://download.java.net/java/early_access/alpine/14/binaries/openjdk-17-ea+14_linux-x64-musl_bin.tar.gz'; 			downloadSha256='f07a1ac921333dafac1cd886ad49600ce143be7efebd32e1a02599a8a0829dd4'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/ssl/certs/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 01 Apr 2021 01:15:20 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c0977514f1a113de97ffc6f5e9fd1873b8d77fb352205316fdc4d7696aab84`  
		Last Modified: Thu, 01 Apr 2021 01:21:03 GMT  
		Size: 928.4 KB (928397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:563752cd6ffc7ae1632f28e21155f16c5b95902be182e29ba84e415f794f40c1`  
		Last Modified: Thu, 01 Apr 2021 01:21:19 GMT  
		Size: 186.8 MB (186797685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
