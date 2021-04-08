## `clojure:openjdk-17-tools-deps-1.10.3.822-alpine`

```console
$ docker pull clojure@sha256:62d52e8e31c9a3d338e95d5905fe4e24d12e2fd07f933d3c8332bcaf39816ef3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-17-tools-deps-1.10.3.822-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:beb5dce06ac9ed560a565ba1906c97a1d733653c829dfc2037b1775e717db232
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.9 MB (208947474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75c6e4136a76a3ba4e3cd934646962defd175e8d34ddd49548fd03d0ef9f73b6`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

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
# Wed, 07 Apr 2021 19:25:20 GMT
ENV CLOJURE_VERSION=1.10.3.822
# Wed, 07 Apr 2021 19:25:20 GMT
WORKDIR /tmp
# Wed, 07 Apr 2021 19:25:28 GMT
RUN apk add --update --no-cache curl bash make && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "ebc820fe0e74de4bd77e6d5bd7db4a262ec1902efdf4d0553309485afcd75abf *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apk del curl
# Wed, 07 Apr 2021 19:25:28 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
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
	-	`sha256:e2e8855f0f47c10cb60cfed3cdb7128e3a1668cea3d551ac8225cd165dc29ff3`  
		Last Modified: Wed, 07 Apr 2021 19:31:32 GMT  
		Size: 18.4 MB (18409445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
