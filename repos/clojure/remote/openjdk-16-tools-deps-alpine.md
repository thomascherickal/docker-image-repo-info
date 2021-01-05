## `clojure:openjdk-16-tools-deps-alpine`

```console
$ docker pull clojure@sha256:576ecaaeb4a22443b0d24e1e699afd1534ab844782574a0f15e3a34384e4a0a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-16-tools-deps-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:ad13d68be48fd9f0b73e1da739b89b6a918828db04ae06576cadaa20f7edfdf9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.6 MB (210574521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b40a8a59e84b54ec2d4427c336a763994b7df73854f7ab91910b4d1797403151`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:15:27 GMT
RUN apk add --no-cache java-cacerts
# Thu, 17 Dec 2020 13:15:27 GMT
ENV JAVA_HOME=/opt/openjdk-16
# Thu, 17 Dec 2020 13:15:28 GMT
ENV PATH=/opt/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 13:15:28 GMT
ENV JAVA_VERSION=16-ea+23
# Thu, 17 Dec 2020 13:16:13 GMT
RUN set -eux; 		arch="$(apk --print-arch)"; 	case "$arch" in 		x86_64) 			downloadUrl=https://download.java.net/java/early_access/alpine/23/binaries/openjdk-16-ea+23_linux-x64-musl_bin.tar.gz; 			downloadSha256=4e1d9054a4407e63fbb74155b247cf3926cffe9491074ace6d8a51d78dd0958d; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/ssl/certs/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 17 Dec 2020 13:16:14 GMT
CMD ["jshell"]
# Tue, 05 Jan 2021 01:24:41 GMT
ENV CLOJURE_VERSION=1.10.1.763
# Tue, 05 Jan 2021 01:24:41 GMT
WORKDIR /tmp
# Tue, 05 Jan 2021 01:24:50 GMT
RUN apk add --update --no-cache curl bash make && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "91421551872d421915c4a598741aefcc6749d3f4aafca9c08f271958e5456e2c *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apk del curl
# Tue, 05 Jan 2021 01:24:51 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e7f0194508bfdf90c2d4c810091723a528db557a8f15dc3342de6f146b13a31`  
		Last Modified: Thu, 17 Dec 2020 13:21:09 GMT  
		Size: 927.2 KB (927220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d12c6ae52764c63121af92fc8ae8af14d42a3a2cbbd239516e262a14c7aca7ac`  
		Last Modified: Thu, 17 Dec 2020 13:21:43 GMT  
		Size: 184.3 MB (184293978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533873451e5725de22fabae2bf8a9e85e3c7fd5ed5714e47e9397112f0539c9d`  
		Last Modified: Tue, 05 Jan 2021 01:29:11 GMT  
		Size: 22.6 MB (22554257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
