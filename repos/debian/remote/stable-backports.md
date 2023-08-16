## `debian:stable-backports`

```console
$ docker pull debian@sha256:3c8c1479047e064264c632b1c1cf941ee63640dd3c9e7c6e28526bd9539ca044
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `debian:stable-backports` - linux; amd64

```console
$ docker pull debian@sha256:c05ba525395fad083646abb88998f557a1f3be0775aff3972cec3b55004234fc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49557591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:330d248e40fe0181c506883c8707b28a918b04221b7d7a4c454c48dcecef80f7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:26:44 GMT
ADD file:467d54fcdcc4a4fc484eb81623a50891c72242f1da2748a7616413dc449fad22 in / 
# Thu, 27 Jul 2023 23:26:44 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:26:48 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1924af148565f8d4a8be4dab08aa865788130cd4461a64b42f5470404fb3f613`  
		Last Modified: Thu, 27 Jul 2023 23:32:41 GMT  
		Size: 49.6 MB (49557366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073b60c96f531b6e2cdfad88bacd7360d600a49d9b19fcd108b0e173b3b3c2be`  
		Last Modified: Thu, 27 Jul 2023 23:32:51 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:1bc092bcf58e6b52fc12c54b28339a01e51d7568046a93b6a4f2acfa5e6a9da3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47415211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3a71e20ab4f69b1566cba1c2b2c784d6cb11807f4d819aba4cc3e911f40d0c2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:49:25 GMT
ADD file:8dc6eaf906602786cbd9987cf43dcee5a498e22fc886e23a09942a544185206d in / 
# Tue, 15 Aug 2023 23:49:25 GMT
CMD ["bash"]
# Tue, 15 Aug 2023 23:49:28 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:bc3aecc99440091f319da44ca13cf8fcc17ea6d16aa081e4dc943a04de7dffad`  
		Last Modified: Tue, 15 Aug 2023 23:53:35 GMT  
		Size: 47.4 MB (47414986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c931aae837293a555f69f1d1ab39ae154a6b2071b0116a9057fb3b22e9ff91ba`  
		Last Modified: Tue, 15 Aug 2023 23:53:44 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:7fa92daf530a3c223bc3052052a7e2e37589eb96c79560bb3c9d8777527a2706
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45233212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cdc1c05c4a0bfedc3732c7313d16ea72e42c087cf7c2076e09a1cc6042329b6`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 28 Jul 2023 00:00:19 GMT
ADD file:20e9751a1ac7b1a4351d33fb8f1d9eafbfa0418af09f0f4dfac07e45c2dd03f1 in / 
# Fri, 28 Jul 2023 00:00:19 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:00:22 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:994d9244915c9e6508d8815d01ebde033ea2886f7b95198654dfdd8af2526b7c`  
		Last Modified: Fri, 28 Jul 2023 00:06:35 GMT  
		Size: 45.2 MB (45232988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58abaa9a96caf18c9eadc88d54ffe8f829e0eab6504a9641292a084b90830c6b`  
		Last Modified: Fri, 28 Jul 2023 00:06:44 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:1197b08341458739995e52580c7380e5b05a0e3d036b3048265cd2748cb68ded
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49591531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d16c7ec8bf942d9fb77982d91eb6e35dc9d2c047f3d56fc87c7517b69ab05797`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:41:13 GMT
ADD file:a09ec75380775bbf01dde2c0e1c1b8cde93bc2a0df9f1f0991ec4ef6eb2d74cb in / 
# Tue, 15 Aug 2023 23:41:14 GMT
CMD ["bash"]
# Tue, 15 Aug 2023 23:41:16 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3e7f93afe9888e6966033933fb176e84297a1aa924b48df5246a9be951cff26d`  
		Last Modified: Tue, 15 Aug 2023 23:46:20 GMT  
		Size: 49.6 MB (49591309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b59c18b1e0d64a55be6fd785707641a93205cf4afbd5a6af10d317cbd40ffd`  
		Last Modified: Tue, 15 Aug 2023 23:46:28 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; 386

```console
$ docker pull debian@sha256:fbc187555324b75fb7c552f65107100ce17bdea422a290ab76d4c4ca5cb40f69
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50568230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d39998b53d00f4dd01d138076ba0a689703f849d4b212887c7ccdb6a20f15af8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:52 GMT
ADD file:b881220bd52b0e29ab527bbb127826af28137394707aa96ef81fc5e8a092b131 in / 
# Tue, 15 Aug 2023 23:40:53 GMT
CMD ["bash"]
# Tue, 15 Aug 2023 23:40:55 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6682406395788a3f43e3ef89b4b2d8f23bd65e00473ca4a3fe73eb68ac15c85a`  
		Last Modified: Tue, 15 Aug 2023 23:47:05 GMT  
		Size: 50.6 MB (50568006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f20b75553f6be14320de84d99fa19a105353ef56360a264681a45ca20b29c8c1`  
		Last Modified: Tue, 15 Aug 2023 23:47:14 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:07d61060db92b65e4efb917c9d04d12c827041bf8f13ad88b3dbe484ecc4e946
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49542274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:062d57e3b04df6cc94bf1ea34d219d2886b1a63889639d8fbfb3304f598323be`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:15:34 GMT
ADD file:224ff2c2330e0b11d4a23e2914ed2a70e26830febc235424ef7e0f8010c3b882 in / 
# Thu, 27 Jul 2023 23:15:40 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:15:53 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:9f78c9f83bb7be271c6dcfb95642a820bcdbb0fe6c6d7131806209e41f2c3dbf`  
		Last Modified: Thu, 27 Jul 2023 23:27:01 GMT  
		Size: 49.5 MB (49542048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd9c0b0a2f467e113d3725888bbce936954d5cbc8b61e556177348cfeacb57a4`  
		Last Modified: Thu, 27 Jul 2023 23:27:12 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:4266eefbda56f2db624b5a262ab645daed940fdbae66f981a2ba794de864f9b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.5 MB (53543567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f3d92704f54b2eff654d6887a3a95cb216126d1323276a5c6ae685c2b5b9b7b`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:09 GMT
ADD file:09c45999929f09514adf2cb9d6d0f0a57f4aacd62c4bd5ef96405b1588914a05 in / 
# Thu, 27 Jul 2023 23:25:12 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:25:16 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1d1be89ccee2abf523e50d302d1b9d4b49c822db5e4182c8f25dba9e0e2f1519`  
		Last Modified: Thu, 27 Jul 2023 23:32:43 GMT  
		Size: 53.5 MB (53543345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c001470affab71ef675f6cb32c77173fc0e763a84dc68d36f50005bd294174f3`  
		Last Modified: Thu, 27 Jul 2023 23:32:56 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; s390x

```console
$ docker pull debian@sha256:65b5381a6e86588380ebc8ec323489dddccd6e7873a5265f1b414b3054779ba2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47922257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bdc7bf77b2e0df60628652df3882fdba36347de59c675e34e4c4e0ab2ffbdef`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:44:19 GMT
ADD file:17756dcd18bc59a255a8c6b01ed9549c2e3abfdfa944090abd110bd44831e414 in / 
# Tue, 15 Aug 2023 23:44:26 GMT
CMD ["bash"]
# Tue, 15 Aug 2023 23:44:32 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2b0ffa164418dcf7104b29fee7c17204350bdc187cf3fe5d71eb1fce50d92471`  
		Last Modified: Tue, 15 Aug 2023 23:49:23 GMT  
		Size: 47.9 MB (47922032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70502d5fff11c2cbd06be7ac42c78e0f767284afe2e701b715492755cb6f9bb6`  
		Last Modified: Tue, 15 Aug 2023 23:49:28 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
