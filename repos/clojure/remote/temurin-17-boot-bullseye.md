## `clojure:temurin-17-boot-bullseye`

```console
$ docker pull clojure@sha256:27000063b7ba479399efe8907ec1eeace4bc10843adbdf9be4a512837c370c2e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:b102bf2c844199f99dff692584f44586838d356e379e76f8e03df157d1ff1d4f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.7 MB (308673407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:376a88ac1c7c8fa0181d6f895c295440316a9f92cf35d6a5fc8a47c6440e930c`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:10:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 08:16:11 GMT
COPY dir:d90c8d6564183f8aad11f93ecfb2f7e0eeff18588ff2b62d7ca3d8d30672bc2c in /opt/java/openjdk 
# Wed, 12 Apr 2023 08:16:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 08:16:13 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 12 Apr 2023 08:16:13 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 12 Apr 2023 08:16:13 GMT
WORKDIR /tmp
# Wed, 12 Apr 2023 08:16:18 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 12 Apr 2023 08:16:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 12 Apr 2023 08:16:18 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 12 Apr 2023 08:16:36 GMT
RUN boot
# Wed, 12 Apr 2023 08:16:36 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 12 Apr 2023 08:16:36 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 12 Apr 2023 08:16:37 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc37eb9b838f833285a35e624da1bfed81e650837c6751e8a6812e51ef22b6ba`  
		Last Modified: Wed, 12 Apr 2023 08:24:36 GMT  
		Size: 192.4 MB (192438264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1745cce68db67688329b43342c67dfc640cab9fd8d28cfcbae6fd20dc7f530`  
		Last Modified: Wed, 12 Apr 2023 08:24:23 GMT  
		Size: 2.4 MB (2361634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f882c7768df9e267037d11a35fb0d19965672aa7ed1e8ced77de709a3f8d2fa`  
		Last Modified: Wed, 12 Apr 2023 08:24:27 GMT  
		Size: 58.8 MB (58820375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e899800dc5d40587b419c9afeafcbe2e96b842de2044fe5a0aadb621713a8fd0`  
		Last Modified: Wed, 12 Apr 2023 08:24:23 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:d61d9fa4e3e0a11162c70c85914867a441b40bd1ec6a92e3ffc1cb00e0b4a9ad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.1 MB (306137935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b64944f09128f18d8722edd3e4e46d367c7ed0e3024ebfb584b613c883395ac`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:42 GMT
ADD file:dd3d4e5fe819950e7d01b44a29dbd790438cd722ba76198910e2597448ab0c6f in / 
# Wed, 12 Apr 2023 00:39:43 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 01:23:04 GMT
COPY dir:44544f5117ae50af040f98b1979efcc18f4c9f0c7257bfc4a37b80697337361a in /opt/java/openjdk 
# Wed, 12 Apr 2023 01:23:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 01:23:09 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 12 Apr 2023 01:23:09 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 12 Apr 2023 01:23:09 GMT
WORKDIR /tmp
# Wed, 12 Apr 2023 01:23:14 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 12 Apr 2023 01:23:14 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 12 Apr 2023 01:23:14 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 12 Apr 2023 01:23:31 GMT
RUN boot
# Wed, 12 Apr 2023 01:23:32 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 12 Apr 2023 01:23:32 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 12 Apr 2023 01:23:32 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:dc80b8cdbfd36cb20231d807a50d704945d1df4da8f6e23197ccfcb629970491`  
		Last Modified: Wed, 12 Apr 2023 00:42:14 GMT  
		Size: 53.7 MB (53705529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6911e57ac771aafcbe41270c1285de884dc5ce0d79a1b3069ec89c3a65e4a6c2`  
		Last Modified: Wed, 12 Apr 2023 01:30:58 GMT  
		Size: 191.3 MB (191260417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50295ccbef2d622619d71394f82358bc9fa77444c9a752eeab3cfb6283a724f4`  
		Last Modified: Wed, 12 Apr 2023 01:30:47 GMT  
		Size: 2.4 MB (2351068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e1b4e3499b217c6da14be39e1d22b620ddd35f56661eabaa0cfc1dd777f5c0`  
		Last Modified: Wed, 12 Apr 2023 01:30:50 GMT  
		Size: 58.8 MB (58820521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0424e97b38c6dc6198ec2a0d6311298be19bc24147a9b04869280659081fe24f`  
		Last Modified: Wed, 12 Apr 2023 01:30:47 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
