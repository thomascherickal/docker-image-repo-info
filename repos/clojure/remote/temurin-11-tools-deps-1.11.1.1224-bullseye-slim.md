## `clojure:temurin-11-tools-deps-1.11.1.1224-bullseye-slim`

```console
$ docker pull clojure@sha256:a68a3e6c34d7e4c61d14fd98a5c52a66784530f82080a70e77f3c424d30fbb52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `clojure:temurin-11-tools-deps-1.11.1.1224-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:35aa6ad7fa287e54f89a7267082c6d450e0c0adb2ee3fdaedc8f49656fdb20fe
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.9 MB (286901741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dd99397f898e28c59210416a8691117c902130475f020c4c2a3a4c6c7f26931`
-	Default Command: `["clj"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:18:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:21:30 GMT
COPY dir:b661686bf8d434588756c45f2ef6e7f314f32f753cf180ef8fb45397388f098c in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:21:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 13 Feb 2023 20:43:41 GMT
ENV CLOJURE_VERSION=1.11.1.1224
# Mon, 13 Feb 2023 20:43:41 GMT
WORKDIR /tmp
# Mon, 13 Feb 2023 20:43:55 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "3bbab4d253eda43e3122fd5705014a69c44944a6dee8ea4d7d567afe157eb4ef *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Mon, 13 Feb 2023 20:43:55 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Mon, 13 Feb 2023 20:43:56 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0acf483a916e651ca447c4add0da489b56284ef3ab648f7c4b8b28762f912a1e`  
		Last Modified: Thu, 09 Feb 2023 09:32:44 GMT  
		Size: 195.2 MB (195240411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae778bc7a63b01d01071484587984c8a597bc572d1bcd2fe7ca8e0f61bc6a6e`  
		Last Modified: Mon, 13 Feb 2023 20:51:56 GMT  
		Size: 61.6 MB (61598203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b8dc43ec59e79e76696c00e33ce0dee5def2f87b9befa12cb582a875d8df28`  
		Last Modified: Mon, 13 Feb 2023 20:51:50 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
