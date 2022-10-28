## `clojure:temurin-8-bullseye-slim`

```console
$ docker pull clojure@sha256:787b715cd54e6137c847151598fa8d88bf544e47853a8509170f7c297c96396f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:90e62fda2b920c7db3a2b13059b0846c7220c47f9a26bff2a826d6de6fe2c339
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.4 MB (196407337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd3d6c17c2c8f2a1a77b4dae0c113c94ed7915c30e3da27fcaf5cd5106d12278`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 25 Oct 2022 02:33:27 GMT
COPY dir:300027169ac55d8fb6f67a0995ca298d5de23ab51f3dc8e227f6e221abd3d2c3 in /opt/java/openjdk 
# Tue, 25 Oct 2022 02:33:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Oct 2022 20:34:21 GMT
ENV CLOJURE_VERSION=1.11.1.1182
# Fri, 28 Oct 2022 20:34:21 GMT
WORKDIR /tmp
# Fri, 28 Oct 2022 20:34:42 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "0e80041419bb91e142e2e8683e4dad6faf79958b603bb63b2a93bdd62c2a4f14 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 28 Oct 2022 20:34:42 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 28 Oct 2022 20:34:43 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c8fc7384965746c1eff2e3c90a689ae0048d4ae23d30592f0dd0e23c474bc5`  
		Last Modified: Tue, 25 Oct 2022 02:48:26 GMT  
		Size: 103.5 MB (103513848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758fca4f1be5b917531f02d817e209584f312a77f121f1fdf6ab870194df9c67`  
		Last Modified: Fri, 28 Oct 2022 20:45:36 GMT  
		Size: 61.5 MB (61472834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d41a5ac6b5284ebd47ce99b3a539dbfbb31bbbfc823ea27fcfb30e3a15083b`  
		Last Modified: Fri, 28 Oct 2022 20:45:28 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:423c88d6bd669fc0662a47bc0d18e6c8b8340f06cb6710172ff341b6764200aa
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.3 MB (194270622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1657e3c513cc5603ca08ce2fb4dea259b606294b11eeba10d00d7e185573b686`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 25 Oct 2022 23:53:46 GMT
COPY dir:7668b70c49687fddef57006c57f288afd02ec3ccd6cde9cbc5231ec8fb9225f1 in /opt/java/openjdk 
# Tue, 25 Oct 2022 23:53:48 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Oct 2022 20:26:37 GMT
ENV CLOJURE_VERSION=1.11.1.1182
# Fri, 28 Oct 2022 20:26:37 GMT
WORKDIR /tmp
# Fri, 28 Oct 2022 20:26:52 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "0e80041419bb91e142e2e8683e4dad6faf79958b603bb63b2a93bdd62c2a4f14 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 28 Oct 2022 20:26:52 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 28 Oct 2022 20:26:52 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ac6f2c932c449efb6a51ce32f57a8b068a89aea64c8b9c5d828f0629cf158f`  
		Last Modified: Wed, 26 Oct 2022 00:13:49 GMT  
		Size: 102.6 MB (102613480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3efdde799b5fe71d608fcac504c975415dfa1c6aa623707ce95ff8cdc23789e7`  
		Last Modified: Fri, 28 Oct 2022 20:35:11 GMT  
		Size: 61.6 MB (61592615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70007942ffb51c647acb582f7b8bafb37b02f6870684016dbd439bfdc0d4da0`  
		Last Modified: Fri, 28 Oct 2022 20:35:05 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
