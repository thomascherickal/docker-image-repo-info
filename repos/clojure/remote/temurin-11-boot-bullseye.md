## `clojure:temurin-11-boot-bullseye`

```console
$ docker pull clojure@sha256:977eb724ffb862ca9ae4f406feb2cf168d9a5742ed3c47d3fb85e0069d15d3cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:60163f87db0c866340a45b5a303067ad7acdb1cda85f58e86bacda3695e88770
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.1 MB (261065285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aebac534aed53c3177fe4b5043945688f3827ce7382bd8f15d8a314db56e3f44`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:57 GMT
ADD file:20f89ff93bfbd6c9fb1a97058a1f3de4485a8974e8a83892072c511fbd2e4134 in / 
# Wed, 16 Aug 2023 00:59:58 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:06 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 31 Aug 2023 23:22:26 GMT
COPY dir:9c2351d5d5cdf669213a7cfcfa52bd6bd8e9fc36b0a8e93328276d7280e1bab3 in /opt/java/openjdk 
# Thu, 31 Aug 2023 23:22:27 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 31 Aug 2023 23:22:27 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 31 Aug 2023 23:22:27 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 31 Aug 2023 23:22:27 GMT
WORKDIR /tmp
# Thu, 31 Aug 2023 23:22:34 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 31 Aug 2023 23:22:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 31 Aug 2023 23:22:34 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 31 Aug 2023 23:22:54 GMT
RUN boot
# Thu, 31 Aug 2023 23:22:54 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:6a70103cc499a199e10e379794c60aa524d9598587cc2bdfe2995642c2da8df7`  
		Last Modified: Wed, 16 Aug 2023 01:04:50 GMT  
		Size: 55.1 MB (55056621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab352bd56ec5464a5d56238b020eb3ec17516ac2525535fdf339dacbad129b6`  
		Last Modified: Thu, 31 Aug 2023 23:41:03 GMT  
		Size: 144.8 MB (144826073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6be63135f619b814c62d6a489e95881d1f61d43f285ef91104ee6d9b806faa0`  
		Last Modified: Thu, 31 Aug 2023 23:40:52 GMT  
		Size: 2.4 MB (2362203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ff43656f08df3911ff04ac4b977251f5aae5442128f1993d1d6edbb03f56ea`  
		Last Modified: Thu, 31 Aug 2023 23:40:55 GMT  
		Size: 58.8 MB (58820388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:180dc85a5c5617b5cb68447f7887c6a8ebe42fafab2f283dbb1003d62abb2aac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.4 MB (256447187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1784c706dc867f4aea147072f33baeb54a8cfa232c7962ebcc8aa050c99ea33`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:03 GMT
ADD file:8973cddb2d84a543b71001635599951bea6485a3526ae4ff916443b584864c83 in / 
# Tue, 15 Aug 2023 23:40:04 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:14 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Sep 2023 01:43:53 GMT
COPY dir:68819d2d348aedadecb99120d7ca4a63dcc1e3aa0bb526ecbd9925396c38234c in /opt/java/openjdk 
# Sat, 02 Sep 2023 01:43:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Sep 2023 01:43:56 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 02 Sep 2023 01:43:56 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 02 Sep 2023 01:43:56 GMT
WORKDIR /tmp
# Sat, 02 Sep 2023 01:44:02 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Sat, 02 Sep 2023 01:44:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 02 Sep 2023 01:44:03 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 02 Sep 2023 01:44:21 GMT
RUN boot
# Sat, 02 Sep 2023 01:44:22 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:e837d9f05c625de5b814b851adbc03559ba02ea7078f57c81a01e18fc65bf42b`  
		Last Modified: Tue, 15 Aug 2023 23:43:37 GMT  
		Size: 53.7 MB (53704779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e4e3a8bbfd2bdf093ae59fc74ef766b5e27c2748069f457d192d1719121d34`  
		Last Modified: Sat, 02 Sep 2023 01:53:12 GMT  
		Size: 141.6 MB (141570380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c5d1cd432757a32b7e23e3061b5bb2748eaa9dfedf7497d88be9e5e34540ca`  
		Last Modified: Sat, 02 Sep 2023 01:53:04 GMT  
		Size: 2.4 MB (2351483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb07bb527fd33975fe235895f466438f89f0ae1fbdb69eb8a00ee2d745c094c0`  
		Last Modified: Sat, 02 Sep 2023 01:53:06 GMT  
		Size: 58.8 MB (58820545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
