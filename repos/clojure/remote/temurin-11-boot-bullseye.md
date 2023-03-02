## `clojure:temurin-11-boot-bullseye`

```console
$ docker pull clojure@sha256:5dc1b7ac965c6647b59b28a444a349d440293945535cbdb2737ace6e3ecbc636
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:10d0ccbdc63d256c733021a32c81f82021244e779cb7da72b3a3cfe502c04f85
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.7 MB (314703469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:377c52835be7e4a6dbe3c22f32311aa12b1274cf663c8016e96ca370bee8e542`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:45 GMT
ADD file:513c5d5e501279c21a05c1d8b66e5f0b02ee4b27f0b928706d92fd9ce11c1be6 in / 
# Wed, 01 Mar 2023 04:09:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 07:40:41 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Mar 2023 07:43:44 GMT
COPY dir:fdbc5e9dec2946fa124877176e92a68dd3fe3a70def5bb906a6040c4a1303a2d in /opt/java/openjdk 
# Wed, 01 Mar 2023 07:43:46 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Mar 2023 07:43:46 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 01 Mar 2023 07:43:46 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 01 Mar 2023 07:43:46 GMT
WORKDIR /tmp
# Wed, 01 Mar 2023 07:43:52 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 01 Mar 2023 07:43:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 01 Mar 2023 07:43:52 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 01 Mar 2023 07:44:11 GMT
RUN boot
# Wed, 01 Mar 2023 07:44:11 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:32fb02163b6bb519a30f909008e852354dae10bdfd6b34190dbdfe8f15403ea0`  
		Last Modified: Wed, 01 Mar 2023 04:13:58 GMT  
		Size: 55.0 MB (55045922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c0b29cc6adaf6091151573ab5a4ba12f03dcfaea1402985879aea0d535da14c`  
		Last Modified: Wed, 01 Mar 2023 07:56:45 GMT  
		Size: 198.5 MB (198475588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ae233260f61fbc119660e2b4a3d274be78160fdce5c91ac58cd4250913a827`  
		Last Modified: Wed, 01 Mar 2023 07:56:31 GMT  
		Size: 2.4 MB (2361542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c675b009ac0b3345f8254cfeff9deb48d31b4620d513d1e51c13368a972eea3a`  
		Last Modified: Wed, 01 Mar 2023 07:56:34 GMT  
		Size: 58.8 MB (58820417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:166b372842cd5ee9711895c86f9fc4e63777cf329cbaad2a9aa84c50f3317212
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **310.1 MB (310114885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0dde59ed2da6f83040dfe03531ecc4a1c562346a68855d0cbd6a0f22085dd79`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:30 GMT
ADD file:a6a1df499d0d5b07fb366d776a11c42ddee6261e2425a921041b38e868192770 in / 
# Wed, 01 Mar 2023 02:20:30 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:01:14 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 02 Mar 2023 07:02:06 GMT
COPY dir:10bda54a6f055ef6cbbc2c7efdd1ef99bb798b3ae26972613c5ee4e57e620aeb in /opt/java/openjdk 
# Thu, 02 Mar 2023 07:02:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 07:02:10 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 02 Mar 2023 07:02:10 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 02 Mar 2023 07:02:10 GMT
WORKDIR /tmp
# Thu, 02 Mar 2023 07:02:16 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 02 Mar 2023 07:02:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 02 Mar 2023 07:02:17 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 02 Mar 2023 07:02:33 GMT
RUN boot
# Thu, 02 Mar 2023 07:02:34 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:0f5fe16b1836feccd4765ac5685fc7a7b9c73445cac94fc595d2ffbc3cb59a7a`  
		Last Modified: Wed, 01 Mar 2023 02:23:53 GMT  
		Size: 53.7 MB (53703215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2257672252a1a5ea1cc84b22bcdf9e8c2de57f555374ecbd0173cf802564a507`  
		Last Modified: Thu, 02 Mar 2023 07:16:55 GMT  
		Size: 195.2 MB (195240142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485dc2deffe492893977de5894b18c3656dce5fcf1466388ba335c35aeed21f8`  
		Last Modified: Thu, 02 Mar 2023 07:16:44 GMT  
		Size: 2.4 MB (2351010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c9a1b084a09d143ce7d278cbe16cbb6c15a4d97ef13e18afd2d21f7419bdc5`  
		Last Modified: Thu, 02 Mar 2023 07:16:47 GMT  
		Size: 58.8 MB (58820518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
