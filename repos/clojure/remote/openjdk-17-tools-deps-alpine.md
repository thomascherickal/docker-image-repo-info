## `clojure:openjdk-17-tools-deps-alpine`

```console
$ docker pull clojure@sha256:0988d45d7e905e6f0a3800a8bdfb7e48e78af0df91ad49b02f12cbc079785d78
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-17-tools-deps-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:2f4df88f77131d36732003ef5d6239a2a00c393e1d5f14d412e90f558de0fa02
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.3 MB (213269799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ad8e513a163d5e6832953e4327b02552a0c701d8cc9503dad5dd5ea6d64d1c0`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

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
# Mon, 22 Feb 2021 22:27:48 GMT
ENV CLOJURE_VERSION=1.10.2.790
# Mon, 22 Feb 2021 22:27:49 GMT
WORKDIR /tmp
# Mon, 22 Feb 2021 22:27:58 GMT
RUN apk add --update --no-cache curl bash make && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "53771e15b9d15f9c87b59096d098af93430f80b7fea09602b1733b1cc62fd515 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apk del curl
# Mon, 22 Feb 2021 22:27:58 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
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
	-	`sha256:babeef2aee514b8f43ef46d0deca8a267bfd95671d810a884fe615aecb9e67a6`  
		Last Modified: Mon, 22 Feb 2021 22:32:51 GMT  
		Size: 22.6 MB (22640375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
