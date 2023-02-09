## `buildpack-deps:testing-scm`

```console
$ docker pull buildpack-deps@sha256:f32d806b6300aa06d48a4fe75303643cb94142765e4cd97f12937758aa5e8df9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
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
$ docker pull buildpack-deps@sha256:c662ffcb44c979007e7fb140b28a4cd74f883737a6089e78435d41a6d4bed227
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.9 MB (133875690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8d10eca82d1261fd1fed8f3543587b363635de612581dee7e1a88d430536f4d`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:50:57 GMT
ADD file:59c477049f0246331c6723687b7f8995e7a8946172b967d10fb8b67146220c33 in / 
# Sat, 04 Feb 2023 06:50:58 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:20:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:20:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Feb 2023 07:20:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:20aeb9ca89f41415a92cd1a5e9ff6c0280e09a250e0f950c9df57d97b0d3efb5`  
		Last Modified: Sat, 04 Feb 2023 06:55:19 GMT  
		Size: 49.0 MB (49043016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd16dee5feec7a2da71bdef1f07b5a546389f1554d69d474530b8f847d0c1890`  
		Last Modified: Sat, 04 Feb 2023 07:28:22 GMT  
		Size: 9.0 MB (9033132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba40466925cfd251e3c9b97a519794ed3580ca83f2135be0ccea17e5b2d6f99`  
		Last Modified: Sat, 04 Feb 2023 07:28:23 GMT  
		Size: 11.4 MB (11354722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e5912b196c98527faa75de1f03b026f5c2740634e4a9498c536214352bbd910`  
		Last Modified: Sat, 04 Feb 2023 07:28:40 GMT  
		Size: 64.4 MB (64444820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:073145d279d4747bb68f077238bad9466d126fb16da99ab317710e93af16da6d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.4 MB (129431086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:569cc62ec33fe806ca3b248021438b8733e8b2594ec7423e87aa221ef56ac1a9`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 01:59:47 GMT
ADD file:e8907ddabcb71a5bb204104a87abac55a5c25cecb9dd58e57df68c8a4f179c2c in / 
# Thu, 09 Feb 2023 01:59:48 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 02:27:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 02:27:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 02:28:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9368d268169994f25b198da907330473abf057d5e3ff164fa3d7c17e9914d5bd`  
		Last Modified: Thu, 09 Feb 2023 02:04:27 GMT  
		Size: 48.0 MB (47988795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:087520a438b3f037351eaf9d5de3f3af21ee452533a5c929c96f44b6cef18eb6`  
		Last Modified: Thu, 09 Feb 2023 02:36:15 GMT  
		Size: 8.5 MB (8481513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b0217a2839f272946e9b327e1bdfd1fa7cd148ab7d8856e88d0f443ed1d22dd`  
		Last Modified: Thu, 09 Feb 2023 02:36:16 GMT  
		Size: 11.0 MB (11001935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bf1b772c721ff6b52047f18260d8e59eef117d7849e8af3f914fbd831307f1`  
		Last Modified: Thu, 09 Feb 2023 02:36:38 GMT  
		Size: 62.0 MB (61958843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:4bbb24bb0ecc806075782f2b5ae821d980aa471190364a6509e20f1f11b40ee3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124184637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1999988a5b1eed26396faa13d55808f3b3436ac68b20774c5995700191feb55`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 09:58:46 GMT
ADD file:7fa388eb21c424f9b3d978f277c454b5cb8a4c4fc0dac864298e9cf12161b132 in / 
# Sat, 04 Feb 2023 09:58:48 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 10:46:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 10:46:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Feb 2023 10:47:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:16b554b0ae696936d2556c56490dc1cb7af234f9a415a93932213ba90d19bd85`  
		Last Modified: Sat, 04 Feb 2023 10:05:12 GMT  
		Size: 45.8 MB (45794144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37939da9cb6c3ba4566c2d20c05dee5ec7361c07649557a19b8e8d844ef0cf4`  
		Last Modified: Sat, 04 Feb 2023 10:57:57 GMT  
		Size: 8.1 MB (8124732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20d72a01582fa10ad6cbabe8e802a8e57b4fb57dd818ac7cf92815d91a6a0a55`  
		Last Modified: Sat, 04 Feb 2023 10:57:57 GMT  
		Size: 10.6 MB (10635854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a385e0a6d4d5d7a96989b13b2566ab1876cc3c1183e9bb336d6f3fbfee7df420`  
		Last Modified: Sat, 04 Feb 2023 10:58:19 GMT  
		Size: 59.6 MB (59629907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f99d3de7d1dade7396b45fa29fee449cf61e16dbc9bce5ebc3c4578f3b86b4b5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.6 MB (133604253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0c449e7578962ab3aa65e6262f0d95cf1a5f467d17f116a9c60be9d4b32e15d`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:08 GMT
ADD file:b40ad920bd7dd081e20adf36435db50381b9998a1de3d2eac6b2c45734ce60b3 in / 
# Sat, 04 Feb 2023 06:17:09 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:43:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 06:43:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Feb 2023 06:43:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a43b5d5927a7651097e784be4430a6ade09951f5b6879cd06b0f51fc7c4812af`  
		Last Modified: Sat, 04 Feb 2023 06:20:30 GMT  
		Size: 49.1 MB (49081538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f6dd523027aa16778d661d27e72bbe882cc841d9a40bcf7ba993f9653c66e5`  
		Last Modified: Sat, 04 Feb 2023 06:51:08 GMT  
		Size: 8.9 MB (8865599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef33a1f8ffdb43ea2d51e44c388d4de6bedede50060c1397f6ae0eff23cd307`  
		Last Modified: Sat, 04 Feb 2023 06:51:09 GMT  
		Size: 11.3 MB (11319794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f81f9fe3edb2827f590b523951ed4c6d26f17d9aa521c3b4da9f99c21d74bb`  
		Last Modified: Sat, 04 Feb 2023 06:51:25 GMT  
		Size: 64.3 MB (64337322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:4b903beb883453ec5cc56f4c8709711ce5fe54092e1ea4da664b3ff103819bef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.2 MB (137178628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42bb74a0e693795d2afd68770eb2599fbbebe5ae6bdf64637f65e2174b4abf5e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 07:48:40 GMT
ADD file:71f93fd08314b2207fb2e5840185c4db4279fa8f008742cf35eaf4daf925d475 in / 
# Sat, 04 Feb 2023 07:48:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:17:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:17:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Feb 2023 08:17:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0b6e1871a6864b2026696c7ffe48da3030a97146a6a0f3ca18f87c19b1ed6e05`  
		Last Modified: Sat, 04 Feb 2023 07:53:55 GMT  
		Size: 50.1 MB (50093420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd7274669ca31ae25c99ffbeb62b7bf63cf6e70c0afea787b6483e8e1e233d5`  
		Last Modified: Sat, 04 Feb 2023 08:25:56 GMT  
		Size: 9.2 MB (9211501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:222e731d14a700e618d6e7298602f00a0ac9884fbe12a867349d9a13ae14bb4a`  
		Last Modified: Sat, 04 Feb 2023 08:25:56 GMT  
		Size: 11.6 MB (11557630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e9553d1e75be1e95f064cd22c826152b2da62a778c20ddc098b2c20f0575749`  
		Last Modified: Sat, 04 Feb 2023 08:26:15 GMT  
		Size: 66.3 MB (66316077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:58f7776ae5802beb5ff95c124b893ff3a2ce121f93e98d305337e9feeeb340d9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.9 MB (131875223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dde5105ffa4ba49e36c8a2afa67c343d1f83bde2ad9dde91a2a56b5056c6d4f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:43:09 GMT
ADD file:bff5ae942e6561f2afffbbd0267d57706f7fdd71ebe43c64b369b20940d55f00 in / 
# Thu, 09 Feb 2023 02:43:14 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:31:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:32:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 07:33:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9aa6addfe979ac43879ea9517851622f7a6c1516568fbd6a0c101c3b86cc1163`  
		Last Modified: Thu, 09 Feb 2023 02:51:51 GMT  
		Size: 49.1 MB (49063446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6db93799880bf6f9525fc696324e0d450fd37ebbb37d356955a9057236da38`  
		Last Modified: Thu, 09 Feb 2023 07:56:29 GMT  
		Size: 8.4 MB (8399010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b19fed47eb69b023968097b12ef67cad0d7e15a03675cc16e3efc9b67a44e4`  
		Last Modified: Thu, 09 Feb 2023 07:56:29 GMT  
		Size: 11.1 MB (11105521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7152f2a237e2d177c5dc02d27a4b1e0433902b36280eb92369c2a9e5620678e`  
		Last Modified: Thu, 09 Feb 2023 07:57:24 GMT  
		Size: 63.3 MB (63307246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:5ef1ccac77b7a35c2624b8940bf82805158775082acc36816c2cfae75b16fa88
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.8 MB (144765041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9664bcd46d31c8a430f2aedffde78fb56d2978323e5ccdd953445f5547d178ba`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 12:24:35 GMT
ADD file:75252aac3ef2cfeb95bfa5e27d34d7632e938a4cc508e662b033aebb438bf9ed in / 
# Sat, 04 Feb 2023 12:24:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 17:56:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:57:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Feb 2023 17:58:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ad7bb1bf81ba24a5e75d96e5759bfa08a04cf654eda26010b8b1bdd6eead92f2`  
		Last Modified: Sat, 04 Feb 2023 12:30:47 GMT  
		Size: 53.1 MB (53066627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a43d91cb4f1d38d440125ef18b21ed870c9dcca915dc7e20243430d8adac5f`  
		Last Modified: Sat, 04 Feb 2023 18:12:46 GMT  
		Size: 9.6 MB (9613419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42696410cee2c14decf6673c1f2af21d8399af5087bd8d0a8aa5836b6eb83e2`  
		Last Modified: Sat, 04 Feb 2023 18:12:47 GMT  
		Size: 12.1 MB (12114689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b254d8489afdf84cf599567f5cd06ddb9dba650b5f29b68b0ecdfae7fc17d0f6`  
		Last Modified: Sat, 04 Feb 2023 18:13:18 GMT  
		Size: 70.0 MB (69970306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:34df88bcae10c5f6c08701e3d38c3c7058b80d1291458843d1e242251076b9dd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.7 MB (130704781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7f58248367caeacdb8799058f1735bf37cccd19ac2f573cae283bf951e27eae`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:40:45 GMT
ADD file:0edac1ca3f05ba1f621c1dab181be5479d166d4a4c6a303bf07be225c572bb84 in / 
# Thu, 09 Feb 2023 02:40:55 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:22:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:22:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 07:23:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:667517dccb1c9b12f559214da46416c75d071090a71194ab7882908fd3eddc8f`  
		Last Modified: Thu, 09 Feb 2023 02:45:19 GMT  
		Size: 47.4 MB (47428619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50816d8e878439c60f498af4735ce27a1ac8c0c9b4fb1af0b2cc5eb3b170d3b9`  
		Last Modified: Thu, 09 Feb 2023 07:39:38 GMT  
		Size: 8.7 MB (8666639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b757e546fa8d91f119cec4fc64f69f4cb03d686f61e9c39493d98bf75ec0b5d`  
		Last Modified: Thu, 09 Feb 2023 07:39:38 GMT  
		Size: 11.2 MB (11218326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:545f4f8d16022f0b19ec3c8035e95c53e495713d06ca6d692cda8901987c1671`  
		Last Modified: Thu, 09 Feb 2023 07:39:53 GMT  
		Size: 63.4 MB (63391197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
