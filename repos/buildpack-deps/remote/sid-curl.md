## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:6e5380abc33a4c38fe2ec9a3502a17e6088eccb6a89c1982db71cd4f0a94d430
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:sid-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:e4ef34e95279a9a43c854e672a84ad5fe8c1cc1baadefe0b48ad9a7018507f30
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.5 MB (71463529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2367076b207da22edeef16880deb9a7c0a69cac4882de607c1d09f6d04a940bd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 02:22:23 GMT
ADD file:66b4753e4d225919cb5470c007009d4dbea725cab1d3ad1cd3c0ac3b35192aa5 in / 
# Tue, 09 Feb 2021 02:22:23 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:37:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:37:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e9e6a013db8a50441790405f039006e736170b55104d06c80015cacba6d5b0f4`  
		Last Modified: Tue, 09 Feb 2021 02:28:28 GMT  
		Size: 54.8 MB (54793268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:082f6b01c7a4634e4f6d0de548009681557bbaedac26abf3e20b536a7b5e5923`  
		Last Modified: Tue, 09 Feb 2021 04:47:21 GMT  
		Size: 5.1 MB (5144121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b4f1dd261e5a91095fe68ed97b0d837c7dd575a8940fc745f7be6b907a906dd`  
		Last Modified: Tue, 09 Feb 2021 04:47:22 GMT  
		Size: 11.5 MB (11526140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:6d45a8d5cdbca349dfaba945341c99017175a8475fbbd0c1c984d2bae1938d6b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.6 MB (68593044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cb9d6f862cb2e73fe6f4e74bba8eb7bc977ac1139bad31347cd22e916d6ab62`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 02:53:02 GMT
ADD file:8a666bde5248b085708640c42b93c850be2265e6a4db5b59c48543ddc8ad0148 in / 
# Tue, 09 Feb 2021 02:53:03 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 03:29:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 03:30:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3b915a09886212577bb3e4444d6bdc576b17746fa48c0239c56c968d81127e7e`  
		Last Modified: Tue, 09 Feb 2021 03:01:34 GMT  
		Size: 52.3 MB (52324134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c594f7d69077392315310232b92354eaa9652361ef5e54825e4aade3a67e2851`  
		Last Modified: Tue, 09 Feb 2021 03:41:51 GMT  
		Size: 5.1 MB (5053985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195684c55108e3d23d6b03082fa8140c8859a738918fed4410211cbac9dd2ee6`  
		Last Modified: Tue, 09 Feb 2021 03:41:52 GMT  
		Size: 11.2 MB (11214925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1751a3a824d3bca3ce7c5c2f77d72e31c7ea8f37460146e7edded57734313dd5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.7 MB (65733213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:029811483a7d2abd2a3534400d8d61cd9bad1d990533f8e2f132df5d9168aaa1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 03:03:31 GMT
ADD file:37f3b4ac2683802bd4615102851fc9dcbc409a3964e047866697c24a568fc90f in / 
# Tue, 09 Feb 2021 03:03:34 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:29:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:29:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b8fd51bd157e6a71bf72bc04c009bb65c4766fc14c9fa5e95c0bf36f393f7ab4`  
		Last Modified: Tue, 09 Feb 2021 03:12:11 GMT  
		Size: 50.0 MB (49982731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d61fff78cf158b64e5f26e7f3c7e3d2e7eeb167059b0e914b1d2626b5c9f1e2`  
		Last Modified: Tue, 09 Feb 2021 04:41:09 GMT  
		Size: 4.9 MB (4914542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5d61b00c2332b32afcd6a8b313f6eee25aac2d20a654993899c9bad1c8191f`  
		Last Modified: Tue, 09 Feb 2021 04:41:10 GMT  
		Size: 10.8 MB (10835940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:dff65dfcc721de1269bee9ad891ebcc6424db9495c0dae2e8c61829d80894b9e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.1 MB (70131865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2627389da93aadf0713f61c3af91a2e7e7f14fc52eaf9f97c727f8749c92dd8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 02:42:06 GMT
ADD file:988aaab917b0b86b69a5ec0bc1b562df25e15f11cbd3997c0eb79c065697d66b in / 
# Tue, 09 Feb 2021 02:42:10 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:46:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:47:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:16d849c3d9b47a494d04ea09283a62946c42f5ebec529d6b0f5c094929bc8e48`  
		Last Modified: Tue, 09 Feb 2021 02:48:27 GMT  
		Size: 53.5 MB (53467842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1a97402a658df9ec658bfe4c46ed0b39e10960a7656f1762b77630edbff325`  
		Last Modified: Tue, 09 Feb 2021 04:58:49 GMT  
		Size: 5.1 MB (5132244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d6b3647e20b39d65d6536d94dd338a68c8214241b59de7f6643aff0bd2a98e`  
		Last Modified: Tue, 09 Feb 2021 04:58:50 GMT  
		Size: 11.5 MB (11531779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:b3507e770ef2f7adac057d8e9896b7fe24b80960aef211a88e1873f52c4bc501
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (72995746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6d5119fcbb7587355532e25debea3367aec6b0382da887f4325f0cedf0a531a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 02:41:17 GMT
ADD file:d3470c47b61c2df201e9fe51e9dd198c152bae2eba84df9bbfcb591bfb29502a in / 
# Tue, 09 Feb 2021 02:41:18 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 03:12:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 03:12:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:14213d5e86eb4e1e7c43e3524429378786d8674960445945ce050c587b83884f`  
		Last Modified: Tue, 09 Feb 2021 02:48:13 GMT  
		Size: 55.8 MB (55792012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2cbabcd8ca39fd619ad8a109f0fe5eea442c6afefd108f3d2a80a49be04524`  
		Last Modified: Tue, 09 Feb 2021 03:22:39 GMT  
		Size: 5.3 MB (5271392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36cacdc0d9d1ac9a69c2a336a43253fbfd3737321bf5e32c6f9ee54465cb2087`  
		Last Modified: Tue, 09 Feb 2021 03:22:40 GMT  
		Size: 11.9 MB (11932342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:d572804532a99622de3788fea709664ba4f1fe29b17777aee1c625354308ae54
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68798549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba88cdd626a29f710372ee14b7a2296ba73b93e1a797d3126bd069a83af6086c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 03:09:52 GMT
ADD file:1bed7e8245b9fdc9b6216dfe7c7a97a236870647ca9e7641f98c8b2f5f165612 in / 
# Tue, 09 Feb 2021 03:09:53 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:09:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:09:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d37dfb54bbee12f1ddd54773820dc4abe1d8525601798200ea891af443d2dcdd`  
		Last Modified: Tue, 09 Feb 2021 03:16:42 GMT  
		Size: 53.0 MB (53038778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c585817c61fcb4aec261a19daa3690feb2d437834958b786381a615e14144fcd`  
		Last Modified: Tue, 09 Feb 2021 04:19:59 GMT  
		Size: 5.1 MB (5107065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:340d3cf0ba9b4e31b7d87e5818d6489e6e7ad7ad78a8a6c448eb31c1288899fc`  
		Last Modified: Tue, 09 Feb 2021 04:20:02 GMT  
		Size: 10.7 MB (10652706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:da824faabb1cf2483f9dbad980dddf2f52929401bd4acbec3c9d00f8ba02bbf7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.9 MB (77871932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:601396709b1c2887e79a72d7aae4ba82e979288ce9e936a41faffeda3a37170f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:25:40 GMT
ADD file:f289d6dea557bc0563fd9221c4857a56c56bb52d981a3ec90ade2f1b76980794 in / 
# Tue, 12 Jan 2021 00:25:56 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 02:21:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 02:22:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:594e638823d3ce0bbedac4d1aebea00f91d28a98d7b98ca680fd90e4c0fc8850`  
		Last Modified: Tue, 12 Jan 2021 00:34:46 GMT  
		Size: 61.0 MB (61048727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3a59148553af7496dfbc29a5704e94338ac15ab898a646dcbab32076a5f00f3`  
		Last Modified: Tue, 12 Jan 2021 02:40:41 GMT  
		Size: 5.4 MB (5400394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45a065f7b5587bec16714bce093a4075fb92b291238fee1bae7d383a16a4052`  
		Last Modified: Tue, 12 Jan 2021 02:40:42 GMT  
		Size: 11.4 MB (11422811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:0d24a64d963e5352a86f397b79f562b3ccea65c3594411b624cc74950e40fda9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69600752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8abf3a26f1a0f83cea68fb1550140f314d137be137829cb4da272f1d8bfaa087`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 02:42:21 GMT
ADD file:6b632451421e7f0411db1927a48466a6b3bc2f7e10a53b00a06799fbec279bdd in / 
# Tue, 09 Feb 2021 02:42:24 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 03:07:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 03:07:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3dd2606d37926391a1e8153ffefee2aaccae04bd432c37c97187880ba3ed01ea`  
		Last Modified: Tue, 09 Feb 2021 02:45:45 GMT  
		Size: 53.1 MB (53060083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dd34d7430306d4b5f56a7983d33fdce7c2f86209989ddeacc68e07134aef96e`  
		Last Modified: Tue, 09 Feb 2021 03:12:40 GMT  
		Size: 5.1 MB (5127742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b9a7cd753b983b2730894814680d1c0b77e08d7affc85900856bd036f96806`  
		Last Modified: Tue, 09 Feb 2021 03:12:41 GMT  
		Size: 11.4 MB (11412927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
