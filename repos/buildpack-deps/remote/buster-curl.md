## `buildpack-deps:buster-curl`

```console
$ docker pull buildpack-deps@sha256:b07fb7354e9b5998aace1272b6c30cb921e36db523a7f08c8af93967c1e6d8f1
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

### `buildpack-deps:buster-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:a0bba8f1fd79022a347c88c8ba94f43b7b9a85b2a241a977a2d15ff65f3b9974
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68268068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae7b4dd26afae147336976cacba2d6de091e5f31ce99148eadb745564c75cdf8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:51 GMT
ADD file:cb5ed7070880d4c0177fbe6dd278adb7926e38cd73e6abd582fd8d67e4bbf06c in / 
# Wed, 17 Nov 2021 02:20:51 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:15:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:15:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1230f17f526cb07307d41462355b10488b994e8bdafe0d8f275a405fa3b33831`  
		Last Modified: Wed, 17 Nov 2021 02:26:06 GMT  
		Size: 50.4 MB (50437098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17d0de332ca1b34d53ca41c2b39ea52ce72f8c1e81c5200e27a8bade3e6ecbb`  
		Last Modified: Wed, 17 Nov 2021 03:24:34 GMT  
		Size: 7.8 MB (7833787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7474d56348f5333567750c1e5f06f899477fd437330627341eafa71bfa1a36ab`  
		Last Modified: Wed, 17 Nov 2021 03:24:34 GMT  
		Size: 10.0 MB (9997183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:b140abc457f97daff918385b366ef37a61f11bd24028a0f05be0fd904723f38c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65218772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ca71e57b57c8f55f460a4ef80141da4552e2dd1317eccfae4a8f32e70126712`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 00:50:58 GMT
ADD file:f9432d6da0faddeaa117c57c0c007cd56738ef01549baf71e5c59939b7e69b6c in / 
# Tue, 12 Oct 2021 00:50:59 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 05:45:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:45:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ae00de77d9c27fe3ba9ea06833b273e4fc0aa128a3a61d3992632e6e3941a78c`  
		Last Modified: Tue, 12 Oct 2021 01:07:01 GMT  
		Size: 48.2 MB (48154085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52282bf2103fc337ab7cc23ebfae979096e6f901b62960b03952c2d52e9978db`  
		Last Modified: Tue, 12 Oct 2021 06:04:31 GMT  
		Size: 7.4 MB (7377193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b1aa5c1e770fff74bdcd066b443f1e1e49f677ae77ec80d22c50e20be8c3b3`  
		Last Modified: Tue, 12 Oct 2021 06:04:32 GMT  
		Size: 9.7 MB (9687494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:e724e938ae162d22679aa13688acc32788d5193b4f552dfd33702ad1843e3bc7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62387132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b37d37a14a96bf4731ecee8b62e9002e52f378b5a25d0f6668dbc7a96554394a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:00:12 GMT
ADD file:d71807613acdf86685f6d640a90e27b7b63cfe0f13d88668ee943aca089d8876 in / 
# Wed, 17 Nov 2021 02:00:13 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:45:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:45:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:10acd81022d17f452439d0385615fa066b8f0ddcf3c1a803872eec5bdc6acf64`  
		Last Modified: Wed, 17 Nov 2021 02:16:00 GMT  
		Size: 45.9 MB (45918099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a9604eb6c465f658d6422593d504030155029fe0c4302451d4369030c29144`  
		Last Modified: Wed, 17 Nov 2021 03:07:14 GMT  
		Size: 7.1 MB (7125194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b043b954c4f0757e89df96897cea2cf1f93c6275466008e4ba7a4b1089c7dd3d`  
		Last Modified: Wed, 17 Nov 2021 03:07:15 GMT  
		Size: 9.3 MB (9343839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c1e616cca54f9840d18070c50cad0360512e66f3195284df61b10d7be06f4ad3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66685108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71c63916904dd879b189d96113422b32fc3f7fb35c2f0f2edc91f9858a2846dc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:28 GMT
ADD file:aed1709ccba6a81b9726b228fad7b81bcf4c16bafe723981ad37076322d78986 in / 
# Tue, 12 Oct 2021 01:41:29 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:59:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:59:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:2ff6d7a9e7d73e4a01b9417518d18c001728c45fa8109ed8f55aaa50e7981482`  
		Last Modified: Tue, 12 Oct 2021 01:48:38 GMT  
		Size: 49.2 MB (49222756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7324ea4098419bc5fa2ac5a138522230bf12cef3996d1740dd00f9d4737d004`  
		Last Modified: Sat, 16 Oct 2021 03:15:37 GMT  
		Size: 7.7 MB (7695063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e213c33a07316d84d829be685bd3b02e1e2bc135f7748c932050e6ed6a3a0d3`  
		Last Modified: Sat, 16 Oct 2021 03:15:37 GMT  
		Size: 9.8 MB (9767289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:2486e26715fffc0103cff821dabfb04a4065f77b779ab7740ee9ef68bf6628bb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69547743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eddce9da46d7c9304a8b60a2eea1e90ec1647b65c857487a9d68b7bb1635d413`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:40:01 GMT
ADD file:1461fa0362c70b5b7a677c57dd48633827fd9635a9cb136730aa7581cc523b46 in / 
# Tue, 12 Oct 2021 01:40:02 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:37:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:38:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f4b233498baa64e956a5f70979351e206bd085bd547a3cf25c08b154348df726`  
		Last Modified: Tue, 12 Oct 2021 01:48:07 GMT  
		Size: 51.2 MB (51207606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece122ff48522de249e81ee22f617bf84d59b003d3c79f44331163046a937e4c`  
		Last Modified: Tue, 12 Oct 2021 04:49:37 GMT  
		Size: 8.0 MB (8000221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:378307f52e8eeddb964324804377cd9fd65b1bf7b848c5b690e63ef92f1fe3d5`  
		Last Modified: Tue, 12 Oct 2021 04:49:37 GMT  
		Size: 10.3 MB (10339916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:1e592540bdca585a60fa24b22ca3a5e330f8e8e095cf48f097604cd0e0f4250c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66349467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a765dbf7709fe9c6821e4c08f9723711989886c37e0a77c9a2f91390c44d5a6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:11:41 GMT
ADD file:37326203d7d5c7764007ca3a26d61a2da861011dddf8992bc1a0b70ba659c0c1 in / 
# Tue, 12 Oct 2021 01:11:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 01:53:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 01:53:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f086aaa10cbe2dfccc93401fe3cce55b2f5eed2ba1a2fe3e34a4501644f9c8fa`  
		Last Modified: Tue, 12 Oct 2021 01:20:49 GMT  
		Size: 49.1 MB (49079545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d616f4bde99abe068eb28ab4b7ac4257ded3b68bf57ef8468607497a525bdd5`  
		Last Modified: Tue, 12 Oct 2021 02:08:26 GMT  
		Size: 7.3 MB (7253602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbdf78718a4b3eb02fe6ebafb667a2227bd7ec3516a96e56b8939f548ee34ee1`  
		Last Modified: Tue, 12 Oct 2021 02:08:26 GMT  
		Size: 10.0 MB (10016320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:c251eb2b5dda1256e94dbe286223fa7a2b7a2150551d407a48b41214a930df2a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73184063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:105266d822080e876b97e27c2bc02e8aa91c73fc45afef1ccb5942266e9800b8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:26:10 GMT
ADD file:94a7157f0c578810dcc73fd2dbdcb4ce021626d9858288c970e007a590c71d44 in / 
# Tue, 12 Oct 2021 01:26:18 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:06:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:07:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:77e7cc3fe486cc9a5ddc4cee43979cbebb5e7c4f36b82ccaa61dbda5dd37dac8`  
		Last Modified: Tue, 12 Oct 2021 01:37:52 GMT  
		Size: 54.2 MB (54183476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef410353e2a31335f42fc4620f0d13cd6062c9ee6aa1dd0b300f7a8cbadedc5`  
		Last Modified: Tue, 12 Oct 2021 04:42:58 GMT  
		Size: 8.3 MB (8272912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f783e122aabe6c06785c6c466429027a12dd9c8c4ca516dcebccf1d0186d751`  
		Last Modified: Tue, 12 Oct 2021 04:42:59 GMT  
		Size: 10.7 MB (10727675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:2f148905d6fe03767f7cb6e8c4fcbd6b5a200f0a6b8a9907394dc5154a203300
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66289868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65862f040a1b0973ae86d1e0f56a13ec80e7c12e566a3f87dab7af1ec5238448`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:40 GMT
ADD file:dc4ee96f81059accdc88a686f80f1714bc9d2f383af71c0d130c08560cea115e in / 
# Wed, 17 Nov 2021 02:42:42 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:10:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:10:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c12eae84d2674466d924a139a276e361afa9f63de21cf77eae19bd94eaac2629`  
		Last Modified: Wed, 17 Nov 2021 02:48:42 GMT  
		Size: 49.0 MB (49005439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564a8b4bf4cf08933f04084cd556e9c716474b9801854ea7c4473c9804894516`  
		Last Modified: Wed, 17 Nov 2021 03:18:14 GMT  
		Size: 7.4 MB (7401273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ffdc4b0bb501f5f5214892baa1a5d53d44ce92b645995a43fe2cfeb2ffec6d1`  
		Last Modified: Wed, 17 Nov 2021 03:18:14 GMT  
		Size: 9.9 MB (9883156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
