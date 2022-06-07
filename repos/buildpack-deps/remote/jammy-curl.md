## `buildpack-deps:jammy-curl`

```console
$ docker pull buildpack-deps@sha256:2b8e0918d329ed826427a253e69fa9627eb51b179be8367ff509a28ca2b785b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:jammy-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:6cffff22d396dd078e5e2cd628ccf844eb73626ec518a80adf4230fb6bb8032f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.8 MB (37803023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a6bccdca61edd1e8afbd8ba332375b4a1c0e9af494e990e9af6c8449b09eb52`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:25 GMT
ADD file:11157b07dde10107f3f6f2b892c869ea83868475d5825167b5f466a7e410eb05 in / 
# Mon, 06 Jun 2022 22:21:26 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 02:16:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 02:16:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:405f018f9d1d0f351c196b841a7c7f226fb8ea448acd6339a9ed8741600275a2`  
		Last Modified: Wed, 01 Jun 2022 03:03:39 GMT  
		Size: 30.4 MB (30423715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bca3245ce06c5f92cf1528db00b152cdde37af4bf05c5d3976141dc4a704c5`  
		Last Modified: Tue, 07 Jun 2022 02:27:12 GMT  
		Size: 3.8 MB (3819557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7cdee01903ed192b91b97760507cc18ed88be4ff61e33e87bfe6f1944605c9`  
		Last Modified: Tue, 07 Jun 2022 02:27:11 GMT  
		Size: 3.6 MB (3559751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:45ae32633fbb689a2adad29576a5a76965ae33cf811d480d33104ad0064eee93
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34298095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6e5a0b82d9c009ece64a5bc9c8c2ab61adca25a238af980eedc27ba40479940`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:59:30 GMT
ADD file:78ae02cb00d8cc788584388eeb9fdc5ca6b45f502d33acd7f6efe7fc2a325683 in / 
# Fri, 29 Apr 2022 22:59:31 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:35:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:35:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5a3411c136d8a6da4e9d7d3abcbfc94f59ecb2935fd02cad49be6a79c899fcaa`  
		Last Modified: Fri, 29 Apr 2022 23:03:59 GMT  
		Size: 27.0 MB (27015834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0fc400254e500236c1a1555f53101f3d136a6466afc02b601d41b663424039`  
		Last Modified: Fri, 29 Apr 2022 23:53:01 GMT  
		Size: 3.6 MB (3569862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aff75e9c518264298a148cc4e8d868ef1588d3fbb3eb5a8f37dbc41d393fb89`  
		Last Modified: Fri, 29 Apr 2022 23:52:59 GMT  
		Size: 3.7 MB (3712399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:95db445f475f3173a67abf9811cd9764f751b8224e99a086c58183a3d5966f66
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 MB (35488221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8101e90791030ea25bf83059013936b4e020b721a1784971e2790b078c9d435`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:52 GMT
ADD file:1e18e22e32f06a7e93275cf3a2eb2a1d3892be27628bdae2de4b2aadb992bd50 in / 
# Fri, 29 Apr 2022 22:49:53 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:19:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:19:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b84950154c181a602d2e93b68e84660f96dc78f94ae36f3df2db8d5701abb6a5`  
		Last Modified: Fri, 29 Apr 2022 22:52:07 GMT  
		Size: 28.4 MB (28376457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4779269ba0c40d25a7dc0dce21c857eb6326260eef418a05d8f7ebca0f0b7c52`  
		Last Modified: Fri, 29 Apr 2022 23:27:13 GMT  
		Size: 3.8 MB (3792535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc5ea7b81dce7b5d5da0ca011f59cd030d00e4c8bdb15aa0451b41aa695a056`  
		Last Modified: Fri, 29 Apr 2022 23:27:13 GMT  
		Size: 3.3 MB (3319229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:240a9e093c82dd630ca98d8e0e8a7646b322e7b0a33b61ea443b1124cda66bb1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35137335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce6f92023f6b88597b197da1cf2abf8a3d385f9e41d47710470e02f9e627420b`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 18:18:50 GMT
ADD file:d19287898059e2e99fffa362a449097aaffb132af21a1d1e72c5b898ff785df6 in / 
# Mon, 06 Jun 2022 18:18:51 GMT
CMD ["bash"]
# Mon, 06 Jun 2022 19:31:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jun 2022 19:32:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1edfbf9ed16b67ab57bd93f6b8aa57ec157383c958bd3e39e94cdac02ca1db32`  
		Last Modified: Mon, 06 Jun 2022 18:41:31 GMT  
		Size: 27.7 MB (27745919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0b2b247adbcda207142d115c60814f361a65d9e79b584f05cf2c7ae16de140`  
		Last Modified: Mon, 06 Jun 2022 20:28:14 GMT  
		Size: 3.6 MB (3614448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e32164a9b5dee9bb43c693f8c7c833ebe435e4b86660f7a14ce30decd26898`  
		Last Modified: Mon, 06 Jun 2022 20:28:12 GMT  
		Size: 3.8 MB (3776968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:36a90e851554607cf3909c58eeb59b3b682382acf4508404e2326f9ec2231850
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35928918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bd65b257285e8de8dd5b5fb1a71d7fb1994aed78b3135dc33656b8b398e21e5`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:31 GMT
ADD file:f64deb7af5cd28d502c52ddec5392a74b3a97eec2157bb03a4c0422eafb13c49 in / 
# Fri, 29 Apr 2022 22:50:33 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:14:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:14:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8346d310386430a355c4f3bd23e20115298043169165d7b84d92e3233b6696f4`  
		Last Modified: Fri, 29 Apr 2022 22:52:24 GMT  
		Size: 28.6 MB (28637232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0e3da9a8d3319d0121a79a6e6c433b298c51996b294808f5718b06ec206c38f`  
		Last Modified: Fri, 29 Apr 2022 23:21:08 GMT  
		Size: 3.8 MB (3821153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bad36c963048b206a25d408e23b027027eda701e952c4b1495d5eb264b7916b5`  
		Last Modified: Fri, 29 Apr 2022 23:21:08 GMT  
		Size: 3.5 MB (3470533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
