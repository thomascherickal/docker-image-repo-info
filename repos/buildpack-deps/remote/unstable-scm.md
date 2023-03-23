## `buildpack-deps:unstable-scm`

```console
$ docker pull buildpack-deps@sha256:14c1f129fc916f448f6fe492c5d2d1a0d228118aeac6817bf035de4089433ef0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:unstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:e98f8806c2af366ca721b9ba594c9cfe50f2004ed51f97131b64eecc1fcb3664
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.1 MB (134053803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f2dba165ba7ec43a775ec8bc4c61adcc06332fd151bef98bfd2d9deffa912cd`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:31:25 GMT
ADD file:8efef3fd1e16c5994e0b27af5c19056cc369818d299aaf62b89b89ad82426fe3 in / 
# Thu, 23 Mar 2023 01:31:25 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:04:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:05:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 06:05:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ddb08f6d450933d22f98a93a56726ec0491dcd496caf4455cfe7066900409348`  
		Last Modified: Thu, 23 Mar 2023 01:35:52 GMT  
		Size: 49.3 MB (49291637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b67c216879c602a3357a3e051406068e953242d0d7b402dd7e6671d414199c7`  
		Last Modified: Thu, 23 Mar 2023 06:09:55 GMT  
		Size: 9.1 MB (9081298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184c8a28afd4da0484a1f9c3cc7e52748726daac5cac85bc0fc702f666f1939e`  
		Last Modified: Thu, 23 Mar 2023 06:09:56 GMT  
		Size: 11.4 MB (11422514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e65c6e206a59e86efff44db2d95c81b3eb92e784a910507906ef0fabd1c750fc`  
		Last Modified: Thu, 23 Mar 2023 06:10:12 GMT  
		Size: 64.3 MB (64258354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:769b660d04142b0b50dc374c44a0b6f21f9c173ee6da78112733f53722b345b1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.2 MB (129237697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edd56cc8039bae242894637cb565ef5a4685943100e6e52d22630c1fe20fb1f8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:49:01 GMT
ADD file:4fadb88d3ead8d91349c79d7e903bbb8f6130b292bda6cb8099131210a815bc1 in / 
# Wed, 01 Mar 2023 01:49:02 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:21:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:21:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:21:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a03e1abdb2ebe924d64faf35eb6563891039999ec54a62f65419caf539ba6a88`  
		Last Modified: Wed, 01 Mar 2023 01:53:21 GMT  
		Size: 48.1 MB (48107781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d446d9cfc1201a906803d21a6e36423e22e9bebf24cf64bd16a4a3a73af61a2`  
		Last Modified: Wed, 01 Mar 2023 02:26:11 GMT  
		Size: 8.5 MB (8514426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14dc22595c5f06cd6d232ff8a3594b9aadef31095cb355dffad2b48a861717bf`  
		Last Modified: Wed, 01 Mar 2023 02:26:11 GMT  
		Size: 11.1 MB (11051502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0760e34b5fee30fa55ba71775caf6a3b2e755775ea03be4db0c03e5d83ff0a3`  
		Last Modified: Wed, 01 Mar 2023 02:26:32 GMT  
		Size: 61.6 MB (61563988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:eec8b1e8acf1938703616b1dd5e636aafaf9a348da0a8b4f760abadf820d5f02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.0 MB (123998226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4711888af9d924bb6d81ff35c959c48dc8dd3764331e7e8f75c4be9208721f1b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:58:39 GMT
ADD file:2cc322ac43103c8e367e39beaccf285da593ce4935ec4b1c90ae321a43b7123b in / 
# Wed, 01 Mar 2023 01:58:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:36:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:37:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:37:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4e5967747d4d88696bd5d5f37c0b5b8bcf8b29f3b448f6d1dd9623bdcc655965`  
		Last Modified: Wed, 01 Mar 2023 02:04:52 GMT  
		Size: 45.9 MB (45878967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00c059161524278c4c36c19bc9e15f881a76d35dfa7907d64e5368fa08cfabe`  
		Last Modified: Wed, 01 Mar 2023 03:11:27 GMT  
		Size: 8.2 MB (8158629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e2cef807b62672343d701b6833953bd521a7ce41702624f45d2d796b0748e2`  
		Last Modified: Wed, 01 Mar 2023 03:11:27 GMT  
		Size: 10.7 MB (10687679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4aec6c2a63ff15795fd7235464c074e62a01aab27b66c75e51aca4b22d1ec07`  
		Last Modified: Wed, 01 Mar 2023 03:11:48 GMT  
		Size: 59.3 MB (59272951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:4e5491f6db871ba1979c616e0434998a34addc854eb6f3d327bd77639389aa11
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.8 MB (133774554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0123a918193fc7abfb1ed93addde3bc3ba068fceacc8cf3e06a58791c38e1e6c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:42 GMT
ADD file:56248f74ca6cf497dee2c80a5824447bf5ee5e730a9c092f440d9c666ec1c076 in / 
# Thu, 23 Mar 2023 00:45:43 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:14:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:14:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 07:14:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3a84baeeebe4b5ede833105ba5c2fe8b6102a8c47c386cc79b5833fea9489c99`  
		Last Modified: Thu, 23 Mar 2023 00:49:34 GMT  
		Size: 49.3 MB (49318983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0d42af9a92d82ccbe90040ec3d71455dfd1d92426d7f302766baf42eb07f8b`  
		Last Modified: Thu, 23 Mar 2023 07:18:50 GMT  
		Size: 8.9 MB (8914256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb28b2a98fb7b8844969dec5b68c7cfa2df0d77f1ab1a55bbfac387493184004`  
		Last Modified: Thu, 23 Mar 2023 07:18:50 GMT  
		Size: 11.4 MB (11388593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97069ba18337ebbd2738aac40ed449af0931f84e6a095665ef234602c5b1fefd`  
		Last Modified: Thu, 23 Mar 2023 07:19:05 GMT  
		Size: 64.2 MB (64152722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:6cde2155211d3f4d8d5db27af2fcc9954e9dbbe93b2e7a4208d6d145acb510de
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.4 MB (137386558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed49974f31df5dbc1da3062aa51816dadfe02a8052b7def49df2b41c34fd9ff7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:40:05 GMT
ADD file:6282b025bbfdc732e0b90ff88ecdc7d48b84ec602874ef46e276d0250551f12e in / 
# Wed, 01 Mar 2023 01:40:06 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:14:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:14:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 02:14:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:417b7bc42b68fb696c2efa25377639c22c351f4705d5168da4f5695d53e4ba47`  
		Last Modified: Wed, 01 Mar 2023 01:46:43 GMT  
		Size: 50.3 MB (50314271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65b68a1e6101c58260f889183e2e061e123bbc07a479a4ee59fff5649daa51d`  
		Last Modified: Wed, 01 Mar 2023 02:26:18 GMT  
		Size: 9.3 MB (9251109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63437f1cf3bc2a6cddc930ecd9a659ccfbcce779ac90a9c50efc7e8c1f56b42`  
		Last Modified: Wed, 01 Mar 2023 02:26:17 GMT  
		Size: 11.8 MB (11808756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd353cc8e971b20a47938912dda14d6fec9624aa9880053413a451cb3bc0f60`  
		Last Modified: Wed, 01 Mar 2023 02:26:41 GMT  
		Size: 66.0 MB (66012422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:1fe2cb894be2bc55a95b04e66763ccec91305b7c7ac438bca7d21d751c7809b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.0 MB (132001554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e553975cc4545e2dfa4c801fc4f1bfe90378add106afcf9e70883c34024f725c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 05:18:32 GMT
ADD file:2d913f7b6c2e804834958b3d144bd7b5150a438e2aaa73cdf2f1be1c64d10100 in / 
# Thu, 23 Mar 2023 05:18:38 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:22:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:23:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 07:24:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:83c1a140184ad386a37a5446dba474a2a8498dff7ae8d2ccd2957aaf8dc1682e`  
		Last Modified: Thu, 23 Mar 2023 05:26:35 GMT  
		Size: 49.3 MB (49291603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaaeb19ea7953e3c0a2cce0d76910d46a1fc5e289c90379ecb81b3e5ba2a0c16`  
		Last Modified: Thu, 23 Mar 2023 07:37:04 GMT  
		Size: 8.4 MB (8439874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ecc4eca24f781c1e786d1fc88cb24202f1248f85adc06cf1b375f5607ec2d93`  
		Last Modified: Thu, 23 Mar 2023 07:37:04 GMT  
		Size: 11.2 MB (11170914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3768b306fba92d6a836552b3ee3a1bb755cd0f7d6618ca028d0643fde06553`  
		Last Modified: Thu, 23 Mar 2023 07:37:53 GMT  
		Size: 63.1 MB (63099163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:0f7a8b3c9b4996e2ee9e65041bb5c8ea311482213b54d004d43cfa0da3bcf469
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.7 MB (144711239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1a4114106d760615f32f4b575122bc6f8862f40d4c00e8535a1aa756c7b5014`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:54 GMT
ADD file:2c1195fd765d1da7082bf383b9c5ef0b244e5398006d53897d5ea40e919399f1 in / 
# Wed, 01 Mar 2023 04:47:57 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:30:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:31:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 05:31:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b6800c47237e7f7a1e5340856e56ba98e2b69a475b2458bb2416fdb0582d8c28`  
		Last Modified: Wed, 01 Mar 2023 04:54:24 GMT  
		Size: 53.3 MB (53273011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ff0fff502cf707b8386c45c579606a759f85d3b49c007814826ad27212fdf5`  
		Last Modified: Wed, 01 Mar 2023 05:41:08 GMT  
		Size: 9.7 MB (9652015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ef4d32b9b5d605909945396d9e13b86c238ff2ea6c800b63cef6d06dc2d6a3`  
		Last Modified: Wed, 01 Mar 2023 05:41:08 GMT  
		Size: 12.2 MB (12168382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecf54311632074a960030227c6fca18a718af9b2631164c5c93529e814a5f50`  
		Last Modified: Wed, 01 Mar 2023 05:41:38 GMT  
		Size: 69.6 MB (69617831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:12a5f9d61b1c3164143a0e4722b12a0a831112cb11724d5a9e4b2846af3b99ad
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.1 MB (124109021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68c2bbfb4b6cf018cd67be63e70545b8af06e1a6861370502c893f5a57168df6`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:09:07 GMT
ADD file:0ead2f17f27ee13f553b88d07f59f56840fc40a7d668942a261c1a8714543b00 in / 
# Thu, 23 Mar 2023 01:09:09 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 01:31:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 01:32:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 01:35:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:94da1857a4ca1e8976329ef725087fbbe73af98bd925fbca65400b32537f3178`  
		Last Modified: Thu, 23 Mar 2023 01:12:27 GMT  
		Size: 45.5 MB (45471889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34c96232283bbd760cb6134bc51d0a8713ce646f72c2f26103aecffb6f0744dc`  
		Last Modified: Thu, 23 Mar 2023 01:44:11 GMT  
		Size: 8.1 MB (8115301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58559086b64d3108c9d17e9f17b13d71448a05197854524491ba5f1c5889ab5`  
		Last Modified: Thu, 23 Mar 2023 01:44:11 GMT  
		Size: 10.8 MB (10788034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5854e28797388adf451df519f9fc31237b24ea2ad1aa16b56d8cc738795ffc24`  
		Last Modified: Thu, 23 Mar 2023 01:45:30 GMT  
		Size: 59.7 MB (59733797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:2d83507acd5909154d62bcfdda5174b1b880e9f302aab12fab33e0a1a53f6646
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.9 MB (130902463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afd200a3874d4c741494aa8f0f571c866d0938b2ca75761b38368f5d1f76ac8d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:44:17 GMT
ADD file:f722c963bb9fb9eed0d7ba7fa5de1fdaf0fac91107cd71702d55f0cc074cd6ee in / 
# Thu, 23 Mar 2023 00:44:20 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:17:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:17:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 07:17:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:866ca1f7e7197a336b8f05cbbb9eb6e6a32a17ade3068f3bd62dd93f926293d6`  
		Last Modified: Thu, 23 Mar 2023 00:47:32 GMT  
		Size: 47.6 MB (47648043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a6b4cd67d490a2c70edebe1070c48db7a7451d2f3907f036960fa85459f9f4`  
		Last Modified: Thu, 23 Mar 2023 07:22:03 GMT  
		Size: 8.7 MB (8713413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ea7fdd8644a777c3ecd69ea57c24497971eabba7d4f9f5d7a151239348da4c`  
		Last Modified: Thu, 23 Mar 2023 07:22:03 GMT  
		Size: 11.3 MB (11285989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae83324033fd40f1d83bc12ac4be12dea69bc5afe1fb1e3fb18bcf2e5108bff`  
		Last Modified: Thu, 23 Mar 2023 07:22:16 GMT  
		Size: 63.3 MB (63255018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
