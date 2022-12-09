## `clojure:temurin-11-tools-deps-1.11.1.1200-bullseye`

```console
$ docker pull clojure@sha256:176f7b689bd94089a5538b262dace6621616510f1f5ad8d6ea242312878b0e8c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-tools-deps-1.11.1.1200-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:5b69a7fe226a54f96f0ce75ab4e3f949c7c630840f27c5c0a54f3ba62ceccc64
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.8 MB (300807903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9b9ae14edd10f73fd250db8f50b3ef60b71412605f04eeac5663a1528a5d281`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:41 GMT
ADD file:553d20b03d45305e58cde07e0c259421bba044155ac90b4559e5cc0b69093347 in / 
# Tue, 06 Dec 2022 01:20:41 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:48:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 06:36:17 GMT
COPY dir:a503569ef9354f7d11d0273f2ab0ff91f3e5c47f548dc54f07c58e44ff27a8a0 in /opt/java/openjdk 
# Fri, 09 Dec 2022 06:36:19 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 06:40:00 GMT
ENV CLOJURE_VERSION=1.11.1.1200
# Fri, 09 Dec 2022 06:40:00 GMT
WORKDIR /tmp
# Fri, 09 Dec 2022 06:40:18 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "694381cb78d44f143bdcc38657507f012ebac4009bc57cec67abef1675447878 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 09 Dec 2022 06:40:19 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 09 Dec 2022 06:40:19 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:f2f58072e9ed1aa1b0143341c5ee83815c00ce47548309fa240155067ab0e698`  
		Last Modified: Tue, 06 Dec 2022 01:24:48 GMT  
		Size: 55.0 MB (55041342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:561532e76f8a67e2ac0114bf68c5fcb2c640ceb1eff7b0f331d366e73f673768`  
		Last Modified: Fri, 09 Dec 2022 06:53:29 GMT  
		Size: 198.5 MB (198454561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb294724c866ac8675fbe92b0019ea93915d88a16f3547514d743b974546b527`  
		Last Modified: Fri, 09 Dec 2022 06:55:19 GMT  
		Size: 47.3 MB (47311381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7639780ea89de0e1288291310678bd8c6b3c7daa485fe841415c325b4626926e`  
		Last Modified: Fri, 09 Dec 2022 06:55:14 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-tools-deps-1.11.1.1200-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:014b712a6dd5580ea9323384cd7229ea2874f3735af1a4495a497d1d12a42d30
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.2 MB (296207203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c51b5f8af01b606c216f925ec3b745725852b1a5580524b41e6e8cad1b1c538b`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:06 GMT
ADD file:b1e7652678bbfc9556636e77d79c947ff1436888e2929f9c5c3ddb42a50c1176 in / 
# Tue, 06 Dec 2022 01:40:07 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:15 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 05:03:32 GMT
COPY dir:e387a3b68139ff88bdac27d5ce097fc680f3cae9fdd88c28cdd91a06f9205180 in /opt/java/openjdk 
# Fri, 09 Dec 2022 05:03:36 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 05:06:44 GMT
ENV CLOJURE_VERSION=1.11.1.1200
# Fri, 09 Dec 2022 05:06:44 GMT
WORKDIR /tmp
# Fri, 09 Dec 2022 05:06:58 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "694381cb78d44f143bdcc38657507f012ebac4009bc57cec67abef1675447878 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 09 Dec 2022 05:06:58 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 09 Dec 2022 05:06:58 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:4948a51a9a3f176f30ac619014f4a2da453a943244eacb53096ee9742eb7cef1`  
		Last Modified: Tue, 06 Dec 2022 01:43:33 GMT  
		Size: 53.7 MB (53699146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1dc93c936f130a0b32765e5801ad37ff3679f9461520ae91ce9b6fa4d65888`  
		Last Modified: Fri, 09 Dec 2022 05:18:13 GMT  
		Size: 195.2 MB (195203416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:075b4d93b30e03752c2c664cd5fa5343bde09c7debaf4c35f1e10297e1e9f7d0`  
		Last Modified: Fri, 09 Dec 2022 05:19:59 GMT  
		Size: 47.3 MB (47304022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679f183dae046627f9279993b7ee893f5e70576f696c87a5feae0a7d572b42ea`  
		Last Modified: Fri, 09 Dec 2022 05:19:54 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
