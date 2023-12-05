## `clojure:temurin-8-tools-deps-1.11.1.1429-bookworm-slim`

```console
$ docker pull clojure@sha256:82255efc9c081a87d7d257bb751b2b8dbe6bb27382763aa48934f2fba128614c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-8-tools-deps-1.11.1.1429-bookworm-slim` - linux; amd64

```console
$ docker pull clojure@sha256:3a91d09bc2eec8e07bc0d9bd1ae2119eaabea31cfb4014e1f2aececc184c204f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.9 MB (204892742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2bfc2daa31204eb7067ee332fca56a62c0590d2263cf08563bd5313197580a5`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:37 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 21 Nov 2023 05:21:37 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:08:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 21 Nov 2023 10:09:00 GMT
COPY dir:a294625293e4e40913c98181a9aeff55bc5e737b728d424dfdc884f576bd8f8d in /opt/java/openjdk 
# Tue, 21 Nov 2023 10:09:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 18:23:01 GMT
ENV CLOJURE_VERSION=1.11.1.1429
# Tue, 05 Dec 2023 18:23:02 GMT
WORKDIR /tmp
# Tue, 05 Dec 2023 18:23:20 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "bf08cfeb007118b7277aa7423734f5d507604b868f7fc44c0f9929ca9cd94ed4 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 05 Dec 2023 18:23:21 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 05 Dec 2023 18:23:21 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea90c3a76d5ae0f9f3f2436cc57135b1df73c229285da25a50b8cae0bd84e9d5`  
		Last Modified: Tue, 21 Nov 2023 10:29:01 GMT  
		Size: 103.6 MB (103598255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e8f012c86892efcbae42e63945076a76ce3efe844b13d7b4d92d79c2b3fc5c`  
		Last Modified: Tue, 05 Dec 2023 18:36:20 GMT  
		Size: 72.1 MB (72143962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd3a4b725c655f7f7a965a25da3589a47326ba33855ce6cfaeebd41fb9e47d7`  
		Last Modified: Tue, 05 Dec 2023 18:36:12 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
