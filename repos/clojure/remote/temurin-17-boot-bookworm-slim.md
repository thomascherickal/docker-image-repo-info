## `clojure:temurin-17-boot-bookworm-slim`

```console
$ docker pull clojure@sha256:3227f200de6e7760cf3d0f9f7d47d6447ca57ac71fe67c89bfe4a5eb9c3ad8e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-bookworm-slim` - linux; amd64

```console
$ docker pull clojure@sha256:650ca63779181d4323bd91fd311e844561fc79456fef5198fb923150f1ec18a4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.3 MB (236346205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8fefbeae249ca1329755fa081a5b2cd48ff0553f67ea4f0672af95e23e87093`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:37 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 21 Nov 2023 05:21:37 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:08:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 21 Nov 2023 10:19:20 GMT
COPY dir:33a61da93c3e1252ff87d5fd5f9955ca53f9f7f200758827548096d130b4307b in /opt/java/openjdk 
# Tue, 21 Nov 2023 10:19:22 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Nov 2023 10:19:22 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 21 Nov 2023 10:19:22 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 21 Nov 2023 10:19:22 GMT
WORKDIR /tmp
# Tue, 21 Nov 2023 10:19:27 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 21 Nov 2023 10:19:27 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 21 Nov 2023 10:19:28 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 21 Nov 2023 10:19:44 GMT
RUN boot
# Tue, 21 Nov 2023 10:19:44 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Tue, 21 Nov 2023 10:19:44 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 21 Nov 2023 10:19:44 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f56b9fcad4feae0d6287b1e515254cbce2d5a24afda8aedd7baae660134d3cb`  
		Last Modified: Tue, 21 Nov 2023 10:35:35 GMT  
		Size: 144.9 MB (144873903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e9df3c664c2554059fc449468ec6672d35404e706d1fce76d9238c999dc3cc`  
		Last Modified: Tue, 21 Nov 2023 10:35:24 GMT  
		Size: 3.5 MB (3501683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242b91b963d74a9e3efeedf15069ed98cdb195df2619a0b485b6a6a0c4887fce`  
		Last Modified: Tue, 21 Nov 2023 10:35:27 GMT  
		Size: 58.8 MB (58820313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f33ed9aefb4d4613d54d19db3340f7bfbda036a09d5009a80d09b46b3f92c604`  
		Last Modified: Tue, 21 Nov 2023 10:35:23 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-bookworm-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:d7a719a6ff16014c1c1cee436e04e5becc7add3f8d186375ee8b09a37280e08e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.0 MB (235006809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a78fb225db6818448704571b2a7e0f45ea351a84384d20fa1d008e5b81254389`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:22:01 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 08:53:31 GMT
COPY dir:b97789a1c2e6d715436236e063679209ed5b51287e172faadc90d7cbd7bc1135 in /opt/java/openjdk 
# Sat, 02 Dec 2023 08:53:35 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 08:53:35 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 02 Dec 2023 08:53:35 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 02 Dec 2023 08:53:35 GMT
WORKDIR /tmp
# Sat, 02 Dec 2023 08:53:40 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Sat, 02 Dec 2023 08:53:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 02 Dec 2023 08:53:40 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 02 Dec 2023 08:53:56 GMT
RUN boot
# Sat, 02 Dec 2023 08:53:57 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Sat, 02 Dec 2023 08:53:57 GMT
ENTRYPOINT ["entrypoint"]
# Sat, 02 Dec 2023 08:53:57 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5174505a545417ed296a7213ad24367c7222fd420ece7b5f7b0bd62c3811e57`  
		Last Modified: Sat, 02 Dec 2023 09:08:12 GMT  
		Size: 143.7 MB (143681757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e37bf8024f8af2ad7371f20dc897038ea349c3e3ae82e03109bf62c01ee1f9a`  
		Last Modified: Sat, 02 Dec 2023 09:08:03 GMT  
		Size: 3.3 MB (3324877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fb6c60c5411387f48e0828bc66c65a041d406527832079e5bfb1c007c53208`  
		Last Modified: Sat, 02 Dec 2023 09:08:05 GMT  
		Size: 58.8 MB (58820498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d85c2c212c6bcc4b56978cb9aa977ba9a3a968182b06214fe391d6139832060`  
		Last Modified: Sat, 02 Dec 2023 09:08:02 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
