## `clojure:temurin-11-tools-deps-bullseye-slim`

```console
$ docker pull clojure@sha256:63dbf7c4227cc5a52b66eb396cc9706353b982d3d41facf2ec4905c615e75bff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-tools-deps-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:0c0ff1608df53a17bcab1557ccea38d10951f05027a319535737721068724f57
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.3 MB (291347662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:022560dd4c55398a9c154f36f9301de792a70538cf613a00cad5d3ba47488384`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:20:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 25 Jan 2023 00:39:28 GMT
COPY dir:7c6c6be58d44c17cd09173c77ba1f0d96ed42a5b7ef2235235262bdd0141924b in /opt/java/openjdk 
# Wed, 25 Jan 2023 00:39:30 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 25 Jan 2023 00:43:27 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Wed, 25 Jan 2023 00:43:27 GMT
WORKDIR /tmp
# Wed, 25 Jan 2023 00:43:45 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 25 Jan 2023 00:43:45 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 25 Jan 2023 00:43:45 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a47d09ee4791f80acce6e1c0ec8e323c79df787142099f3b440887c41fbeeaf`  
		Last Modified: Wed, 25 Jan 2023 00:54:33 GMT  
		Size: 198.5 MB (198475706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb5c69f5a54b4ae215a49cdd47a6b516f3b44623ad456b45fac07f79d9c9852`  
		Last Modified: Wed, 25 Jan 2023 00:56:37 GMT  
		Size: 61.5 MB (61474368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faaeeda3e5a68e9ed50ece1177742ed3291d1250666ee340309b515fd132e666`  
		Last Modified: Wed, 25 Jan 2023 00:56:29 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-tools-deps-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:d834e1dc27fe1ee7e488872c756c96e9ba392b2c372906ce2cb66c25196aae42
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.9 MB (286883096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bd10bde614eb039db6559468afe2c043029bcd7df524d95f171c14885b1baa4`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Jan 2023 20:50:12 GMT
COPY dir:b661686bf8d434588756c45f2ef6e7f314f32f753cf180ef8fb45397388f098c in /opt/java/openjdk 
# Tue, 31 Jan 2023 20:50:16 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 20:53:12 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Tue, 31 Jan 2023 20:53:12 GMT
WORKDIR /tmp
# Tue, 31 Jan 2023 20:53:25 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 31 Jan 2023 20:53:26 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 31 Jan 2023 20:53:26 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5842b36268c5c5b9539a446d9eba4513a75b1955de0b698663ccf059458ac527`  
		Last Modified: Tue, 31 Jan 2023 21:04:34 GMT  
		Size: 195.2 MB (195240302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c26f07ae05e9e7844eb2d13243f1dd4e06e3b328fa0cbfe477b5cc510127a10`  
		Last Modified: Tue, 31 Jan 2023 21:06:16 GMT  
		Size: 61.6 MB (61597362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acdf2a44e28f388056a7f19031576c1b9b933254565ab9ccc83eb980f4c0bf27`  
		Last Modified: Tue, 31 Jan 2023 21:06:10 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
