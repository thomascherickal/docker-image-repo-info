## `clojure:temurin-11-tools-deps-1.11.1.1189-bullseye-slim`

```console
$ docker pull clojure@sha256:e7247e2c230ecfe5ea4b9aa50d866bc37cc480cade240e9f689965e32e205cc5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-tools-deps-1.11.1.1189-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:1e31b7e60d9ca13e1b35d3f1c5c3e61caba3d641cb2f9ec8c3ff41881fcdba53
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.0 MB (291018831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:102b31496a2d8dc2456ca71fbaba3be987031c7a2a7becd415fb299c6727ed62`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 20:11:14 GMT
COPY dir:24028fba84faa85b57bc32be14abf8fad6a4bd4db557cb5499b6d5cf38d97646 in /opt/java/openjdk 
# Wed, 02 Nov 2022 20:11:16 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Nov 2022 20:23:56 GMT
ENV CLOJURE_VERSION=1.11.1.1189
# Thu, 03 Nov 2022 20:23:56 GMT
WORKDIR /tmp
# Thu, 03 Nov 2022 20:24:14 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "1afd91b165776615eca84cce2271e5fe5d5818c55dee0f082b1304bb1464b3e8 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 03 Nov 2022 20:24:15 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 03 Nov 2022 20:24:15 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9424e0e92a9d7ac25f2f902e3550e25f0379d53b383d802d0c0a9174fddd9e5d`  
		Last Modified: Wed, 02 Nov 2022 20:24:52 GMT  
		Size: 198.1 MB (198124751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d78b8060d5a463f57bd267dd75c8f0809e173842494621dbd0d9208908ad8f59`  
		Last Modified: Thu, 03 Nov 2022 20:34:27 GMT  
		Size: 61.5 MB (61473423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84847a60ecd69a1ce5e274fb3e3bcc416ecb22849aa3d08b4eebe6a4ca696b05`  
		Last Modified: Thu, 03 Nov 2022 20:34:20 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-tools-deps-1.11.1.1189-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:0d770d75942a73b570065400b536a547ec22461bfaf563d495fc1d8ef88ff34f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.5 MB (286525140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc24d73f17881a631e94493d86c919f503dacf1d50844d88d4e1cc9f592a37ec`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 20:47:12 GMT
COPY dir:e48336735658172388295f760b71f5f10a9b7d3f960c6e4546718a38dd6452e7 in /opt/java/openjdk 
# Wed, 02 Nov 2022 20:47:16 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Nov 2022 19:45:27 GMT
ENV CLOJURE_VERSION=1.11.1.1189
# Thu, 03 Nov 2022 19:45:27 GMT
WORKDIR /tmp
# Thu, 03 Nov 2022 19:45:40 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "1afd91b165776615eca84cce2271e5fe5d5818c55dee0f082b1304bb1464b3e8 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 03 Nov 2022 19:45:41 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 03 Nov 2022 19:45:41 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc966be4bd15170671412b817450394760b037c8e5e3587768bfc3bbd123d53`  
		Last Modified: Wed, 02 Nov 2022 20:58:36 GMT  
		Size: 194.9 MB (194867681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f68c8d2829f3a4e6ff0f05ea26afd13d1c0bc695aa695e5001692f498686bf4`  
		Last Modified: Thu, 03 Nov 2022 19:53:40 GMT  
		Size: 61.6 MB (61592931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c9ef5d2283d795a6674b834cadcce3645fb602140f6307862e5edbc391f477`  
		Last Modified: Thu, 03 Nov 2022 19:53:33 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
