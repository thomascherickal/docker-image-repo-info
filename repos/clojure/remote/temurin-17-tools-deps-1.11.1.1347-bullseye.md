## `clojure:temurin-17-tools-deps-1.11.1.1347-bullseye`

```console
$ docker pull clojure@sha256:1d6a31f7689f1c6ae5df327d799de61b0efef00cf988f67a7c69ce4ff5f0a27c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-tools-deps-1.11.1.1347-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:fab84715ddad7d3050cce3c557d1c574d4579e098ae1c0c2b59f42e3017ebde8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **319.5 MB (319518813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f75e1ec5742e8b0f5cad5d2de5ee6f8b1a5edec585ea42df9bcb288f252febf5`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:54 GMT
ADD file:e530b0563ea53d97b2f28e62149a665900196f86611df99a88c7a8ab2097b95d in / 
# Mon, 12 Jun 2023 23:20:54 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:43:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 03:49:42 GMT
COPY dir:3373f6afb162f98a7f4cbaf8f00acdb618287ff4fa7a1aab9b85d36a1c441565 in /opt/java/openjdk 
# Tue, 13 Jun 2023 03:49:44 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 03:51:44 GMT
ENV CLOJURE_VERSION=1.11.1.1347
# Tue, 13 Jun 2023 03:51:44 GMT
WORKDIR /tmp
# Tue, 13 Jun 2023 03:52:01 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "d9158bf3a1d92fbf8551656e47a86f42e93d10f1db9defa2124bfee206ce8c8f *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 13 Jun 2023 03:52:02 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 13 Jun 2023 03:52:02 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Tue, 13 Jun 2023 03:52:02 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 13 Jun 2023 03:52:02 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:93c2d578e4211e82e47e7ada9ed05d1869a2362c6f7509f2ee8d91ccebfb7fbd`  
		Last Modified: Mon, 12 Jun 2023 23:26:08 GMT  
		Size: 55.1 MB (55055162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d42f641d3e7c6f97669559265ce43b9d70845285e59b903d626111efdf96ff`  
		Last Modified: Tue, 13 Jun 2023 03:58:44 GMT  
		Size: 192.6 MB (192580397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d6fd78697ecb51641c0a92e4e8fd7db8423a10a6ea61ca7b92892f762b5e60`  
		Last Modified: Tue, 13 Jun 2023 03:59:48 GMT  
		Size: 71.9 MB (71882242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02d09b44af2f057f349f645daefc5d63792f3835af11ec27ec409298399636e`  
		Last Modified: Tue, 13 Jun 2023 03:59:40 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3caac5194d9753deca19d997d956798c41cc7eb34308a0a72fd1604726a25c19`  
		Last Modified: Tue, 13 Jun 2023 03:59:40 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-tools-deps-1.11.1.1347-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:280f926af93896137eaa325e08d15baddcb3ddb6ff8ce9e8cabcd116012d8926
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.1 MB (317090029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4823df93f81b110a1748355325688d3ff177ba53b7d624b1d0148f63f569615e`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:22 GMT
ADD file:caddd2f40296ec5c1bf7487617ca8694cfff9a1d9b7484159e203b6514cb5f5f in / 
# Mon, 12 Jun 2023 23:40:23 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:50:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 04:55:30 GMT
COPY dir:61701986201ad0602f1c757565ae6dd6ea34364a0201d8cacf0d9cb6de78ccff in /opt/java/openjdk 
# Tue, 13 Jun 2023 04:55:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 04:57:14 GMT
ENV CLOJURE_VERSION=1.11.1.1347
# Tue, 13 Jun 2023 04:57:14 GMT
WORKDIR /tmp
# Tue, 13 Jun 2023 04:57:28 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "d9158bf3a1d92fbf8551656e47a86f42e93d10f1db9defa2124bfee206ce8c8f *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 13 Jun 2023 04:57:28 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 13 Jun 2023 04:57:29 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Tue, 13 Jun 2023 04:57:29 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 13 Jun 2023 04:57:29 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:663ccfaf62a5d7b997bca03d1dc6d5dfff01b9e0de08d86dbea8957ea92d7d16`  
		Last Modified: Mon, 12 Jun 2023 23:44:25 GMT  
		Size: 53.7 MB (53704136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b2f5c11cf1de6e6cdfa958273d80e09d9e847bc2a31fc5ff8ab8ff58dfecc86`  
		Last Modified: Tue, 13 Jun 2023 05:03:13 GMT  
		Size: 191.4 MB (191387706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0741140c3a8872d1a0d3514bd184023336e34f6b8884f70382f27c02517cb813`  
		Last Modified: Tue, 13 Jun 2023 05:04:01 GMT  
		Size: 72.0 MB (71997174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43e33e247c30076218968d3da3062e062a2fa086a4331310a59f9012d5d1dbe`  
		Last Modified: Tue, 13 Jun 2023 05:03:55 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5120bdfd22ec3b71b373325658c51cf2c5e98190e5f21e331250ab39e588d5b`  
		Last Modified: Tue, 13 Jun 2023 05:03:55 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
