## `clojure:openjdk-17-tools-deps-1.10.3.814-alpine`

```console
$ docker pull clojure@sha256:82ef07334b6c262cb2084e88dc15d79b75d146e0a263053e5bc3871daba9ba02
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-17-tools-deps-1.10.3.814-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:55a33dc2f5169a8a9afb4e76563d9539a42f7310cef079098720691c313e7ff4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.9 MB (208947726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92f09940b667de26687b7d3356fcf4382121ab2ccb64f3214917b95f3ad22094`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:32 GMT
ADD file:6b081cabb4b256ee07587d249c4989b5b679375529542b81550a65b6f19f274e in / 
# Thu, 25 Mar 2021 22:19:32 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 05:43:36 GMT
RUN apk add --no-cache java-cacerts
# Fri, 26 Mar 2021 05:43:36 GMT
ENV JAVA_HOME=/opt/openjdk-17
# Fri, 26 Mar 2021 05:43:36 GMT
ENV PATH=/opt/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 05:43:37 GMT
ENV JAVA_VERSION=17-ea+14
# Fri, 26 Mar 2021 05:43:50 GMT
RUN set -eux; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			downloadUrl='https://download.java.net/java/early_access/alpine/14/binaries/openjdk-17-ea+14_linux-x64-musl_bin.tar.gz'; 			downloadSha256='f07a1ac921333dafac1cd886ad49600ce143be7efebd32e1a02599a8a0829dd4'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/ssl/certs/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 26 Mar 2021 05:43:51 GMT
CMD ["jshell"]
# Fri, 26 Mar 2021 20:14:36 GMT
ENV CLOJURE_VERSION=1.10.3.814
# Fri, 26 Mar 2021 20:14:37 GMT
WORKDIR /tmp
# Fri, 26 Mar 2021 20:14:45 GMT
RUN apk add --update --no-cache curl bash make && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "ea4a943d32496dc2423a529b32a309f2c0365e56ba251d4a56739c5977b906a3 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apk del curl
# Fri, 26 Mar 2021 20:14:45 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
```

-	Layers:
	-	`sha256:9aae54b2144e5b2b00c610f8805128f4f86822e1e52d3714c463744a431f0f4a`  
		Last Modified: Thu, 25 Mar 2021 22:20:18 GMT  
		Size: 2.8 MB (2811681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24dcb53f37ee333acb4da15f3a4b5ffb66f4b09ce5572a4289f76c2812b07695`  
		Last Modified: Fri, 26 Mar 2021 05:51:31 GMT  
		Size: 928.4 KB (928432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2be41bd5e99b388651a581c5d5b7bd81fcdab12764553d7e30e126e19d6b5bc`  
		Last Modified: Fri, 26 Mar 2021 05:51:50 GMT  
		Size: 186.8 MB (186798158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32991acd546d89d7dab9ff9ad165ebd5a71ce5d06632e13074fea8763a64f62`  
		Last Modified: Fri, 26 Mar 2021 20:24:49 GMT  
		Size: 18.4 MB (18409455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
