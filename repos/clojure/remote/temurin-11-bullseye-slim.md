## `clojure:temurin-11-bullseye-slim`

```console
$ docker pull clojure@sha256:57ecb82fa6b051f62854ead38ff3ee6ad473b976365f70a6db40f7407ac81b41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:ab29a101e2addc594760b2ed726cf5ce1ee9836269a51c27d12916d8ef076c8a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.4 MB (291352386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f57a908f1e914393548823c30a6c8e9a1069e98967bf06a8efdd54edfca3d96`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 06:36:55 GMT
COPY dir:a503569ef9354f7d11d0273f2ab0ff91f3e5c47f548dc54f07c58e44ff27a8a0 in /opt/java/openjdk 
# Fri, 09 Dec 2022 06:36:57 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 06:40:24 GMT
ENV CLOJURE_VERSION=1.11.1.1200
# Fri, 09 Dec 2022 06:40:24 GMT
WORKDIR /tmp
# Fri, 09 Dec 2022 06:40:45 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "694381cb78d44f143bdcc38657507f012ebac4009bc57cec67abef1675447878 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 09 Dec 2022 06:40:45 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 09 Dec 2022 06:40:46 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e074be86582c3a50533f320f376beb62a648a78e56a194a87575eb0c67721bd`  
		Last Modified: Fri, 09 Dec 2022 06:53:53 GMT  
		Size: 198.5 MB (198454556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52ba6790c565599387aa53d29942a16f2d1262ad7f8aef98cf9547deb8c1b97`  
		Last Modified: Fri, 09 Dec 2022 06:55:37 GMT  
		Size: 61.5 MB (61484360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2687bad151fd51d680f443aa6d82763c1e733d94f0aa00c3339ce1402c75cfdc`  
		Last Modified: Fri, 09 Dec 2022 06:55:29 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:417c8792af237d88d9076596ad860f4f95af24393a76773e1838150171eb644d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.9 MB (286867961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b9eca53eb7c40cf954aec530c10e3d83fa8ead771e3ecac5059a994db1126f3`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 05:04:05 GMT
COPY dir:e387a3b68139ff88bdac27d5ce097fc680f3cae9fdd88c28cdd91a06f9205180 in /opt/java/openjdk 
# Fri, 09 Dec 2022 05:04:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 05:07:01 GMT
ENV CLOJURE_VERSION=1.11.1.1200
# Fri, 09 Dec 2022 05:07:01 GMT
WORKDIR /tmp
# Fri, 09 Dec 2022 05:07:16 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "694381cb78d44f143bdcc38657507f012ebac4009bc57cec67abef1675447878 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 09 Dec 2022 05:07:17 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 09 Dec 2022 05:07:17 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44bbb0380eb6b5cd1051003f5ce31baf496a9113c5e9927f76bcf714c433145`  
		Last Modified: Fri, 09 Dec 2022 05:18:38 GMT  
		Size: 195.2 MB (195203372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5b033cea9555aa75257684905e6ce2b2a5be921d7a3b96d799506068ad6dc2`  
		Last Modified: Fri, 09 Dec 2022 05:20:15 GMT  
		Size: 61.6 MB (61603652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83534886cc0526c9a4df6a2545d7ca04ba8907cd48698321497ec8450ed0bd12`  
		Last Modified: Fri, 09 Dec 2022 05:20:09 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
