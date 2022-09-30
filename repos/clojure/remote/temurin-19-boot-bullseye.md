## `clojure:temurin-19-boot-bullseye`

```console
$ docker pull clojure@sha256:238070d38945b78f6190844f63b151a50c6bd6f0f41f52254de5d6a9b81d7521
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:e5a04e95e9d82eef7e8839d73758e611c550f7cb0ce836a65b0c7fd159a120fb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.1 MB (317055187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab0e51adb95b7ff6c9aca7e864100ed6b3c934283f1698d3e9bfffb57b853f6b`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:18 GMT
ADD file:ff01c6dedb67cf22e9b0735e099b9b6367770c4880941862cc7ec0e979b4118b in / 
# Tue, 13 Sep 2022 00:56:19 GMT
CMD ["bash"]
# Fri, 30 Sep 2022 22:20:04 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 30 Sep 2022 22:30:15 GMT
COPY dir:49a4548ab030e4d26793e92b4d74537cf530961ce7b4083b8d383585c96415d5 in /opt/java/openjdk 
# Fri, 30 Sep 2022 22:30:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 30 Sep 2022 22:30:17 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 30 Sep 2022 22:30:17 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 30 Sep 2022 22:30:17 GMT
WORKDIR /tmp
# Fri, 30 Sep 2022 22:30:23 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 30 Sep 2022 22:30:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 30 Sep 2022 22:30:23 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 30 Sep 2022 22:30:43 GMT
RUN boot
# Fri, 30 Sep 2022 22:30:44 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Fri, 30 Sep 2022 22:30:44 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 30 Sep 2022 22:30:44 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:23858da423a6737f0467fab0014e5b53009ea7405d575636af0c3f100bbb2f10`  
		Last Modified: Tue, 13 Sep 2022 01:00:00 GMT  
		Size: 55.0 MB (55029732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34779663f244298cb178ba4e1c1d99578f0e3dc092f48fbd4a5d87c8ef9c2694`  
		Last Modified: Fri, 30 Sep 2022 22:41:33 GMT  
		Size: 200.8 MB (200843780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3bd89337fc908378d78d286fc3765267513dd4a8744e2e95c15ada44a9744dc`  
		Last Modified: Fri, 30 Sep 2022 22:41:18 GMT  
		Size: 2.4 MB (2360803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305763cf1d8620026585ce8d9879fd28ca5d259d2e180d56f363c907d5c5e9d5`  
		Last Modified: Fri, 30 Sep 2022 22:41:21 GMT  
		Size: 58.8 MB (58820469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2637219218ce95899fea5849c4143347dd20fc475e7a130a356118efc8bc1264`  
		Last Modified: Fri, 30 Sep 2022 22:41:18 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:b8d1ed0a5e85e64157f74143a1b15eaab22d8d19efcbe381457f6332bc7a7853
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.4 MB (314439736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bcfe92da2243da2b4489cc865d54fba9dc64591570438fec13cb3746c3d9f8c`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Tue, 13 Sep 2022 02:10:41 GMT
ADD file:879fb0cd23107ac6f53581456074c7ff13c051aa262de3ca16ffa8475cf04dec in / 
# Tue, 13 Sep 2022 02:10:42 GMT
CMD ["bash"]
# Fri, 30 Sep 2022 22:40:22 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 30 Sep 2022 22:51:51 GMT
COPY dir:58f6c37df253d3555e493197f96e3f21593e31d3faf1967e0a7b9d8f0ae9e30c in /opt/java/openjdk 
# Fri, 30 Sep 2022 22:51:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 30 Sep 2022 22:51:52 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 30 Sep 2022 22:51:53 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 30 Sep 2022 22:51:54 GMT
WORKDIR /tmp
# Fri, 30 Sep 2022 22:52:01 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 30 Sep 2022 22:52:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 30 Sep 2022 22:52:02 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 30 Sep 2022 22:52:15 GMT
RUN boot
# Fri, 30 Sep 2022 22:52:16 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Fri, 30 Sep 2022 22:52:16 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 30 Sep 2022 22:52:17 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:10cff8997b4d4f243419e6bede830f1ac33f3d18c5200e5fb80e19333883ec2b`  
		Last Modified: Tue, 13 Sep 2022 02:15:49 GMT  
		Size: 53.7 MB (53691380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4220f2b93d7437cc764fc660fd07338744f7d8b8738c706ed5dda7f1a24b57f0`  
		Last Modified: Fri, 30 Sep 2022 23:07:04 GMT  
		Size: 199.6 MB (199582885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dae0800eb7d3f2cf2b2ee5463818b2a5a6adb4eafd7a7a7e66699aecfd5385c`  
		Last Modified: Fri, 30 Sep 2022 23:06:47 GMT  
		Size: 2.3 MB (2349205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:297e57d15e470339e13559a9a12163c210719d09132cb8298ceec57e81baceda`  
		Last Modified: Fri, 30 Sep 2022 23:06:51 GMT  
		Size: 58.8 MB (58815867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541419dce2166f01985e0058bc93fa44d883d31c446a27957351583ea6db0c2d`  
		Last Modified: Fri, 30 Sep 2022 23:06:46 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
