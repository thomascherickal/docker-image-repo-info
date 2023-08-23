## `clojure:temurin-20-tools-deps-1.11.1.1405-bullseye-slim`

```console
$ docker pull clojure@sha256:36459a0a41b2abe71d86bd72f4cf63c07a23625874ae3482c4a2aba7445e45d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-20-tools-deps-1.11.1.1405-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:17c76647e5a8a7d3c9c9d72f62a6d5bfbe550db3a4c1ce69a5a6bed51f805ec6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.7 MB (246705752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43162b08285fc916bed1f24bf643ef6327af3ab1608c50cdad25af199e7d31f4`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 01:36:02 GMT
COPY dir:6a540db71f2a37db361084aee8addd6817cd7c4f18237e6f852a38e98bdb4182 in /opt/java/openjdk 
# Wed, 16 Aug 2023 01:36:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Aug 2023 20:28:37 GMT
ENV CLOJURE_VERSION=1.11.1.1405
# Wed, 23 Aug 2023 20:28:37 GMT
WORKDIR /tmp
# Wed, 23 Aug 2023 20:28:53 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "e02966d807e5fcee40d3aeee823196fd296cb97e91746f444ac8c6681731b354 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 23 Aug 2023 20:28:53 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 23 Aug 2023 20:28:53 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 23 Aug 2023 20:28:53 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 23 Aug 2023 20:28:53 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f566987b9dae8e5a20c4a3b1a42a6bdf8a8a7b88a5990e626224c1547e0050b0`  
		Last Modified: Wed, 16 Aug 2023 01:44:52 GMT  
		Size: 153.8 MB (153791733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:687b0cebcf3e41a8c630ee9b2924a3ed2c277d766e5f623e96fd9cd7b33e9c2d`  
		Last Modified: Wed, 23 Aug 2023 20:36:42 GMT  
		Size: 61.5 MB (61495321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca79fb09af9f65a8f3fd9ed46564f60913dac13b4ca6df8d05e1efe210ded38`  
		Last Modified: Wed, 23 Aug 2023 20:36:35 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bdfd910cee76e4a5cf5892ae39a1300279277e3522759921816d5a51da06e6d`  
		Last Modified: Wed, 23 Aug 2023 20:36:35 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-20-tools-deps-1.11.1.1405-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:d79266aa5fdb6fe4d615bccc708696edf94df7614c2239a74f697b5fafe78b59
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.8 MB (243796358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e0814599361842ef603a4ce2b283614edcf8c79342aff04ae788abd5537b561`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 01:53:50 GMT
COPY dir:d35c6357dd030960bb6081f48b2bc10afb3da11efc1525ff916214b03be70ddf in /opt/java/openjdk 
# Wed, 16 Aug 2023 01:53:53 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Aug 2023 19:46:44 GMT
ENV CLOJURE_VERSION=1.11.1.1405
# Wed, 23 Aug 2023 19:46:44 GMT
WORKDIR /tmp
# Wed, 23 Aug 2023 19:46:58 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "e02966d807e5fcee40d3aeee823196fd296cb97e91746f444ac8c6681731b354 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 23 Aug 2023 19:46:59 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 23 Aug 2023 19:46:59 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 23 Aug 2023 19:46:59 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 23 Aug 2023 19:46:59 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b04b4e3bfe044338b1636c6d1fe76f6e2c078f769b995d868ef50c1b27e924c`  
		Last Modified: Wed, 16 Aug 2023 02:01:19 GMT  
		Size: 152.1 MB (152120026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:229b05f4fcbc561aca869669b82997e0ac596851adac25d508c4cacef238f4fb`  
		Last Modified: Wed, 23 Aug 2023 19:53:00 GMT  
		Size: 61.6 MB (61612498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8e80e93a2efd5cf58bf98575295acf209b92eb2862a43b0b3ca8fb66bea575`  
		Last Modified: Wed, 23 Aug 2023 19:52:54 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72fbf0a1192211573ddf0becdf706b4fa10eb7dc4865a5aba0cf0760afe906c5`  
		Last Modified: Wed, 23 Aug 2023 19:52:54 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
