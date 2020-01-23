## `clojure:openjdk-14-tools-deps-1.10.1.502-alpine`

```console
$ docker pull clojure@sha256:d4fc37abaeb87cb3d66c7532efe538b26d06b1ee0d083a5bafc58a8a0f82ec17
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-14-tools-deps-1.10.1.502-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:11cc63c660e74ae90ab2c564bce1651e35bfffa12ba6bf5842acb1d58a50f6bd
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.5 MB (224452096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3a829ec75d97082cc602e9111e0f353ab12d07bddcc1546fecf41a44b2b9422`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 19:48:20 GMT
ENV JAVA_HOME=/opt/openjdk-14
# Mon, 21 Oct 2019 19:48:21 GMT
ENV PATH=/opt/openjdk-14/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 21 Oct 2019 19:48:21 GMT
ENV JAVA_VERSION=14-ea+15
# Mon, 21 Oct 2019 19:48:21 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/alpine/15/binaries/openjdk-14-ea+15_linux-x64-musl_bin.tar.gz
# Mon, 21 Oct 2019 19:48:21 GMT
ENV JAVA_SHA256=76091da1b6ed29788f0cf85454d23900a4134286e5feb571247e5861f618d3cd
# Mon, 21 Oct 2019 19:49:55 GMT
RUN set -eux; 		wget -O /openjdk.tgz "$JAVA_URL"; 	echo "$JAVA_SHA256 */openjdk.tgz" | sha256sum -c -; 	mkdir -p "$JAVA_HOME"; 	tar --extract --file /openjdk.tgz --directory "$JAVA_HOME" --strip-components 1; 	rm /openjdk.tgz; 		java -Xshare:dump; 		java --version; 	javac --version
# Mon, 21 Oct 2019 19:49:56 GMT
CMD ["jshell"]
# Thu, 23 Jan 2020 00:30:53 GMT
ENV CLOJURE_VERSION=1.10.1.502
# Thu, 23 Jan 2020 00:30:53 GMT
WORKDIR /tmp
# Thu, 23 Jan 2020 00:31:04 GMT
RUN apk add --update --no-cache curl bash make && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apk del curl
# Thu, 23 Jan 2020 00:31:04 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c141eadf845ae2db8859f319ed5c75bdf9b8b4e29aa9c2ed428c6be11f3e9b16`  
		Last Modified: Mon, 21 Oct 2019 19:52:12 GMT  
		Size: 198.7 MB (198727031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edecba867055a5fb6f4a12e5cca46bdeaf737d97c5e49487375d78c1eaa3e5e3`  
		Last Modified: Thu, 23 Jan 2020 00:34:26 GMT  
		Size: 22.9 MB (22937931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
