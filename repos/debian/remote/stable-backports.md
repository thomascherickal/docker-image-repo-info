## `debian:stable-backports`

```console
$ docker pull debian@sha256:8e3bf962fdc40c014d768d4c92525ebedacca4350cf35657b30b9d7650688356
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
$ docker pull debian@sha256:6ca369829ac04693416b29f1e2c38833d28cfc0e4f160df8a853692e18f30762
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50396138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:332762cbad3b2b27efcded4d27a147d59ca8954dd699f76c6ce0efaef6c8382e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 10 Sep 2020 00:28:58 GMT
ADD file:ac8c004b00b846c70e0c3fea536b0cc5a0937a2a243e58a7f976e25e0c8ac8f6 in / 
# Thu, 10 Sep 2020 00:28:58 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:29:04 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1c2ec57f6e809a5a8cb8436deaa50ee728bb8636363f918f2b03b688d86b8bdd`  
		Last Modified: Thu, 10 Sep 2020 00:36:36 GMT  
		Size: 50.4 MB (50395915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4ed1d4a3df80d18dcf7e080767b9d81123827aa66d37caab18a0d6930df6fd2`  
		Last Modified: Thu, 10 Sep 2020 00:36:56 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:10b3eb76c6bb0a0b34d12b48864cbc37361133bc34b44618a4069163dc67aa95
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48109048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d34e663ba2ef2f608a7f025d94c5a815afe52c01bcdd6fd876399b571736ccd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:57:28 GMT
ADD file:7cfa8b499a5aa63a12d5f28d8d514bbfcf5c1d6c0337d16268573660c7225d36 in / 
# Wed, 09 Sep 2020 23:57:29 GMT
CMD ["bash"]
# Wed, 09 Sep 2020 23:57:37 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4f4b05c6d3fc827d8aaf69e25e815677182776cf17196a89cc6a1efbac58608a`  
		Last Modified: Thu, 10 Sep 2020 00:06:05 GMT  
		Size: 48.1 MB (48108823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47169f5fca4df1fc8fa48abca7aa4da19ae98ca7a982e260f66de72cb0a12fd`  
		Last Modified: Thu, 10 Sep 2020 00:06:13 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:1208e6f1111ba2494ed3d6e37adc9c790f4f21a8abb6db358a59911bcc6c764c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45869524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87bc4c9d504293c0e9b4d73b103cd195296db1c084ce34502c7edfd8285aa440`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 10 Sep 2020 00:12:18 GMT
ADD file:92ecbabfea1e09a6dec1682227c92548b15362d0beb61470ded5f7501a5c1e77 in / 
# Thu, 10 Sep 2020 00:12:20 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:12:29 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:83b6956c0dabd35f252944da2423c440f7e257e05c6697abeb789865f1771e70`  
		Last Modified: Thu, 10 Sep 2020 00:20:37 GMT  
		Size: 45.9 MB (45869298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89caf293a4029566f4cd67f36b7bf0f4ce25a25cfd1e37e48917f95831df2213`  
		Last Modified: Thu, 10 Sep 2020 00:20:44 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:832f7e77d8edae4402e7c28d9ac2afae52c14109aa2c505ff847bc9f80bc74fe
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49175742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc521031da2cd86be86566e16d709e8128aaf71bafa6c3e73136cf62efebe282`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:53:14 GMT
ADD file:8813403f625514e57a7ddfb535c59b5c8bb632bca6e6083740153e79bb823c71 in / 
# Wed, 09 Sep 2020 23:53:24 GMT
CMD ["bash"]
# Wed, 09 Sep 2020 23:53:36 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3f381c302a4e26fc13ce9a484a0412fcb67e6fa5bcda0eb241c36acabb07f943`  
		Last Modified: Thu, 10 Sep 2020 00:00:53 GMT  
		Size: 49.2 MB (49175517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184a62329cf642e2fe96ffa54827b83892d3c15c0d24b260cfcd7ac303d2f49d`  
		Last Modified: Thu, 10 Sep 2020 00:01:01 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; 386

```console
$ docker pull debian@sha256:4b89cc57fc501f5c48223badcd8fea23939bb89d9ccb62a641bce5f59d30875c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51159061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50b3820a92a2c0eb32cdf875e0a55b363d5bdf69302b6a1a63b0f02a55443a3f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:42:53 GMT
ADD file:f53d6d30c5583ebd7cb9f766672adba665371a0b50ca4c8e893fb1dbc4dc1230 in / 
# Wed, 09 Sep 2020 23:42:54 GMT
CMD ["bash"]
# Wed, 09 Sep 2020 23:43:00 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6e1b49f0102f71c537cf980dee0cd10f130f215e1b1e8f8c4ed41051621f4a92`  
		Last Modified: Wed, 09 Sep 2020 23:48:32 GMT  
		Size: 51.2 MB (51158836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e109d306558867d16cbd744d3852eab50447aba21f256569cdc8989c99cc35`  
		Last Modified: Wed, 09 Sep 2020 23:48:35 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:9bb04d30a111d3e859bd96188b75d514eda1d047e9ac8e5337f238c85a03174c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49017427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68ab7fa2aca881391136acd2b69e164ce372f7ee66a18f851e877c4b4c18e4f6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 06:43:32 GMT
ADD file:247bc212623a9a8b4c529b2009a59f5814dea432abd9c1bf7a740350438c5746 in / 
# Tue, 04 Aug 2020 06:43:33 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 06:43:39 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2437a5e79d3b12c528aa02859445b77947c4f28645d91dfe13cef840707eafe8`  
		Last Modified: Tue, 04 Aug 2020 06:50:46 GMT  
		Size: 49.0 MB (49017201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bace872dca909d7f47cb820a928d67cd0315e239d73f5f975832198338dc7d82`  
		Last Modified: Tue, 04 Aug 2020 06:50:57 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:9fc1584d499f087a23085a000a3ceebd60cfe4b5b9d5fe5e80e77b30a9ece7be
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.1 MB (54142899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4d8a60618ae068c213c405ed39348ed4367996520eef73645c567cc465b6639`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 10 Sep 2020 01:12:48 GMT
ADD file:15f2ae61c3ede81266445658025f8a3fedcede47cbe4edf69d9f1bcbfc6a9956 in / 
# Thu, 10 Sep 2020 01:13:01 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 01:13:27 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6f54d1f5e319b13e0551ebcd7777a13d9e19724b15014565cfae5050ee142a4c`  
		Last Modified: Thu, 10 Sep 2020 01:33:22 GMT  
		Size: 54.1 MB (54142675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3d4ea8e9946a7ae66ca055361e4458dc97806c7e32014c2f227bb78c53b98c`  
		Last Modified: Thu, 10 Sep 2020 01:33:37 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; s390x

```console
$ docker pull debian@sha256:2939eb5254547e8764e7f44655c7c1b308dfb98dab0ebed5bc95981ec578093b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48966501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d11528d68293378a3371742c80a8c6b5bd78e0bce651472d557e76ca7337df0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:43:30 GMT
ADD file:5a6265cadb45898fd4e0eb9e317f255b74acfe762909df209b49b068294c10ca in / 
# Wed, 09 Sep 2020 23:43:37 GMT
CMD ["bash"]
# Wed, 09 Sep 2020 23:43:47 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a3726d3830f783b0c0ed7abbbd7efadbb5dee7854adf5bc65f5d6bf42a880960`  
		Last Modified: Wed, 09 Sep 2020 23:47:02 GMT  
		Size: 49.0 MB (48966278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0dd2bbe3a8b173dac7dfbcae7021b6725704140b2c726b0840778594b08508`  
		Last Modified: Wed, 09 Sep 2020 23:47:09 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
