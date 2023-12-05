## `clojure:temurin-21-tools-deps-1.11.1.1429-bookworm-slim`

```console
$ docker pull clojure@sha256:2917434938617d5b5c56939bc6e4f0a58e41e049c7943679a0d180ca3c6d7654
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-21-tools-deps-1.11.1.1429-bookworm-slim` - linux; amd64

```console
$ docker pull clojure@sha256:c1089dfdf3583f8d7f15b3c01f8f4d1bb9f4322c50c28fd4fbe9d72e82a85fb7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.9 MB (259925433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11c8b36999d02122b54a1046b86b8a50845b3a89a82c93c02a12518a8adf51b9`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:37 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 21 Nov 2023 05:21:37 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:08:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 21 Nov 2023 10:23:57 GMT
COPY dir:e6025cb107ac582823e7222bca84438ae7fa7384431777ac5a68b80c2a5b3d9d in /opt/java/openjdk 
# Tue, 21 Nov 2023 10:23:58 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 18:31:54 GMT
ENV CLOJURE_VERSION=1.11.1.1429
# Tue, 05 Dec 2023 18:31:55 GMT
WORKDIR /tmp
# Tue, 05 Dec 2023 18:32:13 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "bf08cfeb007118b7277aa7423734f5d507604b868f7fc44c0f9929ca9cd94ed4 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 05 Dec 2023 18:32:13 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 05 Dec 2023 18:32:14 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Tue, 05 Dec 2023 18:32:14 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 05 Dec 2023 18:32:14 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24fd0a65d057784fe5c633d71a2ead576b1fd12ec0e7f3546576a3b124756e78`  
		Last Modified: Tue, 21 Nov 2023 10:38:59 GMT  
		Size: 158.6 MB (158630529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176dcc87a2d3b741fec2713c3fc87b4c24ff4bd48ce39ac92486b511a2cac914`  
		Last Modified: Tue, 05 Dec 2023 18:43:29 GMT  
		Size: 72.1 MB (72143976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af85ba76035aa908643f957dca63aeb01a482a97d97e8ddf25a62497fd8c630`  
		Last Modified: Tue, 05 Dec 2023 18:43:21 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dec4367437db3d6d46ba9abc186fbdbeb2c1419ea6c61e32236215bf3d19241`  
		Last Modified: Tue, 05 Dec 2023 18:43:21 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
