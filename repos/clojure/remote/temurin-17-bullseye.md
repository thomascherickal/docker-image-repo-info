## `clojure:temurin-17-bullseye`

```console
$ docker pull clojure@sha256:edb0547a706c63fa2cc978e743f8d623c12a9ad7205fc9ae2ae774ffb1fdbe2f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:66093ffc52cfb3995653064743ed4482d75aed38c407770f63f417bde63fe0b1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.5 MB (294464532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b961cdcda9c4a2974bbaa23766af4ccfc93c7cb9f07cb49ff54dd7aa7d2eb192`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:18 GMT
ADD file:ff01c6dedb67cf22e9b0735e099b9b6367770c4880941862cc7ec0e979b4118b in / 
# Tue, 13 Sep 2022 00:56:19 GMT
CMD ["bash"]
# Fri, 30 Sep 2022 22:20:04 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 30 Sep 2022 22:27:08 GMT
COPY dir:4a40d0ddbd507a7d3b3a97117be800fbf93534cac954d63629e4fb22f3cd41ad in /opt/java/openjdk 
# Fri, 30 Sep 2022 22:27:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 30 Sep 2022 22:29:22 GMT
ENV CLOJURE_VERSION=1.11.1.1165
# Fri, 30 Sep 2022 22:29:22 GMT
WORKDIR /tmp
# Fri, 30 Sep 2022 22:29:37 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "72d662bdc99b79037f9e34996272384de35e01e0416d8eb79cc940ee0f0fc808 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 30 Sep 2022 22:29:38 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 30 Sep 2022 22:29:38 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Fri, 30 Sep 2022 22:29:38 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 30 Sep 2022 22:29:38 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:23858da423a6737f0467fab0014e5b53009ea7405d575636af0c3f100bbb2f10`  
		Last Modified: Tue, 13 Sep 2022 01:00:00 GMT  
		Size: 55.0 MB (55029732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0797d39ad88d22b27575060fbd4e4675f49d12e305138f24e08544ecba14490`  
		Last Modified: Fri, 30 Sep 2022 22:39:27 GMT  
		Size: 192.1 MB (192137652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951d6a3d4b74be2cb59e8bf4f0d81f78691f7f38959068d86f6ffef10c542989`  
		Last Modified: Fri, 30 Sep 2022 22:40:40 GMT  
		Size: 47.3 MB (47296131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6dcd254f8c49ff6daea92d60cdf7c0eea39c9ecbcdd4cd8c440cfc0aefb2e1f`  
		Last Modified: Fri, 30 Sep 2022 22:40:34 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f362dac0170787987d1a1d81a409b0970dbe09bdb632e897f9f4e432dad8c60`  
		Last Modified: Fri, 30 Sep 2022 22:40:34 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:e4ebd6eaee8f43704019c12d7382cf31a086d8dbc2a532a49b15592f70103947
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291887498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69d7bec0cef1b3bb0bf9ddee41354c0958f6efe4d9664c06aefce7683dae64ad`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 13 Sep 2022 02:10:41 GMT
ADD file:879fb0cd23107ac6f53581456074c7ff13c051aa262de3ca16ffa8475cf04dec in / 
# Tue, 13 Sep 2022 02:10:42 GMT
CMD ["bash"]
# Fri, 30 Sep 2022 22:40:22 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 30 Sep 2022 22:47:59 GMT
COPY dir:e8b09aac8a69a5f07df362ceeac55cf5f3321b4ba40e9b02e12250e34b34e83e in /opt/java/openjdk 
# Fri, 30 Sep 2022 22:48:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 30 Sep 2022 22:50:40 GMT
ENV CLOJURE_VERSION=1.11.1.1165
# Fri, 30 Sep 2022 22:50:41 GMT
WORKDIR /tmp
# Fri, 30 Sep 2022 22:50:57 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "72d662bdc99b79037f9e34996272384de35e01e0416d8eb79cc940ee0f0fc808 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 30 Sep 2022 22:50:58 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 30 Sep 2022 22:50:59 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Fri, 30 Sep 2022 22:50:59 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 30 Sep 2022 22:51:00 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:10cff8997b4d4f243419e6bede830f1ac33f3d18c5200e5fb80e19333883ec2b`  
		Last Modified: Tue, 13 Sep 2022 02:15:49 GMT  
		Size: 53.7 MB (53691380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ffe5c027f43a0f8dffe3c143fa6c23f9705c59001d637c3093c164b11f8970`  
		Last Modified: Fri, 30 Sep 2022 23:04:37 GMT  
		Size: 190.9 MB (190904318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae31cd4882f6894f7653b1e25e5d320707e687dc101481834b5f20b8e71e5877`  
		Last Modified: Fri, 30 Sep 2022 23:06:01 GMT  
		Size: 47.3 MB (47290778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ac0db7f9a7b037491366609240a4f0a13a6bd9aa4e5da2a1b8831cf7c5b81b`  
		Last Modified: Fri, 30 Sep 2022 23:05:55 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7800b30addffe156a17a7396322af089dc1605a760d6dd2111709dcd088f5aa`  
		Last Modified: Fri, 30 Sep 2022 23:05:55 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
