## `clojure:temurin-17-bullseye-slim`

```console
$ docker pull clojure@sha256:e81da592d1daafb7d0acb63cb271781496a83c840f5a788f146778d37b9ca9f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:787fbb246edd82649f43e1f800ab9fbeae037bcb0a29d901dfba713aa1b83da3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.3 MB (285321797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85914178c9d4948e5f1e05a6c98215321880dd7a2a0c3bd399ba6cf6ca71e627`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 06:42:08 GMT
COPY dir:6d447c71fb5cab25c46568db16879377c790ade488ebb14a9cc6935f6b8bd709 in /opt/java/openjdk 
# Fri, 09 Dec 2022 06:42:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Dec 2022 00:23:17 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Wed, 14 Dec 2022 00:23:18 GMT
WORKDIR /tmp
# Wed, 14 Dec 2022 00:23:35 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 14 Dec 2022 00:23:36 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 14 Dec 2022 00:23:36 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 14 Dec 2022 00:23:36 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 14 Dec 2022 00:23:36 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72b40014e8ed7c4beca3427f678152536843fa5317d5c90ba564c8f93f170d1`  
		Last Modified: Fri, 09 Dec 2022 06:57:07 GMT  
		Size: 192.4 MB (192431264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098ec8c0817feab781da222f60397fcf2604162c41860b308295c40f5b5c36a1`  
		Last Modified: Wed, 14 Dec 2022 00:30:46 GMT  
		Size: 61.5 MB (61476662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de19ef23d6c8de9f6f0fdf7bf00045aa87ea483d73c804d7145f545b164b4eb9`  
		Last Modified: Wed, 14 Dec 2022 00:30:38 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea30d495e630f9bd8801b3c65a70d52e6098583ab96de76216ab6f29d1cd6a7`  
		Last Modified: Wed, 14 Dec 2022 00:30:38 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:8d7c6b5d642d67c5ea39b14b33e70310c1e4e736b02237bf619d79d2577dd934
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.9 MB (282873845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6a93fbc89a3014388d088fecb778da85a0e015045f775482ea9d0e72098282e`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 05:08:26 GMT
COPY dir:533cfee1c12b6052cd1297ebc89704c8b7da6e8016c06b0e341bcec0d4934dde in /opt/java/openjdk 
# Fri, 09 Dec 2022 05:08:30 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Dec 2022 00:42:12 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Wed, 14 Dec 2022 00:42:12 GMT
WORKDIR /tmp
# Wed, 14 Dec 2022 00:42:25 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 14 Dec 2022 00:42:26 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 14 Dec 2022 00:42:26 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 14 Dec 2022 00:42:26 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 14 Dec 2022 00:42:26 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252cfa205e433a4c57ba726668ab09a5be5ab3251c8c31999a816013f05f5e54`  
		Last Modified: Fri, 09 Dec 2022 05:21:35 GMT  
		Size: 191.2 MB (191215205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd2b01c4fd45dd89ee1c502c0479f4d7ea38fc80417933066b2d4e0ca2c1c6f`  
		Last Modified: Wed, 14 Dec 2022 00:48:23 GMT  
		Size: 61.6 MB (61597301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501c02b9853a9fa7060098020fa4b2b6dfd4cc6b4d367b2af0a034eeee5748b5`  
		Last Modified: Wed, 14 Dec 2022 00:48:17 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1690cb65af8d39fac68034835937f82e43840a1699be0215c3783887c1c6834e`  
		Last Modified: Wed, 14 Dec 2022 00:48:17 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
