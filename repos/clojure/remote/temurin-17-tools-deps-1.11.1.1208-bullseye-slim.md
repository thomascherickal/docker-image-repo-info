## `clojure:temurin-17-tools-deps-1.11.1.1208-bullseye-slim`

```console
$ docker pull clojure@sha256:cb2aa68aa31f8b73c67a656349f4fca661c0da567e1cb83a788d0ff54c9d791b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-tools-deps-1.11.1.1208-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:85e0e44e7214202601a00f3352b8400635277620f23fc281e16e049c15ad197e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.3 MB (285311191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd913f3b086231c25935051a2a1c3c1d5088a6a40f0cd777008da2ae31aff3e0`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:20:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 25 Jan 2023 00:45:55 GMT
COPY dir:bb223240e99e5b7e66eb621e33f54e49ced87035f56dd975e567c739be4bfe96 in /opt/java/openjdk 
# Wed, 25 Jan 2023 00:45:57 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 25 Jan 2023 00:49:14 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Wed, 25 Jan 2023 00:49:14 GMT
WORKDIR /tmp
# Wed, 25 Jan 2023 00:49:32 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 25 Jan 2023 00:49:33 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 25 Jan 2023 00:49:33 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 25 Jan 2023 00:49:33 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 25 Jan 2023 00:49:33 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12eef77f7984a993273a61d251f96ca5d233a9d09aa5eaf00dacef6ccb54ad5`  
		Last Modified: Wed, 25 Jan 2023 00:58:21 GMT  
		Size: 192.4 MB (192438146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaefe8af31a183679183868cfc14d6b9bbf61672e0bfa7a555dcda3c5add41a6`  
		Last Modified: Wed, 25 Jan 2023 01:01:01 GMT  
		Size: 61.5 MB (61475056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bba71370b330f8c456ac430ca2f124bb7d8eddd91fc76c612232884cbbea115`  
		Last Modified: Wed, 25 Jan 2023 01:00:53 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8936e9911eb18c20e7a09164c675ae92b2dff2d242d773a5e14de01d1347634f`  
		Last Modified: Wed, 25 Jan 2023 01:00:53 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-tools-deps-1.11.1.1208-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:0b59c2e120f755e9d2fa812729e0ea2815b588e2e87945b79db7d12a980a9d7c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.9 MB (282903485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1acc411485293520211277b87ac3a2647e4385ed75c3dd4f9bd844509d5d7ab`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Jan 2023 20:54:33 GMT
COPY dir:a1bd99c3d82513db94430c73467e1e5c69ea4624d0489571d594afe503e15dc5 in /opt/java/openjdk 
# Tue, 31 Jan 2023 20:54:37 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 20:57:04 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Tue, 31 Jan 2023 20:57:04 GMT
WORKDIR /tmp
# Tue, 31 Jan 2023 20:57:18 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 31 Jan 2023 20:57:18 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 31 Jan 2023 20:57:18 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Tue, 31 Jan 2023 20:57:18 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 31 Jan 2023 20:57:18 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a105a97fdf20185e2d7c3fa185a80f146fc82f987de1e73befa061b450f1bf`  
		Last Modified: Tue, 31 Jan 2023 21:07:37 GMT  
		Size: 191.3 MB (191260408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465368fb9ba57cd68b826a42c6a177d18eee221cd39cd00a0ea817aa45d23e1a`  
		Last Modified: Tue, 31 Jan 2023 21:09:38 GMT  
		Size: 61.6 MB (61597246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a098f673713017dad7fdc849e8bc2b2ffb9bd3dcf399dccfcf220ffdf3e7fa58`  
		Last Modified: Tue, 31 Jan 2023 21:09:32 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4c609efb82e4bfa88a8cfd22e96c381250629038b0fca15fe2c383ff75da04`  
		Last Modified: Tue, 31 Jan 2023 21:09:32 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
