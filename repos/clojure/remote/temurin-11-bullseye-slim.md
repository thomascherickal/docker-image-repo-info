## `clojure:temurin-11-bullseye-slim`

```console
$ docker pull clojure@sha256:f4b613f1eaae0fea183448c44c08600bd60a5ea1eaf10acdd5bddf435c1db2a7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:7d0c5ba30ad6f9bd51d5d81dda193f5b8476917ed580868acee988a26dfebc31
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.4 MB (291448514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad4ba049b0069cbd4fac71d033d8ebb28b205ebe277342e082dab7b08d65aa53`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 02 May 2023 23:46:59 GMT
ADD file:a2378c1b12e95db69e24b9d347441678c6f23239292cce3c822b1524992b6ec4 in / 
# Tue, 02 May 2023 23:47:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 20:24:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 14:55:29 GMT
COPY dir:480a3269dc817a8cead3ef1e03a246c3e173090658469b19c2165cafbd3da5de in /opt/java/openjdk 
# Thu, 04 May 2023 14:55:31 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 19 May 2023 20:28:58 GMT
ENV CLOJURE_VERSION=1.11.1.1323
# Fri, 19 May 2023 20:28:58 GMT
WORKDIR /tmp
# Fri, 19 May 2023 20:29:14 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "c4666f0e2c2397b91554befd71ff6149b2e89acbf90400e1dcf557526cfb593d *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 19 May 2023 20:29:15 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 19 May 2023 20:29:15 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:9e3ea8720c6de96cc9ad544dddc695a3ab73f5581c5d954e0504cc4f80fb5e5c`  
		Last Modified: Tue, 02 May 2023 23:50:22 GMT  
		Size: 31.4 MB (31403516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c8debf5f3c7bd7d820f2797f8d4cfc95b7902d0071ca115228b3f6eb2d872a`  
		Last Modified: Thu, 04 May 2023 15:06:32 GMT  
		Size: 198.5 MB (198549506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2e509042d73ee64dc4be2ae0c675e0dd57903e62533d55add2c9200f1ca351`  
		Last Modified: Fri, 19 May 2023 20:40:08 GMT  
		Size: 61.5 MB (61494874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5fae2b904afa3d428cdff2200765343ffa7b3412376b3f877c7a327077d102`  
		Last Modified: Fri, 19 May 2023 20:40:01 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:a437ee90c9f2028ec10a3eb8d2f49f46c14a8e5324b100ccbaf7b822374e536e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **287.0 MB (286986509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df2b821373f3a7f24629e34fc6b57530f78bccde160bf269164f4579fdb3acad`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:24:57 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 23 May 2023 01:27:27 GMT
COPY dir:377359689ec5fd1035465458ec6eb78fc3e8352f259756650a4953f3054fef1a in /opt/java/openjdk 
# Tue, 23 May 2023 01:27:31 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 01:28:58 GMT
ENV CLOJURE_VERSION=1.11.1.1323
# Tue, 23 May 2023 01:28:58 GMT
WORKDIR /tmp
# Tue, 23 May 2023 01:29:12 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "c4666f0e2c2397b91554befd71ff6149b2e89acbf90400e1dcf557526cfb593d *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 23 May 2023 01:29:12 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 23 May 2023 01:29:12 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d78c86840ae584aab4d9f49c5158125ceb03a9fcfcbb243c03ce4819b42d8729`  
		Last Modified: Tue, 23 May 2023 01:35:49 GMT  
		Size: 195.3 MB (195324209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28a994d481dea037fa7b14a4dfde2a8b44b5e5a5eba9fe853e49a19caa9021e`  
		Last Modified: Tue, 23 May 2023 01:36:40 GMT  
		Size: 61.6 MB (61608938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef8043ed32758ec3530e69404e44504f641e80b0be47273eef8edfc10a89d2e`  
		Last Modified: Tue, 23 May 2023 01:36:34 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
