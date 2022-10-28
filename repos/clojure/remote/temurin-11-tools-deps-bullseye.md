## `clojure:temurin-11-tools-deps-bullseye`

```console
$ docker pull clojure@sha256:26e59c89ad33ade3718d81f749fda277df372c40f4b78becceeabf2ba85c9d86
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-tools-deps-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:f0d2b145e441e9bc3af246b4857d18b0bbda5ab446b67a3f7e06aebcfde2aac1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.5 MB (300472611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8379b99663016c054c0c331aea06101ae359b16aca4a255fd73a89b3bf6b450f`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:42 GMT
ADD file:26702ba2c3e94cb21cdb3c550cf01cf848823d160f3417b559116d4c718e5df0 in / 
# Tue, 25 Oct 2022 01:43:42 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:32:27 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Oct 2022 21:49:24 GMT
COPY dir:80db6f3290e8de5c875b6f069ca1d81f6b5c9f4e34668a64373c380a024a607d in /opt/java/openjdk 
# Wed, 26 Oct 2022 21:49:26 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Oct 2022 20:36:12 GMT
ENV CLOJURE_VERSION=1.11.1.1182
# Fri, 28 Oct 2022 20:36:12 GMT
WORKDIR /tmp
# Fri, 28 Oct 2022 20:36:29 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "0e80041419bb91e142e2e8683e4dad6faf79958b603bb63b2a93bdd62c2a4f14 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 28 Oct 2022 20:36:29 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 28 Oct 2022 20:36:29 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:17c9e6141fdb3387e5a1c07d4f9b6a05ac1498e96029fa3ea55470d4504f7770`  
		Last Modified: Tue, 25 Oct 2022 01:47:28 GMT  
		Size: 55.0 MB (55046332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4b022db123128ccb656b9ae699590cbed8128c83fbb885ba312cca0b50a90c`  
		Last Modified: Wed, 26 Oct 2022 22:07:00 GMT  
		Size: 198.1 MB (198124727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ae793915d73da8181fa0552007458071b8443aa0ab5ff2ddd4e58c0862a2e1`  
		Last Modified: Fri, 28 Oct 2022 20:47:09 GMT  
		Size: 47.3 MB (47300934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083614caec91acd54956f289ef22a5402abdeb87e4aed35bb4bb1432935fb79e`  
		Last Modified: Fri, 28 Oct 2022 20:46:58 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-tools-deps-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:32682602c3ed3c509d087e303d088a60f1c0e560659584ead92db53f2aa81cd5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.9 MB (295863646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30a22fce856f34e9e338aa95502c14995607b6a8e396f47cd69873b4e727955e`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 25 Oct 2022 05:45:55 GMT
ADD file:b16745ece8ef84c028d7e9ac4bf026ac64f885d4170bfcc9d435f237144a1b99 in / 
# Tue, 25 Oct 2022 05:45:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 23:53:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Oct 2022 15:37:43 GMT
COPY dir:0c9c8c2b9cd43799d246d5824c591352650ad79f5d15544287f00c2deb1e4608 in /opt/java/openjdk 
# Wed, 26 Oct 2022 15:37:48 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Oct 2022 20:28:12 GMT
ENV CLOJURE_VERSION=1.11.1.1182
# Fri, 28 Oct 2022 20:28:12 GMT
WORKDIR /tmp
# Fri, 28 Oct 2022 20:28:24 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "0e80041419bb91e142e2e8683e4dad6faf79958b603bb63b2a93bdd62c2a4f14 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 28 Oct 2022 20:28:24 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 28 Oct 2022 20:28:24 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:8e1d92e7d04d2a9a9880cb45dc3c32c2805912cd86abed96d0ada3ff28748205`  
		Last Modified: Tue, 25 Oct 2022 05:48:40 GMT  
		Size: 53.7 MB (53701966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c7a7b51e23fc2e53d8018b07b36bae7b1c261267f2981e18b50be0d7b845881`  
		Last Modified: Wed, 26 Oct 2022 15:57:42 GMT  
		Size: 194.9 MB (194866970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cdb15bdd7e4933aed1c9016f5c222dcb7499ce2d426b52e8046986f798eee3c`  
		Last Modified: Fri, 28 Oct 2022 20:36:20 GMT  
		Size: 47.3 MB (47294092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:175d358e52626595acdd8b14706f676b821c283b36ec52c491b26cf339a55236`  
		Last Modified: Fri, 28 Oct 2022 20:36:15 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
