## `clojure:temurin-8-tools-deps-bullseye`

```console
$ docker pull clojure@sha256:78d65801d2785a9f1260a2d221ee2bc940a3cf756b72d0fd846b777f53bd065a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-tools-deps-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:4ee114671d3a58b10ca71da06cc8fe5685bcd8b3d31ea01e535ba71744feb4aa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.6 MB (181570148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d2127ad46bcf86d6549466beb9aa938c6fded9819a9d24fbb4e992b6d094605`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 02 May 2023 23:46:50 GMT
ADD file:fc290cf8ddb984325474583faa79c5a98c5ea0ec7f606bf360251f63acecf389 in / 
# Tue, 02 May 2023 23:46:51 GMT
CMD ["bash"]
# Wed, 03 May 2023 20:24:09 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 03 May 2023 20:24:11 GMT
COPY dir:715eb4123a1bd94a1f232c902a6f3cdcc4011195a3e566c0f0ddc35dd1e83095 in /opt/java/openjdk 
# Wed, 03 May 2023 20:24:11 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 19 May 2023 20:25:02 GMT
ENV CLOJURE_VERSION=1.11.1.1323
# Fri, 19 May 2023 20:25:02 GMT
WORKDIR /tmp
# Fri, 19 May 2023 20:25:28 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "c4666f0e2c2397b91554befd71ff6149b2e89acbf90400e1dcf557526cfb593d *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 19 May 2023 20:25:28 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 19 May 2023 20:25:28 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:918547b9432687b1e1d238e82dc1e0ea0b736aafbf3c402eea98c6db81a9cb65`  
		Last Modified: Tue, 02 May 2023 23:49:58 GMT  
		Size: 55.0 MB (55049070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5e2c1247e792b32dfc253554b769e50b9d0e00b87bda347fdad278b672e1b2`  
		Last Modified: Wed, 03 May 2023 20:35:03 GMT  
		Size: 54.6 MB (54642112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b9da0a0ff52089db535c9e7bc69b147898d7403053f5f90eaa6f9cf99cabb3`  
		Last Modified: Fri, 19 May 2023 20:37:37 GMT  
		Size: 71.9 MB (71878349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51390ebb4de9332afca5c0750b02d17f8e173ff14a787dc0ab9c3c3d8c5da8b5`  
		Last Modified: Fri, 19 May 2023 20:37:29 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-tools-deps-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:0f905e640e2044cff6e39db899843d0b5015cac59eccfac6b667cf20983f4598
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.4 MB (179430625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dff64e6d5e22d05420107b8f9308752b6cd24ee91014380575bf454c6895862d`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 23 May 2023 00:43:08 GMT
ADD file:a823391455122220a061ff349b66ee33413e968447ec5ba4bd544d9182fa2fbe in / 
# Tue, 23 May 2023 00:43:08 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:24:09 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 23 May 2023 01:24:11 GMT
COPY dir:f6bbe63c81e220d954915791686219263d8c45918fd81b238f7c9f6b21f076f8 in /opt/java/openjdk 
# Tue, 23 May 2023 01:24:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 01:26:12 GMT
ENV CLOJURE_VERSION=1.11.1.1323
# Tue, 23 May 2023 01:26:12 GMT
WORKDIR /tmp
# Tue, 23 May 2023 01:26:32 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "c4666f0e2c2397b91554befd71ff6149b2e89acbf90400e1dcf557526cfb593d *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 23 May 2023 01:26:32 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 23 May 2023 01:26:32 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:b04fae59f135dd79280e4a6da39408e04c6d703c617cbcb1c524dfe6f2962fe5`  
		Last Modified: Tue, 23 May 2023 00:45:45 GMT  
		Size: 53.7 MB (53692612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fec933d3080ef0a9a725f147ed686986ad36ef60808bf5f0ed2091007522988c`  
		Last Modified: Tue, 23 May 2023 01:34:03 GMT  
		Size: 53.7 MB (53742673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4284139b7df9b1bcc0f769b7b1508600aa9b492b4b783c94825f23d8e97bbc2`  
		Last Modified: Tue, 23 May 2023 01:34:51 GMT  
		Size: 72.0 MB (71994726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805ca6238a8e097d81a2771ee02650dabed58043dca9a3577741800f7c96d4c8`  
		Last Modified: Tue, 23 May 2023 01:34:45 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
