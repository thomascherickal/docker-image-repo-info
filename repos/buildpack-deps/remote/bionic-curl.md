## `buildpack-deps:bionic-curl`

```console
$ docker pull buildpack-deps@sha256:78a5c19460736d0826ae13f4b766abf2737fd1c73b3356de7cd3da0ffc11ef5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:bionic-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:5d53242a937ee00a3323ef4e7faf6fbc84427a5a66a0581e4cb613b9d83ac099
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 MB (36376278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d8990e61ac993b6bb50cd509110e224244289b417364b5bacb145ff1c496568`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:40:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:41:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b43550a14e1f5842c45eaf5b0043a8aac335974d12b11847980b58fcfd5416`  
		Last Modified: Mon, 26 Jul 2021 22:10:05 GMT  
		Size: 6.6 MB (6644948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e59c30206e4fabc53c96ec7a836fcdc7cdac49cb93fc1b8e376733f4379cfb`  
		Last Modified: Mon, 26 Jul 2021 22:10:04 GMT  
		Size: 3.0 MB (3022291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:8cd88ad50e848014c72124a58f84fbe85a33a7ce5932658c6e730d6dbb59fba9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30606676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18bd33d28415880a949129908f93919248f16bc8d8fe5d4251e57dd8bbd9107e`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:51:31 GMT
ADD file:93478fff12f14732647e59eaafbd2a694de2f3a162fdc6bb1270acc1c69edc5b in / 
# Mon, 26 Jul 2021 22:51:32 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:14:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:14:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d5092371cc59fda70c1ace542259c1514fc023e571d50c900322f2a052531228`  
		Last Modified: Mon, 26 Jul 2021 22:55:43 GMT  
		Size: 22.3 MB (22306852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08ef2837cc6a640557235061b89ed9a389330802f062137cb313376de279870b`  
		Last Modified: Tue, 27 Jul 2021 01:40:03 GMT  
		Size: 5.7 MB (5715357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ec9e4b1e75d299207a4006fe43a2e34c3fda90619c762ebc07dc792b034642`  
		Last Modified: Tue, 27 Jul 2021 01:40:01 GMT  
		Size: 2.6 MB (2584467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:5d962e80ddffea4d545bda177e9840d262fb1893cdac6acc8cc3863bf9de75bf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.6 MB (32601295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d34eb7034c339584e265fb320d1e0d2496baa28988e145f56a72254e7ec081ad`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:36 GMT
ADD file:27e3c8f7785fef80f6172954da7c3c73734c02b933dc19847e888542897d568f in / 
# Tue, 31 Aug 2021 01:40:36 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:08:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:08:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4028d4a2ab035ee99388f4aa429a83fbaf8022de67206e9a5b69615c71069135`  
		Last Modified: Tue, 31 Aug 2021 01:42:16 GMT  
		Size: 23.7 MB (23730599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4a9b8c6709cd3ea323ffea2dcfa72913a9fdc73837573db0ffa663995a44a8`  
		Last Modified: Tue, 31 Aug 2021 02:18:37 GMT  
		Size: 6.1 MB (6087650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08ad199f9143cc4082ab5e445c913e284b9f2ec63abce0b6b1243561e2810a77`  
		Last Modified: Tue, 31 Aug 2021 02:18:36 GMT  
		Size: 2.8 MB (2783046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:77c62e1928a0a02b1eb69d7cda933975816c77ee2ba1e333f2cb8d916bd3bf92
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37349567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37e6101ebd52b5a1c60f03a674e775c8fa0244a300cbadc8c8f42793a4f5e1b6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:39:08 GMT
ADD file:615269b4e3662feffa9257a896456387554777532f070eae2226fa704e50150e in / 
# Tue, 31 Aug 2021 01:39:08 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 01:57:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:57:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:01a6f9651a524383d1aac8b05ceaf7a079d305146c6bf120b7ffb27247b18230`  
		Last Modified: Tue, 31 Aug 2021 01:40:06 GMT  
		Size: 27.2 MB (27162437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2c7d08d74fca5ace99c2318c3f53f795d5cd713e8df0f41ea3c071a3583372`  
		Last Modified: Tue, 31 Aug 2021 02:09:50 GMT  
		Size: 6.9 MB (6934539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a486c005ec2b9b98efae8ad7204dd1b1e216eabe229174d28fb5b62c9489ea0`  
		Last Modified: Tue, 31 Aug 2021 02:09:49 GMT  
		Size: 3.3 MB (3252591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:2d73cdf00577962a4ff175511e9ae4165e9772824f2aaf3bf2fd988eab5e593e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41215068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:232490ed0858a7bf31e6a80f877808b2daea11c077fe994699f1d5db1808aa43`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:31 GMT
ADD file:2e6f05bbffb47b3ea8e5e4127452e80debc89fb9e22af2dc5c735ea579adad64 in / 
# Mon, 26 Jul 2021 23:12:34 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:58:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:58:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3c742a0b2a0025420dcf1bc91d81de2ffb292328fad483ce715521d725503b66`  
		Last Modified: Mon, 26 Jul 2021 23:15:30 GMT  
		Size: 30.4 MB (30437958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475513220a5f30414e690523f753a7a744d3d79b2e0d3cff2d05038e334855a4`  
		Last Modified: Tue, 27 Jul 2021 04:22:10 GMT  
		Size: 7.1 MB (7057571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb47fd0ae4274e4d82eec5939329f2aa19c6aaecea4b7e24ccdf34312d95fa8`  
		Last Modified: Tue, 27 Jul 2021 04:22:10 GMT  
		Size: 3.7 MB (3719539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b1f689b30d2ae3be28a65adc94df539028bd0f5346b14cbeb8e12d90f6cc549b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34677158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:849662eb467d6d767b9ef21110d9f00f5b75c83c278ee84bef70c174b2e1af68`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:06 GMT
ADD file:587feabbf5ad530bb19e438490116110e0c3f5fd5c8b98bcce6767af928c66de in / 
# Tue, 31 Aug 2021 01:42:10 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:34:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:34:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8a5845e3ee3e2d93d3bcf0f827afe41d646f59cdf52f107306c232b60ffeb3a4`  
		Last Modified: Tue, 31 Aug 2021 01:43:59 GMT  
		Size: 25.4 MB (25366401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae5daa9a040b93bff6544ad59a003cd958048bef64a9f991a5d3150888fcbed`  
		Last Modified: Tue, 31 Aug 2021 02:45:10 GMT  
		Size: 6.3 MB (6335758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32bbf8f7d5625c28aa637939c7029792a4f3b624e300c59cb77575fe7aa84d14`  
		Last Modified: Tue, 31 Aug 2021 02:45:12 GMT  
		Size: 3.0 MB (2974999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
