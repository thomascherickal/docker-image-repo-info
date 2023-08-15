## `clojure:temurin-20-tools-deps-1.11.1.1386-bullseye-slim`

```console
$ docker pull clojure@sha256:6a5ae18c8c29b243c6499ec1791d825b34bdce8d2b2c4e0513f578cb8bedde2e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-20-tools-deps-1.11.1.1386-bullseye-slim` - linux; amd64

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
