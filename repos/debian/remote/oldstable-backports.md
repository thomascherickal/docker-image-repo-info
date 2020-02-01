## `debian:oldstable-backports`

```console
$ docker pull debian@sha256:7584027b9322bed839a18c2130e3b1a9460b4846d0c1f3bdbdd6e055e241437b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `debian:oldstable-backports` - linux; amd64

```console
$ docker pull debian@sha256:c7b9e5b7eefd6c702725d544cb90d07e7f81817d218b14954c08b726ec790577
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45380913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b04e80a4fef089ae638cb073a7882f82d8d6d9e3d18c80acb8390dafbcac67f5`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:21:59 GMT
ADD file:6e8067d7c5bc734d5354c805e413e9b3531bbfa7edcf09cf74889d69a9c1b7aa in / 
# Sat, 01 Feb 2020 17:21:59 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:22:03 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:42c5322200e293aefa43d2bf6b2d5a64f5a304852d323a0b7e4f313aa61ce465`  
		Last Modified: Sat, 01 Feb 2020 17:27:28 GMT  
		Size: 45.4 MB (45380686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787677bedd22e975479ece36f4dfd26be10375c38a83257bc371e6142986a506`  
		Last Modified: Sat, 01 Feb 2020 17:27:32 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:293ec0b3a8062377f2a6b0b6f4842c3772a7ffca8a4c37314fe0e062fe42ce9b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44073580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd4f92619705f5636d52eb619ccf2c07a0b8de3a518066eafabd2168d2d1dbfe`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:51:58 GMT
ADD file:88eb6a2e036ee9675ba9e65e679fbe4498013a75a8bdf854c41d913024843e8b in / 
# Sat, 01 Feb 2020 16:51:59 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 16:52:06 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:bf05242add63765c1b791f1875da9e55bf5c7528a9b950bf661e4f991c40a886`  
		Last Modified: Sat, 01 Feb 2020 16:58:47 GMT  
		Size: 44.1 MB (44073355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d365130ae380bc4b1ddc560427de62c0407dd50da57cbea610b6f0be80382f07`  
		Last Modified: Sat, 01 Feb 2020 16:58:53 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:581a9f0221236896d92d9d47f29c71f6437ae56fb223fec363438d11046f6759
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42108543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4ef4938bbf2fb05be9320da022a6611acacc6ef264e06a28f7af4b28d34e4dd`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:02:07 GMT
ADD file:da5b8147307bb96330166bcc3789cef5b43e32f78c07fa38ce29c5fbe30ffdb0 in / 
# Sat, 01 Feb 2020 17:02:09 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:02:18 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f7582a3e720acb71b6bc2309735b30135604ff8fc4ad9027900150ea3ed7ab34`  
		Last Modified: Sat, 01 Feb 2020 17:09:18 GMT  
		Size: 42.1 MB (42108316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6d8f0f705cae1183de1d9eb7de4c0350793a716cdee38129ded5ff16691661`  
		Last Modified: Sat, 01 Feb 2020 17:09:24 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:5c75010ea38a1186531263433c5842b0cbe50f80f0909345bf0bd470d7fb2d34
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43166913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7605c4ca47eeb17efdebd0918e4952593866a5b695709dc3d0e604eb114eea6`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:24 GMT
ADD file:a33bb00e072b52fadbd86b9c212134f038075273127368b7bf4df6bff5d30e61 in / 
# Sat, 01 Feb 2020 16:41:26 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 16:41:32 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b604eb8d5c86debd6cc978e8e37dd21d4cb833841dd775994aeeae65ca1fee4f`  
		Last Modified: Sat, 01 Feb 2020 16:46:46 GMT  
		Size: 43.2 MB (43166686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f5c20819b6d2a294b06d06df3a3f249c7f9d12c75e31eceb0d97dfc5a747d4`  
		Last Modified: Sat, 01 Feb 2020 16:46:52 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:8354eecd9498afd4140baea93a0663b72538993329da777c22deec31a39813ec
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.1 MB (46100270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b4e9bfb8ce7823e640ba2f2bdb9fe0dfd2d73ee816e9864a18c97ce22860d62`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:40:35 GMT
ADD file:498868594ed3d072bc107cdc15170c340b3d9663b9820310fd4e5b3a16c9dd33 in / 
# Sat, 01 Feb 2020 16:40:35 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 16:40:39 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ff1463d4595c84854be86f76adb774bfc18d9674c9ef7d486059b1018f097f97`  
		Last Modified: Sat, 01 Feb 2020 16:45:48 GMT  
		Size: 46.1 MB (46100044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155ada2b9d5e54a411d2c8603ad0a6656b6ed87b1e7ed8d9e8a1a9f153826988`  
		Last Modified: Sat, 01 Feb 2020 16:45:53 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:51482bc99a560e6ddddf51103228391e2223e80ed1fd2b02ca16c589b6b8d0b8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.7 MB (45652525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c0026dd86f98a89742e5eabab80349eb99eee434b9fba1ae574c3767b51b353`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:18:18 GMT
ADD file:24c12c7f45c024e1138996ab61af1c5e2587bb1b331616115d84ac4f35ec9458 in / 
# Sat, 01 Feb 2020 17:18:22 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:18:32 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5528c959a212e9d2a2d5b79cd417ad6498f5313fe82c7f9bb4fc7bf8142da4c2`  
		Last Modified: Sat, 01 Feb 2020 17:26:51 GMT  
		Size: 45.7 MB (45652297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd0d5487d6387d1aec4cafa98d86908b8d0892ed5afbfbe7d3f1b107a93905f`  
		Last Modified: Sat, 01 Feb 2020 17:27:06 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; s390x

```console
$ docker pull debian@sha256:b680c9a914fa3a585aea3d4bfbb7a90b03e7eb6291ac6cecf9121e5e600f05b9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45241864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52b42f64e023d0c9b2b1a3db26375787230933b84f8d9b915371e1cd4d5f9e3c`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:37 GMT
ADD file:8bfbad9a48a3f18a304d25d5fa8b3224f2a57320916b19d28af9937d5097f1e9 in / 
# Sat, 01 Feb 2020 16:42:40 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 16:42:45 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:eede677b74bffafab95c244f1655c2fe397a1ad002f38a6e92195ca310200202`  
		Last Modified: Sat, 01 Feb 2020 16:46:04 GMT  
		Size: 45.2 MB (45241637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff02dd4aa4253fed36dec7e36fcaf2517776728c51975bf009d6b019ccbac8e2`  
		Last Modified: Sat, 01 Feb 2020 16:46:09 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
