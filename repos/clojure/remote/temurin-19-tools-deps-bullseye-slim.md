## `clojure:temurin-19-tools-deps-bullseye-slim`

```console
$ docker pull clojure@sha256:7f50b6e464abff88c542d85d7498482a19ff3c0fb31f66c370de12d3dc80a839
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-tools-deps-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:cdefa6769c78449895ac04d29d38c2a107d7529aafc1b7b1e45ab06a5290bff8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.0 MB (293976602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1989d6f18548937d3eaef6cd3c133904ed9d2d7ec05994ef7535dab090a87b5`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:20:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 11 Jan 2023 03:29:24 GMT
COPY dir:fef581854733ec7202f8c807463b9e1952aeb6c7a002719c7e54987e50ea4dcb in /opt/java/openjdk 
# Wed, 11 Jan 2023 03:29:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 03:31:21 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Wed, 11 Jan 2023 03:31:21 GMT
WORKDIR /tmp
# Wed, 11 Jan 2023 03:31:39 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 11 Jan 2023 03:31:40 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 11 Jan 2023 03:31:40 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 11 Jan 2023 03:31:40 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 11 Jan 2023 03:31:40 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d8be54a6a27b2dcfcf7bef696c11a2997b5312abc571cedd943a85c4d8dbea`  
		Last Modified: Wed, 11 Jan 2023 03:40:45 GMT  
		Size: 201.1 MB (201103413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8841a4cc93bc01b600525cc70eb1dae2e6353eeeca68ff20dec5ac591aef89`  
		Last Modified: Wed, 11 Jan 2023 03:41:45 GMT  
		Size: 61.5 MB (61475201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e50372e3938ffbbb68db4d6a4851329d9195ad083387baef0132effba1c2a07a`  
		Last Modified: Wed, 11 Jan 2023 03:41:37 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89950848f7d0348a0347811a779cbafba3b21ba5c878b8fec0173d2ee76d31bf`  
		Last Modified: Wed, 11 Jan 2023 03:41:37 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-tools-deps-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:28c05d637573accabbdf13e5ec63add73ce65859c3122425828ab8104ce9ba7f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.5 MB (291506652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92a9fb8bb33b7d112c55c5c14fed02c3e7d22801de2f5ceb0e836bf2e3f39194`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 11 Jan 2023 03:46:26 GMT
COPY dir:4138443eebfda1a2a245638d5bb568645bd34d79b66d39a3be31b5ac6b823d6d in /opt/java/openjdk 
# Wed, 11 Jan 2023 03:46:31 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 03:48:09 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Wed, 11 Jan 2023 03:48:09 GMT
WORKDIR /tmp
# Wed, 11 Jan 2023 03:48:23 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 11 Jan 2023 03:48:23 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 11 Jan 2023 03:48:24 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 11 Jan 2023 03:48:24 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 11 Jan 2023 03:48:24 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa89f4fc9f09a63d5cbae62dce013f90ebadeb7676212824b1c3bb4ea7e3cbc`  
		Last Modified: Wed, 11 Jan 2023 03:56:25 GMT  
		Size: 199.9 MB (199864415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d353ba96047b9aca7f6da60778aaf64a80fa71e3f547e6da68345493b312f3ff`  
		Last Modified: Wed, 11 Jan 2023 03:57:19 GMT  
		Size: 61.6 MB (61596405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72d6fbe1cdcdd1c54460370c5a10c1621185cc4c654cefe7e4d8ab091060e054`  
		Last Modified: Wed, 11 Jan 2023 03:57:13 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04d2b527c68c658a07c2cf3c9b0cb5f84e739bbe1ff70c9ab825e1ba9f869b4`  
		Last Modified: Wed, 11 Jan 2023 03:57:13 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
