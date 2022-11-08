## `clojure:temurin-19-tools-deps-bullseye-slim`

```console
$ docker pull clojure@sha256:056a6f2379676c826c24bfb5917af2b75f1a5db47d5f79b612a74095b2fbf8fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-tools-deps-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:e8185422a26aa51e9e69683967bb659d373b4200afca6a1d3695776f381cbb0d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.0 MB (293997924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3394e619efcbe43e1750362505b855e1db80f1d7bbc76ebc1cc3e15d4be3206b`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 08 Nov 2022 19:51:27 GMT
COPY dir:fef581854733ec7202f8c807463b9e1952aeb6c7a002719c7e54987e50ea4dcb in /opt/java/openjdk 
# Tue, 08 Nov 2022 19:51:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Nov 2022 19:55:20 GMT
ENV CLOJURE_VERSION=1.11.1.1189
# Tue, 08 Nov 2022 19:55:20 GMT
WORKDIR /tmp
# Tue, 08 Nov 2022 19:55:40 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "1afd91b165776615eca84cce2271e5fe5d5818c55dee0f082b1304bb1464b3e8 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 08 Nov 2022 19:55:40 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 08 Nov 2022 19:55:40 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Tue, 08 Nov 2022 19:55:40 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 08 Nov 2022 19:55:40 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c10a8a6939ae868ebbacdafba32bb072252658a353d99bfac452b469d292956a`  
		Last Modified: Tue, 08 Nov 2022 20:01:13 GMT  
		Size: 201.1 MB (201103390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c498be0b95e6b82496d69ddd77dfffe31441ee67fa56062e5218699201fbad`  
		Last Modified: Tue, 08 Nov 2022 20:03:47 GMT  
		Size: 61.5 MB (61473478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac3519067cfe1968456c3989ca47e65748c6fb21160d905e8c69b0b149da946`  
		Last Modified: Tue, 08 Nov 2022 20:03:39 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cdfe167bf255021aca6fb7cfdfa69cfa9a5c73d790116bacb41791e8c0e7843`  
		Last Modified: Tue, 08 Nov 2022 20:03:39 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-tools-deps-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:b248ccf9d11164868dcb2e466ac97eb7f5d9e92e5df20b8742936cb723691bfe
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.5 MB (291522477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de7300410559f12b46cbc47344d38be7044392d7bdbf2abfe5640661c481b1e6`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 08 Nov 2022 22:41:45 GMT
COPY dir:4138443eebfda1a2a245638d5bb568645bd34d79b66d39a3be31b5ac6b823d6d in /opt/java/openjdk 
# Tue, 08 Nov 2022 22:41:49 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Nov 2022 22:45:08 GMT
ENV CLOJURE_VERSION=1.11.1.1189
# Tue, 08 Nov 2022 22:45:08 GMT
WORKDIR /tmp
# Tue, 08 Nov 2022 22:45:21 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "1afd91b165776615eca84cce2271e5fe5d5818c55dee0f082b1304bb1464b3e8 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 08 Nov 2022 22:45:21 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 08 Nov 2022 22:45:21 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Tue, 08 Nov 2022 22:45:21 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 08 Nov 2022 22:45:21 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d87dade7855f65c2325e4aad477888abaabf5a2aa0888be9bbb8d5e0445df5ec`  
		Last Modified: Tue, 08 Nov 2022 22:50:12 GMT  
		Size: 199.9 MB (199864415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56e21179d6a75534fabde501321fce42a0dd358ae9baf77efa919a47b6a295db`  
		Last Modified: Tue, 08 Nov 2022 22:52:04 GMT  
		Size: 61.6 MB (61593130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ca412589252aa45a44e914bea15e324fa25a1b163433047dc68492678fe18c`  
		Last Modified: Tue, 08 Nov 2022 22:51:58 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50abcbee8da6e2b1134658e1ce8749260f1881cf8abeb2f8e6e41794ea71ebb0`  
		Last Modified: Tue, 08 Nov 2022 22:51:58 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
