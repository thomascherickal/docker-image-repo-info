## `clojure:openjdk-17-tools-deps-alpine`

```console
$ docker pull clojure@sha256:16168b7683669e121448071174a20a3b488fd20360a53df3975a29b8f0f7f083
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-17-tools-deps-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:c86b927c656e01bccb886926d7c7f47870c3c96e8a7efa3cfa7fc1cdb2b6e6a7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **209.0 MB (209039209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95dbaaeaa4c91558eab62a077cb9b88ac6c02c8221763eb4960251a9a05dce8d`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Tue, 09 Mar 2021 20:57:21 GMT
RUN apk add --no-cache java-cacerts
# Tue, 09 Mar 2021 20:57:21 GMT
ENV JAVA_HOME=/opt/openjdk-17
# Tue, 09 Mar 2021 20:57:21 GMT
ENV PATH=/opt/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Mar 2021 20:57:21 GMT
ENV JAVA_VERSION=17-ea+10
# Tue, 09 Mar 2021 20:58:11 GMT
RUN set -eux; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			downloadUrl='https://download.java.net/java/early_access/alpine/10/binaries/openjdk-17-ea+10_linux-x64-musl_bin.tar.gz'; 			downloadSha256='fc3ea4225030a5df6191b6027051e705e6c34b72115dfdb36d170d735cb409d5'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/ssl/certs/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 09 Mar 2021 20:58:11 GMT
CMD ["jshell"]
# Fri, 19 Mar 2021 18:59:12 GMT
ENV CLOJURE_VERSION=1.10.3.814
# Fri, 19 Mar 2021 18:59:13 GMT
WORKDIR /tmp
# Fri, 19 Mar 2021 18:59:19 GMT
RUN apk add --update --no-cache curl bash make && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "ea4a943d32496dc2423a529b32a309f2c0365e56ba251d4a56739c5977b906a3 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apk del curl
# Fri, 19 Mar 2021 18:59:19 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b1e51638093d53268f8affa33c76d79b5f585556917511babcc02780047d7b`  
		Last Modified: Tue, 09 Mar 2021 21:11:38 GMT  
		Size: 928.4 KB (928404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fccea66d261db26595f6c615d2361af9b26994c460c6b0736185a09e1cb602a`  
		Last Modified: Tue, 09 Mar 2021 21:11:53 GMT  
		Size: 186.9 MB (186889693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9ea84cbc9eee8920640ee15cab9c4028acc1a61c1e73dd4bc50f43c2c49946`  
		Last Modified: Fri, 19 Mar 2021 19:09:51 GMT  
		Size: 18.4 MB (18409455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
