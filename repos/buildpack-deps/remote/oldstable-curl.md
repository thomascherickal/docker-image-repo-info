## `buildpack-deps:oldstable-curl`

```console
$ docker pull buildpack-deps@sha256:b27585f8b225d620f7a5add1a3431f6bae29a5f8da4d14fd8cbb7a8b24dd2a40
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

### `buildpack-deps:oldstable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:a4fe6b4a447fe604641e68be2c9a8219e7a598a59c2e61707932625e67be74ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68268396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1eee110dd0cede078c2456a9093a2bee02839814774db0ad32eccd5b8cddb008`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:41 GMT
ADD file:e8b516b464e535b435a6ed8609bac98acc90ee30e2a0667f68932f0d924f6e49 in / 
# Tue, 01 Mar 2022 02:13:42 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 06:27:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 06:28:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1c9a8b42b5780ac49c71f392c9512c0167ecc23de9b30b1b5f38747b73097d1a`  
		Last Modified: Tue, 01 Mar 2022 02:19:43 GMT  
		Size: 50.4 MB (50437046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:163066942b43a00ba7f4674c4c1ca90eccc8d99366a3dc47cb64e06ad79c36e5`  
		Last Modified: Tue, 01 Mar 2022 06:37:36 GMT  
		Size: 7.8 MB (7834052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf70e03a8272d87e65c7b1592f97f6e739cf1f5d13cc536670f41c28b086b4cb`  
		Last Modified: Tue, 01 Mar 2022 06:37:37 GMT  
		Size: 10.0 MB (9997298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:826ffeb5239c00a6db9fe1d2f27de182887b33d81d938d812814025ce8f9c63c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65219064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7ad2f3e9ada8e2ff12c82d3bb6a8f1cf2a36a2b3b5576a58ba656cadf54bdfc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:03:21 GMT
ADD file:67f3f7e89901c5f16436fda6f05f959b01ce2654ab6b4cd9d53b597d1a30a97d in / 
# Tue, 01 Mar 2022 02:03:23 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:05:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 03:06:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:cce169e928830f476b72f6fb2bd7ce1b80e59d3bd3d24202f5fbd7a9535fd48c`  
		Last Modified: Tue, 01 Mar 2022 02:19:20 GMT  
		Size: 48.2 MB (48154229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d57d0b9b76245f122bedc54cfb401efe4ae73525e3e5096c640b38010ce60e`  
		Last Modified: Tue, 01 Mar 2022 03:27:49 GMT  
		Size: 7.4 MB (7377224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a657cd7a4baa440bfbce8ec469123713e5b5d23c6629f9fa5b6dd0e75ce50d3a`  
		Last Modified: Tue, 01 Mar 2022 03:27:49 GMT  
		Size: 9.7 MB (9687611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:14c05d8cceea4232fa9af570aa1e3ea77c2379040f4a33a2c1046e1d59f8c05d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62387051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8c2c42158d9acdb8e2933cac63f4739892ead8f78be7d290e1ea9ba0c609b87`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:37 GMT
ADD file:4a03c17db3b0f62e4228d270742fc29d7738d7938390f3f96a317cfa94dd4354 in / 
# Wed, 26 Jan 2022 01:42:38 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 16:41:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 16:41:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:09b22b0a561180e2bdd3b51aacb1daa8c81a5d3ae3bf1edc636e4896d4668b6d`  
		Last Modified: Wed, 26 Jan 2022 01:58:45 GMT  
		Size: 45.9 MB (45918112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d93b0047d8edb6abd99a7e540943c9ebe2dc8c1fee8eb533bb41286f1eb3bdd6`  
		Last Modified: Wed, 26 Jan 2022 17:06:58 GMT  
		Size: 7.1 MB (7125198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea2ab6a31c937166c97d4b7a07181dc528a57075a0752ea3acfc5a548a2ef12`  
		Last Modified: Wed, 26 Jan 2022 17:06:58 GMT  
		Size: 9.3 MB (9343741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:97fbc1a4df94d00544e4b3073821126402fe81f77f5df4b9d2a3285f5f377461
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66685453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d047843828d3b039503bb1a1fae2bf26df06cea8ccbf3480e1f9d7262db39f7b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:41 GMT
ADD file:98a75269e438ff15cee16ad2763fe2698fb436bc4770c0ca27c059f66b65e56a in / 
# Wed, 26 Jan 2022 01:42:42 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:14:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:14:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ccd458f933f7966e412773ee1551aaf2433a5bf9adaae519e2ac7c9c3f8b5f89`  
		Last Modified: Wed, 26 Jan 2022 01:49:28 GMT  
		Size: 49.2 MB (49223041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3524e6d2c855bef1f32da73e00738b2e5e91e6a346d19f8b33e8e8117c82748`  
		Last Modified: Wed, 26 Jan 2022 02:25:05 GMT  
		Size: 7.7 MB (7695112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cc9cf00cd9023559aeda43668c7d9d621318631bab103ae03b8a3787260048`  
		Last Modified: Wed, 26 Jan 2022 02:25:05 GMT  
		Size: 9.8 MB (9767300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:65c5b2a74cb9885931274d82458506d6d9e248c9de986d0266d13f4b8a04ed56
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69548204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b1ecaeb57d80945e1bab47a5788e5204f707c1af26d7a3d606ed23ea93f0fd1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:07:47 GMT
ADD file:bdcedc0826a512fa5720a5481555b67977a75cc3a2c76cf5525f4067f6e30f78 in / 
# Tue, 01 Mar 2022 02:07:47 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 05:42:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 05:42:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:476db560471d1237921e304e3ff8f4080b6678e161577b3284ac8cc10eeacb64`  
		Last Modified: Tue, 01 Mar 2022 02:16:20 GMT  
		Size: 51.2 MB (51207695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c26a779ac27dbfd1d496436ab636b45a1a0157570daf0fe074b2b128251084`  
		Last Modified: Tue, 01 Mar 2022 05:53:41 GMT  
		Size: 8.0 MB (8000492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5f554cfd6e25d31263311f533991fee169f308525eac5bfd2a37a744aca5580`  
		Last Modified: Tue, 01 Mar 2022 05:53:41 GMT  
		Size: 10.3 MB (10340017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:dc9608e1dc34a17d16fb2ff589de1a67730eeaa3262a7c5beab7ebfecdc11e7e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66349640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22d78a7ea31890eaf7527d9452fa1bba293c5999eb54a504bdd91255fd8468e9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:03:19 GMT
ADD file:3571860386733ca996c3c4d7a49193aeb8e67693a3d526fceb67acd916ed1d06 in / 
# Tue, 01 Mar 2022 02:03:20 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:08:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 03:08:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:474e1e24c547862b41e95f278b833c2fe32cf9c18a4d6b9d60bb4693d4deabc3`  
		Last Modified: Tue, 01 Mar 2022 02:13:06 GMT  
		Size: 49.1 MB (49079524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92112e67de2237a86e384a0b009d17d7a4bf3303fa948d3204a1069a9625d91`  
		Last Modified: Tue, 01 Mar 2022 03:24:23 GMT  
		Size: 7.3 MB (7253758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e40614a0b9d501b650586d48df88bbe0b9b8c667aa7e9caa3597967c89127e0e`  
		Last Modified: Tue, 01 Mar 2022 03:24:24 GMT  
		Size: 10.0 MB (10016358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:c3c61bed19b3cac958337daefa51a985e6189ba5ac6ff715e0c9ab73b9684e98
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73184338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8d53a946e62918dcaeff9f761276621cbedea82760c60adbbf6ea615dd84654`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:47:14 GMT
ADD file:f61aa5afb284099d49ca76a66b2e84307475d4294dc51c38aa1c0813341b7be1 in / 
# Wed, 26 Jan 2022 01:47:19 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:45:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:46:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a7abba3661dfb8b7aeb8e78fe3fc795e75399c0bebaf594c4b7cd247f031cdf2`  
		Last Modified: Wed, 26 Jan 2022 01:57:52 GMT  
		Size: 54.2 MB (54183703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4633f0f38ce3cdc47cee5a518e174be090163840cc224e2c01665214c477fb75`  
		Last Modified: Wed, 26 Jan 2022 03:21:32 GMT  
		Size: 8.3 MB (8272980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d070427387f273e22519a534d6d5a272f39776edd7d9acb606542383e076cc6`  
		Last Modified: Wed, 26 Jan 2022 03:21:32 GMT  
		Size: 10.7 MB (10727655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:a222286ae81569534f96c88348514ea9871491e794809e16e90089715785ba2d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66289955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecfae99df03e039e6a10746eeca2b3394cffef73f537a698a948e435f289bda3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:02:09 GMT
ADD file:d42860e0eaa59b8efe33f2b9046be595efe776263ed470e4020317e451efbc47 in / 
# Tue, 01 Mar 2022 02:02:11 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:52:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 03:52:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:05bdf937590b731e3ffabc77f5871a8a9c7e597b417485eb87bc8541e791026b`  
		Last Modified: Tue, 01 Mar 2022 02:07:47 GMT  
		Size: 49.0 MB (49005374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb8877d9e145f9b36d4b6ce925bfba017d214117b3a9ffdded7895c9e5f07ad`  
		Last Modified: Tue, 01 Mar 2022 04:00:50 GMT  
		Size: 7.4 MB (7401505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39f0fcec69d1c8fe79f586cfff15fbfb251a666eb3bd6f16ec55c24d4392017`  
		Last Modified: Tue, 01 Mar 2022 04:00:50 GMT  
		Size: 9.9 MB (9883076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
