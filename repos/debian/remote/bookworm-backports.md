## `debian:bookworm-backports`

```console
$ docker pull debian@sha256:b18d3938011b7cb91c757cdaf5960bebb96607383567fe2f466343d267eb6063
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

### `debian:bookworm-backports` - linux; amd64

```console
$ docker pull debian@sha256:8b84df5c20c93d458fdd0856d24e574bf047a1f03a0db020410461d76e41c1a2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.9 MB (52947938 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7f916209f5e61099f9e1c45d1769fbd57d42e562fccfdd0816394ebf32d40da`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:19:50 GMT
ADD file:05d40d360d088a73d2d9ea8361742b3b0e7f5ac80923374f84acf3d1be6c7798 in / 
# Sat, 28 May 2022 01:19:52 GMT
CMD ["bash"]
# Sat, 28 May 2022 01:19:55 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1afe78e67a22dc5c619d5518a1d45e8f5ca31628fa6b7caa3b645c4fba19faaa`  
		Last Modified: Sat, 28 May 2022 01:24:12 GMT  
		Size: 52.9 MB (52947713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e756dadc00874c1e2c949ed2a120a047e1df616007a74cf8ec8e9f36a2efcca8`  
		Last Modified: Sat, 28 May 2022 01:24:21 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:a8501c9515935127315dd8c83a61d3b162f88c0150aceeead01d3fff6b6c87ee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50737662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02ac339cb6aaa786b3a5446a53bc3576375780a2988e5e783b9e73f84dd6890a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 00:49:02 GMT
ADD file:14b16b308b28ed8604a9f98d47e92522f709988224084eb5d2dfd30d3511e4a4 in / 
# Wed, 11 May 2022 00:49:03 GMT
CMD ["bash"]
# Wed, 11 May 2022 00:49:15 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0baf2800ae4e68af843862199b558f14eac2766cea5651c0837cbd8ee827981f`  
		Last Modified: Wed, 11 May 2022 01:03:42 GMT  
		Size: 50.7 MB (50737437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd980aa5c298f4abd497f7d74bcbfaaa37a9105bd53353acd861dfeeac5218e`  
		Last Modified: Wed, 11 May 2022 01:03:53 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:ed3773dcab35f75def51b4576ab98e94eede5bb60e5fba2f28f644a7b02d2efb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.5 MB (48476570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdbdc62a252d0a15231db45518e06bf6670060c2572d762774858e5c9b571f93`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:58:07 GMT
ADD file:8f129729b10afccc69a16674ae2d85afe02706c13f7c3177672040ce01dc34a2 in / 
# Sat, 28 May 2022 00:58:08 GMT
CMD ["bash"]
# Sat, 28 May 2022 00:58:20 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:138713cd49f1253cc6e27f92b0403100f0c5966f7a66077fd4d7c6ab6a6799df`  
		Last Modified: Sat, 28 May 2022 01:13:41 GMT  
		Size: 48.5 MB (48476343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b27bb8d76642db6eee076d0b50eac530fc4a82d291098143d722288ed3230f9`  
		Last Modified: Sat, 28 May 2022 01:13:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:bc37f527b1a8187030b964efba2d2c9cd4889c4ee167edd3627077c38114b0eb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.0 MB (52043016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92423f50980bc3b2085dbb80d2650cebc0605b29e79086c49e000a4c87515a03`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:39:58 GMT
ADD file:ae47b859bfb40c803f02c28e3f96af8bc788772728d65e218948bb1eaad3bde9 in / 
# Sat, 28 May 2022 00:39:59 GMT
CMD ["bash"]
# Sat, 28 May 2022 00:40:06 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f24ab7edee1353b240b401789e816aa26f6557c18b9a3ac7edd79407f8347c7a`  
		Last Modified: Sat, 28 May 2022 00:46:24 GMT  
		Size: 52.0 MB (52042792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ea835d1ed37a70b0e9cdf993aeddf3430a7b1cf8f0589bed0aa41c02f8352d`  
		Last Modified: Sat, 28 May 2022 00:46:35 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; 386

```console
$ docker pull debian@sha256:e109920ba50acfdc9b750abaf21516b3cf1b45e9d0b761a54e5c5ea9ca2176e7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.9 MB (53948711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32d941dd4e1724ff2eaed769c59069b1d6d2646ab96455465b87c30f44935ac2`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:38:49 GMT
ADD file:ba6ab6618a6fab6f0a1d80573b329e26b602c060d940b76c1774ddab96982cd9 in / 
# Sat, 28 May 2022 00:38:51 GMT
CMD ["bash"]
# Sat, 28 May 2022 00:38:57 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d1098d76e3f40923a061abc8c2e6697409b0a2428eab6f37ae394a7b491b1cad`  
		Last Modified: Sat, 28 May 2022 00:45:27 GMT  
		Size: 53.9 MB (53948486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce13680f03715c9981c64d8eb2ea4c1c43c31f39767230d2e896c39754a341ad`  
		Last Modified: Sat, 28 May 2022 00:45:39 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; mips64le

```console
$ docker pull debian@sha256:8d9f579874f1d6d1d7b1e3687e9421c1547385ad95f00aea4bbe8a45a2b637e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.1 MB (52061859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f19d9a4a679994d3e3c1323ac52b20ca7485951e880316dd160e6c86e082e869`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:09:18 GMT
ADD file:0db9365eff38bea353e789709159951d557685e098127d950e467c83468aadd7 in / 
# Sat, 28 May 2022 01:09:23 GMT
CMD ["bash"]
# Sat, 28 May 2022 01:09:42 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:409912beaa99ac80f6ec57bce7ac6621f4659f5f43cdaf3152de94639a634798`  
		Last Modified: Sat, 28 May 2022 01:19:34 GMT  
		Size: 52.1 MB (52061634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75d3a40fdbecff63c4beb672509e324b6a505607c4dfdf02dd1916814675e701`  
		Last Modified: Sat, 28 May 2022 01:19:44 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:8b279a994ab0ce058b3fe8b97ed989bc6468e8d861cc9131181eb5ef6b3f6148
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.2 MB (57161813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98ed173d89a2ba648d5d53a9fa1058dc2a873413062a25808a408c4db502bd78`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:21:20 GMT
ADD file:af4ab80f98b1cc5089a94e2932d676aad92fb52c2f59476cc64955602ea3d330 in / 
# Sat, 28 May 2022 01:21:26 GMT
CMD ["bash"]
# Sat, 28 May 2022 01:21:48 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b80d749a1cbc85d39c24118acb8615cd7c0ba93c2cb7561974f0473b9863a264`  
		Last Modified: Sat, 28 May 2022 01:30:55 GMT  
		Size: 57.2 MB (57161586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee69cb413e115137616d0f02a36cd1a645ab9e964d6fd148bbf1110c153836f3`  
		Last Modified: Sat, 28 May 2022 01:31:08 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; s390x

```console
$ docker pull debian@sha256:99c08719553df4dc5d7f97df9d772109a2b62a6a0b08fe9b0a1c70ccfca50b52
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51490612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5102dc357f1825025a807485a8611005172c47fca0f8427609990f05b6cde6c`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:41:57 GMT
ADD file:4a6691f8332d56b3f631afa5579acf89d2271614f4a4f77baa24e59c0b2b3016 in / 
# Sat, 28 May 2022 00:42:02 GMT
CMD ["bash"]
# Sat, 28 May 2022 00:42:11 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5c219aa5bd4928fd8e410d747805f6d8a6cede332d701af0c9e39dca3b50c70d`  
		Last Modified: Sat, 28 May 2022 00:48:58 GMT  
		Size: 51.5 MB (51490385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ed6e1a8940d378998d7ed515a829e391754cd12cb9397ae431d5d8672700d1`  
		Last Modified: Sat, 28 May 2022 00:49:05 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
