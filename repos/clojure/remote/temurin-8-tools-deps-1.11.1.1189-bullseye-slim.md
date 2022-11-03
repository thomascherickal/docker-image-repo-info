## `clojure:temurin-8-tools-deps-1.11.1.1189-bullseye-slim`

```console
$ docker pull clojure@sha256:1b177807a554e256f8971c327a5d564dcfaad7c4b4e03bba0a4d9300186f301f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-tools-deps-1.11.1.1189-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:24b152f5f45a0e27da493a070d4fef4716e82552a278ed4b077dcb656462883d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.4 MB (196407893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8514c210a8be31350d50881d57bfb9da674fe75c7bc8b15e8505857cfc6615e`
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
# Thu, 03 Nov 2022 20:21:32 GMT
ENV CLOJURE_VERSION=1.11.1.1189
# Thu, 03 Nov 2022 20:21:32 GMT
WORKDIR /tmp
# Thu, 03 Nov 2022 20:21:51 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "1afd91b165776615eca84cce2271e5fe5d5818c55dee0f082b1304bb1464b3e8 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 03 Nov 2022 20:21:51 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 03 Nov 2022 20:21:51 GMT
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
	-	`sha256:d92204911ce82c777bc538b2724fedc7b875a6829df5b5daf3e2ca4861ee4ef2`  
		Last Modified: Thu, 03 Nov 2022 20:32:36 GMT  
		Size: 61.5 MB (61473389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5cf034bd389cd129095b39c28d96c253e07dc67afe9cf41347e13cad3691e14`  
		Last Modified: Thu, 03 Nov 2022 20:32:28 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-tools-deps-1.11.1.1189-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:287edd03a44c55ac75316396e7d651ec99b21716a6f2dc9d166b73800f623d32
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.3 MB (194271389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79dbf9ef21f5f2cc04b85c80c6d040bfe7f8508719aa2bc06f8bfe43fd836989`
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
# Thu, 03 Nov 2022 19:43:19 GMT
ENV CLOJURE_VERSION=1.11.1.1189
# Thu, 03 Nov 2022 19:43:20 GMT
WORKDIR /tmp
# Thu, 03 Nov 2022 19:43:35 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "1afd91b165776615eca84cce2271e5fe5d5818c55dee0f082b1304bb1464b3e8 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 03 Nov 2022 19:43:35 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 03 Nov 2022 19:43:35 GMT
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
	-	`sha256:72d9ff8abb6696da0b9f74ad886fa95bc7ef541bdfdb2d39f92c8d8cc0ad02e2`  
		Last Modified: Thu, 03 Nov 2022 19:52:09 GMT  
		Size: 61.6 MB (61593381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e875ff94e96a2ac1e76e590c50876bedd5542b3a50e7959e70633d33ac8c82`  
		Last Modified: Thu, 03 Nov 2022 19:52:03 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
