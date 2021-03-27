## `buildpack-deps:bullseye-curl`

```console
$ docker pull buildpack-deps@sha256:6ab39119b832e9de107d615b1524342811f334a8a9e23e40d1fa91f10c3d1a5a
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

### `buildpack-deps:bullseye-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:c6b95c52a994439111d0afa2cddbbbd303fbe3e5be2b97dcc477254f4370e3c5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.8 MB (70832808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f8ba2808da8d64523b144337a787ca964f02f15a6021842c85379907140977a`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 Mar 2021 02:20:04 GMT
ADD file:a858c472d72a55a1ed0b7b2fd2751bac78f77e3549a7533c508022aef7204233 in / 
# Fri, 12 Mar 2021 02:20:04 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:47:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:48:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:da21a291c553cde4f403910fa28fb69cad95f63ce1b378f341eb17738b45a6ac`  
		Last Modified: Fri, 12 Mar 2021 02:24:58 GMT  
		Size: 54.8 MB (54835833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f47dd55341835080544d848892987ce23838db35fe64a0d4338b1494ad6ed1c`  
		Last Modified: Fri, 12 Mar 2021 03:17:40 GMT  
		Size: 5.1 MB (5136253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb0644d825d57df2b92d247999a507695a22522c5fa2bd93de229b003ea515b`  
		Last Modified: Fri, 12 Mar 2021 03:17:40 GMT  
		Size: 10.9 MB (10860722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:1a4fb903bea0b87d5e0ab3a617e1d0aa88d5662547f0477f0c4a8816fbb4ea79
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.0 MB (68034433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:679c47a7a740c66561780e04b2540a37e057d4ecbd4a53c9fd907883a78ce25d`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 07:50:33 GMT
ADD file:1b779b19b47bb1848292d2bf671b599eb9041626b747d8016817e0c7d46ff881 in / 
# Fri, 26 Mar 2021 07:50:38 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 09:04:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 09:05:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d8d862331f8860c127d174052922618c93a166777e5b776e8b08e87702af28cd`  
		Last Modified: Fri, 26 Mar 2021 07:59:08 GMT  
		Size: 52.4 MB (52404525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc6864d5c0a91a133802b130cddb5c9fb77329c250e4f5d77c05e96188cbcb31`  
		Last Modified: Fri, 26 Mar 2021 09:25:47 GMT  
		Size: 5.1 MB (5060013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a0cf03c5e0e5a428fa3a5789c4793210e762dbfb24e1f688a878754fe9ada6`  
		Last Modified: Fri, 26 Mar 2021 09:25:48 GMT  
		Size: 10.6 MB (10569895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:b32eefcfcf8c2ab9a9f795d13c1df92c7d83db7e5f11e96e72157990f2a5cdb4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65212234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a228ac2c3d7ab2ad2ca9cae3cffc504a7738dbf4505065d7121beabc5fa51ef`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 11:15:27 GMT
ADD file:e3651409d9338da981cd9fbd8d9b8511edbde0700ac9e0df8937b859e004990d in / 
# Fri, 26 Mar 2021 11:15:29 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 13:16:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 13:16:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:dd9021b04def024e25507cdd1b0967a20a384ad5cc255120cfb8c5f43495fa74`  
		Last Modified: Fri, 26 Mar 2021 11:26:11 GMT  
		Size: 50.1 MB (50073977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c6023b28762fcb2cca84dd988c0545da69e2cb9cea40e5fb1a14dce3d7d186`  
		Last Modified: Fri, 26 Mar 2021 13:48:58 GMT  
		Size: 4.9 MB (4920097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94408c405dc2689a60515a2dee289cb3495f53f4b4f9758de6995e07aa073eb2`  
		Last Modified: Fri, 26 Mar 2021 13:48:59 GMT  
		Size: 10.2 MB (10218160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:0545668137471868fb0c84a832e95bca9df08265eabeeff04ded48f46490925c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69507023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aeb18a84f643d415851e8619e56a55a2040dbf7c54e4c1a6c204b89fd652c3fb`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 Mar 2021 01:52:22 GMT
ADD file:0b6f3c6d396337f2754d539814c02240e0a459436f4c0992dabf1736069b5a51 in / 
# Fri, 12 Mar 2021 01:52:29 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:26:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:26:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6c214bbe001dfa953738440417693c3487f97b371a108bdd62425a704347faf8`  
		Last Modified: Fri, 12 Mar 2021 02:00:33 GMT  
		Size: 53.5 MB (53521132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1332f0d3a2e68785b75d30a2f0eeb7e0902ecf1068899b78d4a7e90f5201cf7f`  
		Last Modified: Fri, 12 Mar 2021 02:42:02 GMT  
		Size: 5.1 MB (5125702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70aaac2a7c6ebfc86100e530f2607998a0f8d84b4305495031bbfe789e6e1c2d`  
		Last Modified: Fri, 12 Mar 2021 02:42:03 GMT  
		Size: 10.9 MB (10860189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8d57df410d71b485e58af52f40de276fa6dc7718acee41c8e420ca703cd38aa4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.4 MB (72409276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ae7bc35ca7862e216f116b417f999e9e20fae0fcb829ea33ab97e02e5189d34`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 13:52:22 GMT
ADD file:a351d1298a5051f829e330b747943dba9a67cc050d1f23f62be062f669830e9a in / 
# Fri, 26 Mar 2021 13:52:23 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 22:41:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 22:41:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:fb6fc5804fde9f18c538230f43ec9b5dc9c2466d8fc49f7510911c12de70d991`  
		Last Modified: Fri, 26 Mar 2021 14:00:05 GMT  
		Size: 55.9 MB (55881460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47770a32ee01d7a5a9ea596d431299fafb3e5ec55cda781b4b8ba77139d3b742`  
		Last Modified: Fri, 26 Mar 2021 22:54:02 GMT  
		Size: 5.3 MB (5278994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b619575768f273ceeaf065659966267b58a5378b4b7d52fdcd0648e68b378227`  
		Last Modified: Fri, 26 Mar 2021 22:54:03 GMT  
		Size: 11.2 MB (11248822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:de698f1847e01e3eba656590ac4282c13c28806bbfaa0abe79d2760155b29ab0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69111432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d30eb74f5997a0a43c12b8a353cbdaa29ec547d054d1deb883aecfb825cbfb8`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 08:08:46 GMT
ADD file:7e11d2e31071a03f4f43a78cd6af64c7034e2267c839bee84afd1e3bb9916f3e in / 
# Fri, 26 Mar 2021 08:08:47 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 18:13:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 18:13:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8e3b00636426049a0189d8511a90dd5801df2b5793acbaa564ad20c57c4ff115`  
		Last Modified: Fri, 26 Mar 2021 08:14:22 GMT  
		Size: 53.1 MB (53128793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c11a8343730b68d55c2c17295713c1932bfdeed6cd26ba010cb68214e4f5638`  
		Last Modified: Fri, 26 Mar 2021 18:27:18 GMT  
		Size: 5.1 MB (5112340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503e0f155ade594fd8b18a219ba3f1174ed82e7465c9b852325d8a8a11c870d2`  
		Last Modified: Fri, 26 Mar 2021 18:27:20 GMT  
		Size: 10.9 MB (10870299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:3c0cd9061b483b0ee7e38574a3070efed8495b58ff91f1de84caf983232d5518
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.8 MB (75775545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:427fcd31ca49cb171d7712aa16e7e2eb2ddbe26aeb2e034f19fa3658bd1a7fe6`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 15:12:40 GMT
ADD file:28f7d129aaacc2de6bb78dec104b788d0aa25aaac87e07873668354a5b755268 in / 
# Fri, 26 Mar 2021 15:12:49 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 17:11:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 17:13:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:18ddfb418fe2dc2d92f9b851d0345827010c7b001ef98bb5a8b1730d80e2eace`  
		Last Modified: Fri, 26 Mar 2021 15:20:35 GMT  
		Size: 58.8 MB (58756702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e58f4581a73db06180cd5d10d619dc8b47cdbf57bed71dbf9eb53d28bc4749`  
		Last Modified: Fri, 26 Mar 2021 19:34:46 GMT  
		Size: 5.4 MB (5399177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55e302f47f5e7c563d0f23745e32bd160587a44a206808295a2ca9d29a6b9d67`  
		Last Modified: Fri, 26 Mar 2021 19:34:51 GMT  
		Size: 11.6 MB (11619666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:f31dd6a8eb1636da8062ea97d177520f4bd29e6074ef726d50ac28fa99c87257
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69040485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68edaf35df315ad466d464181874f3d04eef57439b3be2efe1587d5de2452c1b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 10:52:51 GMT
ADD file:6dd7d4b323fd63c8ee8a655a79017b62cdad999e420310b15e9568404d02e856 in / 
# Fri, 26 Mar 2021 10:52:58 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 15:39:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 15:39:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:7fcb7355b5dda69e2044a1c24be0597b43954f9d3183dde70ac38aac25df7adb`  
		Last Modified: Fri, 26 Mar 2021 10:56:55 GMT  
		Size: 53.1 MB (53147819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4483fa86d703794bc974862181191f13737481044629eefcee195f179e335064`  
		Last Modified: Fri, 26 Mar 2021 15:53:59 GMT  
		Size: 5.1 MB (5134107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e227b0ad592b8d4f1e74bc91d5c854ab0a75abf65452545c61ce392a04f489f5`  
		Last Modified: Fri, 26 Mar 2021 15:54:00 GMT  
		Size: 10.8 MB (10758559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
