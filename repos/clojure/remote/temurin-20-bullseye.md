## `clojure:temurin-20-bullseye`

```console
$ docker pull clojure@sha256:7b81e73390ab048d4baa0485a23e51496fead7f782935bb447b0c0e86890fc0e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-20-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:6342fb28d89ae2ac55e9e67e956e7f94eb01b1493e286abc10e32c8c2d245a8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.7 MB (329742367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5927eafce4872c1b391d33e7b730a049f64b85cad07ad7499a43aa96fa492b43`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 02 May 2023 23:46:50 GMT
ADD file:fc290cf8ddb984325474583faa79c5a98c5ea0ec7f606bf360251f63acecf389 in / 
# Tue, 02 May 2023 23:46:51 GMT
CMD ["bash"]
# Wed, 03 May 2023 20:24:09 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 03 May 2023 20:32:24 GMT
COPY dir:02736280d197ac4d1b6ebf68d948efb46e7eeffd579505356f8c94946dbcce6f in /opt/java/openjdk 
# Wed, 03 May 2023 20:32:26 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 19 May 2023 20:34:14 GMT
ENV CLOJURE_VERSION=1.11.1.1323
# Fri, 19 May 2023 20:34:14 GMT
WORKDIR /tmp
# Fri, 19 May 2023 20:34:30 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "c4666f0e2c2397b91554befd71ff6149b2e89acbf90400e1dcf557526cfb593d *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 19 May 2023 20:34:31 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 19 May 2023 20:34:31 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Fri, 19 May 2023 20:34:31 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 19 May 2023 20:34:31 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:918547b9432687b1e1d238e82dc1e0ea0b736aafbf3c402eea98c6db81a9cb65`  
		Last Modified: Tue, 02 May 2023 23:49:58 GMT  
		Size: 55.0 MB (55049070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b519f573684f5e9384b4dd8bce8687dcafb967c9c60cf34f85bc177e521ab3c9`  
		Last Modified: Wed, 03 May 2023 20:40:02 GMT  
		Size: 202.8 MB (202813974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9369d9dedd637a8c3971cdb399aaa6aa1e0a5f873f8371c4737e27ae8edba58`  
		Last Modified: Fri, 19 May 2023 20:44:47 GMT  
		Size: 71.9 MB (71878305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5934dff350fca06d51df9520faf749b680fdcaf94a1eac27e173bb339d078eff`  
		Last Modified: Fri, 19 May 2023 20:44:39 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c362097d51fee7da0ca646b6ad30dfcd9ab90567b45cb2fd0f9801ca5cc0860d`  
		Last Modified: Fri, 19 May 2023 20:44:39 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-20-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:96e58fdb7fa1aca3af3c227a4162b244dba1082949140beadf8b201a56b43aec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.8 MB (326846164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f7b034dbebc5fdc24ce0c2981c98f2ca5caf9ba3e3920f2cbbad56379643ee8`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 23 May 2023 00:43:08 GMT
ADD file:a823391455122220a061ff349b66ee33413e968447ec5ba4bd544d9182fa2fbe in / 
# Tue, 23 May 2023 00:43:08 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:24:09 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 23 May 2023 01:31:43 GMT
COPY dir:f555428af67a610819205eec573e23f479077e0999818ee9dc0f3375599d21db in /opt/java/openjdk 
# Tue, 23 May 2023 01:31:47 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 01:32:32 GMT
ENV CLOJURE_VERSION=1.11.1.1323
# Tue, 23 May 2023 01:32:32 GMT
WORKDIR /tmp
# Tue, 23 May 2023 01:32:45 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "c4666f0e2c2397b91554befd71ff6149b2e89acbf90400e1dcf557526cfb593d *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 23 May 2023 01:32:46 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 23 May 2023 01:32:46 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Tue, 23 May 2023 01:32:46 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 23 May 2023 01:32:46 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:b04fae59f135dd79280e4a6da39408e04c6d703c617cbcb1c524dfe6f2962fe5`  
		Last Modified: Tue, 23 May 2023 00:45:45 GMT  
		Size: 53.7 MB (53692612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91d72676a8287a859ac8d81d8fd618b87b45fc2856a39d92b8d00911f0c0630a`  
		Last Modified: Tue, 23 May 2023 01:38:41 GMT  
		Size: 201.2 MB (201157969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32a60fb0e3d6f03ac19327155488e8afe0ce5f75bfdceb6f5c6d0c140110678f`  
		Last Modified: Tue, 23 May 2023 01:39:16 GMT  
		Size: 72.0 MB (71994567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37d436872e210dc073ed1ad193345e0926c574dfbe2b6b98e79d2327f24c542`  
		Last Modified: Tue, 23 May 2023 01:39:10 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc076a5e32ab6362aa7e21ffd15c5fcf799b8f830e4ccbfe0fa2234142daf40a`  
		Last Modified: Tue, 23 May 2023 01:39:10 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
