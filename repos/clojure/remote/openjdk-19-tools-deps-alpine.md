## `clojure:openjdk-19-tools-deps-alpine`

```console
$ docker pull clojure@sha256:7cc63a28dc8a8345a3c1db0ffda9320c7e5fc0d4a25d111468138d8364c2900b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:openjdk-19-tools-deps-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:7b602d4dc984c958d8a8776fa1d82af2afa2620288010cab6d4df98f56eaaa99
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.7 MB (223743298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a9da16eab16107b08c4d7daeb3f5cfed5c4b6b426da82b1d47dee2b15ad4726`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Thu, 17 Mar 2022 04:01:58 GMT
ADD file:cf4b631a115c2bbfbd81cad2d3041bceb64a8136aac92ba8a63b6c51d60af764 in / 
# Thu, 17 Mar 2022 04:01:59 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 18:09:32 GMT
RUN apk add --no-cache java-cacerts
# Thu, 17 Mar 2022 18:09:32 GMT
ENV JAVA_HOME=/opt/openjdk-19
# Thu, 17 Mar 2022 18:09:32 GMT
ENV PATH=/opt/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Mar 2022 18:09:32 GMT
ENV JAVA_VERSION=19-ea+5
# Thu, 17 Mar 2022 18:09:44 GMT
RUN set -eux; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			downloadUrl='https://download.java.net/java/early_access/alpine/5/binaries/openjdk-19-ea+5_linux-x64-musl_bin.tar.gz'; 			downloadSha256='0ee67a41fe97341f131bd4f065ed6092d55c15de5f00f8ba1e57d21eefb2c787'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/ssl/certs/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 17 Mar 2022 18:09:45 GMT
CMD ["jshell"]
# Sat, 19 Mar 2022 11:14:32 GMT
ENV CLOJURE_VERSION=1.10.3.1087
# Sat, 19 Mar 2022 11:14:32 GMT
WORKDIR /tmp
# Sat, 19 Mar 2022 11:14:38 GMT
RUN apk add --no-cache curl bash make git && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "fd3d465ac30095157ce754f1551b840008a6e3503ce5023d042d0490f7bafb98 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apk del curl
# Sat, 19 Mar 2022 11:14:38 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Sat, 19 Mar 2022 11:14:39 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Sat, 19 Mar 2022 11:14:39 GMT
ENTRYPOINT ["entrypoint"]
# Sat, 19 Mar 2022 11:14:39 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:3d243047344378e9b7136d552d48feb7ea8b6fe14ce0990e0cc011d5e369626a`  
		Last Modified: Thu, 17 Mar 2022 04:02:41 GMT  
		Size: 2.8 MB (2812636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95bfa6190a5f1e660dfa661cfeacb195395e181263c1cccbc3920ee6ca80bbd`  
		Last Modified: Thu, 17 Mar 2022 18:26:15 GMT  
		Size: 918.6 KB (918586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79afb24595e792b2b9730c2c5afe2d3318709911a025123e55d49e217ce392f1`  
		Last Modified: Thu, 17 Mar 2022 18:26:30 GMT  
		Size: 190.6 MB (190592804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aaef25c4329b3307db066410477436dd37d077978b3b5ede49d6f527330e3a6`  
		Last Modified: Sat, 19 Mar 2022 11:34:11 GMT  
		Size: 29.4 MB (29418244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31428bfbc64ba45ca0f359e53b6a34566aff1541e6bb3b99056b2611e65e240`  
		Last Modified: Sat, 19 Mar 2022 11:34:09 GMT  
		Size: 624.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7298e26385743123cfaf63ae3810c3674cea3b94967f3e37e744e1e7da5a9733`  
		Last Modified: Sat, 19 Mar 2022 11:34:09 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
