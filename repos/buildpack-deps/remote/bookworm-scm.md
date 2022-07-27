## `buildpack-deps:bookworm-scm`

```console
$ docker pull buildpack-deps@sha256:81b620666932d93dcd665a1705b08359bbdb3b88eff21b40997461c5b4c1aff0
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

### `buildpack-deps:bookworm-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:407aa0eba6ae8ab6c1602d526a845eb647cf39b63943f66e8d68df575678207d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.3 MB (131308163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e97915d144aa55877f4e59be3be2cd81db23845be81a0a9117c61b779c3059ef`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:19:34 GMT
ADD file:e413c7d61ecdc96ab067e1f8bff6ce03c792c94b9d1f54e80cf633052c5d975a in / 
# Tue, 12 Jul 2022 01:19:35 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:46:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:46:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 02:46:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7c7a32fcf1e30b18b7a9a032acf892763291bef7159859a35297bf81217bbee4`  
		Last Modified: Tue, 12 Jul 2022 01:23:29 GMT  
		Size: 53.0 MB (53022393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00146b6ba9670f0b5362fb1ea6716d934ae0d1545d85efb6e7d9871f449ed7f`  
		Last Modified: Tue, 12 Jul 2022 02:53:57 GMT  
		Size: 9.3 MB (9292245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed5201b04ed0ec80bf5f970e6e10f4e241d58bfbeff69ec15faa4c6a34f01b6`  
		Last Modified: Tue, 12 Jul 2022 02:53:57 GMT  
		Size: 11.3 MB (11271764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0139c5963d20aff0bb13d34b320b3eae3eb708f57b7e951ad4fc79ed5f036b1d`  
		Last Modified: Tue, 12 Jul 2022 02:54:16 GMT  
		Size: 57.7 MB (57721761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:a131970f781d1ddb0999fea53bb5425f92cb250534f557a73c0051fd43150e5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125927054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28e1fd3c8ddff84a6c305c2bb2b8b105b4bc2638e7e64a652c6270cd026076e6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:48:59 GMT
ADD file:211648cfc211d73b6facf8b4f6762e1b45f5894d43880d7bf0a7822be746ad58 in / 
# Tue, 12 Jul 2022 00:49:00 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 01:33:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 01:34:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 01:35:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e06063f979dbe8242191c248c95f1840e27b65404e59a60f54bfc1575fabed87`  
		Last Modified: Tue, 12 Jul 2022 01:00:53 GMT  
		Size: 50.8 MB (50821602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc41e44fbad79261bf0a50b7500c64ccd7e7f8b3209de9bb0165c595e95914f3`  
		Last Modified: Tue, 12 Jul 2022 01:54:32 GMT  
		Size: 8.7 MB (8725587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac530a424b46c790de63a633c7ffebf87465fa20a427e8389d6bcaf6ae81028a`  
		Last Modified: Tue, 12 Jul 2022 01:54:33 GMT  
		Size: 10.9 MB (10940766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb848ce011d9c79c4acecf095c49c232424c8788acd7e3d7e583f7360bbba0a`  
		Last Modified: Tue, 12 Jul 2022 01:55:25 GMT  
		Size: 55.4 MB (55439099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:c8232d52be9963d24a3a8cd0c896b18d49ae4835f2ecfab4543d363d578466d5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.9 MB (120933067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ec7e146c17a06dbd56ecc6298bd43299ae9e154ca86a57996fff5f2b8d16f66`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:58:11 GMT
ADD file:5e1c66e0b3334d725bfb0c7f0d2772c9781b78f01d54756b1924de7abe4abea1 in / 
# Tue, 12 Jul 2022 00:58:12 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 03:24:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 03:24:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 03:25:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:eb8579179b8f8463b05b790bf1566472700d70b08d50d0c6cbc776da788afbb7`  
		Last Modified: Tue, 12 Jul 2022 01:10:35 GMT  
		Size: 48.6 MB (48562934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5ec0a68470d880c05a2e75012ae47d36f57e8e96f491c963000d36a5bd0125`  
		Last Modified: Tue, 12 Jul 2022 03:47:36 GMT  
		Size: 8.4 MB (8405468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b47847e9c4da9d8e5006ac7d60da76d9bf81a4a5b77c355988cbc11285cdbff`  
		Last Modified: Tue, 12 Jul 2022 03:47:35 GMT  
		Size: 10.6 MB (10585664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2997eaa99820702f78e7050d7a4fdb14655a32c7d7a887cac88468e2d2c3ba38`  
		Last Modified: Tue, 12 Jul 2022 03:48:23 GMT  
		Size: 53.4 MB (53379001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c97052b65a60c66cd73b52eccbe406228e332a114b30c63d8913f67296854e3e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.1 MB (130075645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c98c4685144dc459a9eab9ed50197aad0c8d42bbb24eb6340621f850e1cc9d4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:39:53 GMT
ADD file:56a82a6c91d29741aef57453822e5502a13bd7841a1b3c8936a6f7b5c0b80bb6 in / 
# Tue, 12 Jul 2022 00:39:55 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:31:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:31:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 02:32:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:73d3feb17dc47282a9451cf8832ac9c5a707630877cc6c832d9f5cf4d3e2d202`  
		Last Modified: Tue, 12 Jul 2022 00:45:00 GMT  
		Size: 52.1 MB (52128620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3f77295745c94527eef3df84e5f089d7404a40e8f243f00fb8ede9cd04cda4`  
		Last Modified: Tue, 12 Jul 2022 02:41:22 GMT  
		Size: 9.1 MB (9132573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22eb759abcb3de672cf64ccea22ebac1e035560b83ba8bbbd82b3c274ccbbf9e`  
		Last Modified: Tue, 12 Jul 2022 02:41:22 GMT  
		Size: 11.1 MB (11057970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05b5010f809c0bdcab6b0d7f86f07e2ac6b592048be8be96dca5d9a6d1fd281`  
		Last Modified: Tue, 12 Jul 2022 02:41:41 GMT  
		Size: 57.8 MB (57756482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:63110ea353fcfbc269f1a39e4239ad80531a4c156787ba43174963b5d6379680
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.1 MB (134132601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e9c71f198f88ae000fc0d39b9fc12e4b881c5367efa83020faedb54f4966747`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:38:44 GMT
ADD file:80ec0e35d6a4c162afe79f40617b47f846a2eb2065f245a230447609d1e7c001 in / 
# Tue, 12 Jul 2022 00:38:45 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 04:24:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 04:24:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 04:24:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ec7f9e3ed305349e742c012dcd142cce637ef3525759fea18f30c5987bf0e2fe`  
		Last Modified: Tue, 12 Jul 2022 00:44:03 GMT  
		Size: 54.0 MB (54004076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4070b35288ac278d35017570259c20c0599ff1459ee03a4492a44fedae6c68f2`  
		Last Modified: Tue, 12 Jul 2022 04:34:48 GMT  
		Size: 9.5 MB (9465776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:001cac3991e538096035178065ed3abbfbbd6211f5e8284e24b2095d4e30a6a8`  
		Last Modified: Tue, 12 Jul 2022 04:34:48 GMT  
		Size: 11.5 MB (11469705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea864c9108f60f8d724f97dc90852428b5c569b5da71ed5812980449f05c0f5`  
		Last Modified: Tue, 12 Jul 2022 04:35:10 GMT  
		Size: 59.2 MB (59193044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:aa503f373e2d629d3d79a7d0dc2d1ef2ef2307cecd9a329ba8b915a3dbbbd497
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128241956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2df6fd1e8c6bafde37703b4f8104049d498f3616ad436678ef0d9ae8828ded30`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 04:39:09 GMT
ADD file:a4c1c80b05ba336cf2c87e4c90f5bd31ad9a6952b41985b49461741377bdf82f in / 
# Tue, 12 Jul 2022 04:39:13 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 05:59:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 06:00:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 06:02:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d42ff6e50c127c0849c96192832cf954071e1fe597bc69ae0894999838a3d95b`  
		Last Modified: Tue, 12 Jul 2022 04:49:46 GMT  
		Size: 52.1 MB (52148304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6761aa7c460392eac1c72e9e3d658302ae105a69f107d6b7fb8bce7f988b5b`  
		Last Modified: Tue, 12 Jul 2022 06:37:09 GMT  
		Size: 8.7 MB (8657917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b6e4ee7231527a7e9598fb19bb5b34e13789124eaff6a2955f130d363356fb1`  
		Last Modified: Tue, 12 Jul 2022 06:37:09 GMT  
		Size: 11.0 MB (11033071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542574c436d1e1a7fb43145fb5d9e92a5cdb77987eceb090b0ddab0819c83fc3`  
		Last Modified: Tue, 12 Jul 2022 06:37:59 GMT  
		Size: 56.4 MB (56402664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:8c136b486e9cb0e25ccf19892551a0f8ea6a0d78c935ac8d2677c2ea4fa569ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.7 MB (141654047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcaa27f75cdcdf0e1266d527df4570f405e961304caef3f5ecf64f185a05d819`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:24:07 GMT
ADD file:ae1b00e1c53ca0bbd56262f1d2cd742362c7a02eed6214e944b4b4762dda64ff in / 
# Tue, 12 Jul 2022 01:24:11 GMT
CMD ["bash"]
# Tue, 26 Jul 2022 22:27:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 26 Jul 2022 22:28:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 26 Jul 2022 22:28:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8000c6ba1eb02ffb5f03a6b7e7d8f71a864844286f05cb8516ff71014b1cb870`  
		Last Modified: Tue, 12 Jul 2022 01:33:34 GMT  
		Size: 57.2 MB (57237580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40aa4d5388d97e0872477cb7660fbd3c341738064717f187dcfc90f0b64e8e89`  
		Last Modified: Tue, 26 Jul 2022 23:45:55 GMT  
		Size: 9.9 MB (9902776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05727228be0751bdf9f161f49f4edda690903161ccbf1593b8a4a16062ad8ce7`  
		Last Modified: Tue, 26 Jul 2022 23:45:54 GMT  
		Size: 12.1 MB (12082979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a298d404e383284543270c337de3d135d6d054da120136936a43e9d452360a`  
		Last Modified: Tue, 26 Jul 2022 23:46:27 GMT  
		Size: 62.4 MB (62430712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:c676981660dc6e99cf522d158b5cd520c9b481d3305c3436862fe968957105d6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128682149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0d7ce3baea6e4e2ca747d284d56fc5de5af4e8c09e07c188e35fa18796a2177`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:42:21 GMT
ADD file:affba659885c7b0f365e0fe6df963322452d3a11e8c5d1f1d1908cadb57c33eb in / 
# Tue, 12 Jul 2022 00:42:27 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:35:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:35:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 02:36:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4819cb6cd77746b912d22ae402922254d55d38be97967a6c3851624256c8a8cb`  
		Last Modified: Tue, 12 Jul 2022 00:52:08 GMT  
		Size: 51.6 MB (51554170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167df8c8442dcbc38170fd2782ed9a5c4e450b990c5d3f5bc8f1e960393fe12b`  
		Last Modified: Tue, 12 Jul 2022 02:52:43 GMT  
		Size: 8.9 MB (8939224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca0453a18e7c0e72daadbe03c9a6c56fb34dc6db87af258b576918425f6bbef`  
		Last Modified: Tue, 12 Jul 2022 02:52:44 GMT  
		Size: 11.2 MB (11162589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2cd49f61cc74bbef5a3244291e37777a8126bb918492ab42eab831098ef945c`  
		Last Modified: Tue, 12 Jul 2022 02:52:59 GMT  
		Size: 57.0 MB (57026166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
