## `clojure:temurin-11-boot-2.8.3-bullseye-slim`

```console
$ docker pull clojure@sha256:486090a89a0a577a55096c99f2c9aca1ecff4ced6d007828fffeb9dea31bf59b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-2.8.3-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:2c3519d27544d9650e2c03ab3c0645e8b61b008f78b6e08e7f512a4101f6a5aa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.1 MB (236141867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13380c1c3ac7495c12708c05f177468dc04ef83c8358704d44a9bae44f11f660`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 31 Aug 2023 20:50:14 GMT
COPY dir:9c2351d5d5cdf669213a7cfcfa52bd6bd8e9fc36b0a8e93328276d7280e1bab3 in /opt/java/openjdk 
# Thu, 31 Aug 2023 23:22:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 31 Aug 2023 23:22:59 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 31 Aug 2023 23:22:59 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 31 Aug 2023 23:22:59 GMT
WORKDIR /tmp
# Thu, 31 Aug 2023 23:23:05 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 31 Aug 2023 23:23:05 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 31 Aug 2023 23:23:05 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 31 Aug 2023 23:23:24 GMT
RUN boot
# Thu, 31 Aug 2023 23:23:24 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d08bb3cc4c5f5565aedec30d167dd9f4534631431ccf2ef52db66770488b231`  
		Last Modified: Thu, 31 Aug 2023 20:54:04 GMT  
		Size: 144.8 MB (144826071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3cb6ad466ce885faf5048f936b61e36769c0a28b486edc05d0dacb2c2fa27a`  
		Last Modified: Thu, 31 Aug 2023 23:41:12 GMT  
		Size: 1.1 MB (1077567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653439b772b1a890046b63fdbd2c04f59a7e6d6d87cbec4b50c31b6bc08f3f9f`  
		Last Modified: Thu, 31 Aug 2023 23:41:15 GMT  
		Size: 58.8 MB (58820551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-2.8.3-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:119dc9699549818833ab18f4b2b6bde9b83470a7ae06823b8bf645254499648b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.5 MB (231518558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a517ea0b09f7eb1394516016085dd4d5088fb3f324c92e7bda0e68c66132b7e`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Sep 2023 01:44:25 GMT
COPY dir:68819d2d348aedadecb99120d7ca4a63dcc1e3aa0bb526ecbd9925396c38234c in /opt/java/openjdk 
# Sat, 02 Sep 2023 01:44:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Sep 2023 01:44:29 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 02 Sep 2023 01:44:29 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 02 Sep 2023 01:44:29 GMT
WORKDIR /tmp
# Sat, 02 Sep 2023 01:44:34 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Sat, 02 Sep 2023 01:44:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 02 Sep 2023 01:44:34 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 02 Sep 2023 01:44:53 GMT
RUN boot
# Sat, 02 Sep 2023 01:44:53 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b924b77d195ee682d4adf6c744cba3a607633e56b93e8e8d9161e1a29b17fc4c`  
		Last Modified: Sat, 02 Sep 2023 01:53:29 GMT  
		Size: 141.6 MB (141570383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52456ab1a7b8f3e40dc2f5930b0b715cac5442cf29aa839c059cc1d68272d66b`  
		Last Modified: Sat, 02 Sep 2023 01:53:21 GMT  
		Size: 1.1 MB (1064876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e52705d096e8881848a5becc6b8ff6fd77725844aa6f96e0ec4f39fbf70d6d`  
		Last Modified: Sat, 02 Sep 2023 01:53:23 GMT  
		Size: 58.8 MB (58820483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
