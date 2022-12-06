## `clojure:temurin-19-boot-bullseye`

```console
$ docker pull clojure@sha256:229f6857ed6242f5a603c88fa748e8bc73764632bc8f9fc303cd0a1e27809cad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:96ed30c7a698b8866f1a2bcdbbc6410a01bb63485a1aad94796165c7d9c0541d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.3 MB (317327678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1bff1ec2078b400384bb7f6124f8da97c3aee4bf9f9fdd15070aaa02f2db3bc`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:41 GMT
ADD file:553d20b03d45305e58cde07e0c259421bba044155ac90b4559e5cc0b69093347 in / 
# Tue, 06 Dec 2022 01:20:41 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:48:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 06 Dec 2022 01:57:42 GMT
COPY dir:fef581854733ec7202f8c807463b9e1952aeb6c7a002719c7e54987e50ea4dcb in /opt/java/openjdk 
# Tue, 06 Dec 2022 01:57:44 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 01:57:44 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 06 Dec 2022 01:57:44 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 06 Dec 2022 01:57:45 GMT
WORKDIR /tmp
# Tue, 06 Dec 2022 01:57:50 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 06 Dec 2022 01:57:51 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 06 Dec 2022 01:57:51 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 06 Dec 2022 01:58:09 GMT
RUN boot
# Tue, 06 Dec 2022 01:58:10 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Tue, 06 Dec 2022 01:58:10 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 06 Dec 2022 01:58:10 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:f2f58072e9ed1aa1b0143341c5ee83815c00ce47548309fa240155067ab0e698`  
		Last Modified: Tue, 06 Dec 2022 01:24:48 GMT  
		Size: 55.0 MB (55041342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5290555b9fd520933dc8e0c6563f92fd2a2cfc886a885094d2288c04a01ae4`  
		Last Modified: Tue, 06 Dec 2022 02:09:00 GMT  
		Size: 201.1 MB (201103430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08be81519dcdfd8889e9981950349894fe25cd9a1b6d7d2c2519d5602fab32e1`  
		Last Modified: Tue, 06 Dec 2022 02:08:45 GMT  
		Size: 2.4 MB (2362007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03a69c6d3fb333cffbfa189fa191907358d8fc940e4fd9df9c2746014ab0b277`  
		Last Modified: Tue, 06 Dec 2022 02:08:48 GMT  
		Size: 58.8 MB (58820500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c8d57dc92696bcedb61a24b994603f41703f6c265b283e65d26b4f80df801c4`  
		Last Modified: Tue, 06 Dec 2022 02:08:44 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:ff362f5ed4e5b5a7257b8e7418db764973292aea66f3390fa445409aeca159d3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.7 MB (314736577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:039a17c34e8056e7ea9af9b2e65f65f9d179b70ced2e992325c2036b88079ac8`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:06 GMT
ADD file:b1e7652678bbfc9556636e77d79c947ff1436888e2929f9c5c3ddb42a50c1176 in / 
# Tue, 06 Dec 2022 01:40:07 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:15 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 06 Dec 2022 02:24:58 GMT
COPY dir:4138443eebfda1a2a245638d5bb568645bd34d79b66d39a3be31b5ac6b823d6d in /opt/java/openjdk 
# Tue, 06 Dec 2022 02:25:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 02:25:03 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 06 Dec 2022 02:25:03 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 06 Dec 2022 02:25:03 GMT
WORKDIR /tmp
# Tue, 06 Dec 2022 02:25:07 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 06 Dec 2022 02:25:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 06 Dec 2022 02:25:08 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 06 Dec 2022 02:25:24 GMT
RUN boot
# Tue, 06 Dec 2022 02:25:24 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Tue, 06 Dec 2022 02:25:24 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 06 Dec 2022 02:25:24 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:4948a51a9a3f176f30ac619014f4a2da453a943244eacb53096ee9742eb7cef1`  
		Last Modified: Tue, 06 Dec 2022 01:43:33 GMT  
		Size: 53.7 MB (53699146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cabaaf976f2d5c56a302b35a76e1a18a5cb39245bb9fc93db9557a6e3e5f0b9`  
		Last Modified: Tue, 06 Dec 2022 02:35:02 GMT  
		Size: 199.9 MB (199864416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60e3496fd36b3ec4bfa4a97baf3cf1b24a6f8afb3cdfabd970c7a93a5e7c3cb`  
		Last Modified: Tue, 06 Dec 2022 02:34:50 GMT  
		Size: 2.4 MB (2352215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c036d654a148e6200f74baa024e72300fd938aaafcbefdcd8f5b76fd4716fa6`  
		Last Modified: Tue, 06 Dec 2022 02:34:52 GMT  
		Size: 58.8 MB (58820399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3a6777f0442a85e6d45b07e2ffd409ca264b50bf706d17be51978f86b51b69`  
		Last Modified: Tue, 06 Dec 2022 02:34:49 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
