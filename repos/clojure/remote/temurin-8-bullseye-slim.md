## `clojure:temurin-8-bullseye-slim`

```console
$ docker pull clojure@sha256:acb472ff69507b9a70668d93e2821b25238fb416b989f15d2b5f124d9912ca70
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:c877c11e23390d597542a89248a0c124eb8594d29b736be8d0d339207ac339ea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.5 MB (147530690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea46608a7e6d5c29410bf3c81064222e01565032d41be5584d9d7090e744ff0a`
-	Default Command: `["clj"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:22:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:22:39 GMT
COPY dir:bbb84183d7ea38d81d8401f01e29d08935ee4c8bf6f90c6527579a1554c3bde1 in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:22:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 09:24:30 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Thu, 09 Feb 2023 09:24:30 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:24:47 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 09 Feb 2023 09:24:48 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 09 Feb 2023 09:24:48 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff09d33db7932dfdb13e1ebfdd9d02620a26713de0236d8aef1f5d2e115b133`  
		Last Modified: Thu, 09 Feb 2023 09:36:59 GMT  
		Size: 54.6 MB (54635563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cb1e9c501b5f14af311daf78aff2557cbe7eec3cbc1ebbe19fd420b5e06c469`  
		Last Modified: Thu, 09 Feb 2023 09:37:57 GMT  
		Size: 61.5 MB (61482698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a1e7bd141809c7ecdc35e99e674882e84777bdf02b6f5486c532e3732953f5`  
		Last Modified: Thu, 09 Feb 2023 09:37:49 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:dec64cecc2181db49074fe9a130c90b8ec70de38ae4b5c98cd5d73519777f06d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.4 MB (145388393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a75a73e9a12e5ea058e7c1b0e099520b803854714b4c1841547b2adf760b492c`
-	Default Command: `["clj"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:18:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:18:59 GMT
COPY dir:b6d7e5613532d986930216de9e0fece0632e82564ce7a6a98baf63b4115f840d in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:19:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 09:20:34 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Thu, 09 Feb 2023 09:20:34 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:20:48 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 09 Feb 2023 09:20:48 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 09 Feb 2023 09:20:48 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd68f0bab68b42136c4251287a12f055f74853a5f1d694a98637f9f09e4ed94`  
		Last Modified: Thu, 09 Feb 2023 09:31:02 GMT  
		Size: 53.7 MB (53727919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c478da5dcf973862e3902394110fd2a69339edeb253173800e2beb4a05ce3996`  
		Last Modified: Thu, 09 Feb 2023 09:31:57 GMT  
		Size: 61.6 MB (61597348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6af08af612af1b2286e6c50fc98f8407394477d59d29c6ce0e4c1c6f397f98`  
		Last Modified: Thu, 09 Feb 2023 09:31:51 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
