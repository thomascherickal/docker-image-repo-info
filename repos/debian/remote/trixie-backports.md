## `debian:trixie-backports`

```console
$ docker pull debian@sha256:60696c112e0cfd9176b07a7b40abe5dd6a7f34096e1bc648213d190d32942af5
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

### `debian:trixie-backports` - linux; amd64

```console
$ docker pull debian@sha256:259fa44d8d662dd38571d125ebbc19013906dedd0bfef64c5abf5e9c5ccb2025
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49514984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6e714484ad17f6c3db573092a3fd18a20f461467541ffe7aa93f417c86cc1c9`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:23:27 GMT
ADD file:34ee641d9bad402a9422c8f96269ac2c74e06369bc362a916c8cdb087156bf70 in / 
# Thu, 07 Sep 2023 00:23:28 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 00:23:32 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e32a7bcba7c1847ff42b03e176da563d6447b045a6f2d5a9ece6acdce60297cc`  
		Last Modified: Thu, 07 Sep 2023 00:30:28 GMT  
		Size: 49.5 MB (49514761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19671cda3819257e821f236a318b8029317bec3f4ab00f5f06597ee42790a259`  
		Last Modified: Thu, 07 Sep 2023 00:30:37 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:7fec2861ba96f461b1a9de4ec2540c1f36e918f9c7ab208e9bc91ab75c275878
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47224288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b4d57b498d475a1f7a2f226d75cd11a401b4299228ebf9cbee69906075f5438`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:49:55 GMT
ADD file:e460e5557be9e7a101d17f1464779b74e918d5484eae72c93315f657014cbcfb in / 
# Thu, 07 Sep 2023 00:49:57 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 00:49:59 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:147684ee075684edef9db37a29f6f4f0713d7a9a164e9e80c3c137d65c34a829`  
		Last Modified: Thu, 07 Sep 2023 00:54:59 GMT  
		Size: 47.2 MB (47224066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a9dd6fb1cf42b89693ee04e58403a7bca9b5e49d24920eb3de92e9ceb595b23`  
		Last Modified: Thu, 07 Sep 2023 00:55:09 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:480a60021ee57ea2d746a3f0fedc46e1a3cd350b774a46280500948f14cb6686
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (45010719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c190965f46ad391a31ac02fef4044f6a9f1b1da69aa6363affd72cc0e1de1c5`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 01:00:27 GMT
ADD file:56aa0cd11d12862eaf421a2ff6a2a518ae07f7d6180a2f0f58a9d10930215950 in / 
# Thu, 07 Sep 2023 01:00:28 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:00:31 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:cbe28254d81156b7683ab6feb96334538a6b59d12717973205a1077d3bcabba5`  
		Last Modified: Thu, 07 Sep 2023 01:06:54 GMT  
		Size: 45.0 MB (45010494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75612bc00e38e620a86bc7f83e39c50acd61e033b88bbe565894514dc82682e`  
		Last Modified: Thu, 07 Sep 2023 01:07:03 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:6cd8cdf5f14afc41624c25d0092b85c79f4dafa5b57876bb4081ef12e929f488
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49445556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc438a54ca46fce1e8053aeb6948d214655bed40b27639c908f41b347a2a0fc6`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:41:23 GMT
ADD file:a310e5bf1552790152899a7201a564545c20b24f32390010fc2f559f8fa49be0 in / 
# Thu, 07 Sep 2023 00:41:23 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 00:41:26 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f494cfd3ac94aec1bba59af935e909f26f6084cbdc423c867e5262b912d699f9`  
		Last Modified: Thu, 07 Sep 2023 00:47:04 GMT  
		Size: 49.4 MB (49445333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a2f165d99ebe9297ea883e367a594ec754889df463677d9665b73d2b11504f`  
		Last Modified: Thu, 07 Sep 2023 00:47:12 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; 386

```console
$ docker pull debian@sha256:2f5d95f2cf441ca4dc7585789558d4f165d69fd5587c4a12ce9a455f1f8d5cce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50534772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0872e0b9c424add32681ef39f565d3ff8fc89e2d2d54a7df9528d8b6733e628`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:41:44 GMT
ADD file:5d53bf28b6cbc8eac8124a07c0bb8e04ee2d0c8989a8b7219612f6ced4f064bc in / 
# Thu, 07 Sep 2023 00:41:45 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 00:41:48 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1e0d37cd24f690f803c53e61b67871ef6d1dd8980331679da74a8059a191a9fa`  
		Last Modified: Thu, 07 Sep 2023 00:49:00 GMT  
		Size: 50.5 MB (50534548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372236cd73ec0e8ed0f2c78979ab15035dcd3484a429af36cd1de37aa792ed10`  
		Last Modified: Thu, 07 Sep 2023 00:49:09 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; mips64le

```console
$ docker pull debian@sha256:fd75b20b33ce3c61e9e00dcdcdfbbc0c700555a43d73a1d7009feb2b3b57a7ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49357733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:420c0e3b3e3eddfaa5f8cf23d9abdfdef7702c48524e17190860c85c32c3d97a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 01:15:52 GMT
ADD file:83fc4a798915040b0cd8aee9a3ff972cb051d033b36a5b578933e29e1b55dc9a in / 
# Thu, 07 Sep 2023 01:15:58 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:16:12 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2b910e4082f491e2e9e9e85a065d99a76c730b5911893631d48aebe5740c1e71`  
		Last Modified: Thu, 07 Sep 2023 01:27:12 GMT  
		Size: 49.4 MB (49357507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b3e6d662e4d850714a68ea7cbbe46bb31e4ee1d67b71e4adfd37f48cb7c38df`  
		Last Modified: Thu, 07 Sep 2023 01:27:22 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:863634a609f64c12275b46cb88c8c93f4c88a7cba13de701c0436694538a1bb7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.5 MB (53456239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f80acf3ce5ed814d9fbcdd7c6ba41b9d27f2743efa5df461c8aaba2b33b2117`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:20:53 GMT
ADD file:1d1937f8a4890754546a2c77f05e3e1d993bb4a60eeb0ed016941880313061ae in / 
# Thu, 07 Sep 2023 00:20:56 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 00:21:01 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:97f3d0760a8a2cb56d7bb85c16a268c56539a98f9e55ebfcfe233a88995c86d9`  
		Last Modified: Thu, 07 Sep 2023 00:27:49 GMT  
		Size: 53.5 MB (53456016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffb718989ef7f449807cef0bbe90fad57e950da7dfcae3fb29597cb361d4123`  
		Last Modified: Thu, 07 Sep 2023 00:27:58 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; s390x

```console
$ docker pull debian@sha256:c742f7d9ce7d7ed93c77f39b8109a7ab3c2096ce7a67a3f7dee239536127f339
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.6 MB (48573972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5eae751da2384cdaae14ea36ac8c24693cdac8bd0c83e8e85204307fc331d4c6`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:47:24 GMT
ADD file:85c1414a9b16cd9b51c31b6e346dff8675b8a78ca36b9b6e41fe6711444ec72a in / 
# Thu, 07 Sep 2023 00:47:27 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 00:47:34 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:020f83d738584194c53a58d8f6c431413868b7fb51d9873c9bc0e26b4292e8cd`  
		Last Modified: Thu, 07 Sep 2023 00:52:16 GMT  
		Size: 48.6 MB (48573746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc32fef2f4d4916b260676588a560c3c19a771525d983dd9b950f463ce63cce2`  
		Last Modified: Thu, 07 Sep 2023 00:52:23 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
