## `clojure:temurin-11-tools-deps-1.11.1.1429-bookworm-slim`

```console
$ docker pull clojure@sha256:5193c9f3be144d8a65a252e826530eb657f3778ba04c55dff1d6c7dca8bb4f97
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-11-tools-deps-1.11.1.1429-bookworm-slim` - linux; amd64

```console
$ docker pull clojure@sha256:efc3f1d3ac2ca25ea5df93af9b892ea970ad9fa2291240500c714f722416f910
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.6 MB (246560767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7704f900bc0318897340c45a0a21e544be3a7797de414b2ddbbf858f9a5ccb1b`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:37 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 21 Nov 2023 05:21:37 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:08:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 09:54:40 GMT
COPY dir:d20aeb749bf0b3fe533952f7903b6aa08724fe8bf03e369130d4e2a6ff71bd3f in /opt/java/openjdk 
# Sat, 02 Dec 2023 09:54:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 18:26:25 GMT
ENV CLOJURE_VERSION=1.11.1.1429
# Tue, 05 Dec 2023 18:26:25 GMT
WORKDIR /tmp
# Tue, 05 Dec 2023 18:26:43 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "bf08cfeb007118b7277aa7423734f5d507604b868f7fc44c0f9929ca9cd94ed4 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 05 Dec 2023 18:26:44 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 05 Dec 2023 18:26:44 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4050ac330d97fd84a1d6329cccff3c6d67aeace4dadb496e6d7467c8568e3c1`  
		Last Modified: Sat, 02 Dec 2023 10:14:01 GMT  
		Size: 145.3 MB (145266397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f82d47d6eafa50f9f78b91e929a11c1d1a07100eb55f2b58ee37498be1ce51c`  
		Last Modified: Tue, 05 Dec 2023 18:38:40 GMT  
		Size: 72.1 MB (72143844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790feafe2d7065fdc539bb286158b9f400e3e148807a83ac2a1d4d0327f7dd73`  
		Last Modified: Tue, 05 Dec 2023 18:38:31 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
