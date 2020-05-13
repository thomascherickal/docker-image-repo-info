## `debian:experimental-20200511`

```console
$ docker pull debian@sha256:19d0007cdd03eb70fc70714ddb897d4d9e721218e7b784a633be3fb8be225609
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

### `debian:experimental-20200511` - linux; amd64

```console
$ docker pull debian@sha256:27f0fd86653b0bb3a2744bdfb909a3789d7ef137993733aed57a164b381a493f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.4 MB (51391170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bba5400875a6a925fb672cc4c52f20bae7f6dcbc052efb7f0a537e120e19a91a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:24:45 GMT
ADD file:4a3ce6e28b74ce2c37d1a283b3b5a52d6754e078dfe7ce5a536dca9801dea0d2 in / 
# Wed, 13 May 2020 21:24:45 GMT
CMD ["bash"]
# Wed, 13 May 2020 21:25:05 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:112696f5bff38e4ee46806902fa2be474354c1abaa6a6ba8f65a49d1aa97f812`  
		Last Modified: Wed, 13 May 2020 21:31:35 GMT  
		Size: 51.4 MB (51390951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f64a88466a51eb217fc60bfebc8e184b655df5479ec05d26295702ec4cc6563`  
		Last Modified: Wed, 13 May 2020 21:31:52 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20200511` - linux; arm variant v5

```console
$ docker pull debian@sha256:f5ab719dc5bcb535b84d1bf77249efc80beb2d840a475f257886c9cb37f84e64
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49359731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8dfdca63947ee7ded96d369a2cb07be91ead6785dd3187aa49d0ecf9ca8f37d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:56:41 GMT
ADD file:aaedc81576841863f768864ab99fd8e46938b134186d2eef36ebcf18b3839312 in / 
# Wed, 13 May 2020 21:56:43 GMT
CMD ["bash"]
# Wed, 13 May 2020 21:57:13 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:51661ac3d1cd00f4be7db3934350a4a73e998e892075c6f2f0ffe7d7bba1ca52`  
		Last Modified: Wed, 13 May 2020 22:04:30 GMT  
		Size: 49.4 MB (49359508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5244e30046ca7b0a83ca5ca0bef411dc3b0f8d44a42a67e4765ebcfe30c9894`  
		Last Modified: Wed, 13 May 2020 22:04:49 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20200511` - linux; arm variant v7

```console
$ docker pull debian@sha256:b1c65c45cbe51b8b6354fbd0aad9725611505cc2d6f02813a83968b5f174102f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47161419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53cbfbff0f9e3ae0cdb94d32acfdeed12acf15546300ec9f6a1515b701968389`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:20:44 GMT
ADD file:3b6b8dd9fe4a90210aefd064ff9295a0ccb81fa41e0e1884a187578c121ba607 in / 
# Wed, 13 May 2020 21:20:48 GMT
CMD ["bash"]
# Wed, 13 May 2020 21:21:17 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:c88ac45bee6ed1ce37ebbfce4905798f0f3dc239af61aeb27e4fb79c243e5e64`  
		Last Modified: Wed, 13 May 2020 21:29:51 GMT  
		Size: 47.2 MB (47161196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dced87d4c3d280f0e2575da5eab8f9f0da9ea332d66aa1815d141695351d7cf`  
		Last Modified: Wed, 13 May 2020 21:30:20 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20200511` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:eeef9e795db00d7143ee9fb2daf3d089dc25487a31d60f39a74dac5bfb23d3bf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50328909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef9cdf53fdec852cd61d69f708041d482849f2da552d1f9032f6abab90d67b72`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:50:13 GMT
ADD file:171e894132b87bcf2948cf6d4009a4055da8efba60fcfc89d9156220f19ad9e1 in / 
# Wed, 13 May 2020 21:50:15 GMT
CMD ["bash"]
# Wed, 13 May 2020 21:51:05 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:16ebee3d16b0ddc93efa379bd168286069e51f46f56519ad6c0978e27e30a543`  
		Last Modified: Wed, 13 May 2020 21:57:22 GMT  
		Size: 50.3 MB (50328687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388a4ceeab63a8de1926afb71badbac3883c94c1f38ca9850150d852b6ae7553`  
		Last Modified: Wed, 13 May 2020 21:57:45 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20200511` - linux; 386

```console
$ docker pull debian@sha256:2dd3290fac835dd5371b7be91cc8c4389eef52ed510d8b7be3dd2eec66b1d24e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52481834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d02e2751d7c53f57a3199929d4df0bd04b2ab97e3f00b10d42e97562cf2f5bd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:43:36 GMT
ADD file:5603e707c482188645031e3aaf992e0b46d1bf8a0a9b40efcda65fa73d601838 in / 
# Wed, 13 May 2020 21:43:36 GMT
CMD ["bash"]
# Wed, 13 May 2020 21:43:56 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:39f7291b6c852d08ea685c0a1956cf268d214782937261b39937ac3fde406ed8`  
		Last Modified: Wed, 13 May 2020 21:51:12 GMT  
		Size: 52.5 MB (52481615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258e6b86790c053637acb0fc93d58bcc65eb769a2ce9457c90bffec78e55cd7f`  
		Last Modified: Wed, 13 May 2020 21:51:29 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20200511` - linux; mips64le

```console
$ docker pull debian@sha256:03d0e0f043093374cb193e433bd2582a04c4f817e55326549df37fe4ba8ccf90
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50132434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e725d0130afb32dc16ad8294aa14011b45a738e4b0465247300af37653d898e5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:54:01 GMT
ADD file:0e892d8398ef551dcc53931d6bf18e38bbb42e1c4bf8bbb14a629bf3b1928dc3 in / 
# Wed, 13 May 2020 22:54:02 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:54:29 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:6d83d488ca1138f3bfdf3aa8f7857fe503c27fc42e640daa18b6df69f246812d`  
		Last Modified: Wed, 13 May 2020 23:05:24 GMT  
		Size: 50.1 MB (50132211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6867872691cb008499da32c9acd6887ab4dc003814893e16ba81d623ca571796`  
		Last Modified: Wed, 13 May 2020 23:06:05 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20200511` - linux; ppc64le

```console
$ docker pull debian@sha256:1b0df8dc27d66d8d88c335fb213db1310cbcf42faa67a706d15a2cdf77bc67fc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.1 MB (55112074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:961716f09839622f0dc56cbc7ef71d243c206ad0829bc34a082e9aa721ed03e5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:49:39 GMT
ADD file:96c446c477820a734d59314710493d0825cafe973ed7ea7a5bc15b41bb7189d9 in / 
# Wed, 13 May 2020 22:49:49 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:54:45 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:cbf71d6a3a102ed468b2b78a0c5fd57091928254edd933a42a11f6d7d866ea0e`  
		Last Modified: Wed, 13 May 2020 23:04:49 GMT  
		Size: 55.1 MB (55111850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faee761aebd762b17ecfd6af9d03f7e4156778056f20fa46ac368fe1d6fa48de`  
		Last Modified: Wed, 13 May 2020 23:05:32 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20200511` - linux; s390x

```console
$ docker pull debian@sha256:65fb2dcf1d5d28c9f4c19e457738c1909a7d6f54650de2ea35aef815a4f72dc9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.0 MB (50002226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfd33fa862f3ae2e018ef69fe8c81178fb9ceb62444c75f63df6125db23ec8f9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:45:22 GMT
ADD file:70201fe502819ff471e290f66527c1f6966d686e6cf5e15c34b34e91f9c371ad in / 
# Wed, 13 May 2020 21:45:24 GMT
CMD ["bash"]
# Wed, 13 May 2020 21:45:43 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:f783b35b669bd4b5a0dcf4a88f1f9f972f96a89ba4b6087493480a1a7cb1270f`  
		Last Modified: Wed, 13 May 2020 21:49:23 GMT  
		Size: 50.0 MB (50002005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e962ac1d72086fea1b66e0245f3ac5eb83aa212fbd41a5ebd4971dcf5c97bb2`  
		Last Modified: Wed, 13 May 2020 21:49:36 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
