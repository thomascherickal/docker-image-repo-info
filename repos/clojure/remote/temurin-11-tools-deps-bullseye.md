## `clojure:temurin-11-tools-deps-bullseye`

```console
$ docker pull clojure@sha256:cd53f1f7545f2339acb56fb0f62c93257a3d65c3e4ed0327541af9a4288eb731
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-tools-deps-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:05c1af12fa3a2a065d3907979248bb15859c4d3dea10387b9bd832f21de8d813
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.8 MB (271768940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5726d8b250c8ac374a02b6b27bb269e73c44b089ff3ee28c728d49daf86d07c9`
-	Default Command: `["clj"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:55 GMT
ADD file:b493776b6d91132ce50735e2d82076620774a1e0a690cf96777ddd6b85f513ef in / 
# Thu, 27 Jul 2023 23:24:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:13:47 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 28 Jul 2023 03:17:02 GMT
COPY dir:2fc258758bb2c25982e4c8348cffe5a1ab54f4c54e52ff852a817cdf5bd62215 in /opt/java/openjdk 
# Fri, 28 Jul 2023 03:17:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 03:18:57 GMT
ENV CLOJURE_VERSION=1.11.1.1347
# Fri, 28 Jul 2023 03:18:57 GMT
WORKDIR /tmp
# Fri, 28 Jul 2023 03:19:14 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "d9158bf3a1d92fbf8551656e47a86f42e93d10f1db9defa2124bfee206ce8c8f *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 28 Jul 2023 03:19:14 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 28 Jul 2023 03:19:14 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:9a9e034800a1747ea288f38f6087c036acac99dd3ec5255bf7798abd8c23a304`  
		Last Modified: Thu, 27 Jul 2023 23:29:45 GMT  
		Size: 55.1 MB (55055571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df166fc4715d337f554c5b6904774af766db5e850d3500e12eeafae147f25b5`  
		Last Modified: Fri, 28 Jul 2023 03:29:39 GMT  
		Size: 144.8 MB (144829492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f65b65319ddeca542a2da0a84840d6521dd62491e8e26fcb2d527c99072da8`  
		Last Modified: Fri, 28 Jul 2023 03:30:36 GMT  
		Size: 71.9 MB (71883260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9a3642a7cab9932873e2e24f58452b893739d8085707ff68ae4d6d4923891c`  
		Last Modified: Fri, 28 Jul 2023 03:30:29 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-tools-deps-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:a195615079f32132f79c09fe431160a409b503a81f53f46e922d12f5db5b0d55
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.3 MB (267271849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d322c3b40c063acc69f61a57e7ac7a66077dac364a08f3a5c5042d49868a706`
-	Default Command: `["clj"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:07 GMT
ADD file:a0144d077c2c6b73bbb5f7e7b8e6b58e4127de2a5faf907cd4e83e4d83437fad in / 
# Thu, 27 Jul 2023 23:43:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 14:29:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 08 Aug 2023 20:20:57 GMT
COPY dir:ddfd64e7bd36f630cd100cf454a9685f9fd0f9483467dbf7a4c9a71ab0af7089 in /opt/java/openjdk 
# Tue, 08 Aug 2023 20:21:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 20:26:20 GMT
ENV CLOJURE_VERSION=1.11.1.1347
# Tue, 08 Aug 2023 20:26:20 GMT
WORKDIR /tmp
# Tue, 08 Aug 2023 20:26:36 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "d9158bf3a1d92fbf8551656e47a86f42e93d10f1db9defa2124bfee206ce8c8f *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 08 Aug 2023 20:26:36 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 08 Aug 2023 20:26:36 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:49185a1a3bc353699370ac57d50a7b7234b59616b6aebde79ba6a0a0314bb107`  
		Last Modified: Thu, 27 Jul 2023 23:46:34 GMT  
		Size: 53.7 MB (53704790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407c6d757b759af4edf90fb98cce4e2d9dcbe1dbefa7c50cb1db816f3fc06be8`  
		Last Modified: Tue, 08 Aug 2023 20:32:30 GMT  
		Size: 141.6 MB (141565363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e942a60cdc72eb7d3eb5f25677dead6707d682ed40995abc689550f4cab2283`  
		Last Modified: Tue, 08 Aug 2023 20:34:17 GMT  
		Size: 72.0 MB (72001077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee60be1e884fa9f717cb865162774396017d82a83a443d1d9733bc32eb52c91`  
		Last Modified: Tue, 08 Aug 2023 20:34:11 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
