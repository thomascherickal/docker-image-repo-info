## `buildpack-deps:bionic-curl`

```console
$ docker pull buildpack-deps@sha256:dcb2d54836f9a7ca1639cd4fd498925e854cfe0a2789eeac075e825d4ec55dd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:bionic-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:fb84bfba9252ad0cad4bf624e06d1c893d3b1a7f55e3cc37aa605f5a67d9441d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 MB (36365486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64c992125c0697acbdc18105c298d44b3c5e089b2fdfaef91658643be66c77d1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 19:38:36 GMT
ADD file:8733c7e8faf03d53cb2143ff6ac405362944cfa07422fccd21a3066cc2f42c83 in / 
# Tue, 06 Sep 2022 19:38:37 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:56:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:56:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:726b8a513d66e3585eb57389171d97fcd348e4914a415891e1da135b85ffa6c3`  
		Last Modified: Fri, 02 Sep 2022 15:41:13 GMT  
		Size: 26.7 MB (26710833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7dbb4551b9c872b2053c38cdd5dd7e02c06107e648b950551a585e5e88394c7`  
		Last Modified: Tue, 06 Sep 2022 20:00:54 GMT  
		Size: 6.6 MB (6630965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79cc7a6dc37d1b46bb3edb182f0a133c77f677de31779964db5569d6137a99d`  
		Last Modified: Tue, 06 Sep 2022 20:00:54 GMT  
		Size: 3.0 MB (3023688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:afe6b279269826bd9d9a9b77ac80bbd54db65cc922bf5a184f06f6a396719d8e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30590180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53b82ac9f9048c0858ffaed15ca8ef98cdc38e7c07be402ef88ebaf6792962c6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 19:33:23 GMT
ADD file:45c82fca220161f3905a06e276f12ec0cb3be5c099cca70bb6d495da10088f7d in / 
# Tue, 06 Sep 2022 19:33:24 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:51:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:52:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:074d633b5bde02245e333b110dde5850e06ea4ebefe4283af6e4dfd8d462b170`  
		Last Modified: Tue, 06 Sep 2022 19:35:07 GMT  
		Size: 22.3 MB (22305954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594729c31c2cb7f63b20f449c44c215064e068c94731174e4b57603ce032fd82`  
		Last Modified: Tue, 06 Sep 2022 19:57:06 GMT  
		Size: 5.7 MB (5698254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da759356c74e12ad90a263cb412b2ea0620a103ffedbdb492aac5586d59cdb83`  
		Last Modified: Tue, 06 Sep 2022 19:57:05 GMT  
		Size: 2.6 MB (2585972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:2a7863e0c4008a73ef0bda24499179d884f903c73c1669375cb88f15c545fc25
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.4 MB (32377184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07c6a028cf3ecfd36dd9d598bbb927e84f8a27631f594cabce0272768f7bb62f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 18:49:02 GMT
ADD file:26cb5ace98a4462b36211bf28f1e73781dd6d8984350d9bd53243dbe50ae180c in / 
# Tue, 06 Sep 2022 18:49:02 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:12:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:12:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d30cf2a6a25aea48a115837d149468c8de7df7fb51f210b9fa1173c065f7b34c`  
		Last Modified: Tue, 06 Sep 2022 18:50:34 GMT  
		Size: 23.7 MB (23734076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79317661c5fe6a8a22ce652c9fb0999eb96ed08b735a16224e9a795c877780d`  
		Last Modified: Tue, 06 Sep 2022 19:16:57 GMT  
		Size: 6.1 MB (6072017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:737382e506f963b99b1453e20a2fcbb6bc4328a0c68bfc3530b2082a5f3da14f`  
		Last Modified: Tue, 06 Sep 2022 19:16:56 GMT  
		Size: 2.6 MB (2571091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:9843a4e78ba03fb07ec7138d9afdaabb3412478c44103fbca5fc8732b1a29bb8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37124393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab6063d4c02c86863842cda863cdd0b9fc41b99181a9d5bb4e10e93c58167700`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 18:40:06 GMT
ADD file:31701667cc90b9f4ce7d6ede94bf7dae4d63c49e62d3725094d547f9601e1165 in / 
# Tue, 06 Sep 2022 18:40:07 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:02:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:02:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:10d3032d1995d3163c20a7f2f197299fae258c2ad020a8fd586fd6b7dd1b0e1d`  
		Last Modified: Tue, 06 Sep 2022 18:40:53 GMT  
		Size: 27.2 MB (27164710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360b65e679bf1db70d92b45a6d39c882e074d441412548705adf35d49a12c70a`  
		Last Modified: Tue, 06 Sep 2022 19:06:33 GMT  
		Size: 6.9 MB (6919740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8820513ab0577fe6133989b66cdc2a5a0b1a97af5280746721af55657c0897d7`  
		Last Modified: Tue, 06 Sep 2022 19:06:32 GMT  
		Size: 3.0 MB (3039943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:17ba421e87b43d3709f030baae5c32ff973f324914ce189a7ec322b8d465f42c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41212000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f2cd514147c478a3ed7fabf6a7c9ce8924b524298a42b113013caf62abee8b5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 19:38:57 GMT
ADD file:1b76d0a41921afefb92711c44ceb312c16828d433b689a951d65c238faa9ac50 in / 
# Tue, 06 Sep 2022 19:38:59 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 20:06:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 20:06:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4abf8f40556a940861bc7fc313acefb89c775273ed06b7d41cfb222ccf8a1438`  
		Last Modified: Tue, 06 Sep 2022 19:40:56 GMT  
		Size: 30.4 MB (30441623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7afd3028934ff054bca1d0bb218e690d2cdb60f7754ad3bb6426c3744e730f`  
		Last Modified: Tue, 06 Sep 2022 20:12:44 GMT  
		Size: 7.1 MB (7050146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33850c25587eb4418b5e6aeccf1c9e6fa5b0baac624020bc56b4d4db8c2742c5`  
		Last Modified: Tue, 06 Sep 2022 20:12:43 GMT  
		Size: 3.7 MB (3720231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:88bdf05d087dec6348b811e7fe133c6de77ad937052d47ef17e19e9f48313d15
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34671530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1271e59da62b67faad96ae96f4a55cbfdf33568b76dbfc4820467a25e9cc5d51`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 18:43:36 GMT
ADD file:dbe2a8e3943129e654ee29c636cab2bb10dd7eb0ac27d51e6954af2ccbe22807 in / 
# Tue, 06 Sep 2022 18:43:37 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:11:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:11:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:be6761156800c616810cb8aeb5b3ae71b9a2082f1c1221210befe119f082e879`  
		Last Modified: Tue, 06 Sep 2022 18:45:00 GMT  
		Size: 25.4 MB (25370130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae409e724954611ea7731639a0dab7c4c59fdb64deb51dba5327bc8c5a085c5f`  
		Last Modified: Tue, 06 Sep 2022 19:17:11 GMT  
		Size: 6.3 MB (6324234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aca3edc7c631417c9e3dbbcb30698aed6531dc2482e10dd41ee221de2d450ca5`  
		Last Modified: Tue, 06 Sep 2022 19:17:11 GMT  
		Size: 3.0 MB (2977166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
