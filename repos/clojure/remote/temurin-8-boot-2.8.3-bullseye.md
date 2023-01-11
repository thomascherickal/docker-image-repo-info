## `clojure:temurin-8-boot-2.8.3-bullseye`

```console
$ docker pull clojure@sha256:e3115856423c940c90af2e2f93f40e22876bd06d45f979cb54a2ccc9b6fcb88b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-boot-2.8.3-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:deef71cf6bfa0a250edf2da3d3787000b8fd9798abce3b475a2625a7ab5e2344
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.7 MB (219737667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ef661f8b9b83b10826023c06a6a4f519e011796a9e5f26c1262b15728b9d162`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:29 GMT
ADD file:917750a82b29f8f7f88a121017bd9dfeb0fbcc8f0697a009f08b6b58246eff4b in / 
# Wed, 11 Jan 2023 02:34:30 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:18:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 11 Jan 2023 03:18:58 GMT
COPY dir:53540f2d79f4eef9b2bf8c4b39ecdbbd82fb14bfcf951e14853afffd2efa2ecb in /opt/java/openjdk 
# Wed, 11 Jan 2023 03:18:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 03:18:59 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 11 Jan 2023 03:18:59 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 11 Jan 2023 03:18:59 GMT
WORKDIR /tmp
# Wed, 11 Jan 2023 03:19:05 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 11 Jan 2023 03:19:05 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 11 Jan 2023 03:19:05 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 11 Jan 2023 03:19:57 GMT
RUN boot
# Wed, 11 Jan 2023 03:19:57 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:bbeef03cda1f5d6c9e20c310c1c91382a6b0a1a2501c3436b28152f13896f082`  
		Last Modified: Wed, 11 Jan 2023 02:38:42 GMT  
		Size: 55.0 MB (55025206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb0ac03ea060d862b95eed061f539ba623b94a8f2eb558fedded843bbe2bed3`  
		Last Modified: Wed, 11 Jan 2023 03:34:32 GMT  
		Size: 103.5 MB (103530609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88f4fde785bdb2ed1a0b3740b87d8c85f5c4695ebe1efc9e248029152bf74c2f`  
		Last Modified: Wed, 11 Jan 2023 03:34:23 GMT  
		Size: 2.4 MB (2360765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2505e8c5841b3d6ead029dad58af1f17e8e06ff5bbf836442f18b6159afe0604`  
		Last Modified: Wed, 11 Jan 2023 03:34:27 GMT  
		Size: 58.8 MB (58821087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-boot-2.8.3-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:95f615413ca9c160cfd8383a13237e155c0547f440ab2c5c7fd99f6ca09f39e6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.5 MB (217479299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdf2e95c446ce9b4187fbadced92df092adaf24df00fc4689e75aa18fac6c1a0`
-	Default Command: `["boot","repl"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:24 GMT
ADD file:9e185c2d9ca8a231a39ee2b1761fcdff75065252d25a65a207acb7a319c1cf23 in / 
# Wed, 11 Jan 2023 02:57:25 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:14 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 11 Jan 2023 03:38:16 GMT
COPY dir:8a3fd802e7e57a45d80b19a89e91b421563b952585d39995819354f278317671 in /opt/java/openjdk 
# Wed, 11 Jan 2023 03:38:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 03:38:18 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 11 Jan 2023 03:38:18 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 11 Jan 2023 03:38:18 GMT
WORKDIR /tmp
# Wed, 11 Jan 2023 03:38:24 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 11 Jan 2023 03:38:24 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 11 Jan 2023 03:38:24 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 11 Jan 2023 03:38:42 GMT
RUN boot
# Wed, 11 Jan 2023 03:38:42 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:c345c9e441f5f49235768af74b8ab37743652d38958afaa000edd56d7b2f0540`  
		Last Modified: Wed, 11 Jan 2023 03:00:56 GMT  
		Size: 53.7 MB (53681859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940f37610f026c5932e22a78105d91762ce8fc1b671393115df608bc205e894c`  
		Last Modified: Wed, 11 Jan 2023 03:50:57 GMT  
		Size: 102.6 MB (102626579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba7cbb1f21cef7f11af4e79f9eb9dbfbc976fe9f2ecf693cc7b19666a22601d6`  
		Last Modified: Wed, 11 Jan 2023 03:50:50 GMT  
		Size: 2.4 MB (2350581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568b5382df9bc90cda18953a775b8fba8ef28893908656d4f11527a814e795a7`  
		Last Modified: Wed, 11 Jan 2023 03:50:53 GMT  
		Size: 58.8 MB (58820280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
