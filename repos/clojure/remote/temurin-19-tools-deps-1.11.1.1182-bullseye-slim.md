## `clojure:temurin-19-tools-deps-1.11.1.1182-bullseye-slim`

```console
$ docker pull clojure@sha256:5048074185d6414bd616a8f0fde335dc8939cb01ac4f4d390844d8f291925224
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-tools-deps-1.11.1.1182-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:f7df3115604858746649d5e47d51085102aa8f5f7538af08f21bd8865881f05f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.7 MB (293737622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef1b6f47166a282c1c1ec07cdd69db5ff026b2cc266b16070838f35a32e13c9c`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 25 Oct 2022 02:43:04 GMT
COPY dir:49a4548ab030e4d26793e92b4d74537cf530961ce7b4083b8d383585c96415d5 in /opt/java/openjdk 
# Tue, 25 Oct 2022 02:43:05 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Oct 2022 20:40:42 GMT
ENV CLOJURE_VERSION=1.11.1.1182
# Fri, 28 Oct 2022 20:40:42 GMT
WORKDIR /tmp
# Fri, 28 Oct 2022 20:40:59 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "0e80041419bb91e142e2e8683e4dad6faf79958b603bb63b2a93bdd62c2a4f14 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 28 Oct 2022 20:41:00 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 28 Oct 2022 20:41:00 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Fri, 28 Oct 2022 20:41:00 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 28 Oct 2022 20:41:00 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef26e3fe67290659a7b3a065746d54031cd623809f8df384628be68ee2d54a24`  
		Last Modified: Tue, 25 Oct 2022 02:54:40 GMT  
		Size: 200.8 MB (200843786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f595ff3b5453490194bd09286f07b03a77483c573b79aa1a139c978da1d288`  
		Last Modified: Fri, 28 Oct 2022 20:51:36 GMT  
		Size: 61.5 MB (61472780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dad7fd52df28d1599e3079d655356804b744df6228b4b0398fcea5401b56c98`  
		Last Modified: Fri, 28 Oct 2022 20:51:28 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01179e29f671afeee7e5a2155659eabc78f2be0a5f1e59dddfa4293297d1ab7c`  
		Last Modified: Fri, 28 Oct 2022 20:51:28 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-tools-deps-1.11.1.1182-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:a1f39fed9658b13c76717e13c0cf90f33bd98ba7e72c94fe900472d495b58fe4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.2 MB (291240076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a06dc0c74bf07203cd801f2a5112ba384c90ede00b85d1360bae33377d13939c`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Oct 2022 15:49:24 GMT
COPY dir:2fc3a52010e404362374a6fbc2449d1ef85a3bc7bb00efe969cabc1864797789 in /opt/java/openjdk 
# Wed, 26 Oct 2022 15:49:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Oct 2022 20:31:20 GMT
ENV CLOJURE_VERSION=1.11.1.1182
# Fri, 28 Oct 2022 20:31:20 GMT
WORKDIR /tmp
# Fri, 28 Oct 2022 20:31:34 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "0e80041419bb91e142e2e8683e4dad6faf79958b603bb63b2a93bdd62c2a4f14 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 28 Oct 2022 20:31:35 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 28 Oct 2022 20:31:35 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Fri, 28 Oct 2022 20:31:35 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 28 Oct 2022 20:31:35 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0786999deff23ea2618e481d077c8e627d22cb087604cb4be63e8e3940eac2be`  
		Last Modified: Wed, 26 Oct 2022 16:05:46 GMT  
		Size: 199.6 MB (199582448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274eb7e6bb2e681bb75df9222b3e13325da29694e75545d670f82797ec487dd8`  
		Last Modified: Fri, 28 Oct 2022 20:39:53 GMT  
		Size: 61.6 MB (61592702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5dfdd3b7c7724288614d5155f03485cf5b92ed6a510afbd42ed2cd778d4fd16`  
		Last Modified: Fri, 28 Oct 2022 20:39:47 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61fd5ee2f2cfaf019fab42a2f053610f8f5bb492d78c5ff04a1b3edf514318ae`  
		Last Modified: Fri, 28 Oct 2022 20:39:47 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
