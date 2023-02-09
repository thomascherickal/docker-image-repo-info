## `clojure:temurin-17-tools-deps-bullseye-slim`

```console
$ docker pull clojure@sha256:ee194cad7632b6688bc2ddc1d4eb6ed6f424314b064a57bd76f7575344fd98af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-tools-deps-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:37f3ea07e836f665d6d1fec4841fe6608d2d321151453b579e35ffd23f1a1524
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.3 MB (285334048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dce22434511190840d064d87b09c6c5381dba8ece54a9f1411fca0b48ea2f4d3`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:22:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:28:39 GMT
COPY dir:5cf52f938fe415b0022fbccb8cf978562c503c0b8313cc9dedf46c1c4edb35cf in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:28:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 09:30:35 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Thu, 09 Feb 2023 09:30:35 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:30:52 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 09 Feb 2023 09:30:52 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 09 Feb 2023 09:30:52 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Thu, 09 Feb 2023 09:30:53 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 09 Feb 2023 09:30:53 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c81d82cb4b2b71263b3117ae53e60d87a90991c692f5ff54bea94797fdf512`  
		Last Modified: Thu, 09 Feb 2023 09:40:40 GMT  
		Size: 192.4 MB (192438189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4435569d1e04606e66efbf96cab54a1591e44698542588da81f818f993e354b8`  
		Last Modified: Thu, 09 Feb 2023 09:41:51 GMT  
		Size: 61.5 MB (61483026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb5c274588d4258eb950fbaa10cc0019974d2ada4c939a9daedad737721434b`  
		Last Modified: Thu, 09 Feb 2023 09:41:43 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ee7932daee08629dd93b675c29f3a139f7ffd10a0768ab0155c1eebdf73e1c`  
		Last Modified: Thu, 09 Feb 2023 09:41:43 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-tools-deps-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:58ed877b959b21f40d6ff407d741b80cca4b8047445f2c3869d59f306ef74b58
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.9 MB (282921019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6667cd06989df251f19d39ec29de8a254b89665750836a824a5766fe0eaa7cf`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:18:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:23:59 GMT
COPY dir:a1bd99c3d82513db94430c73467e1e5c69ea4624d0489571d594afe503e15dc5 in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:24:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 09:25:33 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Thu, 09 Feb 2023 09:25:33 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:25:46 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 09 Feb 2023 09:25:46 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 09 Feb 2023 09:25:46 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Thu, 09 Feb 2023 09:25:46 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 09 Feb 2023 09:25:47 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7586f864daee85da340c78373323940ea5aadab0913592ab630744b3a8d6605`  
		Last Modified: Thu, 09 Feb 2023 09:34:26 GMT  
		Size: 191.3 MB (191260427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:703dfa01564aa9ba5f9dc5bcdc9aa0ce081c79107fc0127ea40a2c8190d52d66`  
		Last Modified: Thu, 09 Feb 2023 09:35:26 GMT  
		Size: 61.6 MB (61597063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e19c4aad078a94e68233a26f6428be2db3d7e3cc1ca7359cd1f405138d33e3b`  
		Last Modified: Thu, 09 Feb 2023 09:35:19 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:844c8e312a92aeab349bd5b9080570b6786c031cb23bd54fdae0846323583a5d`  
		Last Modified: Thu, 09 Feb 2023 09:35:19 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
