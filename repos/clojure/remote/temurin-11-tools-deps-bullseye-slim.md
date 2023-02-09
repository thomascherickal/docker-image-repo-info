## `clojure:temurin-11-tools-deps-bullseye-slim`

```console
$ docker pull clojure@sha256:2421dbe029a20279a0679614e66653831a47a8533c8cb20a1e75ce0277e380ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-tools-deps-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:f59d09598d683a9b4557f35760d96b8f1750f4e6e2f1d6392cc3486e7ea467f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.4 MB (291370749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecc25b06a3664b5ae8de6292b78b3ac7eb2f6172109c29cc0d3dbfdcbb4e5c7b`
-	Default Command: `["clj"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:22:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:25:37 GMT
COPY dir:fdbc5e9dec2946fa124877176e92a68dd3fe3a70def5bb906a6040c4a1303a2d in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:25:38 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 09:27:33 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Thu, 09 Feb 2023 09:27:33 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:27:50 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 09 Feb 2023 09:27:51 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 09 Feb 2023 09:27:51 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9435812fc8d62eb5597536e4d415bb190bf5bd388839bf4cae0567b76b0a6a`  
		Last Modified: Thu, 09 Feb 2023 09:38:48 GMT  
		Size: 198.5 MB (198475423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d8267a73b7f90fe9f86bb4d41f4f2b84ec48f83e6bd4d068eeef7cac9cb229`  
		Last Modified: Thu, 09 Feb 2023 09:39:48 GMT  
		Size: 61.5 MB (61482898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b9ea4d667173468dfb826473812590c5a399fe3c721f47bd6338934e291e2f`  
		Last Modified: Thu, 09 Feb 2023 09:39:40 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-tools-deps-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:97e6aadc9d15506e2ec7c49ab60db84827665d5cbec96d8374d492b890ced831
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.9 MB (286900883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7c60ff82867d940b73424aae394e348d03eebf407cd0da6e8240c8bc70e7774`
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
# Thu, 09 Feb 2023 09:23:03 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Thu, 09 Feb 2023 09:23:04 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:23:17 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 09 Feb 2023 09:23:17 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 09 Feb 2023 09:23:18 GMT
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
	-	`sha256:b4821e0f77060610e79023ea2eaed288965b7fe2355024c1adbf4053417fa739`  
		Last Modified: Thu, 09 Feb 2023 09:33:39 GMT  
		Size: 61.6 MB (61597342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d2864f65ab50e9ca42b77db3e790122afa5786a9508bc2eb172106718431dcc`  
		Last Modified: Thu, 09 Feb 2023 09:33:33 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
