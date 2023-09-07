## `buildpack-deps:trixie-scm`

```console
$ docker pull buildpack-deps@sha256:4818a58595e74e7173e0d7c99beb1cd29079a9e62a4c1b2245e7637a3833c96a
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

### `buildpack-deps:trixie-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:a4dfd87847d6fa84c5002afc1b5768b7ba8b174e016e35eb542a49b14c029fed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.4 MB (134448146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6de79ce7ae844b70a9cf5b602b3104534e1ebded6dfafe47c136bdd6449991e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:23:27 GMT
ADD file:34ee641d9bad402a9422c8f96269ac2c74e06369bc362a916c8cdb087156bf70 in / 
# Thu, 07 Sep 2023 00:23:28 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:02:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:02:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e32a7bcba7c1847ff42b03e176da563d6447b045a6f2d5a9ece6acdce60297cc`  
		Last Modified: Thu, 07 Sep 2023 00:30:28 GMT  
		Size: 49.5 MB (49514761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df261e695bd837ce65c269e99eb1a12049f82c345fa073f411be6c5b6d7d3b75`  
		Last Modified: Thu, 07 Sep 2023 03:09:01 GMT  
		Size: 20.3 MB (20254789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54069e7c97fd71d1911c5424269e3102695ad98bc0a3de4b91415dc3e80fb6c3`  
		Last Modified: Thu, 07 Sep 2023 03:09:18 GMT  
		Size: 64.7 MB (64678596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:f0c79b171b9e8cf0e7b87a63c7eb6d32a11a6429a641d7e80f9e96647303de17
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128884495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:764f7539513208aabe38c178e159fe7a812827bdb28d4e7b14e2aab1576ad815`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:49:55 GMT
ADD file:e460e5557be9e7a101d17f1464779b74e918d5484eae72c93315f657014cbcfb in / 
# Thu, 07 Sep 2023 00:49:57 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:22:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 06:23:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:147684ee075684edef9db37a29f6f4f0713d7a9a164e9e80c3c137d65c34a829`  
		Last Modified: Thu, 07 Sep 2023 00:54:59 GMT  
		Size: 47.2 MB (47224066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a7afb82f9e4205f57e955251cf5cbe9dcdaca025f970b69ebaab4b9eed8a9e5`  
		Last Modified: Thu, 07 Sep 2023 06:28:11 GMT  
		Size: 19.3 MB (19333044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af04160cd2b511280308a841f3ca14519a2fce152c8c2a0afcf50f3744245541`  
		Last Modified: Thu, 07 Sep 2023 06:28:31 GMT  
		Size: 62.3 MB (62327385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f33c8e96705c40209ee56dd09395a9ecb5b713a223dad78a41f6dc954a02c144
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.6 MB (123566268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4c450fc305174f9eb7d21e13717c1d3512ed305729d8775f1410a84fdab7814`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 01:00:27 GMT
ADD file:56aa0cd11d12862eaf421a2ff6a2a518ae07f7d6180a2f0f58a9d10930215950 in / 
# Thu, 07 Sep 2023 01:00:28 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:42:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:42:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cbe28254d81156b7683ab6feb96334538a6b59d12717973205a1077d3bcabba5`  
		Last Modified: Thu, 07 Sep 2023 01:06:54 GMT  
		Size: 45.0 MB (45010494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfbe3001385a2b717c083b0eb81363b8210958afe6ccf0dfe6a62a78df022ec5`  
		Last Modified: Thu, 07 Sep 2023 01:49:25 GMT  
		Size: 18.6 MB (18600941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39960ddda116bc7eddff9010f7bdc11c97332a0ea990a5a7e825d0cdcc2868a`  
		Last Modified: Thu, 07 Sep 2023 01:49:43 GMT  
		Size: 60.0 MB (59954833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d86378cce7cdaeba687c8488c44377b78bc429f5829d0340719faaed95806d4c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.2 MB (134163315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0246e821dcc93738e054fb02bad3e7e6975f7621e6b30e975648587290858ad4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:41:23 GMT
ADD file:a310e5bf1552790152899a7201a564545c20b24f32390010fc2f559f8fa49be0 in / 
# Thu, 07 Sep 2023 00:41:23 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:57:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 06:57:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f494cfd3ac94aec1bba59af935e909f26f6084cbdc423c867e5262b912d699f9`  
		Last Modified: Thu, 07 Sep 2023 00:47:04 GMT  
		Size: 49.4 MB (49445333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d75a1727c91eb5f86c6a99848305fb36072ff8bddf6c097df4ebcaa0486e22c`  
		Last Modified: Thu, 07 Sep 2023 07:02:58 GMT  
		Size: 20.0 MB (20039341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8512e1c04bd8db95cd7d2018336279a792f1ab604ba18e01bdb5f8615fa16e53`  
		Last Modified: Thu, 07 Sep 2023 07:03:14 GMT  
		Size: 64.7 MB (64678641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:31878c48a551e60acfe2aa68406016be01f64a82e69b53d72d0ee701a6f32cbe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.9 MB (137871241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22a958d70d6528e570ffe292108ab492680225ccec8f02c354a108b0551e4342`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:41:44 GMT
ADD file:5d53bf28b6cbc8eac8124a07c0bb8e04ee2d0c8989a8b7219612f6ced4f064bc in / 
# Thu, 07 Sep 2023 00:41:45 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 05:35:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 05:35:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1e0d37cd24f690f803c53e61b67871ef6d1dd8980331679da74a8059a191a9fa`  
		Last Modified: Thu, 07 Sep 2023 00:49:00 GMT  
		Size: 50.5 MB (50534548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62b76d6a16699dd100cc2549b60405a4d0d78dc30f81cc263bee0da056e922a5`  
		Last Modified: Thu, 07 Sep 2023 05:42:45 GMT  
		Size: 20.8 MB (20840661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc12640afdfa7cf01b8781ab7883502fe26134031f798e3a1391eb3c53ff9125`  
		Last Modified: Thu, 07 Sep 2023 05:43:08 GMT  
		Size: 66.5 MB (66496032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:046462eed28745d1caadd54b9dda3bc4b442d35bbd759eb1657dcacd290ea312
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.5 MB (132549205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b26e1bffc8263b56c40daf67e3080482d2c74fb716bd092b220df4286228a706`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 01:15:52 GMT
ADD file:83fc4a798915040b0cd8aee9a3ff972cb051d033b36a5b578933e29e1b55dc9a in / 
# Thu, 07 Sep 2023 01:15:58 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 04:11:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 04:13:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2b910e4082f491e2e9e9e85a065d99a76c730b5911893631d48aebe5740c1e71`  
		Last Modified: Thu, 07 Sep 2023 01:27:12 GMT  
		Size: 49.4 MB (49357507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f9d654b3c49c164cc43a4683b85bf2e1374ecf02ddb2c3f7187cfd204ec3309`  
		Last Modified: Thu, 07 Sep 2023 04:30:10 GMT  
		Size: 19.6 MB (19559687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8decd0a052b38d92ca1b1753f6ddbe6c1df433473ed31f5705fe4bb91479355`  
		Last Modified: Thu, 07 Sep 2023 04:31:01 GMT  
		Size: 63.6 MB (63632011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:8b8a2bc2859573226daefa65eedad79ab9c3bcb0284bd54249d4f5b8ca99e02f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.2 MB (145218490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7144a908bc8439cdb740db09dcb1f031f3aa7c7172e1349601e1ed67b2bb17a1`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:20:53 GMT
ADD file:1d1937f8a4890754546a2c77f05e3e1d993bb4a60eeb0ed016941880313061ae in / 
# Thu, 07 Sep 2023 00:20:56 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 09:37:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 09:38:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:97f3d0760a8a2cb56d7bb85c16a268c56539a98f9e55ebfcfe233a88995c86d9`  
		Last Modified: Thu, 07 Sep 2023 00:27:49 GMT  
		Size: 53.5 MB (53456016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c02194f17d80e36f8422769cee8ff8b9736cebe272d97a858855044f7884c65b`  
		Last Modified: Thu, 07 Sep 2023 09:48:05 GMT  
		Size: 21.6 MB (21604788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3bf662e8f630cc6de0c1ac5e5a0e937ce4eb87519569ce27f0bcc6b3984abfc`  
		Last Modified: Thu, 07 Sep 2023 09:48:33 GMT  
		Size: 70.2 MB (70157686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:3153912f470e6f219f1573347037607b8e81fbccebee62687e23ca51e0e949f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.6 MB (132592718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bb32cd1818329edfddb10d6ffbe980fc8bb2beb29bed3e7c591f60dd2ba2689`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:47:24 GMT
ADD file:85c1414a9b16cd9b51c31b6e346dff8675b8a78ca36b9b6e41fe6711444ec72a in / 
# Thu, 07 Sep 2023 00:47:27 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:16:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:16:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:020f83d738584194c53a58d8f6c431413868b7fb51d9873c9bc0e26b4292e8cd`  
		Last Modified: Thu, 07 Sep 2023 00:52:16 GMT  
		Size: 48.6 MB (48573746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c6a12ceebdf73872641b973e28cbc96d9146f8098bfd6cd4d37ad06255121c`  
		Last Modified: Thu, 07 Sep 2023 01:24:56 GMT  
		Size: 19.9 MB (19925579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fb9a0498809282410280aaa414903e32de7d35875c64b8c0cf8bbd99ad0d45a`  
		Last Modified: Thu, 07 Sep 2023 01:25:12 GMT  
		Size: 64.1 MB (64093393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
