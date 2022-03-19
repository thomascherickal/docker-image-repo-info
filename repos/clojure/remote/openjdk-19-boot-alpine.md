## `clojure:openjdk-19-boot-alpine`

```console
$ docker pull clojure@sha256:7d30542e189f8cfce88db08f9e67afb69906eca4320f406f5d5ba8de2fc9aa64
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:openjdk-19-boot-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:933d8118b13c1adbc11003c85f3de3ea199a5108818d9feceb7f11df0b01d0ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.0 MB (253976225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abb6c60ddd2bb83f07fe4b8f74cd7857d8bffe17932705e5ee67c73ae408ddac`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

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
# Sat, 19 Mar 2022 11:13:58 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 19 Mar 2022 11:13:58 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 19 Mar 2022 11:13:58 GMT
WORKDIR /tmp
# Sat, 19 Mar 2022 11:14:01 GMT
RUN apk add --no-cache bash openssl && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apk del openssl
# Sat, 19 Mar 2022 11:14:01 GMT
ENV PATH=/opt/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 19 Mar 2022 11:14:01 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 19 Mar 2022 11:14:28 GMT
RUN boot
# Sat, 19 Mar 2022 11:14:29 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Sat, 19 Mar 2022 11:14:29 GMT
ENTRYPOINT ["entrypoint"]
# Sat, 19 Mar 2022 11:14:29 GMT
CMD ["repl"]
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
	-	`sha256:89443818f06959cde1b706c4fff30c94074bc6b641edb7f43a5a928ac98f2538`  
		Last Modified: Sat, 19 Mar 2022 11:33:56 GMT  
		Size: 831.3 KB (831325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16c94b012904926f780cdf8a38be4e002ab333932454274d7db6f981abf9e98`  
		Last Modified: Sat, 19 Mar 2022 11:33:59 GMT  
		Size: 58.8 MB (58820465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3e8c0cfca055c0182c7dde2de217919359e1d351aade64fd666e94c3827f0b`  
		Last Modified: Sat, 19 Mar 2022 11:33:56 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
