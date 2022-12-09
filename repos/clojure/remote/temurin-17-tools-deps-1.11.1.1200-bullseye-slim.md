## `clojure:temurin-17-tools-deps-1.11.1.1200-bullseye-slim`

```console
$ docker pull clojure@sha256:9a7fe3d17f4ef3affa95e530516bc16569e7a4d26b4cf5cdf953101880e2bb7a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-tools-deps-1.11.1.1200-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:b44fd5447fc1fc986fb30f6c32bd92770de30b309baa4d6648d856e61c535169
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.3 MB (285329924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:181a7d5d614f057942a8e6ab44678f889066452e558354f5387952b76451e640`
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
# Fri, 09 Dec 2022 06:45:06 GMT
ENV CLOJURE_VERSION=1.11.1.1200
# Fri, 09 Dec 2022 06:45:06 GMT
WORKDIR /tmp
# Fri, 09 Dec 2022 06:45:22 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "694381cb78d44f143bdcc38657507f012ebac4009bc57cec67abef1675447878 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 09 Dec 2022 06:45:23 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 09 Dec 2022 06:45:23 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Fri, 09 Dec 2022 06:45:23 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 09 Dec 2022 06:45:23 GMT
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
	-	`sha256:d72026f7264fa9d03070d969a2d1d5b1b5a36b77ce5f89aa9aa72bbe88e00b90`  
		Last Modified: Fri, 09 Dec 2022 06:59:13 GMT  
		Size: 61.5 MB (61484789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e78563a961a05ae0ff61551c5197b72e46f7c98b48e2fec319c5925a15b4a94d`  
		Last Modified: Fri, 09 Dec 2022 06:59:05 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9adb3a1896578982bc4cf9548ad79742be4f8fc95cbf516cb17c19e290f5fbb6`  
		Last Modified: Fri, 09 Dec 2022 06:59:05 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-tools-deps-1.11.1.1200-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:45b18583bc8be15c6081404f09e43c5d8c1d09b4db2fce2ee12e8e432ef9ad4f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.9 MB (282880866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4450d6071497b7a5a19c6ce6835abcea24f08810216c8045b540bcb9456ae59`
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
# Fri, 09 Dec 2022 05:10:57 GMT
ENV CLOJURE_VERSION=1.11.1.1200
# Fri, 09 Dec 2022 05:10:57 GMT
WORKDIR /tmp
# Fri, 09 Dec 2022 05:11:10 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "694381cb78d44f143bdcc38657507f012ebac4009bc57cec67abef1675447878 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 09 Dec 2022 05:11:11 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 09 Dec 2022 05:11:11 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Fri, 09 Dec 2022 05:11:11 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 09 Dec 2022 05:11:11 GMT
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
	-	`sha256:11705ece7d73f94a4e56efdc9d03cb2155ffa6bab3a2acd976cf6a824a272792`  
		Last Modified: Fri, 09 Dec 2022 05:23:36 GMT  
		Size: 61.6 MB (61604324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ce316e6e2e11d78661b744b6e45b201220d6fe38201773d9fb9e55cebbdd68`  
		Last Modified: Fri, 09 Dec 2022 05:23:29 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5544a1ddcde5b947f44f7fd9ad986c8a908bb9a3763f8b5f9b10404362b893`  
		Last Modified: Fri, 09 Dec 2022 05:23:29 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
