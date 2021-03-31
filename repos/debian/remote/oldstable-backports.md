## `debian:oldstable-backports`

```console
$ docker pull debian@sha256:d9e503d6cba9646fe8ffda3159382f26df271de7b5b0a662797dcb53404ff373
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `debian:oldstable-backports` - linux; amd64

```console
$ docker pull debian@sha256:a9363df3326a7329cc0ea4bf2fc4ed34dfc7322d9732ce97b269bf06cf4a02b6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45380188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8181c98a7f4a8bb65f7aeb10de37816f4e5e086845ca7997120b3c6ad98de091`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:39 GMT
ADD file:d88609450441037d9f94bedd7863c0757adedffc5454ab1e86564c53892f241c in / 
# Tue, 30 Mar 2021 21:49:39 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 21:49:43 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:dbf60affa793c8897a2385d554dfc05cb353a2cc875072921f231e6993d3489d`  
		Last Modified: Tue, 30 Mar 2021 21:54:36 GMT  
		Size: 45.4 MB (45379962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e8773fbadd7557be14461321bc24bc4a29894073e7f38c024eb8b829408fd78`  
		Last Modified: Tue, 30 Mar 2021 21:54:46 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:800ca9465854e69408dc74acf47fcd294cc49726f46dc86e58997da7cb9e684f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44092206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2208f9162a7b0b9bebf442f5eec61dcb91b163e5d258287fcd146b1a1c3de442`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:51:28 GMT
ADD file:37fd91c40ad4803b3533eb01c9428acea8a2bbaac9de1522e7120961985779df in / 
# Tue, 30 Mar 2021 21:51:34 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 21:51:43 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:06a3970b170550ee376fb43d470d710ec0d20a2aec6584021f7cf3ea62188706`  
		Last Modified: Tue, 30 Mar 2021 21:59:08 GMT  
		Size: 44.1 MB (44091981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984fb38d5c2c3edf1cb2eb6fd2a9229a2e0b7b2694815fb8c8693d6147bc6970`  
		Last Modified: Tue, 30 Mar 2021 21:59:15 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:7ad26a1d605d7b26536b16dccf9df2ca175eed48652e8f54ec1d86cabe34fdb3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42120479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b36f814c3b1d5a46424bd46455e5f3a9fbe77241c8703b584aeb07fe4e9cb9ff`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 23:09:00 GMT
ADD file:9479154f63a05d43fe3e1a8184262f8e5d13edbfb33c0304401095c768197598 in / 
# Tue, 30 Mar 2021 23:09:04 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:09:16 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:974eca9395e6d262b50b5df20633e316ddbfbb3f4d00b6251df463f29c237f7c`  
		Last Modified: Tue, 30 Mar 2021 23:16:50 GMT  
		Size: 42.1 MB (42120254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a30b36f8a10199af6b06d3eb1790803ee1706d38769e3fec04e2088e4e0e4ae9`  
		Last Modified: Tue, 30 Mar 2021 23:17:02 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:75f1e08f3bf48b4f9ce4ea198a4c8cf72434f65b599923f9e99eccc0f98e4b28
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43177841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2f37983450965dd4c18586972f9045978ab37977d4cf8a9540fe5734702daa3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:47:31 GMT
ADD file:04791f9f5947bd47ab653948b880a530a33156485a6f3730cb2de01962cffeae in / 
# Tue, 30 Mar 2021 21:47:39 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 21:47:50 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7e58098b448af522274bc252ad866fe1c56efba6ed74d7931be0fd9c28ccbc48`  
		Last Modified: Tue, 30 Mar 2021 21:54:46 GMT  
		Size: 43.2 MB (43177614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d471b5d87a1d1756d9d9057504b242243fab6964845cb0b42c808e4b64270f54`  
		Last Modified: Tue, 30 Mar 2021 21:54:56 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:a95483f1325cd3e5e4224e7d9bab68e59995bc20c929f1187639e9114ba1e611
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.1 MB (46098782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee7e097caf3c4a2a38fefc559c4560f0c32dd48078757d2883aa5e01fd4cfb68`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:40:03 GMT
ADD file:b8c02696233334e537966fc2bf428942697c9c2cabfadc513896052211d79df2 in / 
# Tue, 30 Mar 2021 21:40:04 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 21:40:10 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3096bf74d7801283909c1c270b64ee3e6178771dc32e0bb7007f55a0ff5834d2`  
		Last Modified: Tue, 30 Mar 2021 21:47:08 GMT  
		Size: 46.1 MB (46098555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca64dd39403e9226d1e4bd7982bf56dda7d42d36f3ea8f0e3470131f4afb610d`  
		Last Modified: Tue, 30 Mar 2021 21:47:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
