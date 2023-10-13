## `clojure:temurin-11-bookworm-slim`

```console
$ docker pull clojure@sha256:9a362f3b741193177e79399c06d9231946c6ba1db72a63991fd99a2e5ca7e353
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-bookworm-slim` - linux; amd64

```console
$ docker pull clojure@sha256:35f4d4b3fd4fe5f500adefc28b41b83f9850ae834c626be500854af03afa92c5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.9 MB (245909995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db21d5699849b611a166edd2bf88aecb7970dba5923dd4ba89515fda9c31fa7f`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:50 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Wed, 11 Oct 2023 18:34:51 GMT
CMD ["bash"]
# Fri, 13 Oct 2023 01:28:06 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 13 Oct 2023 12:44:27 GMT
COPY dir:2526dfaf6aedccef54b8de2f87890e86c6d3fe8431985d8e74dcfc29195b01ed in /opt/java/openjdk 
# Fri, 13 Oct 2023 12:44:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 12:50:04 GMT
ENV CLOJURE_VERSION=1.11.1.1413
# Fri, 13 Oct 2023 12:50:04 GMT
WORKDIR /tmp
# Fri, 13 Oct 2023 12:50:22 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "ad9aa1e99c59a4f7eb66450914fbec543337d9fada60dd9d34eec7fe18ae4965 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 13 Oct 2023 12:50:23 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 13 Oct 2023 12:50:23 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58d686df0429bc899b9ad25527714341a548bd057ccf4c6c39ca10ffcf2b6a5`  
		Last Modified: Fri, 13 Oct 2023 13:05:13 GMT  
		Size: 144.8 MB (144826195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9681492da69a52788161d062f888f62d603ab4b1b60c1375d3a34e9a02d669e7`  
		Last Modified: Fri, 13 Oct 2023 13:08:12 GMT  
		Size: 71.9 MB (71933307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161fe7a23eb249e620e35fe523c0b120eea833cdb2309694db8cbc7d82641fd7`  
		Last Modified: Fri, 13 Oct 2023 13:08:03 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-bookworm-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:07ba8bd2edadfe70cc1930e5f2b2e9f4a2d61755c6fcff761db0b46acdba35ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.4 MB (242445260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:796430627e786045cf447e3521749674b1ad3ca0bc49bb1f045934aeac9dce6e`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:51 GMT
ADD file:5c81bfc00a28feb4079c0daa743f829a6a5bbc1a9d40a890cb49e420539a7f15 in / 
# Wed, 11 Oct 2023 18:24:51 GMT
CMD ["bash"]
# Fri, 13 Oct 2023 00:59:51 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 13 Oct 2023 10:12:35 GMT
COPY dir:b4903e9e1c2782550c5bca9cb7b0f840b4fdb810848e07ca44af328ac9dd84f6 in /opt/java/openjdk 
# Fri, 13 Oct 2023 10:12:38 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 10:17:08 GMT
ENV CLOJURE_VERSION=1.11.1.1413
# Fri, 13 Oct 2023 10:17:08 GMT
WORKDIR /tmp
# Fri, 13 Oct 2023 10:17:23 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "ad9aa1e99c59a4f7eb66450914fbec543337d9fada60dd9d34eec7fe18ae4965 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 13 Oct 2023 10:17:24 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 13 Oct 2023 10:17:24 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:1bc163a14ea6a886d1d0f9a9be878b1ffd08a9311e15861137ccd85bb87190f9`  
		Last Modified: Wed, 11 Oct 2023 18:28:28 GMT  
		Size: 29.2 MB (29179284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e7aa7d3902d954c470f86fe2b38acaf6172ca287d14a276c679a36a75e4824`  
		Last Modified: Fri, 13 Oct 2023 10:29:43 GMT  
		Size: 141.6 MB (141570614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b642d5b988c5e334ca844046c7ad8a41ec8a3b93e39883c19ebd6c80f8a79e`  
		Last Modified: Fri, 13 Oct 2023 10:32:26 GMT  
		Size: 71.7 MB (71694744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdfd3604183cdc5196176bb595660ca21eafe2e6941946d7682d1dc8aeeadcc5`  
		Last Modified: Fri, 13 Oct 2023 10:32:17 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
