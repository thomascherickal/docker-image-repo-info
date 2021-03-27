## `buildpack-deps:testing-scm`

```console
$ docker pull buildpack-deps@sha256:797d48d3bbd5131ab70a62288f2b6d4e408dc86fa60ce81f0e7c6102c5c5a73c
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

### `buildpack-deps:testing-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:65d8a1ac0e1c061002e2c7eed00c0799413a365714139ca187bba11fa2180700
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.4 MB (125406375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66ee6e1ffd551bbf88e15ed703c9ddd513715334553d0c3b6725e31156f5f0b2`
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
# Fri, 12 Mar 2021 02:48:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:f5bb105cb94d3a12e9d1648ac4750f9b7b3f837fc623dff8a5676d1892f8ea7b`  
		Last Modified: Fri, 12 Mar 2021 03:18:07 GMT  
		Size: 54.6 MB (54573567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:fc0a96c8059bcbfd4bd01013f1f32bc836a7d3467c3d9c7eba0e7d58243121a6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.3 MB (120348805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c0e82882eb21c312386e36a474e5d40af96374a3c21f7f569b6200bfe90f4de`
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
# Fri, 26 Mar 2021 09:06:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:1985045f60a052a5d3b4e89129ae9f03ece21620c4b057aa105c0c78cc5775a4`  
		Last Modified: Fri, 26 Mar 2021 09:26:11 GMT  
		Size: 52.3 MB (52314372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:895671b64d35c1257769edc7bf65f4e503a02b13978c4926c661e67a3e5d5c39
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115540400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8505cf255310b4f659882c40eaec332ff1c19ee9754274a784fc0f5335f2a668`
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
# Fri, 26 Mar 2021 13:17:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:fd339501262a81addad6326243dbcf62ca43943542cc42a3b06aeda9a9cdec3a`  
		Last Modified: Fri, 26 Mar 2021 13:49:44 GMT  
		Size: 50.3 MB (50328166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:2f43be1b7f7838526097954bf1e85f07dc8face799579bf62862ed8fc40834ea
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124182083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f40e52544647ea29296868ea5dea434c3fa58ef30191d2d9b16420daba220823`
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
# Fri, 12 Mar 2021 02:27:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:d2c201b24dcdc8bd225ab1c164d5ff733c78eb97a701f50d2841449244aa6b43`  
		Last Modified: Fri, 12 Mar 2021 02:42:31 GMT  
		Size: 54.7 MB (54675060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:bb2c76a88da737750fa9435b712d5415ccf01422afa5f8e67b0656af86b33ba7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128318140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e0b147919fd794579b106c522201e2605406ebb82c0499d3dc704085641687c`
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
# Fri, 26 Mar 2021 22:41:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:0ce028724865c02e9ace59fe70b5f2ea0c85782a125e91d44e337fc658f84434`  
		Last Modified: Fri, 26 Mar 2021 22:54:36 GMT  
		Size: 55.9 MB (55908864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:47335ed37ad5ad0bb64b948ce0199b99c49e39aad14216ac3a93a4ae1e7833bf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.4 MB (122410906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23601ef8a9b6fa5044ea0336b0a3203ebf67c9467b5102a4462aa0dcca851619`
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
# Fri, 26 Mar 2021 18:15:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:b5514c276e4dbcbce3dce646bff262cc3c13a68791d15a0585f7a759615c558f`  
		Last Modified: Fri, 26 Mar 2021 18:28:10 GMT  
		Size: 53.3 MB (53299474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:3acbefea54b6c3865dbb6a60514a49df919d0a76d0d7e6ccd01f31a1b5f14fa4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.6 MB (134622038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa9954ed350f1f32e08d008065ac376d26457d9fdd95be10fce4215ea7cc9340`
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
# Fri, 26 Mar 2021 17:15:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:da9f221c0a34707baac4ad94f19a4bd62b803303c74a200e7d8ced228745c108`  
		Last Modified: Fri, 26 Mar 2021 19:36:24 GMT  
		Size: 58.8 MB (58846493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:033377fc76ad18a8c8eda2ed3d7f527a21f542882f779fca5bc76cfb9352d85f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123079434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59f2c005e666e9ae589b4fda2ab2a6bc4db7c967be34f58bf63c919e90103662`
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
# Fri, 26 Mar 2021 15:40:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:e907d7501cb26d3573f807160ae0b0b98d3c254793f034d9f3356af99600645d`  
		Last Modified: Fri, 26 Mar 2021 15:54:24 GMT  
		Size: 54.0 MB (54038949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
