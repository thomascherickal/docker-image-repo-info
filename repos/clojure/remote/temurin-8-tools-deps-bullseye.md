## `clojure:temurin-8-tools-deps-bullseye`

```console
$ docker pull clojure@sha256:e4b79ad1a582bea6d11310673460a92d814e1458d0686802da371ad8c8e1baf9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-tools-deps-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:6f4672ea717672a5ad27911c1ab627beb957ba0a8514fb8cfea8e22f1795bd1c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.6 MB (181551437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca075f8580bef568657a7cd6b20bcce5a1f87a6ff83f10e564fe155447d84f61`
-	Default Command: `["clj"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:05 GMT
ADD file:b03d13d345c29f69557f410c8504e748226756d1f48e5abdb63cd40179b2640c in / 
# Thu, 09 Feb 2023 03:20:05 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:22:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:22:06 GMT
COPY dir:bbb84183d7ea38d81d8401f01e29d08935ee4c8bf6f90c6527579a1554c3bde1 in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:22:06 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 09:24:06 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Thu, 09 Feb 2023 09:24:06 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:24:24 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 09 Feb 2023 09:24:25 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 09 Feb 2023 09:24:25 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:1e4aec178e0864db93a6f97a20bde3445871a4562c1801185eca1238d3a0e80d`  
		Last Modified: Thu, 09 Feb 2023 03:24:47 GMT  
		Size: 55.0 MB (55046771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002e7af6c4fa5dcefe0cea885d5bc9ca4379383c456abb3a1ebe2728ac33a5e7`  
		Last Modified: Thu, 09 Feb 2023 09:36:44 GMT  
		Size: 54.6 MB (54635546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fffce0de5be3f140ca43219ecfb77ec28ad7f9cfc329d54e7036517fe784c61`  
		Last Modified: Thu, 09 Feb 2023 09:37:39 GMT  
		Size: 71.9 MB (71868500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2a9287b379c25bf8a885448e58c59ae4865320def7e162f9eefa611b9e1762`  
		Last Modified: Thu, 09 Feb 2023 09:37:30 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-tools-deps-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:6544044db5d79e8947b5b56defa3775384a2984f8c07d687e78d9371dfd10ea7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.4 MB (179418257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48e771055c340229ab4a8b287e9c4fc24afee7a8a29ec11850038c92a909c3ee`
-	Default Command: `["clj"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:29 GMT
ADD file:5cf2de182dac36d99ec41918889c9755f9c49c56fa0a8d0ca14040c1d8c04541 in / 
# Thu, 09 Feb 2023 03:58:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:17:51 GMT
COPY dir:b6d7e5613532d986930216de9e0fece0632e82564ce7a6a98baf63b4115f840d in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:17:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 09:20:14 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Thu, 09 Feb 2023 09:20:14 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:20:29 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 09 Feb 2023 09:20:29 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 09 Feb 2023 09:20:29 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:80dae1b9d879348c210c40024c6e90ef92677ac3515456375fcbb70bdf07b104`  
		Last Modified: Thu, 09 Feb 2023 04:02:11 GMT  
		Size: 53.7 MB (53703368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c77b7001deefab693beef32501685ba34c540df86923e1b9f608310809ebc1ce`  
		Last Modified: Thu, 09 Feb 2023 09:30:48 GMT  
		Size: 53.7 MB (53727942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b88f96cefdf988545db2be8981e1505423e30813bf68b3032e6cb05d7c026d95`  
		Last Modified: Thu, 09 Feb 2023 09:31:41 GMT  
		Size: 72.0 MB (71986330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05ccc203ebd9b0a3e2d14e535197b301bd6f9b44883c445a1c87ddf482a2449`  
		Last Modified: Thu, 09 Feb 2023 09:31:34 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
