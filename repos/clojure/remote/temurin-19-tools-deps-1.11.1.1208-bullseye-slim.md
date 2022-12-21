## `clojure:temurin-19-tools-deps-1.11.1.1208-bullseye-slim`

```console
$ docker pull clojure@sha256:1862ace79acd12a0242eb87d45ae96032c5371bb1c3818cca43efe42600c3fa8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-tools-deps-1.11.1.1208-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:603e1338425ffcff557f4507f4a6324ff411ce77fb945dba7d2f6e0913d4bf4d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.0 MB (293984751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad0276be6e1e1eae93cad8d0058ce38937a33bbfb8bdcb0b13a8985f51721c20`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:32 GMT
ADD file:73e68ae6852c9afbb2989dc9c5b7c6668843f454b1bdcfb48658bfbc6c4af69e in / 
# Wed, 21 Dec 2022 01:20:33 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:51:06 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 21 Dec 2022 02:00:06 GMT
COPY dir:fef581854733ec7202f8c807463b9e1952aeb6c7a002719c7e54987e50ea4dcb in /opt/java/openjdk 
# Wed, 21 Dec 2022 02:00:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 21 Dec 2022 02:01:56 GMT
ENV CLOJURE_VERSION=1.11.1.1200
# Wed, 21 Dec 2022 02:01:57 GMT
WORKDIR /tmp
# Wed, 21 Dec 2022 02:02:14 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "694381cb78d44f143bdcc38657507f012ebac4009bc57cec67abef1675447878 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 21 Dec 2022 02:02:15 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 21 Dec 2022 02:02:15 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 21 Dec 2022 02:02:15 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 21 Dec 2022 02:02:15 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:3f4ca61aafcd4fc07267a105067db35c0f0ac630e1970f3cd0c7bf552780e985`  
		Last Modified: Wed, 21 Dec 2022 01:24:36 GMT  
		Size: 31.4 MB (31396943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0058afebbfddb0f61fd316c5a4af96e40c10e846cefe669fe9f41c096818b001`  
		Last Modified: Wed, 21 Dec 2022 02:11:21 GMT  
		Size: 201.1 MB (201103405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0003377b647118186bb613c2e152f6f61be834ffa4d04acd8fd5a1eb508a2a18`  
		Last Modified: Wed, 21 Dec 2022 02:12:20 GMT  
		Size: 61.5 MB (61483384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efc9cb3ce84b55e7d03b53a4a19d20456156949cefdeec77a40b5b388f1fbebe`  
		Last Modified: Wed, 21 Dec 2022 02:12:12 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f399cc963084cbf68381ef5bba8e488ae8e141fbfafc6a7775c358651700f414`  
		Last Modified: Wed, 21 Dec 2022 02:12:12 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-tools-deps-1.11.1.1208-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:2609ebf7a7d208c1bbc4bfe7c45d12a6e930fed193cd59c24c4e45d1a278d103
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.5 MB (291512901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f66cf54517f3e8e366eb5bd615a1792f7186708a1610c656d46b71e88a05b19`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:48 GMT
ADD file:3ff0cc8d111595978eb50cdba91144382ce083c400d45785d53dbb03615a4890 in / 
# Wed, 21 Dec 2022 01:39:48 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:18:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 21 Dec 2022 02:26:17 GMT
COPY dir:4138443eebfda1a2a245638d5bb568645bd34d79b66d39a3be31b5ac6b823d6d in /opt/java/openjdk 
# Wed, 21 Dec 2022 02:26:21 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 21 Dec 2022 02:27:53 GMT
ENV CLOJURE_VERSION=1.11.1.1200
# Wed, 21 Dec 2022 02:27:53 GMT
WORKDIR /tmp
# Wed, 21 Dec 2022 02:28:06 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "694381cb78d44f143bdcc38657507f012ebac4009bc57cec67abef1675447878 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 21 Dec 2022 02:28:07 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 21 Dec 2022 02:28:07 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 21 Dec 2022 02:28:07 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 21 Dec 2022 02:28:07 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:4b7f5b2a311310809ab89d92f6f71b0462722fe855d3b92c93098a528aa08791`  
		Last Modified: Wed, 21 Dec 2022 01:43:12 GMT  
		Size: 30.0 MB (30044772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b60207e0d770d0504fd11f154cc640f5bd985f35f0e8a2678ed586914b052fe2`  
		Last Modified: Wed, 21 Dec 2022 02:36:04 GMT  
		Size: 199.9 MB (199864411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8545c82f982e89fd8007a786c43facdf00f856a57b5693edfb754d45bbe030c1`  
		Last Modified: Wed, 21 Dec 2022 02:36:57 GMT  
		Size: 61.6 MB (61602699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d263dd385d3afbdfb1a00d12cdfc2373ea5d218f2645131d64f90cf5ae2a02d8`  
		Last Modified: Wed, 21 Dec 2022 02:36:51 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:728004ab5d318571caa6aaa20a0fdfbfc6083f68b87d59276a30808553c3fb43`  
		Last Modified: Wed, 21 Dec 2022 02:36:51 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
