## `clojure:temurin-19-tools-deps-bullseye-slim`

```console
$ docker pull clojure@sha256:106825d0de814655e235923ce95d40e2ad59aac5a76ae96502434692ecb57844
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-tools-deps-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:6466c4ddc2b0e1e5280030b42e7baf9b482e816506c638ea3a2cf94cd2c5fb83
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.7 MB (293738573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd1f8ddcb1b596b1943c15f15ee2753a1db581465825800a8566e095c6e44b59`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 25 Oct 2022 02:43:04 GMT
COPY dir:49a4548ab030e4d26793e92b4d74537cf530961ce7b4083b8d383585c96415d5 in /opt/java/openjdk 
# Tue, 25 Oct 2022 02:43:05 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Nov 2022 20:27:51 GMT
ENV CLOJURE_VERSION=1.11.1.1189
# Thu, 03 Nov 2022 20:27:52 GMT
WORKDIR /tmp
# Thu, 03 Nov 2022 20:28:09 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "1afd91b165776615eca84cce2271e5fe5d5818c55dee0f082b1304bb1464b3e8 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 03 Nov 2022 20:28:10 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 03 Nov 2022 20:28:10 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Thu, 03 Nov 2022 20:28:10 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 03 Nov 2022 20:28:10 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef26e3fe67290659a7b3a065746d54031cd623809f8df384628be68ee2d54a24`  
		Last Modified: Tue, 25 Oct 2022 02:54:40 GMT  
		Size: 200.8 MB (200843786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993035327f3ea200ca4a83348a9b5c2d8f4c49ec777283fc3e9428e283b017de`  
		Last Modified: Thu, 03 Nov 2022 20:38:45 GMT  
		Size: 61.5 MB (61473731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3dba229aca5226429494a50734c9d9d6ff527916fc28df572e719a8d1d9ef01`  
		Last Modified: Thu, 03 Nov 2022 20:38:38 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e59c8eb442cca7bec68525fd45152e6d0aff4059bc9f8bbc4d060a55d293ee1`  
		Last Modified: Thu, 03 Nov 2022 20:38:38 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-tools-deps-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:47866a98514d7c3362f67bf8a3ebed4050b74d65fd4920ac2d2707e637bbdb22
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.2 MB (291240583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ede9edc66a64948289780d93cc6031d1048b4a0c8a374f9f15771fdeb28b6c3`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Oct 2022 15:49:24 GMT
COPY dir:2fc3a52010e404362374a6fbc2449d1ef85a3bc7bb00efe969cabc1864797789 in /opt/java/openjdk 
# Wed, 26 Oct 2022 15:49:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Nov 2022 19:48:17 GMT
ENV CLOJURE_VERSION=1.11.1.1189
# Thu, 03 Nov 2022 19:48:17 GMT
WORKDIR /tmp
# Thu, 03 Nov 2022 19:48:31 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "1afd91b165776615eca84cce2271e5fe5d5818c55dee0f082b1304bb1464b3e8 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 03 Nov 2022 19:48:31 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 03 Nov 2022 19:48:31 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Thu, 03 Nov 2022 19:48:31 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 03 Nov 2022 19:48:31 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0786999deff23ea2618e481d077c8e627d22cb087604cb4be63e8e3940eac2be`  
		Last Modified: Wed, 26 Oct 2022 16:05:46 GMT  
		Size: 199.6 MB (199582448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9858c576569985571be1ab28c47d98cb3201bd7f3b3c36cd6d1dda63b3d6aaa9`  
		Last Modified: Thu, 03 Nov 2022 19:57:09 GMT  
		Size: 61.6 MB (61593207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b254f1ffd9ef9928e99ef31d861825de2e3ef3990e585535f32c57432a0bb592`  
		Last Modified: Thu, 03 Nov 2022 19:57:03 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac35ecd4c3ef3e0b0e6f5a957d0a74b44b34a6d10a9d1d13dcd97877bcf17a93`  
		Last Modified: Thu, 03 Nov 2022 19:57:03 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
