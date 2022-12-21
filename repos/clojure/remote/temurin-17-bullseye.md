## `clojure:temurin-17-bullseye`

```console
$ docker pull clojure@sha256:f8ab6824c761ee3ee22b850567be781b1e5716d707a3d0af035cd2fdeefa2aef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:c25353d71787a6d561d7109aba4f7a0122a66e532ba268a641e61d83c13fb1e5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.8 MB (294767416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5210dc354959caffdac0dccacd70604b9656d0680a5a501f96a22b330f9a837`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:21 GMT
ADD file:c13b430c8699df107ffd9ea5230b92238bc037a8e1cbbe35d6ab664941d575da in / 
# Wed, 21 Dec 2022 01:20:22 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:50:07 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 21 Dec 2022 01:56:26 GMT
COPY dir:6d447c71fb5cab25c46568db16879377c790ade488ebb14a9cc6935f6b8bd709 in /opt/java/openjdk 
# Wed, 21 Dec 2022 01:56:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 21 Dec 2022 01:58:35 GMT
ENV CLOJURE_VERSION=1.11.1.1200
# Wed, 21 Dec 2022 01:58:35 GMT
WORKDIR /tmp
# Wed, 21 Dec 2022 01:58:50 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "694381cb78d44f143bdcc38657507f012ebac4009bc57cec67abef1675447878 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 21 Dec 2022 01:58:50 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 21 Dec 2022 01:58:50 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 21 Dec 2022 01:58:51 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 21 Dec 2022 01:58:51 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:32de3c850997ce03b6ff4ae8fb00b34b9d7d7f9a35bfcdb8538e22cc7b77c29d`  
		Last Modified: Wed, 21 Dec 2022 01:24:10 GMT  
		Size: 55.0 MB (55025166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b85d928f7af45063c8909fd71ef1d2934126eb27a444735b74dc4b9d177542d7`  
		Last Modified: Wed, 21 Dec 2022 02:08:49 GMT  
		Size: 192.4 MB (192431250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c302995bc4b41104cc2e5e11a646a2261449e2ea48f28d8a83425f8a8ad4f4a`  
		Last Modified: Wed, 21 Dec 2022 02:10:03 GMT  
		Size: 47.3 MB (47309984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940fa71afe48037d4dbb9e6611e39a3324b169651c8a8701ab0e4a9b9f6f1349`  
		Last Modified: Wed, 21 Dec 2022 02:09:56 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e7deddc205aee8ed4567cf4fa59e7a0879b4711da04c8462fd6dc5747f451a`  
		Last Modified: Wed, 21 Dec 2022 02:09:56 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:617eb007273fcebc469fd3925c2938a0dd26934914a7fef0e5ed5b6bc554cc25
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.2 MB (292201066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c39dfab7add6a27e44a5f83a74a0e55590142ea5c4518516e3989b7480eb46d2`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:40 GMT
ADD file:5bbdc914ec8ed60ac85293e88ee1aafc3f0290762e320fc86dc9d79fa201834e in / 
# Wed, 21 Dec 2022 01:39:41 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:18:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 21 Dec 2022 02:23:13 GMT
COPY dir:533cfee1c12b6052cd1297ebc89704c8b7da6e8016c06b0e341bcec0d4934dde in /opt/java/openjdk 
# Wed, 21 Dec 2022 02:23:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 21 Dec 2022 02:25:05 GMT
ENV CLOJURE_VERSION=1.11.1.1200
# Wed, 21 Dec 2022 02:25:05 GMT
WORKDIR /tmp
# Wed, 21 Dec 2022 02:25:17 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "694381cb78d44f143bdcc38657507f012ebac4009bc57cec67abef1675447878 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 21 Dec 2022 02:25:18 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 21 Dec 2022 02:25:18 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 21 Dec 2022 02:25:18 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 21 Dec 2022 02:25:18 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:c3e6129b48b69d14c5e7a5605e2b94003fb71aac82eac46b8689f5b8007af2c5`  
		Last Modified: Wed, 21 Dec 2022 01:42:49 GMT  
		Size: 53.7 MB (53681797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7590a9cfd73d6147f6887d3e0a5cb84fcb61c48a400fb999741e356bc525b005`  
		Last Modified: Wed, 21 Dec 2022 02:33:56 GMT  
		Size: 191.2 MB (191215202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f8b374829a591cac6609feb012b04085e79ec874bbc7e74b4ba95329334b086`  
		Last Modified: Wed, 21 Dec 2022 02:34:57 GMT  
		Size: 47.3 MB (47303052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ece8b3a3f16ae07ab2b3353dcf3eb58047db02e7784b9df0dfa036b51edc157`  
		Last Modified: Wed, 21 Dec 2022 02:34:52 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deeaa984acbea86f8ac1b92321fb6e4792b6f0009aab7285b923319a25e32dd8`  
		Last Modified: Wed, 21 Dec 2022 02:34:52 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
