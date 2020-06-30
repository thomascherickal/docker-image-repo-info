<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `amazonlinux`

-	[`amazonlinux:1`](#amazonlinux1)
-	[`amazonlinux:1-with-sources`](#amazonlinux1-with-sources)
-	[`amazonlinux:2`](#amazonlinux2)
-	[`amazonlinux:2018.03`](#amazonlinux201803)
-	[`amazonlinux:2018.03.0.20200602.1`](#amazonlinux2018030202006021)
-	[`amazonlinux:2018.03.0.20200602.1-with-sources`](#amazonlinux2018030202006021-with-sources)
-	[`amazonlinux:2018.03-with-sources`](#amazonlinux201803-with-sources)
-	[`amazonlinux:2.0.20200602.0`](#amazonlinux20202006020)
-	[`amazonlinux:2.0.20200602.0-with-sources`](#amazonlinux20202006020-with-sources)
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
$ docker pull amazonlinux@sha256:c101215e235f1306e99fc458ad42e0268cc230685e6329f807c32ff603d6a799
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
$ docker pull amazonlinux@sha256:64e35bbe6ac618aef32fc4924b8ab8b576d6085056a285dc311b07ec9138e8c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.1 MB (63079760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c39751b5fb90d450e678e5b9f4403d064d2e730da6c334f7ddcc4c4ffb4a4f33`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Apr 2020 18:58:16 GMT
ADD file:85fc0908f460f80c41755d2b5ab9ff6a025bb2726628ccc4edceb21d2e3f8edf in / 
# Tue, 21 Apr 2020 18:58:18 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0a37a5cd26f245ce54aff575389ef7765520d37d3ea7c437144c936c6adffc8a`  
		Last Modified: Tue, 21 Apr 2020 18:59:54 GMT  
		Size: 63.1 MB (63079760 bytes)  
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

## `amazonlinux:2.0.20200602.0`

```console
$ docker pull amazonlinux@sha256:3f6b711fafaa95348d871b0bf587005f92d1b4a7aa0271c6c2ff884c56c53f5b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:2.0.20200602.0` - linux; amd64

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

## `amazonlinux:2.0.20200602.0-with-sources`

```console
$ docker pull amazonlinux@sha256:0277e63b7b171c97bce713866ce2b1f919ef941b9a33d29e952a2fee31f8e37a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:2.0.20200602.0-with-sources` - linux; amd64

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

## `amazonlinux:2-with-sources`

```console
$ docker pull amazonlinux@sha256:fdf45395e6e6ee2e6fc5cd412c489015a8b9b29df656858b326f3c66f2230671
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
$ docker pull amazonlinux@sha256:4cbc0732124bed6fdb615eaf60c2d4bb7cc134d957d1f9674dc0066a438ce1bc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **478.2 MB (478219309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aca4e24672d702283a87cbf97240f20bed3724d62ff8f8dcfb9a0baed82da19a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Apr 2020 18:58:16 GMT
ADD file:85fc0908f460f80c41755d2b5ab9ff6a025bb2726628ccc4edceb21d2e3f8edf in / 
# Tue, 21 Apr 2020 18:58:18 GMT
CMD ["/bin/bash"]
# Tue, 21 Apr 2020 18:59:09 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-44ab891c498d922bb21e90b6006b12c7f05381ec7e67aba05bb535aae3b261b1.tar.gz"  && echo "a1b70378c6175331c9daa5bee79c8cb36dab14ed1fb0d02bfd33254652f0b846  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:0a37a5cd26f245ce54aff575389ef7765520d37d3ea7c437144c936c6adffc8a`  
		Last Modified: Tue, 21 Apr 2020 18:59:54 GMT  
		Size: 63.1 MB (63079760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4f9d710835018ff01a17ccc9e3b4ce18e9cf9f81a0dc1cf8d455472d9a1d29`  
		Last Modified: Tue, 21 Apr 2020 19:00:52 GMT  
		Size: 415.1 MB (415139549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:latest`

```console
$ docker pull amazonlinux@sha256:c101215e235f1306e99fc458ad42e0268cc230685e6329f807c32ff603d6a799
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
$ docker pull amazonlinux@sha256:64e35bbe6ac618aef32fc4924b8ab8b576d6085056a285dc311b07ec9138e8c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.1 MB (63079760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c39751b5fb90d450e678e5b9f4403d064d2e730da6c334f7ddcc4c4ffb4a4f33`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Apr 2020 18:58:16 GMT
ADD file:85fc0908f460f80c41755d2b5ab9ff6a025bb2726628ccc4edceb21d2e3f8edf in / 
# Tue, 21 Apr 2020 18:58:18 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0a37a5cd26f245ce54aff575389ef7765520d37d3ea7c437144c936c6adffc8a`  
		Last Modified: Tue, 21 Apr 2020 18:59:54 GMT  
		Size: 63.1 MB (63079760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:with-sources`

```console
$ docker pull amazonlinux@sha256:fdf45395e6e6ee2e6fc5cd412c489015a8b9b29df656858b326f3c66f2230671
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
$ docker pull amazonlinux@sha256:4cbc0732124bed6fdb615eaf60c2d4bb7cc134d957d1f9674dc0066a438ce1bc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **478.2 MB (478219309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aca4e24672d702283a87cbf97240f20bed3724d62ff8f8dcfb9a0baed82da19a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Apr 2020 18:58:16 GMT
ADD file:85fc0908f460f80c41755d2b5ab9ff6a025bb2726628ccc4edceb21d2e3f8edf in / 
# Tue, 21 Apr 2020 18:58:18 GMT
CMD ["/bin/bash"]
# Tue, 21 Apr 2020 18:59:09 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-44ab891c498d922bb21e90b6006b12c7f05381ec7e67aba05bb535aae3b261b1.tar.gz"  && echo "a1b70378c6175331c9daa5bee79c8cb36dab14ed1fb0d02bfd33254652f0b846  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:0a37a5cd26f245ce54aff575389ef7765520d37d3ea7c437144c936c6adffc8a`  
		Last Modified: Tue, 21 Apr 2020 18:59:54 GMT  
		Size: 63.1 MB (63079760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4f9d710835018ff01a17ccc9e3b4ce18e9cf9f81a0dc1cf8d455472d9a1d29`  
		Last Modified: Tue, 21 Apr 2020 19:00:52 GMT  
		Size: 415.1 MB (415139549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
