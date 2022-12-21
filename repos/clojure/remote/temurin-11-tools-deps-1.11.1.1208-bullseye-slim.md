## `clojure:temurin-11-tools-deps-1.11.1.1208-bullseye-slim`

```console
$ docker pull clojure@sha256:c124b2d7794871521075a7b6e4539b22ebaa643ee6a73ffa65093712be4843bf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-tools-deps-1.11.1.1208-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:17adc13c9438763316090684ef5ef440ab9b88d90c93c4e9e77dfc28b9bca7db
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.3 MB (291335297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd03ad1bc17d0015a982ecbed64b9158b87ac945edfccd8a40fd932327f1a3a5`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:32 GMT
ADD file:73e68ae6852c9afbb2989dc9c5b7c6668843f454b1bdcfb48658bfbc6c4af69e in / 
# Wed, 21 Dec 2022 01:20:33 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:51:06 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 21 Dec 2022 01:54:03 GMT
COPY dir:a503569ef9354f7d11d0273f2ab0ff91f3e5c47f548dc54f07c58e44ff27a8a0 in /opt/java/openjdk 
# Wed, 21 Dec 2022 01:54:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 21 Dec 2022 01:55:53 GMT
ENV CLOJURE_VERSION=1.11.1.1200
# Wed, 21 Dec 2022 01:55:53 GMT
WORKDIR /tmp
# Wed, 21 Dec 2022 01:56:11 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "694381cb78d44f143bdcc38657507f012ebac4009bc57cec67abef1675447878 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 21 Dec 2022 01:56:11 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 21 Dec 2022 01:56:11 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:3f4ca61aafcd4fc07267a105067db35c0f0ac630e1970f3cd0c7bf552780e985`  
		Last Modified: Wed, 21 Dec 2022 01:24:36 GMT  
		Size: 31.4 MB (31396943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6db9c94a4957a1754107e38ff03b70c980e609a9f349a218009678a8917b1b7`  
		Last Modified: Wed, 21 Dec 2022 02:07:20 GMT  
		Size: 198.5 MB (198454552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436f35d56efc9ffb14f7683894ac86261e76a8c50ba2519ccab9e1cf22adb3e5`  
		Last Modified: Wed, 21 Dec 2022 02:08:19 GMT  
		Size: 61.5 MB (61483184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588bf10a4352aef0528250c3efb34c6b81448b7286246a7e183f0262f8e6143f`  
		Last Modified: Wed, 21 Dec 2022 02:08:11 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-tools-deps-1.11.1.1208-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:f213b001a56fc896613adbec805af2864498fcb7b1f6dac2e581a04d8bbca838
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.9 MB (286851583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc3b67a83ec32fd26faca6858afb294587ae04703cf88fe58f068bc29a8a7c95`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:48 GMT
ADD file:3ff0cc8d111595978eb50cdba91144382ce083c400d45785d53dbb03615a4890 in / 
# Wed, 21 Dec 2022 01:39:48 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:18:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 21 Dec 2022 02:21:14 GMT
COPY dir:e387a3b68139ff88bdac27d5ce097fc680f3cae9fdd88c28cdd91a06f9205180 in /opt/java/openjdk 
# Wed, 21 Dec 2022 02:21:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 21 Dec 2022 02:22:50 GMT
ENV CLOJURE_VERSION=1.11.1.1200
# Wed, 21 Dec 2022 02:22:50 GMT
WORKDIR /tmp
# Wed, 21 Dec 2022 02:23:04 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "694381cb78d44f143bdcc38657507f012ebac4009bc57cec67abef1675447878 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 21 Dec 2022 02:23:05 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 21 Dec 2022 02:23:05 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:4b7f5b2a311310809ab89d92f6f71b0462722fe855d3b92c93098a528aa08791`  
		Last Modified: Wed, 21 Dec 2022 01:43:12 GMT  
		Size: 30.0 MB (30044772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:418e472fbc1e675c21a46f7fc728e7299e4becc0622adce50ed53160c548c7f0`  
		Last Modified: Wed, 21 Dec 2022 02:32:36 GMT  
		Size: 195.2 MB (195203361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05207a973a92f0b5016e2d85d1f7bb95a65ab2f97c9c045c6bb2bacc0e0f0baa`  
		Last Modified: Wed, 21 Dec 2022 02:33:30 GMT  
		Size: 61.6 MB (61602830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb5e66b32b620be516bc1476eef55986cb7d4855d1d210ed6ccfd64ebf19caf`  
		Last Modified: Wed, 21 Dec 2022 02:33:23 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
