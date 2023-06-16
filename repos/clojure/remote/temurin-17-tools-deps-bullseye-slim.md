## `clojure:temurin-17-tools-deps-bullseye-slim`

```console
$ docker pull clojure@sha256:7016b01c66a4efe4a6491b7a67f9695dac56f5fc99c35dafcaf2b7659235af4c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-tools-deps-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:1bb9b2dbcaf4e885e6ffbf6e19f1b73a65ea8eba4a2c2b3ca8d41f061efeb7dd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.5 MB (285494741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ed56988daf34997fd79eb47a4cdfbed62e9c1647cf2f6e51362920e02d8f662`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:44:37 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 03:50:15 GMT
COPY dir:3373f6afb162f98a7f4cbaf8f00acdb618287ff4fa7a1aab9b85d36a1c441565 in /opt/java/openjdk 
# Tue, 13 Jun 2023 03:50:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 03:52:08 GMT
ENV CLOJURE_VERSION=1.11.1.1347
# Tue, 13 Jun 2023 03:52:09 GMT
WORKDIR /tmp
# Tue, 13 Jun 2023 03:52:24 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "d9158bf3a1d92fbf8551656e47a86f42e93d10f1db9defa2124bfee206ce8c8f *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 13 Jun 2023 03:52:25 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 13 Jun 2023 03:52:25 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Tue, 13 Jun 2023 03:52:25 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 13 Jun 2023 03:52:25 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bb32e3062db1c890af593910b7980b172f50d98a42b947310bdadd85c41440`  
		Last Modified: Tue, 13 Jun 2023 03:59:06 GMT  
		Size: 192.6 MB (192580388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09eb290ecd96d3c6b9106bb3ff42a9c129c38f2e32092cadbf263ec6ab3c7b44`  
		Last Modified: Tue, 13 Jun 2023 04:00:04 GMT  
		Size: 61.5 MB (61495932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a887696e32303047d99bfbd19720ea5681dd4feba62b83c331447ae58687f10f`  
		Last Modified: Tue, 13 Jun 2023 03:59:58 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c389cd1afe95e9c422118a6abb97bcfba94c85e5837838a6caeabc44d39547e`  
		Last Modified: Tue, 13 Jun 2023 03:59:58 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-tools-deps-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:ef91ca0b9e423926d459a4169ce5d4e4ae5698fd03bc0ea6c0f7ddc012e4cd6e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.1 MB (283062672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e277c931029c08c2f51384e46eca07578585b617ceec7dfa7b0b3e4de1147eda`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:28:47 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 04:47:00 GMT
COPY dir:a7888c4ea2b71681cd7f19a201b81930752c61fdfa5815ca0d4cf6337d5ee1e8 in /opt/java/openjdk 
# Fri, 16 Jun 2023 04:47:05 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 04:49:36 GMT
ENV CLOJURE_VERSION=1.11.1.1347
# Fri, 16 Jun 2023 04:49:36 GMT
WORKDIR /tmp
# Fri, 16 Jun 2023 04:49:49 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "d9158bf3a1d92fbf8551656e47a86f42e93d10f1db9defa2124bfee206ce8c8f *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 16 Jun 2023 04:49:50 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 16 Jun 2023 04:49:50 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Fri, 16 Jun 2023 04:49:50 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 16 Jun 2023 04:49:50 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:589855d0c7aebd4ca2b50aaf622d291cd44875676cdd56512b687b47b80c59ad`  
		Last Modified: Fri, 16 Jun 2023 04:57:17 GMT  
		Size: 191.4 MB (191387665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b281a5d174f779f90629853e930f60e2c290e5a49bb91d74e268f7871cd23a50`  
		Last Modified: Fri, 16 Jun 2023 04:59:14 GMT  
		Size: 61.6 MB (61611159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e08449e5fa6f24840907b5ac89e9e0372f8b14483b9f1d4e78ca6c4946d67d3`  
		Last Modified: Fri, 16 Jun 2023 04:59:08 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd019d2f239e8a2648e231cd4a02891b529cc92390e0174387106a417f7ec1e`  
		Last Modified: Fri, 16 Jun 2023 04:59:08 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
