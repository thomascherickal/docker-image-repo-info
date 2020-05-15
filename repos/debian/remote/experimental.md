## `debian:experimental`

```console
$ docker pull debian@sha256:4825ace64c2f2bfd8c3687297af61311da4a3522afa5d1eb50a36db432eaff40
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

### `debian:experimental` - linux; amd64

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

### `debian:experimental` - linux; arm variant v5

```console
$ docker pull debian@sha256:553160de9701152d62830a1eae94d051510ae9544928d71bc12bdf4be8b5b948
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49373220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79348a931e55bc68a47f79f7a554bf58b70d05e187aa5df5012d7704bffe1468`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 22:44:12 GMT
ADD file:86dde72a0ab87a01f23f0bc2339837559b947f3e626920eaad484dbb2c920097 in / 
# Thu, 14 May 2020 22:44:13 GMT
CMD ["bash"]
# Thu, 14 May 2020 22:44:40 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:20f4bc02075b420ec27f08f233c21d9dcd74f712769151e4335502e9da73aafe`  
		Last Modified: Thu, 14 May 2020 22:52:03 GMT  
		Size: 49.4 MB (49372997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:393ad04afc168826c552d8f126cbcb90d6cd2d1f5aeeebee1fea7ae0cffae0cf`  
		Last Modified: Thu, 14 May 2020 22:52:35 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v7

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

### `debian:experimental` - linux; arm64 variant v8

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

### `debian:experimental` - linux; 386

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

### `debian:experimental` - linux; mips64le

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

### `debian:experimental` - linux; ppc64le

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

### `debian:experimental` - linux; s390x

```console
$ docker pull debian@sha256:81826624045efdae4f9a1ebfb34f8cf02b2844029aa63e6ad5393a9cd1674477
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.0 MB (50009218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b6377a7c0d1f020995ea700a961e99dddf5cad3194eaea11f026a6826a603f3`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 23:09:28 GMT
ADD file:da245d4a644af8aa0de81134d0b9b79e7ca32a2e5a0da0f1400f9d49406ff756 in / 
# Thu, 14 May 2020 23:09:31 GMT
CMD ["bash"]
# Thu, 14 May 2020 23:09:50 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:46cb5dbdb9422f82669828fe57d0feb67f9a7457725a4b624517b2aaf6a255ac`  
		Last Modified: Thu, 14 May 2020 23:13:41 GMT  
		Size: 50.0 MB (50008997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59318f7fe6a1db54282384c66be0d6cf6e1bd38d2bde4eac022e6b018d21b49`  
		Last Modified: Thu, 14 May 2020 23:13:55 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
