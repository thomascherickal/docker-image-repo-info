## `buildpack-deps:scm`

```console
$ docker pull buildpack-deps@sha256:a2e8b8856756ef61007805039cb6346098df04e1dac22cd669411fa919dbc63a
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

### `buildpack-deps:scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:682857c3673ff1a5a2da6d337545f8f313d0a9de2cbe4d0ac27a7bf8694ed36a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.0 MB (120027015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ca249d8a4d97ccbf96bde49335996c4cd276c3facc21f74a1d246f885ebe723`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 06:28:12 GMT
ADD file:fb54c709daa205bf9d04eb3d90ba068db4c34dfe3b6ec0d7691f677286120903 in / 
# Fri, 15 May 2020 06:28:13 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:32:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:32:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 17:32:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:376057ac6fa17f65688c56977118e2e764b27c348b3f70637fa829cd2a12b200`  
		Last Modified: Fri, 15 May 2020 06:37:20 GMT  
		Size: 50.4 MB (50391294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a63a0a859d859478f30461786a49c2fca3ae7d89ab5b5ce3c81c54951d30f88`  
		Last Modified: Fri, 15 May 2020 17:50:44 GMT  
		Size: 7.8 MB (7812354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496548a8c952b37bdf149ab3654f9085d721ee126b8c73b16860778be5137f5e`  
		Last Modified: Fri, 15 May 2020 17:50:49 GMT  
		Size: 10.0 MB (9996284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2adae3950d4d0f11875568c325d3d542d1f2e2d9b49bdd740bb57fcfc1f6478f`  
		Last Modified: Fri, 15 May 2020 17:51:06 GMT  
		Size: 51.8 MB (51827083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:a15836648b61f4c75b8f8940b4e8efa948feb94024b54d1d3148ae9268b7d217
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114725957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3798670d5489f6096465b52338873eb43f425fb18c448f4b73823a129621d742`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 22:37:33 GMT
ADD file:4c10ab201790c23b97915a6e841b9567581a4fbf17ffbfe84e980ca243a8467f in / 
# Thu, 14 May 2020 22:37:37 GMT
CMD ["bash"]
# Fri, 15 May 2020 03:42:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 03:42:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 03:43:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fb15ddec83dc56686109e855646d15f68bcd184e7d41da9ccbd93503b895e080`  
		Last Modified: Thu, 14 May 2020 22:46:29 GMT  
		Size: 48.1 MB (48107469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c9c9c97e34eb4f2a81e603f898669fb24b84ad169c84d6a88c3cc6c80ec019`  
		Last Modified: Fri, 15 May 2020 04:01:55 GMT  
		Size: 7.4 MB (7359224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03f1d00aaa84dd193d874cc9585feca69c6fa2d283d1fd8d030356afd24de516`  
		Last Modified: Fri, 15 May 2020 04:01:55 GMT  
		Size: 9.7 MB (9687067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc2154178d1d783f1d3d36ef36653de4543bcc6aa884be7b41ec5fb56c43545`  
		Last Modified: Fri, 15 May 2020 04:02:19 GMT  
		Size: 49.6 MB (49572197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:cde1c26d4202048197427db368be855a31bcefdf5cba675ecda98c7ff912c9d9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.7 MB (109664435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0da38497ada155e0e0b64b78a00b623f67a0c15c82a3c42e20a9e6c1e0436857`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 00:59:31 GMT
ADD file:d3b126babe4f145c735dff1d1a8828e523967279b9f25d547fce6f4d5422d0a4 in / 
# Fri, 15 May 2020 00:59:33 GMT
CMD ["bash"]
# Fri, 15 May 2020 10:34:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 10:34:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 10:35:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:33f1e205e6f963868048d05375e218b5a53592240c265ac49b4860e141d25c66`  
		Last Modified: Fri, 15 May 2020 01:11:01 GMT  
		Size: 45.9 MB (45868629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83963556ddab1d93e22197bee7fc0d66da2f25f8ae77f4147c0ebee63db933e3`  
		Last Modified: Fri, 15 May 2020 10:57:21 GMT  
		Size: 7.1 MB (7096812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e52e6e35f16ed7d977f73bf736fe9e27ba863d03fa402e68e53f187ae3c43123`  
		Last Modified: Fri, 15 May 2020 10:57:22 GMT  
		Size: 9.3 MB (9343333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf172e11e265992a6dffd35b590fb6e71abfee19640961a4b80f8e7f8280ce8b`  
		Last Modified: Fri, 15 May 2020 10:57:47 GMT  
		Size: 47.4 MB (47355661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:eca24fdb8fc5b4815d1c91216ba0bd28d699a0dda71beed2bc36c7037e45a160
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.0 MB (118989634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f79b5327f341d4604d263b57bc0e9823cd364614181adb3767fa66b9a4819a1d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:43:08 GMT
ADD file:685903e2621502d2f743969aaf293a5feab58680a95cd93a5ebf2b07f3b5d358 in / 
# Wed, 13 May 2020 21:43:10 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:24:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:24:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 22:24:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0be831822ade5f87765ba6ff26243b12a3ecd4c379df96483549a7992c1fd35b`  
		Last Modified: Wed, 13 May 2020 21:52:50 GMT  
		Size: 49.2 MB (49168115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2879905fcfbdfe9945e6eb39396c6b52b929faf145449ab656f7b35bb6387a`  
		Last Modified: Wed, 13 May 2020 22:39:40 GMT  
		Size: 7.7 MB (7681618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f2769f7d2af01c05219ba1529b243249dcedccd56fabeee3d41d792b819f494`  
		Last Modified: Wed, 13 May 2020 22:39:39 GMT  
		Size: 10.0 MB (9983943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5e8c22f4290c6000d75544c42d271474d93302f7cd74ef79832ba3c93c962a`  
		Last Modified: Wed, 13 May 2020 22:40:02 GMT  
		Size: 52.2 MB (52155958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:d549f0e8335220646d7c6daf82422a09bb7d8dfc520a0eb0d52a4dd069d1756f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.9 MB (122907152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:736e391b7b83de5d6ff6fc16aa70614fbd3a198ccbf6e1f66c9b4a2fb5a179a0`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 07:07:17 GMT
ADD file:8e3b513586e9ff0d65f88b3b2978986693585177fae673aa5432e2934e212cf1 in / 
# Fri, 15 May 2020 07:07:17 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:07:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:07:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 17:07:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8f68852a383b581a180c01bf6d2f7039194fed91451d0686630c59cb80d321c3`  
		Last Modified: Fri, 15 May 2020 07:17:49 GMT  
		Size: 51.2 MB (51157846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:126dd406c4f640ca6230b5a4b713a552e39df8129fac9f67e1c27bfa61d92953`  
		Last Modified: Fri, 15 May 2020 17:26:28 GMT  
		Size: 8.0 MB (7981878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f299696f31e375aea3d6d222d2ddd28b4972fc3855d3fa45ea032ffab0fd57dd`  
		Last Modified: Fri, 15 May 2020 17:26:28 GMT  
		Size: 10.3 MB (10338576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ae07435f995dcd7d000780f0887c530a2218056928cee15a21edf6940cbd9c`  
		Last Modified: Fri, 15 May 2020 17:26:48 GMT  
		Size: 53.4 MB (53428852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:9fb559a17ecf3aceec1f65388fe0920ea7a3afdf52cf83a507fd39551add657a
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.1 MB (117104509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:738fb0310bf0fc232a7e3bfc58278ef088e3f467c20128d92a19237857bcb5aa`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 04:47:51 GMT
ADD file:0ddadadf9bac33aa2c030e9f35797265ae45bedabeeee3c1a7db17849db5d1f6 in / 
# Fri, 15 May 2020 04:47:52 GMT
CMD ["bash"]
# Fri, 15 May 2020 14:37:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 14:37:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 14:38:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2d4d74c73ac68f6d7577b51be94381bbbbfec8dd4e7b329089ca42b7d41a75bf`  
		Last Modified: Fri, 15 May 2020 04:56:25 GMT  
		Size: 49.0 MB (49019343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8404e44ede21b71fba958dcbf67f3e30056b14cfe75ac7c0edc7c26586310d2d`  
		Last Modified: Fri, 15 May 2020 14:51:07 GMT  
		Size: 7.2 MB (7229891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5107f44d6fb498f29d6e1695ffa66a63840c5c7d91adb30d6a538c8cb06b66`  
		Last Modified: Fri, 15 May 2020 14:51:00 GMT  
		Size: 10.0 MB (10015839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75e4e64bf83c899f8786006ad0ef0a1ec9df0a6cd3754a65c48cb5ac4382597`  
		Last Modified: Fri, 15 May 2020 14:52:07 GMT  
		Size: 50.8 MB (50839436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:84895d57d7f38156db0636d4e5d189e61878ae5d5e9ecf94e09f4a0b1677d86e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.6 MB (130582816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fba7835f4d49633e0b09854a0720bd0d5cd8f97adc336d32abfce96e4ce26fa7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:20:32 GMT
ADD file:ed5dc7bd2c0c0dafef9ca4829cd89719c538cd23991fb941589e7fd3bf96b407 in / 
# Wed, 13 May 2020 22:20:38 GMT
CMD ["bash"]
# Wed, 13 May 2020 23:43:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:44:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 23:45:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:19aca0f2a5b89bbc37caa77bbd1612566fadbbce5c3381246fe356d7e5d14774`  
		Last Modified: Wed, 13 May 2020 22:57:18 GMT  
		Size: 54.1 MB (54142914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556cd6fadc0f341d090a18ecfc4b6aedccd3d99f6eb6a336e3bee33f096c095f`  
		Last Modified: Thu, 14 May 2020 00:28:57 GMT  
		Size: 8.3 MB (8252823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633177125031b056c9e79b442829845cc6886ad14d5de3cc2459317eaa054d94`  
		Last Modified: Thu, 14 May 2020 00:28:59 GMT  
		Size: 10.7 MB (10727164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e762e21652d78f0bcf2f8011e2751e5d6be323a639e89c083f93a086fe1b6005`  
		Last Modified: Thu, 14 May 2020 00:30:19 GMT  
		Size: 57.5 MB (57459915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:3d26cee0eafc0ed577a486d9d667c3381f44b3ecd45c70579f95840e0b6a00c9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117599340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:688dd456938ea4ff2da1d909ec5d441864aa7cb939803d346d7f7287e0caae7d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 23:06:22 GMT
ADD file:3b65bac2545f5751eaa8e9967febbe18955f63efa32d5ca3f8bc209e1a8602de in / 
# Thu, 14 May 2020 23:06:24 GMT
CMD ["bash"]
# Fri, 15 May 2020 05:00:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 05:00:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 05:01:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:070f0b30acfe8cf53f3aeaae5982c911acd4c4a652a456c849a94c66117d4067`  
		Last Modified: Thu, 14 May 2020 23:11:09 GMT  
		Size: 49.0 MB (48966486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db7092766f19f5c47b8a2388225b82a8d95d39c4e0ae321805e2a5cf0c8b961`  
		Last Modified: Fri, 15 May 2020 05:08:53 GMT  
		Size: 7.4 MB (7382266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643084632f50b88b1aea5263e63d7dff9175610fe2041ce83dcdbb3d926246d8`  
		Last Modified: Fri, 15 May 2020 05:08:59 GMT  
		Size: 9.9 MB (9882148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4118b891b350fa9ce5f64fd71fe7161ade2a6f32705dbd623b014ff5198f96b0`  
		Last Modified: Fri, 15 May 2020 05:09:13 GMT  
		Size: 51.4 MB (51368440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
