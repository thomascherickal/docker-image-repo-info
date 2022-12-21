## `clojure:temurin-8-boot-bullseye`

```console
$ docker pull clojure@sha256:751b37e626f08744f1bfa9163747b80051768baefafd2c670fa44b1e80c33a12
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:37bd080d02db71cfcef961a95473b903247603a122018575f68175ee5be41517
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.7 MB (219737556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7698576a0421f6347f154f062907471a316966f2e91108014034e2b4887378ad`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:21 GMT
ADD file:c13b430c8699df107ffd9ea5230b92238bc037a8e1cbbe35d6ab664941d575da in / 
# Wed, 21 Dec 2022 01:20:22 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:50:07 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 21 Dec 2022 01:50:10 GMT
COPY dir:53540f2d79f4eef9b2bf8c4b39ecdbbd82fb14bfcf951e14853afffd2efa2ecb in /opt/java/openjdk 
# Wed, 21 Dec 2022 01:50:11 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 21 Dec 2022 01:50:11 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 21 Dec 2022 01:50:11 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 21 Dec 2022 01:50:12 GMT
WORKDIR /tmp
# Wed, 21 Dec 2022 01:50:18 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 21 Dec 2022 01:50:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 21 Dec 2022 01:50:18 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 21 Dec 2022 01:51:02 GMT
RUN boot
# Wed, 21 Dec 2022 01:51:03 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:32de3c850997ce03b6ff4ae8fb00b34b9d7d7f9a35bfcdb8538e22cc7b77c29d`  
		Last Modified: Wed, 21 Dec 2022 01:24:10 GMT  
		Size: 55.0 MB (55025166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81441fc84c30ecd83d6155d0413d2d8a8941b7d8adaa0d20178da27d0be26b86`  
		Last Modified: Wed, 21 Dec 2022 02:05:09 GMT  
		Size: 103.5 MB (103530611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ef34da7201b0b05c9e54d5845e19aa063023cc92222471daf4ca6a66cf547c`  
		Last Modified: Wed, 21 Dec 2022 02:05:01 GMT  
		Size: 2.4 MB (2360808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def13f5b577607edf025eb9f1f43d5bb14298be8f5d1dfbec55bde447bddfc48`  
		Last Modified: Wed, 21 Dec 2022 02:05:05 GMT  
		Size: 58.8 MB (58820971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:0f8385bf32e13a3560dd1e4a826fd38a4bde49432a8d1d9bc71225cbbf07b5b7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.5 MB (217479407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4239fd291d313a6c36a2ad9aed58967fb3adb28fcafd6236b8298e09091504f`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:40 GMT
ADD file:5bbdc914ec8ed60ac85293e88ee1aafc3f0290762e320fc86dc9d79fa201834e in / 
# Wed, 21 Dec 2022 01:39:41 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:18:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 21 Dec 2022 02:18:06 GMT
COPY dir:8a3fd802e7e57a45d80b19a89e91b421563b952585d39995819354f278317671 in /opt/java/openjdk 
# Wed, 21 Dec 2022 02:18:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 21 Dec 2022 02:18:09 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 21 Dec 2022 02:18:09 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 21 Dec 2022 02:18:09 GMT
WORKDIR /tmp
# Wed, 21 Dec 2022 02:18:14 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 21 Dec 2022 02:18:14 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 21 Dec 2022 02:18:14 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 21 Dec 2022 02:18:34 GMT
RUN boot
# Wed, 21 Dec 2022 02:18:34 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:c3e6129b48b69d14c5e7a5605e2b94003fb71aac82eac46b8689f5b8007af2c5`  
		Last Modified: Wed, 21 Dec 2022 01:42:49 GMT  
		Size: 53.7 MB (53681797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6100ae9251c3fa47a7e33ea8291f08f02fc3029cfa40a52f572ccce640a5978`  
		Last Modified: Wed, 21 Dec 2022 02:30:41 GMT  
		Size: 102.6 MB (102626555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3baa29662d8bc4ab6519427cafbb60d58508a68d72cf1330c22e407b0e47b0`  
		Last Modified: Wed, 21 Dec 2022 02:30:33 GMT  
		Size: 2.4 MB (2350654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da7fbb776144b6e58861547ee2fc634bcda15d2d80f3a88f7ad2c4c6757de9b9`  
		Last Modified: Wed, 21 Dec 2022 02:30:36 GMT  
		Size: 58.8 MB (58820401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
