## `clojure:temurin-19-tools-deps-bullseye-slim`

```console
$ docker pull clojure@sha256:87c58edf6da19c209be9a56db71177bce9a5a7b3f1e5d995b76f782ff177d022
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
$ docker pull clojure@sha256:36afe23ca13224fc7895a7eb29e57da4143165c916e549aed4993498cc6db543
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.5 MB (291515981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e982dd70dae686f4f2bc4391936ff14bd50aff8dd3bebab16997e471e6153007`
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
# Thu, 09 Feb 2023 09:27:59 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Thu, 09 Feb 2023 09:27:59 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:28:12 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 09 Feb 2023 09:28:13 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 09 Feb 2023 09:28:13 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Thu, 09 Feb 2023 09:28:13 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 09 Feb 2023 09:28:13 GMT
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
	-	`sha256:d86b47db04cf8e58192035a3a6aad4a7c34c345911f1dbd0891b6101f6c396de`  
		Last Modified: Thu, 09 Feb 2023 09:37:19 GMT  
		Size: 61.6 MB (61597253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36b4fd4d84b560d7190d54bfb4465c4fcaf9e252882a2b21b14c4892173737f`  
		Last Modified: Thu, 09 Feb 2023 09:37:12 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db33a210ae31b810cf8b6bb4ddcbfdd93d760c5ac2243cd71b5f2db4f06e76c`  
		Last Modified: Thu, 09 Feb 2023 09:37:12 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
