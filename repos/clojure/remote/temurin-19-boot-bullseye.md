## `clojure:temurin-19-boot-bullseye`

```console
$ docker pull clojure@sha256:67c591a2850e531943d47f3738ba65ea4e3a45d6fd608c37779af1f1a6ebdd20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:3f2b4cd5a82b81384adde8f909c3f86c802553e8cfb0161a036f3e35c4a8cf37
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.3 MB (317310301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fab26d4664ffaa2d3a68b3701f60699d6e5d7f85196f2afd0ed36887d15ecc6`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:21 GMT
ADD file:c13b430c8699df107ffd9ea5230b92238bc037a8e1cbbe35d6ab664941d575da in / 
# Wed, 21 Dec 2022 01:20:22 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:50:07 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 21 Dec 2022 01:59:28 GMT
COPY dir:fef581854733ec7202f8c807463b9e1952aeb6c7a002719c7e54987e50ea4dcb in /opt/java/openjdk 
# Wed, 21 Dec 2022 01:59:30 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 21 Dec 2022 01:59:30 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 21 Dec 2022 01:59:30 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 21 Dec 2022 01:59:30 GMT
WORKDIR /tmp
# Wed, 21 Dec 2022 01:59:36 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 21 Dec 2022 01:59:36 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 21 Dec 2022 01:59:36 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 21 Dec 2022 01:59:56 GMT
RUN boot
# Wed, 21 Dec 2022 01:59:56 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 21 Dec 2022 01:59:56 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 21 Dec 2022 01:59:56 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:32de3c850997ce03b6ff4ae8fb00b34b9d7d7f9a35bfcdb8538e22cc7b77c29d`  
		Last Modified: Wed, 21 Dec 2022 01:24:10 GMT  
		Size: 55.0 MB (55025166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d80e226f52e65f91550fee64cdd6a467c4da00bac7bed86c44aa550b443f1d`  
		Last Modified: Wed, 21 Dec 2022 02:10:56 GMT  
		Size: 201.1 MB (201103393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e754739fc0e1bf4f36d451e74a4c9fb186056451a4c97fc329c15bc2e54755`  
		Last Modified: Wed, 21 Dec 2022 02:10:41 GMT  
		Size: 2.4 MB (2360818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea8d601246dd8a92c25606aa7076f9e1b3e5cc3fd191e6d8ec478eac4fe6a1df`  
		Last Modified: Wed, 21 Dec 2022 02:10:44 GMT  
		Size: 58.8 MB (58820522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d79ed0981aab55e215fe98037cd80c2c7a9c89833da441cc46a7cf1bd28a1a`  
		Last Modified: Wed, 21 Dec 2022 02:10:40 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:a12b43a85e24463213b2acc776c3329ebfafec22d1399cdbb6522533e2b7460a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.7 MB (314717737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06bd749c2d50a10b0ab70f91009671a39e48f596ef506bdc2a2c1bd158ea3aa6`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:40 GMT
ADD file:5bbdc914ec8ed60ac85293e88ee1aafc3f0290762e320fc86dc9d79fa201834e in / 
# Wed, 21 Dec 2022 01:39:41 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:18:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 21 Dec 2022 02:25:44 GMT
COPY dir:4138443eebfda1a2a245638d5bb568645bd34d79b66d39a3be31b5ac6b823d6d in /opt/java/openjdk 
# Wed, 21 Dec 2022 02:25:49 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 21 Dec 2022 02:25:49 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 21 Dec 2022 02:25:49 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 21 Dec 2022 02:25:49 GMT
WORKDIR /tmp
# Wed, 21 Dec 2022 02:25:54 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 21 Dec 2022 02:25:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 21 Dec 2022 02:25:54 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 21 Dec 2022 02:26:11 GMT
RUN boot
# Wed, 21 Dec 2022 02:26:11 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 21 Dec 2022 02:26:12 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 21 Dec 2022 02:26:12 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:c3e6129b48b69d14c5e7a5605e2b94003fb71aac82eac46b8689f5b8007af2c5`  
		Last Modified: Wed, 21 Dec 2022 01:42:49 GMT  
		Size: 53.7 MB (53681797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5504f1730ed4e1dc3a15ab910d7a54c44be3b7eaa38521d40d2d6396a25c2b74`  
		Last Modified: Wed, 21 Dec 2022 02:35:43 GMT  
		Size: 199.9 MB (199864404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801f1853010684e3f0dc5dce2747af4acbb8a255c79ebfd3eead69984fbc256e`  
		Last Modified: Wed, 21 Dec 2022 02:35:30 GMT  
		Size: 2.4 MB (2350687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5257cdfb79c831515cd23ff921821b515b78b4e700dc59c27d43f6d67548a55`  
		Last Modified: Wed, 21 Dec 2022 02:35:33 GMT  
		Size: 58.8 MB (58820447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:310ae8b69834bbd415d242d70d1dba1019edf48f56576a0cc59562e9fb144da5`  
		Last Modified: Wed, 21 Dec 2022 02:35:30 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
