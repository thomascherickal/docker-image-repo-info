## `debian:bullseye-backports`

```console
$ docker pull debian@sha256:a35de34ad6ff708338855344d71a7e05461a73d53468354d613d5d9a2dc9e0ac
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

### `debian:bullseye-backports` - linux; amd64

```console
$ docker pull debian@sha256:3813b731782d620697e1815b45f096feb253c913b5cb339ab43af89d33c65983
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.9 MB (54919260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cc00d8598741cc3a578bd846d6935c30d79ee72869a64c12e40d3233a72f9da`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:32 GMT
ADD file:c03517c5ddbed4053165bfdf984b27a006fb5f533ca80b5798232d96df221440 in / 
# Tue, 21 Dec 2021 01:22:32 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:22:36 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0e29546d541cdbd309281d21a73a9d1db78665c1b95b74f32b009e0b77a6e1e3`  
		Last Modified: Tue, 21 Dec 2021 01:27:20 GMT  
		Size: 54.9 MB (54919034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff3659419040c9f9b8f4ff210c67ef83c9d99704a4a0d422292dadf846a2a67`  
		Last Modified: Tue, 21 Dec 2021 01:27:36 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:af8acc33e857f79cf62b9f60ecc29f36bdcd9a21af67ffffa6ef0632562f1388
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52453703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47cc717325e24944c0537ace1801db12b547a44b277ef8fa78817fa594e8e40d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:49:56 GMT
ADD file:db9ed01a72c1fdd649cff18681a13e553381a9aeed4464d65b4dce69c950b543 in / 
# Tue, 21 Dec 2021 01:49:57 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:50:13 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:8ebfd0ce585fe0944cf7cb8bb54f56fc87aedca06647b8c9fdf65292617d7d98`  
		Last Modified: Tue, 21 Dec 2021 02:05:04 GMT  
		Size: 52.5 MB (52453475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3024eb9dc6ded8d3c50d98f369ae300af0583345959a598bd10fa74db40c8e`  
		Last Modified: Tue, 21 Dec 2021 02:05:27 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:b4335a7ff40b2b4b0e6b580926e25c657735475f57490aa5cc99987392e9a856
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50134541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce5c5d5f867b4df3c995144c7a86da528f3bd25b535b4efee21f9bfdfe25643e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 09:04:39 GMT
ADD file:f0d0256a657fcc82cba38ec9fe377ae4d30125de11e0003de81177370592b440 in / 
# Thu, 02 Dec 2021 09:04:40 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 09:04:57 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e704987a22630df63d8518dd22b13ec2a4f460fd492ab42b97cdc6f971e7be31`  
		Last Modified: Thu, 02 Dec 2021 09:20:17 GMT  
		Size: 50.1 MB (50134315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe719d1b6db7d10afce634e574e4939d0b3c87b1b89277ef91880ba585c29e80`  
		Last Modified: Thu, 02 Dec 2021 09:20:40 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:b49e0b83aa8fd4d5e688ba6968910b3c5d7e107e377681fde7b81fb5e68a1384
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53604833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8da3b50cfd2b9198d445664b6f9330c786e7e33f26e6e5efe4bde1535311b9af`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:08 GMT
ADD file:9d88e8701cd12aaee44dac3542cc3e4586f6382541afff76e56e8fb5275387d3 in / 
# Tue, 21 Dec 2021 01:42:09 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:42:16 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:94a23d3cb5be24659b25f17537307e7f568d665244f6a383c1c6e51e31080749`  
		Last Modified: Tue, 21 Dec 2021 01:48:23 GMT  
		Size: 53.6 MB (53604608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba899207e36573632939e9df46c01526e069c5ee0a20abbb70223e1afe272c4`  
		Last Modified: Tue, 21 Dec 2021 01:48:42 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; 386

```console
$ docker pull debian@sha256:a10b7b8e8299afbf277efd78ddd07a5525f9ff78ac2c70905eba1c4da929ddac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.9 MB (55925629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7915cd8b44ddfbd1ed75e74d206b585d744dbcaa2f26d02e8499ce6da6508ba8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:39:40 GMT
ADD file:b77df0839dfb103f5f16329bfa0dcf40c1a73b02e312bb2be40ad620f64e7949 in / 
# Tue, 21 Dec 2021 01:39:44 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:39:54 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c13b09ebb011541c3f3a6e423452bf5046e5ba48dfee18e88cc3e3df477c0baa`  
		Last Modified: Tue, 21 Dec 2021 01:48:09 GMT  
		Size: 55.9 MB (55925399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd91e385b9e55ebf835733f802062400cc88f9b5ceaffff93d8f69040c17a73`  
		Last Modified: Tue, 21 Dec 2021 01:48:30 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; mips64le

```console
$ docker pull debian@sha256:16ee757265c568646c1f883e127e5b4a0944151599a2880ca95cd87cbdb04a23
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53184061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:314b195f138a19ec9cebd9ef233994e9df5bc7e0f65d1257b2814c81baf76e49`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 03:08:44 GMT
ADD file:40dd380a63b1628d2ba96873bcf6a035d95f158325e90ad46ed46a6866f06c36 in / 
# Thu, 02 Dec 2021 03:08:45 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:08:51 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0ddc107271364d08a7f7838aeeb4e5f1381785e292f448280a494b1e02dc4e1d`  
		Last Modified: Thu, 02 Dec 2021 03:17:13 GMT  
		Size: 53.2 MB (53183833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d2a390811e6639ef4708eba78bb0c5df64733354bc82f360d9eac03966acf6`  
		Last Modified: Thu, 02 Dec 2021 03:17:30 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:d6364da0e83d54a52b1d6d14fcd0ecd1d7219e2336783a2f3db093c5e3e114f8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.8 MB (58819818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a276987fe68c98aca09f7871c1cd10ac222b56258fda6203a955d54368d28b2`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 07:20:49 GMT
ADD file:781003f73ff5fb7313d2bd58dc99ae83adc49c419929d32a63c29a9d45b5a554 in / 
# Thu, 02 Dec 2021 07:20:54 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 07:21:09 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6ae53eb717439cac2dd934aaff8829ad7eadd86024d1ea6efc5bcd9ad4291200`  
		Last Modified: Thu, 02 Dec 2021 07:31:08 GMT  
		Size: 58.8 MB (58819590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3948742ebfe5dc0824c2321c78c0c0da57d5e96d40779513ce10532a9b4feea8`  
		Last Modified: Thu, 02 Dec 2021 07:31:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; s390x

```console
$ docker pull debian@sha256:7488a6d1e65e03a33f6a2350692c24856cf2727d78578bc4d0de10ce69f06566
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53194882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80699d7695ebc69c697607d3a9cbc8a4c28c542367ed77222a8758b03dcded8f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:08 GMT
ADD file:9bd51bb5b152533abeecc5a52ab1ef27b6fe2b3be150073d286b50d9c422cfb9 in / 
# Tue, 21 Dec 2021 01:42:11 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:42:19 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:893d9e8a132ef3e4de94156342e290ae15179e3e749ae758ca27bd72cd67b6e1`  
		Last Modified: Tue, 21 Dec 2021 01:47:53 GMT  
		Size: 53.2 MB (53194655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad08010eb9285f99f543e14644a3b360ae979f6d685e88c17a94652e73fce3b`  
		Last Modified: Tue, 21 Dec 2021 01:48:06 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
