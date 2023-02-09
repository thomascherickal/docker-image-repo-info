## `clojure:temurin-8-boot-bullseye`

```console
$ docker pull clojure@sha256:1b36a93eb24b5de679bd587cef8570285197f05459602a6effc2eaf18db9121b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:1809cc0e825d5ddbcbacea8fd5459b8e93d22943624b2a52130875c8dc869bb3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.9 MB (170864618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f14d83c3ae8f7ccd80fdbc9cddfe812b6c43a29b6b9d3bbcb4eae4e8d4972832`
-	Default Command: `["boot","repl"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:05 GMT
ADD file:b03d13d345c29f69557f410c8504e748226756d1f48e5abdb63cd40179b2640c in / 
# Thu, 09 Feb 2023 03:20:05 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:22:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:22:06 GMT
COPY dir:bbb84183d7ea38d81d8401f01e29d08935ee4c8bf6f90c6527579a1554c3bde1 in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:22:06 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 09:22:06 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 09 Feb 2023 09:22:06 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 09 Feb 2023 09:22:07 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:22:13 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 09 Feb 2023 09:22:13 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 09 Feb 2023 09:22:13 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 09 Feb 2023 09:22:30 GMT
RUN boot
# Thu, 09 Feb 2023 09:22:31 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:1e4aec178e0864db93a6f97a20bde3445871a4562c1801185eca1238d3a0e80d`  
		Last Modified: Thu, 09 Feb 2023 03:24:47 GMT  
		Size: 55.0 MB (55046771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002e7af6c4fa5dcefe0cea885d5bc9ca4379383c456abb3a1ebe2728ac33a5e7`  
		Last Modified: Thu, 09 Feb 2023 09:36:44 GMT  
		Size: 54.6 MB (54635546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e11256390ab060b83cddfa7c32127256eefdf8a13fd16f7a07bafca272b498c2`  
		Last Modified: Thu, 09 Feb 2023 09:36:37 GMT  
		Size: 2.4 MB (2361729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c060d4c1ab427beb4e0d931b1f7821090f06e68b1cd40a888f8bcb542a7207`  
		Last Modified: Thu, 09 Feb 2023 09:36:41 GMT  
		Size: 58.8 MB (58820572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:52a65fd9994d35b114850a77b91811d3dc5edcb49f96a6da17ea66e3715c4cf2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.6 MB (168603286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d555bc79d27ce86c0c75494ba9314771f668dd04aa716d54393be212c2f767cc`
-	Default Command: `["boot","repl"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:29 GMT
ADD file:5cf2de182dac36d99ec41918889c9755f9c49c56fa0a8d0ca14040c1d8c04541 in / 
# Thu, 09 Feb 2023 03:58:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:17:51 GMT
COPY dir:b6d7e5613532d986930216de9e0fece0632e82564ce7a6a98baf63b4115f840d in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:17:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 09:17:52 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 09 Feb 2023 09:17:52 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 09 Feb 2023 09:17:52 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:17:58 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 09 Feb 2023 09:17:58 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 09 Feb 2023 09:17:58 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 09 Feb 2023 09:18:46 GMT
RUN boot
# Thu, 09 Feb 2023 09:18:46 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:80dae1b9d879348c210c40024c6e90ef92677ac3515456375fcbb70bdf07b104`  
		Last Modified: Thu, 09 Feb 2023 04:02:11 GMT  
		Size: 53.7 MB (53703368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c77b7001deefab693beef32501685ba34c540df86923e1b9f608310809ebc1ce`  
		Last Modified: Thu, 09 Feb 2023 09:30:48 GMT  
		Size: 53.7 MB (53727942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32bf4cd12b86fc4a1205e9e1fb73e359747d2031557c5d2a24c0eabf28d67ca5`  
		Last Modified: Thu, 09 Feb 2023 09:30:44 GMT  
		Size: 2.4 MB (2350992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d31aa3d6eef0f1d0b8b5fa1e24417e08342c2ede4db1eaf5a45c1d8618a8657`  
		Last Modified: Thu, 09 Feb 2023 09:30:46 GMT  
		Size: 58.8 MB (58820984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
