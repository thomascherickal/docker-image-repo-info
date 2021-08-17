## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:0320abbbbc66a5927eac895d51ca27bb4e4574bbd11b6dc258969b8644eb4460
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
$ docker pull buildpack-deps@sha256:02f2a10a3b60bc1dada0e530f00238b5b5fa53b3d005f72cb3ee65aefca5db7d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.0 MB (70952951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b48862eb062e9cda42cf52a979a9e30369b6f2930ec98e7b82b7309c63b1f0f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:46:20 GMT
ADD file:cac9ad9d988141c80929e8c31f4cb388618dac0bbc048d4c5e3b8029c85c576d in / 
# Thu, 22 Jul 2021 00:46:21 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:13:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:13:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:531fc43e70accbfd0e52721b79cfd564769d6f1b7e64a98e9f670327d4c4820e`  
		Last Modified: Thu, 22 Jul 2021 00:51:36 GMT  
		Size: 54.9 MB (54909299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f3334cfec756c2189b8a7cce5cd3ddf363b2acfc7b8a38f1ccf8cdbe4ef115`  
		Last Modified: Thu, 22 Jul 2021 01:21:10 GMT  
		Size: 5.2 MB (5171133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284c0769674315a1486ea9eee2a7dbe2a630850d90b8e445a2b8d7034528be1b`  
		Last Modified: Thu, 22 Jul 2021 01:21:10 GMT  
		Size: 10.9 MB (10872519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:edf5fa9d4767275003022dc627b2afb2d85957ec2ac4eae7e118fce949848181
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68093375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfd2561c5f55824c80adec8586426bc4af358f51ed5307b74b0be821ff1c4be3`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:51:25 GMT
ADD file:7b9b18b6a1a6deb81eb9bf8638d60de26198ba106aaa757dfb838b264fc90252 in / 
# Thu, 22 Jul 2021 00:51:26 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 02:07:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 02:07:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9de879dbb26d0cc624c499f5907a14117d0f357e4e39699d3208c57d5091b537`  
		Last Modified: Thu, 22 Jul 2021 01:04:16 GMT  
		Size: 52.4 MB (52445986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef97169c47ca52a8e66f6ef70d0a4d9e5cfae0f8b72d1937ac646b3bdf48d8a`  
		Last Modified: Thu, 22 Jul 2021 02:24:13 GMT  
		Size: 5.1 MB (5075544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e445910f582e1f6da040a3bdd8886f00fcc077bf63486317b6de7c17cf3ba01`  
		Last Modified: Thu, 22 Jul 2021 02:24:15 GMT  
		Size: 10.6 MB (10571845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:3ce756b0418cb80f7db8b1b6f5dd9ac522caafa228cad80c9b390e248500fff8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65266328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:784bd2504fe75fa53bd427f59a293bede1278ce233f6442e088a961375588261`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 02:05:12 GMT
ADD file:dc3a5129f00ffe49d5f2b5c7472bb0e89235fc02cd3f1cc7d27243e371d4a8e9 in / 
# Thu, 22 Jul 2021 02:05:13 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 04:18:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 04:18:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d81caeed2081307865201ac11c62494bbd309b5efe940cf9cae7a6739c8ca2a0`  
		Last Modified: Thu, 22 Jul 2021 02:18:16 GMT  
		Size: 50.1 MB (50111961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab786a921ccb7c1afe30eca6993da354114a957337287d819030ab934e693711`  
		Last Modified: Thu, 22 Jul 2021 04:38:30 GMT  
		Size: 4.9 MB (4936974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d08ba7697666bbe33ab34e16c74f6a0e1e670f45c2a33f9f3205862bd88c74`  
		Last Modified: Thu, 22 Jul 2021 04:38:31 GMT  
		Size: 10.2 MB (10217393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:95d6d67d8406fecd07f2ca47fb1c181429f99d8aa0fc2ea109f9f7e7ce9e9a1c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.7 MB (69659445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3da9d49ec2b2035e68d98fe9d85208d455692b9c1c6a998f4e214216593a3973`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:47:32 GMT
ADD file:2eb550b4dc61105505c60437af91d7300fc5596834bfce84a75b260663bf4f42 in / 
# Tue, 17 Aug 2021 01:47:32 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:55:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:55:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0c8e1604d5b38112a190afe29ac6b4d1c501651ae9e68b6eaa49788ae64f145d`  
		Last Modified: Tue, 17 Aug 2021 01:56:14 GMT  
		Size: 53.6 MB (53625965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f4b3d12f8e0cac2ab78286575b8f56d2cadedcafd68908cc60821856f5e360`  
		Last Modified: Tue, 17 Aug 2021 08:03:37 GMT  
		Size: 5.2 MB (5160051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb41ce34a000fbba6dafcb340db9d0b7f64a8efd27ff966f77978ddd2c567439`  
		Last Modified: Tue, 17 Aug 2021 08:03:37 GMT  
		Size: 10.9 MB (10873429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:1fff776b370dd15d9693f26b99eb5780cdcdb3bb8e65edd38597f03b4e64d758
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72519728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddda0428d54281258d8a03082810ed4c348538dc58305c7e6a3471f26fe2df0c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:42:42 GMT
ADD file:8d9eb4b2afc4eb0058f4080c5f0eedf0ddef323f1cc5a0403658254d191f117e in / 
# Tue, 17 Aug 2021 01:42:42 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 02:01:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 02:02:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:79e62a40ce7bfbbe436e33c1da1c5661386b9674fe81402fdbfbb42a5b84998b`  
		Last Modified: Tue, 17 Aug 2021 01:52:55 GMT  
		Size: 56.0 MB (55967475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fe3391f9add930caab1f7ad8d326db740aab914960a3522b2baea8f34b06d23`  
		Last Modified: Tue, 17 Aug 2021 02:11:30 GMT  
		Size: 5.3 MB (5301763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5c1c03bbd7c2f8c23dd8b5a8bae89de98d00fe400f6f7c89140aed7a78c6aa7`  
		Last Modified: Tue, 17 Aug 2021 02:11:31 GMT  
		Size: 11.3 MB (11250490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:9574c023c1bd1d12c66b471db94f95c90303711848b34d1757fad4cf185c6a24
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69165997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b353911a5e0986a17337cd29fb8e2c9509b62bfbd1f7a09800bdd6533689a35`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:10:12 GMT
ADD file:21823f99ac9631853baf61992ae48f9aaefd9aa14689bdad76945cbe790d4b23 in / 
# Thu, 22 Jul 2021 00:10:13 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:46:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 00:47:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b7674bbd759fec6741d7d94cfebb5e0cf54c599cb2a824313eb96b1d6622a44b`  
		Last Modified: Thu, 22 Jul 2021 00:16:59 GMT  
		Size: 53.2 MB (53162150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61bbf92e62547174ba9022d0c0fe12fa84126289620f8148cf33269681b8273c`  
		Last Modified: Thu, 22 Jul 2021 00:57:29 GMT  
		Size: 5.1 MB (5130754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2614779dff3229eb62dc8a974d88a9bf60cfd085721871ad71d642e0517eb35`  
		Last Modified: Thu, 22 Jul 2021 00:57:31 GMT  
		Size: 10.9 MB (10873093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:ba100d486ad0576fb0786293c532bde1bad6285f219549e047b3f3e77a94604f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75858815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bfa1fe3c917cffc113af266763354392783eefda7b08b5a25052553e14df5c7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:33 GMT
ADD file:d5172916465206276bfc66e1d963768fd3cda811ba961e86fdbc4b49f0a72dfc in / 
# Thu, 22 Jul 2021 00:19:40 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 04:19:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 04:20:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:bb31d3e4dd3826fb7298bcca3375efce01b08c74be37a5494cb4eaccd247d8e9`  
		Last Modified: Thu, 22 Jul 2021 00:28:17 GMT  
		Size: 58.8 MB (58810717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6ede8e70912b2a939d88a27d547a381f612b6c792d57e726d55e899c3866ec`  
		Last Modified: Thu, 22 Jul 2021 05:18:34 GMT  
		Size: 5.4 MB (5421821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18b90280541d7eb6e7e1d27889a4b6e4dc571eb851a0b49f6da40e06522687e`  
		Last Modified: Thu, 22 Jul 2021 05:18:32 GMT  
		Size: 11.6 MB (11626277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:ea1ea7eb3f215c84403554672c91c22945344400c673d6f1522fd607ee45c612
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.7 MB (65716534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb7bd69c97313ca7d402f43854f393547d6854ae7a3b046c650dadf00adab219`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:45:57 GMT
ADD file:17c3a69ac6b2ac905f0d9d5d8d828215848c91b6aca208c63e3c8c6c3c28ac20 in / 
# Tue, 17 Aug 2021 01:45:59 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 02:28:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 02:29:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:03abe71e39e08cd630ff168b11929dc5c3c5111cfb3d81f5a8183f7ba7162fab`  
		Last Modified: Tue, 17 Aug 2021 02:01:48 GMT  
		Size: 50.4 MB (50437771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1e3ddf2aa723d9dc92fc071b3cc373219cd68de4072a024dc13965f2156705`  
		Last Modified: Tue, 17 Aug 2021 03:07:39 GMT  
		Size: 5.0 MB (4984859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fdbcb287940d650490755774d53a8edf26fba9558538160b4f649b66979ee4d`  
		Last Modified: Tue, 17 Aug 2021 03:07:43 GMT  
		Size: 10.3 MB (10293904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:fab97181f913819d52d80648d12308e39e2b6edf93eed0dd25b6269b1e975638
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69143422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b34924373ab74ba0650cd2931dacfef322ec14458f9202a4078c99c5f43650a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:51:06 GMT
ADD file:ab809bd14c40234cf29151f2485ed39a9fa31f67c202abe6bf8546f5899aa52f in / 
# Tue, 17 Aug 2021 01:51:14 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:37:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:37:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6758b3369d7c595105d273788911a60f3cbd8b26d39dea406c75de4d1da4a084`  
		Last Modified: Tue, 17 Aug 2021 01:59:02 GMT  
		Size: 53.2 MB (53226590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ee5f5767e372ec2c62434ed4325aa1b14846b20d736bdb81e1861163803d98`  
		Last Modified: Tue, 17 Aug 2021 07:45:09 GMT  
		Size: 5.2 MB (5152856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc1daed3fa6142f9fe36fd70a1e631c71aa839f077885d60cb4e7fb21210dacc`  
		Last Modified: Tue, 17 Aug 2021 07:45:10 GMT  
		Size: 10.8 MB (10763976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
