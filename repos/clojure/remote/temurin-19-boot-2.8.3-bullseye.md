## `clojure:temurin-19-boot-2.8.3-bullseye`

```console
$ docker pull clojure@sha256:5769320788c4b4a3311be941c109305fc8d6a0bdfb86c7dbf91a53287e3f4e55
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-boot-2.8.3-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:cdfbe7bfd57c47465e7cd416e0109fa935cbdd09c4ecad6b2a69e9ae3591432d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.3 MB (317342129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6de63c94dd43e15ab8b705614f1049030dbb2f0d03e772b8f4664fb4ea57efdc`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:05 GMT
ADD file:b03d13d345c29f69557f410c8504e748226756d1f48e5abdb63cd40179b2640c in / 
# Thu, 09 Feb 2023 03:20:05 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:22:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:31:09 GMT
COPY dir:94cb5af8175285c10c94286222d8a35302f3f8c290e00011a75c67156659d6ab in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:31:11 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 09:31:11 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 09 Feb 2023 09:31:11 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 09 Feb 2023 09:31:11 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:31:17 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 09 Feb 2023 09:31:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 09 Feb 2023 09:31:17 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 09 Feb 2023 09:31:35 GMT
RUN boot
# Thu, 09 Feb 2023 09:31:35 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Thu, 09 Feb 2023 09:31:35 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 09 Feb 2023 09:31:35 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:1e4aec178e0864db93a6f97a20bde3445871a4562c1801185eca1238d3a0e80d`  
		Last Modified: Thu, 09 Feb 2023 03:24:47 GMT  
		Size: 55.0 MB (55046771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441046777b829253c9900fed7834e1437d44d485f4ec90904dc51bc5aac05148`  
		Last Modified: Thu, 09 Feb 2023 09:42:23 GMT  
		Size: 201.1 MB (201112949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d83e8d70b4ddc7fa2baeb223f53b510152bc8a430e87f8ae7283d651780b370f`  
		Last Modified: Thu, 09 Feb 2023 09:42:08 GMT  
		Size: 2.4 MB (2361683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce97ae42bd76b200ed6a250b45956055d4e90d7dcc3d22cde60fc5b4adc425e`  
		Last Modified: Thu, 09 Feb 2023 09:42:11 GMT  
		Size: 58.8 MB (58820325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edccb83e2efea5b42ae6e4e389186faac15c41a75f6ff307a42bad5d33bf5e59`  
		Last Modified: Thu, 09 Feb 2023 09:42:08 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-boot-2.8.3-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:7a2e9499ffb238589208b11349a05ad000d860d43f25f60e104fcda1d185ffdb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.7 MB (314730277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3a8f1b8350ca89e3d70ec68fcc4915fc80e5a0d820781a82880620993f12cb0`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:29 GMT
ADD file:5cf2de182dac36d99ec41918889c9755f9c49c56fa0a8d0ca14040c1d8c04541 in / 
# Thu, 09 Feb 2023 03:58:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:25:55 GMT
COPY dir:9a6a873ca11063f6f04e7f088397a1fce771e2b1aa8590b72eb07158cfac883f in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:26:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 09:26:00 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 09 Feb 2023 09:26:00 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 09 Feb 2023 09:26:00 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:26:05 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 09 Feb 2023 09:26:05 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 09 Feb 2023 09:26:05 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 09 Feb 2023 09:26:21 GMT
RUN boot
# Thu, 09 Feb 2023 09:26:21 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Thu, 09 Feb 2023 09:26:21 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 09 Feb 2023 09:26:21 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:80dae1b9d879348c210c40024c6e90ef92677ac3515456375fcbb70bdf07b104`  
		Last Modified: Thu, 09 Feb 2023 04:02:11 GMT  
		Size: 53.7 MB (53703368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04575e4d68cefe99b7db24f9eba8de51503dbe724ee7b0b0862498a73eeefbf3`  
		Last Modified: Thu, 09 Feb 2023 09:36:01 GMT  
		Size: 199.9 MB (199855167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad92a7b5ab05b2dcec1229c5d9eff369d4f487e58fe2fff56b119014d60bf1f5`  
		Last Modified: Thu, 09 Feb 2023 09:35:44 GMT  
		Size: 2.4 MB (2350979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3867afd192c0ec457cf73f9543268a6b82948e17beca69ca58af8090704cd44f`  
		Last Modified: Thu, 09 Feb 2023 09:35:46 GMT  
		Size: 58.8 MB (58820361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:755331987ce12c541b212dec261e47399c7d05357d056b8f5c9d27ae72789572`  
		Last Modified: Thu, 09 Feb 2023 09:35:43 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
