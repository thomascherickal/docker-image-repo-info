## `buildpack-deps:testing-scm`

```console
$ docker pull buildpack-deps@sha256:ccb0a7eb5bc35eb9ee1424a0ebe3ecf742b7ab6115b4d107721e680837701c89
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
$ docker pull buildpack-deps@sha256:4d42e40a5aeebd099a59b9532641fdf18084c0a4e69d7db01872a607322290e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115537221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fd679ec1a51c5e60ec3ef8c9926f411d290f511fd775c27646fe4bb4fadb96f`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 00:58:24 GMT
ADD file:5e17f4d5cdf1ff091554ccfa33e22ab2be0c278b0cec1c11b45333deda2cfc79 in / 
# Sat, 10 Apr 2021 00:58:24 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:01:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:01:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 06:02:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:df95183d3a18fe92c278757657c6fef8fcc11f2a9a578df2f2b00dbccf0a8ea6`  
		Last Modified: Sat, 10 Apr 2021 01:06:36 GMT  
		Size: 50.1 MB (50070347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d156c39bdbf88c4fe691e2b8db9d8884ace98a295e72db7f8f2c7a7b09d88301`  
		Last Modified: Sat, 10 Apr 2021 06:18:29 GMT  
		Size: 4.9 MB (4920554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c5c1a00fb4cd0a81f72ea5458a8eb52ee825d2ec64b5b3d6324e8fe844eed2a`  
		Last Modified: Sat, 10 Apr 2021 06:18:30 GMT  
		Size: 10.2 MB (10218022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88f63a9b9b58ff5c896075723b17ad5cc2bd3e1daada4e1379a89a0b57120ce9`  
		Last Modified: Sat, 10 Apr 2021 06:18:54 GMT  
		Size: 50.3 MB (50328298 bytes)  
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
$ docker pull buildpack-deps@sha256:129ac163986f1d7c1a449d132ba28b99270e0a264a65758d649a386baf118b5c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.6 MB (134649324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a278395be452d203838d7f68ce0976bc81f8f2fd06ed7a50e6fce60c200837da`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 01:24:22 GMT
ADD file:c677239aef001babcb1663e8f2e9aadd81b7da6c581bb55368efc93625140098 in / 
# Sat, 10 Apr 2021 01:24:32 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:54:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:56:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 02:00:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ddef5f25272167da6de06606c43b7762709f7f2d95d2624ba3d2adafbd2d13d5`  
		Last Modified: Sat, 10 Apr 2021 01:32:37 GMT  
		Size: 58.8 MB (58783245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e4e8fb057889bcb16e3c8b7bc0f46ac465eaad43d9ecaee96fe62ecab47f05`  
		Last Modified: Sat, 10 Apr 2021 03:03:04 GMT  
		Size: 5.4 MB (5399544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2dbcd738d9aa03edf4d9d84dad745a9d48e9f2d3eb4febce8ec5aea58e4be58`  
		Last Modified: Sat, 10 Apr 2021 03:03:04 GMT  
		Size: 11.6 MB (11619570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17976d558c617922225b59acaffe6c7bfb5a5777d4e19401af2bbc1479562c32`  
		Last Modified: Sat, 10 Apr 2021 03:03:28 GMT  
		Size: 58.8 MB (58846965 bytes)  
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
