## `buildpack-deps:unstable-curl`

```console
$ docker pull buildpack-deps@sha256:e8dd2a1915643f43e89612e8e33244ea349a4d420916e285824797d6e22f0496
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

### `buildpack-deps:unstable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:d99204303e12faea688a7d019fbc3b85477471efab8d74781ff33dbb92713158
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.2 MB (72246154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4343996b06ffde754a6c5a48d8423003766aabad49c840c76a1df9302d618f3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:44:37 GMT
ADD file:859abf2d579747b132742454ad96e32dc879955afff8af84fab63dc41312a0e0 in / 
# Wed, 20 Apr 2022 04:44:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:00:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:212be0dc3a8ffdc400158a5e3a9812f7413dbb5a86269ff50e41b84b37fdb9f7`  
		Last Modified: Wed, 20 Apr 2022 04:50:51 GMT  
		Size: 56.1 MB (56112566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b0603dc0dbc00177fa56a8c1af60fd29d0bf2e8e1e8df8772164b08d8ba1ac`  
		Last Modified: Wed, 20 Apr 2022 07:07:58 GMT  
		Size: 5.2 MB (5209066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da99ea31fc35c2341d30c71a1992c692753c04c61b2e1c25053bc3f9d269992`  
		Last Modified: Wed, 20 Apr 2022 07:07:59 GMT  
		Size: 10.9 MB (10924522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:d0d6bf69eb3c4ce430edda97db0da6f07db8a579400148579d4be27cf123be4b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (68968278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e294faf42fc8e4bcf5c3af754d819101392003b214434b9846f6d65b582cc9f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:53:53 GMT
ADD file:8fcd736cc488ae6bc3f8a0a57f5454dbd34b0c05fd62d2bf748eeb34723c2a85 in / 
# Tue, 29 Mar 2022 00:53:53 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 07:51:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 07:52:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:07dd120b73b0ec25351ce0c0743306437c1d81e0ee7e06f053f28a0e58bfa81f`  
		Last Modified: Tue, 29 Mar 2022 01:09:52 GMT  
		Size: 53.2 MB (53206463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:182e180f96ffc4d0dea65f46ebf08c1601dba09f8a2bb20ff2f15148ff227cfc`  
		Last Modified: Tue, 29 Mar 2022 08:11:41 GMT  
		Size: 5.2 MB (5164114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3369a2a9d3d9efecc9720a25d251260ac8afb4a7a974b188960c5a1759c27c2a`  
		Last Modified: Tue, 29 Mar 2022 08:11:43 GMT  
		Size: 10.6 MB (10597701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:8f17f831d0a70379fddee8408c6ed34b162cc3141623d3cd384cf19471a54204
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.1 MB (66092146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4678e5787f84768abde07766a0a7179d918291bd3886c356fa8e85e5c77e7c73`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 02:22:06 GMT
ADD file:c6f82841459351fabc9a42dbd56f6622b4374e2c684eb76537d4f31022fe8774 in / 
# Tue, 29 Mar 2022 02:22:07 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 20:13:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 20:13:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:20059c5e4ca7052150ded6116965ea89f37bd64493315e1aa29821f6adc82ee1`  
		Last Modified: Tue, 29 Mar 2022 02:38:27 GMT  
		Size: 50.8 MB (50813342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77eab1cf1d505662ced1ce7ca793d43715faa8d1006efb38ac9d64a5e87e1feb`  
		Last Modified: Wed, 30 Mar 2022 21:35:47 GMT  
		Size: 5.0 MB (5034266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5291d60208e61bb5100bd38f070ffe9315b62c07b8c223c04ed5c0a722d4ee4`  
		Last Modified: Wed, 30 Mar 2022 21:35:49 GMT  
		Size: 10.2 MB (10244538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:536a3e330888269809c8b5c4f7a8a13b74020d7b5b2fb8c9fb695ee568d73324
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.0 MB (70951424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cc4a76a150ff343abf2927ec60547ca2de50fa20690a12606913d15dddd37dc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:30:37 GMT
ADD file:21175f4b5f80ba5d755041ff362152a8991b53f89e3c6699275e0c99f6ff6acd in / 
# Wed, 20 Apr 2022 04:30:38 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:47:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 06:47:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:414d522b7454847f294a8c61536f57f36cb195df33ab1fce8c838de3d5ae109e`  
		Last Modified: Wed, 20 Apr 2022 04:38:18 GMT  
		Size: 55.1 MB (55063805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc9a9c4b1c386c65ac98874ab622afc88e90b73f7a0e1c692ab412bdd01c571`  
		Last Modified: Wed, 20 Apr 2022 06:56:31 GMT  
		Size: 5.2 MB (5195986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d918141859173a7d14691da560e5afcbb7c353d5694d9541d73f88867578c95`  
		Last Modified: Wed, 20 Apr 2022 06:56:32 GMT  
		Size: 10.7 MB (10691633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:d0e35b6883322226a82a4b8656d3abbdf6c98ff526ed5516c5c2c45bd41c726c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73598673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5266931c41a8966c4df5fa7b71a72276362c5f9803134c5cf5bf4fcede03bd11`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:39:08 GMT
ADD file:92a4df746589380f0ee875ec89574f67fa2f56164bbf20da79eaa902a778eff6 in / 
# Wed, 20 Apr 2022 07:39:09 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 10:20:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:20:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b42fb3c96c9db2aa67a5b3b033791b735ef01e8c8f15321f44a085532b703190`  
		Last Modified: Wed, 20 Apr 2022 07:47:30 GMT  
		Size: 57.2 MB (57154017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00924a45119800495fe2fa0b6d6aaf354e649da6676746c97c18df9c77e13002`  
		Last Modified: Wed, 20 Apr 2022 10:29:51 GMT  
		Size: 5.3 MB (5340392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3faa8d253e5b8d891d6ce9b90e438656a4b5f68ca7b4dfb8f73c36b3da2e9043`  
		Last Modified: Wed, 20 Apr 2022 10:29:53 GMT  
		Size: 11.1 MB (11104264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:15cb843e06b808b346589d7e0cd6274d568935a1a9ff53e324d15ae17ceb2e70
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.3 MB (70348141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e9778dbc2e50e1377256fbe8bc2ab2623d2241b4a1b7439c0d8f0bf6fec0609`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 07:45:15 GMT
ADD file:8f554d1fa0414c8c5592687851c7ff4646547038f7d464423b75f57ecade0e16 in / 
# Tue, 29 Mar 2022 07:45:20 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 08:45:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 08:46:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:024c5d1fff33205caaf39b2903eafbff594af3ca19d825c46db9f726a37cdcd1`  
		Last Modified: Tue, 29 Mar 2022 07:56:21 GMT  
		Size: 54.5 MB (54453471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1267a248cdd21e2291d70a49d2f9b0a81d371a99832c18a5c27c5cdfcd4ec4`  
		Last Modified: Tue, 29 Mar 2022 09:41:08 GMT  
		Size: 5.2 MB (5222051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240eba6da1031777a8269c912451066c83703897876489a9be1d5150c27d785b`  
		Last Modified: Tue, 29 Mar 2022 09:41:10 GMT  
		Size: 10.7 MB (10672619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:688add30407a46604439f878f96d544a3d605f92f34f516b7ec2b011f2a3e9d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.5 MB (77475350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af29e7c91ce7006815ede2819d0bf691aea7bce17a62b3005029b8aabcf4feea`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:24:04 GMT
ADD file:a3e83f143a1077db22a0c3474af3e1641c2c20856ea005f45b8cb6abc754cb26 in / 
# Tue, 29 Mar 2022 00:24:08 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 06:10:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 06:11:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:836a00544655c89c89efabf058adfe305cc708f5259ae1a48e4f895cb836a2b2`  
		Last Modified: Tue, 29 Mar 2022 00:37:55 GMT  
		Size: 60.2 MB (60217263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4cf9a6305a83e9b7a3d1e30896225843f3509617e9eae396ca2ff8c32153968`  
		Last Modified: Wed, 30 Mar 2022 06:28:38 GMT  
		Size: 5.6 MB (5554821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568b61daaaa9bc8bcd70294105bc93761ba802f89f1ec7a66e7fa6694fd35893`  
		Last Modified: Wed, 30 Mar 2022 06:28:38 GMT  
		Size: 11.7 MB (11703266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:93349757186bb36eaa060d8a06e70fc43beca17e9cd771ebbec6c7ff62bf6170
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67098129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fea3c95a654b7c14713de92578eae790807e92dc48efb35a77c76cd0e6000937`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 00:15:39 GMT
ADD file:250fc868a440657403e5cf8fde95da30be6fa0968ce4385656b837e923d678b0 in / 
# Wed, 20 Apr 2022 00:15:42 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 01:02:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 01:03:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5d7000bee08e5edd84dede58b856acde7ae5b24268b5109b3fe7e2260ac19618`  
		Last Modified: Wed, 20 Apr 2022 00:34:42 GMT  
		Size: 51.8 MB (51757327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa082dac6e71b36c14761bb8e8e6da43417464e08b11b0729bf95f3bd2741231`  
		Last Modified: Wed, 20 Apr 2022 01:35:22 GMT  
		Size: 5.0 MB (5016640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe9981ca4f10e51876d1697f6c0393395afae2737f4194422601ede16a3dfcc`  
		Last Modified: Wed, 20 Apr 2022 01:35:25 GMT  
		Size: 10.3 MB (10324162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:733103240a0f0c7b0b9954c288105e620c0d9683ffa6c9d0d8bf984b8c1b6176
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.1 MB (70130313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce269b9b1061a59b1f4add04a142ea71fd0197700bd7eebd7f362f734d365787`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:53:06 GMT
ADD file:5143c5815a4282433726df7dd89926b3676994be1b8575d259b8fb48d6a6a4de in / 
# Tue, 29 Mar 2022 00:53:09 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 02:28:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 02:28:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c86b61bc0bc235576e3d7696ce7a1c21762146f539dc6eda8173ad30b9a4ad20`  
		Last Modified: Tue, 29 Mar 2022 01:16:39 GMT  
		Size: 54.1 MB (54056452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcff4b07483f3bf89081280922e0b152bf4d0bd3c9886eca04d4701cdfdc8bd1`  
		Last Modified: Wed, 30 Mar 2022 02:35:19 GMT  
		Size: 5.3 MB (5255620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34095a4004eb76305dc89b1fe0dd2923e12bd88528d9b779fd1ba62c9ccf1ed7`  
		Last Modified: Wed, 30 Mar 2022 02:35:19 GMT  
		Size: 10.8 MB (10818241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
