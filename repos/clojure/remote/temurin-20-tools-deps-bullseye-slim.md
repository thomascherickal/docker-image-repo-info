## `clojure:temurin-20-tools-deps-bullseye-slim`

```console
$ docker pull clojure@sha256:cb9cf81ad6a203fc7e625b2037e83e8010c204fb4239f5377d52b6430ed611e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-20-tools-deps-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:a0e7b150885b223dcc2cdb53e9807d1689b4ebcdc88070ae192ce9f4e9f61bad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.7 MB (246711686 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c33fe41b73e72a88c60466813b8c3667b0adcfe1b1ecc861d481c2ea81848b3`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:07 GMT
ADD file:3d726bf0abbc08d6dda026cc406cdfb529deb60071641d164de28fcd62d1c1c0 in / 
# Thu, 27 Jul 2023 23:25:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 02:22:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 28 Jul 2023 03:25:12 GMT
COPY dir:6a540db71f2a37db361084aee8addd6817cd7c4f18237e6f852a38e98bdb4182 in /opt/java/openjdk 
# Fri, 28 Jul 2023 03:25:14 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 14 Aug 2023 23:26:24 GMT
ENV CLOJURE_VERSION=1.11.1.1386
# Mon, 14 Aug 2023 23:26:24 GMT
WORKDIR /tmp
# Mon, 14 Aug 2023 23:26:40 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "3a09e2df4d3abd89b5b1286af0133a36a525ff3acfe1432f98b5c24b170940e8 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Mon, 14 Aug 2023 23:26:40 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Mon, 14 Aug 2023 23:26:40 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Mon, 14 Aug 2023 23:26:40 GMT
ENTRYPOINT ["entrypoint"]
# Mon, 14 Aug 2023 23:26:40 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:1d5252f66ea9b661aceca1027b3d7ca259a50608261a25b51148119ecf086932`  
		Last Modified: Thu, 27 Jul 2023 23:30:08 GMT  
		Size: 31.4 MB (31417602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84c67718933687b640164431cd0c9539313b83f6b7a7e4892cf84a054afbd29b`  
		Last Modified: Fri, 28 Jul 2023 03:33:30 GMT  
		Size: 153.8 MB (153791720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d93657f16210118b4e7a36d72abfa63d95449351cdf1931ae9aeab8a55d5f8`  
		Last Modified: Mon, 14 Aug 2023 23:34:35 GMT  
		Size: 61.5 MB (61501345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b990ff1e5dfeb39d85d2d978541834710825196403cf7f3fd6c276dcd4147cc`  
		Last Modified: Mon, 14 Aug 2023 23:34:28 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6889efe091e12039dbd1615307957a95eeb8c87eae89112cfe2172d7024f987a`  
		Last Modified: Mon, 14 Aug 2023 23:34:28 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-20-tools-deps-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:c40b755d6ed694f3511546f7391d13df1191d36cc9a37719868d10d0e4eb7880
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.8 MB (243798943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcfdd09c4b59e86fecca760f5d6c59ed7a3599cee52541bd97727551bb20d3e2`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:15 GMT
ADD file:085ecd2f941de953afe5513a41a37412d72cbafd982de581ebd2309b3772b51e in / 
# Thu, 27 Jul 2023 23:43:15 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 14:25:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 28 Jul 2023 14:37:53 GMT
COPY dir:d35c6357dd030960bb6081f48b2bc10afb3da11efc1525ff916214b03be70ddf in /opt/java/openjdk 
# Fri, 28 Jul 2023 14:37:57 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 14:38:37 GMT
ENV CLOJURE_VERSION=1.11.1.1347
# Fri, 28 Jul 2023 14:38:37 GMT
WORKDIR /tmp
# Fri, 28 Jul 2023 14:38:50 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "d9158bf3a1d92fbf8551656e47a86f42e93d10f1db9defa2124bfee206ce8c8f *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 28 Jul 2023 14:38:50 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 28 Jul 2023 14:38:50 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Fri, 28 Jul 2023 14:38:51 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 28 Jul 2023 14:38:51 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:795b5d192ab1819e75375fead3f2f931bd86046e3308224944f16a5ec3b97424`  
		Last Modified: Thu, 27 Jul 2023 23:47:14 GMT  
		Size: 30.1 MB (30062831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fefd21a1da6dbe7eece92d1d1806b15acefbf02477009599bae50bf6cfffdb30`  
		Last Modified: Fri, 28 Jul 2023 14:45:06 GMT  
		Size: 152.1 MB (152120007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92a16efd87274424319913dfe4fad924a4609bd1ae5e6fc645108497b12c1ef`  
		Last Modified: Fri, 28 Jul 2023 14:45:40 GMT  
		Size: 61.6 MB (61615090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a506b71dddfb691955f4e81fd59f06a0799dfaff819fee4df1838d4746cf4a7c`  
		Last Modified: Fri, 28 Jul 2023 14:45:33 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39006f1927ae40c45b000f32c9a6d40485e8cc9fb1e49fd170cd55d55f8fbc05`  
		Last Modified: Fri, 28 Jul 2023 14:45:33 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
