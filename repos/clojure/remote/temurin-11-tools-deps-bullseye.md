## `clojure:temurin-11-tools-deps-bullseye`

```console
$ docker pull clojure@sha256:c9e14e3fd3ba3a2582cde32065c89010ac9a8134c110e336725ed028c649ff83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-tools-deps-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:58ce4d48afb08e395e39e3d0b08ccad92e429bb06f52501cecd50a46f669633c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.4 MB (325359825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83cb0c896463c6b36131619d6270279bf6fb0cf232fff4cb4f007f3203efdc35`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:29 GMT
ADD file:917750a82b29f8f7f88a121017bd9dfeb0fbcc8f0697a009f08b6b58246eff4b in / 
# Wed, 11 Jan 2023 02:34:30 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:18:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 25 Jan 2023 00:38:55 GMT
COPY dir:7c6c6be58d44c17cd09173c77ba1f0d96ed42a5b7ef2235235262bdd0141924b in /opt/java/openjdk 
# Wed, 25 Jan 2023 00:38:57 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 25 Jan 2023 00:42:58 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Wed, 25 Jan 2023 00:42:59 GMT
WORKDIR /tmp
# Wed, 25 Jan 2023 00:43:20 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 25 Jan 2023 00:43:21 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 25 Jan 2023 00:43:21 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:bbeef03cda1f5d6c9e20c310c1c91382a6b0a1a2501c3436b28152f13896f082`  
		Last Modified: Wed, 11 Jan 2023 02:38:42 GMT  
		Size: 55.0 MB (55025206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602e2ea8d297cb16cb85100f12e05f8198378e9fa1ddc9b44e587dc662a6b8dc`  
		Last Modified: Wed, 25 Jan 2023 00:54:09 GMT  
		Size: 198.5 MB (198475718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f99aff8a35dbb6449cad0e442e7cc1087597b0ae87cc59f7d16605f8ba74b96`  
		Last Modified: Wed, 25 Jan 2023 00:56:19 GMT  
		Size: 71.9 MB (71858286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b6c7ca607163b30173e09685e0b4a3f76e427e29feb1c228d4c6b2df05a1b6`  
		Last Modified: Wed, 25 Jan 2023 00:56:11 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-tools-deps-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:c5658e442d5699dbcf8bb69f63ac2f2f50c9626553800234482c4d72b3b79b48
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **320.9 MB (320907934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9baef8522da33fc36946baef473c84011c0404fb3fcbb25f1a4384ea7b88609c`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:24 GMT
ADD file:9e185c2d9ca8a231a39ee2b1761fcdff75065252d25a65a207acb7a319c1cf23 in / 
# Wed, 11 Jan 2023 02:57:25 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:14 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Jan 2023 20:49:40 GMT
COPY dir:b661686bf8d434588756c45f2ef6e7f314f32f753cf180ef8fb45397388f098c in /opt/java/openjdk 
# Tue, 31 Jan 2023 20:49:44 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 20:52:48 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Tue, 31 Jan 2023 20:52:48 GMT
WORKDIR /tmp
# Tue, 31 Jan 2023 20:53:05 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 31 Jan 2023 20:53:06 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 31 Jan 2023 20:53:06 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:c345c9e441f5f49235768af74b8ab37743652d38958afaa000edd56d7b2f0540`  
		Last Modified: Wed, 11 Jan 2023 03:00:56 GMT  
		Size: 53.7 MB (53681859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4582f4343bacf57f66f8e6afa3b09983b023babf5d4da2ccacfead5d1e72571`  
		Last Modified: Tue, 31 Jan 2023 21:04:14 GMT  
		Size: 195.2 MB (195240378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b0ec53044066821ce7a335a8146136c3cdae2992deaae853169a44c9e2823b`  
		Last Modified: Tue, 31 Jan 2023 21:05:58 GMT  
		Size: 72.0 MB (71985078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e4a601cecb6f989ea7c1b5af9a254e020d309c1c766d8535843237e7ef4a756`  
		Last Modified: Tue, 31 Jan 2023 21:05:51 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
