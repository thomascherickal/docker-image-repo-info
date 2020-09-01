## `clojure:openjdk-16-boot-alpine`

```console
$ docker pull clojure@sha256:e38550ca4d808792fbac6c0005f15dc29d6c7ec69598eb6eaa87e995cf98b94f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-16-boot-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:35005b2a725644db5e9d75c94b166e95768ff33a707906a0bd0e319811915b7b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.8 MB (260792857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75bf03ebf7ff7c71769653304fdccdaf107e434007c37584b070de2b347624a0`
-	Default Command: `["boot","repl"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Wed, 22 Jul 2020 01:05:44 GMT
RUN apk add --no-cache java-cacerts
# Wed, 22 Jul 2020 01:05:44 GMT
ENV JAVA_HOME=/opt/openjdk-16
# Wed, 22 Jul 2020 01:05:45 GMT
ENV PATH=/opt/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Jul 2020 01:05:45 GMT
ENV JAVA_VERSION=16-ea+5
# Tue, 01 Sep 2020 01:44:22 GMT
RUN set -eux; 		arch="$(apk --print-arch)"; 	case "$arch" in 		x86_64) 			downloadUrl=https://download.java.net/java/early_access/alpine/5/binaries/openjdk-16-ea+5_linux-x64-musl_bin.tar.gz; 			downloadSha256=1ec940bea148a7ececda635c209de3836fe4e6511f5d49d4248cf6d52c77aac8; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/ssl/certs/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 01 Sep 2020 01:44:22 GMT
CMD ["jshell"]
# Tue, 01 Sep 2020 21:19:22 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 01 Sep 2020 21:19:22 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 01 Sep 2020 21:19:23 GMT
WORKDIR /tmp
# Tue, 01 Sep 2020 21:19:24 GMT
RUN apk add --update --no-cache bash openssl && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apk del openssl
# Tue, 01 Sep 2020 21:19:24 GMT
ENV PATH=/opt/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 01 Sep 2020 21:19:24 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 01 Sep 2020 21:19:42 GMT
RUN boot
# Tue, 01 Sep 2020 21:19:43 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a2e4aad8c98294e53534e7aef0572d7a04cc37264f1b4b75d0878244e59c7f`  
		Last Modified: Wed, 22 Jul 2020 01:13:01 GMT  
		Size: 926.4 KB (926401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db897018b4b7f77d0385f8d927829815841e840a5c7b293a8f540a58a2420aaa`  
		Last Modified: Tue, 01 Sep 2020 01:55:28 GMT  
		Size: 197.5 MB (197456532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaaa91e2aa9279269d4fbcfa7888aeb1108dd2fdcf3df6a68bd155143d47e338`  
		Last Modified: Tue, 01 Sep 2020 21:24:19 GMT  
		Size: 792.3 KB (792331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e259dee88dde743b5f13b5479ea652ed4c9f934e4174d802e153d1bfaa26bbd`  
		Last Modified: Tue, 01 Sep 2020 21:24:23 GMT  
		Size: 58.8 MB (58820052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
