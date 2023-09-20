## `clojure:temurin-17-boot-bullseye`

```console
$ docker pull clojure@sha256:fa1e2f7518f5cd98c932f6b0e8e74b32f4ac2b6f96a2bd6491a230a938166d46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:57a8092ec5a8789469047c699b7e509345261c8e5160d05f598cc1d023529e66
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.0 MB (261015430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:417a55b3303ef80fda97ba6f8ac0e0b9edd1e773bac22f8ba2275f4aea5c43ab`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 20 Sep 2023 04:55:51 GMT
ADD file:85db4f4c5016f51f7112a5d09cb7d4620f565a1379ae4b8a03c5ffc23886a876 in / 
# Wed, 20 Sep 2023 04:55:51 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 07:21:46 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 20 Sep 2023 07:27:45 GMT
COPY dir:61bbef45bd137d5078f6a6f774d9bc49d275ae5fe27274294232d075ae1a5bf2 in /opt/java/openjdk 
# Wed, 20 Sep 2023 07:27:47 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Sep 2023 07:27:47 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 20 Sep 2023 07:27:47 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 20 Sep 2023 07:27:47 GMT
WORKDIR /tmp
# Wed, 20 Sep 2023 07:27:53 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 20 Sep 2023 07:27:53 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 20 Sep 2023 07:27:53 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 20 Sep 2023 07:28:10 GMT
RUN boot
# Wed, 20 Sep 2023 07:28:10 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 20 Sep 2023 07:28:11 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 20 Sep 2023 07:28:11 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:ddf874abf16cc990e0fd75a154a34ca0a03ee310ad895a18fb62ae15bf4171fb`  
		Last Modified: Wed, 20 Sep 2023 05:00:41 GMT  
		Size: 55.1 MB (55056714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf4a672ed9955378a963316cbf18411e8a03dfdf04af1c6124a50daf2a46955`  
		Last Modified: Wed, 20 Sep 2023 07:37:17 GMT  
		Size: 144.8 MB (144775739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f8f951f10159e45e345e354fcb2238a13ddc9c44ea8ac2f620f7bbd6adadbc1`  
		Last Modified: Wed, 20 Sep 2023 07:37:05 GMT  
		Size: 2.4 MB (2362095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d7fbe130a41acb26242463b46399a52d39b0f0805b280ca6e0392d9a910a5f`  
		Last Modified: Wed, 20 Sep 2023 07:37:11 GMT  
		Size: 58.8 MB (58820483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba26c4398e028d3d9e75d98163478681361e356df535eb4a24b3408efec78704`  
		Last Modified: Wed, 20 Sep 2023 07:37:05 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:fc34f581a6e7e1ace9d8d38de072bf2f5b4d64b1c32fed6eac5b5001505083e3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.4 MB (258420462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28d6f144409e531127ef08092ad106dbfc1bcccd293e4dcbd7eb9fe377bfe587`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:20 GMT
ADD file:46dcdcde338d2c01fed5db3fac9041736d9305145d8fc2039dd5b3714d38ede8 in / 
# Wed, 20 Sep 2023 02:44:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:47:32 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 20 Sep 2023 09:52:37 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Wed, 20 Sep 2023 09:52:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Sep 2023 09:52:41 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 20 Sep 2023 09:52:41 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 20 Sep 2023 09:52:41 GMT
WORKDIR /tmp
# Wed, 20 Sep 2023 09:52:46 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 20 Sep 2023 09:52:46 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 20 Sep 2023 09:52:46 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 20 Sep 2023 09:53:02 GMT
RUN boot
# Wed, 20 Sep 2023 09:53:02 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 20 Sep 2023 09:53:02 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 20 Sep 2023 09:53:02 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:31f5dc1f52c865588c43d8ec718f14d430e149b28f0b28232da825da7ae28f76`  
		Last Modified: Wed, 20 Sep 2023 02:47:53 GMT  
		Size: 53.7 MB (53704892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4062a5e07d52b88a032ac209012e51040c57c264c0ce7634b347a2550b76e570`  
		Last Modified: Wed, 20 Sep 2023 10:00:59 GMT  
		Size: 143.5 MB (143543478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540bb8dc7a897c949a243e144c7f61aa87f3ee9f0f1f9c709030cddf3f186c46`  
		Last Modified: Wed, 20 Sep 2023 10:00:49 GMT  
		Size: 2.4 MB (2351341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57d05e607a800c3ff49876499505725458f9a29e0b62f8b53de011c92bcb03de`  
		Last Modified: Wed, 20 Sep 2023 10:00:53 GMT  
		Size: 58.8 MB (58820352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568888b00e9fad047ed770a68c40bea366db24b5de6804bc0d208958df507cb6`  
		Last Modified: Wed, 20 Sep 2023 10:00:49 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
