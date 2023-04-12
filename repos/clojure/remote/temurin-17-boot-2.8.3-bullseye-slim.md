## `clojure:temurin-17-boot-2.8.3-bullseye-slim`

```console
$ docker pull clojure@sha256:c21a294647dd0a7153d156870df17f98c0073b967152de8ef4ddcab2f50d46da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-2.8.3-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:6bc6f64e23ee9f392fe599bb9408d01fd11f532f0195a6c76c1e54680e2180ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.8 MB (283754821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6599a3298edfb925455bf23f0ea5bf7e97e7e003f0dac84e34db1ec3b173ba9`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:11:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 08:16:43 GMT
COPY dir:d90c8d6564183f8aad11f93ecfb2f7e0eeff18588ff2b62d7ca3d8d30672bc2c in /opt/java/openjdk 
# Wed, 12 Apr 2023 08:16:45 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 08:16:45 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 12 Apr 2023 08:16:45 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 12 Apr 2023 08:16:45 GMT
WORKDIR /tmp
# Wed, 12 Apr 2023 08:16:50 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 12 Apr 2023 08:16:50 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 12 Apr 2023 08:16:51 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 12 Apr 2023 08:17:07 GMT
RUN boot
# Wed, 12 Apr 2023 08:17:07 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 12 Apr 2023 08:17:07 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 12 Apr 2023 08:17:08 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ddd9ea3ca0dd85f3af3e4aaaa2acdd08b9f289fab659372eedc7fd033de543c`  
		Last Modified: Wed, 12 Apr 2023 08:24:58 GMT  
		Size: 192.4 MB (192438264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bc2aa783461c2455ce30466db6d44e9bfb79562b9f74a368041a4b8bbb8375`  
		Last Modified: Wed, 12 Apr 2023 08:24:44 GMT  
		Size: 1.1 MB (1077517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dfa0bed35d73c82d60ff56e69c7049f4d73eee367f2681c5bda04145378893b`  
		Last Modified: Wed, 12 Apr 2023 08:24:48 GMT  
		Size: 58.8 MB (58820414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2344f048471578d4c77d65475cdc11b4d483ce84e198f55cd92a45eb1f7af4c`  
		Last Modified: Wed, 12 Apr 2023 08:24:44 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-2.8.3-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:2228e55ebd8ca571256030c232467566f6a4eb61d24a79db997f167fd526483b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.2 MB (281209881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37c81eb1277cab1f66e4e8f6be7ece9134b4e36ff0484d62bacdcae681a3c974`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 01:23:36 GMT
COPY dir:44544f5117ae50af040f98b1979efcc18f4c9f0c7257bfc4a37b80697337361a in /opt/java/openjdk 
# Wed, 12 Apr 2023 01:23:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 01:23:41 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 12 Apr 2023 01:23:41 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 12 Apr 2023 01:23:41 GMT
WORKDIR /tmp
# Wed, 12 Apr 2023 01:23:45 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 12 Apr 2023 01:23:45 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 12 Apr 2023 01:23:46 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 12 Apr 2023 01:24:03 GMT
RUN boot
# Wed, 12 Apr 2023 01:24:03 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 12 Apr 2023 01:24:03 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 12 Apr 2023 01:24:04 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9701f65253cb8cdaa00fd933b855a5c7977f66e7e7b1e8cfa93ad00f587f6479`  
		Last Modified: Wed, 12 Apr 2023 01:31:17 GMT  
		Size: 191.3 MB (191260431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22f17e5777fac175e35d05a8536d5a660cc1ac0dad544ce3148a11ebaac7b84e`  
		Last Modified: Wed, 12 Apr 2023 01:31:06 GMT  
		Size: 1.1 MB (1064793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162a183689e03547f641d60c6f589ce955b1b9f36a1303b3da4761a72ca9f0ac`  
		Last Modified: Wed, 12 Apr 2023 01:31:09 GMT  
		Size: 58.8 MB (58820433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b7ba02645ec05b445e21abefd3ad16c69132cab273ccca9c7880fe57b0d201`  
		Last Modified: Wed, 12 Apr 2023 01:31:05 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
