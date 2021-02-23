## `clojure:openjdk-17-boot-alpine`

```console
$ docker pull clojure@sha256:812f85bdf11e9fafd958b6b2bb06981abda1971fa4cc8730d74d2711939ecf98
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-17-boot-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:f7f08e0c7b60035433e91b443275ca2144590840e6e5e28c96bd3299b74abca4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.3 MB (250277843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81b131336ad8dcb5150c7b4a5e557159ea5309b97622d17e48cb9c5f5ba92aea`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Thu, 18 Feb 2021 05:42:40 GMT
RUN apk add --no-cache java-cacerts
# Thu, 18 Feb 2021 05:42:40 GMT
ENV JAVA_HOME=/opt/openjdk-17
# Thu, 18 Feb 2021 05:42:40 GMT
ENV PATH=/opt/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Feb 2021 23:23:06 GMT
ENV JAVA_VERSION=17-ea+10
# Thu, 18 Feb 2021 23:23:53 GMT
RUN set -eux; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			downloadUrl='https://download.java.net/java/early_access/alpine/10/binaries/openjdk-17-ea+10_linux-x64-musl_bin.tar.gz'; 			downloadSha256='fc3ea4225030a5df6191b6027051e705e6c34b72115dfdb36d170d735cb409d5'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/ssl/certs/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 18 Feb 2021 23:23:53 GMT
CMD ["jshell"]
# Mon, 22 Feb 2021 22:27:23 GMT
ENV BOOT_VERSION=2.8.3
# Mon, 22 Feb 2021 22:27:23 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Mon, 22 Feb 2021 22:27:24 GMT
WORKDIR /tmp
# Mon, 22 Feb 2021 22:27:25 GMT
RUN apk add --update --no-cache bash openssl && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apk del openssl
# Mon, 22 Feb 2021 22:27:25 GMT
ENV PATH=/opt/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Mon, 22 Feb 2021 22:27:26 GMT
ENV BOOT_AS_ROOT=yes
# Mon, 22 Feb 2021 22:27:44 GMT
RUN boot
# Mon, 22 Feb 2021 22:27:44 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155cb13c45d5b09951cf0b8e75c365b37550dce6b8ca7c5532d4bd491dd8f3f6`  
		Last Modified: Thu, 18 Feb 2021 05:48:13 GMT  
		Size: 928.2 KB (928245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f816cf83573c02fcf997a8bb0bae3065810e052f3e24cd800d48eb88ebd6b9`  
		Last Modified: Thu, 18 Feb 2021 23:29:59 GMT  
		Size: 186.9 MB (186889522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649915f0ac7e4f475530b6a7ff58eecd5062bbcdb36f2457128d94af4bf0a360`  
		Last Modified: Mon, 22 Feb 2021 22:32:40 GMT  
		Size: 828.4 KB (828408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01fdaaaaf03b146d48d4fe2106838f2e4a72065484c06cdfa37a4c4875908f0`  
		Last Modified: Mon, 22 Feb 2021 22:32:44 GMT  
		Size: 58.8 MB (58820011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
