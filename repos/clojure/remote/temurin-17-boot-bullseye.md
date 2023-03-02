## `clojure:temurin-17-boot-bullseye`

```console
$ docker pull clojure@sha256:5bcfe2d52ffbc13289f4499d64654e8b27062d0c6f466ba1a1814efd5ee9e470
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:70361407735b3ffe9fb3a35ca4ddf8998d937c0849a75412de624a58ff824016
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.7 MB (308666852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:487a25b9a2fe53217bc0e9b5a3a03b9631c58fb4e413128fb78f97469d136a8c`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:45 GMT
ADD file:513c5d5e501279c21a05c1d8b66e5f0b02ee4b27f0b928706d92fd9ce11c1be6 in / 
# Wed, 01 Mar 2023 04:09:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 07:40:41 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 02 Mar 2023 09:00:30 GMT
COPY dir:186a37b080989e6e1268f71ac4b081d0a966a2c5c8b71fa2a808fe83b4537ae1 in /opt/java/openjdk 
# Thu, 02 Mar 2023 09:00:31 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 09:00:31 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 02 Mar 2023 09:00:32 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 02 Mar 2023 09:00:32 GMT
WORKDIR /tmp
# Thu, 02 Mar 2023 09:00:38 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 02 Mar 2023 09:00:38 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 02 Mar 2023 09:00:38 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 02 Mar 2023 09:00:56 GMT
RUN boot
# Thu, 02 Mar 2023 09:00:56 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Thu, 02 Mar 2023 09:00:56 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 02 Mar 2023 09:00:56 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:32fb02163b6bb519a30f909008e852354dae10bdfd6b34190dbdfe8f15403ea0`  
		Last Modified: Wed, 01 Mar 2023 04:13:58 GMT  
		Size: 55.0 MB (55045922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af3cfa1077c96a1e1e95d33920a57958b6fee43d21daec1543eb1ab68b0b9f6`  
		Last Modified: Thu, 02 Mar 2023 09:15:46 GMT  
		Size: 192.4 MB (192438234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32a218378633a09da426ae7f4157a4afe0d312ff37b9279bd66b9828913d04e2`  
		Last Modified: Thu, 02 Mar 2023 09:15:32 GMT  
		Size: 2.4 MB (2361736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4da0e70cf547dbfd71d46da91b4bc6137e189586f698b0fa702915e5fb7e1cd`  
		Last Modified: Thu, 02 Mar 2023 09:15:35 GMT  
		Size: 58.8 MB (58820560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de29b886064e5f059d983328d3c711f4bac59356752e7827f72e5aaf700144bb`  
		Last Modified: Thu, 02 Mar 2023 09:15:32 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:f652aa3666a3e2b7bbdae1b33aa2f8352688c21e05122c7566017cb0855658c3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.1 MB (306135724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eec642b0729a773838f30027ff7e81a9225f70d6749ee8adb29029a70a64b5a0`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:30 GMT
ADD file:a6a1df499d0d5b07fb366d776a11c42ddee6261e2425a921041b38e868192770 in / 
# Wed, 01 Mar 2023 02:20:30 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:01:14 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 02 Mar 2023 07:06:32 GMT
COPY dir:47c117bbc947c5c1164b5a20eeec0ba16c306f5991a85f22c54db31ca24ce4a8 in /opt/java/openjdk 
# Thu, 02 Mar 2023 07:06:36 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 07:06:36 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 02 Mar 2023 07:06:36 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 02 Mar 2023 07:06:36 GMT
WORKDIR /tmp
# Thu, 02 Mar 2023 07:06:41 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 02 Mar 2023 07:06:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 02 Mar 2023 07:06:41 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 02 Mar 2023 07:06:58 GMT
RUN boot
# Thu, 02 Mar 2023 07:06:59 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Thu, 02 Mar 2023 07:06:59 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 02 Mar 2023 07:06:59 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:0f5fe16b1836feccd4765ac5685fc7a7b9c73445cac94fc595d2ffbc3cb59a7a`  
		Last Modified: Wed, 01 Mar 2023 02:23:53 GMT  
		Size: 53.7 MB (53703215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d4bb35cb769be425f0d1c938b7ff57112e361f17e432495be72cb2032f4d92`  
		Last Modified: Thu, 02 Mar 2023 07:20:00 GMT  
		Size: 191.3 MB (191260440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ad538cbfa3ca3cda6ff54422768d6c0750cee9d8560f044d5c5c77086d17fc`  
		Last Modified: Thu, 02 Mar 2023 07:19:50 GMT  
		Size: 2.4 MB (2351070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c18970ebe7e7190e5dade8940e35f7f5d390215908fdf1c3ac20b7000ce4121`  
		Last Modified: Thu, 02 Mar 2023 07:19:53 GMT  
		Size: 58.8 MB (58820598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881a1fd110a14425007f14e3311c9f0a25390623f9e0278c8a31ab48ca8d65d2`  
		Last Modified: Thu, 02 Mar 2023 07:19:49 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
