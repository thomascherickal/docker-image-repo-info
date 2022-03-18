## `openjdk:19-alpine3.14`

```console
$ docker pull openjdk@sha256:b9b75df61f4ab386b2cb269cc92236dd29ef61383ebd777ae974a40ca4552ed7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `openjdk:19-alpine3.14` - linux; amd64

```console
$ docker pull openjdk@sha256:26046cc12d70506cde24e91d3e013adfe2277ab4ee1648a6d6e007decf06cb6d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.3 MB (194322236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6996f84397f3300d0dd286275b07ce6324fefe85c2b34c8e9b979efb4b6a7c6b`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 18:09:51 GMT
RUN apk add --no-cache java-cacerts
# Thu, 17 Mar 2022 18:09:51 GMT
ENV JAVA_HOME=/opt/openjdk-19
# Thu, 17 Mar 2022 18:09:51 GMT
ENV PATH=/opt/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Mar 2022 18:09:52 GMT
ENV JAVA_VERSION=19-ea+5
# Thu, 17 Mar 2022 18:10:03 GMT
RUN set -eux; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			downloadUrl='https://download.java.net/java/early_access/alpine/5/binaries/openjdk-19-ea+5_linux-x64-musl_bin.tar.gz'; 			downloadSha256='0ee67a41fe97341f131bd4f065ed6092d55c15de5f00f8ba1e57d21eefb2c787'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/ssl/certs/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 17 Mar 2022 18:10:04 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fed9b01e8c37f6c932f4dedf1c47c7092e8e350155cf584613d7116b803ad05`  
		Last Modified: Thu, 17 Mar 2022 18:27:05 GMT  
		Size: 913.3 KB (913328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc17396c062847b3a6f2aa89252cb87262e9c983743b6f97761b7ceb7c1450b3`  
		Last Modified: Thu, 17 Mar 2022 18:27:20 GMT  
		Size: 190.6 MB (190592739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
