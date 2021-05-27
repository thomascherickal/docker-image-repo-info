## `buildpack-deps:testing-scm`

```console
$ docker pull buildpack-deps@sha256:69dd63e3db932ff79e809d4d7f85abcb3dc5bca9fc4d85ded18efdc375b1ecac
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
$ docker pull buildpack-deps@sha256:1d462b6c035ddfe3bd592df8d589b36cea6e1f5b61252d7b1494554e978d9ab0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.5 MB (125489056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d36be3d61697f89738962d285c274566e25cf7c674a5d1955c5bfc234b09fc0e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:20:32 GMT
ADD file:22ed184e421fcac775f322850c24589ef2e78ddd12900395d44b2ea74220a62e in / 
# Wed, 12 May 2021 01:20:33 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:53:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:53:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 01:54:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ad4592a9cb6deb788f794c7bc60f66d77280e79869f13e9eccbf34e1d381b95d`  
		Last Modified: Wed, 12 May 2021 01:26:05 GMT  
		Size: 54.9 MB (54897696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0031fb5d71ff82041a35e255a3e6fe3156e3cef3d0d931abc81e62f7b82d201`  
		Last Modified: Wed, 12 May 2021 02:03:22 GMT  
		Size: 5.2 MB (5151352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ddda9701dd94c0ff0f3ece18741e2af4430a8892a7688cff39a016e285d2336`  
		Last Modified: Wed, 12 May 2021 02:03:23 GMT  
		Size: 10.9 MB (10870941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e37b3a94cd546f4a71e3987769539535ef64bf39154d5a6f8e3efe65729191`  
		Last Modified: Wed, 12 May 2021 02:03:45 GMT  
		Size: 54.6 MB (54569067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:9f47b049e92d31b99269a9234b64f993d5bf52ae29d164b4ffdcb55cb218ef35
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.4 MB (120387986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f21d16477fd08693c79cefd09c0d30a83eacdcc236accbc511196498951f231e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 00:53:46 GMT
ADD file:776704b0dea7e9c9856d53c5db99eb2cac12414a59e66258c549cd32602f5f15 in / 
# Wed, 12 May 2021 00:53:53 GMT
CMD ["bash"]
# Wed, 12 May 2021 02:23:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 02:23:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 02:24:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4470c8b9361b9718aac07fcf9a711d40000613ef3e0f694e3da9f5ae091dd9ff`  
		Last Modified: Wed, 12 May 2021 01:08:50 GMT  
		Size: 52.4 MB (52439186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407f3f66bf8c38e7c2fdbc8a5310fca072b83a38277249877ea56d98a54ff91c`  
		Last Modified: Wed, 12 May 2021 02:44:15 GMT  
		Size: 5.1 MB (5061779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89a2f4504c44cdbead13c3dd04342bffcfcf5bfdb9bf1284ed5402541ce8374`  
		Last Modified: Wed, 12 May 2021 02:44:16 GMT  
		Size: 10.6 MB (10570303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c15c5aeea0b008ec61592501ad077ab672ac37b69634a7b95e47e710269e02`  
		Last Modified: Wed, 12 May 2021 02:44:45 GMT  
		Size: 52.3 MB (52316718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f429c96be7e11ea8f1c4195a1e769c8a0b7168d0ce24ba6493e3cbdc2e6cad09
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.6 MB (115567499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:703eb101f6bbdbe592de58286bb868712736b5d82ba97c6121256f9ad926244e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:00:23 GMT
ADD file:8ed6f13e7955c981e57f2e063b7bfca16927ded9fed3cbd231923f2fc092555d in / 
# Wed, 12 May 2021 01:00:25 GMT
CMD ["bash"]
# Thu, 27 May 2021 00:37:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 00:37:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 27 May 2021 00:37:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:50de689ded7920797496a1e9f831f07c907224f7c629bb02a03a96ae30d367de`  
		Last Modified: Wed, 12 May 2021 01:18:10 GMT  
		Size: 50.1 MB (50101718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eadd03179b184db82df36753465390a99da5b2ae95dc934fcd05fb8fd8a676b`  
		Last Modified: Thu, 27 May 2021 01:01:22 GMT  
		Size: 4.9 MB (4921246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10155d4071aabcf375a96f3b69b17f5e9cb5e2f69cc8fea2cb2d87c0db3fa24b`  
		Last Modified: Thu, 27 May 2021 01:01:23 GMT  
		Size: 10.2 MB (10216154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:727eafc84335571443c073433335986852106036b472e391f32ef466b7771cf6`  
		Last Modified: Thu, 27 May 2021 01:01:51 GMT  
		Size: 50.3 MB (50328381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d30e6e79d7e99241ee966863c791779ff79ca1855f0ffa7438423af338e0923b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124262568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:748730ed5ce2b9b2b22ae9f4a1860d9c1b9eabbc0c4b197b0650b6f1e372198e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 00:49:45 GMT
ADD file:ebff33fc47ad7105db0adddceb61f0a2042e3c68d687b2d2c7b6b3f500274d6f in / 
# Wed, 12 May 2021 00:49:48 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:30:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:30:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 01:31:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d62e7e7f99652da0bce9de07c43607f6addba9ce6fe0e71326f752a74878fa68`  
		Last Modified: Wed, 12 May 2021 01:01:01 GMT  
		Size: 53.6 MB (53582545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba77e956dd9ad094e794b7ec0ca07641921b539d7baac543574ba9f8bd4be51`  
		Last Modified: Wed, 12 May 2021 01:47:08 GMT  
		Size: 5.1 MB (5140950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d06261b65703cf603f671a504d79710f5533e58af1907bd71dd4e3b21a4728`  
		Last Modified: Wed, 12 May 2021 01:47:09 GMT  
		Size: 10.9 MB (10872118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74967d868a7693d1cb2869c4ef943b2dee969e46bd5e8e834354f59e8cd4f4c`  
		Last Modified: Wed, 12 May 2021 01:47:29 GMT  
		Size: 54.7 MB (54666955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:197bae3925592872ae1e80848408de600adbc68437c7e47397026581f606e1cb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128353025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0042ffdb7d68017fb9d1da27cd563b3e71a5f6ce56dc238fcb36cb68a06a72a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 00:39:01 GMT
ADD file:ceaf0ce8046ef8c7fbc7c677196bc18e90f63d579058f7d2979a7346253dbb7c in / 
# Wed, 12 May 2021 00:39:01 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:07:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:07:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 01:07:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:09ce53911ae087d5d7231ced04f50f7ae7747f7ef80c2d4b4090d0cc6617c7d2`  
		Last Modified: Wed, 12 May 2021 00:45:16 GMT  
		Size: 55.9 MB (55909415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad480fbad30663344721f178f13bba2d278c9bf5a721096d9f7c3a346310b12`  
		Last Modified: Wed, 12 May 2021 01:16:23 GMT  
		Size: 5.3 MB (5280688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff078b1b0b9af70473b6e6fd1bdfe62efc979b863b78619823a6dbbd4b61e06`  
		Last Modified: Wed, 12 May 2021 01:16:23 GMT  
		Size: 11.3 MB (11250145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0224e764554b88c2469161a7ff1fcfd513b955ce520a91bcd5c578f77519e2a1`  
		Last Modified: Wed, 12 May 2021 01:16:52 GMT  
		Size: 55.9 MB (55912777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:ce260eb6a0cee1da0542bed9a04a91dd1ea8c979a5ed5b502719707182bb7076
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.4 MB (122439597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e28a70453ec6a5979bff260a226c2ed641d49c3d068c6832465b9f078e2aa4f3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:08:19 GMT
ADD file:922c33f98e349794ce38a7ac625e9bc65d1f794fd84e1f2ab7c83977a0de89af in / 
# Wed, 12 May 2021 01:08:20 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:53:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:54:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 01:55:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:24f0fe8ca8f36e5a839c5b70a3bbaed367aa46cbcc14b99b83c845ad805743eb`  
		Last Modified: Wed, 12 May 2021 01:14:33 GMT  
		Size: 53.2 MB (53151765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43463951e38d1f2f7a955b8864df761962ff12a9ce6beed73e8467d9ff81a34e`  
		Last Modified: Wed, 12 May 2021 02:06:36 GMT  
		Size: 5.1 MB (5113419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1db96525d02fdd04163b20988d4da3ff43e5e08388959421bdc796e7bcdf467`  
		Last Modified: Wed, 12 May 2021 02:06:39 GMT  
		Size: 10.9 MB (10872828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a3804ae90d53b30290688cea649e0a23024e3083f2a9fb9ff679d2fe7e7a7a`  
		Last Modified: Wed, 12 May 2021 02:07:28 GMT  
		Size: 53.3 MB (53301585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:8982d06da7891d47e78c4c4546b389f2213e13cf365bed4671fb7f3e0c14ebc4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134668498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67e0af692b2336b78406e7bec812aba505c9af12e0c544a7c55d37b5781af056`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:32:59 GMT
ADD file:dd3e802ee39ef6460fa54303399ebc1f08919c4011f872a9ea00cdee78e2e6eb in / 
# Wed, 12 May 2021 01:33:04 GMT
CMD ["bash"]
# Wed, 12 May 2021 03:14:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 03:15:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 03:18:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:79c001f710a199bddecf6231e4c1152e873413174cb20e083729089e3d15e400`  
		Last Modified: Wed, 12 May 2021 01:41:18 GMT  
		Size: 58.8 MB (58795251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c772a696fa0c3a04186486f51e28b635be426e19d28f70066ae4451f4cdffb8e`  
		Last Modified: Wed, 12 May 2021 04:15:48 GMT  
		Size: 5.4 MB (5399466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b13560e5ca42c500abdc25b1eaba62e4eecf6c07847e8a5ada379658a0a0b10`  
		Last Modified: Wed, 12 May 2021 04:15:51 GMT  
		Size: 11.6 MB (11625194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:117e253db3fe4dab977e1e87362629ddef48d98ecbb831fafb78e822287d9cd8`  
		Last Modified: Wed, 12 May 2021 04:16:57 GMT  
		Size: 58.8 MB (58848587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:88e55e48ee8bbbc019b6fcbdaa55a7a68b5f3880f3673fa9d7b286560de5fa97
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.1 MB (123112093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0172b86a1697ed1e5a08bf17e4f62e5e953f2e76fdb9e8e40f40aa884e5e659`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 00:42:28 GMT
ADD file:2c5346f49f9df572a683f8c527b35a6f38363fdcdc3f84dd717e4350111f9062 in / 
# Wed, 12 May 2021 00:42:33 GMT
CMD ["bash"]
# Wed, 12 May 2021 02:19:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 02:20:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 02:20:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:71407cbee72f89deadd67bbdd36cc0d4779120d71ced9bce9ac9372831cbba70`  
		Last Modified: Wed, 12 May 2021 00:47:20 GMT  
		Size: 53.2 MB (53177252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc796f7149a61cfb08cc70634286e2311f092f65388eacf3e95d14e23854d1a4`  
		Last Modified: Wed, 12 May 2021 02:33:44 GMT  
		Size: 5.1 MB (5134521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67c0172c8b410bf031562e86fc13bf225f23f130018bf00ff007c1112aabb47`  
		Last Modified: Wed, 12 May 2021 02:33:45 GMT  
		Size: 10.8 MB (10760156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2972421e23e5e754213d92f166f1cc6b6fab2b18220978dd827f06ad1d80ab`  
		Last Modified: Wed, 12 May 2021 02:34:01 GMT  
		Size: 54.0 MB (54040164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
