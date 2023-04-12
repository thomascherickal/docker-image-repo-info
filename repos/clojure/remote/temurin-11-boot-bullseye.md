## `clojure:temurin-11-boot-bullseye`

```console
$ docker pull clojure@sha256:bdf3d345c804ffc197f1fb74b6290290db3f1c8379686aa513dec26e70b76cfb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:b0f1dbc48b3cfae5583d835bc5d13c03ffc3fe2200f2046429f3f5571a58b170
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.7 MB (314710790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:324da95e8c9085807c173930af234c29758c30b6b7e98fbeb14d83ae2e04f491`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:10:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 08:13:28 GMT
COPY dir:e649a995635d4b28f1458e8ccc09f5f71440b52479cfda5ea11e99ab14d0ce82 in /opt/java/openjdk 
# Wed, 12 Apr 2023 08:13:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 08:13:29 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 12 Apr 2023 08:13:30 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 12 Apr 2023 08:13:30 GMT
WORKDIR /tmp
# Wed, 12 Apr 2023 08:13:35 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 12 Apr 2023 08:13:35 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 12 Apr 2023 08:13:35 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 12 Apr 2023 08:13:53 GMT
RUN boot
# Wed, 12 Apr 2023 08:13:53 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc28d33e44b328c3a33e1c0717d82dcbea604364ba89e1ab1b64f3d3a2f165a`  
		Last Modified: Wed, 12 Apr 2023 08:22:57 GMT  
		Size: 198.5 MB (198476040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae3b2143d4ed326f1e0809b39c95df8f4a4995de2b037dc310f1fd03667083c5`  
		Last Modified: Wed, 12 Apr 2023 08:22:43 GMT  
		Size: 2.4 MB (2361690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48d892f59e6472b03f84c2dc4956007e920b2efad383764ed7bfc2c3dab5984`  
		Last Modified: Wed, 12 Apr 2023 08:22:47 GMT  
		Size: 58.8 MB (58820324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:58692a3b56a89dcd88ebc25ebbb69e4afe4129d454cc3f38a982287afe402140
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **310.1 MB (310119637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d61fb9dae5bbde82a98288cc9a64a796e6c661dc7c08dcafa3fa0fc2a9af17c1`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:42 GMT
ADD file:dd3d4e5fe819950e7d01b44a29dbd790438cd722ba76198910e2597448ab0c6f in / 
# Wed, 12 Apr 2023 00:39:43 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 01:20:38 GMT
COPY dir:d446509417048b798354227404c222c2c6031477a91cb1b64eded33f5e598adf in /opt/java/openjdk 
# Wed, 12 Apr 2023 01:20:42 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 01:20:43 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 12 Apr 2023 01:20:43 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 12 Apr 2023 01:20:43 GMT
WORKDIR /tmp
# Wed, 12 Apr 2023 01:20:47 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 12 Apr 2023 01:20:48 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 12 Apr 2023 01:20:48 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 12 Apr 2023 01:21:05 GMT
RUN boot
# Wed, 12 Apr 2023 01:21:05 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:dc80b8cdbfd36cb20231d807a50d704945d1df4da8f6e23197ccfcb629970491`  
		Last Modified: Wed, 12 Apr 2023 00:42:14 GMT  
		Size: 53.7 MB (53705529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e34d229c4186d9e7e7ce0aee26abda131ebcee8bee99be5af11bfc1bf391db`  
		Last Modified: Wed, 12 Apr 2023 01:29:24 GMT  
		Size: 195.2 MB (195242537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ee64c8bc6746b8da9e35d0eaac1f05cc6f88126dfde0cd2200960514ff0f54`  
		Last Modified: Wed, 12 Apr 2023 01:29:13 GMT  
		Size: 2.4 MB (2351079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a0924add50f5bf4fac17b84dbc91d24a420b88f61a6154442afbd591f23ff7`  
		Last Modified: Wed, 12 Apr 2023 01:29:15 GMT  
		Size: 58.8 MB (58820492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
