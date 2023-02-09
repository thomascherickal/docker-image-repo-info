## `clojure:temurin-11-boot-2.8.3-bullseye`

```console
$ docker pull clojure@sha256:f96bd3fce722a2f67becbcd01fdd7c21daaf143d07443535f145cf84091b2955
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-boot-2.8.3-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:e45572ec5b7acc604a3d0273b837bdacd4eded29f453cf93103c2cb1dfac094f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.7 MB (314704365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f1c9833dfe683a33aa0c243455c11170c700da3a03bdae7a457fab0e65e814f`
-	Default Command: `["boot","repl"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:05 GMT
ADD file:b03d13d345c29f69557f410c8504e748226756d1f48e5abdb63cd40179b2640c in / 
# Thu, 09 Feb 2023 03:20:05 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:22:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:25:04 GMT
COPY dir:fdbc5e9dec2946fa124877176e92a68dd3fe3a70def5bb906a6040c4a1303a2d in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:25:06 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 09:25:06 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 09 Feb 2023 09:25:06 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 09 Feb 2023 09:25:06 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:25:12 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 09 Feb 2023 09:25:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 09 Feb 2023 09:25:12 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 09 Feb 2023 09:25:29 GMT
RUN boot
# Thu, 09 Feb 2023 09:25:30 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:1e4aec178e0864db93a6f97a20bde3445871a4562c1801185eca1238d3a0e80d`  
		Last Modified: Thu, 09 Feb 2023 03:24:47 GMT  
		Size: 55.0 MB (55046771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36fa5505d5f9a403b5fa799c74b7639e1188ddc30c0db155b99238ff035c03ed`  
		Last Modified: Thu, 09 Feb 2023 09:38:26 GMT  
		Size: 198.5 MB (198475422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356d56fdf570046c64cfef98607a85390634d5bd87538e8008b3cfb278e8b374`  
		Last Modified: Thu, 09 Feb 2023 09:38:11 GMT  
		Size: 2.4 MB (2361639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90bf9a9ba2bf48a6fd6879d38261dd902a3265fc44e5ed5064724ce5bbec65a`  
		Last Modified: Thu, 09 Feb 2023 09:38:14 GMT  
		Size: 58.8 MB (58820533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-boot-2.8.3-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:a3c4cb295b1be2d86eb14c55ffa3875506c3355a1d84fea341c58160b7d3b050
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **310.1 MB (310115027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e56c0d6118e93f3f1092c62384bc8743833a67184ccfb986ed1fb6263bc1766`
-	Default Command: `["boot","repl"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:29 GMT
ADD file:5cf2de182dac36d99ec41918889c9755f9c49c56fa0a8d0ca14040c1d8c04541 in / 
# Thu, 09 Feb 2023 03:58:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:20:57 GMT
COPY dir:b661686bf8d434588756c45f2ef6e7f314f32f753cf180ef8fb45397388f098c in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:21:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 09:21:01 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 09 Feb 2023 09:21:01 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 09 Feb 2023 09:21:01 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:21:06 GMT
RUN apt-get update && apt-get install -y make wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 09 Feb 2023 09:21:06 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 09 Feb 2023 09:21:06 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 09 Feb 2023 09:21:22 GMT
RUN boot
# Thu, 09 Feb 2023 09:21:22 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:80dae1b9d879348c210c40024c6e90ef92677ac3515456375fcbb70bdf07b104`  
		Last Modified: Thu, 09 Feb 2023 04:02:11 GMT  
		Size: 53.7 MB (53703368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84634f2412fd0db390d1dd82c75871f25a933e1333ec652a66114e5288d4d33f`  
		Last Modified: Thu, 09 Feb 2023 09:32:24 GMT  
		Size: 195.2 MB (195240325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c69a9ab919130b6940b208e82c1080cbb95a0913820910f803b169bc48a1b1`  
		Last Modified: Thu, 09 Feb 2023 09:32:12 GMT  
		Size: 2.4 MB (2351008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e17a53c638a5a28494f2a2321fbd85651560a9b4721e18933dec2487366c22`  
		Last Modified: Thu, 09 Feb 2023 09:32:15 GMT  
		Size: 58.8 MB (58820326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
