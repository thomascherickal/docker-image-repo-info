## `clojure:temurin-11-tools-deps-bullseye`

```console
$ docker pull clojure@sha256:7a5ab88b021f66933be9966cb4285927f05ecece16b9a1a0a30e9547b790fe6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-tools-deps-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:cb589e1efee29d27418376b4d8de42a6988a3243453a8d0d53396dc0f8b14a3c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.8 MB (300783617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf1f4b75ab441342824f3a1a370645ee34a10b643e0acc2a5063ae490fe2e530`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:21 GMT
ADD file:c13b430c8699df107ffd9ea5230b92238bc037a8e1cbbe35d6ab664941d575da in / 
# Wed, 21 Dec 2022 01:20:22 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:50:07 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 21 Dec 2022 01:53:31 GMT
COPY dir:a503569ef9354f7d11d0273f2ab0ff91f3e5c47f548dc54f07c58e44ff27a8a0 in /opt/java/openjdk 
# Wed, 21 Dec 2022 01:53:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 21 Dec 2022 01:55:33 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Wed, 21 Dec 2022 01:55:33 GMT
WORKDIR /tmp
# Wed, 21 Dec 2022 01:55:49 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 21 Dec 2022 01:55:49 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 21 Dec 2022 01:55:49 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:32de3c850997ce03b6ff4ae8fb00b34b9d7d7f9a35bfcdb8538e22cc7b77c29d`  
		Last Modified: Wed, 21 Dec 2022 01:24:10 GMT  
		Size: 55.0 MB (55025166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09879893307507e7fe968e99bda720fc4263e5da6b74edf0064ca1f992ab9605`  
		Last Modified: Wed, 21 Dec 2022 02:06:55 GMT  
		Size: 198.5 MB (198454573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7522fed89b4969173a78fe1952c205dad70b599d87d6c013ad6056415e5bff31`  
		Last Modified: Wed, 21 Dec 2022 02:08:00 GMT  
		Size: 47.3 MB (47303262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2a8e0ea00259461afbadbd57a0af8aa875b6c08883fbf8e6b210e8bdaf38d8`  
		Last Modified: Wed, 21 Dec 2022 02:07:54 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-tools-deps-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:c9dbb66f332a0543fa8148282534be38d239607525baf91038537d5cc19b6d36
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.2 MB (296178769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cc48c2f572cb468f150a508c5d3dc6ae63d20264a3c1229bfe210eedc85bca9`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:40 GMT
ADD file:5bbdc914ec8ed60ac85293e88ee1aafc3f0290762e320fc86dc9d79fa201834e in / 
# Wed, 21 Dec 2022 01:39:41 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:18:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 21 Dec 2022 02:20:42 GMT
COPY dir:e387a3b68139ff88bdac27d5ce097fc680f3cae9fdd88c28cdd91a06f9205180 in /opt/java/openjdk 
# Wed, 21 Dec 2022 02:20:46 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 21 Dec 2022 02:22:34 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Wed, 21 Dec 2022 02:22:34 GMT
WORKDIR /tmp
# Wed, 21 Dec 2022 02:22:46 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 21 Dec 2022 02:22:46 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 21 Dec 2022 02:22:46 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:c3e6129b48b69d14c5e7a5605e2b94003fb71aac82eac46b8689f5b8007af2c5`  
		Last Modified: Wed, 21 Dec 2022 01:42:49 GMT  
		Size: 53.7 MB (53681797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba82789481f43d21d6d2ece93afb47a4345ba46f2c082c71dcc84a5ef12fb90`  
		Last Modified: Wed, 21 Dec 2022 02:32:16 GMT  
		Size: 195.2 MB (195203346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb02a030aebc8b61df45da78980133fc2f3e374fe1c8d9b16eb282c3d05678b`  
		Last Modified: Wed, 21 Dec 2022 02:33:13 GMT  
		Size: 47.3 MB (47293007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd86956cb23ca0dbd8c2a3e379f9d9b2b79331c54f0d4af17d8c3334abfc3986`  
		Last Modified: Wed, 21 Dec 2022 02:33:08 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
