## `clojure:temurin-17-boot-bullseye`

```console
$ docker pull clojure@sha256:832c6231d885256992d78014430da2c3c6bddba8a9562285b1772e5b399d20fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-boot-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:ac65a5672a18199eff906f6e3d5496b00aa8b78228e3789373b1ef8806efc966
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.7 MB (308667415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfb665e56006367f10a6f6fb927fb17038964b2a5db0be0fb9f1b4963a1367b6`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:05 GMT
ADD file:b03d13d345c29f69557f410c8504e748226756d1f48e5abdb63cd40179b2640c in / 
# Thu, 09 Feb 2023 03:20:05 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:22:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:28:07 GMT
COPY dir:5cf52f938fe415b0022fbccb8cf978562c503c0b8313cc9dedf46c1c4edb35cf in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:28:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 09:28:09 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 09 Feb 2023 09:28:09 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 09 Feb 2023 09:28:10 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:28:15 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 09 Feb 2023 09:28:16 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 09 Feb 2023 09:28:16 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 09 Feb 2023 09:28:32 GMT
RUN boot
# Thu, 09 Feb 2023 09:28:33 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Thu, 09 Feb 2023 09:28:33 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 09 Feb 2023 09:28:33 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:1e4aec178e0864db93a6f97a20bde3445871a4562c1801185eca1238d3a0e80d`  
		Last Modified: Thu, 09 Feb 2023 03:24:47 GMT  
		Size: 55.0 MB (55046771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1f93ea764dcf05c1b60ac69868cb3e583d17322a93bc9f10b76202e4b5f41e`  
		Last Modified: Thu, 09 Feb 2023 09:40:17 GMT  
		Size: 192.4 MB (192438166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37a8558902508d4fae35ded92a8e32f7b9959c6e33056da0caf70930ad755eaa`  
		Last Modified: Thu, 09 Feb 2023 09:40:03 GMT  
		Size: 2.4 MB (2361758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a5ea8e2a3a165cb7ccae28201238bc6c8ef8fd0f1ac319270805029e022f1e`  
		Last Modified: Thu, 09 Feb 2023 09:40:07 GMT  
		Size: 58.8 MB (58820317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b40f8fd55b9a7572326947ae8f9caa1023d3b08650ed13cedd7d412dd2965fa7`  
		Last Modified: Thu, 09 Feb 2023 09:40:03 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-boot-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:4f1bb6f7583569a5dd9e02f901a2eb9f2106566c2e85555b1041152deaff6d5f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.1 MB (306135531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b075f7b85bf54682a25e767c51a85d703b6642cf623f1f28ef84b482d710135b`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:29 GMT
ADD file:5cf2de182dac36d99ec41918889c9755f9c49c56fa0a8d0ca14040c1d8c04541 in / 
# Thu, 09 Feb 2023 03:58:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:23:26 GMT
COPY dir:a1bd99c3d82513db94430c73467e1e5c69ea4624d0489571d594afe503e15dc5 in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:23:31 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 09:23:31 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 09 Feb 2023 09:23:31 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 09 Feb 2023 09:23:31 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:23:36 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 09 Feb 2023 09:23:36 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 09 Feb 2023 09:23:36 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 09 Feb 2023 09:23:52 GMT
RUN boot
# Thu, 09 Feb 2023 09:23:52 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Thu, 09 Feb 2023 09:23:52 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 09 Feb 2023 09:23:52 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:80dae1b9d879348c210c40024c6e90ef92677ac3515456375fcbb70bdf07b104`  
		Last Modified: Thu, 09 Feb 2023 04:02:11 GMT  
		Size: 53.7 MB (53703368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58beb3d7fb4976caa5ecfe5652ba8512378861c8fbbb227ff0dee4db622d0e2`  
		Last Modified: Thu, 09 Feb 2023 09:34:05 GMT  
		Size: 191.3 MB (191260472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:093a21af92ee2bec084e52149f3bc5fbf78c019b191cd9926f2510e65dd1ed2b`  
		Last Modified: Thu, 09 Feb 2023 09:33:54 GMT  
		Size: 2.4 MB (2351054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a167df6e69ddeb36da09958009cd453743dcf4b83fb9f6f26aaf6a6dd4e3b6cf`  
		Last Modified: Thu, 09 Feb 2023 09:33:56 GMT  
		Size: 58.8 MB (58820238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8abca2f2a5bd7f937c6acaf413949edcce5c7d965ef630accbd367e98a6f8d3`  
		Last Modified: Thu, 09 Feb 2023 09:33:53 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
