## `clojure:temurin-17-tools-deps-1.11.1.1165-bullseye-slim`

```console
$ docker pull clojure@sha256:37043504f827bb1d7c9503682925829d173dbb9e6f0d7adaba18045fa92d8377
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-tools-deps-1.11.1.1165-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:4484d47ab2fe9fff2111248fb1d91cf5b2d6428ffd82793b760ac6c6e8751d69
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.0 MB (285012638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c52aeb1dfba120f724292cfbd44c283fc2fe1d4ba7feb9468216fe518fab8e89`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:29 GMT
ADD file:5bd53bff884e470b3c12425132975ab9c6f99002c62c43bca1ff5cde9d863b92 in / 
# Tue, 13 Sep 2022 00:56:29 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:18:42 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 30 Sep 2022 22:27:47 GMT
COPY dir:4a40d0ddbd507a7d3b3a97117be800fbf93534cac954d63629e4fb22f3cd41ad in /opt/java/openjdk 
# Fri, 30 Sep 2022 22:27:48 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 30 Sep 2022 22:29:42 GMT
ENV CLOJURE_VERSION=1.11.1.1165
# Fri, 30 Sep 2022 22:29:42 GMT
WORKDIR /tmp
# Fri, 30 Sep 2022 22:29:59 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "72d662bdc99b79037f9e34996272384de35e01e0416d8eb79cc940ee0f0fc808 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 30 Sep 2022 22:29:59 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 30 Sep 2022 22:30:00 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Fri, 30 Sep 2022 22:30:00 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 30 Sep 2022 22:30:00 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:31b3f1ad4ce1f369084d0f959813c51df0ca17d9877d5ee88c2db6ff88341430`  
		Last Modified: Tue, 13 Sep 2022 01:00:29 GMT  
		Size: 31.4 MB (31404121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e65a48fb445eb8f9528419bdb749aff629072fae69a78a509e2773ba76d43379`  
		Last Modified: Fri, 30 Sep 2022 22:39:51 GMT  
		Size: 192.1 MB (192137446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11039ffbf9a0632f4e889f0bbb892161917433afb04e401e4e1b6470a50585d2`  
		Last Modified: Fri, 30 Sep 2022 22:40:59 GMT  
		Size: 61.5 MB (61470052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e259c439eee62e0297c57da3273e285bece0cee98edf69ae4c013cb718fdc999`  
		Last Modified: Fri, 30 Sep 2022 22:40:51 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60f554b3bfa0cfa756e1c7d3bce3966e69da77eb94c9b33cd7b197d82cb9235`  
		Last Modified: Fri, 30 Sep 2022 22:40:51 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-tools-deps-1.11.1.1165-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:3c1d008b918eff435310b308005fab1162c8b3037727d2a90ef0056bc159ba83
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.6 MB (282556856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cd2da3225c6f030658c812f4dc25e22dfdd991c7967bedd5c28672b269c0b74`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 13 Sep 2022 02:10:56 GMT
ADD file:e8f00260a993aacae732bef51e6074b6c064d50a8ce1f0c44d53fe9e3c868e43 in / 
# Tue, 13 Sep 2022 02:10:56 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:58:12 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 30 Sep 2022 22:48:36 GMT
COPY dir:e8b09aac8a69a5f07df362ceeac55cf5f3321b4ba40e9b02e12250e34b34e83e in /opt/java/openjdk 
# Fri, 30 Sep 2022 22:48:36 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 30 Sep 2022 22:51:07 GMT
ENV CLOJURE_VERSION=1.11.1.1165
# Fri, 30 Sep 2022 22:51:08 GMT
WORKDIR /tmp
# Fri, 30 Sep 2022 22:51:25 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "72d662bdc99b79037f9e34996272384de35e01e0416d8eb79cc940ee0f0fc808 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 30 Sep 2022 22:51:26 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 30 Sep 2022 22:51:27 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Fri, 30 Sep 2022 22:51:27 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 30 Sep 2022 22:51:28 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:3d898485473e3507374cea2e09f019c2ff5728f0911aa36c70b7a7235e9bc8ac`  
		Last Modified: Tue, 13 Sep 2022 02:16:19 GMT  
		Size: 30.1 MB (30054239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:836e9ee07116b1c34e53212577545c764c310f4ad2784f78e99382d4f859d340`  
		Last Modified: Fri, 30 Sep 2022 23:05:05 GMT  
		Size: 190.9 MB (190904320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756c5ec873f48dd19deb2959fc948c5e86a190ecaaffb860eef57df68851ec61`  
		Last Modified: Fri, 30 Sep 2022 23:06:23 GMT  
		Size: 61.6 MB (61597277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f5445dccc5c2f1d965c2c2cc79311381de84c4a7a82cd8bdcc9fe342f72ec6`  
		Last Modified: Fri, 30 Sep 2022 23:06:15 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b8f9f29b0e7a5d0e11a2b857fee1da6a4f76774f3c654df89f738afb7e9253`  
		Last Modified: Fri, 30 Sep 2022 23:06:15 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
