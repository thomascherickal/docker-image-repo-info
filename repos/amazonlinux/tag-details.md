<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `amazonlinux`

-	[`amazonlinux:1`](#amazonlinux1)
-	[`amazonlinux:1-with-sources`](#amazonlinux1-with-sources)
-	[`amazonlinux:2`](#amazonlinux2)
-	[`amazonlinux:2-with-sources`](#amazonlinux2-with-sources)
-	[`amazonlinux:2.0.20220426.0`](#amazonlinux20202204260)
-	[`amazonlinux:2.0.20220426.0-with-sources`](#amazonlinux20202204260-with-sources)
-	[`amazonlinux:2018.03`](#amazonlinux201803)
-	[`amazonlinux:2018.03-with-sources`](#amazonlinux201803-with-sources)
-	[`amazonlinux:2018.03.0.20220503.0`](#amazonlinux2018030202205030)
-	[`amazonlinux:2018.03.0.20220503.0-with-sources`](#amazonlinux2018030202205030-with-sources)
-	[`amazonlinux:2022`](#amazonlinux2022)
-	[`amazonlinux:2022-with-sources`](#amazonlinux2022-with-sources)
-	[`amazonlinux:2022.0.20220504.1`](#amazonlinux20220202205041)
-	[`amazonlinux:2022.0.20220504.1-with-sources`](#amazonlinux20220202205041-with-sources)
-	[`amazonlinux:devel`](#amazonlinuxdevel)
-	[`amazonlinux:devel-with-sources`](#amazonlinuxdevel-with-sources)
-	[`amazonlinux:latest`](#amazonlinuxlatest)
-	[`amazonlinux:with-sources`](#amazonlinuxwith-sources)

## `amazonlinux:1`

```console
$ docker pull amazonlinux@sha256:1577424aa215cc0749c57da79d912cec36496cf375603865f55aa8c8e012ac5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:1` - linux; amd64

```console
$ docker pull amazonlinux@sha256:65d3e8afed7c267addcfdd863ec1863802130c8cfce8c7f0bc1989ef9b37d750
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62370354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee571057d755a36c540c50e79f85b79dcd31eb72846cca31d09cfd382f2c0007`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 12 May 2022 22:52:38 GMT
ADD file:7be03a5ca96cd8244bae5899aa6c63dbe3e4337104581cdfd80188e91990e157 in / 
# Thu, 12 May 2022 22:52:39 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d9c9737fa7354e459f78712e13ee65dbd185b97c97882c6441cb91cd71e2550c`  
		Last Modified: Thu, 12 May 2022 22:54:14 GMT  
		Size: 62.4 MB (62370354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:1-with-sources`

```console
$ docker pull amazonlinux@sha256:bda80fad2388f170f95c241b14c4e05f5efed2b9215179354d98852255e6ea6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:be9106f88bec4a05ed5a48d5c1be368b2ec6eed4e9bc48a049ba8c112b5f4885
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515021073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d05eec4707c75703bdce6abd77c2fb00614c233b683e9af819205c335b2e666`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 12 May 2022 22:52:38 GMT
ADD file:7be03a5ca96cd8244bae5899aa6c63dbe3e4337104581cdfd80188e91990e157 in / 
# Thu, 12 May 2022 22:52:39 GMT
CMD ["/bin/bash"]
# Thu, 12 May 2022 22:53:03 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-61565aaf9b6c05012b6ed631ec677017e91f86c7397b5f165bb3f2b6b4aad73e.tar.gz"  && echo "4e9b6750e73f78ad5bf47e828febbb175f145654add0d240d65f55737f537be8  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:d9c9737fa7354e459f78712e13ee65dbd185b97c97882c6441cb91cd71e2550c`  
		Last Modified: Thu, 12 May 2022 22:54:14 GMT  
		Size: 62.4 MB (62370354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f474d01f74f4e99d1e4eb26ce6326e089844994984350cb9c172bd8e98016e`  
		Last Modified: Thu, 12 May 2022 22:54:44 GMT  
		Size: 452.7 MB (452650719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2`

```console
$ docker pull amazonlinux@sha256:246ef631c75ea83005889621119fd5cc9cbb5500e193707c38b6c060d597a146
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2` - linux; amd64

```console
$ docker pull amazonlinux@sha256:5ca9e45da788e7bac100dffaf45645cea5af68d46f62144f683c0434e14fd586
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62291142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecdeb69c57ad20820ceb442c918b35228a6c9d04d6458768fdf4e86429cbccca`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 May 2022 23:19:31 GMT
ADD file:386c34c6960464ef8f88891333fb091aef731602a28a185a9d6db27726fbe504 in / 
# Tue, 03 May 2022 23:19:32 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8de5b65bd171294b1e04e0df439f4ea11ce923b642eddf3b3d76d297bfd2670c`  
		Last Modified: Mon, 02 May 2022 22:06:03 GMT  
		Size: 62.3 MB (62291142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:b1377309830b143f16246542ac234b8b0b9251533954bfb9d3ffd79e2c199901
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63902179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1a0df532d4a93ede0e0da29817f5dfdfb9c6653e22e32388de3149618d47cef`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 May 2022 22:39:32 GMT
ADD file:c351a8c80719ef38e02c26849f50bb7d79c24a6347cc2a72ae1a0768964bd113 in / 
# Tue, 03 May 2022 22:39:34 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ec3b4c26678b188d3874bed5e14dd278311fc05c81e418d5f0da36ec38d9f488`  
		Last Modified: Tue, 03 May 2022 03:07:52 GMT  
		Size: 63.9 MB (63902179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2-with-sources`

```console
$ docker pull amazonlinux@sha256:f66f05473f90aa6e14ac926ec03d61af16828a2ff9205fbfa1d3713670b0c166
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:9a3fbba8f30fbd72a0aa0116fd0ef46e8af25d260d01073c266347f116f20399
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **485.7 MB (485712608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6855b0eeeef206786c8c7ac97e546f8677b9d18b2fead70262d5cebc674f86d2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 May 2022 23:19:31 GMT
ADD file:386c34c6960464ef8f88891333fb091aef731602a28a185a9d6db27726fbe504 in / 
# Tue, 03 May 2022 23:19:32 GMT
CMD ["/bin/bash"]
# Tue, 03 May 2022 23:19:53 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-27e5885b1b2e681d27e9e8c451079b8f7f6444b820900db76e8e1f583d454a37.tar.gz"  && echo "fae8bd9cc002cf6ab3af9d777f1bc2646993e0340f2ffac4ddc984a5821a77c2  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:8de5b65bd171294b1e04e0df439f4ea11ce923b642eddf3b3d76d297bfd2670c`  
		Last Modified: Mon, 02 May 2022 22:06:03 GMT  
		Size: 62.3 MB (62291142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab0efe039696303bb91bcd3177af472d1339e2e4cd62297fabd75e1763b9bcb9`  
		Last Modified: Tue, 03 May 2022 23:21:15 GMT  
		Size: 423.4 MB (423421466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:124eb9a22c4bd8d59ea311f776bae5213d1e66db6103732c2c10741bb263f459
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **487.3 MB (487323598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671abfcb4f4c6d925fbecf84883a36ca87a0e7e8aa40bc10b0c3a1678f2b1168`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 May 2022 22:39:32 GMT
ADD file:c351a8c80719ef38e02c26849f50bb7d79c24a6347cc2a72ae1a0768964bd113 in / 
# Tue, 03 May 2022 22:39:34 GMT
CMD ["/bin/bash"]
# Tue, 03 May 2022 22:39:57 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-27e5885b1b2e681d27e9e8c451079b8f7f6444b820900db76e8e1f583d454a37.tar.gz"  && echo "fae8bd9cc002cf6ab3af9d777f1bc2646993e0340f2ffac4ddc984a5821a77c2  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:ec3b4c26678b188d3874bed5e14dd278311fc05c81e418d5f0da36ec38d9f488`  
		Last Modified: Tue, 03 May 2022 03:07:52 GMT  
		Size: 63.9 MB (63902179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189fd58a2d5dc106fd8a0dee23c67eaa14f4c78c0e8fecb154e921df7a05540e`  
		Last Modified: Tue, 03 May 2022 22:41:23 GMT  
		Size: 423.4 MB (423421419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20220426.0`

```console
$ docker pull amazonlinux@sha256:246ef631c75ea83005889621119fd5cc9cbb5500e193707c38b6c060d597a146
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20220426.0` - linux; amd64

```console
$ docker pull amazonlinux@sha256:5ca9e45da788e7bac100dffaf45645cea5af68d46f62144f683c0434e14fd586
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62291142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecdeb69c57ad20820ceb442c918b35228a6c9d04d6458768fdf4e86429cbccca`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 May 2022 23:19:31 GMT
ADD file:386c34c6960464ef8f88891333fb091aef731602a28a185a9d6db27726fbe504 in / 
# Tue, 03 May 2022 23:19:32 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8de5b65bd171294b1e04e0df439f4ea11ce923b642eddf3b3d76d297bfd2670c`  
		Last Modified: Mon, 02 May 2022 22:06:03 GMT  
		Size: 62.3 MB (62291142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2.0.20220426.0` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:b1377309830b143f16246542ac234b8b0b9251533954bfb9d3ffd79e2c199901
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63902179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1a0df532d4a93ede0e0da29817f5dfdfb9c6653e22e32388de3149618d47cef`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 May 2022 22:39:32 GMT
ADD file:c351a8c80719ef38e02c26849f50bb7d79c24a6347cc2a72ae1a0768964bd113 in / 
# Tue, 03 May 2022 22:39:34 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ec3b4c26678b188d3874bed5e14dd278311fc05c81e418d5f0da36ec38d9f488`  
		Last Modified: Tue, 03 May 2022 03:07:52 GMT  
		Size: 63.9 MB (63902179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20220426.0-with-sources`

```console
$ docker pull amazonlinux@sha256:f66f05473f90aa6e14ac926ec03d61af16828a2ff9205fbfa1d3713670b0c166
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20220426.0-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:9a3fbba8f30fbd72a0aa0116fd0ef46e8af25d260d01073c266347f116f20399
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **485.7 MB (485712608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6855b0eeeef206786c8c7ac97e546f8677b9d18b2fead70262d5cebc674f86d2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 May 2022 23:19:31 GMT
ADD file:386c34c6960464ef8f88891333fb091aef731602a28a185a9d6db27726fbe504 in / 
# Tue, 03 May 2022 23:19:32 GMT
CMD ["/bin/bash"]
# Tue, 03 May 2022 23:19:53 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-27e5885b1b2e681d27e9e8c451079b8f7f6444b820900db76e8e1f583d454a37.tar.gz"  && echo "fae8bd9cc002cf6ab3af9d777f1bc2646993e0340f2ffac4ddc984a5821a77c2  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:8de5b65bd171294b1e04e0df439f4ea11ce923b642eddf3b3d76d297bfd2670c`  
		Last Modified: Mon, 02 May 2022 22:06:03 GMT  
		Size: 62.3 MB (62291142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab0efe039696303bb91bcd3177af472d1339e2e4cd62297fabd75e1763b9bcb9`  
		Last Modified: Tue, 03 May 2022 23:21:15 GMT  
		Size: 423.4 MB (423421466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2.0.20220426.0-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:124eb9a22c4bd8d59ea311f776bae5213d1e66db6103732c2c10741bb263f459
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **487.3 MB (487323598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671abfcb4f4c6d925fbecf84883a36ca87a0e7e8aa40bc10b0c3a1678f2b1168`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 May 2022 22:39:32 GMT
ADD file:c351a8c80719ef38e02c26849f50bb7d79c24a6347cc2a72ae1a0768964bd113 in / 
# Tue, 03 May 2022 22:39:34 GMT
CMD ["/bin/bash"]
# Tue, 03 May 2022 22:39:57 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-27e5885b1b2e681d27e9e8c451079b8f7f6444b820900db76e8e1f583d454a37.tar.gz"  && echo "fae8bd9cc002cf6ab3af9d777f1bc2646993e0340f2ffac4ddc984a5821a77c2  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:ec3b4c26678b188d3874bed5e14dd278311fc05c81e418d5f0da36ec38d9f488`  
		Last Modified: Tue, 03 May 2022 03:07:52 GMT  
		Size: 63.9 MB (63902179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189fd58a2d5dc106fd8a0dee23c67eaa14f4c78c0e8fecb154e921df7a05540e`  
		Last Modified: Tue, 03 May 2022 22:41:23 GMT  
		Size: 423.4 MB (423421419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03`

```console
$ docker pull amazonlinux@sha256:1577424aa215cc0749c57da79d912cec36496cf375603865f55aa8c8e012ac5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03` - linux; amd64

```console
$ docker pull amazonlinux@sha256:65d3e8afed7c267addcfdd863ec1863802130c8cfce8c7f0bc1989ef9b37d750
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62370354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee571057d755a36c540c50e79f85b79dcd31eb72846cca31d09cfd382f2c0007`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 12 May 2022 22:52:38 GMT
ADD file:7be03a5ca96cd8244bae5899aa6c63dbe3e4337104581cdfd80188e91990e157 in / 
# Thu, 12 May 2022 22:52:39 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d9c9737fa7354e459f78712e13ee65dbd185b97c97882c6441cb91cd71e2550c`  
		Last Modified: Thu, 12 May 2022 22:54:14 GMT  
		Size: 62.4 MB (62370354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03-with-sources`

```console
$ docker pull amazonlinux@sha256:bda80fad2388f170f95c241b14c4e05f5efed2b9215179354d98852255e6ea6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:be9106f88bec4a05ed5a48d5c1be368b2ec6eed4e9bc48a049ba8c112b5f4885
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515021073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d05eec4707c75703bdce6abd77c2fb00614c233b683e9af819205c335b2e666`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 12 May 2022 22:52:38 GMT
ADD file:7be03a5ca96cd8244bae5899aa6c63dbe3e4337104581cdfd80188e91990e157 in / 
# Thu, 12 May 2022 22:52:39 GMT
CMD ["/bin/bash"]
# Thu, 12 May 2022 22:53:03 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-61565aaf9b6c05012b6ed631ec677017e91f86c7397b5f165bb3f2b6b4aad73e.tar.gz"  && echo "4e9b6750e73f78ad5bf47e828febbb175f145654add0d240d65f55737f537be8  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:d9c9737fa7354e459f78712e13ee65dbd185b97c97882c6441cb91cd71e2550c`  
		Last Modified: Thu, 12 May 2022 22:54:14 GMT  
		Size: 62.4 MB (62370354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f474d01f74f4e99d1e4eb26ce6326e089844994984350cb9c172bd8e98016e`  
		Last Modified: Thu, 12 May 2022 22:54:44 GMT  
		Size: 452.7 MB (452650719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20220503.0`

```console
$ docker pull amazonlinux@sha256:1577424aa215cc0749c57da79d912cec36496cf375603865f55aa8c8e012ac5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03.0.20220503.0` - linux; amd64

```console
$ docker pull amazonlinux@sha256:65d3e8afed7c267addcfdd863ec1863802130c8cfce8c7f0bc1989ef9b37d750
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62370354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee571057d755a36c540c50e79f85b79dcd31eb72846cca31d09cfd382f2c0007`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 12 May 2022 22:52:38 GMT
ADD file:7be03a5ca96cd8244bae5899aa6c63dbe3e4337104581cdfd80188e91990e157 in / 
# Thu, 12 May 2022 22:52:39 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d9c9737fa7354e459f78712e13ee65dbd185b97c97882c6441cb91cd71e2550c`  
		Last Modified: Thu, 12 May 2022 22:54:14 GMT  
		Size: 62.4 MB (62370354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20220503.0-with-sources`

```console
$ docker pull amazonlinux@sha256:bda80fad2388f170f95c241b14c4e05f5efed2b9215179354d98852255e6ea6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03.0.20220503.0-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:be9106f88bec4a05ed5a48d5c1be368b2ec6eed4e9bc48a049ba8c112b5f4885
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515021073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d05eec4707c75703bdce6abd77c2fb00614c233b683e9af819205c335b2e666`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 12 May 2022 22:52:38 GMT
ADD file:7be03a5ca96cd8244bae5899aa6c63dbe3e4337104581cdfd80188e91990e157 in / 
# Thu, 12 May 2022 22:52:39 GMT
CMD ["/bin/bash"]
# Thu, 12 May 2022 22:53:03 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-61565aaf9b6c05012b6ed631ec677017e91f86c7397b5f165bb3f2b6b4aad73e.tar.gz"  && echo "4e9b6750e73f78ad5bf47e828febbb175f145654add0d240d65f55737f537be8  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:d9c9737fa7354e459f78712e13ee65dbd185b97c97882c6441cb91cd71e2550c`  
		Last Modified: Thu, 12 May 2022 22:54:14 GMT  
		Size: 62.4 MB (62370354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f474d01f74f4e99d1e4eb26ce6326e089844994984350cb9c172bd8e98016e`  
		Last Modified: Thu, 12 May 2022 22:54:44 GMT  
		Size: 452.7 MB (452650719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022`

```console
$ docker pull amazonlinux@sha256:3b1eddcdaaf8d664e960b9d48c77c29ee81f108e54673e4015f924993ea81cdf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022` - linux; amd64

```console
$ docker pull amazonlinux@sha256:8453a47334b50bd11a6dc8a9ff7c3e40a4ba284f0dc68c5e0edf328b11fe372f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70559972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dbdf168f78243e4eec0ca6653835b7c0d5723635f3956c67c801241670d5d17`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 12 May 2022 22:53:16 GMT
ADD file:3f4e8a0a50db5cf56025980f5849c0c840ba9116680528c507adff04d9287c7e in / 
# Thu, 12 May 2022 22:53:17 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:7516adf672a9b100319b04f4b961b4cc3070ca53af354317e3d80c6a73ca275f`  
		Last Modified: Thu, 12 May 2022 22:55:06 GMT  
		Size: 70.6 MB (70559972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:6254b7a9191c78cc08dfbdf1becd92b54a76d7976043bcd31ab104982d65b736
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69117442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bea8bae0c8c1a8e3676cee260156f268461e8787f92d1a62e7ccccc1f4bca19`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 12 May 2022 22:03:11 GMT
ADD file:8406e9d49dfceecd7a1c2cbf960e61dfe58dc85ab0ec500fe43df4123ea56b54 in / 
# Thu, 12 May 2022 22:03:13 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:57916acdbf1d56e1afdf905446c5a93b04658842560d4e5c51a61a1881c5f8b4`  
		Last Modified: Thu, 12 May 2022 22:04:21 GMT  
		Size: 69.1 MB (69117442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022-with-sources`

```console
$ docker pull amazonlinux@sha256:95e0415cbddc9a78c7c3d739fb7f7dba165b3608489c651e106b16f7ce9fb442
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:302cafedc0bb193cb86bbf729250cfe5198abb36814f5073704a5d31fb76408a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **489.3 MB (489309531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22b46dbb32e5b71640810f230fa6749b7c2d6b43be596cd2052cbfb85bec4c5d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 12 May 2022 22:53:16 GMT
ADD file:3f4e8a0a50db5cf56025980f5849c0c840ba9116680528c507adff04d9287c7e in / 
# Thu, 12 May 2022 22:53:17 GMT
CMD ["/bin/bash"]
# Thu, 12 May 2022 22:53:39 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-505b05ef761a138f8860c413d1520f5756d3a4ea82c5f6052934f3c34a880580.tar.gz"  && echo "bcbcae8a56de8cd107a736a9032b166d5ae7a15c72dbc2e8029ec7ac75d4c5da  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:7516adf672a9b100319b04f4b961b4cc3070ca53af354317e3d80c6a73ca275f`  
		Last Modified: Thu, 12 May 2022 22:55:06 GMT  
		Size: 70.6 MB (70559972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a4b54850ae445fac5d810015c4dce9a59828591287cf034e8d8687a5f42db1`  
		Last Modified: Thu, 12 May 2022 22:55:34 GMT  
		Size: 418.7 MB (418749559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:db26696e2371b0e24bc72edf8c118bd9cb18821dfe4f2343495d33eb93aaf2fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **487.9 MB (487866967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7afbb6532b42550d7ce56e9d45b1a30eddbbdf33eef198e4ba4b1123cf9ae38`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 12 May 2022 22:03:11 GMT
ADD file:8406e9d49dfceecd7a1c2cbf960e61dfe58dc85ab0ec500fe43df4123ea56b54 in / 
# Thu, 12 May 2022 22:03:13 GMT
CMD ["/bin/bash"]
# Thu, 12 May 2022 22:03:35 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-505b05ef761a138f8860c413d1520f5756d3a4ea82c5f6052934f3c34a880580.tar.gz"  && echo "bcbcae8a56de8cd107a736a9032b166d5ae7a15c72dbc2e8029ec7ac75d4c5da  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:57916acdbf1d56e1afdf905446c5a93b04658842560d4e5c51a61a1881c5f8b4`  
		Last Modified: Thu, 12 May 2022 22:04:21 GMT  
		Size: 69.1 MB (69117442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f37a59badfcabe5a4ef65d9e6f67b552297ca000f896c8a7f5bffc17447a49`  
		Last Modified: Thu, 12 May 2022 22:05:01 GMT  
		Size: 418.7 MB (418749525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022.0.20220504.1`

```console
$ docker pull amazonlinux@sha256:3b1eddcdaaf8d664e960b9d48c77c29ee81f108e54673e4015f924993ea81cdf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022.0.20220504.1` - linux; amd64

```console
$ docker pull amazonlinux@sha256:8453a47334b50bd11a6dc8a9ff7c3e40a4ba284f0dc68c5e0edf328b11fe372f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70559972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dbdf168f78243e4eec0ca6653835b7c0d5723635f3956c67c801241670d5d17`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 12 May 2022 22:53:16 GMT
ADD file:3f4e8a0a50db5cf56025980f5849c0c840ba9116680528c507adff04d9287c7e in / 
# Thu, 12 May 2022 22:53:17 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:7516adf672a9b100319b04f4b961b4cc3070ca53af354317e3d80c6a73ca275f`  
		Last Modified: Thu, 12 May 2022 22:55:06 GMT  
		Size: 70.6 MB (70559972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022.0.20220504.1` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:6254b7a9191c78cc08dfbdf1becd92b54a76d7976043bcd31ab104982d65b736
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69117442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bea8bae0c8c1a8e3676cee260156f268461e8787f92d1a62e7ccccc1f4bca19`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 12 May 2022 22:03:11 GMT
ADD file:8406e9d49dfceecd7a1c2cbf960e61dfe58dc85ab0ec500fe43df4123ea56b54 in / 
# Thu, 12 May 2022 22:03:13 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:57916acdbf1d56e1afdf905446c5a93b04658842560d4e5c51a61a1881c5f8b4`  
		Last Modified: Thu, 12 May 2022 22:04:21 GMT  
		Size: 69.1 MB (69117442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022.0.20220504.1-with-sources`

```console
$ docker pull amazonlinux@sha256:95e0415cbddc9a78c7c3d739fb7f7dba165b3608489c651e106b16f7ce9fb442
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022.0.20220504.1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:302cafedc0bb193cb86bbf729250cfe5198abb36814f5073704a5d31fb76408a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **489.3 MB (489309531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22b46dbb32e5b71640810f230fa6749b7c2d6b43be596cd2052cbfb85bec4c5d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 12 May 2022 22:53:16 GMT
ADD file:3f4e8a0a50db5cf56025980f5849c0c840ba9116680528c507adff04d9287c7e in / 
# Thu, 12 May 2022 22:53:17 GMT
CMD ["/bin/bash"]
# Thu, 12 May 2022 22:53:39 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-505b05ef761a138f8860c413d1520f5756d3a4ea82c5f6052934f3c34a880580.tar.gz"  && echo "bcbcae8a56de8cd107a736a9032b166d5ae7a15c72dbc2e8029ec7ac75d4c5da  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:7516adf672a9b100319b04f4b961b4cc3070ca53af354317e3d80c6a73ca275f`  
		Last Modified: Thu, 12 May 2022 22:55:06 GMT  
		Size: 70.6 MB (70559972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a4b54850ae445fac5d810015c4dce9a59828591287cf034e8d8687a5f42db1`  
		Last Modified: Thu, 12 May 2022 22:55:34 GMT  
		Size: 418.7 MB (418749559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022.0.20220504.1-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:db26696e2371b0e24bc72edf8c118bd9cb18821dfe4f2343495d33eb93aaf2fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **487.9 MB (487866967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7afbb6532b42550d7ce56e9d45b1a30eddbbdf33eef198e4ba4b1123cf9ae38`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 12 May 2022 22:03:11 GMT
ADD file:8406e9d49dfceecd7a1c2cbf960e61dfe58dc85ab0ec500fe43df4123ea56b54 in / 
# Thu, 12 May 2022 22:03:13 GMT
CMD ["/bin/bash"]
# Thu, 12 May 2022 22:03:35 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-505b05ef761a138f8860c413d1520f5756d3a4ea82c5f6052934f3c34a880580.tar.gz"  && echo "bcbcae8a56de8cd107a736a9032b166d5ae7a15c72dbc2e8029ec7ac75d4c5da  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:57916acdbf1d56e1afdf905446c5a93b04658842560d4e5c51a61a1881c5f8b4`  
		Last Modified: Thu, 12 May 2022 22:04:21 GMT  
		Size: 69.1 MB (69117442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f37a59badfcabe5a4ef65d9e6f67b552297ca000f896c8a7f5bffc17447a49`  
		Last Modified: Thu, 12 May 2022 22:05:01 GMT  
		Size: 418.7 MB (418749525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:devel`

```console
$ docker pull amazonlinux@sha256:3b1eddcdaaf8d664e960b9d48c77c29ee81f108e54673e4015f924993ea81cdf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:devel` - linux; amd64

```console
$ docker pull amazonlinux@sha256:8453a47334b50bd11a6dc8a9ff7c3e40a4ba284f0dc68c5e0edf328b11fe372f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70559972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dbdf168f78243e4eec0ca6653835b7c0d5723635f3956c67c801241670d5d17`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 12 May 2022 22:53:16 GMT
ADD file:3f4e8a0a50db5cf56025980f5849c0c840ba9116680528c507adff04d9287c7e in / 
# Thu, 12 May 2022 22:53:17 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:7516adf672a9b100319b04f4b961b4cc3070ca53af354317e3d80c6a73ca275f`  
		Last Modified: Thu, 12 May 2022 22:55:06 GMT  
		Size: 70.6 MB (70559972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:devel` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:6254b7a9191c78cc08dfbdf1becd92b54a76d7976043bcd31ab104982d65b736
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69117442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bea8bae0c8c1a8e3676cee260156f268461e8787f92d1a62e7ccccc1f4bca19`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 12 May 2022 22:03:11 GMT
ADD file:8406e9d49dfceecd7a1c2cbf960e61dfe58dc85ab0ec500fe43df4123ea56b54 in / 
# Thu, 12 May 2022 22:03:13 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:57916acdbf1d56e1afdf905446c5a93b04658842560d4e5c51a61a1881c5f8b4`  
		Last Modified: Thu, 12 May 2022 22:04:21 GMT  
		Size: 69.1 MB (69117442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:devel-with-sources`

```console
$ docker pull amazonlinux@sha256:95e0415cbddc9a78c7c3d739fb7f7dba165b3608489c651e106b16f7ce9fb442
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:devel-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:302cafedc0bb193cb86bbf729250cfe5198abb36814f5073704a5d31fb76408a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **489.3 MB (489309531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22b46dbb32e5b71640810f230fa6749b7c2d6b43be596cd2052cbfb85bec4c5d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 12 May 2022 22:53:16 GMT
ADD file:3f4e8a0a50db5cf56025980f5849c0c840ba9116680528c507adff04d9287c7e in / 
# Thu, 12 May 2022 22:53:17 GMT
CMD ["/bin/bash"]
# Thu, 12 May 2022 22:53:39 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-505b05ef761a138f8860c413d1520f5756d3a4ea82c5f6052934f3c34a880580.tar.gz"  && echo "bcbcae8a56de8cd107a736a9032b166d5ae7a15c72dbc2e8029ec7ac75d4c5da  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:7516adf672a9b100319b04f4b961b4cc3070ca53af354317e3d80c6a73ca275f`  
		Last Modified: Thu, 12 May 2022 22:55:06 GMT  
		Size: 70.6 MB (70559972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a4b54850ae445fac5d810015c4dce9a59828591287cf034e8d8687a5f42db1`  
		Last Modified: Thu, 12 May 2022 22:55:34 GMT  
		Size: 418.7 MB (418749559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:devel-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:db26696e2371b0e24bc72edf8c118bd9cb18821dfe4f2343495d33eb93aaf2fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **487.9 MB (487866967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7afbb6532b42550d7ce56e9d45b1a30eddbbdf33eef198e4ba4b1123cf9ae38`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 12 May 2022 22:03:11 GMT
ADD file:8406e9d49dfceecd7a1c2cbf960e61dfe58dc85ab0ec500fe43df4123ea56b54 in / 
# Thu, 12 May 2022 22:03:13 GMT
CMD ["/bin/bash"]
# Thu, 12 May 2022 22:03:35 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-505b05ef761a138f8860c413d1520f5756d3a4ea82c5f6052934f3c34a880580.tar.gz"  && echo "bcbcae8a56de8cd107a736a9032b166d5ae7a15c72dbc2e8029ec7ac75d4c5da  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:57916acdbf1d56e1afdf905446c5a93b04658842560d4e5c51a61a1881c5f8b4`  
		Last Modified: Thu, 12 May 2022 22:04:21 GMT  
		Size: 69.1 MB (69117442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f37a59badfcabe5a4ef65d9e6f67b552297ca000f896c8a7f5bffc17447a49`  
		Last Modified: Thu, 12 May 2022 22:05:01 GMT  
		Size: 418.7 MB (418749525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:latest`

```console
$ docker pull amazonlinux@sha256:246ef631c75ea83005889621119fd5cc9cbb5500e193707c38b6c060d597a146
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:latest` - linux; amd64

```console
$ docker pull amazonlinux@sha256:5ca9e45da788e7bac100dffaf45645cea5af68d46f62144f683c0434e14fd586
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62291142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecdeb69c57ad20820ceb442c918b35228a6c9d04d6458768fdf4e86429cbccca`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 May 2022 23:19:31 GMT
ADD file:386c34c6960464ef8f88891333fb091aef731602a28a185a9d6db27726fbe504 in / 
# Tue, 03 May 2022 23:19:32 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8de5b65bd171294b1e04e0df439f4ea11ce923b642eddf3b3d76d297bfd2670c`  
		Last Modified: Mon, 02 May 2022 22:06:03 GMT  
		Size: 62.3 MB (62291142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:latest` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:b1377309830b143f16246542ac234b8b0b9251533954bfb9d3ffd79e2c199901
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63902179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1a0df532d4a93ede0e0da29817f5dfdfb9c6653e22e32388de3149618d47cef`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 May 2022 22:39:32 GMT
ADD file:c351a8c80719ef38e02c26849f50bb7d79c24a6347cc2a72ae1a0768964bd113 in / 
# Tue, 03 May 2022 22:39:34 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ec3b4c26678b188d3874bed5e14dd278311fc05c81e418d5f0da36ec38d9f488`  
		Last Modified: Tue, 03 May 2022 03:07:52 GMT  
		Size: 63.9 MB (63902179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:with-sources`

```console
$ docker pull amazonlinux@sha256:f66f05473f90aa6e14ac926ec03d61af16828a2ff9205fbfa1d3713670b0c166
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:9a3fbba8f30fbd72a0aa0116fd0ef46e8af25d260d01073c266347f116f20399
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **485.7 MB (485712608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6855b0eeeef206786c8c7ac97e546f8677b9d18b2fead70262d5cebc674f86d2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 May 2022 23:19:31 GMT
ADD file:386c34c6960464ef8f88891333fb091aef731602a28a185a9d6db27726fbe504 in / 
# Tue, 03 May 2022 23:19:32 GMT
CMD ["/bin/bash"]
# Tue, 03 May 2022 23:19:53 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-27e5885b1b2e681d27e9e8c451079b8f7f6444b820900db76e8e1f583d454a37.tar.gz"  && echo "fae8bd9cc002cf6ab3af9d777f1bc2646993e0340f2ffac4ddc984a5821a77c2  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:8de5b65bd171294b1e04e0df439f4ea11ce923b642eddf3b3d76d297bfd2670c`  
		Last Modified: Mon, 02 May 2022 22:06:03 GMT  
		Size: 62.3 MB (62291142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab0efe039696303bb91bcd3177af472d1339e2e4cd62297fabd75e1763b9bcb9`  
		Last Modified: Tue, 03 May 2022 23:21:15 GMT  
		Size: 423.4 MB (423421466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:124eb9a22c4bd8d59ea311f776bae5213d1e66db6103732c2c10741bb263f459
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **487.3 MB (487323598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671abfcb4f4c6d925fbecf84883a36ca87a0e7e8aa40bc10b0c3a1678f2b1168`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 May 2022 22:39:32 GMT
ADD file:c351a8c80719ef38e02c26849f50bb7d79c24a6347cc2a72ae1a0768964bd113 in / 
# Tue, 03 May 2022 22:39:34 GMT
CMD ["/bin/bash"]
# Tue, 03 May 2022 22:39:57 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-27e5885b1b2e681d27e9e8c451079b8f7f6444b820900db76e8e1f583d454a37.tar.gz"  && echo "fae8bd9cc002cf6ab3af9d777f1bc2646993e0340f2ffac4ddc984a5821a77c2  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:ec3b4c26678b188d3874bed5e14dd278311fc05c81e418d5f0da36ec38d9f488`  
		Last Modified: Tue, 03 May 2022 03:07:52 GMT  
		Size: 63.9 MB (63902179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189fd58a2d5dc106fd8a0dee23c67eaa14f4c78c0e8fecb154e921df7a05540e`  
		Last Modified: Tue, 03 May 2022 22:41:23 GMT  
		Size: 423.4 MB (423421419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
