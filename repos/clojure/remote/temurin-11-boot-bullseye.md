## `clojure:temurin-11-boot-bullseye`

```console
$ docker pull clojure@sha256:3573801ded81dc1f44a5ffb6be41007ea193f8005d2b57e7a8dec2f33f2b5eea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:70cf2741fc116acff506cd79650a95287e906b763f8eedc1e5bfa64e368fab34
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.5 MB (261513653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de7fba3f89a7a879fae76ff157a4157abde978c0f61b1a03d4842bfbd1ba431d`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:46 GMT
ADD file:71543995e4d314b0c86da5ddf8e0cb74649767d30b3e5b6261360de354f0567b in / 
# Tue, 21 Nov 2023 05:21:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:09:28 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 21 Nov 2023 10:14:43 GMT
COPY dir:a96babc4beed1ce86268c08da8bb1232eedf77a64576d0e7cc109ca29beb78ef in /opt/java/openjdk 
# Tue, 21 Nov 2023 10:14:44 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Nov 2023 10:14:44 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 21 Nov 2023 10:14:44 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 21 Nov 2023 10:14:44 GMT
WORKDIR /tmp
# Tue, 21 Nov 2023 10:14:49 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 21 Nov 2023 10:14:50 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 21 Nov 2023 10:14:50 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 21 Nov 2023 10:15:06 GMT
RUN boot
# Tue, 21 Nov 2023 10:15:06 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:d1da99c2f14827498c4a9bb3623ae909b44564bdabad1802f064169069df81fb`  
		Last Modified: Tue, 21 Nov 2023 05:26:17 GMT  
		Size: 55.1 MB (55057903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffe902143c3fd99b4ac9a0291a2832730d347def235a791db08e9e5f1c82f26a`  
		Last Modified: Tue, 21 Nov 2023 10:32:35 GMT  
		Size: 145.3 MB (145266698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef5d38aa19bed21dac754717ba7e6b148a33262d5cc337d76520834921cbfb5`  
		Last Modified: Tue, 21 Nov 2023 10:32:24 GMT  
		Size: 2.4 MB (2368671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9dfe129b5aac900a6feb2318905f774d2dc4c2a3681d08a5123f2b59534b38`  
		Last Modified: Tue, 21 Nov 2023 10:32:27 GMT  
		Size: 58.8 MB (58820381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:6551823c01e59ec11503948b22e69156619580585ef7a660783af1c0fbf10b1f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.9 MB (256887546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e784e18de9153b6c84170342bff836284a84ac85ecba5a058fdcd4e34027e00`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:13 GMT
ADD file:614987b9855939825ad2383e7bacbf14ea208d74906982bba3a67126702c8371 in / 
# Tue, 21 Nov 2023 06:27:13 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:22:29 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 08:45:30 GMT
COPY dir:201fdbb3aef6b177b9038d3dd5bbe865568281c78c7bc0c153b57943d571a0b6 in /opt/java/openjdk 
# Sat, 02 Dec 2023 08:45:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 08:45:33 GMT
ENV BOOT_VERSION=2.8.3
# Sat, 02 Dec 2023 08:45:33 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sat, 02 Dec 2023 08:45:33 GMT
WORKDIR /tmp
# Sat, 02 Dec 2023 08:45:39 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Sat, 02 Dec 2023 08:45:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sat, 02 Dec 2023 08:45:39 GMT
ENV BOOT_AS_ROOT=yes
# Sat, 02 Dec 2023 08:45:55 GMT
RUN boot
# Sat, 02 Dec 2023 08:45:55 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:bbf382c14c7b19b81c612f639e09e6a7b04eccd4481d0abac48b8ace9faae3b3`  
		Last Modified: Tue, 21 Nov 2023 06:30:47 GMT  
		Size: 53.7 MB (53707872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c831d867f0110557a683e007e761887afd75ea0947b774de2aedd6660dc51bc`  
		Last Modified: Sat, 02 Dec 2023 09:04:13 GMT  
		Size: 142.0 MB (142001789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d12b7149ec2be0f0a5580cae28762cbe7e53be9e57f0e70a4cc16a6284995db6`  
		Last Modified: Sat, 02 Dec 2023 09:04:04 GMT  
		Size: 2.4 MB (2357436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0adf65169126afd45b67a476ac08e81c96cca8dd40d62f9db4669ad0607d4f`  
		Last Modified: Sat, 02 Dec 2023 09:04:06 GMT  
		Size: 58.8 MB (58820449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
