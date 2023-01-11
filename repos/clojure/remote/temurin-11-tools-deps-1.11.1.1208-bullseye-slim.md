## `clojure:temurin-11-tools-deps-1.11.1.1208-bullseye-slim`

```console
$ docker pull clojure@sha256:b5bfdbde0636ef0e21b1d85558028bad555d4b42d17a01b333cc2268045ca777
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-tools-deps-1.11.1.1208-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:85c3a6b532cc8a38e844ef900e2c1895497bf7a91366d16e306573d9c1b4733a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.3 MB (291327276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1d3c942b97cdabfd9c1ced1eba97ac8643cd6333451200b667f8cd96824060e`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:20:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 11 Jan 2023 03:23:09 GMT
COPY dir:a503569ef9354f7d11d0273f2ab0ff91f3e5c47f548dc54f07c58e44ff27a8a0 in /opt/java/openjdk 
# Wed, 11 Jan 2023 03:23:11 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 03:25:06 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Wed, 11 Jan 2023 03:25:06 GMT
WORKDIR /tmp
# Wed, 11 Jan 2023 03:25:24 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 11 Jan 2023 03:25:24 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 11 Jan 2023 03:25:24 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6154d41a3f1328e19471ffc2c51bb92391c00f8d743c0e0d90ec13704d92355f`  
		Last Modified: Wed, 11 Jan 2023 03:36:43 GMT  
		Size: 198.5 MB (198454554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943ad686ece6cd985f52636efa0c915789a39652b3377996135bec7405fd5cd9`  
		Last Modified: Wed, 11 Jan 2023 03:37:42 GMT  
		Size: 61.5 MB (61475132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3846bbc146d5cc449932e681904d3bed4d4a838f68e3b5ee07f0f4c571580fe1`  
		Last Modified: Wed, 11 Jan 2023 03:37:35 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-tools-deps-1.11.1.1208-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:4e2d42744d7d49308c96cbb724ec6c7857d96a14c87d0a898530f624258d5f34
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.8 MB (286845117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7b25fa85bf4210b96c65bf86e45ec629ebb334fe23142d6319ec10f26e5d1a4`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 11 Jan 2023 03:41:23 GMT
COPY dir:e387a3b68139ff88bdac27d5ce097fc680f3cae9fdd88c28cdd91a06f9205180 in /opt/java/openjdk 
# Wed, 11 Jan 2023 03:41:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 03:43:00 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Wed, 11 Jan 2023 03:43:00 GMT
WORKDIR /tmp
# Wed, 11 Jan 2023 03:43:14 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 11 Jan 2023 03:43:14 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 11 Jan 2023 03:43:15 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b36725901023c32b079908ac189f7af623d07d41cf568b06bb3bc24cee19a2`  
		Last Modified: Wed, 11 Jan 2023 03:52:52 GMT  
		Size: 195.2 MB (195203408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb0d7fd613165e80277484a044d6b2dd6d57d4a802f834f69105f4beeb21c57`  
		Last Modified: Wed, 11 Jan 2023 03:53:48 GMT  
		Size: 61.6 MB (61596278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18eafac19364c0d99eac5fbdcac2f9262ac5b3417e9854b5b3773d8c86eef26e`  
		Last Modified: Wed, 11 Jan 2023 03:53:41 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
