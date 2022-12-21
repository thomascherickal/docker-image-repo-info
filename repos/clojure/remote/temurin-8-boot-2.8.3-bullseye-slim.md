## `clojure:temurin-8-boot-2.8.3-bullseye-slim`

```console
$ docker pull clojure@sha256:09cd3addfc642f5573807ee28e98f1801359b6243627a4d4824dea4676ac3668
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-boot-2.8.3-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:0335ef55450f44ab3e9dd6de2024bc27c62eda97cdcd464254024e7e4789a78a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.8 MB (194825387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f17c5e95170d504a2eccb1a0d4378497d93eb562d49904ff749dd3f1e4cd21f4`
-	Default Command: `["boot","repl"]`

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
# Wed, 21 Dec 2022 01:51:08 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 21 Dec 2022 01:51:08 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 21 Dec 2022 01:51:08 GMT
WORKDIR /tmp
# Wed, 21 Dec 2022 01:51:14 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 21 Dec 2022 01:51:14 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 21 Dec 2022 01:51:14 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 21 Dec 2022 01:51:34 GMT
RUN boot
# Wed, 21 Dec 2022 01:51:34 GMT
CMD ["boot" "repl"]
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
	-	`sha256:f15c459d35c0f0ca505a1f3581ef4e4339f94204b3367a3d7d4b6c65cd4d286f`  
		Last Modified: Wed, 21 Dec 2022 02:05:18 GMT  
		Size: 1.1 MB (1077370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07fb038a96a78f8589d379f337ecb3313e2ff3edec01184ff52c6c98489a73a6`  
		Last Modified: Wed, 21 Dec 2022 02:05:22 GMT  
		Size: 58.8 MB (58820455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-boot-2.8.3-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:838cd5bded7f3b012c61bf666cc936f134be3970b20566c12f7056b113f8f214
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.6 MB (192556554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba0bfa83eb5192371c060befa97da45c2a75a02ebb0be4f2f4339f63c6c28cf6`
-	Default Command: `["boot","repl"]`

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
# Wed, 21 Dec 2022 02:18:42 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 21 Dec 2022 02:18:42 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 21 Dec 2022 02:18:42 GMT
WORKDIR /tmp
# Wed, 21 Dec 2022 02:18:47 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 21 Dec 2022 02:18:47 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 21 Dec 2022 02:18:47 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 21 Dec 2022 02:19:05 GMT
RUN boot
# Wed, 21 Dec 2022 02:19:05 GMT
CMD ["boot" "repl"]
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
	-	`sha256:09210ebbb35c4079ebece665b29f0fb8dd4f3252340c448949c0540408a4aa5e`  
		Last Modified: Wed, 21 Dec 2022 02:30:49 GMT  
		Size: 1.1 MB (1064645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6860ebc808f53d810e4787359d161f7f8a0e5c60ef7e635a09239098d7228d5e`  
		Last Modified: Wed, 21 Dec 2022 02:30:52 GMT  
		Size: 58.8 MB (58820551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
