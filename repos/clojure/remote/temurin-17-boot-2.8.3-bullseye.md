## `clojure:temurin-17-boot-2.8.3-bullseye`

```console
$ docker pull clojure@sha256:1536ece49bbe8c849f82e14329cb7e71e8924f3536b8944506a142bdc51098c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-2.8.3-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:08d46fd54c8fb485acee2d1ffd959455881c24da681c6e85fac43e38b0c6bf76
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.7 MB (308655531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:976c20891c0409dd5311433522741ad38d0913447a8c9e821348c71913789f2b`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:41 GMT
ADD file:553d20b03d45305e58cde07e0c259421bba044155ac90b4559e5cc0b69093347 in / 
# Tue, 06 Dec 2022 01:20:41 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:48:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 06 Dec 2022 01:54:43 GMT
COPY dir:fa15c3254735d08fe4cb4c940d6fc08efc9755ff0499a6eb8e51c961cea48d5c in /opt/java/openjdk 
# Tue, 06 Dec 2022 01:54:45 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 01:54:45 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 06 Dec 2022 01:54:45 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 06 Dec 2022 01:54:45 GMT
WORKDIR /tmp
# Tue, 06 Dec 2022 01:54:51 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 06 Dec 2022 01:54:51 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 06 Dec 2022 01:54:51 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 06 Dec 2022 01:55:10 GMT
RUN boot
# Tue, 06 Dec 2022 01:55:10 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Tue, 06 Dec 2022 01:55:10 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 06 Dec 2022 01:55:10 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:f2f58072e9ed1aa1b0143341c5ee83815c00ce47548309fa240155067ab0e698`  
		Last Modified: Tue, 06 Dec 2022 01:24:48 GMT  
		Size: 55.0 MB (55041342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c44c11d030ccad72929755f22eeb76adeb4e273253c295bb22aa0cd941361f3`  
		Last Modified: Tue, 06 Dec 2022 02:06:58 GMT  
		Size: 192.4 MB (192431239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd9d7d1bced7b293214c349bbb1971d08549a0eb653466dab9b4434567179235`  
		Last Modified: Tue, 06 Dec 2022 02:06:44 GMT  
		Size: 2.4 MB (2361961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3398294e7e9e4f3a24fa784024530cf0e5ea35229eebb093d85bf2d61be22f7`  
		Last Modified: Tue, 06 Dec 2022 02:06:48 GMT  
		Size: 58.8 MB (58820590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05982ee7f945a411ff307c36caadfcfe9957b5ca68e30ef26afbd28e1fa4997a`  
		Last Modified: Tue, 06 Dec 2022 02:06:43 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-2.8.3-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:c9108e6c146ebd9272a3844528d3bd4437a7f1798c3190c6ef2cab9ce3aa18aa
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.1 MB (306087595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7bcbb14d9eb51124e36e201a13413a18c7f457a5a1a8c14738f93e2f4eec07f`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:06 GMT
ADD file:b1e7652678bbfc9556636e77d79c947ff1436888e2929f9c5c3ddb42a50c1176 in / 
# Tue, 06 Dec 2022 01:40:07 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:15 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 06 Dec 2022 02:22:20 GMT
COPY dir:36850aee002fdc5445f17d75b8266c48f8e705973ece815c3b53d28b6656ac3e in /opt/java/openjdk 
# Tue, 06 Dec 2022 02:22:24 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 02:22:24 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 06 Dec 2022 02:22:24 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 06 Dec 2022 02:22:25 GMT
WORKDIR /tmp
# Tue, 06 Dec 2022 02:22:29 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 06 Dec 2022 02:22:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 06 Dec 2022 02:22:30 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 06 Dec 2022 02:22:47 GMT
RUN boot
# Tue, 06 Dec 2022 02:22:47 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Tue, 06 Dec 2022 02:22:47 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 06 Dec 2022 02:22:47 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:4948a51a9a3f176f30ac619014f4a2da453a943244eacb53096ee9742eb7cef1`  
		Last Modified: Tue, 06 Dec 2022 01:43:33 GMT  
		Size: 53.7 MB (53699146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e740ce804b4f2a8b5a6fbc891e6b48bdae55634c8831862b9b2bcc60b87ad1`  
		Last Modified: Tue, 06 Dec 2022 02:33:14 GMT  
		Size: 191.2 MB (191215247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:163814feecb9d64f67e3f68577f32d594f9d78050a171d2f03fbae4e9a571caf`  
		Last Modified: Tue, 06 Dec 2022 02:33:03 GMT  
		Size: 2.4 MB (2352273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0786d7e658874901f67f6f7c92ee4677460135e640b607f7c43ef8b0629e24d`  
		Last Modified: Tue, 06 Dec 2022 02:33:05 GMT  
		Size: 58.8 MB (58820529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7686e6aac68ddc951898c68452bc2f8fb16423483365af1fdcfdf5c7945fdcd`  
		Last Modified: Tue, 06 Dec 2022 02:33:02 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
