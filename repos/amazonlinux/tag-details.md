<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `amazonlinux`

-	[`amazonlinux:1`](#amazonlinux1)
-	[`amazonlinux:1-with-sources`](#amazonlinux1-with-sources)
-	[`amazonlinux:2`](#amazonlinux2)
-	[`amazonlinux:2018.03`](#amazonlinux201803)
-	[`amazonlinux:2018.03.0.20200602.1`](#amazonlinux2018030202006021)
-	[`amazonlinux:2018.03.0.20200602.1-with-sources`](#amazonlinux2018030202006021-with-sources)
-	[`amazonlinux:2018.03-with-sources`](#amazonlinux201803-with-sources)
-	[`amazonlinux:2.0.20200722.0`](#amazonlinux20202007220)
-	[`amazonlinux:2.0.20200722.0-with-sources`](#amazonlinux20202007220-with-sources)
-	[`amazonlinux:2-with-sources`](#amazonlinux2-with-sources)
-	[`amazonlinux:latest`](#amazonlinuxlatest)
-	[`amazonlinux:with-sources`](#amazonlinuxwith-sources)

## `amazonlinux:1`

```console
$ docker pull amazonlinux@sha256:c51f954d859ae9e93f5ecbe8a1132659e39523098b98f9563ffd85b7e1c5cb42
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:1` - linux; amd64

```console
$ docker pull amazonlinux@sha256:7d26828be43385154dc3a82a1f99582aab4393627d42c7fd6f30eb6a53ce1756
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62388725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc9c4a7803b516986783f06f67b1633a79f722a5f1020e13e45b2b25b8eceb54`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Jun 2020 20:20:44 GMT
ADD file:57cbe23b8338dfe8556aa5f457a9536aa0e77d85a240a9fdf983475533103983 in / 
# Tue, 30 Jun 2020 20:20:44 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c9b7c64960cf08ea94a99af6be882845791831279dd11cc6b5e2d822cd07d521`  
		Last Modified: Tue, 30 Jun 2020 20:22:52 GMT  
		Size: 62.4 MB (62388725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:1-with-sources`

```console
$ docker pull amazonlinux@sha256:9176d717c354eac59d8663a7e7ad0104c78ae224c39f1348e0b9876b1adaf127
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:3cf2daadc91456359e4ae9e026c7d4eefe9c8e7de92022934b026e42e53c934b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **449.2 MB (449205154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63bc71b24526296605dbb1eacf91d9fa3044556bff9e493bab7d2fe38fd1c724`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Jun 2020 20:20:44 GMT
ADD file:57cbe23b8338dfe8556aa5f457a9536aa0e77d85a240a9fdf983475533103983 in / 
# Tue, 30 Jun 2020 20:20:44 GMT
CMD ["/bin/bash"]
# Tue, 30 Jun 2020 20:21:04 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-de8e94c334f37301fbb7ac231f1decb67297aa7138fb78c484cf0a2e5f930f11.tar.gz"  && echo "6a4587bb7665170c749dde5bfe60522fec92b691c3e190abd7ac089908fb8ae7  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:c9b7c64960cf08ea94a99af6be882845791831279dd11cc6b5e2d822cd07d521`  
		Last Modified: Tue, 30 Jun 2020 20:22:52 GMT  
		Size: 62.4 MB (62388725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04759c21924907a37db95bd7a1988d1f037bbd8befbc41b5d195d069b993dae0`  
		Last Modified: Tue, 30 Jun 2020 20:23:17 GMT  
		Size: 386.8 MB (386816429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2`

```console
$ docker pull amazonlinux@sha256:76fb97750c68e0531b0c7fa405ecdb591ec78c0be763d04e9db1cbbc6adf2a06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2` - linux; amd64

```console
$ docker pull amazonlinux@sha256:0577d32514319ffd10530dd830b4c572392268581a3306a607d80232e89920ee
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.7 MB (61684682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa0a6a710ca769421fa34c49a9f0f1220bd5806618ae9e3d6ea92624a7c1679b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Jun 2020 20:20:04 GMT
ADD file:788af9048b1c163347d7a8349f8ecf5721b4d8b63395ec8c6ca6d0732f57acdd in / 
# Tue, 30 Jun 2020 20:20:05 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3d24604292f287c31563b1f563e83307e7915909506659401fb07c1c3e6e164c`  
		Last Modified: Tue, 30 Jun 2020 20:21:31 GMT  
		Size: 61.7 MB (61684682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:088e20f837c765a31a68edca3b0de66c41e2dade66f578978eafa449a54b9195
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.2 MB (63163782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7998763f76db6be78121ac805b29d9fcfcd9f9918198a544c56b4c29d977008e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Jun 2020 21:59:07 GMT
ADD file:c597ed16b945b44bdc9a607ac9730b470dd169fb94a5ca4e000d07318157d4f8 in / 
# Tue, 30 Jun 2020 21:59:09 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:6c0fd36c9881cb99dbcd7fe98cfd04a4a653e35c4c1195b7cb7d339eaec9dd79`  
		Last Modified: Tue, 30 Jun 2020 22:00:22 GMT  
		Size: 63.2 MB (63163782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03`

```console
$ docker pull amazonlinux@sha256:c51f954d859ae9e93f5ecbe8a1132659e39523098b98f9563ffd85b7e1c5cb42
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:2018.03` - linux; amd64

```console
$ docker pull amazonlinux@sha256:7d26828be43385154dc3a82a1f99582aab4393627d42c7fd6f30eb6a53ce1756
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62388725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc9c4a7803b516986783f06f67b1633a79f722a5f1020e13e45b2b25b8eceb54`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Jun 2020 20:20:44 GMT
ADD file:57cbe23b8338dfe8556aa5f457a9536aa0e77d85a240a9fdf983475533103983 in / 
# Tue, 30 Jun 2020 20:20:44 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c9b7c64960cf08ea94a99af6be882845791831279dd11cc6b5e2d822cd07d521`  
		Last Modified: Tue, 30 Jun 2020 20:22:52 GMT  
		Size: 62.4 MB (62388725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20200602.1`

```console
$ docker pull amazonlinux@sha256:c51f954d859ae9e93f5ecbe8a1132659e39523098b98f9563ffd85b7e1c5cb42
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:2018.03.0.20200602.1` - linux; amd64

```console
$ docker pull amazonlinux@sha256:7d26828be43385154dc3a82a1f99582aab4393627d42c7fd6f30eb6a53ce1756
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62388725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc9c4a7803b516986783f06f67b1633a79f722a5f1020e13e45b2b25b8eceb54`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Jun 2020 20:20:44 GMT
ADD file:57cbe23b8338dfe8556aa5f457a9536aa0e77d85a240a9fdf983475533103983 in / 
# Tue, 30 Jun 2020 20:20:44 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c9b7c64960cf08ea94a99af6be882845791831279dd11cc6b5e2d822cd07d521`  
		Last Modified: Tue, 30 Jun 2020 20:22:52 GMT  
		Size: 62.4 MB (62388725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20200602.1-with-sources`

```console
$ docker pull amazonlinux@sha256:9176d717c354eac59d8663a7e7ad0104c78ae224c39f1348e0b9876b1adaf127
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:2018.03.0.20200602.1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:3cf2daadc91456359e4ae9e026c7d4eefe9c8e7de92022934b026e42e53c934b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **449.2 MB (449205154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63bc71b24526296605dbb1eacf91d9fa3044556bff9e493bab7d2fe38fd1c724`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Jun 2020 20:20:44 GMT
ADD file:57cbe23b8338dfe8556aa5f457a9536aa0e77d85a240a9fdf983475533103983 in / 
# Tue, 30 Jun 2020 20:20:44 GMT
CMD ["/bin/bash"]
# Tue, 30 Jun 2020 20:21:04 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-de8e94c334f37301fbb7ac231f1decb67297aa7138fb78c484cf0a2e5f930f11.tar.gz"  && echo "6a4587bb7665170c749dde5bfe60522fec92b691c3e190abd7ac089908fb8ae7  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:c9b7c64960cf08ea94a99af6be882845791831279dd11cc6b5e2d822cd07d521`  
		Last Modified: Tue, 30 Jun 2020 20:22:52 GMT  
		Size: 62.4 MB (62388725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04759c21924907a37db95bd7a1988d1f037bbd8befbc41b5d195d069b993dae0`  
		Last Modified: Tue, 30 Jun 2020 20:23:17 GMT  
		Size: 386.8 MB (386816429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03-with-sources`

```console
$ docker pull amazonlinux@sha256:9176d717c354eac59d8663a7e7ad0104c78ae224c39f1348e0b9876b1adaf127
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:2018.03-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:3cf2daadc91456359e4ae9e026c7d4eefe9c8e7de92022934b026e42e53c934b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **449.2 MB (449205154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63bc71b24526296605dbb1eacf91d9fa3044556bff9e493bab7d2fe38fd1c724`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Jun 2020 20:20:44 GMT
ADD file:57cbe23b8338dfe8556aa5f457a9536aa0e77d85a240a9fdf983475533103983 in / 
# Tue, 30 Jun 2020 20:20:44 GMT
CMD ["/bin/bash"]
# Tue, 30 Jun 2020 20:21:04 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-de8e94c334f37301fbb7ac231f1decb67297aa7138fb78c484cf0a2e5f930f11.tar.gz"  && echo "6a4587bb7665170c749dde5bfe60522fec92b691c3e190abd7ac089908fb8ae7  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:c9b7c64960cf08ea94a99af6be882845791831279dd11cc6b5e2d822cd07d521`  
		Last Modified: Tue, 30 Jun 2020 20:22:52 GMT  
		Size: 62.4 MB (62388725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04759c21924907a37db95bd7a1988d1f037bbd8befbc41b5d195d069b993dae0`  
		Last Modified: Tue, 30 Jun 2020 20:23:17 GMT  
		Size: 386.8 MB (386816429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20200722.0`

**does not exist** (yet?)

## `amazonlinux:2.0.20200722.0-with-sources`

**does not exist** (yet?)

## `amazonlinux:2-with-sources`

```console
$ docker pull amazonlinux@sha256:cabd4899d925930e6492d4e7cb8ed7e2fb369e03119a834b072c43b71f348c1d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:420d5d3cfb86d4e124377ab32bc6f9e1504a07d63c0fff4282c49aa7c436c9ec
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **476.9 MB (476922148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d80a4bcf0ffd4b139a9c3d2390bb8b6aa5e6b6aeecef63d6934d908bcde98229`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Jun 2020 20:20:04 GMT
ADD file:788af9048b1c163347d7a8349f8ecf5721b4d8b63395ec8c6ca6d0732f57acdd in / 
# Tue, 30 Jun 2020 20:20:05 GMT
CMD ["/bin/bash"]
# Tue, 30 Jun 2020 20:20:29 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-9af89b3a0cae0f976ef3a0f7b0a0568f88bb8a6a99cb0b19d4c75a7af24fdd7d.tar.gz"  && echo "3d1d16d828b58c8855a5899401da4cbf47e3096cbf2bd798d9a690b9021e2326  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:3d24604292f287c31563b1f563e83307e7915909506659401fb07c1c3e6e164c`  
		Last Modified: Tue, 30 Jun 2020 20:21:31 GMT  
		Size: 61.7 MB (61684682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b36c1db94ea96b1c9c9ff14be0be653f85063ac10bae9324bc5545309ee7fd`  
		Last Modified: Tue, 30 Jun 2020 20:22:34 GMT  
		Size: 415.2 MB (415237466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:89428213350981feb89f90d3d9417e2976391753480a3346dc1fe4a42ea8d250
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **478.4 MB (478401288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a630e3503fb5aabbc497b6e5973256244ca6d91ce3962264478679c2e709cf5b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Jun 2020 21:59:07 GMT
ADD file:c597ed16b945b44bdc9a607ac9730b470dd169fb94a5ca4e000d07318157d4f8 in / 
# Tue, 30 Jun 2020 21:59:09 GMT
CMD ["/bin/bash"]
# Tue, 30 Jun 2020 21:59:48 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-9af89b3a0cae0f976ef3a0f7b0a0568f88bb8a6a99cb0b19d4c75a7af24fdd7d.tar.gz"  && echo "3d1d16d828b58c8855a5899401da4cbf47e3096cbf2bd798d9a690b9021e2326  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:6c0fd36c9881cb99dbcd7fe98cfd04a4a653e35c4c1195b7cb7d339eaec9dd79`  
		Last Modified: Tue, 30 Jun 2020 22:00:22 GMT  
		Size: 63.2 MB (63163782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04069174b6fe5d0ab7681b352a7509678c8561b0fb6c1c9aaeb0acbca7da1d67`  
		Last Modified: Tue, 30 Jun 2020 22:01:09 GMT  
		Size: 415.2 MB (415237506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:latest`

```console
$ docker pull amazonlinux@sha256:76fb97750c68e0531b0c7fa405ecdb591ec78c0be763d04e9db1cbbc6adf2a06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:latest` - linux; amd64

```console
$ docker pull amazonlinux@sha256:0577d32514319ffd10530dd830b4c572392268581a3306a607d80232e89920ee
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.7 MB (61684682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa0a6a710ca769421fa34c49a9f0f1220bd5806618ae9e3d6ea92624a7c1679b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Jun 2020 20:20:04 GMT
ADD file:788af9048b1c163347d7a8349f8ecf5721b4d8b63395ec8c6ca6d0732f57acdd in / 
# Tue, 30 Jun 2020 20:20:05 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3d24604292f287c31563b1f563e83307e7915909506659401fb07c1c3e6e164c`  
		Last Modified: Tue, 30 Jun 2020 20:21:31 GMT  
		Size: 61.7 MB (61684682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:latest` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:088e20f837c765a31a68edca3b0de66c41e2dade66f578978eafa449a54b9195
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.2 MB (63163782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7998763f76db6be78121ac805b29d9fcfcd9f9918198a544c56b4c29d977008e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Jun 2020 21:59:07 GMT
ADD file:c597ed16b945b44bdc9a607ac9730b470dd169fb94a5ca4e000d07318157d4f8 in / 
# Tue, 30 Jun 2020 21:59:09 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:6c0fd36c9881cb99dbcd7fe98cfd04a4a653e35c4c1195b7cb7d339eaec9dd79`  
		Last Modified: Tue, 30 Jun 2020 22:00:22 GMT  
		Size: 63.2 MB (63163782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:with-sources`

```console
$ docker pull amazonlinux@sha256:cabd4899d925930e6492d4e7cb8ed7e2fb369e03119a834b072c43b71f348c1d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:420d5d3cfb86d4e124377ab32bc6f9e1504a07d63c0fff4282c49aa7c436c9ec
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **476.9 MB (476922148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d80a4bcf0ffd4b139a9c3d2390bb8b6aa5e6b6aeecef63d6934d908bcde98229`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Jun 2020 20:20:04 GMT
ADD file:788af9048b1c163347d7a8349f8ecf5721b4d8b63395ec8c6ca6d0732f57acdd in / 
# Tue, 30 Jun 2020 20:20:05 GMT
CMD ["/bin/bash"]
# Tue, 30 Jun 2020 20:20:29 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-9af89b3a0cae0f976ef3a0f7b0a0568f88bb8a6a99cb0b19d4c75a7af24fdd7d.tar.gz"  && echo "3d1d16d828b58c8855a5899401da4cbf47e3096cbf2bd798d9a690b9021e2326  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:3d24604292f287c31563b1f563e83307e7915909506659401fb07c1c3e6e164c`  
		Last Modified: Tue, 30 Jun 2020 20:21:31 GMT  
		Size: 61.7 MB (61684682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b36c1db94ea96b1c9c9ff14be0be653f85063ac10bae9324bc5545309ee7fd`  
		Last Modified: Tue, 30 Jun 2020 20:22:34 GMT  
		Size: 415.2 MB (415237466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:89428213350981feb89f90d3d9417e2976391753480a3346dc1fe4a42ea8d250
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **478.4 MB (478401288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a630e3503fb5aabbc497b6e5973256244ca6d91ce3962264478679c2e709cf5b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Jun 2020 21:59:07 GMT
ADD file:c597ed16b945b44bdc9a607ac9730b470dd169fb94a5ca4e000d07318157d4f8 in / 
# Tue, 30 Jun 2020 21:59:09 GMT
CMD ["/bin/bash"]
# Tue, 30 Jun 2020 21:59:48 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-9af89b3a0cae0f976ef3a0f7b0a0568f88bb8a6a99cb0b19d4c75a7af24fdd7d.tar.gz"  && echo "3d1d16d828b58c8855a5899401da4cbf47e3096cbf2bd798d9a690b9021e2326  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:6c0fd36c9881cb99dbcd7fe98cfd04a4a653e35c4c1195b7cb7d339eaec9dd79`  
		Last Modified: Tue, 30 Jun 2020 22:00:22 GMT  
		Size: 63.2 MB (63163782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04069174b6fe5d0ab7681b352a7509678c8561b0fb6c1c9aaeb0acbca7da1d67`  
		Last Modified: Tue, 30 Jun 2020 22:01:09 GMT  
		Size: 415.2 MB (415237506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
