## `registry:latest`

```console
$ docker pull registry@sha256:8d4469f4986428830e1e83839f986843821a5ccffeb1b625a6d7bba84390e5a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `registry:latest` - linux; amd64

```console
$ docker pull registry@sha256:f4d532d482a050a3bb02886be6d6deda9c22cf8df44b1465f04c8648ee573a70
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9590880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65f3b3441f044d142ca365389fe0532900b4f4c7ffc47cb65f7bc7bd45857f06`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Wed, 10 May 2023 00:00:10 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 17:20:06 GMT
RUN set -eux; 	version='2.8.2'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='b68ffb849bcdb49639dc91ba97baba6618346f95fedc0fcc94871b31d515d205' ;; 		aarch64) arch='arm64';   sha256='3d500cf4f7f21ade4bdfef28012aef8e1ec2b221d2d8d36d201d94dda84fa727' ;; 		armhf)   arch='armv6';   sha256='e65aeccf69e779681f75b488c4e955f9d9b6aa1d7cf961a9307e8b6d40229373' ;; 		armv7)   arch='armv7';   sha256='045154b2be7a6a3b5d35e14e9afcd29d01813f46ce7ea2ea40958048b621dfd0' ;; 		ppc64le) arch='ppc64le'; sha256='21f5523bb0815af9b7e41b52824d422679309773a14a841e8e685e1f521c1ee0' ;; 		s390x)   arch='s390x';   sha256='2ec05870ffa8c47e764e8de08d00dd0748698cf36394e4b3a503a1339b93e251' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Thu, 11 May 2023 17:20:06 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Thu, 11 May 2023 17:20:06 GMT
VOLUME [/var/lib/registry]
# Thu, 11 May 2023 17:20:07 GMT
EXPOSE 5000
# Thu, 11 May 2023 17:20:07 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Thu, 11 May 2023 17:20:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 11 May 2023 17:20:07 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:8a49fdb3b6a5ff2bd8ec6a86c05b2922a0f7454579ecc07637e94dfd1d0639b6`  
		Last Modified: Tue, 09 May 2023 23:11:26 GMT  
		Size: 3.4 MB (3397490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58116d8bf56953e5f30b7f50257c5bb2b5ba4aba460cb69f2ac57eea00aaa5dc`  
		Last Modified: Wed, 10 May 2023 00:00:24 GMT  
		Size: 284.7 KB (284686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb4a93be51cb152747162cdf555b5b3bbd25dd82ff49f0304e9d00bae094e1b`  
		Last Modified: Thu, 11 May 2023 17:20:17 GMT  
		Size: 5.9 MB (5908092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbdeff65a266fe3c101211f34861a8417504b5df21e7709804cabc620431e7ca`  
		Last Modified: Thu, 11 May 2023 17:20:16 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b102b34ed3d9bd4732a4ac45a5ee2eeee0898be385fafae3b9d85c6e7bc27b0`  
		Last Modified: Thu, 11 May 2023 17:20:16 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:latest` - linux; arm variant v6

```console
$ docker pull registry@sha256:137754a1df36fb9eaf0527edf4fbc657dd120153361a67d61060d5d35eca7463
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9010828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90939e0d115bddf8d2cf6c97b18b832cf788e0e06b2f1b73cc057d4611b9b751`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Tue, 09 May 2023 23:11:04 GMT
ADD file:f87a991e2e9f185fd4a88569d86a9b8e5bc07182e7fa613b95acab25986f2a6c in / 
# Tue, 09 May 2023 23:11:04 GMT
CMD ["/bin/sh"]
# Tue, 09 May 2023 23:59:13 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 17:49:24 GMT
RUN set -eux; 	version='2.8.2'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='b68ffb849bcdb49639dc91ba97baba6618346f95fedc0fcc94871b31d515d205' ;; 		aarch64) arch='arm64';   sha256='3d500cf4f7f21ade4bdfef28012aef8e1ec2b221d2d8d36d201d94dda84fa727' ;; 		armhf)   arch='armv6';   sha256='e65aeccf69e779681f75b488c4e955f9d9b6aa1d7cf961a9307e8b6d40229373' ;; 		armv7)   arch='armv7';   sha256='045154b2be7a6a3b5d35e14e9afcd29d01813f46ce7ea2ea40958048b621dfd0' ;; 		ppc64le) arch='ppc64le'; sha256='21f5523bb0815af9b7e41b52824d422679309773a14a841e8e685e1f521c1ee0' ;; 		s390x)   arch='s390x';   sha256='2ec05870ffa8c47e764e8de08d00dd0748698cf36394e4b3a503a1339b93e251' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Thu, 11 May 2023 17:49:24 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Thu, 11 May 2023 17:49:24 GMT
VOLUME [/var/lib/registry]
# Thu, 11 May 2023 17:49:24 GMT
EXPOSE 5000
# Thu, 11 May 2023 17:49:24 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Thu, 11 May 2023 17:49:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 11 May 2023 17:49:24 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:015ee8d9fb3dca1b18815f1e4ee0d325d1f40cde6f2df4dd307918f7b69167d7`  
		Last Modified: Tue, 09 May 2023 23:11:20 GMT  
		Size: 3.2 MB (3155679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a91154cf231582e0efd441a318760e357cccbcf664976f729d125fe63ccdc9`  
		Last Modified: Tue, 09 May 2023 23:59:27 GMT  
		Size: 284.9 KB (284873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d2b1344e4251975a13c51e7b80c210706ea389367535414144ae145662a30e`  
		Last Modified: Thu, 11 May 2023 17:49:33 GMT  
		Size: 5.6 MB (5569663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0cc14925f38cfb62724629cf4e9b9e63b2e065ffee0d9382087f0a43d01d92`  
		Last Modified: Thu, 11 May 2023 17:49:32 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189c1c0e8c1d4000cd9ace94e39982abc237c7940037d8e5bb1457cdc5eef9d0`  
		Last Modified: Thu, 11 May 2023 17:49:32 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:latest` - linux; arm variant v7

```console
$ docker pull registry@sha256:80b84658c5caac33e6c5f55206a53d134570cebda652dc5a788bb4a288fe414d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8752276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ed117e22f8803964aed6192f206a763be1c7b12853a5e00124dfbfd443a3fa5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Wed, 14 Jun 2023 22:36:15 GMT
ADD file:082f034323c559f3cb9feb6422c88b1ec8017f436d6109e238a5c5384a32a90a in / 
# Wed, 14 Jun 2023 22:36:15 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 02:14:54 GMT
RUN apk add --no-cache ca-certificates
# Thu, 15 Jun 2023 05:22:56 GMT
RUN set -eux; 	version='2.8.2'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='b68ffb849bcdb49639dc91ba97baba6618346f95fedc0fcc94871b31d515d205' ;; 		aarch64) arch='arm64';   sha256='3d500cf4f7f21ade4bdfef28012aef8e1ec2b221d2d8d36d201d94dda84fa727' ;; 		armhf)   arch='armv6';   sha256='e65aeccf69e779681f75b488c4e955f9d9b6aa1d7cf961a9307e8b6d40229373' ;; 		armv7)   arch='armv7';   sha256='045154b2be7a6a3b5d35e14e9afcd29d01813f46ce7ea2ea40958048b621dfd0' ;; 		ppc64le) arch='ppc64le'; sha256='21f5523bb0815af9b7e41b52824d422679309773a14a841e8e685e1f521c1ee0' ;; 		s390x)   arch='s390x';   sha256='2ec05870ffa8c47e764e8de08d00dd0748698cf36394e4b3a503a1339b93e251' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Thu, 15 Jun 2023 05:22:56 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Thu, 15 Jun 2023 05:22:56 GMT
VOLUME [/var/lib/registry]
# Thu, 15 Jun 2023 05:22:56 GMT
EXPOSE 5000
# Thu, 15 Jun 2023 05:22:57 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Thu, 15 Jun 2023 05:22:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 05:22:57 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:633ba29fd335042456b6e2c073636f6fa30de56f1331c442914739b92a479974`  
		Last Modified: Wed, 14 Jun 2023 22:36:49 GMT  
		Size: 2.9 MB (2898508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad2d22fcfeec0ce3f819b7931d5f6b12f8aa5ed452de9e2200f594a3bacfa30`  
		Last Modified: Thu, 15 Jun 2023 02:23:48 GMT  
		Size: 284.1 KB (284075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f82f5b96eddb4e03ab9932f1e65da2619a090d99a8c76a1197a8e3874719d90d`  
		Last Modified: Thu, 15 Jun 2023 05:23:06 GMT  
		Size: 5.6 MB (5569080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccd0cc1417b7d0481142da5e88aaa5a69849fba699c9796723c9cf202f6c85ab`  
		Last Modified: Thu, 15 Jun 2023 05:23:04 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8e00d27434e35a082eb0aae0dbbec8d1606be9170f78a7d8ef73ea9bcb641a`  
		Last Modified: Thu, 15 Jun 2023 05:23:04 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:latest` - linux; arm64 variant v8

```console
$ docker pull registry@sha256:c30ede0bee1037a3b325363e907e96e56240850448ae5bc16905b104cbed5043
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8999291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daace2c8ce4cba7f607a3aa20f4f8dcd7f41506e179f350017f6322150be5516`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 23:22:17 GMT
RUN apk add --no-cache ca-certificates
# Thu, 15 Jun 2023 05:11:09 GMT
RUN set -eux; 	version='2.8.2'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='b68ffb849bcdb49639dc91ba97baba6618346f95fedc0fcc94871b31d515d205' ;; 		aarch64) arch='arm64';   sha256='3d500cf4f7f21ade4bdfef28012aef8e1ec2b221d2d8d36d201d94dda84fa727' ;; 		armhf)   arch='armv6';   sha256='e65aeccf69e779681f75b488c4e955f9d9b6aa1d7cf961a9307e8b6d40229373' ;; 		armv7)   arch='armv7';   sha256='045154b2be7a6a3b5d35e14e9afcd29d01813f46ce7ea2ea40958048b621dfd0' ;; 		ppc64le) arch='ppc64le'; sha256='21f5523bb0815af9b7e41b52824d422679309773a14a841e8e685e1f521c1ee0' ;; 		s390x)   arch='s390x';   sha256='2ec05870ffa8c47e764e8de08d00dd0748698cf36394e4b3a503a1339b93e251' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Thu, 15 Jun 2023 05:11:09 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Thu, 15 Jun 2023 05:11:10 GMT
VOLUME [/var/lib/registry]
# Thu, 15 Jun 2023 05:11:10 GMT
EXPOSE 5000
# Thu, 15 Jun 2023 05:11:10 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Thu, 15 Jun 2023 05:11:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 05:11:10 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a768fa670f57b0faf1a0a8cb211432ed97307628729fa53e3ea9981ba7512d4`  
		Last Modified: Wed, 14 Jun 2023 23:27:58 GMT  
		Size: 286.3 KB (286290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c6c92738d9e96414d6811cc15d0745f9b06de8e4612fbd889d310e8ab6c0ae`  
		Last Modified: Thu, 15 Jun 2023 05:11:30 GMT  
		Size: 5.4 MB (5383139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76a9836469a21944692d08ac0b4695e542a8b522e1af315b5cdeb5bcdc1e4559`  
		Last Modified: Thu, 15 Jun 2023 05:11:30 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffab796d570071e2ce5f269ae57fa492668c1360f6645cea69a67064b6f73119`  
		Last Modified: Thu, 15 Jun 2023 05:11:30 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:latest` - linux; ppc64le

```console
$ docker pull registry@sha256:d4b0d0513766bedf1bf33e88a7b23d04dceac8e368813baee08b5c65432c65e6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8916659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af2e915b088a3875782825bd7f4fc6c890028b38f5f376241b21b1acf7bc8e7b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Tue, 09 May 2023 23:11:09 GMT
ADD file:0a227602737a24c596923d3fd0a7c8b7d9000dbc6b80561473def09abbebbfa6 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Tue, 09 May 2023 23:59:39 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 18:16:49 GMT
RUN set -eux; 	version='2.8.2'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='b68ffb849bcdb49639dc91ba97baba6618346f95fedc0fcc94871b31d515d205' ;; 		aarch64) arch='arm64';   sha256='3d500cf4f7f21ade4bdfef28012aef8e1ec2b221d2d8d36d201d94dda84fa727' ;; 		armhf)   arch='armv6';   sha256='e65aeccf69e779681f75b488c4e955f9d9b6aa1d7cf961a9307e8b6d40229373' ;; 		armv7)   arch='armv7';   sha256='045154b2be7a6a3b5d35e14e9afcd29d01813f46ce7ea2ea40958048b621dfd0' ;; 		ppc64le) arch='ppc64le'; sha256='21f5523bb0815af9b7e41b52824d422679309773a14a841e8e685e1f521c1ee0' ;; 		s390x)   arch='s390x';   sha256='2ec05870ffa8c47e764e8de08d00dd0748698cf36394e4b3a503a1339b93e251' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Thu, 11 May 2023 18:16:51 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Thu, 11 May 2023 18:16:52 GMT
VOLUME [/var/lib/registry]
# Thu, 11 May 2023 18:16:53 GMT
EXPOSE 5000
# Thu, 11 May 2023 18:16:54 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Thu, 11 May 2023 18:16:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 11 May 2023 18:16:56 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:5c0986f188e93dd7e76a4dc49a9170da2cd124709f5e1590b378e31a2b0d9587`  
		Last Modified: Tue, 09 May 2023 23:11:31 GMT  
		Size: 3.4 MB (3385631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376ba25ac41cec041d831e456ad293ec2efd7e4fd1357ae113210bfddd447a5f`  
		Last Modified: Wed, 10 May 2023 00:00:00 GMT  
		Size: 286.7 KB (286653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b1ec9c6f465b15b306336acae5c5a598d5e2882c1168215695fa4a7494fe38`  
		Last Modified: Thu, 11 May 2023 18:17:10 GMT  
		Size: 5.2 MB (5243762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab0002319e03ce2dc9ecb8a56ad4fc3df776e0c2128bbdd67590ae9f51d6af0`  
		Last Modified: Thu, 11 May 2023 18:17:08 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb78034d869215f477a6fd619a5df23be5bc66c20ca407b0e0a0b5e83b91e61a`  
		Last Modified: Thu, 11 May 2023 18:17:08 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:latest` - linux; s390x

```console
$ docker pull registry@sha256:c540add056d1cc2eba53ea2f671f907b59819e8e1cdd14c36b38b64ffb40d70f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9162894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03520cb0cb8a95cf4d8e70ca1aed5c2543df76542b02771b86469d919ffe7c00`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Tue, 09 May 2023 23:11:06 GMT
ADD file:89d6e366e8ab41011a5866f8ca43aac6cfef00edffebad565918ab632a6d6210 in / 
# Tue, 09 May 2023 23:11:07 GMT
CMD ["/bin/sh"]
# Wed, 10 May 2023 00:00:53 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 17:42:38 GMT
RUN set -eux; 	version='2.8.2'; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  arch='amd64';   sha256='b68ffb849bcdb49639dc91ba97baba6618346f95fedc0fcc94871b31d515d205' ;; 		aarch64) arch='arm64';   sha256='3d500cf4f7f21ade4bdfef28012aef8e1ec2b221d2d8d36d201d94dda84fa727' ;; 		armhf)   arch='armv6';   sha256='e65aeccf69e779681f75b488c4e955f9d9b6aa1d7cf961a9307e8b6d40229373' ;; 		armv7)   arch='armv7';   sha256='045154b2be7a6a3b5d35e14e9afcd29d01813f46ce7ea2ea40958048b621dfd0' ;; 		ppc64le) arch='ppc64le'; sha256='21f5523bb0815af9b7e41b52824d422679309773a14a841e8e685e1f521c1ee0' ;; 		s390x)   arch='s390x';   sha256='2ec05870ffa8c47e764e8de08d00dd0748698cf36394e4b3a503a1339b93e251' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget -O registry.tar.gz "https://github.com/distribution/distribution/releases/download/v${version}/registry_${version}_linux_${arch}.tar.gz"; 	echo "$sha256 *registry.tar.gz" | sha256sum -c -; 	tar --extract --verbose --file registry.tar.gz --directory /bin/ registry; 	rm registry.tar.gz; 	registry --version
# Thu, 11 May 2023 17:42:39 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Thu, 11 May 2023 17:42:39 GMT
VOLUME [/var/lib/registry]
# Thu, 11 May 2023 17:42:39 GMT
EXPOSE 5000
# Thu, 11 May 2023 17:42:39 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Thu, 11 May 2023 17:42:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 11 May 2023 17:42:39 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:25da54cc0a08f4ca602c6bcd3e52d70082eb8a25ee022bc9f1dda019de49197a`  
		Last Modified: Tue, 09 May 2023 23:11:35 GMT  
		Size: 3.2 MB (3226303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a72fc573296d33547281b8f37ff15a477a2844bdd1fff61bf191b5f18e14354`  
		Last Modified: Wed, 10 May 2023 00:01:13 GMT  
		Size: 285.1 KB (285083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b57f17af6c94a06241e21d886a8abe587e6b440450b254c676f1c4b786f3ac`  
		Last Modified: Thu, 11 May 2023 17:42:50 GMT  
		Size: 5.7 MB (5650895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7454e9ed0758cf37d79d72486800a8831527fa61ba8783dbdefe536c753bf153`  
		Last Modified: Thu, 11 May 2023 17:42:50 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e54e7e37ae1feb01f31a9b42769989472883d00bb6ea9cf8d76a223cd28aa3ec`  
		Last Modified: Thu, 11 May 2023 17:42:49 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
