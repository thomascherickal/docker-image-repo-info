<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mono`

-	[`mono:5`](#mono5)
-	[`mono:5.20`](#mono520)
-	[`mono:5.20.1`](#mono5201)
-	[`mono:5.20.1.34`](#mono520134)
-	[`mono:5.20.1.34-slim`](#mono520134-slim)
-	[`mono:5.20.1-slim`](#mono5201-slim)
-	[`mono:5.20-slim`](#mono520-slim)
-	[`mono:5-slim`](#mono5-slim)
-	[`mono:6`](#mono6)
-	[`mono:6.4`](#mono64)
-	[`mono:6.4.0`](#mono640)
-	[`mono:6.4.0.198`](#mono640198)
-	[`mono:6.4.0.198-slim`](#mono640198-slim)
-	[`mono:6.4.0-slim`](#mono640-slim)
-	[`mono:6.4-slim`](#mono64-slim)
-	[`mono:6.6`](#mono66)
-	[`mono:6.6.0`](#mono660)
-	[`mono:6.6.0.161`](#mono660161)
-	[`mono:6.6.0.161-slim`](#mono660161-slim)
-	[`mono:6.6.0-slim`](#mono660-slim)
-	[`mono:6.6-slim`](#mono66-slim)
-	[`mono:6-slim`](#mono6-slim)
-	[`mono:latest`](#monolatest)
-	[`mono:slim`](#monoslim)

## `mono:5`

```console
$ docker pull mono@sha256:53dcdf176ceb5ed6ac9f8a0b999bd4e6859b4892f6d5a2a76e00ee6a00c44b58
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:5` - linux; amd64

```console
$ docker pull mono@sha256:f7a803fe550efe9aef81e8a44e8a43729c816b850f2e49040a7e081593700c1f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.3 MB (218283730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8aea3091220b44022c0f20929d510fe88b3cc4cdcde3057a185c15a282df8301`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:59:24 GMT
ADD file:2c1f5e08834f13ccb9c2326204eb2556e03239d00171e75755c7195289374c61 in / 
# Fri, 22 Nov 2019 14:59:25 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 23:00:40 GMT
ENV MONO_VERSION=5.20.1.34
# Fri, 22 Nov 2019 23:00:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 22 Nov 2019 23:01:21 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 22 Nov 2019 23:19:59 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d599a449871ee73b960e80d176b989365dfecb4c8f337bf21e8853862403ee9b`  
		Last Modified: Fri, 22 Nov 2019 15:06:36 GMT  
		Size: 22.5 MB (22524572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a778528e98113a69fcb62273f311379c55bd8759ce0e9ceeaedb433d4526e4a`  
		Last Modified: Fri, 22 Nov 2019 23:20:53 GMT  
		Size: 244.5 KB (244453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b697dbbf0ffb85ff1635ce5da0576d788dec98d69f5be271d5283cb190995d4d`  
		Last Modified: Fri, 22 Nov 2019 23:21:06 GMT  
		Size: 55.5 MB (55521485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b21954383b73fbad8beeae6b731b48d025852b1d498453b26562e7bfa977c7`  
		Last Modified: Fri, 22 Nov 2019 23:22:54 GMT  
		Size: 140.0 MB (139993220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5` - linux; arm variant v5

```console
$ docker pull mono@sha256:921141ae8dd056ee2c6ab66dde3ee626f76ecebd3941aaef44a81385fa7eb3e6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.0 MB (170952313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3270863ca29345901057a594ed47d2cb0e53b9b46570af2b4297f3a0e092cfa3`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:53:16 GMT
ADD file:7d6af454b55cb354e31c096e935358dd5914688ded04ebc76243a4ff598c4495 in / 
# Sat, 28 Dec 2019 04:53:18 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:31:47 GMT
ENV MONO_VERSION=5.20.1.34
# Sat, 28 Dec 2019 07:32:25 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:33:38 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 28 Dec 2019 07:43:54 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af28f499fd964f4506ea46c2ac342bc52328a8c30cd633661b69f383a5144e9b`  
		Last Modified: Sat, 28 Dec 2019 05:00:23 GMT  
		Size: 21.2 MB (21202822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e30f4dec85338cf63b2a0a4635e2307d966fbfa5356fe9e83d6a9bcf294768c4`  
		Last Modified: Sat, 28 Dec 2019 07:44:59 GMT  
		Size: 244.6 KB (244563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d859f970551d160b36092ef79b226a92798c6c82b5610774fb345988f6ab6cb`  
		Last Modified: Sat, 28 Dec 2019 07:45:08 GMT  
		Size: 24.3 MB (24265462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb69e22f6d5bc15e3d4811d51cca77b50460d4f38ad4131151a2df9b8fee768`  
		Last Modified: Sat, 28 Dec 2019 07:48:01 GMT  
		Size: 125.2 MB (125239466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5` - linux; arm variant v7

```console
$ docker pull mono@sha256:ea5d643ecc5f26c0f9f1edeb49fee6ea5323762e8727d392a1f813c4b8862460
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.0 MB (167004578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:631abf1b9406641e5331da51a0d793dd163877e353aece2468f77d0b962d5775`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 05:03:51 GMT
ADD file:2002ba672e32ae75369830ed6a4734ce62e0118e42390b4d657f0985d6b7fd6a in / 
# Sat, 28 Dec 2019 05:03:53 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:39:44 GMT
ENV MONO_VERSION=5.20.1.34
# Sat, 28 Dec 2019 07:40:06 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:40:54 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 28 Dec 2019 07:50:10 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:77cf262539006c8df77496f500f74a8c1edd158062440fd94d43d5b1292cefee`  
		Last Modified: Sat, 28 Dec 2019 05:11:13 GMT  
		Size: 19.3 MB (19311587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d99eb936b9cc5835bf59846bd4e0ae6c236cda6f4adce2cb3d14125cb51956`  
		Last Modified: Sat, 28 Dec 2019 07:51:22 GMT  
		Size: 244.6 KB (244557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fd6bf39cd6ba01aa22f88d8bed99d3c486440b3a5a1d22c82716aa505d7702`  
		Last Modified: Sat, 28 Dec 2019 07:51:30 GMT  
		Size: 23.6 MB (23561478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a7e7be5a6639501eb7d74f9ca29ade62656f3ca932b2c23aaca5ff7ea944c5`  
		Last Modified: Sat, 28 Dec 2019 07:54:12 GMT  
		Size: 123.9 MB (123886956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:5bfa6d768088cbca6586d03476e2eb7eb2eb2ea0fb7370a6fa5a87759bf22585
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.8 MB (187815600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c75f84637df2a208fba18263667843579351fb12ec432b5865f8b6eddd963ba5`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:50 GMT
ADD file:8e4d0a1e6805c641fc9d18ebad82e4b01d85c6cb9f87d1ef47d75d150212a392 in / 
# Fri, 22 Nov 2019 13:45:53 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 20:56:16 GMT
ENV MONO_VERSION=5.20.1.34
# Fri, 22 Nov 2019 20:56:36 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 22 Nov 2019 20:57:14 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 22 Nov 2019 21:07:37 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:98a64bf4db7d2219b4fdd8182188d9422810dee890e997095bfb564a0482eed6`  
		Last Modified: Fri, 22 Nov 2019 13:52:17 GMT  
		Size: 20.4 MB (20385759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d1f78621344e3d91b8757cd69682a85fcacf7b02a199108cef35d380060188`  
		Last Modified: Fri, 22 Nov 2019 21:08:54 GMT  
		Size: 244.4 KB (244405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12210f2195af5163abba98ca92acf6283bf09e73698d41cee74183f5402ce55`  
		Last Modified: Fri, 22 Nov 2019 21:09:03 GMT  
		Size: 28.2 MB (28156046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a7680edeae996703f6ee15ad4398d036c169866908acbb816410973a13de969`  
		Last Modified: Fri, 22 Nov 2019 21:11:52 GMT  
		Size: 139.0 MB (139029390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5` - linux; 386

```console
$ docker pull mono@sha256:ec9d6818f5778553dfef85050a25e2cb122b90b5b06d537e5874e70a54bda52d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.8 MB (227782795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:358a8ef155cd2f22c5a4151a7c72c80bdefe7a456ffafae9a33de702305eb44a`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 16:54:44 GMT
ADD file:19d04f738434c76e2dbd14b48de2f0f03afa883b15f638c6ecbbf382df03567c in / 
# Fri, 22 Nov 2019 16:54:44 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 01:09:08 GMT
ENV MONO_VERSION=5.20.1.34
# Sat, 23 Nov 2019 01:09:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 23 Nov 2019 01:09:51 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 23 Nov 2019 01:16:25 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f26c9a85c76e393c9f2313b30e82d09f933d2dd4883620de242c7d21f8812e91`  
		Last Modified: Fri, 22 Nov 2019 17:03:03 GMT  
		Size: 23.2 MB (23152070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17fdd7c327a6ddaec1d04dab27737393102e01ec89d0f21c4dedee4e86eb1f34`  
		Last Modified: Sat, 23 Nov 2019 01:17:31 GMT  
		Size: 244.5 KB (244482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2816ec1c0521b0d2a95dd902cbe502786519966ce0073eb6de1bf01d58bd90c3`  
		Last Modified: Sat, 23 Nov 2019 01:17:48 GMT  
		Size: 58.6 MB (58552039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:064c1b59b86a05462dd6cae5082b0af2f54cb64d012af553452de527389b3b97`  
		Last Modified: Sat, 23 Nov 2019 01:20:16 GMT  
		Size: 145.8 MB (145834204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5` - linux; ppc64le

```console
$ docker pull mono@sha256:b414ce326f06449a5a441ad050f57286bf41f79b0e0130a25928f9f9617f3e8e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.3 MB (173304358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee71b36f2a14a9487be1b834ccb9a4c1682b90900f74f6a88ba2a4c937fa4272`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:21 GMT
ADD file:a1ee5955ff3ede8df9558f4bec0c7962d54c43374f857e1da7e2639ddf82a9f1 in / 
# Sat, 28 Dec 2019 04:23:24 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:05:00 GMT
ENV MONO_VERSION=5.20.1.34
# Sat, 28 Dec 2019 06:05:42 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 06:06:42 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 28 Dec 2019 06:21:25 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af52e7ef6e83efadeae17be91daa6ecf61b7dfb39709c29be9b24876e60c0e36`  
		Last Modified: Sat, 28 Dec 2019 04:33:19 GMT  
		Size: 22.8 MB (22800791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:657bad46700417171f7961a2ff50ecc946522119a9a065f23416906ee79d822d`  
		Last Modified: Sat, 28 Dec 2019 06:22:56 GMT  
		Size: 244.5 KB (244499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c9779877dadfcd9c157fa02d2fbd6becf203c18e9c2727702df72179644d61`  
		Last Modified: Sat, 28 Dec 2019 06:23:14 GMT  
		Size: 24.6 MB (24638971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f31ee19914bb9f2e2b65604baa6905997d5f54e1d4012f6ed60ed63ad1b3c735`  
		Last Modified: Sat, 28 Dec 2019 06:25:31 GMT  
		Size: 125.6 MB (125620097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.20`

```console
$ docker pull mono@sha256:53dcdf176ceb5ed6ac9f8a0b999bd4e6859b4892f6d5a2a76e00ee6a00c44b58
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:5.20` - linux; amd64

```console
$ docker pull mono@sha256:f7a803fe550efe9aef81e8a44e8a43729c816b850f2e49040a7e081593700c1f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.3 MB (218283730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8aea3091220b44022c0f20929d510fe88b3cc4cdcde3057a185c15a282df8301`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:59:24 GMT
ADD file:2c1f5e08834f13ccb9c2326204eb2556e03239d00171e75755c7195289374c61 in / 
# Fri, 22 Nov 2019 14:59:25 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 23:00:40 GMT
ENV MONO_VERSION=5.20.1.34
# Fri, 22 Nov 2019 23:00:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 22 Nov 2019 23:01:21 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 22 Nov 2019 23:19:59 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d599a449871ee73b960e80d176b989365dfecb4c8f337bf21e8853862403ee9b`  
		Last Modified: Fri, 22 Nov 2019 15:06:36 GMT  
		Size: 22.5 MB (22524572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a778528e98113a69fcb62273f311379c55bd8759ce0e9ceeaedb433d4526e4a`  
		Last Modified: Fri, 22 Nov 2019 23:20:53 GMT  
		Size: 244.5 KB (244453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b697dbbf0ffb85ff1635ce5da0576d788dec98d69f5be271d5283cb190995d4d`  
		Last Modified: Fri, 22 Nov 2019 23:21:06 GMT  
		Size: 55.5 MB (55521485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b21954383b73fbad8beeae6b731b48d025852b1d498453b26562e7bfa977c7`  
		Last Modified: Fri, 22 Nov 2019 23:22:54 GMT  
		Size: 140.0 MB (139993220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20` - linux; arm variant v5

```console
$ docker pull mono@sha256:921141ae8dd056ee2c6ab66dde3ee626f76ecebd3941aaef44a81385fa7eb3e6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.0 MB (170952313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3270863ca29345901057a594ed47d2cb0e53b9b46570af2b4297f3a0e092cfa3`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:53:16 GMT
ADD file:7d6af454b55cb354e31c096e935358dd5914688ded04ebc76243a4ff598c4495 in / 
# Sat, 28 Dec 2019 04:53:18 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:31:47 GMT
ENV MONO_VERSION=5.20.1.34
# Sat, 28 Dec 2019 07:32:25 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:33:38 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 28 Dec 2019 07:43:54 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af28f499fd964f4506ea46c2ac342bc52328a8c30cd633661b69f383a5144e9b`  
		Last Modified: Sat, 28 Dec 2019 05:00:23 GMT  
		Size: 21.2 MB (21202822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e30f4dec85338cf63b2a0a4635e2307d966fbfa5356fe9e83d6a9bcf294768c4`  
		Last Modified: Sat, 28 Dec 2019 07:44:59 GMT  
		Size: 244.6 KB (244563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d859f970551d160b36092ef79b226a92798c6c82b5610774fb345988f6ab6cb`  
		Last Modified: Sat, 28 Dec 2019 07:45:08 GMT  
		Size: 24.3 MB (24265462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb69e22f6d5bc15e3d4811d51cca77b50460d4f38ad4131151a2df9b8fee768`  
		Last Modified: Sat, 28 Dec 2019 07:48:01 GMT  
		Size: 125.2 MB (125239466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20` - linux; arm variant v7

```console
$ docker pull mono@sha256:ea5d643ecc5f26c0f9f1edeb49fee6ea5323762e8727d392a1f813c4b8862460
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.0 MB (167004578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:631abf1b9406641e5331da51a0d793dd163877e353aece2468f77d0b962d5775`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 05:03:51 GMT
ADD file:2002ba672e32ae75369830ed6a4734ce62e0118e42390b4d657f0985d6b7fd6a in / 
# Sat, 28 Dec 2019 05:03:53 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:39:44 GMT
ENV MONO_VERSION=5.20.1.34
# Sat, 28 Dec 2019 07:40:06 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:40:54 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 28 Dec 2019 07:50:10 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:77cf262539006c8df77496f500f74a8c1edd158062440fd94d43d5b1292cefee`  
		Last Modified: Sat, 28 Dec 2019 05:11:13 GMT  
		Size: 19.3 MB (19311587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d99eb936b9cc5835bf59846bd4e0ae6c236cda6f4adce2cb3d14125cb51956`  
		Last Modified: Sat, 28 Dec 2019 07:51:22 GMT  
		Size: 244.6 KB (244557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fd6bf39cd6ba01aa22f88d8bed99d3c486440b3a5a1d22c82716aa505d7702`  
		Last Modified: Sat, 28 Dec 2019 07:51:30 GMT  
		Size: 23.6 MB (23561478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a7e7be5a6639501eb7d74f9ca29ade62656f3ca932b2c23aaca5ff7ea944c5`  
		Last Modified: Sat, 28 Dec 2019 07:54:12 GMT  
		Size: 123.9 MB (123886956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:5bfa6d768088cbca6586d03476e2eb7eb2eb2ea0fb7370a6fa5a87759bf22585
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.8 MB (187815600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c75f84637df2a208fba18263667843579351fb12ec432b5865f8b6eddd963ba5`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:50 GMT
ADD file:8e4d0a1e6805c641fc9d18ebad82e4b01d85c6cb9f87d1ef47d75d150212a392 in / 
# Fri, 22 Nov 2019 13:45:53 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 20:56:16 GMT
ENV MONO_VERSION=5.20.1.34
# Fri, 22 Nov 2019 20:56:36 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 22 Nov 2019 20:57:14 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 22 Nov 2019 21:07:37 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:98a64bf4db7d2219b4fdd8182188d9422810dee890e997095bfb564a0482eed6`  
		Last Modified: Fri, 22 Nov 2019 13:52:17 GMT  
		Size: 20.4 MB (20385759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d1f78621344e3d91b8757cd69682a85fcacf7b02a199108cef35d380060188`  
		Last Modified: Fri, 22 Nov 2019 21:08:54 GMT  
		Size: 244.4 KB (244405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12210f2195af5163abba98ca92acf6283bf09e73698d41cee74183f5402ce55`  
		Last Modified: Fri, 22 Nov 2019 21:09:03 GMT  
		Size: 28.2 MB (28156046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a7680edeae996703f6ee15ad4398d036c169866908acbb816410973a13de969`  
		Last Modified: Fri, 22 Nov 2019 21:11:52 GMT  
		Size: 139.0 MB (139029390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20` - linux; 386

```console
$ docker pull mono@sha256:ec9d6818f5778553dfef85050a25e2cb122b90b5b06d537e5874e70a54bda52d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.8 MB (227782795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:358a8ef155cd2f22c5a4151a7c72c80bdefe7a456ffafae9a33de702305eb44a`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 16:54:44 GMT
ADD file:19d04f738434c76e2dbd14b48de2f0f03afa883b15f638c6ecbbf382df03567c in / 
# Fri, 22 Nov 2019 16:54:44 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 01:09:08 GMT
ENV MONO_VERSION=5.20.1.34
# Sat, 23 Nov 2019 01:09:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 23 Nov 2019 01:09:51 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 23 Nov 2019 01:16:25 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f26c9a85c76e393c9f2313b30e82d09f933d2dd4883620de242c7d21f8812e91`  
		Last Modified: Fri, 22 Nov 2019 17:03:03 GMT  
		Size: 23.2 MB (23152070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17fdd7c327a6ddaec1d04dab27737393102e01ec89d0f21c4dedee4e86eb1f34`  
		Last Modified: Sat, 23 Nov 2019 01:17:31 GMT  
		Size: 244.5 KB (244482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2816ec1c0521b0d2a95dd902cbe502786519966ce0073eb6de1bf01d58bd90c3`  
		Last Modified: Sat, 23 Nov 2019 01:17:48 GMT  
		Size: 58.6 MB (58552039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:064c1b59b86a05462dd6cae5082b0af2f54cb64d012af553452de527389b3b97`  
		Last Modified: Sat, 23 Nov 2019 01:20:16 GMT  
		Size: 145.8 MB (145834204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20` - linux; ppc64le

```console
$ docker pull mono@sha256:b414ce326f06449a5a441ad050f57286bf41f79b0e0130a25928f9f9617f3e8e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.3 MB (173304358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee71b36f2a14a9487be1b834ccb9a4c1682b90900f74f6a88ba2a4c937fa4272`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:21 GMT
ADD file:a1ee5955ff3ede8df9558f4bec0c7962d54c43374f857e1da7e2639ddf82a9f1 in / 
# Sat, 28 Dec 2019 04:23:24 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:05:00 GMT
ENV MONO_VERSION=5.20.1.34
# Sat, 28 Dec 2019 06:05:42 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 06:06:42 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 28 Dec 2019 06:21:25 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af52e7ef6e83efadeae17be91daa6ecf61b7dfb39709c29be9b24876e60c0e36`  
		Last Modified: Sat, 28 Dec 2019 04:33:19 GMT  
		Size: 22.8 MB (22800791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:657bad46700417171f7961a2ff50ecc946522119a9a065f23416906ee79d822d`  
		Last Modified: Sat, 28 Dec 2019 06:22:56 GMT  
		Size: 244.5 KB (244499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c9779877dadfcd9c157fa02d2fbd6becf203c18e9c2727702df72179644d61`  
		Last Modified: Sat, 28 Dec 2019 06:23:14 GMT  
		Size: 24.6 MB (24638971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f31ee19914bb9f2e2b65604baa6905997d5f54e1d4012f6ed60ed63ad1b3c735`  
		Last Modified: Sat, 28 Dec 2019 06:25:31 GMT  
		Size: 125.6 MB (125620097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.20.1`

```console
$ docker pull mono@sha256:53dcdf176ceb5ed6ac9f8a0b999bd4e6859b4892f6d5a2a76e00ee6a00c44b58
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:5.20.1` - linux; amd64

```console
$ docker pull mono@sha256:f7a803fe550efe9aef81e8a44e8a43729c816b850f2e49040a7e081593700c1f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.3 MB (218283730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8aea3091220b44022c0f20929d510fe88b3cc4cdcde3057a185c15a282df8301`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:59:24 GMT
ADD file:2c1f5e08834f13ccb9c2326204eb2556e03239d00171e75755c7195289374c61 in / 
# Fri, 22 Nov 2019 14:59:25 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 23:00:40 GMT
ENV MONO_VERSION=5.20.1.34
# Fri, 22 Nov 2019 23:00:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 22 Nov 2019 23:01:21 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 22 Nov 2019 23:19:59 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d599a449871ee73b960e80d176b989365dfecb4c8f337bf21e8853862403ee9b`  
		Last Modified: Fri, 22 Nov 2019 15:06:36 GMT  
		Size: 22.5 MB (22524572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a778528e98113a69fcb62273f311379c55bd8759ce0e9ceeaedb433d4526e4a`  
		Last Modified: Fri, 22 Nov 2019 23:20:53 GMT  
		Size: 244.5 KB (244453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b697dbbf0ffb85ff1635ce5da0576d788dec98d69f5be271d5283cb190995d4d`  
		Last Modified: Fri, 22 Nov 2019 23:21:06 GMT  
		Size: 55.5 MB (55521485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b21954383b73fbad8beeae6b731b48d025852b1d498453b26562e7bfa977c7`  
		Last Modified: Fri, 22 Nov 2019 23:22:54 GMT  
		Size: 140.0 MB (139993220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1` - linux; arm variant v5

```console
$ docker pull mono@sha256:921141ae8dd056ee2c6ab66dde3ee626f76ecebd3941aaef44a81385fa7eb3e6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.0 MB (170952313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3270863ca29345901057a594ed47d2cb0e53b9b46570af2b4297f3a0e092cfa3`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:53:16 GMT
ADD file:7d6af454b55cb354e31c096e935358dd5914688ded04ebc76243a4ff598c4495 in / 
# Sat, 28 Dec 2019 04:53:18 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:31:47 GMT
ENV MONO_VERSION=5.20.1.34
# Sat, 28 Dec 2019 07:32:25 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:33:38 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 28 Dec 2019 07:43:54 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af28f499fd964f4506ea46c2ac342bc52328a8c30cd633661b69f383a5144e9b`  
		Last Modified: Sat, 28 Dec 2019 05:00:23 GMT  
		Size: 21.2 MB (21202822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e30f4dec85338cf63b2a0a4635e2307d966fbfa5356fe9e83d6a9bcf294768c4`  
		Last Modified: Sat, 28 Dec 2019 07:44:59 GMT  
		Size: 244.6 KB (244563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d859f970551d160b36092ef79b226a92798c6c82b5610774fb345988f6ab6cb`  
		Last Modified: Sat, 28 Dec 2019 07:45:08 GMT  
		Size: 24.3 MB (24265462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb69e22f6d5bc15e3d4811d51cca77b50460d4f38ad4131151a2df9b8fee768`  
		Last Modified: Sat, 28 Dec 2019 07:48:01 GMT  
		Size: 125.2 MB (125239466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1` - linux; arm variant v7

```console
$ docker pull mono@sha256:ea5d643ecc5f26c0f9f1edeb49fee6ea5323762e8727d392a1f813c4b8862460
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.0 MB (167004578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:631abf1b9406641e5331da51a0d793dd163877e353aece2468f77d0b962d5775`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 05:03:51 GMT
ADD file:2002ba672e32ae75369830ed6a4734ce62e0118e42390b4d657f0985d6b7fd6a in / 
# Sat, 28 Dec 2019 05:03:53 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:39:44 GMT
ENV MONO_VERSION=5.20.1.34
# Sat, 28 Dec 2019 07:40:06 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:40:54 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 28 Dec 2019 07:50:10 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:77cf262539006c8df77496f500f74a8c1edd158062440fd94d43d5b1292cefee`  
		Last Modified: Sat, 28 Dec 2019 05:11:13 GMT  
		Size: 19.3 MB (19311587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d99eb936b9cc5835bf59846bd4e0ae6c236cda6f4adce2cb3d14125cb51956`  
		Last Modified: Sat, 28 Dec 2019 07:51:22 GMT  
		Size: 244.6 KB (244557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fd6bf39cd6ba01aa22f88d8bed99d3c486440b3a5a1d22c82716aa505d7702`  
		Last Modified: Sat, 28 Dec 2019 07:51:30 GMT  
		Size: 23.6 MB (23561478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a7e7be5a6639501eb7d74f9ca29ade62656f3ca932b2c23aaca5ff7ea944c5`  
		Last Modified: Sat, 28 Dec 2019 07:54:12 GMT  
		Size: 123.9 MB (123886956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:5bfa6d768088cbca6586d03476e2eb7eb2eb2ea0fb7370a6fa5a87759bf22585
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.8 MB (187815600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c75f84637df2a208fba18263667843579351fb12ec432b5865f8b6eddd963ba5`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:50 GMT
ADD file:8e4d0a1e6805c641fc9d18ebad82e4b01d85c6cb9f87d1ef47d75d150212a392 in / 
# Fri, 22 Nov 2019 13:45:53 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 20:56:16 GMT
ENV MONO_VERSION=5.20.1.34
# Fri, 22 Nov 2019 20:56:36 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 22 Nov 2019 20:57:14 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 22 Nov 2019 21:07:37 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:98a64bf4db7d2219b4fdd8182188d9422810dee890e997095bfb564a0482eed6`  
		Last Modified: Fri, 22 Nov 2019 13:52:17 GMT  
		Size: 20.4 MB (20385759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d1f78621344e3d91b8757cd69682a85fcacf7b02a199108cef35d380060188`  
		Last Modified: Fri, 22 Nov 2019 21:08:54 GMT  
		Size: 244.4 KB (244405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12210f2195af5163abba98ca92acf6283bf09e73698d41cee74183f5402ce55`  
		Last Modified: Fri, 22 Nov 2019 21:09:03 GMT  
		Size: 28.2 MB (28156046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a7680edeae996703f6ee15ad4398d036c169866908acbb816410973a13de969`  
		Last Modified: Fri, 22 Nov 2019 21:11:52 GMT  
		Size: 139.0 MB (139029390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1` - linux; 386

```console
$ docker pull mono@sha256:ec9d6818f5778553dfef85050a25e2cb122b90b5b06d537e5874e70a54bda52d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.8 MB (227782795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:358a8ef155cd2f22c5a4151a7c72c80bdefe7a456ffafae9a33de702305eb44a`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 16:54:44 GMT
ADD file:19d04f738434c76e2dbd14b48de2f0f03afa883b15f638c6ecbbf382df03567c in / 
# Fri, 22 Nov 2019 16:54:44 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 01:09:08 GMT
ENV MONO_VERSION=5.20.1.34
# Sat, 23 Nov 2019 01:09:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 23 Nov 2019 01:09:51 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 23 Nov 2019 01:16:25 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f26c9a85c76e393c9f2313b30e82d09f933d2dd4883620de242c7d21f8812e91`  
		Last Modified: Fri, 22 Nov 2019 17:03:03 GMT  
		Size: 23.2 MB (23152070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17fdd7c327a6ddaec1d04dab27737393102e01ec89d0f21c4dedee4e86eb1f34`  
		Last Modified: Sat, 23 Nov 2019 01:17:31 GMT  
		Size: 244.5 KB (244482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2816ec1c0521b0d2a95dd902cbe502786519966ce0073eb6de1bf01d58bd90c3`  
		Last Modified: Sat, 23 Nov 2019 01:17:48 GMT  
		Size: 58.6 MB (58552039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:064c1b59b86a05462dd6cae5082b0af2f54cb64d012af553452de527389b3b97`  
		Last Modified: Sat, 23 Nov 2019 01:20:16 GMT  
		Size: 145.8 MB (145834204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1` - linux; ppc64le

```console
$ docker pull mono@sha256:b414ce326f06449a5a441ad050f57286bf41f79b0e0130a25928f9f9617f3e8e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.3 MB (173304358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee71b36f2a14a9487be1b834ccb9a4c1682b90900f74f6a88ba2a4c937fa4272`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:21 GMT
ADD file:a1ee5955ff3ede8df9558f4bec0c7962d54c43374f857e1da7e2639ddf82a9f1 in / 
# Sat, 28 Dec 2019 04:23:24 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:05:00 GMT
ENV MONO_VERSION=5.20.1.34
# Sat, 28 Dec 2019 06:05:42 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 06:06:42 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 28 Dec 2019 06:21:25 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af52e7ef6e83efadeae17be91daa6ecf61b7dfb39709c29be9b24876e60c0e36`  
		Last Modified: Sat, 28 Dec 2019 04:33:19 GMT  
		Size: 22.8 MB (22800791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:657bad46700417171f7961a2ff50ecc946522119a9a065f23416906ee79d822d`  
		Last Modified: Sat, 28 Dec 2019 06:22:56 GMT  
		Size: 244.5 KB (244499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c9779877dadfcd9c157fa02d2fbd6becf203c18e9c2727702df72179644d61`  
		Last Modified: Sat, 28 Dec 2019 06:23:14 GMT  
		Size: 24.6 MB (24638971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f31ee19914bb9f2e2b65604baa6905997d5f54e1d4012f6ed60ed63ad1b3c735`  
		Last Modified: Sat, 28 Dec 2019 06:25:31 GMT  
		Size: 125.6 MB (125620097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.20.1.34`

```console
$ docker pull mono@sha256:53dcdf176ceb5ed6ac9f8a0b999bd4e6859b4892f6d5a2a76e00ee6a00c44b58
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:5.20.1.34` - linux; amd64

```console
$ docker pull mono@sha256:f7a803fe550efe9aef81e8a44e8a43729c816b850f2e49040a7e081593700c1f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.3 MB (218283730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8aea3091220b44022c0f20929d510fe88b3cc4cdcde3057a185c15a282df8301`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:59:24 GMT
ADD file:2c1f5e08834f13ccb9c2326204eb2556e03239d00171e75755c7195289374c61 in / 
# Fri, 22 Nov 2019 14:59:25 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 23:00:40 GMT
ENV MONO_VERSION=5.20.1.34
# Fri, 22 Nov 2019 23:00:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 22 Nov 2019 23:01:21 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 22 Nov 2019 23:19:59 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d599a449871ee73b960e80d176b989365dfecb4c8f337bf21e8853862403ee9b`  
		Last Modified: Fri, 22 Nov 2019 15:06:36 GMT  
		Size: 22.5 MB (22524572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a778528e98113a69fcb62273f311379c55bd8759ce0e9ceeaedb433d4526e4a`  
		Last Modified: Fri, 22 Nov 2019 23:20:53 GMT  
		Size: 244.5 KB (244453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b697dbbf0ffb85ff1635ce5da0576d788dec98d69f5be271d5283cb190995d4d`  
		Last Modified: Fri, 22 Nov 2019 23:21:06 GMT  
		Size: 55.5 MB (55521485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b21954383b73fbad8beeae6b731b48d025852b1d498453b26562e7bfa977c7`  
		Last Modified: Fri, 22 Nov 2019 23:22:54 GMT  
		Size: 140.0 MB (139993220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1.34` - linux; arm variant v5

```console
$ docker pull mono@sha256:921141ae8dd056ee2c6ab66dde3ee626f76ecebd3941aaef44a81385fa7eb3e6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.0 MB (170952313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3270863ca29345901057a594ed47d2cb0e53b9b46570af2b4297f3a0e092cfa3`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:53:16 GMT
ADD file:7d6af454b55cb354e31c096e935358dd5914688ded04ebc76243a4ff598c4495 in / 
# Sat, 28 Dec 2019 04:53:18 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:31:47 GMT
ENV MONO_VERSION=5.20.1.34
# Sat, 28 Dec 2019 07:32:25 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:33:38 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 28 Dec 2019 07:43:54 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af28f499fd964f4506ea46c2ac342bc52328a8c30cd633661b69f383a5144e9b`  
		Last Modified: Sat, 28 Dec 2019 05:00:23 GMT  
		Size: 21.2 MB (21202822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e30f4dec85338cf63b2a0a4635e2307d966fbfa5356fe9e83d6a9bcf294768c4`  
		Last Modified: Sat, 28 Dec 2019 07:44:59 GMT  
		Size: 244.6 KB (244563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d859f970551d160b36092ef79b226a92798c6c82b5610774fb345988f6ab6cb`  
		Last Modified: Sat, 28 Dec 2019 07:45:08 GMT  
		Size: 24.3 MB (24265462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb69e22f6d5bc15e3d4811d51cca77b50460d4f38ad4131151a2df9b8fee768`  
		Last Modified: Sat, 28 Dec 2019 07:48:01 GMT  
		Size: 125.2 MB (125239466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1.34` - linux; arm variant v7

```console
$ docker pull mono@sha256:ea5d643ecc5f26c0f9f1edeb49fee6ea5323762e8727d392a1f813c4b8862460
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.0 MB (167004578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:631abf1b9406641e5331da51a0d793dd163877e353aece2468f77d0b962d5775`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 05:03:51 GMT
ADD file:2002ba672e32ae75369830ed6a4734ce62e0118e42390b4d657f0985d6b7fd6a in / 
# Sat, 28 Dec 2019 05:03:53 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:39:44 GMT
ENV MONO_VERSION=5.20.1.34
# Sat, 28 Dec 2019 07:40:06 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:40:54 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 28 Dec 2019 07:50:10 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:77cf262539006c8df77496f500f74a8c1edd158062440fd94d43d5b1292cefee`  
		Last Modified: Sat, 28 Dec 2019 05:11:13 GMT  
		Size: 19.3 MB (19311587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d99eb936b9cc5835bf59846bd4e0ae6c236cda6f4adce2cb3d14125cb51956`  
		Last Modified: Sat, 28 Dec 2019 07:51:22 GMT  
		Size: 244.6 KB (244557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fd6bf39cd6ba01aa22f88d8bed99d3c486440b3a5a1d22c82716aa505d7702`  
		Last Modified: Sat, 28 Dec 2019 07:51:30 GMT  
		Size: 23.6 MB (23561478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a7e7be5a6639501eb7d74f9ca29ade62656f3ca932b2c23aaca5ff7ea944c5`  
		Last Modified: Sat, 28 Dec 2019 07:54:12 GMT  
		Size: 123.9 MB (123886956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1.34` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:5bfa6d768088cbca6586d03476e2eb7eb2eb2ea0fb7370a6fa5a87759bf22585
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.8 MB (187815600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c75f84637df2a208fba18263667843579351fb12ec432b5865f8b6eddd963ba5`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:50 GMT
ADD file:8e4d0a1e6805c641fc9d18ebad82e4b01d85c6cb9f87d1ef47d75d150212a392 in / 
# Fri, 22 Nov 2019 13:45:53 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 20:56:16 GMT
ENV MONO_VERSION=5.20.1.34
# Fri, 22 Nov 2019 20:56:36 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 22 Nov 2019 20:57:14 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 22 Nov 2019 21:07:37 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:98a64bf4db7d2219b4fdd8182188d9422810dee890e997095bfb564a0482eed6`  
		Last Modified: Fri, 22 Nov 2019 13:52:17 GMT  
		Size: 20.4 MB (20385759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d1f78621344e3d91b8757cd69682a85fcacf7b02a199108cef35d380060188`  
		Last Modified: Fri, 22 Nov 2019 21:08:54 GMT  
		Size: 244.4 KB (244405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12210f2195af5163abba98ca92acf6283bf09e73698d41cee74183f5402ce55`  
		Last Modified: Fri, 22 Nov 2019 21:09:03 GMT  
		Size: 28.2 MB (28156046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a7680edeae996703f6ee15ad4398d036c169866908acbb816410973a13de969`  
		Last Modified: Fri, 22 Nov 2019 21:11:52 GMT  
		Size: 139.0 MB (139029390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1.34` - linux; 386

```console
$ docker pull mono@sha256:ec9d6818f5778553dfef85050a25e2cb122b90b5b06d537e5874e70a54bda52d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.8 MB (227782795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:358a8ef155cd2f22c5a4151a7c72c80bdefe7a456ffafae9a33de702305eb44a`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 16:54:44 GMT
ADD file:19d04f738434c76e2dbd14b48de2f0f03afa883b15f638c6ecbbf382df03567c in / 
# Fri, 22 Nov 2019 16:54:44 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 01:09:08 GMT
ENV MONO_VERSION=5.20.1.34
# Sat, 23 Nov 2019 01:09:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 23 Nov 2019 01:09:51 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 23 Nov 2019 01:16:25 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f26c9a85c76e393c9f2313b30e82d09f933d2dd4883620de242c7d21f8812e91`  
		Last Modified: Fri, 22 Nov 2019 17:03:03 GMT  
		Size: 23.2 MB (23152070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17fdd7c327a6ddaec1d04dab27737393102e01ec89d0f21c4dedee4e86eb1f34`  
		Last Modified: Sat, 23 Nov 2019 01:17:31 GMT  
		Size: 244.5 KB (244482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2816ec1c0521b0d2a95dd902cbe502786519966ce0073eb6de1bf01d58bd90c3`  
		Last Modified: Sat, 23 Nov 2019 01:17:48 GMT  
		Size: 58.6 MB (58552039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:064c1b59b86a05462dd6cae5082b0af2f54cb64d012af553452de527389b3b97`  
		Last Modified: Sat, 23 Nov 2019 01:20:16 GMT  
		Size: 145.8 MB (145834204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1.34` - linux; ppc64le

```console
$ docker pull mono@sha256:b414ce326f06449a5a441ad050f57286bf41f79b0e0130a25928f9f9617f3e8e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.3 MB (173304358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee71b36f2a14a9487be1b834ccb9a4c1682b90900f74f6a88ba2a4c937fa4272`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:21 GMT
ADD file:a1ee5955ff3ede8df9558f4bec0c7962d54c43374f857e1da7e2639ddf82a9f1 in / 
# Sat, 28 Dec 2019 04:23:24 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:05:00 GMT
ENV MONO_VERSION=5.20.1.34
# Sat, 28 Dec 2019 06:05:42 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 06:06:42 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 28 Dec 2019 06:21:25 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af52e7ef6e83efadeae17be91daa6ecf61b7dfb39709c29be9b24876e60c0e36`  
		Last Modified: Sat, 28 Dec 2019 04:33:19 GMT  
		Size: 22.8 MB (22800791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:657bad46700417171f7961a2ff50ecc946522119a9a065f23416906ee79d822d`  
		Last Modified: Sat, 28 Dec 2019 06:22:56 GMT  
		Size: 244.5 KB (244499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c9779877dadfcd9c157fa02d2fbd6becf203c18e9c2727702df72179644d61`  
		Last Modified: Sat, 28 Dec 2019 06:23:14 GMT  
		Size: 24.6 MB (24638971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f31ee19914bb9f2e2b65604baa6905997d5f54e1d4012f6ed60ed63ad1b3c735`  
		Last Modified: Sat, 28 Dec 2019 06:25:31 GMT  
		Size: 125.6 MB (125620097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.20.1.34-slim`

```console
$ docker pull mono@sha256:fad7e9f817756726acf65804320f04b4fdf8bac797d8401341746bdf68b2deea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:5.20.1.34-slim` - linux; amd64

```console
$ docker pull mono@sha256:0592cc29402a7ca6500507520bedacb9586a57bc2537eff9b28a687c8bdfcb0f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78290510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a027603eae9737dd691aa5014a90d99367b7eecf2f653b9adc0eac9ec03b501`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:59:24 GMT
ADD file:2c1f5e08834f13ccb9c2326204eb2556e03239d00171e75755c7195289374c61 in / 
# Fri, 22 Nov 2019 14:59:25 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 23:00:40 GMT
ENV MONO_VERSION=5.20.1.34
# Fri, 22 Nov 2019 23:00:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 22 Nov 2019 23:01:21 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d599a449871ee73b960e80d176b989365dfecb4c8f337bf21e8853862403ee9b`  
		Last Modified: Fri, 22 Nov 2019 15:06:36 GMT  
		Size: 22.5 MB (22524572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a778528e98113a69fcb62273f311379c55bd8759ce0e9ceeaedb433d4526e4a`  
		Last Modified: Fri, 22 Nov 2019 23:20:53 GMT  
		Size: 244.5 KB (244453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b697dbbf0ffb85ff1635ce5da0576d788dec98d69f5be271d5283cb190995d4d`  
		Last Modified: Fri, 22 Nov 2019 23:21:06 GMT  
		Size: 55.5 MB (55521485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1.34-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:84ba79b228b895ae28fc2cc6e7b153952f08df639473bf6a6ad88b31b82f0a01
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.7 MB (45712847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58072baece060776cb79a8f6bdbdc0f3a9c5a85bda29c3ac356f0068443d3d8e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:53:16 GMT
ADD file:7d6af454b55cb354e31c096e935358dd5914688ded04ebc76243a4ff598c4495 in / 
# Sat, 28 Dec 2019 04:53:18 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:31:47 GMT
ENV MONO_VERSION=5.20.1.34
# Sat, 28 Dec 2019 07:32:25 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:33:38 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af28f499fd964f4506ea46c2ac342bc52328a8c30cd633661b69f383a5144e9b`  
		Last Modified: Sat, 28 Dec 2019 05:00:23 GMT  
		Size: 21.2 MB (21202822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e30f4dec85338cf63b2a0a4635e2307d966fbfa5356fe9e83d6a9bcf294768c4`  
		Last Modified: Sat, 28 Dec 2019 07:44:59 GMT  
		Size: 244.6 KB (244563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d859f970551d160b36092ef79b226a92798c6c82b5610774fb345988f6ab6cb`  
		Last Modified: Sat, 28 Dec 2019 07:45:08 GMT  
		Size: 24.3 MB (24265462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1.34-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:d804f4bb2c5ff9bf8088ea66eb9543f3addacd400ed79782099001d18d396a31
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43117622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee7b70d3c2d1b9f9631a97c637f72660d3b7ae52250cb5c5dd618a88cd22aef6`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 05:03:51 GMT
ADD file:2002ba672e32ae75369830ed6a4734ce62e0118e42390b4d657f0985d6b7fd6a in / 
# Sat, 28 Dec 2019 05:03:53 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:39:44 GMT
ENV MONO_VERSION=5.20.1.34
# Sat, 28 Dec 2019 07:40:06 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:40:54 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:77cf262539006c8df77496f500f74a8c1edd158062440fd94d43d5b1292cefee`  
		Last Modified: Sat, 28 Dec 2019 05:11:13 GMT  
		Size: 19.3 MB (19311587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d99eb936b9cc5835bf59846bd4e0ae6c236cda6f4adce2cb3d14125cb51956`  
		Last Modified: Sat, 28 Dec 2019 07:51:22 GMT  
		Size: 244.6 KB (244557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fd6bf39cd6ba01aa22f88d8bed99d3c486440b3a5a1d22c82716aa505d7702`  
		Last Modified: Sat, 28 Dec 2019 07:51:30 GMT  
		Size: 23.6 MB (23561478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1.34-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:c70c2a465869690309ead8ecb21d2666227b91f29c516bdd83f76401971f1eb2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48786210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d294783fe09c22b968e4554d4c1036210d3c33216f18191162e7a7a8906c2bf5`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:50 GMT
ADD file:8e4d0a1e6805c641fc9d18ebad82e4b01d85c6cb9f87d1ef47d75d150212a392 in / 
# Fri, 22 Nov 2019 13:45:53 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 20:56:16 GMT
ENV MONO_VERSION=5.20.1.34
# Fri, 22 Nov 2019 20:56:36 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 22 Nov 2019 20:57:14 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:98a64bf4db7d2219b4fdd8182188d9422810dee890e997095bfb564a0482eed6`  
		Last Modified: Fri, 22 Nov 2019 13:52:17 GMT  
		Size: 20.4 MB (20385759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d1f78621344e3d91b8757cd69682a85fcacf7b02a199108cef35d380060188`  
		Last Modified: Fri, 22 Nov 2019 21:08:54 GMT  
		Size: 244.4 KB (244405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12210f2195af5163abba98ca92acf6283bf09e73698d41cee74183f5402ce55`  
		Last Modified: Fri, 22 Nov 2019 21:09:03 GMT  
		Size: 28.2 MB (28156046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1.34-slim` - linux; 386

```console
$ docker pull mono@sha256:aeb30511071e436d97fab67b58ae9f28156aaf5e5a1aea254e196f07a5799029
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81948591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9df4c050882f709b336300ef25d6031952ea040cc3b8f48d37274be3816fb1b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 16:54:44 GMT
ADD file:19d04f738434c76e2dbd14b48de2f0f03afa883b15f638c6ecbbf382df03567c in / 
# Fri, 22 Nov 2019 16:54:44 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 01:09:08 GMT
ENV MONO_VERSION=5.20.1.34
# Sat, 23 Nov 2019 01:09:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 23 Nov 2019 01:09:51 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f26c9a85c76e393c9f2313b30e82d09f933d2dd4883620de242c7d21f8812e91`  
		Last Modified: Fri, 22 Nov 2019 17:03:03 GMT  
		Size: 23.2 MB (23152070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17fdd7c327a6ddaec1d04dab27737393102e01ec89d0f21c4dedee4e86eb1f34`  
		Last Modified: Sat, 23 Nov 2019 01:17:31 GMT  
		Size: 244.5 KB (244482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2816ec1c0521b0d2a95dd902cbe502786519966ce0073eb6de1bf01d58bd90c3`  
		Last Modified: Sat, 23 Nov 2019 01:17:48 GMT  
		Size: 58.6 MB (58552039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1.34-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:aed3a9827f0d572f25d9f40d95b1f6932009f3fa43c45edd12c7bd4a1a7e118d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.7 MB (47684261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:558f9d54d3463ad40c540b19d52f4576c3edd30ec719da37da034a8bcdc494ca`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:21 GMT
ADD file:a1ee5955ff3ede8df9558f4bec0c7962d54c43374f857e1da7e2639ddf82a9f1 in / 
# Sat, 28 Dec 2019 04:23:24 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:05:00 GMT
ENV MONO_VERSION=5.20.1.34
# Sat, 28 Dec 2019 06:05:42 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 06:06:42 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af52e7ef6e83efadeae17be91daa6ecf61b7dfb39709c29be9b24876e60c0e36`  
		Last Modified: Sat, 28 Dec 2019 04:33:19 GMT  
		Size: 22.8 MB (22800791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:657bad46700417171f7961a2ff50ecc946522119a9a065f23416906ee79d822d`  
		Last Modified: Sat, 28 Dec 2019 06:22:56 GMT  
		Size: 244.5 KB (244499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c9779877dadfcd9c157fa02d2fbd6becf203c18e9c2727702df72179644d61`  
		Last Modified: Sat, 28 Dec 2019 06:23:14 GMT  
		Size: 24.6 MB (24638971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.20.1-slim`

```console
$ docker pull mono@sha256:fad7e9f817756726acf65804320f04b4fdf8bac797d8401341746bdf68b2deea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:5.20.1-slim` - linux; amd64

```console
$ docker pull mono@sha256:0592cc29402a7ca6500507520bedacb9586a57bc2537eff9b28a687c8bdfcb0f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78290510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a027603eae9737dd691aa5014a90d99367b7eecf2f653b9adc0eac9ec03b501`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:59:24 GMT
ADD file:2c1f5e08834f13ccb9c2326204eb2556e03239d00171e75755c7195289374c61 in / 
# Fri, 22 Nov 2019 14:59:25 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 23:00:40 GMT
ENV MONO_VERSION=5.20.1.34
# Fri, 22 Nov 2019 23:00:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 22 Nov 2019 23:01:21 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d599a449871ee73b960e80d176b989365dfecb4c8f337bf21e8853862403ee9b`  
		Last Modified: Fri, 22 Nov 2019 15:06:36 GMT  
		Size: 22.5 MB (22524572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a778528e98113a69fcb62273f311379c55bd8759ce0e9ceeaedb433d4526e4a`  
		Last Modified: Fri, 22 Nov 2019 23:20:53 GMT  
		Size: 244.5 KB (244453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b697dbbf0ffb85ff1635ce5da0576d788dec98d69f5be271d5283cb190995d4d`  
		Last Modified: Fri, 22 Nov 2019 23:21:06 GMT  
		Size: 55.5 MB (55521485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:84ba79b228b895ae28fc2cc6e7b153952f08df639473bf6a6ad88b31b82f0a01
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.7 MB (45712847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58072baece060776cb79a8f6bdbdc0f3a9c5a85bda29c3ac356f0068443d3d8e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:53:16 GMT
ADD file:7d6af454b55cb354e31c096e935358dd5914688ded04ebc76243a4ff598c4495 in / 
# Sat, 28 Dec 2019 04:53:18 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:31:47 GMT
ENV MONO_VERSION=5.20.1.34
# Sat, 28 Dec 2019 07:32:25 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:33:38 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af28f499fd964f4506ea46c2ac342bc52328a8c30cd633661b69f383a5144e9b`  
		Last Modified: Sat, 28 Dec 2019 05:00:23 GMT  
		Size: 21.2 MB (21202822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e30f4dec85338cf63b2a0a4635e2307d966fbfa5356fe9e83d6a9bcf294768c4`  
		Last Modified: Sat, 28 Dec 2019 07:44:59 GMT  
		Size: 244.6 KB (244563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d859f970551d160b36092ef79b226a92798c6c82b5610774fb345988f6ab6cb`  
		Last Modified: Sat, 28 Dec 2019 07:45:08 GMT  
		Size: 24.3 MB (24265462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:d804f4bb2c5ff9bf8088ea66eb9543f3addacd400ed79782099001d18d396a31
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43117622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee7b70d3c2d1b9f9631a97c637f72660d3b7ae52250cb5c5dd618a88cd22aef6`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 05:03:51 GMT
ADD file:2002ba672e32ae75369830ed6a4734ce62e0118e42390b4d657f0985d6b7fd6a in / 
# Sat, 28 Dec 2019 05:03:53 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:39:44 GMT
ENV MONO_VERSION=5.20.1.34
# Sat, 28 Dec 2019 07:40:06 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:40:54 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:77cf262539006c8df77496f500f74a8c1edd158062440fd94d43d5b1292cefee`  
		Last Modified: Sat, 28 Dec 2019 05:11:13 GMT  
		Size: 19.3 MB (19311587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d99eb936b9cc5835bf59846bd4e0ae6c236cda6f4adce2cb3d14125cb51956`  
		Last Modified: Sat, 28 Dec 2019 07:51:22 GMT  
		Size: 244.6 KB (244557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fd6bf39cd6ba01aa22f88d8bed99d3c486440b3a5a1d22c82716aa505d7702`  
		Last Modified: Sat, 28 Dec 2019 07:51:30 GMT  
		Size: 23.6 MB (23561478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:c70c2a465869690309ead8ecb21d2666227b91f29c516bdd83f76401971f1eb2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48786210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d294783fe09c22b968e4554d4c1036210d3c33216f18191162e7a7a8906c2bf5`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:50 GMT
ADD file:8e4d0a1e6805c641fc9d18ebad82e4b01d85c6cb9f87d1ef47d75d150212a392 in / 
# Fri, 22 Nov 2019 13:45:53 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 20:56:16 GMT
ENV MONO_VERSION=5.20.1.34
# Fri, 22 Nov 2019 20:56:36 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 22 Nov 2019 20:57:14 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:98a64bf4db7d2219b4fdd8182188d9422810dee890e997095bfb564a0482eed6`  
		Last Modified: Fri, 22 Nov 2019 13:52:17 GMT  
		Size: 20.4 MB (20385759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d1f78621344e3d91b8757cd69682a85fcacf7b02a199108cef35d380060188`  
		Last Modified: Fri, 22 Nov 2019 21:08:54 GMT  
		Size: 244.4 KB (244405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12210f2195af5163abba98ca92acf6283bf09e73698d41cee74183f5402ce55`  
		Last Modified: Fri, 22 Nov 2019 21:09:03 GMT  
		Size: 28.2 MB (28156046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1-slim` - linux; 386

```console
$ docker pull mono@sha256:aeb30511071e436d97fab67b58ae9f28156aaf5e5a1aea254e196f07a5799029
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81948591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9df4c050882f709b336300ef25d6031952ea040cc3b8f48d37274be3816fb1b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 16:54:44 GMT
ADD file:19d04f738434c76e2dbd14b48de2f0f03afa883b15f638c6ecbbf382df03567c in / 
# Fri, 22 Nov 2019 16:54:44 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 01:09:08 GMT
ENV MONO_VERSION=5.20.1.34
# Sat, 23 Nov 2019 01:09:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 23 Nov 2019 01:09:51 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f26c9a85c76e393c9f2313b30e82d09f933d2dd4883620de242c7d21f8812e91`  
		Last Modified: Fri, 22 Nov 2019 17:03:03 GMT  
		Size: 23.2 MB (23152070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17fdd7c327a6ddaec1d04dab27737393102e01ec89d0f21c4dedee4e86eb1f34`  
		Last Modified: Sat, 23 Nov 2019 01:17:31 GMT  
		Size: 244.5 KB (244482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2816ec1c0521b0d2a95dd902cbe502786519966ce0073eb6de1bf01d58bd90c3`  
		Last Modified: Sat, 23 Nov 2019 01:17:48 GMT  
		Size: 58.6 MB (58552039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:aed3a9827f0d572f25d9f40d95b1f6932009f3fa43c45edd12c7bd4a1a7e118d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.7 MB (47684261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:558f9d54d3463ad40c540b19d52f4576c3edd30ec719da37da034a8bcdc494ca`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:21 GMT
ADD file:a1ee5955ff3ede8df9558f4bec0c7962d54c43374f857e1da7e2639ddf82a9f1 in / 
# Sat, 28 Dec 2019 04:23:24 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:05:00 GMT
ENV MONO_VERSION=5.20.1.34
# Sat, 28 Dec 2019 06:05:42 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 06:06:42 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af52e7ef6e83efadeae17be91daa6ecf61b7dfb39709c29be9b24876e60c0e36`  
		Last Modified: Sat, 28 Dec 2019 04:33:19 GMT  
		Size: 22.8 MB (22800791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:657bad46700417171f7961a2ff50ecc946522119a9a065f23416906ee79d822d`  
		Last Modified: Sat, 28 Dec 2019 06:22:56 GMT  
		Size: 244.5 KB (244499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c9779877dadfcd9c157fa02d2fbd6becf203c18e9c2727702df72179644d61`  
		Last Modified: Sat, 28 Dec 2019 06:23:14 GMT  
		Size: 24.6 MB (24638971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.20-slim`

```console
$ docker pull mono@sha256:fad7e9f817756726acf65804320f04b4fdf8bac797d8401341746bdf68b2deea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:5.20-slim` - linux; amd64

```console
$ docker pull mono@sha256:0592cc29402a7ca6500507520bedacb9586a57bc2537eff9b28a687c8bdfcb0f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78290510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a027603eae9737dd691aa5014a90d99367b7eecf2f653b9adc0eac9ec03b501`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:59:24 GMT
ADD file:2c1f5e08834f13ccb9c2326204eb2556e03239d00171e75755c7195289374c61 in / 
# Fri, 22 Nov 2019 14:59:25 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 23:00:40 GMT
ENV MONO_VERSION=5.20.1.34
# Fri, 22 Nov 2019 23:00:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 22 Nov 2019 23:01:21 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d599a449871ee73b960e80d176b989365dfecb4c8f337bf21e8853862403ee9b`  
		Last Modified: Fri, 22 Nov 2019 15:06:36 GMT  
		Size: 22.5 MB (22524572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a778528e98113a69fcb62273f311379c55bd8759ce0e9ceeaedb433d4526e4a`  
		Last Modified: Fri, 22 Nov 2019 23:20:53 GMT  
		Size: 244.5 KB (244453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b697dbbf0ffb85ff1635ce5da0576d788dec98d69f5be271d5283cb190995d4d`  
		Last Modified: Fri, 22 Nov 2019 23:21:06 GMT  
		Size: 55.5 MB (55521485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:84ba79b228b895ae28fc2cc6e7b153952f08df639473bf6a6ad88b31b82f0a01
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.7 MB (45712847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58072baece060776cb79a8f6bdbdc0f3a9c5a85bda29c3ac356f0068443d3d8e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:53:16 GMT
ADD file:7d6af454b55cb354e31c096e935358dd5914688ded04ebc76243a4ff598c4495 in / 
# Sat, 28 Dec 2019 04:53:18 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:31:47 GMT
ENV MONO_VERSION=5.20.1.34
# Sat, 28 Dec 2019 07:32:25 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:33:38 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af28f499fd964f4506ea46c2ac342bc52328a8c30cd633661b69f383a5144e9b`  
		Last Modified: Sat, 28 Dec 2019 05:00:23 GMT  
		Size: 21.2 MB (21202822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e30f4dec85338cf63b2a0a4635e2307d966fbfa5356fe9e83d6a9bcf294768c4`  
		Last Modified: Sat, 28 Dec 2019 07:44:59 GMT  
		Size: 244.6 KB (244563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d859f970551d160b36092ef79b226a92798c6c82b5610774fb345988f6ab6cb`  
		Last Modified: Sat, 28 Dec 2019 07:45:08 GMT  
		Size: 24.3 MB (24265462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:d804f4bb2c5ff9bf8088ea66eb9543f3addacd400ed79782099001d18d396a31
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43117622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee7b70d3c2d1b9f9631a97c637f72660d3b7ae52250cb5c5dd618a88cd22aef6`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 05:03:51 GMT
ADD file:2002ba672e32ae75369830ed6a4734ce62e0118e42390b4d657f0985d6b7fd6a in / 
# Sat, 28 Dec 2019 05:03:53 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:39:44 GMT
ENV MONO_VERSION=5.20.1.34
# Sat, 28 Dec 2019 07:40:06 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:40:54 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:77cf262539006c8df77496f500f74a8c1edd158062440fd94d43d5b1292cefee`  
		Last Modified: Sat, 28 Dec 2019 05:11:13 GMT  
		Size: 19.3 MB (19311587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d99eb936b9cc5835bf59846bd4e0ae6c236cda6f4adce2cb3d14125cb51956`  
		Last Modified: Sat, 28 Dec 2019 07:51:22 GMT  
		Size: 244.6 KB (244557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fd6bf39cd6ba01aa22f88d8bed99d3c486440b3a5a1d22c82716aa505d7702`  
		Last Modified: Sat, 28 Dec 2019 07:51:30 GMT  
		Size: 23.6 MB (23561478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:c70c2a465869690309ead8ecb21d2666227b91f29c516bdd83f76401971f1eb2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48786210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d294783fe09c22b968e4554d4c1036210d3c33216f18191162e7a7a8906c2bf5`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:50 GMT
ADD file:8e4d0a1e6805c641fc9d18ebad82e4b01d85c6cb9f87d1ef47d75d150212a392 in / 
# Fri, 22 Nov 2019 13:45:53 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 20:56:16 GMT
ENV MONO_VERSION=5.20.1.34
# Fri, 22 Nov 2019 20:56:36 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 22 Nov 2019 20:57:14 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:98a64bf4db7d2219b4fdd8182188d9422810dee890e997095bfb564a0482eed6`  
		Last Modified: Fri, 22 Nov 2019 13:52:17 GMT  
		Size: 20.4 MB (20385759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d1f78621344e3d91b8757cd69682a85fcacf7b02a199108cef35d380060188`  
		Last Modified: Fri, 22 Nov 2019 21:08:54 GMT  
		Size: 244.4 KB (244405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12210f2195af5163abba98ca92acf6283bf09e73698d41cee74183f5402ce55`  
		Last Modified: Fri, 22 Nov 2019 21:09:03 GMT  
		Size: 28.2 MB (28156046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20-slim` - linux; 386

```console
$ docker pull mono@sha256:aeb30511071e436d97fab67b58ae9f28156aaf5e5a1aea254e196f07a5799029
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81948591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9df4c050882f709b336300ef25d6031952ea040cc3b8f48d37274be3816fb1b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 16:54:44 GMT
ADD file:19d04f738434c76e2dbd14b48de2f0f03afa883b15f638c6ecbbf382df03567c in / 
# Fri, 22 Nov 2019 16:54:44 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 01:09:08 GMT
ENV MONO_VERSION=5.20.1.34
# Sat, 23 Nov 2019 01:09:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 23 Nov 2019 01:09:51 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f26c9a85c76e393c9f2313b30e82d09f933d2dd4883620de242c7d21f8812e91`  
		Last Modified: Fri, 22 Nov 2019 17:03:03 GMT  
		Size: 23.2 MB (23152070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17fdd7c327a6ddaec1d04dab27737393102e01ec89d0f21c4dedee4e86eb1f34`  
		Last Modified: Sat, 23 Nov 2019 01:17:31 GMT  
		Size: 244.5 KB (244482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2816ec1c0521b0d2a95dd902cbe502786519966ce0073eb6de1bf01d58bd90c3`  
		Last Modified: Sat, 23 Nov 2019 01:17:48 GMT  
		Size: 58.6 MB (58552039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:aed3a9827f0d572f25d9f40d95b1f6932009f3fa43c45edd12c7bd4a1a7e118d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.7 MB (47684261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:558f9d54d3463ad40c540b19d52f4576c3edd30ec719da37da034a8bcdc494ca`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:21 GMT
ADD file:a1ee5955ff3ede8df9558f4bec0c7962d54c43374f857e1da7e2639ddf82a9f1 in / 
# Sat, 28 Dec 2019 04:23:24 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:05:00 GMT
ENV MONO_VERSION=5.20.1.34
# Sat, 28 Dec 2019 06:05:42 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 06:06:42 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af52e7ef6e83efadeae17be91daa6ecf61b7dfb39709c29be9b24876e60c0e36`  
		Last Modified: Sat, 28 Dec 2019 04:33:19 GMT  
		Size: 22.8 MB (22800791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:657bad46700417171f7961a2ff50ecc946522119a9a065f23416906ee79d822d`  
		Last Modified: Sat, 28 Dec 2019 06:22:56 GMT  
		Size: 244.5 KB (244499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c9779877dadfcd9c157fa02d2fbd6becf203c18e9c2727702df72179644d61`  
		Last Modified: Sat, 28 Dec 2019 06:23:14 GMT  
		Size: 24.6 MB (24638971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5-slim`

```console
$ docker pull mono@sha256:fad7e9f817756726acf65804320f04b4fdf8bac797d8401341746bdf68b2deea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:5-slim` - linux; amd64

```console
$ docker pull mono@sha256:0592cc29402a7ca6500507520bedacb9586a57bc2537eff9b28a687c8bdfcb0f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78290510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a027603eae9737dd691aa5014a90d99367b7eecf2f653b9adc0eac9ec03b501`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:59:24 GMT
ADD file:2c1f5e08834f13ccb9c2326204eb2556e03239d00171e75755c7195289374c61 in / 
# Fri, 22 Nov 2019 14:59:25 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 23:00:40 GMT
ENV MONO_VERSION=5.20.1.34
# Fri, 22 Nov 2019 23:00:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 22 Nov 2019 23:01:21 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d599a449871ee73b960e80d176b989365dfecb4c8f337bf21e8853862403ee9b`  
		Last Modified: Fri, 22 Nov 2019 15:06:36 GMT  
		Size: 22.5 MB (22524572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a778528e98113a69fcb62273f311379c55bd8759ce0e9ceeaedb433d4526e4a`  
		Last Modified: Fri, 22 Nov 2019 23:20:53 GMT  
		Size: 244.5 KB (244453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b697dbbf0ffb85ff1635ce5da0576d788dec98d69f5be271d5283cb190995d4d`  
		Last Modified: Fri, 22 Nov 2019 23:21:06 GMT  
		Size: 55.5 MB (55521485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:84ba79b228b895ae28fc2cc6e7b153952f08df639473bf6a6ad88b31b82f0a01
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.7 MB (45712847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58072baece060776cb79a8f6bdbdc0f3a9c5a85bda29c3ac356f0068443d3d8e`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:53:16 GMT
ADD file:7d6af454b55cb354e31c096e935358dd5914688ded04ebc76243a4ff598c4495 in / 
# Sat, 28 Dec 2019 04:53:18 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:31:47 GMT
ENV MONO_VERSION=5.20.1.34
# Sat, 28 Dec 2019 07:32:25 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:33:38 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af28f499fd964f4506ea46c2ac342bc52328a8c30cd633661b69f383a5144e9b`  
		Last Modified: Sat, 28 Dec 2019 05:00:23 GMT  
		Size: 21.2 MB (21202822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e30f4dec85338cf63b2a0a4635e2307d966fbfa5356fe9e83d6a9bcf294768c4`  
		Last Modified: Sat, 28 Dec 2019 07:44:59 GMT  
		Size: 244.6 KB (244563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d859f970551d160b36092ef79b226a92798c6c82b5610774fb345988f6ab6cb`  
		Last Modified: Sat, 28 Dec 2019 07:45:08 GMT  
		Size: 24.3 MB (24265462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:d804f4bb2c5ff9bf8088ea66eb9543f3addacd400ed79782099001d18d396a31
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43117622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee7b70d3c2d1b9f9631a97c637f72660d3b7ae52250cb5c5dd618a88cd22aef6`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 05:03:51 GMT
ADD file:2002ba672e32ae75369830ed6a4734ce62e0118e42390b4d657f0985d6b7fd6a in / 
# Sat, 28 Dec 2019 05:03:53 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:39:44 GMT
ENV MONO_VERSION=5.20.1.34
# Sat, 28 Dec 2019 07:40:06 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:40:54 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:77cf262539006c8df77496f500f74a8c1edd158062440fd94d43d5b1292cefee`  
		Last Modified: Sat, 28 Dec 2019 05:11:13 GMT  
		Size: 19.3 MB (19311587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d99eb936b9cc5835bf59846bd4e0ae6c236cda6f4adce2cb3d14125cb51956`  
		Last Modified: Sat, 28 Dec 2019 07:51:22 GMT  
		Size: 244.6 KB (244557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fd6bf39cd6ba01aa22f88d8bed99d3c486440b3a5a1d22c82716aa505d7702`  
		Last Modified: Sat, 28 Dec 2019 07:51:30 GMT  
		Size: 23.6 MB (23561478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:c70c2a465869690309ead8ecb21d2666227b91f29c516bdd83f76401971f1eb2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48786210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d294783fe09c22b968e4554d4c1036210d3c33216f18191162e7a7a8906c2bf5`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:50 GMT
ADD file:8e4d0a1e6805c641fc9d18ebad82e4b01d85c6cb9f87d1ef47d75d150212a392 in / 
# Fri, 22 Nov 2019 13:45:53 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 20:56:16 GMT
ENV MONO_VERSION=5.20.1.34
# Fri, 22 Nov 2019 20:56:36 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 22 Nov 2019 20:57:14 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:98a64bf4db7d2219b4fdd8182188d9422810dee890e997095bfb564a0482eed6`  
		Last Modified: Fri, 22 Nov 2019 13:52:17 GMT  
		Size: 20.4 MB (20385759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d1f78621344e3d91b8757cd69682a85fcacf7b02a199108cef35d380060188`  
		Last Modified: Fri, 22 Nov 2019 21:08:54 GMT  
		Size: 244.4 KB (244405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12210f2195af5163abba98ca92acf6283bf09e73698d41cee74183f5402ce55`  
		Last Modified: Fri, 22 Nov 2019 21:09:03 GMT  
		Size: 28.2 MB (28156046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5-slim` - linux; 386

```console
$ docker pull mono@sha256:aeb30511071e436d97fab67b58ae9f28156aaf5e5a1aea254e196f07a5799029
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81948591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9df4c050882f709b336300ef25d6031952ea040cc3b8f48d37274be3816fb1b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 16:54:44 GMT
ADD file:19d04f738434c76e2dbd14b48de2f0f03afa883b15f638c6ecbbf382df03567c in / 
# Fri, 22 Nov 2019 16:54:44 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 01:09:08 GMT
ENV MONO_VERSION=5.20.1.34
# Sat, 23 Nov 2019 01:09:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 23 Nov 2019 01:09:51 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f26c9a85c76e393c9f2313b30e82d09f933d2dd4883620de242c7d21f8812e91`  
		Last Modified: Fri, 22 Nov 2019 17:03:03 GMT  
		Size: 23.2 MB (23152070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17fdd7c327a6ddaec1d04dab27737393102e01ec89d0f21c4dedee4e86eb1f34`  
		Last Modified: Sat, 23 Nov 2019 01:17:31 GMT  
		Size: 244.5 KB (244482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2816ec1c0521b0d2a95dd902cbe502786519966ce0073eb6de1bf01d58bd90c3`  
		Last Modified: Sat, 23 Nov 2019 01:17:48 GMT  
		Size: 58.6 MB (58552039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:aed3a9827f0d572f25d9f40d95b1f6932009f3fa43c45edd12c7bd4a1a7e118d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.7 MB (47684261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:558f9d54d3463ad40c540b19d52f4576c3edd30ec719da37da034a8bcdc494ca`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:21 GMT
ADD file:a1ee5955ff3ede8df9558f4bec0c7962d54c43374f857e1da7e2639ddf82a9f1 in / 
# Sat, 28 Dec 2019 04:23:24 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:05:00 GMT
ENV MONO_VERSION=5.20.1.34
# Sat, 28 Dec 2019 06:05:42 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 06:06:42 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af52e7ef6e83efadeae17be91daa6ecf61b7dfb39709c29be9b24876e60c0e36`  
		Last Modified: Sat, 28 Dec 2019 04:33:19 GMT  
		Size: 22.8 MB (22800791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:657bad46700417171f7961a2ff50ecc946522119a9a065f23416906ee79d822d`  
		Last Modified: Sat, 28 Dec 2019 06:22:56 GMT  
		Size: 244.5 KB (244499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c9779877dadfcd9c157fa02d2fbd6becf203c18e9c2727702df72179644d61`  
		Last Modified: Sat, 28 Dec 2019 06:23:14 GMT  
		Size: 24.6 MB (24638971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6`

```console
$ docker pull mono@sha256:f5ff533f0bafd79c6e7d6938294e6ea09c9743aada81db4a25edab25ab46cdcc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6` - linux; amd64

```console
$ docker pull mono@sha256:36bbaae3165f4dbbe0c166c151e638fc5c48e638ceb8c6070636f1c01d061206
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.2 MB (233196810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0211b82d6aefd6ae2c5a588c2119889733c462fda32a0210e20ea91fd4956312`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:59:24 GMT
ADD file:2c1f5e08834f13ccb9c2326204eb2556e03239d00171e75755c7195289374c61 in / 
# Fri, 22 Nov 2019 14:59:25 GMT
CMD ["bash"]
# Tue, 10 Dec 2019 22:11:17 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 10 Dec 2019 22:11:31 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 10 Dec 2019 22:12:14 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 10 Dec 2019 22:23:55 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d599a449871ee73b960e80d176b989365dfecb4c8f337bf21e8853862403ee9b`  
		Last Modified: Fri, 22 Nov 2019 15:06:36 GMT  
		Size: 22.5 MB (22524572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d110a8d8d6a5fa5a2ed11b6480fdb8ddd3752cc065f9bb4601207fe6c2a5ccaa`  
		Last Modified: Tue, 10 Dec 2019 22:24:24 GMT  
		Size: 244.5 KB (244460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df5758d8b4d450d2162c07e6a21fcfd0720544194e831610eb80d1780f188bc`  
		Last Modified: Tue, 10 Dec 2019 22:24:39 GMT  
		Size: 63.0 MB (62973805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db3f1cd295be39d3d4a0ec3b1ef1190b9ac6a4c1cd9f4ee0769d0a6e0e6aa69`  
		Last Modified: Tue, 10 Dec 2019 22:25:22 GMT  
		Size: 147.5 MB (147453973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; arm variant v5

```console
$ docker pull mono@sha256:71075f43a6acd5d4900e8b4050bc87b552302d7b550e2d9da1a55aa37eb95852
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.7 MB (176653531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41594e91a86b24e549ebe9f4c951e2403e6e22200d648d599d853dbc7ebe37a5`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:53:16 GMT
ADD file:7d6af454b55cb354e31c096e935358dd5914688ded04ebc76243a4ff598c4495 in / 
# Sat, 28 Dec 2019 04:53:18 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:28:31 GMT
ENV MONO_VERSION=6.6.0.161
# Sat, 28 Dec 2019 07:28:56 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:29:51 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 28 Dec 2019 07:37:00 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af28f499fd964f4506ea46c2ac342bc52328a8c30cd633661b69f383a5144e9b`  
		Last Modified: Sat, 28 Dec 2019 05:00:23 GMT  
		Size: 21.2 MB (21202822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f759ae685ca874cea702ae1f63627810d814a2cae6a44c704003176e0c8b37c`  
		Last Modified: Sat, 28 Dec 2019 07:44:23 GMT  
		Size: 244.6 KB (244552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:720fbe46ab0c5e8c2e3e9ed44413d9fde2ad1d45d9161dd0c6a021855acc1b78`  
		Last Modified: Sat, 28 Dec 2019 07:44:33 GMT  
		Size: 25.4 MB (25416500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906dd0e12894eb03a4ab34eacdf91d163dfd6c09d61c9005e666875d42c1b91b`  
		Last Modified: Sat, 28 Dec 2019 07:46:06 GMT  
		Size: 129.8 MB (129789657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; arm variant v7

```console
$ docker pull mono@sha256:7e7ebdba687fb7bac2a796eb557210fe8f5fa55c86cfa342bd56d213a27dcaf3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.7 MB (172655347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c77176fb08c03220255179938d178739f8882569f72ecaae83ba7b5fc620aef`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 05:03:51 GMT
ADD file:2002ba672e32ae75369830ed6a4734ce62e0118e42390b4d657f0985d6b7fd6a in / 
# Sat, 28 Dec 2019 05:03:53 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:37:00 GMT
ENV MONO_VERSION=6.6.0.161
# Sat, 28 Dec 2019 07:37:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:38:02 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 28 Dec 2019 07:44:03 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:77cf262539006c8df77496f500f74a8c1edd158062440fd94d43d5b1292cefee`  
		Last Modified: Sat, 28 Dec 2019 05:11:13 GMT  
		Size: 19.3 MB (19311587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ea3a0398ee0834c6b8b5a98490a2451261135d85bbd06845c7077aff2a4667`  
		Last Modified: Sat, 28 Dec 2019 07:50:49 GMT  
		Size: 244.5 KB (244525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f543438b2494429fd7ef0a5cbe2145241dfa4aa2f1008038a251526056612dc`  
		Last Modified: Sat, 28 Dec 2019 07:50:58 GMT  
		Size: 24.6 MB (24648229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184b3a33ac95fb2ba207e6fc82f4e7fac1dc71bad49531f182c2a7046b54bd39`  
		Last Modified: Sat, 28 Dec 2019 07:52:21 GMT  
		Size: 128.5 MB (128451006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:9d331c132d88d02b360e8d415ca3ce11ac4b29fce0711e4bf57768bd608750d7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.5 MB (194538550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:185e12dba59e302b48ff069147dffe83d87755aee21ec6b8f56bc46ff2e325fa`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:50 GMT
ADD file:8e4d0a1e6805c641fc9d18ebad82e4b01d85c6cb9f87d1ef47d75d150212a392 in / 
# Fri, 22 Nov 2019 13:45:53 GMT
CMD ["bash"]
# Tue, 10 Dec 2019 22:32:06 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 10 Dec 2019 22:32:29 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 10 Dec 2019 22:33:16 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 10 Dec 2019 22:36:34 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:98a64bf4db7d2219b4fdd8182188d9422810dee890e997095bfb564a0482eed6`  
		Last Modified: Fri, 22 Nov 2019 13:52:17 GMT  
		Size: 20.4 MB (20385759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a200380ef45d7e798a6c00bf777add415c1dcd43827dfd4245e9a70a44551c16`  
		Last Modified: Tue, 10 Dec 2019 22:37:08 GMT  
		Size: 244.4 KB (244414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d827d45253e033764c27bafc3cf0f6f6a7c489c4cbfc72204de1e80d360e4ad`  
		Last Modified: Tue, 10 Dec 2019 22:37:19 GMT  
		Size: 29.4 MB (29433771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b857a6aa08dd2c3efd831641f352d721803f51db7005a61c8b24cd3bc8835076`  
		Last Modified: Tue, 10 Dec 2019 22:38:16 GMT  
		Size: 144.5 MB (144474606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; 386

```console
$ docker pull mono@sha256:cb86414bf1a5dea08a730c594cd416e9811c28a017a19c1ef38413d28b7c43f1
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.4 MB (241440758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8236e6d4318ea3a6c3150c668ccd4b5ad0a54f9ec9b8b6ae6f5f9025d7c159c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 16:54:44 GMT
ADD file:19d04f738434c76e2dbd14b48de2f0f03afa883b15f638c6ecbbf382df03567c in / 
# Fri, 22 Nov 2019 16:54:44 GMT
CMD ["bash"]
# Tue, 10 Dec 2019 22:40:38 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 10 Dec 2019 22:40:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 10 Dec 2019 22:41:28 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 10 Dec 2019 22:44:08 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f26c9a85c76e393c9f2313b30e82d09f933d2dd4883620de242c7d21f8812e91`  
		Last Modified: Fri, 22 Nov 2019 17:03:03 GMT  
		Size: 23.2 MB (23152070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd443cfef677c492dd94fe413c0d2136b767456782251d33c6f1317711c7ebb`  
		Last Modified: Tue, 10 Dec 2019 22:44:33 GMT  
		Size: 244.5 KB (244499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd896b7ec3d7536139b522b4d9ce45dfd161f148c667dbc616035478ae145c7`  
		Last Modified: Tue, 10 Dec 2019 22:44:49 GMT  
		Size: 66.7 MB (66749782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f932dceff64bdede65b0f1e5a3443dc9749d88d7ad89b99977d0339b81891b5d`  
		Last Modified: Tue, 10 Dec 2019 22:45:37 GMT  
		Size: 151.3 MB (151294407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; ppc64le

```console
$ docker pull mono@sha256:8be78d5e96a5e63f2d4754a3686943f1d8edfd75c46a313cd27984c010e27c52
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.9 MB (178943769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c75d8bc1699ea912f280f4dcb86edababad529239b8eeb28e3801bcd9a015066`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:21 GMT
ADD file:a1ee5955ff3ede8df9558f4bec0c7962d54c43374f857e1da7e2639ddf82a9f1 in / 
# Sat, 28 Dec 2019 04:23:24 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:00:10 GMT
ENV MONO_VERSION=6.6.0.161
# Sat, 28 Dec 2019 06:01:14 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 06:02:17 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 28 Dec 2019 06:11:01 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af52e7ef6e83efadeae17be91daa6ecf61b7dfb39709c29be9b24876e60c0e36`  
		Last Modified: Sat, 28 Dec 2019 04:33:19 GMT  
		Size: 22.8 MB (22800791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367bf0f7a48952d80f9489622c9b118004dd0fd4763a1fd6153d9b12a571b1ee`  
		Last Modified: Sat, 28 Dec 2019 06:22:04 GMT  
		Size: 244.5 KB (244543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf3902985b2f759ba0edff57a78d4eb7e81f59e8327b7d243b8f3b4b8ca7c79`  
		Last Modified: Sat, 28 Dec 2019 06:22:14 GMT  
		Size: 25.8 MB (25828829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b12c28397b6cede6691c7e5447b466791fb395f4ecb3d1fb78e68dc1ffe4eb9`  
		Last Modified: Sat, 28 Dec 2019 06:24:05 GMT  
		Size: 130.1 MB (130069606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.4`

```console
$ docker pull mono@sha256:23cfeb120eb032fd466687c75c9c48c22b2330fed6435e27ea289bd7f2458003
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.4` - linux; amd64

```console
$ docker pull mono@sha256:03fcc004eba262d5068fe2c69aa21ba66284913091ada922e3f52e62d9676174
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.9 MB (229861563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ba93b1033ba2ccaf8b5dbe036fab3faba421ea1b94e183c9cfac7feee17c507`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:59:24 GMT
ADD file:2c1f5e08834f13ccb9c2326204eb2556e03239d00171e75755c7195289374c61 in / 
# Fri, 22 Nov 2019 14:59:25 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 22:59:02 GMT
ENV MONO_VERSION=6.4.0.198
# Fri, 22 Nov 2019 22:59:16 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 22 Nov 2019 22:59:47 GMT
RUN echo "deb http://download.mono-project.com/repo/debian vs-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 22 Nov 2019 23:10:02 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d599a449871ee73b960e80d176b989365dfecb4c8f337bf21e8853862403ee9b`  
		Last Modified: Fri, 22 Nov 2019 15:06:36 GMT  
		Size: 22.5 MB (22524572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d97711e218db482a8b5126b3a4e42b4d779e333becec529e3a1db4a35e37453`  
		Last Modified: Fri, 22 Nov 2019 23:20:12 GMT  
		Size: 244.5 KB (244459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce311d3c9c556425ac31acae067c848ad34faf95766b476fe942501d8c16307`  
		Last Modified: Fri, 22 Nov 2019 23:20:25 GMT  
		Size: 62.2 MB (62239606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98cc01904b7faa8a884765e56bc1f600b68f5b72b302a5d9aea1c483efa850d`  
		Last Modified: Fri, 22 Nov 2019 23:21:43 GMT  
		Size: 144.9 MB (144852926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.4` - linux; arm variant v5

```console
$ docker pull mono@sha256:38c5f861b60869c07145058d2627a5c2c32426c6062056c03eb295f78eb4225d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.4 MB (173418183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3fc9fcb755d681a693abbf48833028bd63cdc15bf29f7292a31b53e52d272de`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:53:16 GMT
ADD file:7d6af454b55cb354e31c096e935358dd5914688ded04ebc76243a4ff598c4495 in / 
# Sat, 28 Dec 2019 04:53:18 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:30:03 GMT
ENV MONO_VERSION=6.4.0.198
# Sat, 28 Dec 2019 07:30:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:31:25 GMT
RUN echo "deb http://download.mono-project.com/repo/debian vs-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 28 Dec 2019 07:40:16 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af28f499fd964f4506ea46c2ac342bc52328a8c30cd633661b69f383a5144e9b`  
		Last Modified: Sat, 28 Dec 2019 05:00:23 GMT  
		Size: 21.2 MB (21202822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:debae7c5f49ec88a1db98a0ab201bf2fc1c1bd7f8e8fd029cf0c926d7b4d9da9`  
		Last Modified: Sat, 28 Dec 2019 07:44:43 GMT  
		Size: 244.5 KB (244542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057c0aaa360539994c1b5892216ac926631ea19ea1269ba0e36963e8ac6fc0f9`  
		Last Modified: Sat, 28 Dec 2019 07:44:52 GMT  
		Size: 24.8 MB (24756037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890129caff8054d546862c6b2b367a181759eb470ec3ce30f2964ce61bda8e7e`  
		Last Modified: Sat, 28 Dec 2019 07:47:08 GMT  
		Size: 127.2 MB (127214782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.4` - linux; arm variant v7

```console
$ docker pull mono@sha256:1b171ee2d4a07104ee9cdb7ab6ee8b55e889638ef5dc7bb85b5b4cad39bf92b5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.4 MB (169420597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59fa7d9e9d02ab70d0cfec4f31a640faf31a35662a6a11ad86f677613a3b0bc6`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 05:03:51 GMT
ADD file:2002ba672e32ae75369830ed6a4734ce62e0118e42390b4d657f0985d6b7fd6a in / 
# Sat, 28 Dec 2019 05:03:53 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:38:14 GMT
ENV MONO_VERSION=6.4.0.198
# Sat, 28 Dec 2019 07:38:37 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:39:23 GMT
RUN echo "deb http://download.mono-project.com/repo/debian vs-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 28 Dec 2019 07:47:03 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:77cf262539006c8df77496f500f74a8c1edd158062440fd94d43d5b1292cefee`  
		Last Modified: Sat, 28 Dec 2019 05:11:13 GMT  
		Size: 19.3 MB (19311587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e822ed95bf5ce7f17aeafa98a5c3daf139a20f5759c74336dd13161b850c91`  
		Last Modified: Sat, 28 Dec 2019 07:51:09 GMT  
		Size: 244.6 KB (244564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e67aa2e5005496faabced9b401bd4fc0df82ce220f788a8b482d5e4573297b`  
		Last Modified: Sat, 28 Dec 2019 07:51:15 GMT  
		Size: 24.0 MB (24034502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a9a9874fc368a6ceef4a8e0dfcaf9bd43fcaecea141c0e2e9d6f4126e645f94`  
		Last Modified: Sat, 28 Dec 2019 07:53:12 GMT  
		Size: 125.8 MB (125829944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.4` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:a677a1b7a7dfef327b1e3baa12da34d087b76fde9881b73aeb1231b1e988fd21
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.2 MB (191241428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:028fb1ab94481a5a9131760e452b701b3566c99279c1a7ddbd2526031cd29b9f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:50 GMT
ADD file:8e4d0a1e6805c641fc9d18ebad82e4b01d85c6cb9f87d1ef47d75d150212a392 in / 
# Fri, 22 Nov 2019 13:45:53 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 20:53:28 GMT
ENV MONO_VERSION=6.4.0.198
# Fri, 22 Nov 2019 20:53:48 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 22 Nov 2019 20:54:31 GMT
RUN echo "deb http://download.mono-project.com/repo/debian vs-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 22 Nov 2019 21:00:32 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:98a64bf4db7d2219b4fdd8182188d9422810dee890e997095bfb564a0482eed6`  
		Last Modified: Fri, 22 Nov 2019 13:52:17 GMT  
		Size: 20.4 MB (20385759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a2743b1fbbbe91732990b09c66ef2caee87b5e2cc4a4c3b56fab159729df2f`  
		Last Modified: Fri, 22 Nov 2019 21:08:13 GMT  
		Size: 244.4 KB (244416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db34d520760acec2af59a6940f6b8c2d2af12071dcfc75a183d61e8ae2af23b2`  
		Last Modified: Fri, 22 Nov 2019 21:08:23 GMT  
		Size: 28.8 MB (28763549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f51dba474fc794e019ebb14c554acb9144144a5c07e3bd414fa033f5614a33`  
		Last Modified: Fri, 22 Nov 2019 21:09:57 GMT  
		Size: 141.8 MB (141847704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.4` - linux; 386

```console
$ docker pull mono@sha256:a6212470f1a502c249b8e5ac0e10591419c877b09ee2e7e0d6e6839b7358c898
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.1 MB (238104231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf42d0822c40b3ad59b251a2006460ec49ebb69c7643a39e5d43ea4200f18d6a`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 16:54:44 GMT
ADD file:19d04f738434c76e2dbd14b48de2f0f03afa883b15f638c6ecbbf382df03567c in / 
# Fri, 22 Nov 2019 16:54:44 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 01:07:21 GMT
ENV MONO_VERSION=6.4.0.198
# Sat, 23 Nov 2019 01:07:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 23 Nov 2019 01:08:08 GMT
RUN echo "deb http://download.mono-project.com/repo/debian vs-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 23 Nov 2019 01:12:18 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f26c9a85c76e393c9f2313b30e82d09f933d2dd4883620de242c7d21f8812e91`  
		Last Modified: Fri, 22 Nov 2019 17:03:03 GMT  
		Size: 23.2 MB (23152070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d54843b46358cc679b7b9ed6ac3c98102566536014e6820854dba519e772b0c`  
		Last Modified: Sat, 23 Nov 2019 01:16:39 GMT  
		Size: 244.5 KB (244506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f96e801e3047c9e846bbae422970ab17d1e71a0c136e22ec473666ba1c84fb2`  
		Last Modified: Sat, 23 Nov 2019 01:16:58 GMT  
		Size: 65.9 MB (65947639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08206ccbadeb2b9c91e2ea96cda6de8f1d3e99efa357dace0fa35e319c5891fa`  
		Last Modified: Sat, 23 Nov 2019 01:18:38 GMT  
		Size: 148.8 MB (148760016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.4` - linux; ppc64le

```console
$ docker pull mono@sha256:61bdb2e25fbb1b6f71fc44db3978ea7e775eaaa57b9a336d20b09a09cfc141a4
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.7 MB (175730508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:697edf6ad26895ac6c63d1fd807706f5c137a779a9abd2553bfd6611c300b409`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:21 GMT
ADD file:a1ee5955ff3ede8df9558f4bec0c7962d54c43374f857e1da7e2639ddf82a9f1 in / 
# Sat, 28 Dec 2019 04:23:24 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:02:35 GMT
ENV MONO_VERSION=6.4.0.198
# Sat, 28 Dec 2019 06:03:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 06:04:47 GMT
RUN echo "deb http://download.mono-project.com/repo/debian vs-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 28 Dec 2019 06:15:49 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af52e7ef6e83efadeae17be91daa6ecf61b7dfb39709c29be9b24876e60c0e36`  
		Last Modified: Sat, 28 Dec 2019 04:33:19 GMT  
		Size: 22.8 MB (22800791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85fc9eb11582da6a0be73b7e1050501cffcf51b26db363a95a648082a6b08178`  
		Last Modified: Sat, 28 Dec 2019 06:22:31 GMT  
		Size: 244.6 KB (244593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b94466b100a0063e3f8901325084fae9a526a1601a842a3d15a58fe1086a174`  
		Last Modified: Sat, 28 Dec 2019 06:22:43 GMT  
		Size: 25.1 MB (25123343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7045ddebde43ede8d3cd65d6b58848fa905fd02d72bf2d99e68257f3e75e73ef`  
		Last Modified: Sat, 28 Dec 2019 06:24:50 GMT  
		Size: 127.6 MB (127561781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.4.0`

```console
$ docker pull mono@sha256:23cfeb120eb032fd466687c75c9c48c22b2330fed6435e27ea289bd7f2458003
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.4.0` - linux; amd64

```console
$ docker pull mono@sha256:03fcc004eba262d5068fe2c69aa21ba66284913091ada922e3f52e62d9676174
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.9 MB (229861563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ba93b1033ba2ccaf8b5dbe036fab3faba421ea1b94e183c9cfac7feee17c507`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:59:24 GMT
ADD file:2c1f5e08834f13ccb9c2326204eb2556e03239d00171e75755c7195289374c61 in / 
# Fri, 22 Nov 2019 14:59:25 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 22:59:02 GMT
ENV MONO_VERSION=6.4.0.198
# Fri, 22 Nov 2019 22:59:16 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 22 Nov 2019 22:59:47 GMT
RUN echo "deb http://download.mono-project.com/repo/debian vs-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 22 Nov 2019 23:10:02 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d599a449871ee73b960e80d176b989365dfecb4c8f337bf21e8853862403ee9b`  
		Last Modified: Fri, 22 Nov 2019 15:06:36 GMT  
		Size: 22.5 MB (22524572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d97711e218db482a8b5126b3a4e42b4d779e333becec529e3a1db4a35e37453`  
		Last Modified: Fri, 22 Nov 2019 23:20:12 GMT  
		Size: 244.5 KB (244459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce311d3c9c556425ac31acae067c848ad34faf95766b476fe942501d8c16307`  
		Last Modified: Fri, 22 Nov 2019 23:20:25 GMT  
		Size: 62.2 MB (62239606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98cc01904b7faa8a884765e56bc1f600b68f5b72b302a5d9aea1c483efa850d`  
		Last Modified: Fri, 22 Nov 2019 23:21:43 GMT  
		Size: 144.9 MB (144852926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.4.0` - linux; arm variant v5

```console
$ docker pull mono@sha256:38c5f861b60869c07145058d2627a5c2c32426c6062056c03eb295f78eb4225d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.4 MB (173418183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3fc9fcb755d681a693abbf48833028bd63cdc15bf29f7292a31b53e52d272de`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:53:16 GMT
ADD file:7d6af454b55cb354e31c096e935358dd5914688ded04ebc76243a4ff598c4495 in / 
# Sat, 28 Dec 2019 04:53:18 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:30:03 GMT
ENV MONO_VERSION=6.4.0.198
# Sat, 28 Dec 2019 07:30:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:31:25 GMT
RUN echo "deb http://download.mono-project.com/repo/debian vs-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 28 Dec 2019 07:40:16 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af28f499fd964f4506ea46c2ac342bc52328a8c30cd633661b69f383a5144e9b`  
		Last Modified: Sat, 28 Dec 2019 05:00:23 GMT  
		Size: 21.2 MB (21202822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:debae7c5f49ec88a1db98a0ab201bf2fc1c1bd7f8e8fd029cf0c926d7b4d9da9`  
		Last Modified: Sat, 28 Dec 2019 07:44:43 GMT  
		Size: 244.5 KB (244542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057c0aaa360539994c1b5892216ac926631ea19ea1269ba0e36963e8ac6fc0f9`  
		Last Modified: Sat, 28 Dec 2019 07:44:52 GMT  
		Size: 24.8 MB (24756037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890129caff8054d546862c6b2b367a181759eb470ec3ce30f2964ce61bda8e7e`  
		Last Modified: Sat, 28 Dec 2019 07:47:08 GMT  
		Size: 127.2 MB (127214782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.4.0` - linux; arm variant v7

```console
$ docker pull mono@sha256:1b171ee2d4a07104ee9cdb7ab6ee8b55e889638ef5dc7bb85b5b4cad39bf92b5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.4 MB (169420597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59fa7d9e9d02ab70d0cfec4f31a640faf31a35662a6a11ad86f677613a3b0bc6`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 05:03:51 GMT
ADD file:2002ba672e32ae75369830ed6a4734ce62e0118e42390b4d657f0985d6b7fd6a in / 
# Sat, 28 Dec 2019 05:03:53 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:38:14 GMT
ENV MONO_VERSION=6.4.0.198
# Sat, 28 Dec 2019 07:38:37 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:39:23 GMT
RUN echo "deb http://download.mono-project.com/repo/debian vs-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 28 Dec 2019 07:47:03 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:77cf262539006c8df77496f500f74a8c1edd158062440fd94d43d5b1292cefee`  
		Last Modified: Sat, 28 Dec 2019 05:11:13 GMT  
		Size: 19.3 MB (19311587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e822ed95bf5ce7f17aeafa98a5c3daf139a20f5759c74336dd13161b850c91`  
		Last Modified: Sat, 28 Dec 2019 07:51:09 GMT  
		Size: 244.6 KB (244564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e67aa2e5005496faabced9b401bd4fc0df82ce220f788a8b482d5e4573297b`  
		Last Modified: Sat, 28 Dec 2019 07:51:15 GMT  
		Size: 24.0 MB (24034502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a9a9874fc368a6ceef4a8e0dfcaf9bd43fcaecea141c0e2e9d6f4126e645f94`  
		Last Modified: Sat, 28 Dec 2019 07:53:12 GMT  
		Size: 125.8 MB (125829944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.4.0` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:a677a1b7a7dfef327b1e3baa12da34d087b76fde9881b73aeb1231b1e988fd21
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.2 MB (191241428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:028fb1ab94481a5a9131760e452b701b3566c99279c1a7ddbd2526031cd29b9f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:50 GMT
ADD file:8e4d0a1e6805c641fc9d18ebad82e4b01d85c6cb9f87d1ef47d75d150212a392 in / 
# Fri, 22 Nov 2019 13:45:53 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 20:53:28 GMT
ENV MONO_VERSION=6.4.0.198
# Fri, 22 Nov 2019 20:53:48 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 22 Nov 2019 20:54:31 GMT
RUN echo "deb http://download.mono-project.com/repo/debian vs-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 22 Nov 2019 21:00:32 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:98a64bf4db7d2219b4fdd8182188d9422810dee890e997095bfb564a0482eed6`  
		Last Modified: Fri, 22 Nov 2019 13:52:17 GMT  
		Size: 20.4 MB (20385759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a2743b1fbbbe91732990b09c66ef2caee87b5e2cc4a4c3b56fab159729df2f`  
		Last Modified: Fri, 22 Nov 2019 21:08:13 GMT  
		Size: 244.4 KB (244416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db34d520760acec2af59a6940f6b8c2d2af12071dcfc75a183d61e8ae2af23b2`  
		Last Modified: Fri, 22 Nov 2019 21:08:23 GMT  
		Size: 28.8 MB (28763549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f51dba474fc794e019ebb14c554acb9144144a5c07e3bd414fa033f5614a33`  
		Last Modified: Fri, 22 Nov 2019 21:09:57 GMT  
		Size: 141.8 MB (141847704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.4.0` - linux; 386

```console
$ docker pull mono@sha256:a6212470f1a502c249b8e5ac0e10591419c877b09ee2e7e0d6e6839b7358c898
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.1 MB (238104231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf42d0822c40b3ad59b251a2006460ec49ebb69c7643a39e5d43ea4200f18d6a`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 16:54:44 GMT
ADD file:19d04f738434c76e2dbd14b48de2f0f03afa883b15f638c6ecbbf382df03567c in / 
# Fri, 22 Nov 2019 16:54:44 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 01:07:21 GMT
ENV MONO_VERSION=6.4.0.198
# Sat, 23 Nov 2019 01:07:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 23 Nov 2019 01:08:08 GMT
RUN echo "deb http://download.mono-project.com/repo/debian vs-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 23 Nov 2019 01:12:18 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f26c9a85c76e393c9f2313b30e82d09f933d2dd4883620de242c7d21f8812e91`  
		Last Modified: Fri, 22 Nov 2019 17:03:03 GMT  
		Size: 23.2 MB (23152070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d54843b46358cc679b7b9ed6ac3c98102566536014e6820854dba519e772b0c`  
		Last Modified: Sat, 23 Nov 2019 01:16:39 GMT  
		Size: 244.5 KB (244506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f96e801e3047c9e846bbae422970ab17d1e71a0c136e22ec473666ba1c84fb2`  
		Last Modified: Sat, 23 Nov 2019 01:16:58 GMT  
		Size: 65.9 MB (65947639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08206ccbadeb2b9c91e2ea96cda6de8f1d3e99efa357dace0fa35e319c5891fa`  
		Last Modified: Sat, 23 Nov 2019 01:18:38 GMT  
		Size: 148.8 MB (148760016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.4.0` - linux; ppc64le

```console
$ docker pull mono@sha256:61bdb2e25fbb1b6f71fc44db3978ea7e775eaaa57b9a336d20b09a09cfc141a4
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.7 MB (175730508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:697edf6ad26895ac6c63d1fd807706f5c137a779a9abd2553bfd6611c300b409`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:21 GMT
ADD file:a1ee5955ff3ede8df9558f4bec0c7962d54c43374f857e1da7e2639ddf82a9f1 in / 
# Sat, 28 Dec 2019 04:23:24 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:02:35 GMT
ENV MONO_VERSION=6.4.0.198
# Sat, 28 Dec 2019 06:03:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 06:04:47 GMT
RUN echo "deb http://download.mono-project.com/repo/debian vs-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 28 Dec 2019 06:15:49 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af52e7ef6e83efadeae17be91daa6ecf61b7dfb39709c29be9b24876e60c0e36`  
		Last Modified: Sat, 28 Dec 2019 04:33:19 GMT  
		Size: 22.8 MB (22800791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85fc9eb11582da6a0be73b7e1050501cffcf51b26db363a95a648082a6b08178`  
		Last Modified: Sat, 28 Dec 2019 06:22:31 GMT  
		Size: 244.6 KB (244593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b94466b100a0063e3f8901325084fae9a526a1601a842a3d15a58fe1086a174`  
		Last Modified: Sat, 28 Dec 2019 06:22:43 GMT  
		Size: 25.1 MB (25123343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7045ddebde43ede8d3cd65d6b58848fa905fd02d72bf2d99e68257f3e75e73ef`  
		Last Modified: Sat, 28 Dec 2019 06:24:50 GMT  
		Size: 127.6 MB (127561781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.4.0.198`

```console
$ docker pull mono@sha256:23cfeb120eb032fd466687c75c9c48c22b2330fed6435e27ea289bd7f2458003
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.4.0.198` - linux; amd64

```console
$ docker pull mono@sha256:03fcc004eba262d5068fe2c69aa21ba66284913091ada922e3f52e62d9676174
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.9 MB (229861563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ba93b1033ba2ccaf8b5dbe036fab3faba421ea1b94e183c9cfac7feee17c507`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:59:24 GMT
ADD file:2c1f5e08834f13ccb9c2326204eb2556e03239d00171e75755c7195289374c61 in / 
# Fri, 22 Nov 2019 14:59:25 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 22:59:02 GMT
ENV MONO_VERSION=6.4.0.198
# Fri, 22 Nov 2019 22:59:16 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 22 Nov 2019 22:59:47 GMT
RUN echo "deb http://download.mono-project.com/repo/debian vs-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 22 Nov 2019 23:10:02 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d599a449871ee73b960e80d176b989365dfecb4c8f337bf21e8853862403ee9b`  
		Last Modified: Fri, 22 Nov 2019 15:06:36 GMT  
		Size: 22.5 MB (22524572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d97711e218db482a8b5126b3a4e42b4d779e333becec529e3a1db4a35e37453`  
		Last Modified: Fri, 22 Nov 2019 23:20:12 GMT  
		Size: 244.5 KB (244459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce311d3c9c556425ac31acae067c848ad34faf95766b476fe942501d8c16307`  
		Last Modified: Fri, 22 Nov 2019 23:20:25 GMT  
		Size: 62.2 MB (62239606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98cc01904b7faa8a884765e56bc1f600b68f5b72b302a5d9aea1c483efa850d`  
		Last Modified: Fri, 22 Nov 2019 23:21:43 GMT  
		Size: 144.9 MB (144852926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.4.0.198` - linux; arm variant v5

```console
$ docker pull mono@sha256:38c5f861b60869c07145058d2627a5c2c32426c6062056c03eb295f78eb4225d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.4 MB (173418183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3fc9fcb755d681a693abbf48833028bd63cdc15bf29f7292a31b53e52d272de`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:53:16 GMT
ADD file:7d6af454b55cb354e31c096e935358dd5914688ded04ebc76243a4ff598c4495 in / 
# Sat, 28 Dec 2019 04:53:18 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:30:03 GMT
ENV MONO_VERSION=6.4.0.198
# Sat, 28 Dec 2019 07:30:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:31:25 GMT
RUN echo "deb http://download.mono-project.com/repo/debian vs-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 28 Dec 2019 07:40:16 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af28f499fd964f4506ea46c2ac342bc52328a8c30cd633661b69f383a5144e9b`  
		Last Modified: Sat, 28 Dec 2019 05:00:23 GMT  
		Size: 21.2 MB (21202822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:debae7c5f49ec88a1db98a0ab201bf2fc1c1bd7f8e8fd029cf0c926d7b4d9da9`  
		Last Modified: Sat, 28 Dec 2019 07:44:43 GMT  
		Size: 244.5 KB (244542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057c0aaa360539994c1b5892216ac926631ea19ea1269ba0e36963e8ac6fc0f9`  
		Last Modified: Sat, 28 Dec 2019 07:44:52 GMT  
		Size: 24.8 MB (24756037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890129caff8054d546862c6b2b367a181759eb470ec3ce30f2964ce61bda8e7e`  
		Last Modified: Sat, 28 Dec 2019 07:47:08 GMT  
		Size: 127.2 MB (127214782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.4.0.198` - linux; arm variant v7

```console
$ docker pull mono@sha256:1b171ee2d4a07104ee9cdb7ab6ee8b55e889638ef5dc7bb85b5b4cad39bf92b5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.4 MB (169420597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59fa7d9e9d02ab70d0cfec4f31a640faf31a35662a6a11ad86f677613a3b0bc6`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 05:03:51 GMT
ADD file:2002ba672e32ae75369830ed6a4734ce62e0118e42390b4d657f0985d6b7fd6a in / 
# Sat, 28 Dec 2019 05:03:53 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:38:14 GMT
ENV MONO_VERSION=6.4.0.198
# Sat, 28 Dec 2019 07:38:37 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:39:23 GMT
RUN echo "deb http://download.mono-project.com/repo/debian vs-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 28 Dec 2019 07:47:03 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:77cf262539006c8df77496f500f74a8c1edd158062440fd94d43d5b1292cefee`  
		Last Modified: Sat, 28 Dec 2019 05:11:13 GMT  
		Size: 19.3 MB (19311587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e822ed95bf5ce7f17aeafa98a5c3daf139a20f5759c74336dd13161b850c91`  
		Last Modified: Sat, 28 Dec 2019 07:51:09 GMT  
		Size: 244.6 KB (244564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e67aa2e5005496faabced9b401bd4fc0df82ce220f788a8b482d5e4573297b`  
		Last Modified: Sat, 28 Dec 2019 07:51:15 GMT  
		Size: 24.0 MB (24034502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a9a9874fc368a6ceef4a8e0dfcaf9bd43fcaecea141c0e2e9d6f4126e645f94`  
		Last Modified: Sat, 28 Dec 2019 07:53:12 GMT  
		Size: 125.8 MB (125829944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.4.0.198` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:a677a1b7a7dfef327b1e3baa12da34d087b76fde9881b73aeb1231b1e988fd21
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.2 MB (191241428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:028fb1ab94481a5a9131760e452b701b3566c99279c1a7ddbd2526031cd29b9f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:50 GMT
ADD file:8e4d0a1e6805c641fc9d18ebad82e4b01d85c6cb9f87d1ef47d75d150212a392 in / 
# Fri, 22 Nov 2019 13:45:53 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 20:53:28 GMT
ENV MONO_VERSION=6.4.0.198
# Fri, 22 Nov 2019 20:53:48 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 22 Nov 2019 20:54:31 GMT
RUN echo "deb http://download.mono-project.com/repo/debian vs-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 22 Nov 2019 21:00:32 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:98a64bf4db7d2219b4fdd8182188d9422810dee890e997095bfb564a0482eed6`  
		Last Modified: Fri, 22 Nov 2019 13:52:17 GMT  
		Size: 20.4 MB (20385759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a2743b1fbbbe91732990b09c66ef2caee87b5e2cc4a4c3b56fab159729df2f`  
		Last Modified: Fri, 22 Nov 2019 21:08:13 GMT  
		Size: 244.4 KB (244416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db34d520760acec2af59a6940f6b8c2d2af12071dcfc75a183d61e8ae2af23b2`  
		Last Modified: Fri, 22 Nov 2019 21:08:23 GMT  
		Size: 28.8 MB (28763549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f51dba474fc794e019ebb14c554acb9144144a5c07e3bd414fa033f5614a33`  
		Last Modified: Fri, 22 Nov 2019 21:09:57 GMT  
		Size: 141.8 MB (141847704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.4.0.198` - linux; 386

```console
$ docker pull mono@sha256:a6212470f1a502c249b8e5ac0e10591419c877b09ee2e7e0d6e6839b7358c898
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.1 MB (238104231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf42d0822c40b3ad59b251a2006460ec49ebb69c7643a39e5d43ea4200f18d6a`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 16:54:44 GMT
ADD file:19d04f738434c76e2dbd14b48de2f0f03afa883b15f638c6ecbbf382df03567c in / 
# Fri, 22 Nov 2019 16:54:44 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 01:07:21 GMT
ENV MONO_VERSION=6.4.0.198
# Sat, 23 Nov 2019 01:07:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 23 Nov 2019 01:08:08 GMT
RUN echo "deb http://download.mono-project.com/repo/debian vs-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 23 Nov 2019 01:12:18 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f26c9a85c76e393c9f2313b30e82d09f933d2dd4883620de242c7d21f8812e91`  
		Last Modified: Fri, 22 Nov 2019 17:03:03 GMT  
		Size: 23.2 MB (23152070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d54843b46358cc679b7b9ed6ac3c98102566536014e6820854dba519e772b0c`  
		Last Modified: Sat, 23 Nov 2019 01:16:39 GMT  
		Size: 244.5 KB (244506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f96e801e3047c9e846bbae422970ab17d1e71a0c136e22ec473666ba1c84fb2`  
		Last Modified: Sat, 23 Nov 2019 01:16:58 GMT  
		Size: 65.9 MB (65947639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08206ccbadeb2b9c91e2ea96cda6de8f1d3e99efa357dace0fa35e319c5891fa`  
		Last Modified: Sat, 23 Nov 2019 01:18:38 GMT  
		Size: 148.8 MB (148760016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.4.0.198` - linux; ppc64le

```console
$ docker pull mono@sha256:61bdb2e25fbb1b6f71fc44db3978ea7e775eaaa57b9a336d20b09a09cfc141a4
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.7 MB (175730508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:697edf6ad26895ac6c63d1fd807706f5c137a779a9abd2553bfd6611c300b409`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:21 GMT
ADD file:a1ee5955ff3ede8df9558f4bec0c7962d54c43374f857e1da7e2639ddf82a9f1 in / 
# Sat, 28 Dec 2019 04:23:24 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:02:35 GMT
ENV MONO_VERSION=6.4.0.198
# Sat, 28 Dec 2019 06:03:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 06:04:47 GMT
RUN echo "deb http://download.mono-project.com/repo/debian vs-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 28 Dec 2019 06:15:49 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af52e7ef6e83efadeae17be91daa6ecf61b7dfb39709c29be9b24876e60c0e36`  
		Last Modified: Sat, 28 Dec 2019 04:33:19 GMT  
		Size: 22.8 MB (22800791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85fc9eb11582da6a0be73b7e1050501cffcf51b26db363a95a648082a6b08178`  
		Last Modified: Sat, 28 Dec 2019 06:22:31 GMT  
		Size: 244.6 KB (244593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b94466b100a0063e3f8901325084fae9a526a1601a842a3d15a58fe1086a174`  
		Last Modified: Sat, 28 Dec 2019 06:22:43 GMT  
		Size: 25.1 MB (25123343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7045ddebde43ede8d3cd65d6b58848fa905fd02d72bf2d99e68257f3e75e73ef`  
		Last Modified: Sat, 28 Dec 2019 06:24:50 GMT  
		Size: 127.6 MB (127561781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.4.0.198-slim`

```console
$ docker pull mono@sha256:7c3cf1e75d0175b96a6896b98cf8ec3f42353b0105577cf6987de63a3fe6dea2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.4.0.198-slim` - linux; amd64

```console
$ docker pull mono@sha256:7a15bca26a8cf7d934ad14208df631ee2dec877629ac1235e75f7b8b814a1625
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.0 MB (85008637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:026f91a4b8fb522bad9088aa82f78d3cb54c7229a136c7582af994bcc5804e16`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:59:24 GMT
ADD file:2c1f5e08834f13ccb9c2326204eb2556e03239d00171e75755c7195289374c61 in / 
# Fri, 22 Nov 2019 14:59:25 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 22:59:02 GMT
ENV MONO_VERSION=6.4.0.198
# Fri, 22 Nov 2019 22:59:16 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 22 Nov 2019 22:59:47 GMT
RUN echo "deb http://download.mono-project.com/repo/debian vs-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d599a449871ee73b960e80d176b989365dfecb4c8f337bf21e8853862403ee9b`  
		Last Modified: Fri, 22 Nov 2019 15:06:36 GMT  
		Size: 22.5 MB (22524572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d97711e218db482a8b5126b3a4e42b4d779e333becec529e3a1db4a35e37453`  
		Last Modified: Fri, 22 Nov 2019 23:20:12 GMT  
		Size: 244.5 KB (244459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce311d3c9c556425ac31acae067c848ad34faf95766b476fe942501d8c16307`  
		Last Modified: Fri, 22 Nov 2019 23:20:25 GMT  
		Size: 62.2 MB (62239606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.4.0.198-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:fa9c25bcb3cbddea501fe7fb1e5468bdfb9d6b7afd88e172e576189e926f304f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.2 MB (46203401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e23c0fe1f4d6ca48e32de474b52be4e77587a1707aa8abe9d3e834b28e90bbfe`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:53:16 GMT
ADD file:7d6af454b55cb354e31c096e935358dd5914688ded04ebc76243a4ff598c4495 in / 
# Sat, 28 Dec 2019 04:53:18 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:30:03 GMT
ENV MONO_VERSION=6.4.0.198
# Sat, 28 Dec 2019 07:30:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:31:25 GMT
RUN echo "deb http://download.mono-project.com/repo/debian vs-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af28f499fd964f4506ea46c2ac342bc52328a8c30cd633661b69f383a5144e9b`  
		Last Modified: Sat, 28 Dec 2019 05:00:23 GMT  
		Size: 21.2 MB (21202822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:debae7c5f49ec88a1db98a0ab201bf2fc1c1bd7f8e8fd029cf0c926d7b4d9da9`  
		Last Modified: Sat, 28 Dec 2019 07:44:43 GMT  
		Size: 244.5 KB (244542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057c0aaa360539994c1b5892216ac926631ea19ea1269ba0e36963e8ac6fc0f9`  
		Last Modified: Sat, 28 Dec 2019 07:44:52 GMT  
		Size: 24.8 MB (24756037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.4.0.198-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:20749c49255566c003b86ebffacdb862d2ba57a2db7c71baba890542c8b44226
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.6 MB (43590653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:595cc4caa293b852ce915daf545b46dddc98617867e5466fb92003d85a055711`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 05:03:51 GMT
ADD file:2002ba672e32ae75369830ed6a4734ce62e0118e42390b4d657f0985d6b7fd6a in / 
# Sat, 28 Dec 2019 05:03:53 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:38:14 GMT
ENV MONO_VERSION=6.4.0.198
# Sat, 28 Dec 2019 07:38:37 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:39:23 GMT
RUN echo "deb http://download.mono-project.com/repo/debian vs-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:77cf262539006c8df77496f500f74a8c1edd158062440fd94d43d5b1292cefee`  
		Last Modified: Sat, 28 Dec 2019 05:11:13 GMT  
		Size: 19.3 MB (19311587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e822ed95bf5ce7f17aeafa98a5c3daf139a20f5759c74336dd13161b850c91`  
		Last Modified: Sat, 28 Dec 2019 07:51:09 GMT  
		Size: 244.6 KB (244564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e67aa2e5005496faabced9b401bd4fc0df82ce220f788a8b482d5e4573297b`  
		Last Modified: Sat, 28 Dec 2019 07:51:15 GMT  
		Size: 24.0 MB (24034502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.4.0.198-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:1f4934f1efe69c26a98185a2bc99e580a526aa735cc4da9844aff46be9a15fe5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49393724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc3943b43108c053d1ea7c38ad4ed1e150e4bdab803de5acf46dff74c87bfa76`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:50 GMT
ADD file:8e4d0a1e6805c641fc9d18ebad82e4b01d85c6cb9f87d1ef47d75d150212a392 in / 
# Fri, 22 Nov 2019 13:45:53 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 20:53:28 GMT
ENV MONO_VERSION=6.4.0.198
# Fri, 22 Nov 2019 20:53:48 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 22 Nov 2019 20:54:31 GMT
RUN echo "deb http://download.mono-project.com/repo/debian vs-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:98a64bf4db7d2219b4fdd8182188d9422810dee890e997095bfb564a0482eed6`  
		Last Modified: Fri, 22 Nov 2019 13:52:17 GMT  
		Size: 20.4 MB (20385759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a2743b1fbbbe91732990b09c66ef2caee87b5e2cc4a4c3b56fab159729df2f`  
		Last Modified: Fri, 22 Nov 2019 21:08:13 GMT  
		Size: 244.4 KB (244416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db34d520760acec2af59a6940f6b8c2d2af12071dcfc75a183d61e8ae2af23b2`  
		Last Modified: Fri, 22 Nov 2019 21:08:23 GMT  
		Size: 28.8 MB (28763549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.4.0.198-slim` - linux; 386

```console
$ docker pull mono@sha256:6b3298a6b8ce9aff69db1eddccb45ef69b667caefedcfb1880962f18abc0f2ec
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.3 MB (89344215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26dc5bc379839014faebab7da7370e7557adfc4c8d4f775698580a3206a6934e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 16:54:44 GMT
ADD file:19d04f738434c76e2dbd14b48de2f0f03afa883b15f638c6ecbbf382df03567c in / 
# Fri, 22 Nov 2019 16:54:44 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 01:07:21 GMT
ENV MONO_VERSION=6.4.0.198
# Sat, 23 Nov 2019 01:07:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 23 Nov 2019 01:08:08 GMT
RUN echo "deb http://download.mono-project.com/repo/debian vs-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f26c9a85c76e393c9f2313b30e82d09f933d2dd4883620de242c7d21f8812e91`  
		Last Modified: Fri, 22 Nov 2019 17:03:03 GMT  
		Size: 23.2 MB (23152070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d54843b46358cc679b7b9ed6ac3c98102566536014e6820854dba519e772b0c`  
		Last Modified: Sat, 23 Nov 2019 01:16:39 GMT  
		Size: 244.5 KB (244506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f96e801e3047c9e846bbae422970ab17d1e71a0c136e22ec473666ba1c84fb2`  
		Last Modified: Sat, 23 Nov 2019 01:16:58 GMT  
		Size: 65.9 MB (65947639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.4.0.198-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:e696b74e509b6aeef319821d8417a54ff5f6003098436984d1c99e3debae17de
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48168727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:162ad102e676c3e612d565f88ffaa89080fa7d9cf970059e8e7c34b5b5410d2f`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:21 GMT
ADD file:a1ee5955ff3ede8df9558f4bec0c7962d54c43374f857e1da7e2639ddf82a9f1 in / 
# Sat, 28 Dec 2019 04:23:24 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:02:35 GMT
ENV MONO_VERSION=6.4.0.198
# Sat, 28 Dec 2019 06:03:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 06:04:47 GMT
RUN echo "deb http://download.mono-project.com/repo/debian vs-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af52e7ef6e83efadeae17be91daa6ecf61b7dfb39709c29be9b24876e60c0e36`  
		Last Modified: Sat, 28 Dec 2019 04:33:19 GMT  
		Size: 22.8 MB (22800791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85fc9eb11582da6a0be73b7e1050501cffcf51b26db363a95a648082a6b08178`  
		Last Modified: Sat, 28 Dec 2019 06:22:31 GMT  
		Size: 244.6 KB (244593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b94466b100a0063e3f8901325084fae9a526a1601a842a3d15a58fe1086a174`  
		Last Modified: Sat, 28 Dec 2019 06:22:43 GMT  
		Size: 25.1 MB (25123343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.4.0-slim`

```console
$ docker pull mono@sha256:7c3cf1e75d0175b96a6896b98cf8ec3f42353b0105577cf6987de63a3fe6dea2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.4.0-slim` - linux; amd64

```console
$ docker pull mono@sha256:7a15bca26a8cf7d934ad14208df631ee2dec877629ac1235e75f7b8b814a1625
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.0 MB (85008637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:026f91a4b8fb522bad9088aa82f78d3cb54c7229a136c7582af994bcc5804e16`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:59:24 GMT
ADD file:2c1f5e08834f13ccb9c2326204eb2556e03239d00171e75755c7195289374c61 in / 
# Fri, 22 Nov 2019 14:59:25 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 22:59:02 GMT
ENV MONO_VERSION=6.4.0.198
# Fri, 22 Nov 2019 22:59:16 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 22 Nov 2019 22:59:47 GMT
RUN echo "deb http://download.mono-project.com/repo/debian vs-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d599a449871ee73b960e80d176b989365dfecb4c8f337bf21e8853862403ee9b`  
		Last Modified: Fri, 22 Nov 2019 15:06:36 GMT  
		Size: 22.5 MB (22524572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d97711e218db482a8b5126b3a4e42b4d779e333becec529e3a1db4a35e37453`  
		Last Modified: Fri, 22 Nov 2019 23:20:12 GMT  
		Size: 244.5 KB (244459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce311d3c9c556425ac31acae067c848ad34faf95766b476fe942501d8c16307`  
		Last Modified: Fri, 22 Nov 2019 23:20:25 GMT  
		Size: 62.2 MB (62239606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.4.0-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:fa9c25bcb3cbddea501fe7fb1e5468bdfb9d6b7afd88e172e576189e926f304f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.2 MB (46203401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e23c0fe1f4d6ca48e32de474b52be4e77587a1707aa8abe9d3e834b28e90bbfe`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:53:16 GMT
ADD file:7d6af454b55cb354e31c096e935358dd5914688ded04ebc76243a4ff598c4495 in / 
# Sat, 28 Dec 2019 04:53:18 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:30:03 GMT
ENV MONO_VERSION=6.4.0.198
# Sat, 28 Dec 2019 07:30:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:31:25 GMT
RUN echo "deb http://download.mono-project.com/repo/debian vs-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af28f499fd964f4506ea46c2ac342bc52328a8c30cd633661b69f383a5144e9b`  
		Last Modified: Sat, 28 Dec 2019 05:00:23 GMT  
		Size: 21.2 MB (21202822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:debae7c5f49ec88a1db98a0ab201bf2fc1c1bd7f8e8fd029cf0c926d7b4d9da9`  
		Last Modified: Sat, 28 Dec 2019 07:44:43 GMT  
		Size: 244.5 KB (244542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057c0aaa360539994c1b5892216ac926631ea19ea1269ba0e36963e8ac6fc0f9`  
		Last Modified: Sat, 28 Dec 2019 07:44:52 GMT  
		Size: 24.8 MB (24756037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.4.0-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:20749c49255566c003b86ebffacdb862d2ba57a2db7c71baba890542c8b44226
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.6 MB (43590653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:595cc4caa293b852ce915daf545b46dddc98617867e5466fb92003d85a055711`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 05:03:51 GMT
ADD file:2002ba672e32ae75369830ed6a4734ce62e0118e42390b4d657f0985d6b7fd6a in / 
# Sat, 28 Dec 2019 05:03:53 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:38:14 GMT
ENV MONO_VERSION=6.4.0.198
# Sat, 28 Dec 2019 07:38:37 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:39:23 GMT
RUN echo "deb http://download.mono-project.com/repo/debian vs-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:77cf262539006c8df77496f500f74a8c1edd158062440fd94d43d5b1292cefee`  
		Last Modified: Sat, 28 Dec 2019 05:11:13 GMT  
		Size: 19.3 MB (19311587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e822ed95bf5ce7f17aeafa98a5c3daf139a20f5759c74336dd13161b850c91`  
		Last Modified: Sat, 28 Dec 2019 07:51:09 GMT  
		Size: 244.6 KB (244564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e67aa2e5005496faabced9b401bd4fc0df82ce220f788a8b482d5e4573297b`  
		Last Modified: Sat, 28 Dec 2019 07:51:15 GMT  
		Size: 24.0 MB (24034502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.4.0-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:1f4934f1efe69c26a98185a2bc99e580a526aa735cc4da9844aff46be9a15fe5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49393724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc3943b43108c053d1ea7c38ad4ed1e150e4bdab803de5acf46dff74c87bfa76`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:50 GMT
ADD file:8e4d0a1e6805c641fc9d18ebad82e4b01d85c6cb9f87d1ef47d75d150212a392 in / 
# Fri, 22 Nov 2019 13:45:53 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 20:53:28 GMT
ENV MONO_VERSION=6.4.0.198
# Fri, 22 Nov 2019 20:53:48 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 22 Nov 2019 20:54:31 GMT
RUN echo "deb http://download.mono-project.com/repo/debian vs-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:98a64bf4db7d2219b4fdd8182188d9422810dee890e997095bfb564a0482eed6`  
		Last Modified: Fri, 22 Nov 2019 13:52:17 GMT  
		Size: 20.4 MB (20385759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a2743b1fbbbe91732990b09c66ef2caee87b5e2cc4a4c3b56fab159729df2f`  
		Last Modified: Fri, 22 Nov 2019 21:08:13 GMT  
		Size: 244.4 KB (244416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db34d520760acec2af59a6940f6b8c2d2af12071dcfc75a183d61e8ae2af23b2`  
		Last Modified: Fri, 22 Nov 2019 21:08:23 GMT  
		Size: 28.8 MB (28763549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.4.0-slim` - linux; 386

```console
$ docker pull mono@sha256:6b3298a6b8ce9aff69db1eddccb45ef69b667caefedcfb1880962f18abc0f2ec
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.3 MB (89344215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26dc5bc379839014faebab7da7370e7557adfc4c8d4f775698580a3206a6934e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 16:54:44 GMT
ADD file:19d04f738434c76e2dbd14b48de2f0f03afa883b15f638c6ecbbf382df03567c in / 
# Fri, 22 Nov 2019 16:54:44 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 01:07:21 GMT
ENV MONO_VERSION=6.4.0.198
# Sat, 23 Nov 2019 01:07:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 23 Nov 2019 01:08:08 GMT
RUN echo "deb http://download.mono-project.com/repo/debian vs-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f26c9a85c76e393c9f2313b30e82d09f933d2dd4883620de242c7d21f8812e91`  
		Last Modified: Fri, 22 Nov 2019 17:03:03 GMT  
		Size: 23.2 MB (23152070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d54843b46358cc679b7b9ed6ac3c98102566536014e6820854dba519e772b0c`  
		Last Modified: Sat, 23 Nov 2019 01:16:39 GMT  
		Size: 244.5 KB (244506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f96e801e3047c9e846bbae422970ab17d1e71a0c136e22ec473666ba1c84fb2`  
		Last Modified: Sat, 23 Nov 2019 01:16:58 GMT  
		Size: 65.9 MB (65947639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.4.0-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:e696b74e509b6aeef319821d8417a54ff5f6003098436984d1c99e3debae17de
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48168727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:162ad102e676c3e612d565f88ffaa89080fa7d9cf970059e8e7c34b5b5410d2f`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:21 GMT
ADD file:a1ee5955ff3ede8df9558f4bec0c7962d54c43374f857e1da7e2639ddf82a9f1 in / 
# Sat, 28 Dec 2019 04:23:24 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:02:35 GMT
ENV MONO_VERSION=6.4.0.198
# Sat, 28 Dec 2019 06:03:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 06:04:47 GMT
RUN echo "deb http://download.mono-project.com/repo/debian vs-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af52e7ef6e83efadeae17be91daa6ecf61b7dfb39709c29be9b24876e60c0e36`  
		Last Modified: Sat, 28 Dec 2019 04:33:19 GMT  
		Size: 22.8 MB (22800791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85fc9eb11582da6a0be73b7e1050501cffcf51b26db363a95a648082a6b08178`  
		Last Modified: Sat, 28 Dec 2019 06:22:31 GMT  
		Size: 244.6 KB (244593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b94466b100a0063e3f8901325084fae9a526a1601a842a3d15a58fe1086a174`  
		Last Modified: Sat, 28 Dec 2019 06:22:43 GMT  
		Size: 25.1 MB (25123343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.4-slim`

```console
$ docker pull mono@sha256:7c3cf1e75d0175b96a6896b98cf8ec3f42353b0105577cf6987de63a3fe6dea2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.4-slim` - linux; amd64

```console
$ docker pull mono@sha256:7a15bca26a8cf7d934ad14208df631ee2dec877629ac1235e75f7b8b814a1625
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.0 MB (85008637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:026f91a4b8fb522bad9088aa82f78d3cb54c7229a136c7582af994bcc5804e16`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:59:24 GMT
ADD file:2c1f5e08834f13ccb9c2326204eb2556e03239d00171e75755c7195289374c61 in / 
# Fri, 22 Nov 2019 14:59:25 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 22:59:02 GMT
ENV MONO_VERSION=6.4.0.198
# Fri, 22 Nov 2019 22:59:16 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 22 Nov 2019 22:59:47 GMT
RUN echo "deb http://download.mono-project.com/repo/debian vs-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d599a449871ee73b960e80d176b989365dfecb4c8f337bf21e8853862403ee9b`  
		Last Modified: Fri, 22 Nov 2019 15:06:36 GMT  
		Size: 22.5 MB (22524572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d97711e218db482a8b5126b3a4e42b4d779e333becec529e3a1db4a35e37453`  
		Last Modified: Fri, 22 Nov 2019 23:20:12 GMT  
		Size: 244.5 KB (244459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce311d3c9c556425ac31acae067c848ad34faf95766b476fe942501d8c16307`  
		Last Modified: Fri, 22 Nov 2019 23:20:25 GMT  
		Size: 62.2 MB (62239606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.4-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:fa9c25bcb3cbddea501fe7fb1e5468bdfb9d6b7afd88e172e576189e926f304f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.2 MB (46203401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e23c0fe1f4d6ca48e32de474b52be4e77587a1707aa8abe9d3e834b28e90bbfe`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:53:16 GMT
ADD file:7d6af454b55cb354e31c096e935358dd5914688ded04ebc76243a4ff598c4495 in / 
# Sat, 28 Dec 2019 04:53:18 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:30:03 GMT
ENV MONO_VERSION=6.4.0.198
# Sat, 28 Dec 2019 07:30:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:31:25 GMT
RUN echo "deb http://download.mono-project.com/repo/debian vs-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af28f499fd964f4506ea46c2ac342bc52328a8c30cd633661b69f383a5144e9b`  
		Last Modified: Sat, 28 Dec 2019 05:00:23 GMT  
		Size: 21.2 MB (21202822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:debae7c5f49ec88a1db98a0ab201bf2fc1c1bd7f8e8fd029cf0c926d7b4d9da9`  
		Last Modified: Sat, 28 Dec 2019 07:44:43 GMT  
		Size: 244.5 KB (244542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057c0aaa360539994c1b5892216ac926631ea19ea1269ba0e36963e8ac6fc0f9`  
		Last Modified: Sat, 28 Dec 2019 07:44:52 GMT  
		Size: 24.8 MB (24756037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.4-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:20749c49255566c003b86ebffacdb862d2ba57a2db7c71baba890542c8b44226
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.6 MB (43590653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:595cc4caa293b852ce915daf545b46dddc98617867e5466fb92003d85a055711`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 05:03:51 GMT
ADD file:2002ba672e32ae75369830ed6a4734ce62e0118e42390b4d657f0985d6b7fd6a in / 
# Sat, 28 Dec 2019 05:03:53 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:38:14 GMT
ENV MONO_VERSION=6.4.0.198
# Sat, 28 Dec 2019 07:38:37 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:39:23 GMT
RUN echo "deb http://download.mono-project.com/repo/debian vs-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:77cf262539006c8df77496f500f74a8c1edd158062440fd94d43d5b1292cefee`  
		Last Modified: Sat, 28 Dec 2019 05:11:13 GMT  
		Size: 19.3 MB (19311587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e822ed95bf5ce7f17aeafa98a5c3daf139a20f5759c74336dd13161b850c91`  
		Last Modified: Sat, 28 Dec 2019 07:51:09 GMT  
		Size: 244.6 KB (244564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e67aa2e5005496faabced9b401bd4fc0df82ce220f788a8b482d5e4573297b`  
		Last Modified: Sat, 28 Dec 2019 07:51:15 GMT  
		Size: 24.0 MB (24034502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.4-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:1f4934f1efe69c26a98185a2bc99e580a526aa735cc4da9844aff46be9a15fe5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49393724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc3943b43108c053d1ea7c38ad4ed1e150e4bdab803de5acf46dff74c87bfa76`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:50 GMT
ADD file:8e4d0a1e6805c641fc9d18ebad82e4b01d85c6cb9f87d1ef47d75d150212a392 in / 
# Fri, 22 Nov 2019 13:45:53 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 20:53:28 GMT
ENV MONO_VERSION=6.4.0.198
# Fri, 22 Nov 2019 20:53:48 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 22 Nov 2019 20:54:31 GMT
RUN echo "deb http://download.mono-project.com/repo/debian vs-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:98a64bf4db7d2219b4fdd8182188d9422810dee890e997095bfb564a0482eed6`  
		Last Modified: Fri, 22 Nov 2019 13:52:17 GMT  
		Size: 20.4 MB (20385759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a2743b1fbbbe91732990b09c66ef2caee87b5e2cc4a4c3b56fab159729df2f`  
		Last Modified: Fri, 22 Nov 2019 21:08:13 GMT  
		Size: 244.4 KB (244416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db34d520760acec2af59a6940f6b8c2d2af12071dcfc75a183d61e8ae2af23b2`  
		Last Modified: Fri, 22 Nov 2019 21:08:23 GMT  
		Size: 28.8 MB (28763549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.4-slim` - linux; 386

```console
$ docker pull mono@sha256:6b3298a6b8ce9aff69db1eddccb45ef69b667caefedcfb1880962f18abc0f2ec
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.3 MB (89344215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26dc5bc379839014faebab7da7370e7557adfc4c8d4f775698580a3206a6934e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 16:54:44 GMT
ADD file:19d04f738434c76e2dbd14b48de2f0f03afa883b15f638c6ecbbf382df03567c in / 
# Fri, 22 Nov 2019 16:54:44 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 01:07:21 GMT
ENV MONO_VERSION=6.4.0.198
# Sat, 23 Nov 2019 01:07:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 23 Nov 2019 01:08:08 GMT
RUN echo "deb http://download.mono-project.com/repo/debian vs-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f26c9a85c76e393c9f2313b30e82d09f933d2dd4883620de242c7d21f8812e91`  
		Last Modified: Fri, 22 Nov 2019 17:03:03 GMT  
		Size: 23.2 MB (23152070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d54843b46358cc679b7b9ed6ac3c98102566536014e6820854dba519e772b0c`  
		Last Modified: Sat, 23 Nov 2019 01:16:39 GMT  
		Size: 244.5 KB (244506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f96e801e3047c9e846bbae422970ab17d1e71a0c136e22ec473666ba1c84fb2`  
		Last Modified: Sat, 23 Nov 2019 01:16:58 GMT  
		Size: 65.9 MB (65947639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.4-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:e696b74e509b6aeef319821d8417a54ff5f6003098436984d1c99e3debae17de
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48168727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:162ad102e676c3e612d565f88ffaa89080fa7d9cf970059e8e7c34b5b5410d2f`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:21 GMT
ADD file:a1ee5955ff3ede8df9558f4bec0c7962d54c43374f857e1da7e2639ddf82a9f1 in / 
# Sat, 28 Dec 2019 04:23:24 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:02:35 GMT
ENV MONO_VERSION=6.4.0.198
# Sat, 28 Dec 2019 06:03:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 06:04:47 GMT
RUN echo "deb http://download.mono-project.com/repo/debian vs-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af52e7ef6e83efadeae17be91daa6ecf61b7dfb39709c29be9b24876e60c0e36`  
		Last Modified: Sat, 28 Dec 2019 04:33:19 GMT  
		Size: 22.8 MB (22800791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85fc9eb11582da6a0be73b7e1050501cffcf51b26db363a95a648082a6b08178`  
		Last Modified: Sat, 28 Dec 2019 06:22:31 GMT  
		Size: 244.6 KB (244593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b94466b100a0063e3f8901325084fae9a526a1601a842a3d15a58fe1086a174`  
		Last Modified: Sat, 28 Dec 2019 06:22:43 GMT  
		Size: 25.1 MB (25123343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.6`

```console
$ docker pull mono@sha256:f5ff533f0bafd79c6e7d6938294e6ea09c9743aada81db4a25edab25ab46cdcc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.6` - linux; amd64

```console
$ docker pull mono@sha256:36bbaae3165f4dbbe0c166c151e638fc5c48e638ceb8c6070636f1c01d061206
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.2 MB (233196810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0211b82d6aefd6ae2c5a588c2119889733c462fda32a0210e20ea91fd4956312`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:59:24 GMT
ADD file:2c1f5e08834f13ccb9c2326204eb2556e03239d00171e75755c7195289374c61 in / 
# Fri, 22 Nov 2019 14:59:25 GMT
CMD ["bash"]
# Tue, 10 Dec 2019 22:11:17 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 10 Dec 2019 22:11:31 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 10 Dec 2019 22:12:14 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 10 Dec 2019 22:23:55 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d599a449871ee73b960e80d176b989365dfecb4c8f337bf21e8853862403ee9b`  
		Last Modified: Fri, 22 Nov 2019 15:06:36 GMT  
		Size: 22.5 MB (22524572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d110a8d8d6a5fa5a2ed11b6480fdb8ddd3752cc065f9bb4601207fe6c2a5ccaa`  
		Last Modified: Tue, 10 Dec 2019 22:24:24 GMT  
		Size: 244.5 KB (244460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df5758d8b4d450d2162c07e6a21fcfd0720544194e831610eb80d1780f188bc`  
		Last Modified: Tue, 10 Dec 2019 22:24:39 GMT  
		Size: 63.0 MB (62973805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db3f1cd295be39d3d4a0ec3b1ef1190b9ac6a4c1cd9f4ee0769d0a6e0e6aa69`  
		Last Modified: Tue, 10 Dec 2019 22:25:22 GMT  
		Size: 147.5 MB (147453973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6` - linux; arm variant v5

```console
$ docker pull mono@sha256:71075f43a6acd5d4900e8b4050bc87b552302d7b550e2d9da1a55aa37eb95852
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.7 MB (176653531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41594e91a86b24e549ebe9f4c951e2403e6e22200d648d599d853dbc7ebe37a5`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:53:16 GMT
ADD file:7d6af454b55cb354e31c096e935358dd5914688ded04ebc76243a4ff598c4495 in / 
# Sat, 28 Dec 2019 04:53:18 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:28:31 GMT
ENV MONO_VERSION=6.6.0.161
# Sat, 28 Dec 2019 07:28:56 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:29:51 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 28 Dec 2019 07:37:00 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af28f499fd964f4506ea46c2ac342bc52328a8c30cd633661b69f383a5144e9b`  
		Last Modified: Sat, 28 Dec 2019 05:00:23 GMT  
		Size: 21.2 MB (21202822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f759ae685ca874cea702ae1f63627810d814a2cae6a44c704003176e0c8b37c`  
		Last Modified: Sat, 28 Dec 2019 07:44:23 GMT  
		Size: 244.6 KB (244552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:720fbe46ab0c5e8c2e3e9ed44413d9fde2ad1d45d9161dd0c6a021855acc1b78`  
		Last Modified: Sat, 28 Dec 2019 07:44:33 GMT  
		Size: 25.4 MB (25416500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906dd0e12894eb03a4ab34eacdf91d163dfd6c09d61c9005e666875d42c1b91b`  
		Last Modified: Sat, 28 Dec 2019 07:46:06 GMT  
		Size: 129.8 MB (129789657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6` - linux; arm variant v7

```console
$ docker pull mono@sha256:7e7ebdba687fb7bac2a796eb557210fe8f5fa55c86cfa342bd56d213a27dcaf3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.7 MB (172655347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c77176fb08c03220255179938d178739f8882569f72ecaae83ba7b5fc620aef`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 05:03:51 GMT
ADD file:2002ba672e32ae75369830ed6a4734ce62e0118e42390b4d657f0985d6b7fd6a in / 
# Sat, 28 Dec 2019 05:03:53 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:37:00 GMT
ENV MONO_VERSION=6.6.0.161
# Sat, 28 Dec 2019 07:37:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:38:02 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 28 Dec 2019 07:44:03 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:77cf262539006c8df77496f500f74a8c1edd158062440fd94d43d5b1292cefee`  
		Last Modified: Sat, 28 Dec 2019 05:11:13 GMT  
		Size: 19.3 MB (19311587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ea3a0398ee0834c6b8b5a98490a2451261135d85bbd06845c7077aff2a4667`  
		Last Modified: Sat, 28 Dec 2019 07:50:49 GMT  
		Size: 244.5 KB (244525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f543438b2494429fd7ef0a5cbe2145241dfa4aa2f1008038a251526056612dc`  
		Last Modified: Sat, 28 Dec 2019 07:50:58 GMT  
		Size: 24.6 MB (24648229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184b3a33ac95fb2ba207e6fc82f4e7fac1dc71bad49531f182c2a7046b54bd39`  
		Last Modified: Sat, 28 Dec 2019 07:52:21 GMT  
		Size: 128.5 MB (128451006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:9d331c132d88d02b360e8d415ca3ce11ac4b29fce0711e4bf57768bd608750d7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.5 MB (194538550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:185e12dba59e302b48ff069147dffe83d87755aee21ec6b8f56bc46ff2e325fa`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:50 GMT
ADD file:8e4d0a1e6805c641fc9d18ebad82e4b01d85c6cb9f87d1ef47d75d150212a392 in / 
# Fri, 22 Nov 2019 13:45:53 GMT
CMD ["bash"]
# Tue, 10 Dec 2019 22:32:06 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 10 Dec 2019 22:32:29 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 10 Dec 2019 22:33:16 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 10 Dec 2019 22:36:34 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:98a64bf4db7d2219b4fdd8182188d9422810dee890e997095bfb564a0482eed6`  
		Last Modified: Fri, 22 Nov 2019 13:52:17 GMT  
		Size: 20.4 MB (20385759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a200380ef45d7e798a6c00bf777add415c1dcd43827dfd4245e9a70a44551c16`  
		Last Modified: Tue, 10 Dec 2019 22:37:08 GMT  
		Size: 244.4 KB (244414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d827d45253e033764c27bafc3cf0f6f6a7c489c4cbfc72204de1e80d360e4ad`  
		Last Modified: Tue, 10 Dec 2019 22:37:19 GMT  
		Size: 29.4 MB (29433771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b857a6aa08dd2c3efd831641f352d721803f51db7005a61c8b24cd3bc8835076`  
		Last Modified: Tue, 10 Dec 2019 22:38:16 GMT  
		Size: 144.5 MB (144474606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6` - linux; 386

```console
$ docker pull mono@sha256:cb86414bf1a5dea08a730c594cd416e9811c28a017a19c1ef38413d28b7c43f1
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.4 MB (241440758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8236e6d4318ea3a6c3150c668ccd4b5ad0a54f9ec9b8b6ae6f5f9025d7c159c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 16:54:44 GMT
ADD file:19d04f738434c76e2dbd14b48de2f0f03afa883b15f638c6ecbbf382df03567c in / 
# Fri, 22 Nov 2019 16:54:44 GMT
CMD ["bash"]
# Tue, 10 Dec 2019 22:40:38 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 10 Dec 2019 22:40:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 10 Dec 2019 22:41:28 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 10 Dec 2019 22:44:08 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f26c9a85c76e393c9f2313b30e82d09f933d2dd4883620de242c7d21f8812e91`  
		Last Modified: Fri, 22 Nov 2019 17:03:03 GMT  
		Size: 23.2 MB (23152070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd443cfef677c492dd94fe413c0d2136b767456782251d33c6f1317711c7ebb`  
		Last Modified: Tue, 10 Dec 2019 22:44:33 GMT  
		Size: 244.5 KB (244499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd896b7ec3d7536139b522b4d9ce45dfd161f148c667dbc616035478ae145c7`  
		Last Modified: Tue, 10 Dec 2019 22:44:49 GMT  
		Size: 66.7 MB (66749782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f932dceff64bdede65b0f1e5a3443dc9749d88d7ad89b99977d0339b81891b5d`  
		Last Modified: Tue, 10 Dec 2019 22:45:37 GMT  
		Size: 151.3 MB (151294407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6` - linux; ppc64le

```console
$ docker pull mono@sha256:8be78d5e96a5e63f2d4754a3686943f1d8edfd75c46a313cd27984c010e27c52
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.9 MB (178943769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c75d8bc1699ea912f280f4dcb86edababad529239b8eeb28e3801bcd9a015066`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:21 GMT
ADD file:a1ee5955ff3ede8df9558f4bec0c7962d54c43374f857e1da7e2639ddf82a9f1 in / 
# Sat, 28 Dec 2019 04:23:24 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:00:10 GMT
ENV MONO_VERSION=6.6.0.161
# Sat, 28 Dec 2019 06:01:14 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 06:02:17 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 28 Dec 2019 06:11:01 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af52e7ef6e83efadeae17be91daa6ecf61b7dfb39709c29be9b24876e60c0e36`  
		Last Modified: Sat, 28 Dec 2019 04:33:19 GMT  
		Size: 22.8 MB (22800791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367bf0f7a48952d80f9489622c9b118004dd0fd4763a1fd6153d9b12a571b1ee`  
		Last Modified: Sat, 28 Dec 2019 06:22:04 GMT  
		Size: 244.5 KB (244543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf3902985b2f759ba0edff57a78d4eb7e81f59e8327b7d243b8f3b4b8ca7c79`  
		Last Modified: Sat, 28 Dec 2019 06:22:14 GMT  
		Size: 25.8 MB (25828829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b12c28397b6cede6691c7e5447b466791fb395f4ecb3d1fb78e68dc1ffe4eb9`  
		Last Modified: Sat, 28 Dec 2019 06:24:05 GMT  
		Size: 130.1 MB (130069606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.6.0`

```console
$ docker pull mono@sha256:f5ff533f0bafd79c6e7d6938294e6ea09c9743aada81db4a25edab25ab46cdcc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.6.0` - linux; amd64

```console
$ docker pull mono@sha256:36bbaae3165f4dbbe0c166c151e638fc5c48e638ceb8c6070636f1c01d061206
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.2 MB (233196810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0211b82d6aefd6ae2c5a588c2119889733c462fda32a0210e20ea91fd4956312`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:59:24 GMT
ADD file:2c1f5e08834f13ccb9c2326204eb2556e03239d00171e75755c7195289374c61 in / 
# Fri, 22 Nov 2019 14:59:25 GMT
CMD ["bash"]
# Tue, 10 Dec 2019 22:11:17 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 10 Dec 2019 22:11:31 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 10 Dec 2019 22:12:14 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 10 Dec 2019 22:23:55 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d599a449871ee73b960e80d176b989365dfecb4c8f337bf21e8853862403ee9b`  
		Last Modified: Fri, 22 Nov 2019 15:06:36 GMT  
		Size: 22.5 MB (22524572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d110a8d8d6a5fa5a2ed11b6480fdb8ddd3752cc065f9bb4601207fe6c2a5ccaa`  
		Last Modified: Tue, 10 Dec 2019 22:24:24 GMT  
		Size: 244.5 KB (244460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df5758d8b4d450d2162c07e6a21fcfd0720544194e831610eb80d1780f188bc`  
		Last Modified: Tue, 10 Dec 2019 22:24:39 GMT  
		Size: 63.0 MB (62973805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db3f1cd295be39d3d4a0ec3b1ef1190b9ac6a4c1cd9f4ee0769d0a6e0e6aa69`  
		Last Modified: Tue, 10 Dec 2019 22:25:22 GMT  
		Size: 147.5 MB (147453973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0` - linux; arm variant v5

```console
$ docker pull mono@sha256:71075f43a6acd5d4900e8b4050bc87b552302d7b550e2d9da1a55aa37eb95852
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.7 MB (176653531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41594e91a86b24e549ebe9f4c951e2403e6e22200d648d599d853dbc7ebe37a5`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:53:16 GMT
ADD file:7d6af454b55cb354e31c096e935358dd5914688ded04ebc76243a4ff598c4495 in / 
# Sat, 28 Dec 2019 04:53:18 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:28:31 GMT
ENV MONO_VERSION=6.6.0.161
# Sat, 28 Dec 2019 07:28:56 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:29:51 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 28 Dec 2019 07:37:00 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af28f499fd964f4506ea46c2ac342bc52328a8c30cd633661b69f383a5144e9b`  
		Last Modified: Sat, 28 Dec 2019 05:00:23 GMT  
		Size: 21.2 MB (21202822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f759ae685ca874cea702ae1f63627810d814a2cae6a44c704003176e0c8b37c`  
		Last Modified: Sat, 28 Dec 2019 07:44:23 GMT  
		Size: 244.6 KB (244552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:720fbe46ab0c5e8c2e3e9ed44413d9fde2ad1d45d9161dd0c6a021855acc1b78`  
		Last Modified: Sat, 28 Dec 2019 07:44:33 GMT  
		Size: 25.4 MB (25416500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906dd0e12894eb03a4ab34eacdf91d163dfd6c09d61c9005e666875d42c1b91b`  
		Last Modified: Sat, 28 Dec 2019 07:46:06 GMT  
		Size: 129.8 MB (129789657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0` - linux; arm variant v7

```console
$ docker pull mono@sha256:7e7ebdba687fb7bac2a796eb557210fe8f5fa55c86cfa342bd56d213a27dcaf3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.7 MB (172655347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c77176fb08c03220255179938d178739f8882569f72ecaae83ba7b5fc620aef`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 05:03:51 GMT
ADD file:2002ba672e32ae75369830ed6a4734ce62e0118e42390b4d657f0985d6b7fd6a in / 
# Sat, 28 Dec 2019 05:03:53 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:37:00 GMT
ENV MONO_VERSION=6.6.0.161
# Sat, 28 Dec 2019 07:37:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:38:02 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 28 Dec 2019 07:44:03 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:77cf262539006c8df77496f500f74a8c1edd158062440fd94d43d5b1292cefee`  
		Last Modified: Sat, 28 Dec 2019 05:11:13 GMT  
		Size: 19.3 MB (19311587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ea3a0398ee0834c6b8b5a98490a2451261135d85bbd06845c7077aff2a4667`  
		Last Modified: Sat, 28 Dec 2019 07:50:49 GMT  
		Size: 244.5 KB (244525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f543438b2494429fd7ef0a5cbe2145241dfa4aa2f1008038a251526056612dc`  
		Last Modified: Sat, 28 Dec 2019 07:50:58 GMT  
		Size: 24.6 MB (24648229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184b3a33ac95fb2ba207e6fc82f4e7fac1dc71bad49531f182c2a7046b54bd39`  
		Last Modified: Sat, 28 Dec 2019 07:52:21 GMT  
		Size: 128.5 MB (128451006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:9d331c132d88d02b360e8d415ca3ce11ac4b29fce0711e4bf57768bd608750d7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.5 MB (194538550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:185e12dba59e302b48ff069147dffe83d87755aee21ec6b8f56bc46ff2e325fa`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:50 GMT
ADD file:8e4d0a1e6805c641fc9d18ebad82e4b01d85c6cb9f87d1ef47d75d150212a392 in / 
# Fri, 22 Nov 2019 13:45:53 GMT
CMD ["bash"]
# Tue, 10 Dec 2019 22:32:06 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 10 Dec 2019 22:32:29 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 10 Dec 2019 22:33:16 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 10 Dec 2019 22:36:34 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:98a64bf4db7d2219b4fdd8182188d9422810dee890e997095bfb564a0482eed6`  
		Last Modified: Fri, 22 Nov 2019 13:52:17 GMT  
		Size: 20.4 MB (20385759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a200380ef45d7e798a6c00bf777add415c1dcd43827dfd4245e9a70a44551c16`  
		Last Modified: Tue, 10 Dec 2019 22:37:08 GMT  
		Size: 244.4 KB (244414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d827d45253e033764c27bafc3cf0f6f6a7c489c4cbfc72204de1e80d360e4ad`  
		Last Modified: Tue, 10 Dec 2019 22:37:19 GMT  
		Size: 29.4 MB (29433771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b857a6aa08dd2c3efd831641f352d721803f51db7005a61c8b24cd3bc8835076`  
		Last Modified: Tue, 10 Dec 2019 22:38:16 GMT  
		Size: 144.5 MB (144474606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0` - linux; 386

```console
$ docker pull mono@sha256:cb86414bf1a5dea08a730c594cd416e9811c28a017a19c1ef38413d28b7c43f1
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.4 MB (241440758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8236e6d4318ea3a6c3150c668ccd4b5ad0a54f9ec9b8b6ae6f5f9025d7c159c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 16:54:44 GMT
ADD file:19d04f738434c76e2dbd14b48de2f0f03afa883b15f638c6ecbbf382df03567c in / 
# Fri, 22 Nov 2019 16:54:44 GMT
CMD ["bash"]
# Tue, 10 Dec 2019 22:40:38 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 10 Dec 2019 22:40:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 10 Dec 2019 22:41:28 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 10 Dec 2019 22:44:08 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f26c9a85c76e393c9f2313b30e82d09f933d2dd4883620de242c7d21f8812e91`  
		Last Modified: Fri, 22 Nov 2019 17:03:03 GMT  
		Size: 23.2 MB (23152070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd443cfef677c492dd94fe413c0d2136b767456782251d33c6f1317711c7ebb`  
		Last Modified: Tue, 10 Dec 2019 22:44:33 GMT  
		Size: 244.5 KB (244499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd896b7ec3d7536139b522b4d9ce45dfd161f148c667dbc616035478ae145c7`  
		Last Modified: Tue, 10 Dec 2019 22:44:49 GMT  
		Size: 66.7 MB (66749782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f932dceff64bdede65b0f1e5a3443dc9749d88d7ad89b99977d0339b81891b5d`  
		Last Modified: Tue, 10 Dec 2019 22:45:37 GMT  
		Size: 151.3 MB (151294407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0` - linux; ppc64le

```console
$ docker pull mono@sha256:8be78d5e96a5e63f2d4754a3686943f1d8edfd75c46a313cd27984c010e27c52
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.9 MB (178943769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c75d8bc1699ea912f280f4dcb86edababad529239b8eeb28e3801bcd9a015066`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:21 GMT
ADD file:a1ee5955ff3ede8df9558f4bec0c7962d54c43374f857e1da7e2639ddf82a9f1 in / 
# Sat, 28 Dec 2019 04:23:24 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:00:10 GMT
ENV MONO_VERSION=6.6.0.161
# Sat, 28 Dec 2019 06:01:14 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 06:02:17 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 28 Dec 2019 06:11:01 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af52e7ef6e83efadeae17be91daa6ecf61b7dfb39709c29be9b24876e60c0e36`  
		Last Modified: Sat, 28 Dec 2019 04:33:19 GMT  
		Size: 22.8 MB (22800791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367bf0f7a48952d80f9489622c9b118004dd0fd4763a1fd6153d9b12a571b1ee`  
		Last Modified: Sat, 28 Dec 2019 06:22:04 GMT  
		Size: 244.5 KB (244543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf3902985b2f759ba0edff57a78d4eb7e81f59e8327b7d243b8f3b4b8ca7c79`  
		Last Modified: Sat, 28 Dec 2019 06:22:14 GMT  
		Size: 25.8 MB (25828829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b12c28397b6cede6691c7e5447b466791fb395f4ecb3d1fb78e68dc1ffe4eb9`  
		Last Modified: Sat, 28 Dec 2019 06:24:05 GMT  
		Size: 130.1 MB (130069606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.6.0.161`

```console
$ docker pull mono@sha256:f5ff533f0bafd79c6e7d6938294e6ea09c9743aada81db4a25edab25ab46cdcc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.6.0.161` - linux; amd64

```console
$ docker pull mono@sha256:36bbaae3165f4dbbe0c166c151e638fc5c48e638ceb8c6070636f1c01d061206
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.2 MB (233196810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0211b82d6aefd6ae2c5a588c2119889733c462fda32a0210e20ea91fd4956312`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:59:24 GMT
ADD file:2c1f5e08834f13ccb9c2326204eb2556e03239d00171e75755c7195289374c61 in / 
# Fri, 22 Nov 2019 14:59:25 GMT
CMD ["bash"]
# Tue, 10 Dec 2019 22:11:17 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 10 Dec 2019 22:11:31 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 10 Dec 2019 22:12:14 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 10 Dec 2019 22:23:55 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d599a449871ee73b960e80d176b989365dfecb4c8f337bf21e8853862403ee9b`  
		Last Modified: Fri, 22 Nov 2019 15:06:36 GMT  
		Size: 22.5 MB (22524572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d110a8d8d6a5fa5a2ed11b6480fdb8ddd3752cc065f9bb4601207fe6c2a5ccaa`  
		Last Modified: Tue, 10 Dec 2019 22:24:24 GMT  
		Size: 244.5 KB (244460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df5758d8b4d450d2162c07e6a21fcfd0720544194e831610eb80d1780f188bc`  
		Last Modified: Tue, 10 Dec 2019 22:24:39 GMT  
		Size: 63.0 MB (62973805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db3f1cd295be39d3d4a0ec3b1ef1190b9ac6a4c1cd9f4ee0769d0a6e0e6aa69`  
		Last Modified: Tue, 10 Dec 2019 22:25:22 GMT  
		Size: 147.5 MB (147453973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0.161` - linux; arm variant v5

```console
$ docker pull mono@sha256:71075f43a6acd5d4900e8b4050bc87b552302d7b550e2d9da1a55aa37eb95852
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.7 MB (176653531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41594e91a86b24e549ebe9f4c951e2403e6e22200d648d599d853dbc7ebe37a5`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:53:16 GMT
ADD file:7d6af454b55cb354e31c096e935358dd5914688ded04ebc76243a4ff598c4495 in / 
# Sat, 28 Dec 2019 04:53:18 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:28:31 GMT
ENV MONO_VERSION=6.6.0.161
# Sat, 28 Dec 2019 07:28:56 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:29:51 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 28 Dec 2019 07:37:00 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af28f499fd964f4506ea46c2ac342bc52328a8c30cd633661b69f383a5144e9b`  
		Last Modified: Sat, 28 Dec 2019 05:00:23 GMT  
		Size: 21.2 MB (21202822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f759ae685ca874cea702ae1f63627810d814a2cae6a44c704003176e0c8b37c`  
		Last Modified: Sat, 28 Dec 2019 07:44:23 GMT  
		Size: 244.6 KB (244552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:720fbe46ab0c5e8c2e3e9ed44413d9fde2ad1d45d9161dd0c6a021855acc1b78`  
		Last Modified: Sat, 28 Dec 2019 07:44:33 GMT  
		Size: 25.4 MB (25416500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906dd0e12894eb03a4ab34eacdf91d163dfd6c09d61c9005e666875d42c1b91b`  
		Last Modified: Sat, 28 Dec 2019 07:46:06 GMT  
		Size: 129.8 MB (129789657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0.161` - linux; arm variant v7

```console
$ docker pull mono@sha256:7e7ebdba687fb7bac2a796eb557210fe8f5fa55c86cfa342bd56d213a27dcaf3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.7 MB (172655347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c77176fb08c03220255179938d178739f8882569f72ecaae83ba7b5fc620aef`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 05:03:51 GMT
ADD file:2002ba672e32ae75369830ed6a4734ce62e0118e42390b4d657f0985d6b7fd6a in / 
# Sat, 28 Dec 2019 05:03:53 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:37:00 GMT
ENV MONO_VERSION=6.6.0.161
# Sat, 28 Dec 2019 07:37:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:38:02 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 28 Dec 2019 07:44:03 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:77cf262539006c8df77496f500f74a8c1edd158062440fd94d43d5b1292cefee`  
		Last Modified: Sat, 28 Dec 2019 05:11:13 GMT  
		Size: 19.3 MB (19311587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ea3a0398ee0834c6b8b5a98490a2451261135d85bbd06845c7077aff2a4667`  
		Last Modified: Sat, 28 Dec 2019 07:50:49 GMT  
		Size: 244.5 KB (244525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f543438b2494429fd7ef0a5cbe2145241dfa4aa2f1008038a251526056612dc`  
		Last Modified: Sat, 28 Dec 2019 07:50:58 GMT  
		Size: 24.6 MB (24648229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184b3a33ac95fb2ba207e6fc82f4e7fac1dc71bad49531f182c2a7046b54bd39`  
		Last Modified: Sat, 28 Dec 2019 07:52:21 GMT  
		Size: 128.5 MB (128451006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0.161` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:9d331c132d88d02b360e8d415ca3ce11ac4b29fce0711e4bf57768bd608750d7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.5 MB (194538550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:185e12dba59e302b48ff069147dffe83d87755aee21ec6b8f56bc46ff2e325fa`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:50 GMT
ADD file:8e4d0a1e6805c641fc9d18ebad82e4b01d85c6cb9f87d1ef47d75d150212a392 in / 
# Fri, 22 Nov 2019 13:45:53 GMT
CMD ["bash"]
# Tue, 10 Dec 2019 22:32:06 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 10 Dec 2019 22:32:29 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 10 Dec 2019 22:33:16 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 10 Dec 2019 22:36:34 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:98a64bf4db7d2219b4fdd8182188d9422810dee890e997095bfb564a0482eed6`  
		Last Modified: Fri, 22 Nov 2019 13:52:17 GMT  
		Size: 20.4 MB (20385759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a200380ef45d7e798a6c00bf777add415c1dcd43827dfd4245e9a70a44551c16`  
		Last Modified: Tue, 10 Dec 2019 22:37:08 GMT  
		Size: 244.4 KB (244414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d827d45253e033764c27bafc3cf0f6f6a7c489c4cbfc72204de1e80d360e4ad`  
		Last Modified: Tue, 10 Dec 2019 22:37:19 GMT  
		Size: 29.4 MB (29433771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b857a6aa08dd2c3efd831641f352d721803f51db7005a61c8b24cd3bc8835076`  
		Last Modified: Tue, 10 Dec 2019 22:38:16 GMT  
		Size: 144.5 MB (144474606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0.161` - linux; 386

```console
$ docker pull mono@sha256:cb86414bf1a5dea08a730c594cd416e9811c28a017a19c1ef38413d28b7c43f1
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.4 MB (241440758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8236e6d4318ea3a6c3150c668ccd4b5ad0a54f9ec9b8b6ae6f5f9025d7c159c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 16:54:44 GMT
ADD file:19d04f738434c76e2dbd14b48de2f0f03afa883b15f638c6ecbbf382df03567c in / 
# Fri, 22 Nov 2019 16:54:44 GMT
CMD ["bash"]
# Tue, 10 Dec 2019 22:40:38 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 10 Dec 2019 22:40:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 10 Dec 2019 22:41:28 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 10 Dec 2019 22:44:08 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f26c9a85c76e393c9f2313b30e82d09f933d2dd4883620de242c7d21f8812e91`  
		Last Modified: Fri, 22 Nov 2019 17:03:03 GMT  
		Size: 23.2 MB (23152070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd443cfef677c492dd94fe413c0d2136b767456782251d33c6f1317711c7ebb`  
		Last Modified: Tue, 10 Dec 2019 22:44:33 GMT  
		Size: 244.5 KB (244499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd896b7ec3d7536139b522b4d9ce45dfd161f148c667dbc616035478ae145c7`  
		Last Modified: Tue, 10 Dec 2019 22:44:49 GMT  
		Size: 66.7 MB (66749782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f932dceff64bdede65b0f1e5a3443dc9749d88d7ad89b99977d0339b81891b5d`  
		Last Modified: Tue, 10 Dec 2019 22:45:37 GMT  
		Size: 151.3 MB (151294407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0.161` - linux; ppc64le

```console
$ docker pull mono@sha256:8be78d5e96a5e63f2d4754a3686943f1d8edfd75c46a313cd27984c010e27c52
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.9 MB (178943769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c75d8bc1699ea912f280f4dcb86edababad529239b8eeb28e3801bcd9a015066`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:21 GMT
ADD file:a1ee5955ff3ede8df9558f4bec0c7962d54c43374f857e1da7e2639ddf82a9f1 in / 
# Sat, 28 Dec 2019 04:23:24 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:00:10 GMT
ENV MONO_VERSION=6.6.0.161
# Sat, 28 Dec 2019 06:01:14 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 06:02:17 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 28 Dec 2019 06:11:01 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af52e7ef6e83efadeae17be91daa6ecf61b7dfb39709c29be9b24876e60c0e36`  
		Last Modified: Sat, 28 Dec 2019 04:33:19 GMT  
		Size: 22.8 MB (22800791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367bf0f7a48952d80f9489622c9b118004dd0fd4763a1fd6153d9b12a571b1ee`  
		Last Modified: Sat, 28 Dec 2019 06:22:04 GMT  
		Size: 244.5 KB (244543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf3902985b2f759ba0edff57a78d4eb7e81f59e8327b7d243b8f3b4b8ca7c79`  
		Last Modified: Sat, 28 Dec 2019 06:22:14 GMT  
		Size: 25.8 MB (25828829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b12c28397b6cede6691c7e5447b466791fb395f4ecb3d1fb78e68dc1ffe4eb9`  
		Last Modified: Sat, 28 Dec 2019 06:24:05 GMT  
		Size: 130.1 MB (130069606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.6.0.161-slim`

```console
$ docker pull mono@sha256:e137fc49776b95ce1c44047ea9deaa69244ce56f0b833f9fda25e2b4af4ab49d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.6.0.161-slim` - linux; amd64

```console
$ docker pull mono@sha256:3fbc1438cf4ad5f9927ff4c8fd1bde9f827ac55f8065814f00fe4ef8e5b0ba40
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.7 MB (85742837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6194e440ff3046e473b21a8f2e394eb21ce932bec1df73a0dc7b98b2d06990e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:59:24 GMT
ADD file:2c1f5e08834f13ccb9c2326204eb2556e03239d00171e75755c7195289374c61 in / 
# Fri, 22 Nov 2019 14:59:25 GMT
CMD ["bash"]
# Tue, 10 Dec 2019 22:11:17 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 10 Dec 2019 22:11:31 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 10 Dec 2019 22:12:14 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d599a449871ee73b960e80d176b989365dfecb4c8f337bf21e8853862403ee9b`  
		Last Modified: Fri, 22 Nov 2019 15:06:36 GMT  
		Size: 22.5 MB (22524572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d110a8d8d6a5fa5a2ed11b6480fdb8ddd3752cc065f9bb4601207fe6c2a5ccaa`  
		Last Modified: Tue, 10 Dec 2019 22:24:24 GMT  
		Size: 244.5 KB (244460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df5758d8b4d450d2162c07e6a21fcfd0720544194e831610eb80d1780f188bc`  
		Last Modified: Tue, 10 Dec 2019 22:24:39 GMT  
		Size: 63.0 MB (62973805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0.161-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:263841647b1413f97ede49244a3250c2bd9224534cfda1f58a4cef015523f95e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46863874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f24cceab2b02f7699b97ad45390d24175d4f6cbc35951f14304e31bb40284717`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:53:16 GMT
ADD file:7d6af454b55cb354e31c096e935358dd5914688ded04ebc76243a4ff598c4495 in / 
# Sat, 28 Dec 2019 04:53:18 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:28:31 GMT
ENV MONO_VERSION=6.6.0.161
# Sat, 28 Dec 2019 07:28:56 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:29:51 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af28f499fd964f4506ea46c2ac342bc52328a8c30cd633661b69f383a5144e9b`  
		Last Modified: Sat, 28 Dec 2019 05:00:23 GMT  
		Size: 21.2 MB (21202822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f759ae685ca874cea702ae1f63627810d814a2cae6a44c704003176e0c8b37c`  
		Last Modified: Sat, 28 Dec 2019 07:44:23 GMT  
		Size: 244.6 KB (244552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:720fbe46ab0c5e8c2e3e9ed44413d9fde2ad1d45d9161dd0c6a021855acc1b78`  
		Last Modified: Sat, 28 Dec 2019 07:44:33 GMT  
		Size: 25.4 MB (25416500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0.161-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:70f8a6f90eedb2b040cdfe84d228b3b26f0549a32b275183a056543a822ebc44
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44204341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f0d6480804e64f949cbbdd9cc9ba45c6e077cd0266e5641b4822ce6ac3e6663`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 05:03:51 GMT
ADD file:2002ba672e32ae75369830ed6a4734ce62e0118e42390b4d657f0985d6b7fd6a in / 
# Sat, 28 Dec 2019 05:03:53 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:37:00 GMT
ENV MONO_VERSION=6.6.0.161
# Sat, 28 Dec 2019 07:37:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:38:02 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:77cf262539006c8df77496f500f74a8c1edd158062440fd94d43d5b1292cefee`  
		Last Modified: Sat, 28 Dec 2019 05:11:13 GMT  
		Size: 19.3 MB (19311587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ea3a0398ee0834c6b8b5a98490a2451261135d85bbd06845c7077aff2a4667`  
		Last Modified: Sat, 28 Dec 2019 07:50:49 GMT  
		Size: 244.5 KB (244525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f543438b2494429fd7ef0a5cbe2145241dfa4aa2f1008038a251526056612dc`  
		Last Modified: Sat, 28 Dec 2019 07:50:58 GMT  
		Size: 24.6 MB (24648229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0.161-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:c71f8c65cdbb3beccdfee0f7c89b9759cdd7559800c2d53820b2dc232ead5311
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50063944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c674cf5e286615ef8d8b03cbda9840dbfdfd5f9e5f8da1cc02ef19acda0215b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:50 GMT
ADD file:8e4d0a1e6805c641fc9d18ebad82e4b01d85c6cb9f87d1ef47d75d150212a392 in / 
# Fri, 22 Nov 2019 13:45:53 GMT
CMD ["bash"]
# Tue, 10 Dec 2019 22:32:06 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 10 Dec 2019 22:32:29 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 10 Dec 2019 22:33:16 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:98a64bf4db7d2219b4fdd8182188d9422810dee890e997095bfb564a0482eed6`  
		Last Modified: Fri, 22 Nov 2019 13:52:17 GMT  
		Size: 20.4 MB (20385759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a200380ef45d7e798a6c00bf777add415c1dcd43827dfd4245e9a70a44551c16`  
		Last Modified: Tue, 10 Dec 2019 22:37:08 GMT  
		Size: 244.4 KB (244414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d827d45253e033764c27bafc3cf0f6f6a7c489c4cbfc72204de1e80d360e4ad`  
		Last Modified: Tue, 10 Dec 2019 22:37:19 GMT  
		Size: 29.4 MB (29433771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0.161-slim` - linux; 386

```console
$ docker pull mono@sha256:20815f6f85d3625af3bab809cbd0189f28793864ae7eece04b7b0b16287d55f8
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.1 MB (90146351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51cf847eb7ced4d53e982f60c5343ba2adc72eb520774f12209b44d8ee8ddeaf`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 16:54:44 GMT
ADD file:19d04f738434c76e2dbd14b48de2f0f03afa883b15f638c6ecbbf382df03567c in / 
# Fri, 22 Nov 2019 16:54:44 GMT
CMD ["bash"]
# Tue, 10 Dec 2019 22:40:38 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 10 Dec 2019 22:40:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 10 Dec 2019 22:41:28 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f26c9a85c76e393c9f2313b30e82d09f933d2dd4883620de242c7d21f8812e91`  
		Last Modified: Fri, 22 Nov 2019 17:03:03 GMT  
		Size: 23.2 MB (23152070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd443cfef677c492dd94fe413c0d2136b767456782251d33c6f1317711c7ebb`  
		Last Modified: Tue, 10 Dec 2019 22:44:33 GMT  
		Size: 244.5 KB (244499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd896b7ec3d7536139b522b4d9ce45dfd161f148c667dbc616035478ae145c7`  
		Last Modified: Tue, 10 Dec 2019 22:44:49 GMT  
		Size: 66.7 MB (66749782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0.161-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:a7840aa6d9953b14f7d37472ed11dc4785cff7c5edbf16718bfc36a6d9cf58b6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48874163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ea84dffac95f8be085f5eeb79990afa1341135da9867d71688f2d9a3b61bfbf`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:21 GMT
ADD file:a1ee5955ff3ede8df9558f4bec0c7962d54c43374f857e1da7e2639ddf82a9f1 in / 
# Sat, 28 Dec 2019 04:23:24 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:00:10 GMT
ENV MONO_VERSION=6.6.0.161
# Sat, 28 Dec 2019 06:01:14 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 06:02:17 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af52e7ef6e83efadeae17be91daa6ecf61b7dfb39709c29be9b24876e60c0e36`  
		Last Modified: Sat, 28 Dec 2019 04:33:19 GMT  
		Size: 22.8 MB (22800791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367bf0f7a48952d80f9489622c9b118004dd0fd4763a1fd6153d9b12a571b1ee`  
		Last Modified: Sat, 28 Dec 2019 06:22:04 GMT  
		Size: 244.5 KB (244543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf3902985b2f759ba0edff57a78d4eb7e81f59e8327b7d243b8f3b4b8ca7c79`  
		Last Modified: Sat, 28 Dec 2019 06:22:14 GMT  
		Size: 25.8 MB (25828829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.6.0-slim`

```console
$ docker pull mono@sha256:e137fc49776b95ce1c44047ea9deaa69244ce56f0b833f9fda25e2b4af4ab49d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.6.0-slim` - linux; amd64

```console
$ docker pull mono@sha256:3fbc1438cf4ad5f9927ff4c8fd1bde9f827ac55f8065814f00fe4ef8e5b0ba40
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.7 MB (85742837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6194e440ff3046e473b21a8f2e394eb21ce932bec1df73a0dc7b98b2d06990e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:59:24 GMT
ADD file:2c1f5e08834f13ccb9c2326204eb2556e03239d00171e75755c7195289374c61 in / 
# Fri, 22 Nov 2019 14:59:25 GMT
CMD ["bash"]
# Tue, 10 Dec 2019 22:11:17 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 10 Dec 2019 22:11:31 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 10 Dec 2019 22:12:14 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d599a449871ee73b960e80d176b989365dfecb4c8f337bf21e8853862403ee9b`  
		Last Modified: Fri, 22 Nov 2019 15:06:36 GMT  
		Size: 22.5 MB (22524572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d110a8d8d6a5fa5a2ed11b6480fdb8ddd3752cc065f9bb4601207fe6c2a5ccaa`  
		Last Modified: Tue, 10 Dec 2019 22:24:24 GMT  
		Size: 244.5 KB (244460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df5758d8b4d450d2162c07e6a21fcfd0720544194e831610eb80d1780f188bc`  
		Last Modified: Tue, 10 Dec 2019 22:24:39 GMT  
		Size: 63.0 MB (62973805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:263841647b1413f97ede49244a3250c2bd9224534cfda1f58a4cef015523f95e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46863874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f24cceab2b02f7699b97ad45390d24175d4f6cbc35951f14304e31bb40284717`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:53:16 GMT
ADD file:7d6af454b55cb354e31c096e935358dd5914688ded04ebc76243a4ff598c4495 in / 
# Sat, 28 Dec 2019 04:53:18 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:28:31 GMT
ENV MONO_VERSION=6.6.0.161
# Sat, 28 Dec 2019 07:28:56 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:29:51 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af28f499fd964f4506ea46c2ac342bc52328a8c30cd633661b69f383a5144e9b`  
		Last Modified: Sat, 28 Dec 2019 05:00:23 GMT  
		Size: 21.2 MB (21202822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f759ae685ca874cea702ae1f63627810d814a2cae6a44c704003176e0c8b37c`  
		Last Modified: Sat, 28 Dec 2019 07:44:23 GMT  
		Size: 244.6 KB (244552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:720fbe46ab0c5e8c2e3e9ed44413d9fde2ad1d45d9161dd0c6a021855acc1b78`  
		Last Modified: Sat, 28 Dec 2019 07:44:33 GMT  
		Size: 25.4 MB (25416500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:70f8a6f90eedb2b040cdfe84d228b3b26f0549a32b275183a056543a822ebc44
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44204341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f0d6480804e64f949cbbdd9cc9ba45c6e077cd0266e5641b4822ce6ac3e6663`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 05:03:51 GMT
ADD file:2002ba672e32ae75369830ed6a4734ce62e0118e42390b4d657f0985d6b7fd6a in / 
# Sat, 28 Dec 2019 05:03:53 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:37:00 GMT
ENV MONO_VERSION=6.6.0.161
# Sat, 28 Dec 2019 07:37:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:38:02 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:77cf262539006c8df77496f500f74a8c1edd158062440fd94d43d5b1292cefee`  
		Last Modified: Sat, 28 Dec 2019 05:11:13 GMT  
		Size: 19.3 MB (19311587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ea3a0398ee0834c6b8b5a98490a2451261135d85bbd06845c7077aff2a4667`  
		Last Modified: Sat, 28 Dec 2019 07:50:49 GMT  
		Size: 244.5 KB (244525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f543438b2494429fd7ef0a5cbe2145241dfa4aa2f1008038a251526056612dc`  
		Last Modified: Sat, 28 Dec 2019 07:50:58 GMT  
		Size: 24.6 MB (24648229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:c71f8c65cdbb3beccdfee0f7c89b9759cdd7559800c2d53820b2dc232ead5311
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50063944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c674cf5e286615ef8d8b03cbda9840dbfdfd5f9e5f8da1cc02ef19acda0215b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:50 GMT
ADD file:8e4d0a1e6805c641fc9d18ebad82e4b01d85c6cb9f87d1ef47d75d150212a392 in / 
# Fri, 22 Nov 2019 13:45:53 GMT
CMD ["bash"]
# Tue, 10 Dec 2019 22:32:06 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 10 Dec 2019 22:32:29 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 10 Dec 2019 22:33:16 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:98a64bf4db7d2219b4fdd8182188d9422810dee890e997095bfb564a0482eed6`  
		Last Modified: Fri, 22 Nov 2019 13:52:17 GMT  
		Size: 20.4 MB (20385759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a200380ef45d7e798a6c00bf777add415c1dcd43827dfd4245e9a70a44551c16`  
		Last Modified: Tue, 10 Dec 2019 22:37:08 GMT  
		Size: 244.4 KB (244414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d827d45253e033764c27bafc3cf0f6f6a7c489c4cbfc72204de1e80d360e4ad`  
		Last Modified: Tue, 10 Dec 2019 22:37:19 GMT  
		Size: 29.4 MB (29433771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0-slim` - linux; 386

```console
$ docker pull mono@sha256:20815f6f85d3625af3bab809cbd0189f28793864ae7eece04b7b0b16287d55f8
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.1 MB (90146351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51cf847eb7ced4d53e982f60c5343ba2adc72eb520774f12209b44d8ee8ddeaf`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 16:54:44 GMT
ADD file:19d04f738434c76e2dbd14b48de2f0f03afa883b15f638c6ecbbf382df03567c in / 
# Fri, 22 Nov 2019 16:54:44 GMT
CMD ["bash"]
# Tue, 10 Dec 2019 22:40:38 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 10 Dec 2019 22:40:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 10 Dec 2019 22:41:28 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f26c9a85c76e393c9f2313b30e82d09f933d2dd4883620de242c7d21f8812e91`  
		Last Modified: Fri, 22 Nov 2019 17:03:03 GMT  
		Size: 23.2 MB (23152070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd443cfef677c492dd94fe413c0d2136b767456782251d33c6f1317711c7ebb`  
		Last Modified: Tue, 10 Dec 2019 22:44:33 GMT  
		Size: 244.5 KB (244499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd896b7ec3d7536139b522b4d9ce45dfd161f148c667dbc616035478ae145c7`  
		Last Modified: Tue, 10 Dec 2019 22:44:49 GMT  
		Size: 66.7 MB (66749782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:a7840aa6d9953b14f7d37472ed11dc4785cff7c5edbf16718bfc36a6d9cf58b6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48874163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ea84dffac95f8be085f5eeb79990afa1341135da9867d71688f2d9a3b61bfbf`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:21 GMT
ADD file:a1ee5955ff3ede8df9558f4bec0c7962d54c43374f857e1da7e2639ddf82a9f1 in / 
# Sat, 28 Dec 2019 04:23:24 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:00:10 GMT
ENV MONO_VERSION=6.6.0.161
# Sat, 28 Dec 2019 06:01:14 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 06:02:17 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af52e7ef6e83efadeae17be91daa6ecf61b7dfb39709c29be9b24876e60c0e36`  
		Last Modified: Sat, 28 Dec 2019 04:33:19 GMT  
		Size: 22.8 MB (22800791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367bf0f7a48952d80f9489622c9b118004dd0fd4763a1fd6153d9b12a571b1ee`  
		Last Modified: Sat, 28 Dec 2019 06:22:04 GMT  
		Size: 244.5 KB (244543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf3902985b2f759ba0edff57a78d4eb7e81f59e8327b7d243b8f3b4b8ca7c79`  
		Last Modified: Sat, 28 Dec 2019 06:22:14 GMT  
		Size: 25.8 MB (25828829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.6-slim`

```console
$ docker pull mono@sha256:e137fc49776b95ce1c44047ea9deaa69244ce56f0b833f9fda25e2b4af4ab49d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.6-slim` - linux; amd64

```console
$ docker pull mono@sha256:3fbc1438cf4ad5f9927ff4c8fd1bde9f827ac55f8065814f00fe4ef8e5b0ba40
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.7 MB (85742837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6194e440ff3046e473b21a8f2e394eb21ce932bec1df73a0dc7b98b2d06990e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:59:24 GMT
ADD file:2c1f5e08834f13ccb9c2326204eb2556e03239d00171e75755c7195289374c61 in / 
# Fri, 22 Nov 2019 14:59:25 GMT
CMD ["bash"]
# Tue, 10 Dec 2019 22:11:17 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 10 Dec 2019 22:11:31 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 10 Dec 2019 22:12:14 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d599a449871ee73b960e80d176b989365dfecb4c8f337bf21e8853862403ee9b`  
		Last Modified: Fri, 22 Nov 2019 15:06:36 GMT  
		Size: 22.5 MB (22524572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d110a8d8d6a5fa5a2ed11b6480fdb8ddd3752cc065f9bb4601207fe6c2a5ccaa`  
		Last Modified: Tue, 10 Dec 2019 22:24:24 GMT  
		Size: 244.5 KB (244460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df5758d8b4d450d2162c07e6a21fcfd0720544194e831610eb80d1780f188bc`  
		Last Modified: Tue, 10 Dec 2019 22:24:39 GMT  
		Size: 63.0 MB (62973805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:263841647b1413f97ede49244a3250c2bd9224534cfda1f58a4cef015523f95e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46863874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f24cceab2b02f7699b97ad45390d24175d4f6cbc35951f14304e31bb40284717`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:53:16 GMT
ADD file:7d6af454b55cb354e31c096e935358dd5914688ded04ebc76243a4ff598c4495 in / 
# Sat, 28 Dec 2019 04:53:18 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:28:31 GMT
ENV MONO_VERSION=6.6.0.161
# Sat, 28 Dec 2019 07:28:56 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:29:51 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af28f499fd964f4506ea46c2ac342bc52328a8c30cd633661b69f383a5144e9b`  
		Last Modified: Sat, 28 Dec 2019 05:00:23 GMT  
		Size: 21.2 MB (21202822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f759ae685ca874cea702ae1f63627810d814a2cae6a44c704003176e0c8b37c`  
		Last Modified: Sat, 28 Dec 2019 07:44:23 GMT  
		Size: 244.6 KB (244552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:720fbe46ab0c5e8c2e3e9ed44413d9fde2ad1d45d9161dd0c6a021855acc1b78`  
		Last Modified: Sat, 28 Dec 2019 07:44:33 GMT  
		Size: 25.4 MB (25416500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:70f8a6f90eedb2b040cdfe84d228b3b26f0549a32b275183a056543a822ebc44
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44204341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f0d6480804e64f949cbbdd9cc9ba45c6e077cd0266e5641b4822ce6ac3e6663`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 05:03:51 GMT
ADD file:2002ba672e32ae75369830ed6a4734ce62e0118e42390b4d657f0985d6b7fd6a in / 
# Sat, 28 Dec 2019 05:03:53 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:37:00 GMT
ENV MONO_VERSION=6.6.0.161
# Sat, 28 Dec 2019 07:37:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:38:02 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:77cf262539006c8df77496f500f74a8c1edd158062440fd94d43d5b1292cefee`  
		Last Modified: Sat, 28 Dec 2019 05:11:13 GMT  
		Size: 19.3 MB (19311587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ea3a0398ee0834c6b8b5a98490a2451261135d85bbd06845c7077aff2a4667`  
		Last Modified: Sat, 28 Dec 2019 07:50:49 GMT  
		Size: 244.5 KB (244525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f543438b2494429fd7ef0a5cbe2145241dfa4aa2f1008038a251526056612dc`  
		Last Modified: Sat, 28 Dec 2019 07:50:58 GMT  
		Size: 24.6 MB (24648229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:c71f8c65cdbb3beccdfee0f7c89b9759cdd7559800c2d53820b2dc232ead5311
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50063944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c674cf5e286615ef8d8b03cbda9840dbfdfd5f9e5f8da1cc02ef19acda0215b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:50 GMT
ADD file:8e4d0a1e6805c641fc9d18ebad82e4b01d85c6cb9f87d1ef47d75d150212a392 in / 
# Fri, 22 Nov 2019 13:45:53 GMT
CMD ["bash"]
# Tue, 10 Dec 2019 22:32:06 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 10 Dec 2019 22:32:29 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 10 Dec 2019 22:33:16 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:98a64bf4db7d2219b4fdd8182188d9422810dee890e997095bfb564a0482eed6`  
		Last Modified: Fri, 22 Nov 2019 13:52:17 GMT  
		Size: 20.4 MB (20385759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a200380ef45d7e798a6c00bf777add415c1dcd43827dfd4245e9a70a44551c16`  
		Last Modified: Tue, 10 Dec 2019 22:37:08 GMT  
		Size: 244.4 KB (244414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d827d45253e033764c27bafc3cf0f6f6a7c489c4cbfc72204de1e80d360e4ad`  
		Last Modified: Tue, 10 Dec 2019 22:37:19 GMT  
		Size: 29.4 MB (29433771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6-slim` - linux; 386

```console
$ docker pull mono@sha256:20815f6f85d3625af3bab809cbd0189f28793864ae7eece04b7b0b16287d55f8
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.1 MB (90146351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51cf847eb7ced4d53e982f60c5343ba2adc72eb520774f12209b44d8ee8ddeaf`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 16:54:44 GMT
ADD file:19d04f738434c76e2dbd14b48de2f0f03afa883b15f638c6ecbbf382df03567c in / 
# Fri, 22 Nov 2019 16:54:44 GMT
CMD ["bash"]
# Tue, 10 Dec 2019 22:40:38 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 10 Dec 2019 22:40:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 10 Dec 2019 22:41:28 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f26c9a85c76e393c9f2313b30e82d09f933d2dd4883620de242c7d21f8812e91`  
		Last Modified: Fri, 22 Nov 2019 17:03:03 GMT  
		Size: 23.2 MB (23152070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd443cfef677c492dd94fe413c0d2136b767456782251d33c6f1317711c7ebb`  
		Last Modified: Tue, 10 Dec 2019 22:44:33 GMT  
		Size: 244.5 KB (244499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd896b7ec3d7536139b522b4d9ce45dfd161f148c667dbc616035478ae145c7`  
		Last Modified: Tue, 10 Dec 2019 22:44:49 GMT  
		Size: 66.7 MB (66749782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:a7840aa6d9953b14f7d37472ed11dc4785cff7c5edbf16718bfc36a6d9cf58b6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48874163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ea84dffac95f8be085f5eeb79990afa1341135da9867d71688f2d9a3b61bfbf`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:21 GMT
ADD file:a1ee5955ff3ede8df9558f4bec0c7962d54c43374f857e1da7e2639ddf82a9f1 in / 
# Sat, 28 Dec 2019 04:23:24 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:00:10 GMT
ENV MONO_VERSION=6.6.0.161
# Sat, 28 Dec 2019 06:01:14 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 06:02:17 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af52e7ef6e83efadeae17be91daa6ecf61b7dfb39709c29be9b24876e60c0e36`  
		Last Modified: Sat, 28 Dec 2019 04:33:19 GMT  
		Size: 22.8 MB (22800791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367bf0f7a48952d80f9489622c9b118004dd0fd4763a1fd6153d9b12a571b1ee`  
		Last Modified: Sat, 28 Dec 2019 06:22:04 GMT  
		Size: 244.5 KB (244543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf3902985b2f759ba0edff57a78d4eb7e81f59e8327b7d243b8f3b4b8ca7c79`  
		Last Modified: Sat, 28 Dec 2019 06:22:14 GMT  
		Size: 25.8 MB (25828829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6-slim`

```console
$ docker pull mono@sha256:e137fc49776b95ce1c44047ea9deaa69244ce56f0b833f9fda25e2b4af4ab49d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6-slim` - linux; amd64

```console
$ docker pull mono@sha256:3fbc1438cf4ad5f9927ff4c8fd1bde9f827ac55f8065814f00fe4ef8e5b0ba40
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.7 MB (85742837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6194e440ff3046e473b21a8f2e394eb21ce932bec1df73a0dc7b98b2d06990e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:59:24 GMT
ADD file:2c1f5e08834f13ccb9c2326204eb2556e03239d00171e75755c7195289374c61 in / 
# Fri, 22 Nov 2019 14:59:25 GMT
CMD ["bash"]
# Tue, 10 Dec 2019 22:11:17 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 10 Dec 2019 22:11:31 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 10 Dec 2019 22:12:14 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d599a449871ee73b960e80d176b989365dfecb4c8f337bf21e8853862403ee9b`  
		Last Modified: Fri, 22 Nov 2019 15:06:36 GMT  
		Size: 22.5 MB (22524572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d110a8d8d6a5fa5a2ed11b6480fdb8ddd3752cc065f9bb4601207fe6c2a5ccaa`  
		Last Modified: Tue, 10 Dec 2019 22:24:24 GMT  
		Size: 244.5 KB (244460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df5758d8b4d450d2162c07e6a21fcfd0720544194e831610eb80d1780f188bc`  
		Last Modified: Tue, 10 Dec 2019 22:24:39 GMT  
		Size: 63.0 MB (62973805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:263841647b1413f97ede49244a3250c2bd9224534cfda1f58a4cef015523f95e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46863874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f24cceab2b02f7699b97ad45390d24175d4f6cbc35951f14304e31bb40284717`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:53:16 GMT
ADD file:7d6af454b55cb354e31c096e935358dd5914688ded04ebc76243a4ff598c4495 in / 
# Sat, 28 Dec 2019 04:53:18 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:28:31 GMT
ENV MONO_VERSION=6.6.0.161
# Sat, 28 Dec 2019 07:28:56 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:29:51 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af28f499fd964f4506ea46c2ac342bc52328a8c30cd633661b69f383a5144e9b`  
		Last Modified: Sat, 28 Dec 2019 05:00:23 GMT  
		Size: 21.2 MB (21202822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f759ae685ca874cea702ae1f63627810d814a2cae6a44c704003176e0c8b37c`  
		Last Modified: Sat, 28 Dec 2019 07:44:23 GMT  
		Size: 244.6 KB (244552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:720fbe46ab0c5e8c2e3e9ed44413d9fde2ad1d45d9161dd0c6a021855acc1b78`  
		Last Modified: Sat, 28 Dec 2019 07:44:33 GMT  
		Size: 25.4 MB (25416500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:70f8a6f90eedb2b040cdfe84d228b3b26f0549a32b275183a056543a822ebc44
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44204341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f0d6480804e64f949cbbdd9cc9ba45c6e077cd0266e5641b4822ce6ac3e6663`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 05:03:51 GMT
ADD file:2002ba672e32ae75369830ed6a4734ce62e0118e42390b4d657f0985d6b7fd6a in / 
# Sat, 28 Dec 2019 05:03:53 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:37:00 GMT
ENV MONO_VERSION=6.6.0.161
# Sat, 28 Dec 2019 07:37:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:38:02 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:77cf262539006c8df77496f500f74a8c1edd158062440fd94d43d5b1292cefee`  
		Last Modified: Sat, 28 Dec 2019 05:11:13 GMT  
		Size: 19.3 MB (19311587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ea3a0398ee0834c6b8b5a98490a2451261135d85bbd06845c7077aff2a4667`  
		Last Modified: Sat, 28 Dec 2019 07:50:49 GMT  
		Size: 244.5 KB (244525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f543438b2494429fd7ef0a5cbe2145241dfa4aa2f1008038a251526056612dc`  
		Last Modified: Sat, 28 Dec 2019 07:50:58 GMT  
		Size: 24.6 MB (24648229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:c71f8c65cdbb3beccdfee0f7c89b9759cdd7559800c2d53820b2dc232ead5311
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50063944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c674cf5e286615ef8d8b03cbda9840dbfdfd5f9e5f8da1cc02ef19acda0215b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:50 GMT
ADD file:8e4d0a1e6805c641fc9d18ebad82e4b01d85c6cb9f87d1ef47d75d150212a392 in / 
# Fri, 22 Nov 2019 13:45:53 GMT
CMD ["bash"]
# Tue, 10 Dec 2019 22:32:06 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 10 Dec 2019 22:32:29 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 10 Dec 2019 22:33:16 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:98a64bf4db7d2219b4fdd8182188d9422810dee890e997095bfb564a0482eed6`  
		Last Modified: Fri, 22 Nov 2019 13:52:17 GMT  
		Size: 20.4 MB (20385759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a200380ef45d7e798a6c00bf777add415c1dcd43827dfd4245e9a70a44551c16`  
		Last Modified: Tue, 10 Dec 2019 22:37:08 GMT  
		Size: 244.4 KB (244414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d827d45253e033764c27bafc3cf0f6f6a7c489c4cbfc72204de1e80d360e4ad`  
		Last Modified: Tue, 10 Dec 2019 22:37:19 GMT  
		Size: 29.4 MB (29433771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; 386

```console
$ docker pull mono@sha256:20815f6f85d3625af3bab809cbd0189f28793864ae7eece04b7b0b16287d55f8
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.1 MB (90146351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51cf847eb7ced4d53e982f60c5343ba2adc72eb520774f12209b44d8ee8ddeaf`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 16:54:44 GMT
ADD file:19d04f738434c76e2dbd14b48de2f0f03afa883b15f638c6ecbbf382df03567c in / 
# Fri, 22 Nov 2019 16:54:44 GMT
CMD ["bash"]
# Tue, 10 Dec 2019 22:40:38 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 10 Dec 2019 22:40:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 10 Dec 2019 22:41:28 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f26c9a85c76e393c9f2313b30e82d09f933d2dd4883620de242c7d21f8812e91`  
		Last Modified: Fri, 22 Nov 2019 17:03:03 GMT  
		Size: 23.2 MB (23152070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd443cfef677c492dd94fe413c0d2136b767456782251d33c6f1317711c7ebb`  
		Last Modified: Tue, 10 Dec 2019 22:44:33 GMT  
		Size: 244.5 KB (244499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd896b7ec3d7536139b522b4d9ce45dfd161f148c667dbc616035478ae145c7`  
		Last Modified: Tue, 10 Dec 2019 22:44:49 GMT  
		Size: 66.7 MB (66749782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:a7840aa6d9953b14f7d37472ed11dc4785cff7c5edbf16718bfc36a6d9cf58b6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48874163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ea84dffac95f8be085f5eeb79990afa1341135da9867d71688f2d9a3b61bfbf`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:21 GMT
ADD file:a1ee5955ff3ede8df9558f4bec0c7962d54c43374f857e1da7e2639ddf82a9f1 in / 
# Sat, 28 Dec 2019 04:23:24 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:00:10 GMT
ENV MONO_VERSION=6.6.0.161
# Sat, 28 Dec 2019 06:01:14 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 06:02:17 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af52e7ef6e83efadeae17be91daa6ecf61b7dfb39709c29be9b24876e60c0e36`  
		Last Modified: Sat, 28 Dec 2019 04:33:19 GMT  
		Size: 22.8 MB (22800791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367bf0f7a48952d80f9489622c9b118004dd0fd4763a1fd6153d9b12a571b1ee`  
		Last Modified: Sat, 28 Dec 2019 06:22:04 GMT  
		Size: 244.5 KB (244543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf3902985b2f759ba0edff57a78d4eb7e81f59e8327b7d243b8f3b4b8ca7c79`  
		Last Modified: Sat, 28 Dec 2019 06:22:14 GMT  
		Size: 25.8 MB (25828829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:latest`

```console
$ docker pull mono@sha256:f5ff533f0bafd79c6e7d6938294e6ea09c9743aada81db4a25edab25ab46cdcc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:latest` - linux; amd64

```console
$ docker pull mono@sha256:36bbaae3165f4dbbe0c166c151e638fc5c48e638ceb8c6070636f1c01d061206
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.2 MB (233196810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0211b82d6aefd6ae2c5a588c2119889733c462fda32a0210e20ea91fd4956312`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:59:24 GMT
ADD file:2c1f5e08834f13ccb9c2326204eb2556e03239d00171e75755c7195289374c61 in / 
# Fri, 22 Nov 2019 14:59:25 GMT
CMD ["bash"]
# Tue, 10 Dec 2019 22:11:17 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 10 Dec 2019 22:11:31 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 10 Dec 2019 22:12:14 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 10 Dec 2019 22:23:55 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d599a449871ee73b960e80d176b989365dfecb4c8f337bf21e8853862403ee9b`  
		Last Modified: Fri, 22 Nov 2019 15:06:36 GMT  
		Size: 22.5 MB (22524572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d110a8d8d6a5fa5a2ed11b6480fdb8ddd3752cc065f9bb4601207fe6c2a5ccaa`  
		Last Modified: Tue, 10 Dec 2019 22:24:24 GMT  
		Size: 244.5 KB (244460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df5758d8b4d450d2162c07e6a21fcfd0720544194e831610eb80d1780f188bc`  
		Last Modified: Tue, 10 Dec 2019 22:24:39 GMT  
		Size: 63.0 MB (62973805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db3f1cd295be39d3d4a0ec3b1ef1190b9ac6a4c1cd9f4ee0769d0a6e0e6aa69`  
		Last Modified: Tue, 10 Dec 2019 22:25:22 GMT  
		Size: 147.5 MB (147453973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm variant v5

```console
$ docker pull mono@sha256:71075f43a6acd5d4900e8b4050bc87b552302d7b550e2d9da1a55aa37eb95852
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.7 MB (176653531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41594e91a86b24e549ebe9f4c951e2403e6e22200d648d599d853dbc7ebe37a5`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:53:16 GMT
ADD file:7d6af454b55cb354e31c096e935358dd5914688ded04ebc76243a4ff598c4495 in / 
# Sat, 28 Dec 2019 04:53:18 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:28:31 GMT
ENV MONO_VERSION=6.6.0.161
# Sat, 28 Dec 2019 07:28:56 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:29:51 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 28 Dec 2019 07:37:00 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af28f499fd964f4506ea46c2ac342bc52328a8c30cd633661b69f383a5144e9b`  
		Last Modified: Sat, 28 Dec 2019 05:00:23 GMT  
		Size: 21.2 MB (21202822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f759ae685ca874cea702ae1f63627810d814a2cae6a44c704003176e0c8b37c`  
		Last Modified: Sat, 28 Dec 2019 07:44:23 GMT  
		Size: 244.6 KB (244552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:720fbe46ab0c5e8c2e3e9ed44413d9fde2ad1d45d9161dd0c6a021855acc1b78`  
		Last Modified: Sat, 28 Dec 2019 07:44:33 GMT  
		Size: 25.4 MB (25416500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906dd0e12894eb03a4ab34eacdf91d163dfd6c09d61c9005e666875d42c1b91b`  
		Last Modified: Sat, 28 Dec 2019 07:46:06 GMT  
		Size: 129.8 MB (129789657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm variant v7

```console
$ docker pull mono@sha256:7e7ebdba687fb7bac2a796eb557210fe8f5fa55c86cfa342bd56d213a27dcaf3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.7 MB (172655347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c77176fb08c03220255179938d178739f8882569f72ecaae83ba7b5fc620aef`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 05:03:51 GMT
ADD file:2002ba672e32ae75369830ed6a4734ce62e0118e42390b4d657f0985d6b7fd6a in / 
# Sat, 28 Dec 2019 05:03:53 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:37:00 GMT
ENV MONO_VERSION=6.6.0.161
# Sat, 28 Dec 2019 07:37:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:38:02 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 28 Dec 2019 07:44:03 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:77cf262539006c8df77496f500f74a8c1edd158062440fd94d43d5b1292cefee`  
		Last Modified: Sat, 28 Dec 2019 05:11:13 GMT  
		Size: 19.3 MB (19311587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ea3a0398ee0834c6b8b5a98490a2451261135d85bbd06845c7077aff2a4667`  
		Last Modified: Sat, 28 Dec 2019 07:50:49 GMT  
		Size: 244.5 KB (244525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f543438b2494429fd7ef0a5cbe2145241dfa4aa2f1008038a251526056612dc`  
		Last Modified: Sat, 28 Dec 2019 07:50:58 GMT  
		Size: 24.6 MB (24648229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184b3a33ac95fb2ba207e6fc82f4e7fac1dc71bad49531f182c2a7046b54bd39`  
		Last Modified: Sat, 28 Dec 2019 07:52:21 GMT  
		Size: 128.5 MB (128451006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:9d331c132d88d02b360e8d415ca3ce11ac4b29fce0711e4bf57768bd608750d7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.5 MB (194538550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:185e12dba59e302b48ff069147dffe83d87755aee21ec6b8f56bc46ff2e325fa`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:50 GMT
ADD file:8e4d0a1e6805c641fc9d18ebad82e4b01d85c6cb9f87d1ef47d75d150212a392 in / 
# Fri, 22 Nov 2019 13:45:53 GMT
CMD ["bash"]
# Tue, 10 Dec 2019 22:32:06 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 10 Dec 2019 22:32:29 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 10 Dec 2019 22:33:16 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 10 Dec 2019 22:36:34 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:98a64bf4db7d2219b4fdd8182188d9422810dee890e997095bfb564a0482eed6`  
		Last Modified: Fri, 22 Nov 2019 13:52:17 GMT  
		Size: 20.4 MB (20385759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a200380ef45d7e798a6c00bf777add415c1dcd43827dfd4245e9a70a44551c16`  
		Last Modified: Tue, 10 Dec 2019 22:37:08 GMT  
		Size: 244.4 KB (244414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d827d45253e033764c27bafc3cf0f6f6a7c489c4cbfc72204de1e80d360e4ad`  
		Last Modified: Tue, 10 Dec 2019 22:37:19 GMT  
		Size: 29.4 MB (29433771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b857a6aa08dd2c3efd831641f352d721803f51db7005a61c8b24cd3bc8835076`  
		Last Modified: Tue, 10 Dec 2019 22:38:16 GMT  
		Size: 144.5 MB (144474606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; 386

```console
$ docker pull mono@sha256:cb86414bf1a5dea08a730c594cd416e9811c28a017a19c1ef38413d28b7c43f1
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.4 MB (241440758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8236e6d4318ea3a6c3150c668ccd4b5ad0a54f9ec9b8b6ae6f5f9025d7c159c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 16:54:44 GMT
ADD file:19d04f738434c76e2dbd14b48de2f0f03afa883b15f638c6ecbbf382df03567c in / 
# Fri, 22 Nov 2019 16:54:44 GMT
CMD ["bash"]
# Tue, 10 Dec 2019 22:40:38 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 10 Dec 2019 22:40:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 10 Dec 2019 22:41:28 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 10 Dec 2019 22:44:08 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f26c9a85c76e393c9f2313b30e82d09f933d2dd4883620de242c7d21f8812e91`  
		Last Modified: Fri, 22 Nov 2019 17:03:03 GMT  
		Size: 23.2 MB (23152070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd443cfef677c492dd94fe413c0d2136b767456782251d33c6f1317711c7ebb`  
		Last Modified: Tue, 10 Dec 2019 22:44:33 GMT  
		Size: 244.5 KB (244499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd896b7ec3d7536139b522b4d9ce45dfd161f148c667dbc616035478ae145c7`  
		Last Modified: Tue, 10 Dec 2019 22:44:49 GMT  
		Size: 66.7 MB (66749782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f932dceff64bdede65b0f1e5a3443dc9749d88d7ad89b99977d0339b81891b5d`  
		Last Modified: Tue, 10 Dec 2019 22:45:37 GMT  
		Size: 151.3 MB (151294407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; ppc64le

```console
$ docker pull mono@sha256:8be78d5e96a5e63f2d4754a3686943f1d8edfd75c46a313cd27984c010e27c52
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.9 MB (178943769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c75d8bc1699ea912f280f4dcb86edababad529239b8eeb28e3801bcd9a015066`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:21 GMT
ADD file:a1ee5955ff3ede8df9558f4bec0c7962d54c43374f857e1da7e2639ddf82a9f1 in / 
# Sat, 28 Dec 2019 04:23:24 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:00:10 GMT
ENV MONO_VERSION=6.6.0.161
# Sat, 28 Dec 2019 06:01:14 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 06:02:17 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 28 Dec 2019 06:11:01 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af52e7ef6e83efadeae17be91daa6ecf61b7dfb39709c29be9b24876e60c0e36`  
		Last Modified: Sat, 28 Dec 2019 04:33:19 GMT  
		Size: 22.8 MB (22800791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367bf0f7a48952d80f9489622c9b118004dd0fd4763a1fd6153d9b12a571b1ee`  
		Last Modified: Sat, 28 Dec 2019 06:22:04 GMT  
		Size: 244.5 KB (244543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf3902985b2f759ba0edff57a78d4eb7e81f59e8327b7d243b8f3b4b8ca7c79`  
		Last Modified: Sat, 28 Dec 2019 06:22:14 GMT  
		Size: 25.8 MB (25828829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b12c28397b6cede6691c7e5447b466791fb395f4ecb3d1fb78e68dc1ffe4eb9`  
		Last Modified: Sat, 28 Dec 2019 06:24:05 GMT  
		Size: 130.1 MB (130069606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:slim`

```console
$ docker pull mono@sha256:e137fc49776b95ce1c44047ea9deaa69244ce56f0b833f9fda25e2b4af4ab49d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:slim` - linux; amd64

```console
$ docker pull mono@sha256:3fbc1438cf4ad5f9927ff4c8fd1bde9f827ac55f8065814f00fe4ef8e5b0ba40
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.7 MB (85742837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6194e440ff3046e473b21a8f2e394eb21ce932bec1df73a0dc7b98b2d06990e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:59:24 GMT
ADD file:2c1f5e08834f13ccb9c2326204eb2556e03239d00171e75755c7195289374c61 in / 
# Fri, 22 Nov 2019 14:59:25 GMT
CMD ["bash"]
# Tue, 10 Dec 2019 22:11:17 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 10 Dec 2019 22:11:31 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 10 Dec 2019 22:12:14 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d599a449871ee73b960e80d176b989365dfecb4c8f337bf21e8853862403ee9b`  
		Last Modified: Fri, 22 Nov 2019 15:06:36 GMT  
		Size: 22.5 MB (22524572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d110a8d8d6a5fa5a2ed11b6480fdb8ddd3752cc065f9bb4601207fe6c2a5ccaa`  
		Last Modified: Tue, 10 Dec 2019 22:24:24 GMT  
		Size: 244.5 KB (244460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df5758d8b4d450d2162c07e6a21fcfd0720544194e831610eb80d1780f188bc`  
		Last Modified: Tue, 10 Dec 2019 22:24:39 GMT  
		Size: 63.0 MB (62973805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:263841647b1413f97ede49244a3250c2bd9224534cfda1f58a4cef015523f95e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46863874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f24cceab2b02f7699b97ad45390d24175d4f6cbc35951f14304e31bb40284717`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:53:16 GMT
ADD file:7d6af454b55cb354e31c096e935358dd5914688ded04ebc76243a4ff598c4495 in / 
# Sat, 28 Dec 2019 04:53:18 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:28:31 GMT
ENV MONO_VERSION=6.6.0.161
# Sat, 28 Dec 2019 07:28:56 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:29:51 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af28f499fd964f4506ea46c2ac342bc52328a8c30cd633661b69f383a5144e9b`  
		Last Modified: Sat, 28 Dec 2019 05:00:23 GMT  
		Size: 21.2 MB (21202822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f759ae685ca874cea702ae1f63627810d814a2cae6a44c704003176e0c8b37c`  
		Last Modified: Sat, 28 Dec 2019 07:44:23 GMT  
		Size: 244.6 KB (244552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:720fbe46ab0c5e8c2e3e9ed44413d9fde2ad1d45d9161dd0c6a021855acc1b78`  
		Last Modified: Sat, 28 Dec 2019 07:44:33 GMT  
		Size: 25.4 MB (25416500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:70f8a6f90eedb2b040cdfe84d228b3b26f0549a32b275183a056543a822ebc44
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44204341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f0d6480804e64f949cbbdd9cc9ba45c6e077cd0266e5641b4822ce6ac3e6663`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 05:03:51 GMT
ADD file:2002ba672e32ae75369830ed6a4734ce62e0118e42390b4d657f0985d6b7fd6a in / 
# Sat, 28 Dec 2019 05:03:53 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:37:00 GMT
ENV MONO_VERSION=6.6.0.161
# Sat, 28 Dec 2019 07:37:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:38:02 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:77cf262539006c8df77496f500f74a8c1edd158062440fd94d43d5b1292cefee`  
		Last Modified: Sat, 28 Dec 2019 05:11:13 GMT  
		Size: 19.3 MB (19311587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ea3a0398ee0834c6b8b5a98490a2451261135d85bbd06845c7077aff2a4667`  
		Last Modified: Sat, 28 Dec 2019 07:50:49 GMT  
		Size: 244.5 KB (244525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f543438b2494429fd7ef0a5cbe2145241dfa4aa2f1008038a251526056612dc`  
		Last Modified: Sat, 28 Dec 2019 07:50:58 GMT  
		Size: 24.6 MB (24648229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:c71f8c65cdbb3beccdfee0f7c89b9759cdd7559800c2d53820b2dc232ead5311
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50063944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c674cf5e286615ef8d8b03cbda9840dbfdfd5f9e5f8da1cc02ef19acda0215b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:50 GMT
ADD file:8e4d0a1e6805c641fc9d18ebad82e4b01d85c6cb9f87d1ef47d75d150212a392 in / 
# Fri, 22 Nov 2019 13:45:53 GMT
CMD ["bash"]
# Tue, 10 Dec 2019 22:32:06 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 10 Dec 2019 22:32:29 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 10 Dec 2019 22:33:16 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:98a64bf4db7d2219b4fdd8182188d9422810dee890e997095bfb564a0482eed6`  
		Last Modified: Fri, 22 Nov 2019 13:52:17 GMT  
		Size: 20.4 MB (20385759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a200380ef45d7e798a6c00bf777add415c1dcd43827dfd4245e9a70a44551c16`  
		Last Modified: Tue, 10 Dec 2019 22:37:08 GMT  
		Size: 244.4 KB (244414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d827d45253e033764c27bafc3cf0f6f6a7c489c4cbfc72204de1e80d360e4ad`  
		Last Modified: Tue, 10 Dec 2019 22:37:19 GMT  
		Size: 29.4 MB (29433771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; 386

```console
$ docker pull mono@sha256:20815f6f85d3625af3bab809cbd0189f28793864ae7eece04b7b0b16287d55f8
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.1 MB (90146351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51cf847eb7ced4d53e982f60c5343ba2adc72eb520774f12209b44d8ee8ddeaf`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 16:54:44 GMT
ADD file:19d04f738434c76e2dbd14b48de2f0f03afa883b15f638c6ecbbf382df03567c in / 
# Fri, 22 Nov 2019 16:54:44 GMT
CMD ["bash"]
# Tue, 10 Dec 2019 22:40:38 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 10 Dec 2019 22:40:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 10 Dec 2019 22:41:28 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f26c9a85c76e393c9f2313b30e82d09f933d2dd4883620de242c7d21f8812e91`  
		Last Modified: Fri, 22 Nov 2019 17:03:03 GMT  
		Size: 23.2 MB (23152070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd443cfef677c492dd94fe413c0d2136b767456782251d33c6f1317711c7ebb`  
		Last Modified: Tue, 10 Dec 2019 22:44:33 GMT  
		Size: 244.5 KB (244499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd896b7ec3d7536139b522b4d9ce45dfd161f148c667dbc616035478ae145c7`  
		Last Modified: Tue, 10 Dec 2019 22:44:49 GMT  
		Size: 66.7 MB (66749782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; ppc64le

```console
$ docker pull mono@sha256:a7840aa6d9953b14f7d37472ed11dc4785cff7c5edbf16718bfc36a6d9cf58b6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48874163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ea84dffac95f8be085f5eeb79990afa1341135da9867d71688f2d9a3b61bfbf`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:21 GMT
ADD file:a1ee5955ff3ede8df9558f4bec0c7962d54c43374f857e1da7e2639ddf82a9f1 in / 
# Sat, 28 Dec 2019 04:23:24 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:00:10 GMT
ENV MONO_VERSION=6.6.0.161
# Sat, 28 Dec 2019 06:01:14 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 06:02:17 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af52e7ef6e83efadeae17be91daa6ecf61b7dfb39709c29be9b24876e60c0e36`  
		Last Modified: Sat, 28 Dec 2019 04:33:19 GMT  
		Size: 22.8 MB (22800791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367bf0f7a48952d80f9489622c9b118004dd0fd4763a1fd6153d9b12a571b1ee`  
		Last Modified: Sat, 28 Dec 2019 06:22:04 GMT  
		Size: 244.5 KB (244543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf3902985b2f759ba0edff57a78d4eb7e81f59e8327b7d243b8f3b4b8ca7c79`  
		Last Modified: Sat, 28 Dec 2019 06:22:14 GMT  
		Size: 25.8 MB (25828829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
