## `debian:oldstable-backports`

```console
$ docker pull debian@sha256:112d71e7109f8babffe55680e1515acd8e31ad58fa8ffa9059725f884d58ff15
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

### `debian:oldstable-backports` - linux; amd64

```console
$ docker pull debian@sha256:bde4642431cb6c0887dec5d74258f72ca6a0135124114c636f7d54a5bdc1318e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.1 MB (55056924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:486429588c85b5b240b918a7a728c16563854cfd71e1165adc2f3c3abd417855`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 04:56:56 GMT
ADD file:5ddd46193e88de9c4805490b6be8adec88d9fff72c6abdc4180fb2b03d02de64 in / 
# Wed, 20 Sep 2023 04:56:56 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 04:57:00 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c9b646f5dff3118490eab81e47a0b1c7c1f431f0da99a0c786b44c335ebefe95`  
		Last Modified: Wed, 20 Sep 2023 05:02:36 GMT  
		Size: 55.1 MB (55056698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d9b10f01dfece3ede37f62a0c0345afcda139a56d7e2ef4b7d24b2d8eb4a7c`  
		Last Modified: Wed, 20 Sep 2023 05:02:45 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:434160a4e353c6e2c523ce24aadc43af9a65f89fa64cf84e9dbbe0d8b6a35f11
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.6 MB (52563365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:951fc455f579d55b50ce4e9fb6a7ac2eb8d32366cd1b26f09fedf446bd4a17ac`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:38:06 GMT
ADD file:da1ec7816bb4779ff99eeaf749c3b64e98dbb058fb9b388970e70e6f0429ca30 in / 
# Wed, 11 Oct 2023 17:38:07 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:38:09 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:898468ed91f754fb929ec7597c79f49e3b926e76e037a02d099b5efc966c5435`  
		Last Modified: Wed, 11 Oct 2023 17:41:52 GMT  
		Size: 52.6 MB (52563140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4e68980b4aeb49b8ae7026ab17402966f4f0b0559121b1bd110c7d22f0a94b`  
		Last Modified: Wed, 11 Oct 2023 17:42:01 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:cd1ba5f77ca06712bfe9f0906e7d208e03e0e35131bba1dc15751780b5a2fd45
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50215953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee5b6cef0639f2ceecb0ad62bc975a5b3e041521e7e2e2df968947b5563bc44c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:43:15 GMT
ADD file:010bde6be30784c390d5138fd9cd7c469ad66c671eeefeb13c0e3c5186b70d86 in / 
# Wed, 11 Oct 2023 17:43:15 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:43:18 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:cb4669bc4f8e091586991944d88167c76cb15c78accb55788140ac1b9b3250f9`  
		Last Modified: Wed, 11 Oct 2023 17:48:45 GMT  
		Size: 50.2 MB (50215725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e0032f4096be8d6bda80f0f95a994730169e3f77c407258cef3c93419431f7`  
		Last Modified: Wed, 11 Oct 2023 17:48:54 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:c0015d6f7e307abf5e8dbbc0e59256b24225e5a2519b6027d45a10239c6c119a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53705106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d856472b558fc55d617578865a34db42d1fb4bfc86510e7a6a8e9958f6435a3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 02:45:02 GMT
ADD file:d17683ba7f6b9175b6b7355c2a92df3ac32d932885900024a59637e9e84daed8 in / 
# Wed, 20 Sep 2023 02:45:02 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 02:45:05 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0250f3c681d4d2407c6615b27e9cef12ae5c5df4efb11d3c6073565ea79cd584`  
		Last Modified: Wed, 20 Sep 2023 02:49:35 GMT  
		Size: 53.7 MB (53704883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d21f03d83f060d7bd6a6596a5f7cdde8753dd313babc062d554d186fd03e07`  
		Last Modified: Wed, 20 Sep 2023 02:49:43 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:ccffa478aab20cc8e8da61cdfe3993c7b72766e9cdefefd6c777930cb2d58cf9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (56046559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:535940e9176c0ca78db707193f44884f84ffee522881f6df63179818787d91b6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:41:58 GMT
ADD file:fbb4026de842788be138f442c68c97c4cd9f05fbe7e282eb2a1bec5508f411c5 in / 
# Wed, 11 Oct 2023 17:41:59 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:42:02 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a4036d421c6eaaaaafb97abc75064e1210fdd67750a5efbda6e3aa357d14a344`  
		Last Modified: Wed, 11 Oct 2023 17:48:22 GMT  
		Size: 56.0 MB (56046332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80f8954bd43ebf0e9403e42d04fdfcee8637ba2810f0c095aea1c5f54cd1ab6`  
		Last Modified: Wed, 11 Oct 2023 17:48:34 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:b6574b6d93136d6829fa35ac573a2b56466b986cdcc80b6b888e05c6e70e3215
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53289261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8021769bee64a371938659a9cc9397d00da3015118d74f9fc2c655caf0af9ec8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:51:24 GMT
ADD file:ffbea6ab30b7fadd815d53bb877e69b127714ea9976b06db2bc05bec98962215 in / 
# Wed, 11 Oct 2023 17:51:31 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:51:43 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e9dd1c85503ac6114304b94839ac51b6680fe86f0655e8a065dae67b6f39d32c`  
		Last Modified: Wed, 11 Oct 2023 18:02:50 GMT  
		Size: 53.3 MB (53289034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1260349e339ac2822ae504b7ab5a6b0a0dd90ebe629ab4b7884ddc5435527e36`  
		Last Modified: Wed, 11 Oct 2023 18:03:01 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:783b8b3d15434db7e4e3696fa129b7e301a4a7225654a4fb78c5fbc366f8c160
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.9 MB (58929953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0347e5dd70675504cff15050cd94b019a0d6ca9391784948ba1f269e62b706a7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:45:10 GMT
ADD file:47e58d18fb3653863b860db8f28b0e0be7ddb16ba79312033774149e613a2814 in / 
# Wed, 11 Oct 2023 17:45:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:45:17 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:425a16ca69e3109409f9fe8599a7e621808840c05aeddec98718a2a5a38c8258`  
		Last Modified: Wed, 11 Oct 2023 17:51:21 GMT  
		Size: 58.9 MB (58929726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca8b071f6dacc738b58abac73af102a9a8d398625e8ad6ba6e5333cc671a9d9f`  
		Last Modified: Wed, 11 Oct 2023 17:51:33 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; s390x

```console
$ docker pull debian@sha256:17e12bff615831fa340bf347958bd1db78853cee18477d84b65e641f8246b198
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53296560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a63b3495b299326adc0a6f6f9bcc5ee2a9acbdec03d5e7cf42cfab1750dd55d9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:51:11 GMT
ADD file:5c0693dfa39dd52d24f19239d55e43f0d2af245a32ae838ab8f32cf565c738e1 in / 
# Wed, 11 Oct 2023 17:51:15 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:51:21 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:035365d8ea846b3f48e8ae9876bee8e58e3af876d6745beefa24a3ab58db0c74`  
		Last Modified: Wed, 11 Oct 2023 17:58:08 GMT  
		Size: 53.3 MB (53296335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b185611ba09069c6e9b0d304aac44e6f29dc911fc62f50207afe932ab62adf25`  
		Last Modified: Wed, 11 Oct 2023 17:58:27 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
