## `clojure:temurin-11-boot-bullseye`

```console
$ docker pull clojure@sha256:0fea89b26939b85132024893738a434f3d09472a821b716f8bef3f7164682a30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:d1f303e2160e707d55c6fd1ba823f119ce09c54b4870e7559ec225f103f8159b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.1 MB (261065358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eecffec0ce5812305f759d2dfebb565a889c702ea81b7f50b4bfabf8bf798748`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 20 Sep 2023 04:55:51 GMT
ADD file:85db4f4c5016f51f7112a5d09cb7d4620f565a1379ae4b8a03c5ffc23886a876 in / 
# Wed, 20 Sep 2023 04:55:51 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 07:21:46 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 20 Sep 2023 07:24:52 GMT
COPY dir:3e9b1d3d54369337872a2b8aa8c30068d69b28c2def3ec3bf07ba34bd69d48a0 in /opt/java/openjdk 
# Wed, 20 Sep 2023 07:24:53 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Sep 2023 07:24:53 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 20 Sep 2023 07:24:54 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 20 Sep 2023 07:24:54 GMT
WORKDIR /tmp
# Wed, 20 Sep 2023 07:24:59 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 20 Sep 2023 07:25:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 20 Sep 2023 07:25:00 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 20 Sep 2023 07:25:20 GMT
RUN boot
# Wed, 20 Sep 2023 07:25:20 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:ddf874abf16cc990e0fd75a154a34ca0a03ee310ad895a18fb62ae15bf4171fb`  
		Last Modified: Wed, 20 Sep 2023 05:00:41 GMT  
		Size: 55.1 MB (55056714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d2593b379fff1802970ddf266f34d6bd5d13fda962a549ac1b0e11020096b1`  
		Last Modified: Wed, 20 Sep 2023 07:35:34 GMT  
		Size: 144.8 MB (144826046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bc3c67b3eba7c868eecee43a21f6efd25eb2b00f4c47ea902a459a050be28e`  
		Last Modified: Wed, 20 Sep 2023 07:35:23 GMT  
		Size: 2.4 MB (2362085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a21e8dadd7bb670003a0e2be43047dfdc2d13ac0cd3d815edd9b289c41a7a7`  
		Last Modified: Wed, 20 Sep 2023 07:35:27 GMT  
		Size: 58.8 MB (58820513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:f0c7d1334122aa539eebbce661f148f0a1864ce74ee01e9283729f5ec8494a13
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.4 MB (256447142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41dde469b9f0823777098feeb503fd0a370bee57e42758063b0a4eea6a09fbb6`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:20 GMT
ADD file:46dcdcde338d2c01fed5db3fac9041736d9305145d8fc2039dd5b3714d38ede8 in / 
# Wed, 20 Sep 2023 02:44:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:47:32 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 20 Sep 2023 09:50:06 GMT
COPY dir:68819d2d348aedadecb99120d7ca4a63dcc1e3aa0bb526ecbd9925396c38234c in /opt/java/openjdk 
# Wed, 20 Sep 2023 09:50:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Sep 2023 09:50:10 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 20 Sep 2023 09:50:10 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 20 Sep 2023 09:50:10 GMT
WORKDIR /tmp
# Wed, 20 Sep 2023 09:50:15 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 20 Sep 2023 09:50:15 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 20 Sep 2023 09:50:15 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 20 Sep 2023 09:50:32 GMT
RUN boot
# Wed, 20 Sep 2023 09:50:32 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:31f5dc1f52c865588c43d8ec718f14d430e149b28f0b28232da825da7ae28f76`  
		Last Modified: Wed, 20 Sep 2023 02:47:53 GMT  
		Size: 53.7 MB (53704892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2e9551e9fa1a88478be15e148497b5eb08d83b0df41acb2137ae71348d461c`  
		Last Modified: Wed, 20 Sep 2023 09:59:21 GMT  
		Size: 141.6 MB (141570486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22bee27e065d6b1f801e11b07a4ff404c72f8beb8f8e3fc1a53dc501a2510dd1`  
		Last Modified: Wed, 20 Sep 2023 09:59:11 GMT  
		Size: 2.4 MB (2351391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523911394d1dc90a71d048e76e85ae86e0f54a29a8240152fe76060dd014c9bf`  
		Last Modified: Wed, 20 Sep 2023 09:59:16 GMT  
		Size: 58.8 MB (58820373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
