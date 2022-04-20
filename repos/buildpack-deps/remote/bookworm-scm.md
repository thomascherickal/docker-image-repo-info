## `buildpack-deps:bookworm-scm`

```console
$ docker pull buildpack-deps@sha256:fffdaa75e2e29dec2cabb126348a4fccfda8ed630a2927636531970ab5e7c431
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

### `buildpack-deps:bookworm-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:2ed9e32ee75449bc6a8e8e74aa75bc0fc034437a40099ba1cd847dd9d2aeb8ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.2 MB (129163594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f478d2f4a3f7e6c4f4f24d4dcf66c7b61f677f47fe30c96a6a9529910c9ddb0b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:42:54 GMT
ADD file:b5180fc4d45b984afa69f3cdfa95980bcdfd76d75f704f74f1aa60e416272f1a in / 
# Wed, 20 Apr 2022 04:42:54 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:56:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 06:56:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 06:56:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8cb01d170a54a4c7fd7c1969e79df0a453468ebabfe1d860b863f7a3b6fbbc2f`  
		Last Modified: Wed, 20 Apr 2022 04:47:18 GMT  
		Size: 55.6 MB (55578729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec411cc74e7329b4aa762298d902d14025f16214d6dfccffc28adffa29c655c`  
		Last Modified: Wed, 20 Apr 2022 07:04:37 GMT  
		Size: 5.2 MB (5208374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3518a73a45d857ec3136592d439326badcede35952ad723c33e4148b5e83d9`  
		Last Modified: Wed, 20 Apr 2022 07:04:37 GMT  
		Size: 10.9 MB (10924132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fee26143ae45bb521ee21c064678ca5bf451d9c940e15c92b78ccd693581c0c`  
		Last Modified: Wed, 20 Apr 2022 07:04:56 GMT  
		Size: 57.5 MB (57452359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:bb7f5c46626d12381975d367b143219edf2203af090efcb0c68b3db1d72f886f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.6 MB (123565854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbb50557e3713520235216ce35aab735bafc92f342a1927d468deccd32bbc2b7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:07 GMT
ADD file:6b5b5c095508b777a2c8b2633d97d6143bfab0320bed58e8e335179bfd681fc9 in / 
# Tue, 29 Mar 2022 00:49:08 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 07:38:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 07:38:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 07:39:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b209f6efb315c2c09d16e50d6077a10a401191c741a83c3c6c0767fe202d69d`  
		Last Modified: Tue, 29 Mar 2022 01:03:30 GMT  
		Size: 53.0 MB (52995524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bc9d490149e4bcb11fe298e2c5a923c08cc31f08662f9f7637aca6473309b73`  
		Last Modified: Tue, 29 Mar 2022 08:02:54 GMT  
		Size: 5.2 MB (5163931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1132e128b11ccea17e38c248a34ec3142776903dcca038a3e7789c9e8f52f6a1`  
		Last Modified: Tue, 29 Mar 2022 08:02:56 GMT  
		Size: 10.6 MB (10597029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bea4cefcae02c237fe7371ca4d568c1f51b28d10f874dfcdd78ad48b4b5234f`  
		Last Modified: Tue, 29 Mar 2022 08:03:39 GMT  
		Size: 54.8 MB (54809370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:21f66e4092ab551782c796084940b5907898fcc50999fb031990333b9f5638df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.7 MB (118657535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dc33a412ccde92fbff156e9e0ea046d7091849d57949d4e6b1bdd5f2648be3f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 02:16:59 GMT
ADD file:5ab9a8a4847f677425562eebef8854e58592bb57501d4bc6f521315d90815c3c in / 
# Tue, 29 Mar 2022 02:17:01 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 20:02:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 20:03:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 30 Mar 2022 20:03:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c7c8b286eb908a262d0005e4560150fabc15db4a3531f7e00f77b76643457e6c`  
		Last Modified: Tue, 29 Mar 2022 02:32:14 GMT  
		Size: 50.6 MB (50609802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d739161e2986c208982baa48eed3572da3097ebf10a7f4e51faf03c0273ea371`  
		Last Modified: Wed, 30 Mar 2022 20:27:35 GMT  
		Size: 5.0 MB (5023298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94e98cfbaf9038f43192a4328368893d374a691bbc690dd7b94222d51e41dfd`  
		Last Modified: Wed, 30 Mar 2022 20:27:37 GMT  
		Size: 10.2 MB (10244161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ff68e3ac47baa10b1f98b0d5f14dbfc37964e7a2b10b452927f86c64fd0f84`  
		Last Modified: Wed, 30 Mar 2022 20:28:25 GMT  
		Size: 52.8 MB (52780274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:fd52811891081d0cca612515a585490a7dca25f45c00c856b759732061a1b9da
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127864531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6dc0826f90274e47dea58aad1efd0aefc5af813c7d865310ad3f6847a3412f4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:28:29 GMT
ADD file:23397ad30e34521aa2c0881ab09c9c75f58316594a1c14f01cfcb212161c32fc in / 
# Wed, 20 Apr 2022 04:28:30 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:42:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 06:42:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 06:42:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c6d996fb7c2fde9d95056213e2cc0a2ea025cc86ce1ceeac46b8c51b2d458d84`  
		Last Modified: Wed, 20 Apr 2022 04:34:39 GMT  
		Size: 54.5 MB (54493289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ee691ff28baa681054135ac8fa72e16199a7024e056d33c427338a21e4dc9a`  
		Last Modified: Wed, 20 Apr 2022 06:53:00 GMT  
		Size: 5.2 MB (5195219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b23bcd2aa6bcebcec9157dcb6c0fecb23e91f1255c588550180d6cd7f9fc26`  
		Last Modified: Wed, 20 Apr 2022 06:53:02 GMT  
		Size: 10.7 MB (10691123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e004e1e477153d2e7cdf23a84ae9b22b0d4d1493b45f04c0e19e20d1ad88f9b`  
		Last Modified: Wed, 20 Apr 2022 06:53:22 GMT  
		Size: 57.5 MB (57484900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:7e7f4df6480567258d5bdbd4f7a72bbe07a707af36338964e6ae0e39615fe3cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.7 MB (131744957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d38e772feb103d65506c709d2a96069d476b1bb7becdc4177965fd44cd85b9c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:41:20 GMT
ADD file:828aa883b729cb9e3bbc9efef043626425a2803461bd7b07862d746e2df08c10 in / 
# Tue, 29 Mar 2022 00:41:21 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 17:53:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:53:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 17:54:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4e0acfe1e9e31a265994eee72788e1a0b4b33edc5c9d6fc978fd65d87aa94b53`  
		Last Modified: Tue, 29 Mar 2022 00:47:47 GMT  
		Size: 56.6 MB (56628219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e1b01718568970f8976ea798ed333d8acb22b4cdc57a341b078bb0a7e4e4dc`  
		Last Modified: Tue, 29 Mar 2022 18:13:41 GMT  
		Size: 5.4 MB (5400088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296971f2bacc0edb451554653b20751f9adfa0cbce82cb5e06a78c72076b036a`  
		Last Modified: Tue, 29 Mar 2022 18:13:41 GMT  
		Size: 11.1 MB (11103529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556f03b11aedb9bbc81a6111cf72e7c011c9682d79ce42ad6dba4bac5f1a2340`  
		Last Modified: Tue, 29 Mar 2022 18:14:03 GMT  
		Size: 58.6 MB (58613121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:b8fee69864b233a92ed8b6d5822a190fa190cfe5632e646f47ad57f1ae989978
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.1 MB (126085794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e672d1ede339aba1da7ceb30c333dd3b1a868d93299b70e01fa0f2ff4f96b09`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 07:40:39 GMT
ADD file:88e75745fdbfd0784c1c18134a0a52a5534df18201a6f49555a5c618b4531804 in / 
# Tue, 29 Mar 2022 07:40:44 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 08:16:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 08:17:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 08:19:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bdc3f4c024aea887030bcf477ee808da6aa3e6683fb111845d94ab4f2480ff24`  
		Last Modified: Tue, 29 Mar 2022 07:50:58 GMT  
		Size: 54.2 MB (54240334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e94f68f0d96094b4bd1aa9ba6f4465ec7d6879ed28f910b949ffb165eef3fe`  
		Last Modified: Tue, 29 Mar 2022 08:54:21 GMT  
		Size: 5.2 MB (5221857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd581c56a027feec68bb7a881cac731bca045297cd76398414512c34351a063d`  
		Last Modified: Tue, 29 Mar 2022 08:54:24 GMT  
		Size: 10.7 MB (10672471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3631eb84b5e85d4e37526f1ae6b1259a7a43e8e02c45f72f851783117629e90a`  
		Last Modified: Tue, 29 Mar 2022 08:55:13 GMT  
		Size: 56.0 MB (55951132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:0053bed0b7a1e1761cb1fee867ed996db25d9904be642887e9f2dd3d1d4f06c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.1 MB (139113055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5155314e54075e4a93b0f43156dc592225d511d363017c2b4162b88121bed87`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:20:10 GMT
ADD file:c9ff325b9fe680d344c36e7e25729f90711bdf646908892ebdc0f3a53d92bc50 in / 
# Tue, 29 Mar 2022 00:20:29 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 05:30:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 05:32:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 30 Mar 2022 05:34:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fc5522fc3ca5c5e9e4af133a35ed8a4e104c9366b7ab66c3cc5601aef68f175a`  
		Last Modified: Tue, 29 Mar 2022 00:30:15 GMT  
		Size: 60.0 MB (59999423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31127088a5022a99c9c420931875f462b30887ac8cdd2b9832e9a48833053641`  
		Last Modified: Wed, 30 Mar 2022 06:23:56 GMT  
		Size: 5.5 MB (5543257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f20e81de5da1931ed0a987d558ca1844e91b01be66fe4fa9f9a11ab9c2e851f7`  
		Last Modified: Wed, 30 Mar 2022 06:23:56 GMT  
		Size: 11.7 MB (11702051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9353b28a9fb4647d78b62d393fd6fe5b2983eee962f4429ab69b8baedb393997`  
		Last Modified: Wed, 30 Mar 2022 06:24:21 GMT  
		Size: 61.9 MB (61868324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:37305a789a3733ebe0b8150df0204f5d8bc3b689a8bac40fd4858f460d8b7464
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126462957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d02bcac061e8afd5b333d1b4d067667873e79da6df5df79de20694d5b33fd111`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:51:05 GMT
ADD file:9a99e896abdfac4163e20511778572abbec89bf317a3c3dad1f6fe0c63b126b1 in / 
# Tue, 29 Mar 2022 00:51:11 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 02:23:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 02:23:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 30 Mar 2022 02:24:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4c231abb22533340c714e28363f98b83f5da88a6702fdfc7d06ed65b8f2e70e1`  
		Last Modified: Tue, 29 Mar 2022 00:57:13 GMT  
		Size: 53.8 MB (53839067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b1f72f77effa39a86785d5e5242154a329664927615884293ae53de3228e345`  
		Last Modified: Wed, 30 Mar 2022 02:32:53 GMT  
		Size: 5.2 MB (5245181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a40794a51d7ee7ef5a9c0175be5b9245646cf0f2703acbb34ea8e72c731272f5`  
		Last Modified: Wed, 30 Mar 2022 02:32:53 GMT  
		Size: 10.8 MB (10819318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c986ac3bb53ec5a4892c250c435a3e59ee79ddb71f265aa5d083d3f87a1faf3b`  
		Last Modified: Wed, 30 Mar 2022 02:33:07 GMT  
		Size: 56.6 MB (56559391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
