## `buildpack-deps:oldstable-scm`

```console
$ docker pull buildpack-deps@sha256:a793417291dc1bc7d745e55b39cc5ca06337d15f6d243abd2e41498b21f568cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:oldstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:45516fe8f853bf2eb1eb4a3a7290b246052ef8a8bfdf17173d2e8f4599abb435
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.2 MB (120179034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aad5b762119c7e8363a9c14c69c4188e26381be23b7d7b40e024984597e3f688`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:54 GMT
ADD file:4bf66d4081da52e8b692fcff96aad84d3e68bda4f62e870e8f4803153c70e24c in / 
# Wed, 11 Jan 2023 02:34:55 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:05:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 03:05:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 Jan 2023 03:06:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ac7f2e1c758675427623d0da4faa88b336c62466c15a98af61efd3f015282f2f`  
		Last Modified: Wed, 11 Jan 2023 02:39:26 GMT  
		Size: 50.4 MB (50448910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbcdf7fce05b60278ea57279b4fd04f78778f80a6d64b6f875afc4bde32c2d1b`  
		Last Modified: Wed, 11 Jan 2023 03:13:10 GMT  
		Size: 7.9 MB (7859410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed0c2752d8478245519a7aab5e660053796af3c7ea7b34ad3df855b33ff5502`  
		Last Modified: Wed, 11 Jan 2023 03:13:09 GMT  
		Size: 10.0 MB (10001385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf01cd4ea334ab5c64bed24016c153dc7c276f552f468e564664e739dac31e09`  
		Last Modified: Wed, 11 Jan 2023 03:13:25 GMT  
		Size: 51.9 MB (51869329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:4f2e84a1bed00ac0607140ce62ac18f7240847a140d130e5fc9ef260dc2b9dcd
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109809727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3778c99214c8c8ad162e26946572eeb20d495aab35c533a3c94792e6733f3cc6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:58:37 GMT
ADD file:aeeb7c51d456bb161dca543eacf9cf356a7b5ab0505401ec5a04b590a09353eb in / 
# Wed, 21 Dec 2022 01:58:38 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:29:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:29:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 21 Dec 2022 02:29:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c6063743b06c86630fb56f8ff5fab94f69ee547fb713805d49d9a99ed6ed8b52`  
		Last Modified: Wed, 21 Dec 2022 02:05:34 GMT  
		Size: 45.9 MB (45915614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759517224594ae5ac12414b070002578f41404acf8f575343f0c567f65000c77`  
		Last Modified: Wed, 21 Dec 2022 02:39:20 GMT  
		Size: 7.1 MB (7147847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c5260ca8282e3cc7c3555d566866b390494e7bd2a7d9f221d67bc0e59a796c9`  
		Last Modified: Wed, 21 Dec 2022 02:39:21 GMT  
		Size: 9.3 MB (9348911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10232c2fbb3336070671d9a9a9ba6bde9af810a535d5358d6b00aa5f6acd69e4`  
		Last Modified: Wed, 21 Dec 2022 02:39:40 GMT  
		Size: 47.4 MB (47397355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:418510093979147d8c5e47c4e34f78abe24bc1c898ef6dce8d6e26577f93e91c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.2 MB (119155580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ea0cf1a740ba289e8420918bfc2af03c79460e0b087d046e53c5c62e8bc8e2c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:54 GMT
ADD file:2129940567ffc1f6fc724b59b8ab1f337db54cd9164e50494822bcedd46d85c7 in / 
# Wed, 21 Dec 2022 01:39:55 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:07:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:07:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 21 Dec 2022 02:07:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ebd367421c805cd84d245a61615aeaa29bb9c2fdbdb111a373ee13b9934d9cf9`  
		Last Modified: Wed, 21 Dec 2022 01:43:31 GMT  
		Size: 49.2 MB (49233817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2a650584f22c4b0b1ceb1f2afaa0462e3ae41ecb07c7cb82d338e99fc3a9e5`  
		Last Modified: Wed, 21 Dec 2022 02:13:37 GMT  
		Size: 7.7 MB (7727254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4859d8b8d8b84e5f11d435628f9c17fbbf42bab8f1e960e9142d545c44a21c`  
		Last Modified: Wed, 21 Dec 2022 02:13:37 GMT  
		Size: 10.0 MB (10003411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9601af78fc4fcd830dac782c2beaea046f8ff4f93fe94827fc2b7d4c3f7c07c9`  
		Last Modified: Wed, 21 Dec 2022 02:13:52 GMT  
		Size: 52.2 MB (52191098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:63f1d19797c51f0c11b49086eac62f45b0c3a16b0d1b0f605b649932e316505d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.8 MB (122834074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b073a416ae8302fef9eb120690e80ef578bd6cda9591633e1b81a3249f6e440`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:32 GMT
ADD file:761d50db794e5887a7dd528cff032401788413ed374043f8995fb4370f61a175 in / 
# Wed, 21 Dec 2022 01:39:32 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 09:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 09:54:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 21 Dec 2022 09:54:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e8258458fa95364a2e7bf12aba19bd9fab7ebbb3144d9ff63b54fe3bdb605cc5`  
		Last Modified: Wed, 21 Dec 2022 01:45:08 GMT  
		Size: 51.2 MB (51207743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00a8f013f9cd8ac22f5327c59808641022657a0cac2bdb1c3eb73b487c77a33`  
		Last Modified: Wed, 21 Dec 2022 10:01:30 GMT  
		Size: 8.0 MB (8026073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5069b3ddc6d943d5145605f59b1624a8f00ee9deac834aea81d071c2cd6a16e`  
		Last Modified: Wed, 21 Dec 2022 10:01:30 GMT  
		Size: 10.1 MB (10127974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e12615e464affd32d36088dfafa685d0ceeef3ec6a1d077f00765fbf68bf4a`  
		Last Modified: Wed, 21 Dec 2022 10:01:48 GMT  
		Size: 53.5 MB (53472284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
