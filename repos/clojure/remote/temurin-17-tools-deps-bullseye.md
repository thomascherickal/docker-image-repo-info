## `clojure:temurin-17-tools-deps-bullseye`

```console
$ docker pull clojure@sha256:cffe772eebbfc7830ae82d86e37506e067a60d4b0f81af8d7831d9513442695f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-tools-deps-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:68bdfeb4da4a9d30c1300bbb84bc90e5cfcbb3743ab09776122c695c059cd544
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **319.4 MB (319372212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:210d5424f610fb3686af1c12f50f98248e8cbfdb4a5213863f89cb9c38418dad`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:10:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 08:16:11 GMT
COPY dir:d90c8d6564183f8aad11f93ecfb2f7e0eeff18588ff2b62d7ca3d8d30672bc2c in /opt/java/openjdk 
# Wed, 12 Apr 2023 08:16:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 17 Apr 2023 22:24:53 GMT
ENV CLOJURE_VERSION=1.11.1.1273
# Mon, 17 Apr 2023 22:24:53 GMT
WORKDIR /tmp
# Mon, 17 Apr 2023 22:25:10 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4938afe6c0690d2a6553141857742d94a7350c02b4fa57cd6a9c1b7cbe66492e *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Mon, 17 Apr 2023 22:25:10 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Mon, 17 Apr 2023 22:25:10 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Mon, 17 Apr 2023 22:25:10 GMT
ENTRYPOINT ["entrypoint"]
# Mon, 17 Apr 2023 22:25:11 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc37eb9b838f833285a35e624da1bfed81e650837c6751e8a6812e51ef22b6ba`  
		Last Modified: Wed, 12 Apr 2023 08:24:36 GMT  
		Size: 192.4 MB (192438264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439e767ed48c70883103fe2dd850ba9d5028f8e8f8d5087a2068bafb3bb86a42`  
		Last Modified: Mon, 17 Apr 2023 22:32:21 GMT  
		Size: 71.9 MB (71880192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5b79fd198079ec8d3f981ab536474a27f8569450915733137bbc5c863dea99`  
		Last Modified: Mon, 17 Apr 2023 22:32:13 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46e74f17711919414b2c041fbef7751708af27fe5ea8d8c36c93d1ddce417fd`  
		Last Modified: Mon, 17 Apr 2023 22:32:13 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-tools-deps-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:32b6253146d7d94e56d64fefbc057acf90f8174a6e5a88c44c3fa6da263a0237
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.0 MB (316963927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b740352f5c61cf7ef489e66239bb15f384c83f73ff555c8cb5019f75da6498c3`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:42 GMT
ADD file:dd3d4e5fe819950e7d01b44a29dbd790438cd722ba76198910e2597448ab0c6f in / 
# Wed, 12 Apr 2023 00:39:43 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 01:23:04 GMT
COPY dir:44544f5117ae50af040f98b1979efcc18f4c9f0c7257bfc4a37b80697337361a in /opt/java/openjdk 
# Wed, 12 Apr 2023 01:23:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 17 Apr 2023 21:43:51 GMT
ENV CLOJURE_VERSION=1.11.1.1273
# Mon, 17 Apr 2023 21:43:52 GMT
WORKDIR /tmp
# Mon, 17 Apr 2023 21:44:05 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4938afe6c0690d2a6553141857742d94a7350c02b4fa57cd6a9c1b7cbe66492e *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Mon, 17 Apr 2023 21:44:06 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Mon, 17 Apr 2023 21:44:06 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Mon, 17 Apr 2023 21:44:06 GMT
ENTRYPOINT ["entrypoint"]
# Mon, 17 Apr 2023 21:44:06 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:dc80b8cdbfd36cb20231d807a50d704945d1df4da8f6e23197ccfcb629970491`  
		Last Modified: Wed, 12 Apr 2023 00:42:14 GMT  
		Size: 53.7 MB (53705529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6911e57ac771aafcbe41270c1285de884dc5ce0d79a1b3069ec89c3a65e4a6c2`  
		Last Modified: Wed, 12 Apr 2023 01:30:58 GMT  
		Size: 191.3 MB (191260417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a826b8b9c20fd85b40fdfffe5d53389dd62387f2aee05075aa672facfe14eab`  
		Last Modified: Mon, 17 Apr 2023 21:49:34 GMT  
		Size: 72.0 MB (71996963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ac5f0d71faa1f956a55b194bc7cb7977d9e54c5b4438583f782ee286d4b191`  
		Last Modified: Mon, 17 Apr 2023 21:49:28 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466e4f8801e361df319dea02b29eaa0c0a8ca080d76a12a74cf96e7d1ff5ccc4`  
		Last Modified: Mon, 17 Apr 2023 21:49:28 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
