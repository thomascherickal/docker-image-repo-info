## `debian:oldstable-backports`

```console
$ docker pull debian@sha256:ffd6d060fc2414b3d9b6020aa51b453dd3e49447cef3ace1c12e17a318958a82
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
$ docker pull debian@sha256:fa0fc44f6769657f062a211c90fd2aff6a84f7ea709d7597ade8a8466f1cbbd2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50437374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:689dd8a8c0190098bb69db46a4410ed7f7072026d4b728dbeb3629aa58282f69`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:49:13 GMT
ADD file:727d381013020657d0ea06936e18db69c00d3d7918cc16c77d2cfb6a9ad026ed in / 
# Thu, 02 Dec 2021 02:49:14 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 02:49:18 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c3c495d499fdeac64577c90a02b6f56ffe3bb292a5933eccdecc356592911990`  
		Last Modified: Thu, 02 Dec 2021 02:55:29 GMT  
		Size: 50.4 MB (50437148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716506d5d2e79f47423db32049a2aba0305f4f3efb45ede74c082fe2c3d287ce`  
		Last Modified: Thu, 02 Dec 2021 02:55:38 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:f5bb61ddcaa8f202c63d805c7c2ec0053a8f4e9fdb128b0caa4f31337a419aa1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48154481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e99ec2c79c2a252dd1858213bb53b1b24b76566186fa3ec50e2ec003cf50d20`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:53:27 GMT
ADD file:d8c62c2c6db6ac7253c8966bbab4a452f351083da48bce4e8a7e023d05cb4868 in / 
# Thu, 02 Dec 2021 02:53:28 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 02:53:46 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:9443aed163ada1996b6a4926db892bae972cb41a90eb43fc1aa3e41e548cc6ef`  
		Last Modified: Thu, 02 Dec 2021 03:12:26 GMT  
		Size: 48.2 MB (48154253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039682d56034b43852b6943aa2a09ebc6593128a0a4fb1683cbb8970b46bf437`  
		Last Modified: Thu, 02 Dec 2021 03:12:39 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:ffd3aa9d8303eb40f67646ca91643b82d2ab9b239f07ce815ad06fac846bdfcd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45918373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1280ad4745d8fb8720aa1f1c266566efe211f252eaba1fe5136c4dcd058e3aff`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 09:07:48 GMT
ADD file:d689e3ffbe5a9093757a074e3d1acdb65c85272d0eb78c1aa2e3f06f1851ed3e in / 
# Thu, 02 Dec 2021 09:07:49 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 09:08:03 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:55d0d188b6cef9fa757431d5096d86fdeba0ed57204b92b46b8c5693ed803cf8`  
		Last Modified: Thu, 02 Dec 2021 09:24:17 GMT  
		Size: 45.9 MB (45918145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b6051864e1e88fa4659e2150c64e97542345331c5de08703736519651dd706`  
		Last Modified: Thu, 02 Dec 2021 09:24:29 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:1f7953ebe7207ffb305e6f3638dddfaeb9bd090428d886d879eecfc88bb5294e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49223241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e337e3fc0437ffc9122fd2ac344a28c22dd4d92201bfbebf2a130a8f464967e4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 08:09:07 GMT
ADD file:9265461c71d8020fccde00a7f028b5c68a98ea40c006b7d3b4194a5b79b65cf8 in / 
# Thu, 02 Dec 2021 08:09:08 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 08:09:13 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ea88d642ca215518972db1cb023909e2bc60c764d12130c1cfb58c3bf9eda4a5`  
		Last Modified: Thu, 02 Dec 2021 08:42:38 GMT  
		Size: 49.2 MB (49223015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994bac4260d95b8f8e8f4435529ce954c83ea9d92e590a35776a616f45220f74`  
		Last Modified: Thu, 02 Dec 2021 08:42:48 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:a354c1cf38d2aea5506af93c882c00fd5c75ba648bd971a02bc37525d37f98c2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51207920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9aa6c3913b62d21f5f9bb3881836fce20e3cccd99e3cc2b652c14d12d9d49c7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:41:05 GMT
ADD file:6b57ce5fa1d11564a26e5ab54847764d46fe0883cfac29e2307148381922aeda in / 
# Thu, 02 Dec 2021 02:41:06 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 02:41:12 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3183e716e1ddb8ec3eed0a1203242019e72c30039c8a85751a3cc0b7d4904eb9`  
		Last Modified: Thu, 02 Dec 2021 02:50:17 GMT  
		Size: 51.2 MB (51207693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81bed7be1fce687f992c3b7979323d56e76a6767c4e0cb13560396b3c19608e`  
		Last Modified: Thu, 02 Dec 2021 02:50:28 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:75be13bd9520041c3eaec40e3f572a3f4769e471f85de9fa6ca58541fc658263
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49079728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:239ac22140d20d190e15da35e966cbf4de02e4b5f32a553a4edcc89a822f9a6b`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 03:10:30 GMT
ADD file:051ec5dbe3f56d986bb36a6fe098d9d6151ddb551084397500a4a4dca3251734 in / 
# Thu, 02 Dec 2021 03:10:31 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:10:39 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:40aa185b5b46f05f565b33bb29719a5397bd901481c4197dc2bf0dad30b6e898`  
		Last Modified: Thu, 02 Dec 2021 03:20:06 GMT  
		Size: 49.1 MB (49079501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ba36d7997ef6c5662337196087ce175f37fce8b8bf0ba45fdeb2dec8f84961`  
		Last Modified: Thu, 02 Dec 2021 03:20:16 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:25bbea59e568d57f820a1019a53af009435dc5f869aff6753f5037aff7a14cd6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.2 MB (54184024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fd601da654041d2569905fc3bce556389d948132c00615962ab226dbfb85c27`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 07:22:34 GMT
ADD file:5e7326e39d36f27614697f320d418f06a9752f32126bbb2340960d01470a974f in / 
# Thu, 02 Dec 2021 07:22:42 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 07:22:56 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:15873646b07eef157f2a4878c244f2cae2dbaffc11d4dee6f73d2eed62bb3e1c`  
		Last Modified: Thu, 02 Dec 2021 07:33:08 GMT  
		Size: 54.2 MB (54183798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497bb367449c5142ceb23a5e6c7f3c3fdc742e122bfc70833cb6288ccc8b0fd0`  
		Last Modified: Thu, 02 Dec 2021 07:33:20 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; s390x

```console
$ docker pull debian@sha256:5f1b3b5cc89dbef289d906ee5fce7dd2a20689e096dc495520a9d0ae391f509c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49005702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9afc7327a9e4589f9123e42a37aa81b7422bbf14bbc677d16debb3fb54d25168`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 07:19:54 GMT
ADD file:a0a3bc8e7d6fbffb5878126ad10898698b2da0a375bd440cf84c12957fc7de02 in / 
# Thu, 02 Dec 2021 07:19:58 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 07:20:06 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6a8878fd7892d788226602917026282869ad6674949c96abf3f4c0881606b786`  
		Last Modified: Thu, 02 Dec 2021 07:26:02 GMT  
		Size: 49.0 MB (49005475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64bdce72218de24254065d2392727f3929fe305266543a1a839106645a0f61d`  
		Last Modified: Thu, 02 Dec 2021 07:26:09 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
