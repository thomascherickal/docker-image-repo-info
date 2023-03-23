## `clojure:temurin-19-boot-2.8.3-bullseye-slim`

```console
$ docker pull clojure@sha256:9191ab25c7c13b7661380434a30ce9191899b946455c84d9abbb1967e250f088
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-boot-2.8.3-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:7345c5f31f67017aa55b633b8a5273b22fb51955851b77962a5577dc8cc5ad57
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.4 MB (292422733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b4f72c9fd155941f144083a67d6031ed5a2d702bf8202a1d852f5eeaaef2750`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:17:46 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:25:51 GMT
COPY dir:94cb5af8175285c10c94286222d8a35302f3f8c290e00011a75c67156659d6ab in /opt/java/openjdk 
# Thu, 23 Mar 2023 06:25:53 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 06:25:53 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 23 Mar 2023 06:25:53 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 23 Mar 2023 06:25:53 GMT
WORKDIR /tmp
# Thu, 23 Mar 2023 06:25:59 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 23 Mar 2023 06:25:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 23 Mar 2023 06:25:59 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 23 Mar 2023 06:26:17 GMT
RUN boot
# Thu, 23 Mar 2023 06:26:17 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Thu, 23 Mar 2023 06:26:17 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 23 Mar 2023 06:26:17 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d50160c605f9c02acd78ef392f7194eee61162e99ab69aa71a85d2c04e97ff86`  
		Last Modified: Thu, 23 Mar 2023 06:34:39 GMT  
		Size: 201.1 MB (201112949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6e2cf555b6166533c8045030491a3db9263abce06badaf56d5f11b6d716ac5`  
		Last Modified: Thu, 23 Mar 2023 06:34:25 GMT  
		Size: 1.1 MB (1077376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6551611d2227fa1341ec3fc51b17d5731340dba5c2e61147ba369437b886a905`  
		Last Modified: Thu, 23 Mar 2023 06:34:28 GMT  
		Size: 58.8 MB (58820604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ca31cec064e2beb83b7d1f53cb83f4c0ac6b0d4bbd823f5b19962274b2680d5`  
		Last Modified: Thu, 23 Mar 2023 06:34:24 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-boot-2.8.3-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:a0efc88d2cba5472ffa9e5d4329aa7f22832eb67a262604d69ae4e5a0e206af0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.8 MB (289803428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae65c6c3fd1de467ac53849a4dcfa9f748bbfd068983fac411bbe83417cef6e9`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:52:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:59:40 GMT
COPY dir:9a6a873ca11063f6f04e7f088397a1fce771e2b1aa8590b72eb07158cfac883f in /opt/java/openjdk 
# Thu, 23 Mar 2023 06:59:44 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 06:59:45 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 23 Mar 2023 06:59:45 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 23 Mar 2023 06:59:45 GMT
WORKDIR /tmp
# Thu, 23 Mar 2023 06:59:49 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 23 Mar 2023 06:59:49 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 23 Mar 2023 06:59:49 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 23 Mar 2023 07:00:06 GMT
RUN boot
# Thu, 23 Mar 2023 07:00:06 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Thu, 23 Mar 2023 07:00:06 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 23 Mar 2023 07:00:06 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274b1a27e7816b7f1e1f1324be385765b25723b5eddb3f339875cd4a1fa13c6e`  
		Last Modified: Thu, 23 Mar 2023 07:07:40 GMT  
		Size: 199.9 MB (199855165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e460a2cd70fd668ce0697a3549a7a0adad53d902fd232bd5cb5e0ff5701b2b5`  
		Last Modified: Thu, 23 Mar 2023 07:07:29 GMT  
		Size: 1.1 MB (1064646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d776d66f4c79aa7f60346d2f1991f7a311abf027e2aa9cfda346d2e698b01041`  
		Last Modified: Thu, 23 Mar 2023 07:07:32 GMT  
		Size: 58.8 MB (58820519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc70418f15530fe0828a6f09e2aadaaab35780bb515e9efcc120d2937f94e01`  
		Last Modified: Thu, 23 Mar 2023 07:07:28 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
