## `clojure:temurin-17-boot-bullseye-slim`

```console
$ docker pull clojure@sha256:d007a69fe1941b97c86839a690db990f005076e0e78e2a2dc7aa921ce0424666
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:a40831e2f164ae9346a40139caeb5b1ab72622ba3044a26321484a2abae9571d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.7 MB (283747737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:034dd8f30790f3903d953610f891c5cae2c24f1be60ef1a0ba1a99779c23e374`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:17:46 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:23:11 GMT
COPY dir:d90c8d6564183f8aad11f93ecfb2f7e0eeff18588ff2b62d7ca3d8d30672bc2c in /opt/java/openjdk 
# Thu, 23 Mar 2023 06:23:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 06:23:13 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 23 Mar 2023 06:23:13 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 23 Mar 2023 06:23:13 GMT
WORKDIR /tmp
# Thu, 23 Mar 2023 06:23:18 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 23 Mar 2023 06:23:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 23 Mar 2023 06:23:18 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 23 Mar 2023 06:23:37 GMT
RUN boot
# Thu, 23 Mar 2023 06:23:37 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Thu, 23 Mar 2023 06:23:37 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 23 Mar 2023 06:23:37 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f5c96fe943f36d4d8aa8ab4df9c0bd26f8cd6280632e002706fc7d61a975aa`  
		Last Modified: Thu, 23 Mar 2023 06:32:52 GMT  
		Size: 192.4 MB (192438234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:654673d2ed11bf33ade2936bb436ac1c5f0d6b0a6334cfcef869934a26169cc2`  
		Last Modified: Thu, 23 Mar 2023 06:32:39 GMT  
		Size: 1.1 MB (1077355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8064ff32f2d464c339ce44d2c5dfac1f1dc0b0a9efb136e882442fd7f96676d`  
		Last Modified: Thu, 23 Mar 2023 06:32:42 GMT  
		Size: 58.8 MB (58820346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071dc29d7fb03705c007f30ceb02f6ad2a638a72e8d3a329ebb84d2f513d9b2a`  
		Last Modified: Thu, 23 Mar 2023 06:32:38 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:32861290b8edb1b9ed807cec82db5c9670394a6cdb237ed7ad5242081ce8ed59
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.2 MB (281208472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ba27adb607ff178dc80f04bfc13cfbbc0ccf66b61b68c07af28e45c2fd6974c`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:52:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:57:23 GMT
COPY dir:44544f5117ae50af040f98b1979efcc18f4c9f0c7257bfc4a37b80697337361a in /opt/java/openjdk 
# Thu, 23 Mar 2023 06:57:27 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 06:57:27 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 23 Mar 2023 06:57:27 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 23 Mar 2023 06:57:27 GMT
WORKDIR /tmp
# Thu, 23 Mar 2023 06:57:32 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 23 Mar 2023 06:57:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 23 Mar 2023 06:57:32 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 23 Mar 2023 06:57:48 GMT
RUN boot
# Thu, 23 Mar 2023 06:57:48 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Thu, 23 Mar 2023 06:57:48 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 23 Mar 2023 06:57:48 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce46c3fded23542cb5a993d929bb8b2dfc32a31d4c9928588d2da3bc91d84fec`  
		Last Modified: Thu, 23 Mar 2023 07:06:00 GMT  
		Size: 191.3 MB (191260416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25349c3db413815dbaa5cf82aeeabff709ef6972182881dbd5508c3c546c14ee`  
		Last Modified: Thu, 23 Mar 2023 07:05:50 GMT  
		Size: 1.1 MB (1064632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35ca6c0d718963c678ab43b03e3018cc25620628d50292f4fbf9ea3b81f8874`  
		Last Modified: Thu, 23 Mar 2023 07:05:52 GMT  
		Size: 58.8 MB (58820326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cab638daabd95b873585a48711fab8225b400ec2ff512f0f0f1115d4d9fd8f9`  
		Last Modified: Thu, 23 Mar 2023 07:05:49 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
