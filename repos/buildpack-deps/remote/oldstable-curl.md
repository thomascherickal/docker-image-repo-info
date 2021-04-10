## `buildpack-deps:oldstable-curl`

```console
$ docker pull buildpack-deps@sha256:85b3a60f6c6d765943e2f0503e1e131c767070a2575094a06837b836258ba65e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:oldstable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:88832576c1a9348c193649e23540a48fa2501ee36e33156192c2906632d781f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.0 MB (61008868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b560f62fab6d0899138570386d4ad5d60c28cff6341f5f6671d457079be50c12`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 01:21:41 GMT
ADD file:e3d37689e896a83d39040f2c95091ff88f3899b5b410dbf76908dd6c938b8cb5 in / 
# Sat, 10 Apr 2021 01:21:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:57:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:57:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:76b8ef87096fa726adbe8f073ef69bb5664bac19474c5cce4dd69e08a234903b`  
		Last Modified: Sat, 10 Apr 2021 01:27:52 GMT  
		Size: 45.4 MB (45380037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2bafe8a0f40509cc10249087268e66a662e437f10e9598a09abb5687038a57`  
		Last Modified: Sat, 10 Apr 2021 02:04:34 GMT  
		Size: 11.3 MB (11286411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53ce1fd2746e8d2037f1b0b91ddea0cc7411eb3e5949fe10c0320aca8f7392b`  
		Last Modified: Sat, 10 Apr 2021 02:04:33 GMT  
		Size: 4.3 MB (4342420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:8cd6f7b31220e115788095d9b8c6b69317b5c027883857b727ad83840a9be91d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.6 MB (58587500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f70b36b082fd49ca0b9611792b5b7c6c2596458f5c1ee721f45f58eb6cedb25`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 00:54:22 GMT
ADD file:2fde330dbb713eea654f455b487331e4137626ec1c35ae3aa85c3f491f38e06b in / 
# Sat, 10 Apr 2021 00:54:25 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:12:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 02:12:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:af7c3baa863c80017202aecc5f5cd17980d74282a48ecafa299d3fb5746ca972`  
		Last Modified: Sat, 10 Apr 2021 01:01:51 GMT  
		Size: 44.1 MB (44091992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab52e2e4b39d3057f42ae9ee5b81feee8bc424cd73a1ec2920c5574bad020c6d`  
		Last Modified: Sat, 10 Apr 2021 02:22:08 GMT  
		Size: 10.3 MB (10333980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce3eb302410c6011819ea89cc8eac0368b0645e7908614accf7ab4cb711e3a0b`  
		Last Modified: Sat, 10 Apr 2021 02:22:07 GMT  
		Size: 4.2 MB (4161528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:6ef455cfc00ef176dea754b9f9563542aa0816edb18e59af817ed192fdb2bc84
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (55981186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1e6afeade22b6731d4449ede5c7a260dd3ad5d617854df0b74cb622b7d66c1b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 23:11:31 GMT
ADD file:65b5cf73b0b90f1f459a64d5706f2420deed7cdc5a9e13abacf5bcb05cc3138d in / 
# Tue, 30 Mar 2021 23:11:34 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 01:29:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 01:29:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:80ad3ae4821828f32ce9b3e0f76c3c8f157a7f111e64ffad3ba40287904dfc63`  
		Last Modified: Tue, 30 Mar 2021 23:18:47 GMT  
		Size: 42.1 MB (42120250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24b448d9cdc0300784b14c4a254300d86c316aca568d8b068cdc585ff456ccca`  
		Last Modified: Wed, 31 Mar 2021 01:39:43 GMT  
		Size: 9.9 MB (9939722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3845e857248fe8de10609204e4eb4db8efcbb33c6a2f9e10b7d3efe4c3c625be`  
		Last Modified: Wed, 31 Mar 2021 01:39:41 GMT  
		Size: 3.9 MB (3921214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:621bad28212c16f5ef043202b91f020eabca148f0e2fd366e454122f2e1021cf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.5 MB (57475374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75fed89e5d69c6d5e398d55a55dfe9ed3abc75a5d117f1b39c7bfee3080d674c`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 00:43:48 GMT
ADD file:64990d14743657dbcbe885739e43ac964a0239a63e4693e6401b0884ab96e09b in / 
# Sat, 10 Apr 2021 00:43:50 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:53:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:53:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:30bd672115ff6f225cb98d2d7f1ed62feb72c2612297b2ac615e762e436c64ec`  
		Last Modified: Sat, 10 Apr 2021 00:49:51 GMT  
		Size: 43.2 MB (43177772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7d38e5813e5a59ee1d86fb1c7c8c344342d0ec418aa440509260354958f9ad`  
		Last Modified: Sat, 10 Apr 2021 02:03:48 GMT  
		Size: 10.2 MB (10200972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8ce7d8aff50ac8c0f7baa508791ea69df0fa3c7dac0ab9be8933ce3ef5b68a`  
		Last Modified: Sat, 10 Apr 2021 02:03:46 GMT  
		Size: 4.1 MB (4096630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:a5faea88d3a31bb9029e78d51932b4624ebdcebfe4fee38e92465de8ec17d03a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (62000145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f0118e3706e26bcab4d4ebaeedf970657b5a5d251a0486e59e133c4e3eafa90`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:41:30 GMT
ADD file:1df7a35a36c49061902cf634a894b34a55a9c020976547cf6d2dda96879854bc in / 
# Tue, 30 Mar 2021 21:41:30 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:01:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:01:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:667bc6614d317ea77075a4e2f4ee7ef7d7b696f50d426cec38048d3ca20f1aa1`  
		Last Modified: Tue, 30 Mar 2021 21:49:28 GMT  
		Size: 46.1 MB (46098556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51d5e0a8886ebed26c676639259bf05d50ff3b0285ea4b8afd1492ea424e7ff`  
		Last Modified: Wed, 31 Mar 2021 00:11:48 GMT  
		Size: 11.3 MB (11336592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76cd0bba69d5c567fef7e770351f3ae71bdff83884b1d5af86d4dcd6ea6ff7a9`  
		Last Modified: Wed, 31 Mar 2021 00:11:48 GMT  
		Size: 4.6 MB (4564997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
