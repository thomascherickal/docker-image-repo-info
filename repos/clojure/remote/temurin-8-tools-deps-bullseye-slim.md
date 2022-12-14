## `clojure:temurin-8-tools-deps-bullseye-slim`

```console
$ docker pull clojure@sha256:6c5e4ad34113a6a858dcc14ac185613fccf34b64abb3ac61acefc0ddfca0e935
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-tools-deps-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:94ebdf70bb7f3e5fd217b434ee5eb52e8d694c93dfd634d6d8371b72fcfc9543
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.4 MB (196420834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10193d0c404a08c28366bdb2c486bc0255ee01ec384618838dd87f91b3ffce1f`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 06 Dec 2022 01:49:18 GMT
COPY dir:53540f2d79f4eef9b2bf8c4b39ecdbbd82fb14bfcf951e14853afffd2efa2ecb in /opt/java/openjdk 
# Tue, 06 Dec 2022 01:49:19 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Dec 2022 00:20:39 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Wed, 14 Dec 2022 00:20:39 GMT
WORKDIR /tmp
# Wed, 14 Dec 2022 00:21:04 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 14 Dec 2022 00:21:04 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 14 Dec 2022 00:21:04 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4affc3cd73f667de2263e106409ed3d854f8bd2cd76ecd0a5e3aca312c862bff`  
		Last Modified: Tue, 06 Dec 2022 02:03:39 GMT  
		Size: 103.5 MB (103530647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c535312239e80690eeb522063cac3fde7cee485c84e28c36fcc31087e1e6f75`  
		Last Modified: Wed, 14 Dec 2022 00:28:41 GMT  
		Size: 61.5 MB (61476717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b4a2ab6e7a189d15ca146f77bffa3188faa2f2f63e472c8bc603ed3bdde9cfd`  
		Last Modified: Wed, 14 Dec 2022 00:28:34 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-tools-deps-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:f009cf6f75a9f7682e0b5e32f8a22ba81430a9a31d6a9abd3fe70518ac0c640f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.3 MB (194284902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c103bd4f2efddbc3ae50c44dbce5a2d1571bc5ccc51378a05195972aaa9193b9`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 06 Dec 2022 02:17:49 GMT
COPY dir:8a3fd802e7e57a45d80b19a89e91b421563b952585d39995819354f278317671 in /opt/java/openjdk 
# Tue, 06 Dec 2022 02:17:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Dec 2022 00:40:05 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Wed, 14 Dec 2022 00:40:05 GMT
WORKDIR /tmp
# Wed, 14 Dec 2022 00:40:23 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 14 Dec 2022 00:40:23 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 14 Dec 2022 00:40:23 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5df8fef8a794006d98d0afa5f4cd031bef7bb0b991129e393fd59e5565be509`  
		Last Modified: Tue, 06 Dec 2022 02:30:13 GMT  
		Size: 102.6 MB (102626601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2710e4447a41144de190fa4a2f92842bbb79d981a4921e7e1ba2dc6735bb64`  
		Last Modified: Wed, 14 Dec 2022 00:46:48 GMT  
		Size: 61.6 MB (61597362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455384b9fae87f37c4ddf98e6d1683a45b6b07777704f26e2fe5e70c57b9191e`  
		Last Modified: Wed, 14 Dec 2022 00:46:42 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
