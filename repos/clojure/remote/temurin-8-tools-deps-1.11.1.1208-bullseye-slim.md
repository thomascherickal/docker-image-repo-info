## `clojure:temurin-8-tools-deps-1.11.1.1208-bullseye-slim`

```console
$ docker pull clojure@sha256:b2f90b0b77899e23c42635eb60f0082ea8271d5416ccdbd6d0bbf9ae079736bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-tools-deps-1.11.1.1208-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:fc86434e1ce6b315bdf0a9907c2225ad1ef5254a225ae001d165cb5ad7a038e9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.4 MB (196402719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfae7bee4891c9bf74bbd77b4fb86ea7196e04f28503f3efc3c6358132a626f1`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:32 GMT
ADD file:73e68ae6852c9afbb2989dc9c5b7c6668843f454b1bdcfb48658bfbc6c4af69e in / 
# Wed, 21 Dec 2022 01:20:33 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:51:06 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 21 Dec 2022 01:51:07 GMT
COPY dir:53540f2d79f4eef9b2bf8c4b39ecdbbd82fb14bfcf951e14853afffd2efa2ecb in /opt/java/openjdk 
# Wed, 21 Dec 2022 01:51:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 21 Dec 2022 01:52:58 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Wed, 21 Dec 2022 01:52:58 GMT
WORKDIR /tmp
# Wed, 21 Dec 2022 01:53:17 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 21 Dec 2022 01:53:17 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 21 Dec 2022 01:53:17 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:3f4ca61aafcd4fc07267a105067db35c0f0ac630e1970f3cd0c7bf552780e985`  
		Last Modified: Wed, 21 Dec 2022 01:24:36 GMT  
		Size: 31.4 MB (31396943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaa9331b7c1be2cd4339b5a6494af1557213ce63d328d2559ee407cadf3c9a05`  
		Last Modified: Wed, 21 Dec 2022 02:05:27 GMT  
		Size: 103.5 MB (103530619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eb321d518d6d6223e133ef6b28f7650c98b9c9696fd7c65bcb1eb7e60147f65`  
		Last Modified: Wed, 21 Dec 2022 02:06:25 GMT  
		Size: 61.5 MB (61474538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30425803d416c0cb2f200b3a66819c62bd7687242a1bcc72a623a2c1829bb01e`  
		Last Modified: Wed, 21 Dec 2022 02:06:17 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-tools-deps-1.11.1.1208-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:437d7e486075400b5d84e2fa59d3d6a4e2deb113e3a08a8b0777b0869145010e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.3 MB (194268359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9cc9df15a4c83b32f1b5d68234000c0efd7db6c42fd2f02002e03fef9961d00`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:48 GMT
ADD file:3ff0cc8d111595978eb50cdba91144382ce083c400d45785d53dbb03615a4890 in / 
# Wed, 21 Dec 2022 01:39:48 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:18:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 21 Dec 2022 02:18:39 GMT
COPY dir:8a3fd802e7e57a45d80b19a89e91b421563b952585d39995819354f278317671 in /opt/java/openjdk 
# Wed, 21 Dec 2022 02:18:42 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 21 Dec 2022 02:20:16 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Wed, 21 Dec 2022 02:20:16 GMT
WORKDIR /tmp
# Wed, 21 Dec 2022 02:20:31 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 21 Dec 2022 02:20:31 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 21 Dec 2022 02:20:31 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:4b7f5b2a311310809ab89d92f6f71b0462722fe855d3b92c93098a528aa08791`  
		Last Modified: Wed, 21 Dec 2022 01:43:12 GMT  
		Size: 30.0 MB (30044772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d47e381e4493cb18501cb04a7b8967399acfcff81143cd3425cada9baae403`  
		Last Modified: Wed, 21 Dec 2022 02:30:56 GMT  
		Size: 102.6 MB (102626586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4c1bcdc679ce425ba2ae9911fdb5a480e233c66125a389ff7cd06b7ec2e3c6`  
		Last Modified: Wed, 21 Dec 2022 02:31:51 GMT  
		Size: 61.6 MB (61596384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91af23a46bf679f753243f0bedddfda37f078d571533d85789a08abf3966ef63`  
		Last Modified: Wed, 21 Dec 2022 02:31:45 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
