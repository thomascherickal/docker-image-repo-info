## `clojure:temurin-8-bullseye`

```console
$ docker pull clojure@sha256:6304e73950e8d15890de11bf00a15adcab7e7fd35076c139278301d98ac86900
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:53263d6bb7bdd78d27fe153c767eb2fb2a00ae5b91b5f537db47ff70022bfb29
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.4 MB (230414707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9499e23e4c08fc4340a506ab23c507a73bb8d486f40c3a3b4f2d54e3e0abe643`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:29 GMT
ADD file:917750a82b29f8f7f88a121017bd9dfeb0fbcc8f0697a009f08b6b58246eff4b in / 
# Wed, 11 Jan 2023 02:34:30 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:18:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 11 Jan 2023 03:18:58 GMT
COPY dir:53540f2d79f4eef9b2bf8c4b39ecdbbd82fb14bfcf951e14853afffd2efa2ecb in /opt/java/openjdk 
# Wed, 11 Jan 2023 03:18:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 03:21:41 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Wed, 11 Jan 2023 03:21:41 GMT
WORKDIR /tmp
# Wed, 11 Jan 2023 03:22:00 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 11 Jan 2023 03:22:01 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 11 Jan 2023 03:22:01 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:bbeef03cda1f5d6c9e20c310c1c91382a6b0a1a2501c3436b28152f13896f082`  
		Last Modified: Wed, 11 Jan 2023 02:38:42 GMT  
		Size: 55.0 MB (55025206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb0ac03ea060d862b95eed061f539ba623b94a8f2eb558fedded843bbe2bed3`  
		Last Modified: Wed, 11 Jan 2023 03:34:32 GMT  
		Size: 103.5 MB (103530609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed02605e7c3b046da147c20516d8db404376224910d77c4a3e4167d58e8cd4af`  
		Last Modified: Wed, 11 Jan 2023 03:35:32 GMT  
		Size: 71.9 MB (71858275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a49ab59ebc2c45a63b21239ede6c7ea13541d05c03ca04d73acb74dce511879f`  
		Last Modified: Wed, 11 Jan 2023 03:35:24 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:8fc4395892f8aa53c28cb8f4511a9cef2f95be480192302e11235cfa54a7dc09
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.3 MB (228288366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef2fa1526aed49a9f9ae03dc36984294f1ffc390a9ecc555f6dd71d3905dd7ea`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:24 GMT
ADD file:9e185c2d9ca8a231a39ee2b1761fcdff75065252d25a65a207acb7a319c1cf23 in / 
# Wed, 11 Jan 2023 02:57:25 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:14 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 11 Jan 2023 03:38:16 GMT
COPY dir:8a3fd802e7e57a45d80b19a89e91b421563b952585d39995819354f278317671 in /opt/java/openjdk 
# Wed, 11 Jan 2023 03:38:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 03:40:09 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Wed, 11 Jan 2023 03:40:09 GMT
WORKDIR /tmp
# Wed, 11 Jan 2023 03:40:23 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 11 Jan 2023 03:40:24 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 11 Jan 2023 03:40:24 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:c345c9e441f5f49235768af74b8ab37743652d38958afaa000edd56d7b2f0540`  
		Last Modified: Wed, 11 Jan 2023 03:00:56 GMT  
		Size: 53.7 MB (53681859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940f37610f026c5932e22a78105d91762ce8fc1b671393115df608bc205e894c`  
		Last Modified: Wed, 11 Jan 2023 03:50:57 GMT  
		Size: 102.6 MB (102626579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033acabcff05d179fe41ea43da5cf8f6ad9e14324675397f02bf1e63db405feb`  
		Last Modified: Wed, 11 Jan 2023 03:51:50 GMT  
		Size: 72.0 MB (71979313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a280e20e321a3ea3b3f56e772633a571c0e7ffb4cb35756b3f0f1ccc634404c`  
		Last Modified: Wed, 11 Jan 2023 03:51:44 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
