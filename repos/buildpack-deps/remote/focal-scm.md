## `buildpack-deps:focal-scm`

```console
$ docker pull buildpack-deps@sha256:4465794cf302f98968f6b677b0a61c97abe78aa1f75135e493c6b614690f6192
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:focal-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:7ad91f5bc79abd012aa84bf3ae64f626eb7eeb8e711e57f9bd2f163d2eac7de6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.7 MB (100683269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc5457e36bff271ad9896846715e324a195c4083d4749034159d0029d47252df`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:06:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:07:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 03:07:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4774ed347ee7aae0f4029cf9fcdc82fb078d2849f5379c2b3cd0d78fac5608ef`  
		Last Modified: Fri, 01 Oct 2021 03:18:54 GMT  
		Size: 7.8 MB (7770752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f807ec5dd5b51b82a425eb00c21aff5367e6944b5d689b16480bb86b55eeba`  
		Last Modified: Fri, 01 Oct 2021 03:18:53 GMT  
		Size: 3.6 MB (3624639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c250b71bd9a093349f8995026b169a3c6ac13ec9deca245d216b4293d68de144`  
		Last Modified: Fri, 01 Oct 2021 03:19:13 GMT  
		Size: 60.7 MB (60718964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:3a61d944bb68e7c20853916e0ebf65b59600c6691ad38bc20026e8860da4a59c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.4 MB (89388833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:768431def83a292eefc32a7aebb536b9aacdd6fb88a516d63ef547131dddadef`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:58:58 GMT
ADD file:17b7faea72ce285877ae2e83ecc15fc88de184361899edfcb561531ea121090b in / 
# Sat, 02 Oct 2021 05:58:59 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:20:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:21:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 02 Oct 2021 22:22:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:29a0bfee4452af9c258710b3049350eec1ed6ee85e33634a638e982934e59d83`  
		Last Modified: Sat, 02 Oct 2021 06:03:00 GMT  
		Size: 24.1 MB (24067218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366ab467c7f452a8e5cb76b5ed3c9cbce43f7cb04f7024c6478ca446f92e399b`  
		Last Modified: Sat, 02 Oct 2021 22:38:21 GMT  
		Size: 6.8 MB (6766828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d36dec707683a0afbc780af0a45ca17744ac7a0f640d578af3195478d90621`  
		Last Modified: Sat, 02 Oct 2021 22:38:18 GMT  
		Size: 3.1 MB (3103932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:035a89a55aa2f31698e17865b0d77f83527531ba06367f3a102622156308cc19`  
		Last Modified: Sat, 02 Oct 2021 22:39:13 GMT  
		Size: 55.5 MB (55450855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:696e75f38cfed35972c462e702a6009c506e6e349401bf8287ab1c1a75bc00a3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99175759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f3c038017047e55e8000b4e31fac47994fdb7740f8bd392338795912c12ca9f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:17:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:17:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 03:17:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689db6ff62963b3e4aae6a2abb554c5d5882b06774174e624ba845094921121b`  
		Last Modified: Fri, 01 Oct 2021 03:25:21 GMT  
		Size: 7.6 MB (7635218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9f06ec2d3b194d9726a65c75b82d7339dc700bc20d923f047e02a735a78925`  
		Last Modified: Fri, 01 Oct 2021 03:25:20 GMT  
		Size: 3.6 MB (3600459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab6b6364c13aa6082dc2050a10d5035c25a02706281100e29c0ad568f624b29`  
		Last Modified: Fri, 01 Oct 2021 03:25:43 GMT  
		Size: 60.8 MB (60767677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:c004774b38314517688fc6d7d94f8e6f42c0a8d1039132f47cc28362ddbcf89a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.9 MB (115861039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d7512b0ae7b5e20b692c2aaddd3902fccd66cca69da3d103fe14b95a702faf7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:10:40 GMT
ADD file:7e5ee5560faaa801aa10a76122190026f8c1da00c809f4fb6ff441751ba0c90f in / 
# Tue, 31 Aug 2021 02:10:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:39:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:40:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:43:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:59390c695558464c51dc1fced64934b549770630192a1639ac6a90f59bd63b13`  
		Last Modified: Tue, 31 Aug 2021 02:14:21 GMT  
		Size: 33.3 MB (33291791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feea9c7aedd6fb1a65cbeb9dbdebba7c78d501eb289eb92d2a11549fdbcac73f`  
		Last Modified: Tue, 31 Aug 2021 05:12:25 GMT  
		Size: 8.7 MB (8725966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c4311ec6f0315cc94b2915046b0ea2dd892eece9196a601d82612067c158282`  
		Last Modified: Tue, 31 Aug 2021 05:11:56 GMT  
		Size: 4.5 MB (4456534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8feb34377851231e9abee7d1f2f04aab8d35c219fec2687aac4046aae381b19e`  
		Last Modified: Tue, 31 Aug 2021 05:14:33 GMT  
		Size: 69.4 MB (69386748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:ab12db445536d99cc55a13c70085c271777f232dfbd09ac2056e5c0c7d30350a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.1 MB (98113036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:403e51f1da78f84c9ef754ad1f475ec1078f576d75597b0aa4b8edb22af9801d`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:28 GMT
ADD file:28b3d1959812d7666f9f73b52562cdaaaf84ff25ce6331995e21c66bb31b0cc2 in / 
# Fri, 01 Oct 2021 01:42:30 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:34:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:34:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 02:35:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:21245da3aae0a4172d9a415c8ba92069601c8a55fc39b783bce7981e97de1b4d`  
		Last Modified: Fri, 01 Oct 2021 01:44:02 GMT  
		Size: 27.1 MB (27122910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6fa25b21a93cb1d9a61a6d35cabe2d161b63a3706869aeb57c0df4be4472b4`  
		Last Modified: Fri, 01 Oct 2021 02:42:05 GMT  
		Size: 7.4 MB (7427440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a836aa79819738132b60bb1aa2d42907d593dc879d3785ca6afff3f6adda654`  
		Last Modified: Fri, 01 Oct 2021 02:42:05 GMT  
		Size: 3.5 MB (3542126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651550a9a41cdd82a572e95f64a221b84cd8e9d72e164544f480714afe537054`  
		Last Modified: Fri, 01 Oct 2021 02:42:21 GMT  
		Size: 60.0 MB (60020560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
