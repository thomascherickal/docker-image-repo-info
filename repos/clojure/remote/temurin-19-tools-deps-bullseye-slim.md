## `clojure:temurin-19-tools-deps-bullseye-slim`

```console
$ docker pull clojure@sha256:1b52f8ae1ceb13025a1935f2e65777592998a379874121733c39ab13a474640a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-tools-deps-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:ce29d9baf6d85c82acd33c3253b2819d79bd82d37749f570cafdc559df09bce4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.0 MB (294008751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01557ff4628154d86f13dc2aa4349bf7f980c42dff0530459be7c49e899a0e5d`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:22:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:31:41 GMT
COPY dir:94cb5af8175285c10c94286222d8a35302f3f8c290e00011a75c67156659d6ab in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:31:43 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 09:33:37 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Thu, 09 Feb 2023 09:33:37 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:33:55 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 09 Feb 2023 09:33:56 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 09 Feb 2023 09:33:56 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Thu, 09 Feb 2023 09:33:56 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 09 Feb 2023 09:33:56 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4864f8db9c8a9f2cc75ddf386c4ed7fdb7fd8a6d6a8e917a1fefd0d654a89ada`  
		Last Modified: Thu, 09 Feb 2023 09:42:47 GMT  
		Size: 201.1 MB (201112993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283203a444d9734460dc671e296185f2b6c1b04d978f8d8ad7d5dc9acab7c901`  
		Last Modified: Thu, 09 Feb 2023 09:43:46 GMT  
		Size: 61.5 MB (61482924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00601691b3829eb7ef3aaa421e8504139739dca48c3a5ca2aecd6da8715942a0`  
		Last Modified: Thu, 09 Feb 2023 09:43:38 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ae14e3adf8a4fe6816e72c95ab1d68ad02494aa48994b455217f29ea7b2757`  
		Last Modified: Thu, 09 Feb 2023 09:43:38 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-tools-deps-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:92be6be33bc4ae3eacd05e94796670470ed04a964eea507b8b5c1e6f404b6f87
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.5 MB (291517754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3853265bbf9e649b3710729044a706d878303f5a1d846432c31cda6c7bee2f74`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:18:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:26:28 GMT
COPY dir:9a6a873ca11063f6f04e7f088397a1fce771e2b1aa8590b72eb07158cfac883f in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:26:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 13 Feb 2023 20:46:33 GMT
ENV CLOJURE_VERSION=1.11.1.1224
# Mon, 13 Feb 2023 20:46:33 GMT
WORKDIR /tmp
# Mon, 13 Feb 2023 20:46:46 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "3bbab4d253eda43e3122fd5705014a69c44944a6dee8ea4d7d567afe157eb4ef *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Mon, 13 Feb 2023 20:46:47 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Mon, 13 Feb 2023 20:46:47 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Mon, 13 Feb 2023 20:46:47 GMT
ENTRYPOINT ["entrypoint"]
# Mon, 13 Feb 2023 20:46:47 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef88b0545c043fbdf4b8f9e944c5439147e4d7ceb092637c3f142d7ec06d0749`  
		Last Modified: Thu, 09 Feb 2023 09:36:23 GMT  
		Size: 199.9 MB (199855198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c04a0f850e6d8e2e7f6adc67ac76fec241ad38df204ab78b01bfdc78fe1c54b`  
		Last Modified: Mon, 13 Feb 2023 20:55:02 GMT  
		Size: 61.6 MB (61599028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd9d3a46936560ba68ab87add56cf3e34d4096fb7065777e9ba3582a0c95acc`  
		Last Modified: Mon, 13 Feb 2023 20:54:56 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a335d4e0c52debdb39db007d5ad21ecba001a2e60fc3f5ab92ce1d560397fbe`  
		Last Modified: Mon, 13 Feb 2023 20:54:56 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
