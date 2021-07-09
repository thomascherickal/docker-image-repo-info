## `debian:stable-backports`

```console
$ docker pull debian@sha256:6648aa24713c8c5801c5016aa077e807747f25b7aadce1f308b07e8f75314678
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

### `debian:stable-backports` - linux; amd64

```console
$ docker pull debian@sha256:10eb356f218bcaf1702fbd5c4f02618b4337ef471fa6b8b8b1f17420ad53ae7b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50435814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7828e4b11efa0939b769b4ce8369e772cdd6c88df37b44939a4697a84ba1b942`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:21:35 GMT
ADD file:41185c941f63910539569a6cfcdcaf59f0ad79be76b4b715622298cba61e3a84 in / 
# Wed, 23 Jun 2021 00:21:36 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:21:39 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6edcd7ca1d42237759a1ee40df0c1d246a143241d8d9b00047a9954b2e320c80`  
		Last Modified: Wed, 23 Jun 2021 00:27:21 GMT  
		Size: 50.4 MB (50435589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8555db18502ad1378119f46890d694aa07f6831e87da2d140bcb0bf538908dc`  
		Last Modified: Wed, 23 Jun 2021 00:27:31 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:3e9c331f3dc11a47126b6cc399487a373952e0c319186f86d81ffe01c88b1736
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48153907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a88aaa185aac9d7554966fb4c1134d98f807c165d120c1bbe389662800675c73`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:52:00 GMT
ADD file:1d6b6f278e86632d9ad4e6ff24e247607239dae72fce0e5bb27ff7396a64f256 in / 
# Tue, 22 Jun 2021 23:52:02 GMT
CMD ["bash"]
# Tue, 22 Jun 2021 23:52:13 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:172111cdaaab7a9cbef25450adbe2e7b39f9de54d9439f5ce282f159490daca8`  
		Last Modified: Wed, 23 Jun 2021 00:05:05 GMT  
		Size: 48.2 MB (48153683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0a4133c358d888a981fa3358c275277efab0902c0a4f1516ae606fc10489d3`  
		Last Modified: Wed, 23 Jun 2021 00:05:17 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:b75e83ea81f75481368ba530455f0db8f9e50da80011555f84b97aea5a23488e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45917719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22c496cd9417d872fe2af655182c6e0342aa253c7e975c1002f39252071c156e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:22:20 GMT
ADD file:6f3da50b31a89c3c4e712c435d7803c2bb1ea0befd49dba3c34be9449803df0b in / 
# Wed, 23 Jun 2021 00:22:21 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:22:33 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f83f2e6dbc24445b0877f1bd423ba712a70a0927ffca7ae9c75f8f4ca19447a1`  
		Last Modified: Wed, 23 Jun 2021 00:34:58 GMT  
		Size: 45.9 MB (45917495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f71b672c96c975c999d135f78263f7883a9d75d98d5b2a599ba7f73bdc3a17`  
		Last Modified: Wed, 23 Jun 2021 00:35:10 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:548fbbee2b2a4b2891d6bef50a0cb0dfd21f6f3612e01edd7f6aef31b5020beb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49222210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f010153c4a5a4b6970e9387aa4fb72c8c85695894a7a19966dc499590f5ede65`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:32 GMT
ADD file:b7191ce7430d8de72731d617fd845ff6557a0d5cda03f808ec20155ebca26589 in / 
# Tue, 22 Jun 2021 23:50:33 GMT
CMD ["bash"]
# Tue, 22 Jun 2021 23:50:38 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:63a655563c37a127fd9deda43ac0387c29009d5a131bbcc813329f13b111c354`  
		Last Modified: Tue, 22 Jun 2021 23:57:11 GMT  
		Size: 49.2 MB (49221988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3886cc913c4e2d8dcc51f630393a5e3c40ff845168bed5c8ebe8183be6442f`  
		Last Modified: Tue, 22 Jun 2021 23:57:22 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; 386

```console
$ docker pull debian@sha256:e9f93818169abb2a4ee7c600181a1630e203464803eadb7c847e8836c26dddb6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51207311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:636a1067f369359cdd3f890a62969fd223fb5c805179fd95af919872d642fce9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:40:42 GMT
ADD file:848f79fff1c7d691e38b6793b85e872aa483772edd5a57e3d9c8d592695ac510 in / 
# Tue, 22 Jun 2021 23:40:43 GMT
CMD ["bash"]
# Tue, 22 Jun 2021 23:40:49 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:dff37ba8b425454e55a02597e88ed4121dcc1d8f56587645bb5b16cd6e5a5a76`  
		Last Modified: Tue, 22 Jun 2021 23:48:27 GMT  
		Size: 51.2 MB (51207088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af22ff08265cfe3000dca2f03576fa330c4d037bea4c2d4b7b00c21d77f34298`  
		Last Modified: Tue, 22 Jun 2021 23:48:40 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:7ade3e3f0993129018fc5b8a9c363cbccfe95562deff18c8ae798a838c617a55
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49080562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b59fd0c7b77d8281f9f95a39bc30e90ed03b59297cfdfbda9aa0f89f109c8ad1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:10:39 GMT
ADD file:b21b5b26447b31c72e0b0ade460273f6704fa1afb3efc4be3f39dcb1653ac2be in / 
# Wed, 23 Jun 2021 00:10:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:10:46 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c85cd9928c01190c9a8ff2b2c79cd1fa216c36c09a2e9bfea379076b935012a4`  
		Last Modified: Wed, 23 Jun 2021 00:17:48 GMT  
		Size: 49.1 MB (49080337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e339c2e8551a030dd8581dcabfcb3f328cf2cc7e164388ca35bf2611e07b6591`  
		Last Modified: Wed, 23 Jun 2021 00:17:59 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:7e69b245239ba667c0a60ad729ce2b7fd0ffa4d25a9c519630f88d9270de7e91
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.2 MB (54182702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a8b9840c76114227f73026ace7f77e4ed88501ca07cb6d7fdb67ab877f71352`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:31:49 GMT
ADD file:4a65bec5c00bf8d1ddc6fd8b8d51e294b6b6e721ff513b9aa8352f5836f7a92a in / 
# Wed, 23 Jun 2021 00:31:57 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:32:13 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0c31a67cda63a96fa595b136aa0fe10da5dc942fe7100fbbe23b3abd495c291b`  
		Last Modified: Wed, 23 Jun 2021 00:38:13 GMT  
		Size: 54.2 MB (54182477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e943a0c458bbb987c4b8de1b45a464bbc2f83035577d3a4453bb759a644ef7`  
		Last Modified: Wed, 23 Jun 2021 00:38:24 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; s390x

```console
$ docker pull debian@sha256:a3184e35f0a5eb4431756eada672cec169e6564d9c97e87c209eb7c763c94b9c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49004145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c71ff259f155282268dceaf6d92166e21781bb70633f51b851d8c2d6187ef89c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Jul 2021 02:51:13 GMT
ADD file:ce41158759c22931a2226b06f73728349765b0c1462d349840e31af609ab839e in / 
# Fri, 09 Jul 2021 02:51:16 GMT
CMD ["bash"]
# Fri, 09 Jul 2021 02:51:24 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e767eb3772cf8b5212c9ce0829b85eb3551a0e2712fd1e8a654417be36719b0f`  
		Last Modified: Tue, 22 Jun 2021 23:46:21 GMT  
		Size: 49.0 MB (49003920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:971ae1dd8e9b52688e91f1b319ab1db39730e476c5327f15cf6523a1e0ca4fef`  
		Last Modified: Fri, 09 Jul 2021 02:55:38 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
