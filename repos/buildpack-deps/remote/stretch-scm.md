## `buildpack-deps:stretch-scm`

```console
$ docker pull buildpack-deps@sha256:db9f26ae1424f4f2bc445293dd0a878e185fb8e432d9179807a04f386ae20253
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

### `buildpack-deps:stretch-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:d11f15aaf173d009e8b4f67e2e42f9412898b4a352aab588b9cfdfedfdffe892
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.5 MB (110547424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ca26fe061c64059423a6cbe0df9841ec5204b0bdb1410468f443c71b40a0c98`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:23:20 GMT
ADD file:6e16bc9cf28c19a1fb1fb516411643e33cbd2bdb7b6c2ce2468c6583c89871a2 in / 
# Tue, 09 Jun 2020 01:23:21 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:56:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:56:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 01:56:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:81fc1918191541a2ffb6ed1cd8386ef8302aea1b0613ebc768a00e76c1f34bb9`  
		Last Modified: Tue, 09 Jun 2020 01:27:59 GMT  
		Size: 45.4 MB (45375796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee49ee6a23d1c7e6b8b574c905dcd4a53efb869a539a957d3e47bc3698f01dc8`  
		Last Modified: Tue, 09 Jun 2020 02:02:39 GMT  
		Size: 10.7 MB (10749020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82851092453815ec861754ded7101fcfa3b648d09a0818ced17ea80478f179a3`  
		Last Modified: Tue, 09 Jun 2020 02:02:38 GMT  
		Size: 4.3 MB (4339890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8f58c4fcca04f9622e97db77618075b618c24a58cce6c6860ca54c9a887745b`  
		Last Modified: Tue, 09 Jun 2020 02:02:52 GMT  
		Size: 50.1 MB (50082718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:cb6b8807673619c1e3d7a2effad482a605a2235106d1f7dda00b8b8a606ef228
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.4 MB (106356238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c15f9ce56fa9449d5b109769d3bd100c827772d48ff8506843828ce2f007ef1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 00:55:26 GMT
ADD file:f75089c5817628b287da52c6067110dff0b6f4efb6fecf5feafa8e2daea1fecf in / 
# Tue, 09 Jun 2020 00:55:29 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:50:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:51:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 01:52:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cc933a187a21289c01459e983ea69dee29bfb61a3aa7a3a8ae010865977afb50`  
		Last Modified: Tue, 09 Jun 2020 01:02:51 GMT  
		Size: 44.1 MB (44069276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68c7016c4c1d54a8db75f1447c8c65687212f5e02de9f8e71e96be5abfb19eb7`  
		Last Modified: Tue, 09 Jun 2020 02:02:28 GMT  
		Size: 9.8 MB (9822538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f44c27923f5148de038dcd58d2b75b2ecca861b7107bfc51bb816b60c3b0f2`  
		Last Modified: Tue, 09 Jun 2020 02:02:27 GMT  
		Size: 4.2 MB (4158984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7ae1f234399a8d90f81be560a4083dd91474c8d9c8e1e1c2b60792951bed5d`  
		Last Modified: Tue, 09 Jun 2020 02:02:52 GMT  
		Size: 48.3 MB (48305440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:99f2a6fe4194dff2952eb21e0fa5efbe34e5028f09b269ce8d5c5ffeb7e21440
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101876969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d93909f13e1ff0344121fd8c1e37c4cc00dbaa39e58701b274c447736546fc7d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:06:07 GMT
ADD file:c0b9ed1244ec0acfc9054c7cb80c768878e3da99740f981ba3a82bdd854305db in / 
# Tue, 09 Jun 2020 01:06:09 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:02:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:02:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:03:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2566ca784846d2d0d4f9105084d94d68d8ea1a82a06a76c5bcd991ce5a10cda1`  
		Last Modified: Tue, 09 Jun 2020 01:13:35 GMT  
		Size: 42.1 MB (42102504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f976b5a12722f5e6e115157695654d36452b713c7fa64a860f8c9e14859402`  
		Last Modified: Tue, 09 Jun 2020 02:15:15 GMT  
		Size: 9.4 MB (9443335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35142ef6ea6c722cd0397799ab151e5da354eabc784b3acef29def7fa34e9bc`  
		Last Modified: Tue, 09 Jun 2020 02:15:13 GMT  
		Size: 3.9 MB (3918433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7773eda6b7a8801a6f09bd4ce443b7e88397ed16265ecd37f55af57db56c4658`  
		Last Modified: Tue, 09 Jun 2020 02:15:36 GMT  
		Size: 46.4 MB (46412697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:35ccdf41c143355950fe74d84d257d52cb8cc8285d3798da6832a5c02c66db80
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (104989571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0b25057bc04a176893c0e590d4cefe90ccea2f36e8d5a52dc88a124e71ca684`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:22 GMT
ADD file:5cbf00485aed776e940988cadfad6853c640c13635ae54fb2b00aafccfe81a73 in / 
# Tue, 09 Jun 2020 01:54:25 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:39:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:39:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:40:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4c4f692ec920eecb1f30d9ef8e50125217decc872d7ada6eeccc36c6dcb49e4d`  
		Last Modified: Tue, 09 Jun 2020 02:00:09 GMT  
		Size: 43.2 MB (43160923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0990c417a21ef9e268cc0822cd23968c4b17cded8170cce0c4d8f7e020e6fd`  
		Last Modified: Tue, 09 Jun 2020 02:50:17 GMT  
		Size: 9.7 MB (9699635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6b83fd41426d182f67fdac882a6bfcd3aad22d7226a653ae58d3046bd46b5e`  
		Last Modified: Tue, 09 Jun 2020 02:50:15 GMT  
		Size: 4.1 MB (4094104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2de3ad924e80f0d130d0bd9ed8ea866eefeb610874bce14fd8347d032772220`  
		Last Modified: Tue, 09 Jun 2020 02:50:36 GMT  
		Size: 48.0 MB (48034909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:4a5bc8a2c945e80c082b2df44d8818c8d708ab4df55ac973b05eec3b3f1c33ea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.0 MB (113044697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f89e3ecfa230ac4ba0af6352ea68f72cedba080178d25e1dc211d22e0f5d0d4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:42:17 GMT
ADD file:6bbeeb0773b96fccb4cd5ba81dd19ec3580f8d8a3cdd3f1d6a3d2b514fbd6eb1 in / 
# Tue, 09 Jun 2020 01:42:18 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:26:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:26:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:27:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9e88f215fab896e3a7d1d2ce75c0d79960b236066e9033b97e76ca7f01ff2fdc`  
		Last Modified: Tue, 09 Jun 2020 01:48:12 GMT  
		Size: 46.1 MB (46094854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1130784446f3179c75741e18b159e7bca5d46db60bb1f9f57d67953023a50899`  
		Last Modified: Tue, 09 Jun 2020 02:37:03 GMT  
		Size: 10.8 MB (10772863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e32fbc0a9c533b460544bce821a796b4f02dd4da61100073a18fba329807ae`  
		Last Modified: Tue, 09 Jun 2020 02:37:01 GMT  
		Size: 4.6 MB (4561121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62e9df71276e8af2305be9b32aca4dd788168bd7fe3c6029ddd8e4e8057f7d33`  
		Last Modified: Tue, 09 Jun 2020 02:37:31 GMT  
		Size: 51.6 MB (51615859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:f5aafa6013a8e32bfaf6d4253abe53479e4f46100ff45a1ddf5e25d4c431f6ce
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.7 MB (108709008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:526f5616b33a756c2c85a5499334d980b301b8622614e8290a516dd11a5fb6ee`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:12:47 GMT
ADD file:de9470ab1a8469c3a824a48056d16d354ec41a887b8b0e6f7b13cedc73a3f316 in / 
# Tue, 09 Jun 2020 01:12:48 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:00:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:01:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:02:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5fdce7db54786a0dce8a238fc9218fa25a9ccc5d0ac32920fd67f03f5571b347`  
		Last Modified: Tue, 09 Jun 2020 01:22:55 GMT  
		Size: 45.0 MB (45049756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffa9955e6182b5a1d2e59bd120f03d4bbf4c0e4c86773a33e7f98fea4f73a0d`  
		Last Modified: Tue, 09 Jun 2020 02:18:06 GMT  
		Size: 9.8 MB (9789501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2d1a085f35901bc4dc96d415aa9abf95233373a94aa4e89e20c50cd9fc6cb1`  
		Last Modified: Tue, 09 Jun 2020 02:18:02 GMT  
		Size: 4.4 MB (4394502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:968e741ea7d876279f8195bfcd9ef6e5eab8463b6e69fb92b9cb61225e843228`  
		Last Modified: Tue, 09 Jun 2020 02:18:56 GMT  
		Size: 49.5 MB (49475249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:29da8a63cf35fa0e373e78683ea697d733d91fc6727c9b28b1183dec703c05ce
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110026709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b93600833a7d838c146a1ad78daf95df52d8d3f9593e8ff62e9848b82c856a8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:39:29 GMT
ADD file:fa4c7e3ca04f092e53cc791a32c929663412df3f68de2733bb867053577bf1d1 in / 
# Wed, 13 May 2020 22:39:34 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:08:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 00:08:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 14 May 2020 00:10:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7732483b686efe14a1cf8add89a1568b83892e243798fba30808f1fc6287210b`  
		Last Modified: Wed, 13 May 2020 23:02:10 GMT  
		Size: 45.6 MB (45646193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df33ef5c6dd4781defd528815174987b67a617a4fbddd5e5241a2f67a34098cb`  
		Last Modified: Thu, 14 May 2020 00:37:47 GMT  
		Size: 10.0 MB (10002565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02507bd450f72bbb529f56f9579bb7169fc9be7900bc5b9b0587e4855e51ad8d`  
		Last Modified: Thu, 14 May 2020 00:37:41 GMT  
		Size: 4.3 MB (4296673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a5abe5a03ebb35ed027af57237427bf1650677f1d4c6a907f88cf889b5e403`  
		Last Modified: Thu, 14 May 2020 00:39:16 GMT  
		Size: 50.1 MB (50081278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:19274ec54033af94340703b565ec1236995f024bcf5e0b13c29a83be08717dae
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.4 MB (110396418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:686bf322e5113d05fce7dc1096eafbf9a9a0f069628ab87a2d563adc6e8f4f9a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:44:05 GMT
ADD file:ce4b8c76522cbe8599502985424901aee9d30d37296761d47dbcb9b0770f7aa2 in / 
# Tue, 09 Jun 2020 01:44:08 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:13:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:13:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:13:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cc8faf537ff83acc994f80bcea99d8e073aa05b5eb0dab5ce495510af0b6d1f6`  
		Last Modified: Tue, 09 Jun 2020 01:47:50 GMT  
		Size: 45.2 MB (45232505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9816eeae17f469b3b58481bdbae04cc1b7b69f8d8a6ef15f6972d91ba2f29ee8`  
		Last Modified: Tue, 09 Jun 2020 02:19:43 GMT  
		Size: 10.3 MB (10280522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a7344ca59dab92a8238f2df0ea3779840ec21afc295e24f39259558c3bfc05`  
		Last Modified: Tue, 09 Jun 2020 02:19:48 GMT  
		Size: 4.4 MB (4372414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a9332093631759dcfd58267f270de204b0c9388802581c972141e78700c0bb`  
		Last Modified: Tue, 09 Jun 2020 02:20:00 GMT  
		Size: 50.5 MB (50510977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
