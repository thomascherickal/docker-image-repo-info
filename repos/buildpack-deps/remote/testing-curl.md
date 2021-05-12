## `buildpack-deps:testing-curl`

```console
$ docker pull buildpack-deps@sha256:abb89703bc25c8645713026ba4c67d6ad8066ba35daeb4f77afdd39c8db5f4e8
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

### `buildpack-deps:testing-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:9a10566b78162fe23500659a58aab24fb7102d8f01db4244cd17b0fcd0a10dd3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.9 MB (70919989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bf3c55eb4d22e0e006f905ae4939a5fe0fbf88199e4e116d4dbf18e28ee61b6`
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

### `buildpack-deps:testing-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:023be4ff25ce84cca5b926c3c741cd6c6115bf258a8414ea448f2bd428f8a373
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68071268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57a1674491c650cc7650accd92263d2e03f4a007edf5a47c4e482022a7febbce`
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

### `buildpack-deps:testing-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:467993d573bdaa4860681a4d23a164133279cbc2bb23e8bed22d72435668a48f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65208923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bc26b1a036b9e96b3d68db0d1e59462f25af4e526eaeaf82eebf61c5751bbf7`
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

### `buildpack-deps:testing-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:40efbfb6eccc0735c5f9e09c325ad83691cd031c2eed6949cf3579b278f54129
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69595613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c63c5abd84285ee7f6d152f3f0cf4adaf6f20e199ceafa7f56f8dff6577332e6`
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

### `buildpack-deps:testing-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:29d08a93906150067a8056aae7966db91fd4e72aac97c73a0b5820a83ab08b62
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.4 MB (72440248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:357793fd9a4739a2c5030f24f6f186643b876e7825749e8f067645f2d562212d`
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

### `buildpack-deps:testing-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:fecf5dcf1a970f6fe0d6d0d13cd5e67252a7f68d126ab31864605a34a71f1ff5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69138012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1fa0b01fd3747657df5ddd9418b2787e9ad9061a32d7916e79d9562754d25a7`
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

### `buildpack-deps:testing-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:7a695c6d7c42b4f52475f6457119a7fafe3c9b516db6fb5d34e739ffd2ec6902
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.8 MB (75802359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d6a8d229c7f6cef8da58fe6f4191533a85693de63ce9b4ffb3612862c809120`
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

### `buildpack-deps:testing-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:e6c1faa355349481075438f24ddb81b016e779f09d0d54d8ef06c577aac12232
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69071929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae7fb004489f27403807977274cd0cf458fd24a5483406baa73ca2b3eff9c783`
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
