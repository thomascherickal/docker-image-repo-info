## `buildpack-deps:testing-scm`

```console
$ docker pull buildpack-deps@sha256:c9ebde16fdfd7ad045adf9d650621fd72bccdbaff656e25b8cd17c098f04b26a
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
$ docker pull buildpack-deps@sha256:000ac73bce79972e52d53c962a31162be24fdc559f0538904ee6a0150d222c68
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.8 MB (130843993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7945f5e0e10aedb5f27374316d0f3c7b5531582fae4f0662e75f879cc562a3f4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:03 GMT
ADD file:ca5a5911d0951e5c75f1790eb644a6fd41dcb9712fa2af0fb6d3a537a72e6ad8 in / 
# Tue, 04 Oct 2022 23:26:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:52:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:52:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:52:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6674a3ae4f8f54c2f747bad2069e50ce00e352d650887729310d984cebecea22`  
		Last Modified: Tue, 04 Oct 2022 23:29:50 GMT  
		Size: 53.0 MB (52962415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e064222ce493e48ae4ceac8f18316e08d2afb963ad57bd63b8630a0ae009f8`  
		Last Modified: Wed, 05 Oct 2022 01:18:07 GMT  
		Size: 9.3 MB (9298646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab229472e3a483409ce2bbc4d461fc6512c03c687daf6546b52705bc7f18961`  
		Last Modified: Wed, 05 Oct 2022 01:18:08 GMT  
		Size: 11.4 MB (11381655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93a5a87ebbd4472db252972521c82b5789bcc45b6bf1ff4d5e59ab129a4847a`  
		Last Modified: Wed, 05 Oct 2022 01:18:25 GMT  
		Size: 57.2 MB (57201277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:76c19a30a9435307f522fa8cf1dbcdccb8f516374061fe31b679685aa343ee52
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126538340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:427da1a6eb6e49b0df355a4e6927bfc5d6cb15925c03abdeeefebff0425b24f7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:48:31 GMT
ADD file:2f3df348b6a9200fcbcfe13a10334cef72dca5f19d7ed73055f7a03ff08122f7 in / 
# Tue, 04 Oct 2022 23:48:31 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:12:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:12:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:13:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2843f1fd91937d710e0d158046e9c23fe034f11c8c934a478f443b561be758dc`  
		Last Modified: Tue, 04 Oct 2022 23:52:36 GMT  
		Size: 51.8 MB (51838659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0cbaeabf686852f0109b0402554bbb882e0b7f95b9befb62dcb2c9cf5334b69`  
		Last Modified: Wed, 05 Oct 2022 00:22:23 GMT  
		Size: 8.7 MB (8744107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01b61654d50a40ae8ba57e261eb049904e5e6879f2e9421bb37a8653997b3e6`  
		Last Modified: Wed, 05 Oct 2022 00:22:23 GMT  
		Size: 11.0 MB (11029995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed53865dde9c538a03f148e1ba35bf9cb11545d6cc64b982f47d173fc76948ae`  
		Last Modified: Wed, 05 Oct 2022 00:22:46 GMT  
		Size: 54.9 MB (54925579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:2daee8056defbefb7c44552cd1459e5679697f2c0b0d6dcea2ec5040b4ea1137
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121762340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65bd8e30ab8ce2052ff48b213f632b23717eb24125bc8a555a52332d56a64ce4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:57:54 GMT
ADD file:9f3a74b8856c0affe36dd4e0700a8a2686a9d2275934fd9af95135f13731d10e in / 
# Tue, 04 Oct 2022 23:57:54 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:29:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:29:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:29:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b2ee1685df1bf13149eece9e0085c6befe355f21deeea69484a3ab1fab51e40c`  
		Last Modified: Wed, 05 Oct 2022 00:03:53 GMT  
		Size: 49.7 MB (49692608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237b865ef48770b9d41964e18461ec2d393677f4fc653a0953e9f0b9773d47ac`  
		Last Modified: Wed, 05 Oct 2022 00:52:01 GMT  
		Size: 8.4 MB (8396889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902b8eea02f53006b302a3dbae787275ce520ccf78df670e0dcafbfd1c4e17cd`  
		Last Modified: Wed, 05 Oct 2022 00:52:01 GMT  
		Size: 10.7 MB (10661490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540119c620ce1fcebd013dc72077ca8f4751440b9eb633b56bd350f29e749420`  
		Last Modified: Wed, 05 Oct 2022 00:52:26 GMT  
		Size: 53.0 MB (53011353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:8bd29cc6e3327087e44602b825e057b36ed595b23c5b4451a42a8ddfdb93e872
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130368561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5abbf020de6bd883644790336ab7cc1f2320e68c6bf79ff501813588c5f050d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:00 GMT
ADD file:269c8bec4871d84b9133706a2f391209619d53c0bfa56121c740757cf5798fcb in / 
# Tue, 04 Oct 2022 23:44:02 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:21:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:21:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:21:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2debf9e7f23054c81a936da9b01c5db9f72a55d4810f7bf0e5641bd1748d90b7`  
		Last Modified: Tue, 04 Oct 2022 23:49:11 GMT  
		Size: 53.0 MB (52980389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a790615211c3ee762ced64a5b81859f93d76062f4cf9c83d396fb13c24f7cf`  
		Last Modified: Wed, 05 Oct 2022 00:36:13 GMT  
		Size: 9.1 MB (9128105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae70f6dfe035ba217dd9a40e630bb3cae03e8d9cef649641a8a502495edf00c0`  
		Last Modified: Wed, 05 Oct 2022 00:36:13 GMT  
		Size: 11.1 MB (11134219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf9ff2029a6f8ea8f4523829a06c0ce632548ee555f4321818634a64fb364c59`  
		Last Modified: Wed, 05 Oct 2022 00:36:33 GMT  
		Size: 57.1 MB (57125848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:bb8f335fbccf0d2040d44a9901f5d5892fddf6faf56f84c2699db34d21e91570
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.3 MB (132265500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:533c3f4baead23baa420e1ab640834843dc1a50aec17fc4a2c085177b12d89ce`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:21:54 GMT
ADD file:f47fc1d53965bb08e38b482e78bd79e3cbeecc53e586ffd88bff0e6fed0a1f3c in / 
# Tue, 25 Oct 2022 02:21:55 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:12:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:12:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 05:13:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11f88873ba86e184f57ba78457d36c4f22e16eaffb9c293964adc7905e18bfe5`  
		Last Modified: Tue, 25 Oct 2022 02:27:09 GMT  
		Size: 52.2 MB (52224672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:683bf09527f61248ec1a0fa70be7388069c28d961ae31bd3a05c43ae41192a7a`  
		Last Modified: Tue, 25 Oct 2022 05:26:29 GMT  
		Size: 9.3 MB (9330348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823ddfa7a0daf2e9e0c4b6ce038b2e2cce83bde4ba9aef56fb6911d8241ca03d`  
		Last Modified: Tue, 25 Oct 2022 05:26:29 GMT  
		Size: 12.1 MB (12094186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f47813fb488b28b2af09c6f4d188832f52b886546c7885a3bb2d1b67b0d69be`  
		Last Modified: Tue, 25 Oct 2022 05:26:48 GMT  
		Size: 58.6 MB (58616294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:c942e931db31d5c2e72264278254cf3270324e3f44fb7f1395d1bb1521d12600
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.8 MB (128793781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40553f8f691301cee00d5f713fbac8c57b59252c2dd9245ae7f5714fe6e1495d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:08:36 GMT
ADD file:f17f2d6b2018174ed9b628a69ee630ae6e011a3022bb5a0f3196ef9009d39270 in / 
# Wed, 05 Oct 2022 00:08:41 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:01:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:02:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 01:04:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:17006ab86ecbcadb62dabb0d565c7783b28660c51cccb5d7b46f01518a3753a3`  
		Last Modified: Wed, 05 Oct 2022 00:16:34 GMT  
		Size: 53.0 MB (52966979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cc6e8e3ab563929336c7963595d1f292897822342a96c95dcb7cff4bc403b4`  
		Last Modified: Wed, 05 Oct 2022 01:28:47 GMT  
		Size: 8.7 MB (8663556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018c7dae3a16e88ec9bace52486f5c77ed5891921868e64784dd35f09d55ab46`  
		Last Modified: Wed, 05 Oct 2022 01:28:47 GMT  
		Size: 11.1 MB (11128331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e031ef7803b56989f08a0276998fb1edfcabb65ab13ea4a75513a55ad575bc42`  
		Last Modified: Wed, 05 Oct 2022 01:29:37 GMT  
		Size: 56.0 MB (56034915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:4f2eaeafdc00619b3261438eb3732374c930801515ce7e52579cb5d5d02a7892
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.0 MB (141048219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b370e6a9d424eb45d4884582c0ce53e633a01193c47b684cbeee1f478abed237`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:16:56 GMT
ADD file:22dddefde9f3e8eff6049751a459a3c4fdade46622016ce6269b630157170962 in / 
# Tue, 04 Oct 2022 23:16:59 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:47:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Oct 2022 23:47:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Oct 2022 23:48:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8fd653dd210d0ff49ceb9b32e662a564ab01445265e165edd4f963c3953f5b33`  
		Last Modified: Tue, 04 Oct 2022 23:22:42 GMT  
		Size: 57.1 MB (57111564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0f7f38b022f1a84d71f8e4124fe0133ced1b702ee627bff0eb3e756558fbdd`  
		Last Modified: Wed, 05 Oct 2022 00:02:33 GMT  
		Size: 9.9 MB (9883282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79064b2f900a5a0fc53fac8232b1268f1f2e3496cc5722826e03a2b768366be9`  
		Last Modified: Wed, 05 Oct 2022 00:02:33 GMT  
		Size: 12.1 MB (12143792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e113e7ad373417ab9b8860252dfab9e3cb296c126693a7c0b8ad045607bed6`  
		Last Modified: Wed, 05 Oct 2022 00:03:02 GMT  
		Size: 61.9 MB (61909581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:221812309a8315f40e7a00439dfae7b687e3828c543190683390eec5bc6263dd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126484316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c27b9f13f925e68613971e6806d863cbc335c648a119e6ce33664f7874816557`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:13:56 GMT
ADD file:92a462945d4b32c30f41478992b9ab30d452ac37b0ecef64e2325e4e99296ea8 in / 
# Tue, 25 Oct 2022 01:13:58 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:29:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:29:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 02:30:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e544dc28605cf962b36f5ba4703f824c022460d64f8973e49764cd76163df5ff`  
		Last Modified: Tue, 25 Oct 2022 01:18:08 GMT  
		Size: 49.6 MB (49578501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50715b09b75ed5a3b59f5532be8529ac130746e899c823894a3ee91fc976a5ed`  
		Last Modified: Tue, 25 Oct 2022 02:48:44 GMT  
		Size: 8.8 MB (8785586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09bb8ed5a6b2d134cb7b866721196b0adaa54ab94d27c13c65773f16fffc143d`  
		Last Modified: Tue, 25 Oct 2022 02:48:44 GMT  
		Size: 11.7 MB (11727044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094b78b28a264fd0d8e36e29b1b3e4c349049eedd6af26957228a4bb291b7f90`  
		Last Modified: Tue, 25 Oct 2022 02:48:58 GMT  
		Size: 56.4 MB (56393185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
