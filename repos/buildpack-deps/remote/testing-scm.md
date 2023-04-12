## `buildpack-deps:testing-scm`

```console
$ docker pull buildpack-deps@sha256:907b39297280c3a61968666abca19a4e062b756799e98dd0a89a676b04172ac1
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

### `buildpack-deps:testing-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:9ed3be818675099491b2a9c5066bbd63d5283caa5f3b77d978ea95ecb43f2d61
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.9 MB (133896234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba56358263d5c537ab77ee622af1e53f4ab231c655f7637aa7739d9b469a80da`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:35 GMT
ADD file:1cb6c660a2e3ea14b2a11bb8b80f53920c3da423a0ad7004391bfab4db4d0177 in / 
# Wed, 12 Apr 2023 00:19:36 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:48:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:49:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 07:49:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cc556c281183180fae02d57fa6fb60ed0a99d9040936278743dc4022bfb0c686`  
		Last Modified: Wed, 12 Apr 2023 00:22:48 GMT  
		Size: 49.3 MB (49292938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8022b43d7c31d74c341d297cf10031ff0c51f596473a0c1945ee83a841094638`  
		Last Modified: Wed, 12 Apr 2023 07:56:29 GMT  
		Size: 9.1 MB (9083160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db75f726ec67539c4823cb16851963ebe5838a853b0e769fd662020fad918781`  
		Last Modified: Wed, 12 Apr 2023 07:56:29 GMT  
		Size: 11.4 MB (11422437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8a9e299258b84de99d6d739eb84b5b1632005f9c7723f2dd9e209fb1a8aaa3`  
		Last Modified: Wed, 12 Apr 2023 07:56:46 GMT  
		Size: 64.1 MB (64097699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:344b53de882fcda7c2d453195595144a3c69b6e842ee71d13d6da33ab28ecc50
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.2 MB (129241091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5754c39ab542288953f32e05c79772f7f299ee5ef462be8bd98f34a5d5ae07f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:48:19 GMT
ADD file:df1103dce44baa95c92287ab5016f36d5cc45c6062116ebf5273f7e79a00915c in / 
# Wed, 12 Apr 2023 00:48:20 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:11:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:11:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:12:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:795c0ca2726dffdb0e5ef6ffa341d17ec672d5915011f1a93a05e8c95a4779ae`  
		Last Modified: Wed, 12 Apr 2023 00:50:12 GMT  
		Size: 48.1 MB (48110879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e70c1a23fdf0fd320a61a2506f0ca4a391a319de8403734e4af8d678a6081fc`  
		Last Modified: Wed, 12 Apr 2023 01:20:09 GMT  
		Size: 8.5 MB (8523001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27111cd5fb1057675f2e0b269790dc264d344d6e4b7ad92ff941f90a496167b`  
		Last Modified: Wed, 12 Apr 2023 01:20:09 GMT  
		Size: 11.1 MB (11065924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ed8d7f4b0f78246beda91a51ddbc4ab368fe6f04bb2432498c3f5a76cbc010`  
		Last Modified: Wed, 12 Apr 2023 01:20:30 GMT  
		Size: 61.5 MB (61541287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:b598cfea4a2fdd4babbe11e7f9770817e72eb9f2af57e7f8c34b858af1d56d2e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.0 MB (123989849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:411c875b6d761c0534bb297279832abe2d22d60dd23cd2e13d5d061f524a4799`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 11 Apr 2023 23:59:10 GMT
ADD file:aa1c08333544c05fc5317d775ee99af7479c6fa5f35b74652f6126a7a5099958 in / 
# Tue, 11 Apr 2023 23:59:11 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 09:32:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 09:32:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 09:32:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:81b1dd69f2a38ad14b0919ab9c395aafeb137158539ab6531ac5743690a0ebb7`  
		Last Modified: Wed, 12 Apr 2023 00:02:26 GMT  
		Size: 45.9 MB (45883114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f399f5abf6c810daac72b311feda8726e38c0c228183ccf5d0da4de0b8ec79f4`  
		Last Modified: Wed, 12 Apr 2023 09:43:59 GMT  
		Size: 8.2 MB (8169132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3453014a13bae733f0a1d38594c31a25841303277602f61394efaff085c42288`  
		Last Modified: Wed, 12 Apr 2023 09:43:59 GMT  
		Size: 10.7 MB (10690179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b1d5c89a8ad9820582b69420d902dbb04e78a440ab16e42dd52a5778aea37e4`  
		Last Modified: Wed, 12 Apr 2023 09:44:19 GMT  
		Size: 59.2 MB (59247424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:14fe92b486d2fa872ed5792948ef263bf382710d96156521bba91db6409d8adf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.6 MB (133624598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13f0946fdc4f05c98259e0c4a796a7215b79fdfac56393722a52de699ef3ad2c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:27 GMT
ADD file:efed18ef2a003bff7e64e7049455216e51876402083581032c35085328e416f6 in / 
# Wed, 12 Apr 2023 00:39:28 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:04:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:04:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:04:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b0f987ce91d920ae0a705ed6c9824f1bbbfa282defb8986614030eb8e2bc0b4e`  
		Last Modified: Wed, 12 Apr 2023 00:41:45 GMT  
		Size: 49.3 MB (49345365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e6a618ee06e99ebfbb7809c1cc4902cb717d294243f3765f170fd1c8eaf94a`  
		Last Modified: Wed, 12 Apr 2023 01:12:23 GMT  
		Size: 8.9 MB (8915044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59c3f19470d2fd9e1407a7ddcbac3c316a999a143865347f221db18517e0838`  
		Last Modified: Wed, 12 Apr 2023 01:12:24 GMT  
		Size: 11.4 MB (11389565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b373ae05bf678c385bace283c65197a2bbc2a334c528ed7b58a01d93131de585`  
		Last Modified: Wed, 12 Apr 2023 01:12:39 GMT  
		Size: 64.0 MB (63974624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:1b7217dd58c62e94d4df1bd3fe5e75114d9fdb3da6a3d8338c1e2534008bffce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.4 MB (137369491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ed8865cd6ac62a089861253f45fe5c6131b992aa6d88dd85645089c3f5ada23`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:38:30 GMT
ADD file:7718865253a3489583d40f8c7a7beede0c20cebbab68bb3e97ad2e84082afcb7 in / 
# Wed, 12 Apr 2023 00:38:30 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:02:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:02:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 01:03:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a4ce9e81f634822e5166ef3eef875a4140795ac18afe0391433d72c7865bf67b`  
		Last Modified: Wed, 12 Apr 2023 00:41:43 GMT  
		Size: 50.3 MB (50317977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e54183fe5cb0866f886a93c0d098d38e649286a2b516b64d9658dd40f5d74b`  
		Last Modified: Wed, 12 Apr 2023 01:13:34 GMT  
		Size: 9.3 MB (9264042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76896a8c48193a86329dc809066c177aedc76d55811eb32ca7c80c1ab06f66f1`  
		Last Modified: Wed, 12 Apr 2023 01:13:34 GMT  
		Size: 11.8 MB (11827045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba7e1ed0df9a2a8a6501d91360cea22ab988653bf057d73c44ecb41e49f6151`  
		Last Modified: Wed, 12 Apr 2023 01:13:56 GMT  
		Size: 66.0 MB (65960427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:febd8b1b579bb8f8c6e10e278729e85eedae1a13b46197fcaf699aee460de42a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131823277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f8ca8bc3fe142102f73eaa97cc8abc67f75fa29f8c4f921365762e6e5e75e17`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 05:15:54 GMT
ADD file:454bfcbdd9d738730885002e9124aea5e8eb4920ca5d3bf13bb9f4707023bd67 in / 
# Thu, 23 Mar 2023 05:15:59 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:03:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:04:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 07:05:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70edc5cd98f5a2e589d309248c77122dabf95f437c0448b99513b15ef209f244`  
		Last Modified: Thu, 23 Mar 2023 05:23:55 GMT  
		Size: 49.3 MB (49291654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74250ff8fd2374ebbb2086f535377d5246a78ee51939da5984dc42e7afe6d2f5`  
		Last Modified: Thu, 23 Mar 2023 07:30:58 GMT  
		Size: 8.4 MB (8439840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649c3b2ae326a6eb2a81faaff9322b317ad4788f4c53f6c3b6721724ed9f3d04`  
		Last Modified: Thu, 23 Mar 2023 07:30:58 GMT  
		Size: 11.2 MB (11154181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce72fc6141c1bf4e5dcee62655f6469a6796ecc6186b5f6d227dd67b147c683`  
		Last Modified: Thu, 23 Mar 2023 07:31:48 GMT  
		Size: 62.9 MB (62937602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:ff9ad1cd6f756acfad0e6713004c604f421a818881a59a65cdf72c3ac1f32b42
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.7 MB (144706710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34d4f37092672a6f4eee455d949bb5dc19844135bb11f8290db298507672facf`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:07:22 GMT
ADD file:b747fc06f7ee1d3e19fc9cf3aa83e6ab4caa056a72d230caf616e67849bfe112 in / 
# Wed, 12 Apr 2023 00:07:25 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 09:24:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 09:25:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 09:26:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8314f03b76ec928732612641a4f8420e3c4c25719b48503230bf6c03979aeb2e`  
		Last Modified: Wed, 12 Apr 2023 00:11:50 GMT  
		Size: 53.3 MB (53299984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823af2d3550f6b52577dc50d69a272726b10382b4fae65d06e3b7196165e42d5`  
		Last Modified: Wed, 12 Apr 2023 09:43:31 GMT  
		Size: 9.7 MB (9663796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f73dc4aed694f9f90cd285bb10ed1d4652e9e29ca42e3ae9b7e2148cb39b812`  
		Last Modified: Wed, 12 Apr 2023 09:43:31 GMT  
		Size: 12.2 MB (12184513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1002e389de5d993e4a73f7cf4311d2ac394084c1570912d013506d78ea334895`  
		Last Modified: Wed, 12 Apr 2023 09:43:59 GMT  
		Size: 69.6 MB (69558417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:f1a6a91892b66c97ca28c0d4aa10b5706ce5d49d91fcfb33f33d04a191068ce7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.8 MB (130773785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1798d2a8c091800a97b7795b2e2f35680f165f0a95d7f44b12965f19623788f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 11 Apr 2023 23:59:19 GMT
ADD file:5d2b35b45a0f23e2f2e93f9c311eb34a92e4591ea27979236d801e512d44cb85 in / 
# Tue, 11 Apr 2023 23:59:31 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:24:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:24:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 00:25:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8a09cd2374da8355612e7d4c91d55107a3f089816ae52b2c91b9e08e6a895ab1`  
		Last Modified: Wed, 12 Apr 2023 00:04:39 GMT  
		Size: 47.7 MB (47670407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d047361c12b2aeb253b1923b053dcc960101b3b3348af8f15f95f7fda2b89e4`  
		Last Modified: Wed, 12 Apr 2023 00:32:00 GMT  
		Size: 8.7 MB (8713846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a462d218c24c21390b32ace449f4f47a57624b858dc05a37c31cb7f6e21c41`  
		Last Modified: Wed, 12 Apr 2023 00:32:00 GMT  
		Size: 11.3 MB (11288081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628da1a495c0341f28b24cb228c4984d7d8a718059c95991d67739f4a4602e4b`  
		Last Modified: Wed, 12 Apr 2023 00:32:14 GMT  
		Size: 63.1 MB (63101451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
