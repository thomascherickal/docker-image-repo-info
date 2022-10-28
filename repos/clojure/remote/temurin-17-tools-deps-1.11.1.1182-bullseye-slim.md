## `clojure:temurin-17-tools-deps-1.11.1.1182-bullseye-slim`

```console
$ docker pull clojure@sha256:5e01cfbd35540926f553114b3af3ad55d71644251b3c54a3cdcc68f6b562c361
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-tools-deps-1.11.1.1182-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:78440a1ed8e7d7fd0f09d84b491082566928558df3a2079e312478630b34f964
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.0 MB (285031398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65779f7949ee111fdc0f3066589afe2bad21d11db65a285ba2736f479d55eb69`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Oct 2022 21:55:22 GMT
COPY dir:b50a87fd6710a805ef25d6c1dd2c5f7aa37ef63d04ab1c00c91801848dae94f0 in /opt/java/openjdk 
# Wed, 26 Oct 2022 21:55:24 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Oct 2022 20:38:40 GMT
ENV CLOJURE_VERSION=1.11.1.1182
# Fri, 28 Oct 2022 20:38:40 GMT
WORKDIR /tmp
# Fri, 28 Oct 2022 20:38:58 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "0e80041419bb91e142e2e8683e4dad6faf79958b603bb63b2a93bdd62c2a4f14 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 28 Oct 2022 20:38:58 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 28 Oct 2022 20:38:58 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Fri, 28 Oct 2022 20:38:58 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 28 Oct 2022 20:38:59 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e670a3c00fcddd4db26555e9c844d563ed2f95a3a416c451f078b9d2826bd660`  
		Last Modified: Wed, 26 Oct 2022 22:11:01 GMT  
		Size: 192.1 MB (192137485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160e5ece56406d69949db95ee97d082911873672b8eb0c26a66e43694e89877f`  
		Last Modified: Fri, 28 Oct 2022 20:49:30 GMT  
		Size: 61.5 MB (61472858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f05ee03850381e0350b27aa520a3d05930983221d004d39c3e40a0ac5e7331f`  
		Last Modified: Fri, 28 Oct 2022 20:49:23 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c94a93d58b54303e98da0796237910b3402b68938ab08a66605ba9434920f3`  
		Last Modified: Fri, 28 Oct 2022 20:49:23 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-tools-deps-1.11.1.1182-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:587e05c8c3788022e38f9b283b7383d924504a54b914125b578d9bec56f9f112
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.6 MB (282561758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54d0068cb94418c33826a50a23c85da1f563baab9261fa7dbf2b8ba1b5133111`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Oct 2022 15:45:22 GMT
COPY dir:580c509aa131da1d31de9db8eed968c1f0ef93ad270f258b0b43d9d7d72bba84 in /opt/java/openjdk 
# Wed, 26 Oct 2022 15:45:26 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Oct 2022 20:29:54 GMT
ENV CLOJURE_VERSION=1.11.1.1182
# Fri, 28 Oct 2022 20:29:54 GMT
WORKDIR /tmp
# Fri, 28 Oct 2022 20:30:08 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "0e80041419bb91e142e2e8683e4dad6faf79958b603bb63b2a93bdd62c2a4f14 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 28 Oct 2022 20:30:09 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 28 Oct 2022 20:30:09 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Fri, 28 Oct 2022 20:30:09 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 28 Oct 2022 20:30:09 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5227b5452ba825facdc158312391c195512969f1ab7a485e56b2a432c2fcf433`  
		Last Modified: Wed, 26 Oct 2022 16:01:26 GMT  
		Size: 190.9 MB (190904076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee99f3c2ca95bb94a861edeaf73a7782e80b3f9f3dd995ab9974a1dec1424d90`  
		Last Modified: Fri, 28 Oct 2022 20:38:07 GMT  
		Size: 61.6 MB (61592754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1389f863ac43647abe73f9b3d35abd291aa0725db43578581161f90a4de6d0d3`  
		Last Modified: Fri, 28 Oct 2022 20:38:01 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0247f1b4cb7f034db02885ceaec75db5cffa1f9862d53f6a7ec6421bfacf70fa`  
		Last Modified: Fri, 28 Oct 2022 20:38:01 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
