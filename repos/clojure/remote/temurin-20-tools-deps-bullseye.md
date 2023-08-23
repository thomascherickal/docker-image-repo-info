## `clojure:temurin-20-tools-deps-bullseye`

```console
$ docker pull clojure@sha256:bcfedb437d9cdd84b30b0774ef9e2dd4c8e242e0df70babf438b1c2950d4ad0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-20-tools-deps-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:de64c110cc3fc7f0480be86c92b913205056f9aa94cc167f724c93e9609c006c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.7 MB (280729209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34983e0bbe722b4106830c224b5c5970d56e89a2464ec92945de20d1c3cca285`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:57 GMT
ADD file:20f89ff93bfbd6c9fb1a97058a1f3de4485a8974e8a83892072c511fbd2e4134 in / 
# Wed, 16 Aug 2023 00:59:58 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:06 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 01:35:34 GMT
COPY dir:6a540db71f2a37db361084aee8addd6817cd7c4f18237e6f852a38e98bdb4182 in /opt/java/openjdk 
# Wed, 16 Aug 2023 01:35:35 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Aug 2023 20:28:16 GMT
ENV CLOJURE_VERSION=1.11.1.1405
# Wed, 23 Aug 2023 20:28:16 GMT
WORKDIR /tmp
# Wed, 23 Aug 2023 20:28:32 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "e02966d807e5fcee40d3aeee823196fd296cb97e91746f444ac8c6681731b354 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 23 Aug 2023 20:28:33 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 23 Aug 2023 20:28:33 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 23 Aug 2023 20:28:33 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 23 Aug 2023 20:28:33 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:6a70103cc499a199e10e379794c60aa524d9598587cc2bdfe2995642c2da8df7`  
		Last Modified: Wed, 16 Aug 2023 01:04:50 GMT  
		Size: 55.1 MB (55056621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90caec4e7b99b48f1f89782ec874bda17eaa1c0668d0881c12015fed8413ae7c`  
		Last Modified: Wed, 16 Aug 2023 01:44:30 GMT  
		Size: 153.8 MB (153791716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa53b1db65ec1027fd1503aa009aabbfba8ca750f4ca41cef90e5e8a78b381ef`  
		Last Modified: Wed, 23 Aug 2023 20:36:24 GMT  
		Size: 71.9 MB (71879857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf1e2dfcc9e3a92bffaadca22e24fcced56a66e41c1275fcc1dea717c187b71`  
		Last Modified: Wed, 23 Aug 2023 20:36:16 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba648aa7dfcb7cd293bc0baba0db7f21943dc5750e9d7c854e5e559a5f840cd3`  
		Last Modified: Wed, 23 Aug 2023 20:36:16 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-20-tools-deps-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:a7652270d5f6e9b159fe11d5a08698e67d4bee625222dc229b346489507f6745
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.8 MB (277824581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b18c66e4e404e58f0045eb376485502ca95d3614adf01ed3f588f90d28d186ef`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:03 GMT
ADD file:8973cddb2d84a543b71001635599951bea6485a3526ae4ff916443b584864c83 in / 
# Tue, 15 Aug 2023 23:40:04 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:14 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 01:53:28 GMT
COPY dir:d35c6357dd030960bb6081f48b2bc10afb3da11efc1525ff916214b03be70ddf in /opt/java/openjdk 
# Wed, 16 Aug 2023 01:53:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Aug 2023 19:46:24 GMT
ENV CLOJURE_VERSION=1.11.1.1405
# Wed, 23 Aug 2023 19:46:24 GMT
WORKDIR /tmp
# Wed, 23 Aug 2023 19:46:38 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "e02966d807e5fcee40d3aeee823196fd296cb97e91746f444ac8c6681731b354 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 23 Aug 2023 19:46:39 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 23 Aug 2023 19:46:39 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 23 Aug 2023 19:46:39 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 23 Aug 2023 19:46:39 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:e837d9f05c625de5b814b851adbc03559ba02ea7078f57c81a01e18fc65bf42b`  
		Last Modified: Tue, 15 Aug 2023 23:43:37 GMT  
		Size: 53.7 MB (53704779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80577829fd2ca0f87088aee439e2af91b6b5d473c01321aca658e856bb10ee3f`  
		Last Modified: Wed, 16 Aug 2023 02:01:01 GMT  
		Size: 152.1 MB (152120028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f15a3b1ebd3f8f8b77b7d2f2c2a78c4c3eb35d9a833888df2cf646cacdf1221`  
		Last Modified: Wed, 23 Aug 2023 19:52:44 GMT  
		Size: 72.0 MB (71998758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d42bf326fa4bf7b2ef9f35ac59410a81b0b5941347be0b0ea017611d5d941e`  
		Last Modified: Wed, 23 Aug 2023 19:52:37 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26dac715b334a5357cbab09892b7afc7457f15c78bdc5786876ecd84ffcab5cc`  
		Last Modified: Wed, 23 Aug 2023 19:52:37 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
