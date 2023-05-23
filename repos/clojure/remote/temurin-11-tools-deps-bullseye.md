## `clojure:temurin-11-tools-deps-bullseye`

```console
$ docker pull clojure@sha256:d8810b9dfec76f0d8300dfce2e1526139b3f41edd69b19143e4fea4745343771
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-tools-deps-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:2dd59c680221987e079f9b2f0b32825406bae5d9d23c3c8b63336e541fd964e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.5 MB (325477605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f589acb2faa9fe003c36a5442e498fc507f642e66558a35c6f10bb45f40ca1b`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 02 May 2023 23:46:50 GMT
ADD file:fc290cf8ddb984325474583faa79c5a98c5ea0ec7f606bf360251f63acecf389 in / 
# Tue, 02 May 2023 23:46:51 GMT
CMD ["bash"]
# Wed, 03 May 2023 20:24:09 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 14:54:57 GMT
COPY dir:480a3269dc817a8cead3ef1e03a246c3e173090658469b19c2165cafbd3da5de in /opt/java/openjdk 
# Thu, 04 May 2023 14:54:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 19 May 2023 20:28:38 GMT
ENV CLOJURE_VERSION=1.11.1.1323
# Fri, 19 May 2023 20:28:38 GMT
WORKDIR /tmp
# Fri, 19 May 2023 20:28:55 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "c4666f0e2c2397b91554befd71ff6149b2e89acbf90400e1dcf557526cfb593d *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 19 May 2023 20:28:56 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 19 May 2023 20:28:56 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:918547b9432687b1e1d238e82dc1e0ea0b736aafbf3c402eea98c6db81a9cb65`  
		Last Modified: Tue, 02 May 2023 23:49:58 GMT  
		Size: 55.0 MB (55049070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37cf5ecc63589948ba9028f7a7ba75093cb9a0b0ec0aa545ceb047392800d2b1`  
		Last Modified: Thu, 04 May 2023 15:06:11 GMT  
		Size: 198.5 MB (198549481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab58c617e899955a2c1e40c0284ab7a5867c00bada80037d53831ab27f185748`  
		Last Modified: Fri, 19 May 2023 20:39:51 GMT  
		Size: 71.9 MB (71878436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0917b996da2c2c31a3ffce989601eea825ebaeac3b587483a34e21314eb96cdc`  
		Last Modified: Fri, 19 May 2023 20:39:43 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-tools-deps-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:05de433f303989ee081ef10b3744dce798469b5680c80aa0a41433de99eb7bb9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.0 MB (321012367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a36ac5e2d4c9b9b99ef83264cbe203caa929618283d1514354aa7f74cfcd610`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 23 May 2023 00:43:08 GMT
ADD file:a823391455122220a061ff349b66ee33413e968447ec5ba4bd544d9182fa2fbe in / 
# Tue, 23 May 2023 00:43:08 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:24:09 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 23 May 2023 01:26:55 GMT
COPY dir:377359689ec5fd1035465458ec6eb78fc3e8352f259756650a4953f3054fef1a in /opt/java/openjdk 
# Tue, 23 May 2023 01:27:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 01:28:42 GMT
ENV CLOJURE_VERSION=1.11.1.1323
# Tue, 23 May 2023 01:28:42 GMT
WORKDIR /tmp
# Tue, 23 May 2023 01:28:56 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "c4666f0e2c2397b91554befd71ff6149b2e89acbf90400e1dcf557526cfb593d *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 23 May 2023 01:28:57 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 23 May 2023 01:28:57 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:b04fae59f135dd79280e4a6da39408e04c6d703c617cbcb1c524dfe6f2962fe5`  
		Last Modified: Tue, 23 May 2023 00:45:45 GMT  
		Size: 53.7 MB (53692612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e206de1cfcbe93e5295be6e8b68ac1878120e16eb1f6a6d4211f2d2a345f1fe`  
		Last Modified: Tue, 23 May 2023 01:35:30 GMT  
		Size: 195.3 MB (195324210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2aef4f5dd05c91dc00449577b8c6db615ded50dbd6d29d774b5594fe0c5db3`  
		Last Modified: Tue, 23 May 2023 01:36:24 GMT  
		Size: 72.0 MB (71994928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c8b883aa484591596e54bc02b176e7986b76e3374c298b1ca4e73c89b7b890`  
		Last Modified: Tue, 23 May 2023 01:36:18 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
