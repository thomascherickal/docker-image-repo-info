## `buildpack-deps:buster-curl`

```console
$ docker pull buildpack-deps@sha256:fcf1a0047ef30d3c54dde9ff65e59f1618d05202f5ce484b812bff527f85f22d
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

### `buildpack-deps:buster-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:7aa8b70d2c532b739c4f167a755fe2f0050fa38e6c43e1a9c0c983f538e03867
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.2 MB (68199932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fbf89244556ee6249387c7eda49dbb176a7938e2a62334d646dbc68acfca102`
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

### `buildpack-deps:buster-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:21a8460a8f4b5fc22ae1414dac0dec3ff4780d72ba119e1ff8be181f1b852eaa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65153760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69358fdfc3fdfa945b4ded4e2e30af44930841a6a002bd4e2e8fa20cca73eefb`
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

### `buildpack-deps:buster-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:d84c71f4740f2c6262ec3e9d7d5ed190de3491623daeb22f07236af0b6be78e2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62308774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:376beccf4679d579394f49879526260de6ae525cdb5c03c14bb6847556880477`
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

### `buildpack-deps:buster-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:9fc2c0e145ca90545c87dd989e1af9ff9b9a0a8afbb1d14ea5188d6e11711fcf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.8 MB (66833676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e36bedb554a4deb0b8bd65adc3d002e1052f1d9964ef022e1feb62d61cf67f20`
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

### `buildpack-deps:buster-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:dd914f7596e6163c9f4f17eee1766b772ae3762f8f5a06f5f0e2b7214247a6fc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69478300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62ebd2b88ce8e5bfd92c1e6a24988238eacdf44f925ed90a9cc440012367e545`
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

### `buildpack-deps:buster-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:7741f7228d90c33f1040bf3418c37192838f1de08d7cbf74a064776495ee7b75
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66265073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f5d67a33d92040b1942dac5dad8d2493e8d21128e3ff916ab56aae89401365a`
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

### `buildpack-deps:buster-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:e9c85cbadb9dede3ee701f29df342e65c63ee65b0d9e4892bc05c9e16be419ad
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.1 MB (73122901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:768a27c5becd22499b08263ef59424cf90dbbac75dbf1d5c35ac5b720856b2bc`
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

### `buildpack-deps:buster-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:654d56221ae88c0047d06eea5d0689e04033d448510b08a6dbb228afeec83e51
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.2 MB (66230900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02cb7e7fc103eee92dd967676c07dfbd7110b06e798b222debb22a9af04155f1`
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
