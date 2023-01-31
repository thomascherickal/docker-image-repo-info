## `clojure:temurin-17-boot-2.8.3-bullseye`

```console
$ docker pull clojure@sha256:3e3924ea09733c82749006717cb024a66cd4602673b2fd26e1f2c6ea8b6185ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-2.8.3-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:8a4584fee4810f1efb8a44706b2642f859f6032d9a0e50f133edec2c46616faf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.6 MB (308644898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e48e65a5ee78c4b2be6ab34915b35238709c42c3f1c568517e751307a8cfd17`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:29 GMT
ADD file:917750a82b29f8f7f88a121017bd9dfeb0fbcc8f0697a009f08b6b58246eff4b in / 
# Wed, 11 Jan 2023 02:34:30 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:18:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 25 Jan 2023 00:45:22 GMT
COPY dir:bb223240e99e5b7e66eb621e33f54e49ced87035f56dd975e567c739be4bfe96 in /opt/java/openjdk 
# Wed, 25 Jan 2023 00:45:24 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 25 Jan 2023 00:45:24 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 25 Jan 2023 00:45:24 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 25 Jan 2023 00:45:24 GMT
WORKDIR /tmp
# Wed, 25 Jan 2023 00:45:30 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 25 Jan 2023 00:45:31 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 25 Jan 2023 00:45:31 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 25 Jan 2023 00:45:48 GMT
RUN boot
# Wed, 25 Jan 2023 00:45:48 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 25 Jan 2023 00:45:48 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 25 Jan 2023 00:45:48 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:bbeef03cda1f5d6c9e20c310c1c91382a6b0a1a2501c3436b28152f13896f082`  
		Last Modified: Wed, 11 Jan 2023 02:38:42 GMT  
		Size: 55.0 MB (55025206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147288dc8989fb24ee233733fb7ef84c2cf5d7be2f0863fe9ea1e153e52a350f`  
		Last Modified: Wed, 25 Jan 2023 00:57:58 GMT  
		Size: 192.4 MB (192438164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:117d7a4824bc4d2c9db632d2aed76365b9ff1dff689a3b742f6698a4dfa4f7e5`  
		Last Modified: Wed, 25 Jan 2023 00:57:43 GMT  
		Size: 2.4 MB (2360635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93bb362a493d7f7ad065de9e46d29e66ef91b974cbb23e33531a99e71862c91`  
		Last Modified: Wed, 25 Jan 2023 00:57:47 GMT  
		Size: 58.8 MB (58820494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003c9ac5587341842c4bdec8eb3f2766052d23da6da598e74968e82a4ce46f03`  
		Last Modified: Wed, 25 Jan 2023 00:57:43 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-2.8.3-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:9fe8402695fe9e3a6c1bbadad704c80c479500e60f56e9a62c8320ba077cca86
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.1 MB (306113640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d945e430ffa6932c677f8a5ef3b0b8dc77434e23795a6828f9781317e89fd23c`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:24 GMT
ADD file:9e185c2d9ca8a231a39ee2b1761fcdff75065252d25a65a207acb7a319c1cf23 in / 
# Wed, 11 Jan 2023 02:57:25 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:14 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Jan 2023 20:54:01 GMT
COPY dir:a1bd99c3d82513db94430c73467e1e5c69ea4624d0489571d594afe503e15dc5 in /opt/java/openjdk 
# Tue, 31 Jan 2023 20:54:05 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 20:54:05 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 31 Jan 2023 20:54:05 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 31 Jan 2023 20:54:05 GMT
WORKDIR /tmp
# Tue, 31 Jan 2023 20:54:10 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 31 Jan 2023 20:54:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 31 Jan 2023 20:54:10 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 31 Jan 2023 20:54:26 GMT
RUN boot
# Tue, 31 Jan 2023 20:54:26 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Tue, 31 Jan 2023 20:54:26 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 31 Jan 2023 20:54:26 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:c345c9e441f5f49235768af74b8ab37743652d38958afaa000edd56d7b2f0540`  
		Last Modified: Wed, 11 Jan 2023 03:00:56 GMT  
		Size: 53.7 MB (53681859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f61d91708311a5923680a9fa5ce56fc7a173443a91b20c1941a3baab459e19`  
		Last Modified: Tue, 31 Jan 2023 21:07:15 GMT  
		Size: 191.3 MB (191260441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eefd809c14a6ec784cfb1ee90836e5f999f4cf2ae94ce5167b9f58432bebca37`  
		Last Modified: Tue, 31 Jan 2023 21:07:04 GMT  
		Size: 2.4 MB (2350670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01abbdc1d447d9c300ffadc75ca1e4a1c84125856f249fe8547dca652c5aef7a`  
		Last Modified: Tue, 31 Jan 2023 21:07:07 GMT  
		Size: 58.8 MB (58820268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:043a984918a0cb8bdfe9072aefa9ff7f1b0ba7fa902d8b5f91904cc8dd46ae4f`  
		Last Modified: Tue, 31 Jan 2023 21:07:04 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
