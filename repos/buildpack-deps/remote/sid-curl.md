## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:021706d0d55d40a96982ded0e76f1b459dc2b5c4ae0fb28e6076d9232929e2e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:sid-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:7d2668493b4f046b71c6260d3279c31c6ba4f2a286b05c50c2f5b4e868e1cf3d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.7 MB (73749616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6413f0d2d0378de2d6a8d9d1402a6084483971c14f3fd113e9eb890502af0b02`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:26:24 GMT
ADD file:89538c836015e15bfe955d940c080e251ce5b25e2cfaac73d8ce77f8475cd08f in / 
# Thu, 27 Jul 2023 23:26:25 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:05:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9828fc546889681c4c23160b0ee9abb2a08f99ec58b166856cf38d03e0173700`  
		Last Modified: Thu, 27 Jul 2023 23:32:15 GMT  
		Size: 49.5 MB (49462924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1415ec03edfc71940d466b16992ddd3915658c3368432ddd33223a9bf80a2b`  
		Last Modified: Fri, 28 Jul 2023 03:10:17 GMT  
		Size: 24.3 MB (24286692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:774563c7ab34b698df26f2291a44ab24b899f0da48b5794c4a9e51b889427e90
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.3 MB (70346529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6be2e6d9a14df3fc131f09bce7ad48cdbaba68d086d00efc976e7c7d409a7f17`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:49:11 GMT
ADD file:2d486f4790de50d5a173ed5147c22ebcaaade283f5bdf6b62bc072050fc164c1 in / 
# Tue, 15 Aug 2023 23:49:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:44:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0fb27bc4b8f884dd1bc1129dd87397bcc993ec915005657bd21811eb84745100`  
		Last Modified: Tue, 15 Aug 2023 23:53:08 GMT  
		Size: 47.4 MB (47403781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f883267a6e0fd23a7321e7809daf18ea9fde5af7d382347913aa6b73346ef73`  
		Last Modified: Wed, 16 Aug 2023 00:49:09 GMT  
		Size: 22.9 MB (22942748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:7aa62e1d9c56fdf41c87e3887595f8c62f23d55bc0264ed2eed3cb92781c30a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.4 MB (67359941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbae1d38f1729ba21724854f9beb2bc47acb5dda4f340347d633af0d94e57f0b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 00:18:42 GMT
ADD file:2a1f1ecc1cfa876ccc22e6ef2a3a4ea39a83aec70ecde3f7cdaddee69dac2002 in / 
# Wed, 16 Aug 2023 00:18:43 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:34:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ccc7cdd48defe44f9a45f06f57d69b192155657bc5d244f915958c2027d645c3`  
		Last Modified: Wed, 16 Aug 2023 00:24:10 GMT  
		Size: 45.2 MB (45189279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6609fcf5feea7fb712abd4f4cc12586f4960ac4271da561ebf2ff0717e096c5`  
		Last Modified: Wed, 16 Aug 2023 05:50:44 GMT  
		Size: 22.2 MB (22170662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f357b484f94d65bee85830215f8a99bd873b9b6c588d9b18d73a660d1b7d230b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.3 MB (73342350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ad8010747ba13453458120a56606c915f892703fb198850dde407010ab2ae49`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:41:01 GMT
ADD file:8064072457ccf7b4072e08095fa84f96b0fe3387ec8f302afde022186aa3eab5 in / 
# Tue, 15 Aug 2023 23:41:01 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4513653e4d749342b34f60c592adaf0ef4af993e76a913a1c086a4229a0e3afe`  
		Last Modified: Tue, 15 Aug 2023 23:45:54 GMT  
		Size: 49.5 MB (49531730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f5de6e756ae0263d5d8056bc2a6f2a8e87f5e28dde8b746fa6cb29bcd33513`  
		Last Modified: Wed, 16 Aug 2023 01:41:04 GMT  
		Size: 23.8 MB (23810620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:d97b42d29a664dcae93cfd874db1be9d3c194cb92623f2447128c5bb0a572761
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75747069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02ac27c3bf31307e25bfee6c4ee200ddeab2b6f606757de278d52f1d0566c9aa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:34 GMT
ADD file:d86f66385d3993c597ac040a976cd8a826b097d014cc4f3b69d8ebfaa5aa6eff in / 
# Tue, 15 Aug 2023 23:40:35 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:32:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e41394c7daa90fb4aae0f67d43af5ee9838fb125e249fc0002bfdc3b90bb6c05`  
		Last Modified: Tue, 15 Aug 2023 23:46:33 GMT  
		Size: 50.6 MB (50631355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55fb36009acd0e1d753239daf3a185a717a7e268ceb556a566bab97416024ee1`  
		Last Modified: Wed, 16 Aug 2023 00:38:32 GMT  
		Size: 25.1 MB (25115714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:6d22f564936ef6047f439f288c6487d49ea9ea94a3d3d823ba789aae0b57477f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73200135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73a82efa8a0cbd2145763c100f743ab0c6073cedbe7ab03288024f57dd678d67`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:14:28 GMT
ADD file:5d5d4b53ad51debb95681500ba4a990279ff7fdd2ff80d4d4333b7dc647c0543 in / 
# Thu, 27 Jul 2023 23:14:34 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:28:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b48d6f46b6cff8bfdf81f7ffbfa05dff828e1d7545e640bf61d5486c1b79892`  
		Last Modified: Thu, 27 Jul 2023 23:25:52 GMT  
		Size: 49.3 MB (49334598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde2d4334b6bd5986094b014a83b3832c21ffb948989d6fb842246593177f671`  
		Last Modified: Fri, 28 Jul 2023 01:37:45 GMT  
		Size: 23.9 MB (23865537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:dd603885105b996b2f2ac71bdbc6418f425ef338b8ccd9a0f89d91b542e774a8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.5 MB (79495428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18a1a539a3d7557346dd1bc8a2d6ee409a1be725c2e2443794e3c9a9de8a62ab`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 01:11:08 GMT
ADD file:34567402b37eab48970f90189fd56c47e39acba6d260f0587409ca36a8d36458 in / 
# Wed, 16 Aug 2023 01:11:10 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:49:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c0db36c7b4f2702f9e0075ee892fe4761e0f37f5cc9d73192725313c01591737`  
		Last Modified: Wed, 16 Aug 2023 01:18:29 GMT  
		Size: 53.6 MB (53551877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08327233d2cd5240264b2d14e300da4220731205ebdb79a082288235d814fe5f`  
		Last Modified: Wed, 16 Aug 2023 02:13:00 GMT  
		Size: 25.9 MB (25943551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:463277650cb87ff963c4f3e246c78101c2bf595bfdcfda04fb4db350e9dc1592
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69007846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a46d4dea6048745e0f58711f73e97cfebd76971edb90fbbf0cf7dc14a24ec144`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:09:51 GMT
ADD file:fdcff160dcad587bb28b0cba721c24193be4ab5de90a2d503cba3d329b78797b in / 
# Thu, 27 Jul 2023 23:09:54 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:32:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f8b93f818da821e670e126126d6da395bdf2888315b8baa1a6912378c2f4e02c`  
		Last Modified: Thu, 27 Jul 2023 23:12:55 GMT  
		Size: 45.7 MB (45656956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdc8d46a9f89f9d06db33ee07cddd8aa1a54e242cd6463179064bb8e0711848`  
		Last Modified: Thu, 27 Jul 2023 23:45:49 GMT  
		Size: 23.4 MB (23350890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:5df31820934ef52dc9dc24dd1fcdb4b91a3fe8bf2ad43a7f4804416b0d88d208
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.1 MB (73050169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e8ca8ec8e68c1439425282cb5c2b9588e08b3dfb887b123af12009d46531388`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:43:50 GMT
ADD file:a27e7d7c954291d644437a8054f06f492700f1ce13d3a9e2c3bbd71afd0869cf in / 
# Tue, 15 Aug 2023 23:43:56 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 04:24:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:db9f34e47daed3854a411cee94f611a7139b82002ae54802c9a44d3faccaaea7`  
		Last Modified: Tue, 15 Aug 2023 23:49:01 GMT  
		Size: 48.6 MB (48594395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2492f56fd0a0d7311e408655d1a40ad1f5ce8d34da47a127ae2f85baf9cdfd9b`  
		Last Modified: Wed, 16 Aug 2023 04:37:57 GMT  
		Size: 24.5 MB (24455774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
