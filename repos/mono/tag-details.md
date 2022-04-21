<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mono`

-	[`mono:6`](#mono6)
-	[`mono:6-slim`](#mono6-slim)
-	[`mono:6.10`](#mono610)
-	[`mono:6.10-slim`](#mono610-slim)
-	[`mono:6.10.0`](#mono6100)
-	[`mono:6.10.0-slim`](#mono6100-slim)
-	[`mono:6.10.0.104`](#mono6100104)
-	[`mono:6.10.0.104-slim`](#mono6100104-slim)
-	[`mono:6.12`](#mono612)
-	[`mono:6.12-slim`](#mono612-slim)
-	[`mono:6.12.0`](#mono6120)
-	[`mono:6.12.0-slim`](#mono6120-slim)
-	[`mono:6.12.0.122`](#mono6120122)
-	[`mono:6.12.0.122-slim`](#mono6120122-slim)
-	[`mono:latest`](#monolatest)
-	[`mono:slim`](#monoslim)

## `mono:6`

```console
$ docker pull mono@sha256:8e6aa0dc91a317d6b4ada45be67e01948c3b620226538928a4374ccea987abbc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6` - linux; amd64

```console
$ docker pull mono@sha256:0c36486cbda2ab995af85a2e9bbe62cc56bd2cf77d030fb67c3c228c920d74cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.1 MB (236125631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a50ead981e57279bc2232fe42e0e534ddd348365a0df2aa9f7a6ea1043c1412e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:48 GMT
ADD file:011a43ee23214c201afb7f3b5be592f374b89a4c71aea82ca66146bbbc31b959 in / 
# Wed, 20 Apr 2022 04:43:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 15:27:27 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 15:27:35 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 15:27:54 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 20 Apr 2022 15:33:01 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4be315f6562fccf08fd6c749557e31e45ab6d987370e20e2c4933ddb04ddd5ff`  
		Last Modified: Wed, 20 Apr 2022 04:49:15 GMT  
		Size: 27.1 MB (27140664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20d9f7ad1a1561508daa15f30ed450e8279f8633fc277a84bd6f5b1d00ecf314`  
		Last Modified: Wed, 20 Apr 2022 15:39:01 GMT  
		Size: 2.8 MB (2777363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4214d10d224872d47c1c108360a2890678eff5f2e288cdefa4f0882ac8ff9e46`  
		Last Modified: Wed, 20 Apr 2022 15:39:10 GMT  
		Size: 64.8 MB (64759348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa0a929eb8545fe353e58ddc4af329eefbe9e50f63bbbf938d0256d77246e6a`  
		Last Modified: Wed, 20 Apr 2022 15:40:09 GMT  
		Size: 141.4 MB (141448256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; arm variant v5

```console
$ docker pull mono@sha256:258511710254d92fe26e82049f226a7e527f0ed49778129c70646e9fc329af2a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.0 MB (191957036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac351dfd94cc0f2249f8760f8fedebcc5a814cdd11a7bef18de24f24f52c37fa`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:17:47 GMT
ADD file:5b740716d202d2f3494df5e108c0ba999125920ed9c97803fe0ccdfeba5cf518 in / 
# Wed, 20 Apr 2022 07:17:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 13:45:59 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 13:46:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 13:47:13 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 20 Apr 2022 13:52:09 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1fc8704cfa531d4583c5d4d571b836a82c02a812dae88792c4397cf1c1770405`  
		Last Modified: Wed, 20 Apr 2022 07:33:54 GMT  
		Size: 24.9 MB (24889592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de67cfe4308dcefca53d406cca104b0f4db6a1d2dda37929256a8f8761e5550a`  
		Last Modified: Wed, 20 Apr 2022 13:56:57 GMT  
		Size: 2.5 MB (2467647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641f8380b2823093df874b2b79c65d2f31452f99f5896f56a17614cbcb1dc971`  
		Last Modified: Wed, 20 Apr 2022 13:57:13 GMT  
		Size: 24.5 MB (24492891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68839de10302780399729e3999eb88f5e1ed8ca5c135b146dbb11f63aa458dfa`  
		Last Modified: Wed, 20 Apr 2022 13:59:38 GMT  
		Size: 140.1 MB (140106906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; arm variant v7

```console
$ docker pull mono@sha256:ad3a93a04d11ffb9206df13b87aa8a10890bc78b826eef7fbbbb160387b29507
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.9 MB (187864260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c65447e8e52004d2ac80a42c301fd6f3eb5fe6898ca081f77decd51bed084fc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 13:28:26 GMT
ADD file:2a755b6e7bf01ec959b8bb848b6d46f292821a0bf08e04d565991ec4bdbea029 in / 
# Wed, 20 Apr 2022 13:28:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 22:05:17 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 22:05:41 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 22:06:24 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 20 Apr 2022 22:10:56 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:88467ac22b4358b1b60009f6332ba9e12b7a82a36bef334d91d68dbf8b58d96f`  
		Last Modified: Wed, 20 Apr 2022 13:45:04 GMT  
		Size: 22.7 MB (22747865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e27b3994c35244605adec982fe00db7376f48e5ec599c253a2465ef79124c80`  
		Last Modified: Wed, 20 Apr 2022 22:15:27 GMT  
		Size: 2.4 MB (2366878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8554905d57c581805a8fc875940e3e39baa10f0bbc841e4b1f192d1c968eafc2`  
		Last Modified: Wed, 20 Apr 2022 22:15:44 GMT  
		Size: 23.8 MB (23782556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b332d3b0da4d9e0bbb73a313bd1158fad6ed98c34ac243e90a2b37dcdac08e4`  
		Last Modified: Wed, 20 Apr 2022 22:18:18 GMT  
		Size: 139.0 MB (138966961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:617fd6f5ff9238ff8782c0b154f5fbb1e51864ad1f009da0d0c5fcd54ff179c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.5 MB (214465680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:721976153f55a700a3368032ce347eb3ae7b930fc6151b879332e0e99f1ca0cc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:36 GMT
ADD file:5de4397c1295f7249c93907be599d96efbd9cd25909340d245ec8d1c9770f444 in / 
# Wed, 20 Apr 2022 04:29:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 09:34:15 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 09:34:25 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 09:34:40 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 20 Apr 2022 09:36:17 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:6c3e5b218d6477ff77053280968d5bdeaa5dcf16a803e917d98dd0ea8b93ac82`  
		Last Modified: Wed, 20 Apr 2022 04:36:38 GMT  
		Size: 25.9 MB (25908349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5583d434a71d4775ae033dd3567325a5f5d01a34ff9f805631b17426570d60`  
		Last Modified: Wed, 20 Apr 2022 09:38:16 GMT  
		Size: 2.6 MB (2641065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1df7a4f3775402176b947b2ffb1f930879581b64904846f29bd8e5aa4000e4d`  
		Last Modified: Wed, 20 Apr 2022 09:38:20 GMT  
		Size: 29.3 MB (29318359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f80c1eac9d435a1e808ae3c8eaf8a76d9e653e54edc1090cf4c2fc47f29f6e`  
		Last Modified: Wed, 20 Apr 2022 09:39:21 GMT  
		Size: 156.6 MB (156597907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; 386

```console
$ docker pull mono@sha256:ef781f5c402c37c294ccf7397654b6a780c16c68ab05b1ee598260446e0049b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.7 MB (241696337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:faa267e26ab7e853336277f2575154ad396b6536c3cd9e8ba22824250ccc6fbd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:38:03 GMT
ADD file:602a25173054242f635a5a299845b7f1b56864ac5d3b8af1ae29dec3a9da119f in / 
# Wed, 20 Apr 2022 07:38:04 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:49:08 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 12:49:17 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 12:49:40 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 20 Apr 2022 12:51:19 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a13b13d818745c4d2234aab71df26e4a01bfe59f396ab62f20d156b94803650c`  
		Last Modified: Wed, 20 Apr 2022 07:45:46 GMT  
		Size: 27.8 MB (27799825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc07624832ff4b064bd2b3797a6774618e27f4c3a1e24419874628eeb613e7ba`  
		Last Modified: Wed, 20 Apr 2022 12:53:02 GMT  
		Size: 2.8 MB (2789161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d6af1a94baa95c219eaba2db2fb27e299572ac8d2859e1399838abdccae784c`  
		Last Modified: Wed, 20 Apr 2022 12:53:11 GMT  
		Size: 68.6 MB (68568946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec0646bfa3d97be6f7515ad03d0cbb859adebe6cf3785cf1d36d06c8aa3f224`  
		Last Modified: Wed, 20 Apr 2022 12:54:22 GMT  
		Size: 142.5 MB (142538405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; ppc64le

```console
$ docker pull mono@sha256:abb2d6df6d771036e5878f2d8d5f7be07336dc420c2f33f5cbcd387ff20e7215
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.6 MB (203607651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d706be5bbbd80d2cfe56b5ed3350e0a17769f9e9c5ce4ee417df1efdd40f9f5d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 09:47:47 GMT
ADD file:69078e7ae6d887f7e36ae048f98f784678fbd8b7a8ec27e3c2bce0d68a47236d in / 
# Wed, 20 Apr 2022 09:47:51 GMT
CMD ["bash"]
# Thu, 21 Apr 2022 08:14:20 GMT
ENV MONO_VERSION=6.12.0.122
# Thu, 21 Apr 2022 08:15:04 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 21 Apr 2022 08:16:01 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 21 Apr 2022 08:25:53 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1aacfa28cbcef999a852ce9c261b67f15f0ccd8450cd1dbfe7b0dc88e6b5aba2`  
		Last Modified: Wed, 20 Apr 2022 09:58:02 GMT  
		Size: 30.6 MB (30560296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b4fd6959397baa971e32512d4c0d1d094bea59e1bf9b3442d8a345c6f7cd81`  
		Last Modified: Thu, 21 Apr 2022 08:33:06 GMT  
		Size: 2.9 MB (2892563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff24986d59f2106922e32fbd04b151763111155f6440aa41d390cbab27fca8c8`  
		Last Modified: Thu, 21 Apr 2022 08:33:11 GMT  
		Size: 26.9 MB (26873691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c14de3289c90efbcb5ba56806674834ab22b34135aa29d559635cdfb7805907`  
		Last Modified: Thu, 21 Apr 2022 08:34:20 GMT  
		Size: 143.3 MB (143281101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6-slim`

```console
$ docker pull mono@sha256:df384bda4d7d65b1fc3842d0eaa6d5bb7d188c95f274e7cc8403b002c6ec8b82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6-slim` - linux; amd64

```console
$ docker pull mono@sha256:f0d95c21aa0a9490ae955fe78fc0f316616807db95b5790b5cd7b4391ac8568d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94677375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4291e2c603690115cbb2d33ea0dee4ab69b47aa89201a4fc53d449bd5c5e9d02`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:48 GMT
ADD file:011a43ee23214c201afb7f3b5be592f374b89a4c71aea82ca66146bbbc31b959 in / 
# Wed, 20 Apr 2022 04:43:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 15:27:27 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 15:27:35 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 15:27:54 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4be315f6562fccf08fd6c749557e31e45ab6d987370e20e2c4933ddb04ddd5ff`  
		Last Modified: Wed, 20 Apr 2022 04:49:15 GMT  
		Size: 27.1 MB (27140664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20d9f7ad1a1561508daa15f30ed450e8279f8633fc277a84bd6f5b1d00ecf314`  
		Last Modified: Wed, 20 Apr 2022 15:39:01 GMT  
		Size: 2.8 MB (2777363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4214d10d224872d47c1c108360a2890678eff5f2e288cdefa4f0882ac8ff9e46`  
		Last Modified: Wed, 20 Apr 2022 15:39:10 GMT  
		Size: 64.8 MB (64759348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:c3b087e497272a1ff39fc23bc98d4fe778bf411c3c00de946f43fe57cd6e9d50
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51850130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03bf635a6d765f56a65311bc43513ec14a0451754d992adcadcf3c7f67503ca8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:17:47 GMT
ADD file:5b740716d202d2f3494df5e108c0ba999125920ed9c97803fe0ccdfeba5cf518 in / 
# Wed, 20 Apr 2022 07:17:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 13:45:59 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 13:46:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 13:47:13 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1fc8704cfa531d4583c5d4d571b836a82c02a812dae88792c4397cf1c1770405`  
		Last Modified: Wed, 20 Apr 2022 07:33:54 GMT  
		Size: 24.9 MB (24889592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de67cfe4308dcefca53d406cca104b0f4db6a1d2dda37929256a8f8761e5550a`  
		Last Modified: Wed, 20 Apr 2022 13:56:57 GMT  
		Size: 2.5 MB (2467647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641f8380b2823093df874b2b79c65d2f31452f99f5896f56a17614cbcb1dc971`  
		Last Modified: Wed, 20 Apr 2022 13:57:13 GMT  
		Size: 24.5 MB (24492891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:faff62d5274b7437f4216c427da824165d03a1c90c7c0f79e08533937b868eee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48897299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:659c685d861a835af511fa1dc5758b62d34b1e713f3db36f2e4f3d1cc184057c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 13:28:26 GMT
ADD file:2a755b6e7bf01ec959b8bb848b6d46f292821a0bf08e04d565991ec4bdbea029 in / 
# Wed, 20 Apr 2022 13:28:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 22:05:17 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 22:05:41 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 22:06:24 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:88467ac22b4358b1b60009f6332ba9e12b7a82a36bef334d91d68dbf8b58d96f`  
		Last Modified: Wed, 20 Apr 2022 13:45:04 GMT  
		Size: 22.7 MB (22747865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e27b3994c35244605adec982fe00db7376f48e5ec599c253a2465ef79124c80`  
		Last Modified: Wed, 20 Apr 2022 22:15:27 GMT  
		Size: 2.4 MB (2366878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8554905d57c581805a8fc875940e3e39baa10f0bbc841e4b1f192d1c968eafc2`  
		Last Modified: Wed, 20 Apr 2022 22:15:44 GMT  
		Size: 23.8 MB (23782556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:0f3837c80f89d4cc61d33d11680310dd7b9170aa4a20287829db1cf4ff83169c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57867773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a03207fd5f3c9c31e878dec4d955581897e75177774ac4915f726360915f8e8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:36 GMT
ADD file:5de4397c1295f7249c93907be599d96efbd9cd25909340d245ec8d1c9770f444 in / 
# Wed, 20 Apr 2022 04:29:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 09:34:15 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 09:34:25 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 09:34:40 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:6c3e5b218d6477ff77053280968d5bdeaa5dcf16a803e917d98dd0ea8b93ac82`  
		Last Modified: Wed, 20 Apr 2022 04:36:38 GMT  
		Size: 25.9 MB (25908349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5583d434a71d4775ae033dd3567325a5f5d01a34ff9f805631b17426570d60`  
		Last Modified: Wed, 20 Apr 2022 09:38:16 GMT  
		Size: 2.6 MB (2641065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1df7a4f3775402176b947b2ffb1f930879581b64904846f29bd8e5aa4000e4d`  
		Last Modified: Wed, 20 Apr 2022 09:38:20 GMT  
		Size: 29.3 MB (29318359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; 386

```console
$ docker pull mono@sha256:a620c36d6b438c94797eaa6b17b2452369ac55ab8a59a1bcf8b4501df1eea0c5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99157932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95ff55aea4f3ffc1da74cea929a23a78ed6dc8901847098c5878018368c9da5d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:38:03 GMT
ADD file:602a25173054242f635a5a299845b7f1b56864ac5d3b8af1ae29dec3a9da119f in / 
# Wed, 20 Apr 2022 07:38:04 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:49:08 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 12:49:17 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 12:49:40 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a13b13d818745c4d2234aab71df26e4a01bfe59f396ab62f20d156b94803650c`  
		Last Modified: Wed, 20 Apr 2022 07:45:46 GMT  
		Size: 27.8 MB (27799825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc07624832ff4b064bd2b3797a6774618e27f4c3a1e24419874628eeb613e7ba`  
		Last Modified: Wed, 20 Apr 2022 12:53:02 GMT  
		Size: 2.8 MB (2789161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d6af1a94baa95c219eaba2db2fb27e299572ac8d2859e1399838abdccae784c`  
		Last Modified: Wed, 20 Apr 2022 12:53:11 GMT  
		Size: 68.6 MB (68568946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:13e28a240194ffdaa1ab1b8b10b807978db6ed7eec8e4d427b0ff2c6d38130b8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.3 MB (60326550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:806eebb6c6b16141507ab480ab6238efd982bbe9375a51cabbc00f5cd2fa62b5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 09:47:47 GMT
ADD file:69078e7ae6d887f7e36ae048f98f784678fbd8b7a8ec27e3c2bce0d68a47236d in / 
# Wed, 20 Apr 2022 09:47:51 GMT
CMD ["bash"]
# Thu, 21 Apr 2022 08:14:20 GMT
ENV MONO_VERSION=6.12.0.122
# Thu, 21 Apr 2022 08:15:04 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 21 Apr 2022 08:16:01 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1aacfa28cbcef999a852ce9c261b67f15f0ccd8450cd1dbfe7b0dc88e6b5aba2`  
		Last Modified: Wed, 20 Apr 2022 09:58:02 GMT  
		Size: 30.6 MB (30560296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b4fd6959397baa971e32512d4c0d1d094bea59e1bf9b3442d8a345c6f7cd81`  
		Last Modified: Thu, 21 Apr 2022 08:33:06 GMT  
		Size: 2.9 MB (2892563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff24986d59f2106922e32fbd04b151763111155f6440aa41d390cbab27fca8c8`  
		Last Modified: Thu, 21 Apr 2022 08:33:11 GMT  
		Size: 26.9 MB (26873691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10`

```console
$ docker pull mono@sha256:e41b67d54fb7d512ed0d1ff03444368d0bcbc6e181e6acd8595997d510f3b579
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.10` - linux; amd64

```console
$ docker pull mono@sha256:267540e87836271ff00bfad52c21dfc29f04f8686360a8c7790e959e4a5beab6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.0 MB (225005254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59e31c6453c88e8b1eadae06b24055a3c63c97bfd312dd97ca0d0d6aa3bc3358`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:48 GMT
ADD file:011a43ee23214c201afb7f3b5be592f374b89a4c71aea82ca66146bbbc31b959 in / 
# Wed, 20 Apr 2022 04:43:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 15:28:00 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 20 Apr 2022 15:28:08 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 15:28:35 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 20 Apr 2022 15:38:34 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4be315f6562fccf08fd6c749557e31e45ab6d987370e20e2c4933ddb04ddd5ff`  
		Last Modified: Wed, 20 Apr 2022 04:49:15 GMT  
		Size: 27.1 MB (27140664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c12dd5e44bf113633b7b789afce59d2c53cecb26c0693c47714e66ecd2b791b`  
		Last Modified: Wed, 20 Apr 2022 15:39:27 GMT  
		Size: 2.8 MB (2777352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf9809b5ba703db3a6b728b82e97ac17e874b7f3e1b617c6d07823e9aae072f1`  
		Last Modified: Wed, 20 Apr 2022 15:39:37 GMT  
		Size: 64.8 MB (64778853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6ff02d78da9ac75dffb18fad228a95dc17cbe7ec2e45e3c124576d1cf96730`  
		Last Modified: Wed, 20 Apr 2022 15:40:51 GMT  
		Size: 130.3 MB (130308385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; arm variant v5

```console
$ docker pull mono@sha256:c21ddc74f1ee678d26a4aba4428901c2889dc42c0737262ae205ec6dd5bb7c00
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.9 MB (180857223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d17c4501c297c80f49fd52b919d90e4d75484134cc71509d5ab04fdf40e596fb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:17:47 GMT
ADD file:5b740716d202d2f3494df5e108c0ba999125920ed9c97803fe0ccdfeba5cf518 in / 
# Wed, 20 Apr 2022 07:17:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 13:47:33 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 20 Apr 2022 13:48:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 13:48:48 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 20 Apr 2022 13:55:30 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1fc8704cfa531d4583c5d4d571b836a82c02a812dae88792c4397cf1c1770405`  
		Last Modified: Wed, 20 Apr 2022 07:33:54 GMT  
		Size: 24.9 MB (24889592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c5aa1543e8c9a4e82aa5c90d45e997347b2b2b85405e8d14879e0576d7df05a`  
		Last Modified: Wed, 20 Apr 2022 13:57:37 GMT  
		Size: 2.5 MB (2467655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:125bf149bad0edeae0dc7ad63977373207cea521e833db746a0098de085b98d6`  
		Last Modified: Wed, 20 Apr 2022 13:57:55 GMT  
		Size: 24.5 MB (24521761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6245f63551657140eed74fd21cdb79948901f1b69d7d7b036779d01667e2a59`  
		Last Modified: Wed, 20 Apr 2022 14:01:33 GMT  
		Size: 129.0 MB (128978215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; arm variant v7

```console
$ docker pull mono@sha256:2cec20e212eddef7773607ff9375f0c5d9a1096964b6af0350b0c0e1c206ba83
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.8 MB (176759115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8eda3475765acc4ffab5cc260d0a5aa6fdb589829a3e14001544cc19b9c9b929`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 13:28:26 GMT
ADD file:2a755b6e7bf01ec959b8bb848b6d46f292821a0bf08e04d565991ec4bdbea029 in / 
# Wed, 20 Apr 2022 13:28:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 22:06:40 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 20 Apr 2022 22:07:05 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 22:07:49 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 20 Apr 2022 22:14:04 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:88467ac22b4358b1b60009f6332ba9e12b7a82a36bef334d91d68dbf8b58d96f`  
		Last Modified: Wed, 20 Apr 2022 13:45:04 GMT  
		Size: 22.7 MB (22747865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d8152d34419455b6bf7d8c0f2724cffc7860178bd5f7d2b0977f1f3a88ba2b`  
		Last Modified: Wed, 20 Apr 2022 22:16:07 GMT  
		Size: 2.4 MB (2366963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030a0bfd9369a7ac4c283002f40b9eff5fe55a3f7dd2ab033754f096aae7b225`  
		Last Modified: Wed, 20 Apr 2022 22:16:24 GMT  
		Size: 23.8 MB (23814893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c213333d5cb65819a25c36d23181bfb12e6e88a9f44def07f0338f879e3726a`  
		Last Modified: Wed, 20 Apr 2022 22:20:05 GMT  
		Size: 127.8 MB (127829394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:db4ccba0ea3a15d03bce129dc7b8f8c1d17eb414d22d0ce50f04c91aa9dc8e6b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.4 MB (203357942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:542f1d2be1793e91d33d40c760fdeff6d2626a9c03e0bb060de4fc1929460c11`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:36 GMT
ADD file:5de4397c1295f7249c93907be599d96efbd9cd25909340d245ec8d1c9770f444 in / 
# Wed, 20 Apr 2022 04:29:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 09:34:48 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 20 Apr 2022 09:34:57 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 09:35:12 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 20 Apr 2022 09:37:30 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:6c3e5b218d6477ff77053280968d5bdeaa5dcf16a803e917d98dd0ea8b93ac82`  
		Last Modified: Wed, 20 Apr 2022 04:36:38 GMT  
		Size: 25.9 MB (25908349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df56c08b5590c539b81f96718f5057b07ceaaf7017a28704b0f095af7166af2f`  
		Last Modified: Wed, 20 Apr 2022 09:38:39 GMT  
		Size: 2.6 MB (2641023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34f53b7c9a1d5af7034cdc60069b6b9c3b2099c676574b0de7e22085ba360dc`  
		Last Modified: Wed, 20 Apr 2022 09:38:44 GMT  
		Size: 29.4 MB (29361704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3f7de6536f999251c110135ca6a52d08565af7071c6fe5eea96fbd6578aa58`  
		Last Modified: Wed, 20 Apr 2022 09:40:03 GMT  
		Size: 145.4 MB (145446866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; 386

```console
$ docker pull mono@sha256:3e640bbe614e2c612a0234a760239253353017f54ea632d8e70ca5007fc1129d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.6 MB (230599389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38c8b38fb0ee5f997e90812c188e9956c7ea18acf1131589a9e1d93bc640c80a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:38:03 GMT
ADD file:602a25173054242f635a5a299845b7f1b56864ac5d3b8af1ae29dec3a9da119f in / 
# Wed, 20 Apr 2022 07:38:04 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:49:46 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 20 Apr 2022 12:49:55 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 12:50:19 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 20 Apr 2022 12:52:21 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a13b13d818745c4d2234aab71df26e4a01bfe59f396ab62f20d156b94803650c`  
		Last Modified: Wed, 20 Apr 2022 07:45:46 GMT  
		Size: 27.8 MB (27799825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc19bd2071107b873877fbe3bf3e623d524ecd131b76d25f818ed40f8888a5ae`  
		Last Modified: Wed, 20 Apr 2022 12:53:33 GMT  
		Size: 2.8 MB (2789172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c731ec96f4a6bd8004ee92ad713c93444a1f646c970369e7c6d60ed2ffcf37b`  
		Last Modified: Wed, 20 Apr 2022 12:53:47 GMT  
		Size: 68.6 MB (68594373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af0ca9622588725474f2f5434ce305f02b1b9a597c878f49af99e99c444e22d`  
		Last Modified: Wed, 20 Apr 2022 12:55:04 GMT  
		Size: 131.4 MB (131416019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; ppc64le

```console
$ docker pull mono@sha256:4c88c0b5ac02dbaa91e5fe480820eb22fdc55f20bff0d7df9777d0a91922c678
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.4 MB (192387948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:387368637882df34976d77a30673f716abdd5419b3123ad8df120f22b5fcf888`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 09:47:47 GMT
ADD file:69078e7ae6d887f7e36ae048f98f784678fbd8b7a8ec27e3c2bce0d68a47236d in / 
# Wed, 20 Apr 2022 09:47:51 GMT
CMD ["bash"]
# Thu, 21 Apr 2022 08:16:13 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 21 Apr 2022 08:17:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 21 Apr 2022 08:18:20 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 21 Apr 2022 08:32:10 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1aacfa28cbcef999a852ce9c261b67f15f0ccd8450cd1dbfe7b0dc88e6b5aba2`  
		Last Modified: Wed, 20 Apr 2022 09:58:02 GMT  
		Size: 30.6 MB (30560296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de0a54d8df38d9e19040e4cc35d23ae39540f55b101c788d75b0f5bd7962f0a`  
		Last Modified: Thu, 21 Apr 2022 08:33:33 GMT  
		Size: 2.9 MB (2892565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1d68d6079e85f0ac3901f7af3c469922c3215d043be6e89e661e469915359b`  
		Last Modified: Thu, 21 Apr 2022 08:33:39 GMT  
		Size: 26.9 MB (26917630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d122d2862ed40219e98f737a6743b292bffac45b31c4f9fe88dc4d81365574e2`  
		Last Modified: Thu, 21 Apr 2022 08:35:08 GMT  
		Size: 132.0 MB (132017457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10-slim`

```console
$ docker pull mono@sha256:ff8040cc7d0ad003a0784be5d7217770d837595a8525e1fa6d3288fad7b3967d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.10-slim` - linux; amd64

```console
$ docker pull mono@sha256:b832b286c91b52d8ceb75e10c045dd0b8091eacc7dec1bf578cc93f787789094
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94696869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bac78024d85353c207f9dcab4346ac9427e1db31bba198d343bd15b9ed785115`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:48 GMT
ADD file:011a43ee23214c201afb7f3b5be592f374b89a4c71aea82ca66146bbbc31b959 in / 
# Wed, 20 Apr 2022 04:43:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 15:28:00 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 20 Apr 2022 15:28:08 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 15:28:35 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4be315f6562fccf08fd6c749557e31e45ab6d987370e20e2c4933ddb04ddd5ff`  
		Last Modified: Wed, 20 Apr 2022 04:49:15 GMT  
		Size: 27.1 MB (27140664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c12dd5e44bf113633b7b789afce59d2c53cecb26c0693c47714e66ecd2b791b`  
		Last Modified: Wed, 20 Apr 2022 15:39:27 GMT  
		Size: 2.8 MB (2777352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf9809b5ba703db3a6b728b82e97ac17e874b7f3e1b617c6d07823e9aae072f1`  
		Last Modified: Wed, 20 Apr 2022 15:39:37 GMT  
		Size: 64.8 MB (64778853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:c20dba7db17e25a0be339572fb3d52ce94d16cba9ac00d848d9c2521aa32516e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51879008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e82eef5d0fd90db316ae1e2eaede51fe23e748b0d05b2e224f14dbc82477f22`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:17:47 GMT
ADD file:5b740716d202d2f3494df5e108c0ba999125920ed9c97803fe0ccdfeba5cf518 in / 
# Wed, 20 Apr 2022 07:17:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 13:47:33 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 20 Apr 2022 13:48:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 13:48:48 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1fc8704cfa531d4583c5d4d571b836a82c02a812dae88792c4397cf1c1770405`  
		Last Modified: Wed, 20 Apr 2022 07:33:54 GMT  
		Size: 24.9 MB (24889592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c5aa1543e8c9a4e82aa5c90d45e997347b2b2b85405e8d14879e0576d7df05a`  
		Last Modified: Wed, 20 Apr 2022 13:57:37 GMT  
		Size: 2.5 MB (2467655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:125bf149bad0edeae0dc7ad63977373207cea521e833db746a0098de085b98d6`  
		Last Modified: Wed, 20 Apr 2022 13:57:55 GMT  
		Size: 24.5 MB (24521761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:6beca2f9eb9de605de516a5f5c87895701d1992d3d23b49d3093e9ee30fb527f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48929721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b85dce8f495fd90df563aba07128ceab1ede7236275f6dc501a20977712f0b1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 13:28:26 GMT
ADD file:2a755b6e7bf01ec959b8bb848b6d46f292821a0bf08e04d565991ec4bdbea029 in / 
# Wed, 20 Apr 2022 13:28:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 22:06:40 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 20 Apr 2022 22:07:05 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 22:07:49 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:88467ac22b4358b1b60009f6332ba9e12b7a82a36bef334d91d68dbf8b58d96f`  
		Last Modified: Wed, 20 Apr 2022 13:45:04 GMT  
		Size: 22.7 MB (22747865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d8152d34419455b6bf7d8c0f2724cffc7860178bd5f7d2b0977f1f3a88ba2b`  
		Last Modified: Wed, 20 Apr 2022 22:16:07 GMT  
		Size: 2.4 MB (2366963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030a0bfd9369a7ac4c283002f40b9eff5fe55a3f7dd2ab033754f096aae7b225`  
		Last Modified: Wed, 20 Apr 2022 22:16:24 GMT  
		Size: 23.8 MB (23814893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:fd0ffe089ab133d58978ea5e51d43135e9a8c87b86be3997fd1e5b0d581cc2ee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57911076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:147cc7fd6295707399eab462793e12cbddb6d439837b2897b3c69b2125dbc6e2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:36 GMT
ADD file:5de4397c1295f7249c93907be599d96efbd9cd25909340d245ec8d1c9770f444 in / 
# Wed, 20 Apr 2022 04:29:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 09:34:48 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 20 Apr 2022 09:34:57 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 09:35:12 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:6c3e5b218d6477ff77053280968d5bdeaa5dcf16a803e917d98dd0ea8b93ac82`  
		Last Modified: Wed, 20 Apr 2022 04:36:38 GMT  
		Size: 25.9 MB (25908349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df56c08b5590c539b81f96718f5057b07ceaaf7017a28704b0f095af7166af2f`  
		Last Modified: Wed, 20 Apr 2022 09:38:39 GMT  
		Size: 2.6 MB (2641023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34f53b7c9a1d5af7034cdc60069b6b9c3b2099c676574b0de7e22085ba360dc`  
		Last Modified: Wed, 20 Apr 2022 09:38:44 GMT  
		Size: 29.4 MB (29361704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; 386

```console
$ docker pull mono@sha256:8a2f06c25415df8cc6ae7315e81ca06a9ff079a357c05caf0d1b57045ad265fa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99183370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a4588d79da86f7cab111b6c2fc82a13c1680b1134d953242a251f3c0da28b4a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:38:03 GMT
ADD file:602a25173054242f635a5a299845b7f1b56864ac5d3b8af1ae29dec3a9da119f in / 
# Wed, 20 Apr 2022 07:38:04 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:49:46 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 20 Apr 2022 12:49:55 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 12:50:19 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a13b13d818745c4d2234aab71df26e4a01bfe59f396ab62f20d156b94803650c`  
		Last Modified: Wed, 20 Apr 2022 07:45:46 GMT  
		Size: 27.8 MB (27799825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc19bd2071107b873877fbe3bf3e623d524ecd131b76d25f818ed40f8888a5ae`  
		Last Modified: Wed, 20 Apr 2022 12:53:33 GMT  
		Size: 2.8 MB (2789172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c731ec96f4a6bd8004ee92ad713c93444a1f646c970369e7c6d60ed2ffcf37b`  
		Last Modified: Wed, 20 Apr 2022 12:53:47 GMT  
		Size: 68.6 MB (68594373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:6203bc52c8d103d8b3443f587b445dc6560c72ccb9e3be3e8c362cdcaafce09e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.4 MB (60370491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e04bf5f65354fea4785a3e0189d9f0898c08bcad2e4f9aef81b0aeac97243bac`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 09:47:47 GMT
ADD file:69078e7ae6d887f7e36ae048f98f784678fbd8b7a8ec27e3c2bce0d68a47236d in / 
# Wed, 20 Apr 2022 09:47:51 GMT
CMD ["bash"]
# Thu, 21 Apr 2022 08:16:13 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 21 Apr 2022 08:17:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 21 Apr 2022 08:18:20 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1aacfa28cbcef999a852ce9c261b67f15f0ccd8450cd1dbfe7b0dc88e6b5aba2`  
		Last Modified: Wed, 20 Apr 2022 09:58:02 GMT  
		Size: 30.6 MB (30560296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de0a54d8df38d9e19040e4cc35d23ae39540f55b101c788d75b0f5bd7962f0a`  
		Last Modified: Thu, 21 Apr 2022 08:33:33 GMT  
		Size: 2.9 MB (2892565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1d68d6079e85f0ac3901f7af3c469922c3215d043be6e89e661e469915359b`  
		Last Modified: Thu, 21 Apr 2022 08:33:39 GMT  
		Size: 26.9 MB (26917630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10.0`

```console
$ docker pull mono@sha256:e41b67d54fb7d512ed0d1ff03444368d0bcbc6e181e6acd8595997d510f3b579
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.10.0` - linux; amd64

```console
$ docker pull mono@sha256:267540e87836271ff00bfad52c21dfc29f04f8686360a8c7790e959e4a5beab6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.0 MB (225005254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59e31c6453c88e8b1eadae06b24055a3c63c97bfd312dd97ca0d0d6aa3bc3358`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:48 GMT
ADD file:011a43ee23214c201afb7f3b5be592f374b89a4c71aea82ca66146bbbc31b959 in / 
# Wed, 20 Apr 2022 04:43:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 15:28:00 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 20 Apr 2022 15:28:08 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 15:28:35 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 20 Apr 2022 15:38:34 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4be315f6562fccf08fd6c749557e31e45ab6d987370e20e2c4933ddb04ddd5ff`  
		Last Modified: Wed, 20 Apr 2022 04:49:15 GMT  
		Size: 27.1 MB (27140664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c12dd5e44bf113633b7b789afce59d2c53cecb26c0693c47714e66ecd2b791b`  
		Last Modified: Wed, 20 Apr 2022 15:39:27 GMT  
		Size: 2.8 MB (2777352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf9809b5ba703db3a6b728b82e97ac17e874b7f3e1b617c6d07823e9aae072f1`  
		Last Modified: Wed, 20 Apr 2022 15:39:37 GMT  
		Size: 64.8 MB (64778853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6ff02d78da9ac75dffb18fad228a95dc17cbe7ec2e45e3c124576d1cf96730`  
		Last Modified: Wed, 20 Apr 2022 15:40:51 GMT  
		Size: 130.3 MB (130308385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; arm variant v5

```console
$ docker pull mono@sha256:c21ddc74f1ee678d26a4aba4428901c2889dc42c0737262ae205ec6dd5bb7c00
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.9 MB (180857223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d17c4501c297c80f49fd52b919d90e4d75484134cc71509d5ab04fdf40e596fb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:17:47 GMT
ADD file:5b740716d202d2f3494df5e108c0ba999125920ed9c97803fe0ccdfeba5cf518 in / 
# Wed, 20 Apr 2022 07:17:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 13:47:33 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 20 Apr 2022 13:48:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 13:48:48 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 20 Apr 2022 13:55:30 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1fc8704cfa531d4583c5d4d571b836a82c02a812dae88792c4397cf1c1770405`  
		Last Modified: Wed, 20 Apr 2022 07:33:54 GMT  
		Size: 24.9 MB (24889592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c5aa1543e8c9a4e82aa5c90d45e997347b2b2b85405e8d14879e0576d7df05a`  
		Last Modified: Wed, 20 Apr 2022 13:57:37 GMT  
		Size: 2.5 MB (2467655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:125bf149bad0edeae0dc7ad63977373207cea521e833db746a0098de085b98d6`  
		Last Modified: Wed, 20 Apr 2022 13:57:55 GMT  
		Size: 24.5 MB (24521761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6245f63551657140eed74fd21cdb79948901f1b69d7d7b036779d01667e2a59`  
		Last Modified: Wed, 20 Apr 2022 14:01:33 GMT  
		Size: 129.0 MB (128978215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; arm variant v7

```console
$ docker pull mono@sha256:2cec20e212eddef7773607ff9375f0c5d9a1096964b6af0350b0c0e1c206ba83
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.8 MB (176759115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8eda3475765acc4ffab5cc260d0a5aa6fdb589829a3e14001544cc19b9c9b929`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 13:28:26 GMT
ADD file:2a755b6e7bf01ec959b8bb848b6d46f292821a0bf08e04d565991ec4bdbea029 in / 
# Wed, 20 Apr 2022 13:28:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 22:06:40 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 20 Apr 2022 22:07:05 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 22:07:49 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 20 Apr 2022 22:14:04 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:88467ac22b4358b1b60009f6332ba9e12b7a82a36bef334d91d68dbf8b58d96f`  
		Last Modified: Wed, 20 Apr 2022 13:45:04 GMT  
		Size: 22.7 MB (22747865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d8152d34419455b6bf7d8c0f2724cffc7860178bd5f7d2b0977f1f3a88ba2b`  
		Last Modified: Wed, 20 Apr 2022 22:16:07 GMT  
		Size: 2.4 MB (2366963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030a0bfd9369a7ac4c283002f40b9eff5fe55a3f7dd2ab033754f096aae7b225`  
		Last Modified: Wed, 20 Apr 2022 22:16:24 GMT  
		Size: 23.8 MB (23814893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c213333d5cb65819a25c36d23181bfb12e6e88a9f44def07f0338f879e3726a`  
		Last Modified: Wed, 20 Apr 2022 22:20:05 GMT  
		Size: 127.8 MB (127829394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:db4ccba0ea3a15d03bce129dc7b8f8c1d17eb414d22d0ce50f04c91aa9dc8e6b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.4 MB (203357942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:542f1d2be1793e91d33d40c760fdeff6d2626a9c03e0bb060de4fc1929460c11`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:36 GMT
ADD file:5de4397c1295f7249c93907be599d96efbd9cd25909340d245ec8d1c9770f444 in / 
# Wed, 20 Apr 2022 04:29:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 09:34:48 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 20 Apr 2022 09:34:57 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 09:35:12 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 20 Apr 2022 09:37:30 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:6c3e5b218d6477ff77053280968d5bdeaa5dcf16a803e917d98dd0ea8b93ac82`  
		Last Modified: Wed, 20 Apr 2022 04:36:38 GMT  
		Size: 25.9 MB (25908349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df56c08b5590c539b81f96718f5057b07ceaaf7017a28704b0f095af7166af2f`  
		Last Modified: Wed, 20 Apr 2022 09:38:39 GMT  
		Size: 2.6 MB (2641023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34f53b7c9a1d5af7034cdc60069b6b9c3b2099c676574b0de7e22085ba360dc`  
		Last Modified: Wed, 20 Apr 2022 09:38:44 GMT  
		Size: 29.4 MB (29361704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3f7de6536f999251c110135ca6a52d08565af7071c6fe5eea96fbd6578aa58`  
		Last Modified: Wed, 20 Apr 2022 09:40:03 GMT  
		Size: 145.4 MB (145446866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; 386

```console
$ docker pull mono@sha256:3e640bbe614e2c612a0234a760239253353017f54ea632d8e70ca5007fc1129d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.6 MB (230599389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38c8b38fb0ee5f997e90812c188e9956c7ea18acf1131589a9e1d93bc640c80a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:38:03 GMT
ADD file:602a25173054242f635a5a299845b7f1b56864ac5d3b8af1ae29dec3a9da119f in / 
# Wed, 20 Apr 2022 07:38:04 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:49:46 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 20 Apr 2022 12:49:55 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 12:50:19 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 20 Apr 2022 12:52:21 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a13b13d818745c4d2234aab71df26e4a01bfe59f396ab62f20d156b94803650c`  
		Last Modified: Wed, 20 Apr 2022 07:45:46 GMT  
		Size: 27.8 MB (27799825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc19bd2071107b873877fbe3bf3e623d524ecd131b76d25f818ed40f8888a5ae`  
		Last Modified: Wed, 20 Apr 2022 12:53:33 GMT  
		Size: 2.8 MB (2789172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c731ec96f4a6bd8004ee92ad713c93444a1f646c970369e7c6d60ed2ffcf37b`  
		Last Modified: Wed, 20 Apr 2022 12:53:47 GMT  
		Size: 68.6 MB (68594373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af0ca9622588725474f2f5434ce305f02b1b9a597c878f49af99e99c444e22d`  
		Last Modified: Wed, 20 Apr 2022 12:55:04 GMT  
		Size: 131.4 MB (131416019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; ppc64le

```console
$ docker pull mono@sha256:4c88c0b5ac02dbaa91e5fe480820eb22fdc55f20bff0d7df9777d0a91922c678
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.4 MB (192387948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:387368637882df34976d77a30673f716abdd5419b3123ad8df120f22b5fcf888`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 09:47:47 GMT
ADD file:69078e7ae6d887f7e36ae048f98f784678fbd8b7a8ec27e3c2bce0d68a47236d in / 
# Wed, 20 Apr 2022 09:47:51 GMT
CMD ["bash"]
# Thu, 21 Apr 2022 08:16:13 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 21 Apr 2022 08:17:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 21 Apr 2022 08:18:20 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 21 Apr 2022 08:32:10 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1aacfa28cbcef999a852ce9c261b67f15f0ccd8450cd1dbfe7b0dc88e6b5aba2`  
		Last Modified: Wed, 20 Apr 2022 09:58:02 GMT  
		Size: 30.6 MB (30560296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de0a54d8df38d9e19040e4cc35d23ae39540f55b101c788d75b0f5bd7962f0a`  
		Last Modified: Thu, 21 Apr 2022 08:33:33 GMT  
		Size: 2.9 MB (2892565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1d68d6079e85f0ac3901f7af3c469922c3215d043be6e89e661e469915359b`  
		Last Modified: Thu, 21 Apr 2022 08:33:39 GMT  
		Size: 26.9 MB (26917630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d122d2862ed40219e98f737a6743b292bffac45b31c4f9fe88dc4d81365574e2`  
		Last Modified: Thu, 21 Apr 2022 08:35:08 GMT  
		Size: 132.0 MB (132017457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10.0-slim`

```console
$ docker pull mono@sha256:ff8040cc7d0ad003a0784be5d7217770d837595a8525e1fa6d3288fad7b3967d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.10.0-slim` - linux; amd64

```console
$ docker pull mono@sha256:b832b286c91b52d8ceb75e10c045dd0b8091eacc7dec1bf578cc93f787789094
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94696869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bac78024d85353c207f9dcab4346ac9427e1db31bba198d343bd15b9ed785115`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:48 GMT
ADD file:011a43ee23214c201afb7f3b5be592f374b89a4c71aea82ca66146bbbc31b959 in / 
# Wed, 20 Apr 2022 04:43:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 15:28:00 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 20 Apr 2022 15:28:08 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 15:28:35 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4be315f6562fccf08fd6c749557e31e45ab6d987370e20e2c4933ddb04ddd5ff`  
		Last Modified: Wed, 20 Apr 2022 04:49:15 GMT  
		Size: 27.1 MB (27140664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c12dd5e44bf113633b7b789afce59d2c53cecb26c0693c47714e66ecd2b791b`  
		Last Modified: Wed, 20 Apr 2022 15:39:27 GMT  
		Size: 2.8 MB (2777352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf9809b5ba703db3a6b728b82e97ac17e874b7f3e1b617c6d07823e9aae072f1`  
		Last Modified: Wed, 20 Apr 2022 15:39:37 GMT  
		Size: 64.8 MB (64778853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:c20dba7db17e25a0be339572fb3d52ce94d16cba9ac00d848d9c2521aa32516e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51879008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e82eef5d0fd90db316ae1e2eaede51fe23e748b0d05b2e224f14dbc82477f22`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:17:47 GMT
ADD file:5b740716d202d2f3494df5e108c0ba999125920ed9c97803fe0ccdfeba5cf518 in / 
# Wed, 20 Apr 2022 07:17:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 13:47:33 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 20 Apr 2022 13:48:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 13:48:48 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1fc8704cfa531d4583c5d4d571b836a82c02a812dae88792c4397cf1c1770405`  
		Last Modified: Wed, 20 Apr 2022 07:33:54 GMT  
		Size: 24.9 MB (24889592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c5aa1543e8c9a4e82aa5c90d45e997347b2b2b85405e8d14879e0576d7df05a`  
		Last Modified: Wed, 20 Apr 2022 13:57:37 GMT  
		Size: 2.5 MB (2467655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:125bf149bad0edeae0dc7ad63977373207cea521e833db746a0098de085b98d6`  
		Last Modified: Wed, 20 Apr 2022 13:57:55 GMT  
		Size: 24.5 MB (24521761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:6beca2f9eb9de605de516a5f5c87895701d1992d3d23b49d3093e9ee30fb527f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48929721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b85dce8f495fd90df563aba07128ceab1ede7236275f6dc501a20977712f0b1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 13:28:26 GMT
ADD file:2a755b6e7bf01ec959b8bb848b6d46f292821a0bf08e04d565991ec4bdbea029 in / 
# Wed, 20 Apr 2022 13:28:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 22:06:40 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 20 Apr 2022 22:07:05 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 22:07:49 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:88467ac22b4358b1b60009f6332ba9e12b7a82a36bef334d91d68dbf8b58d96f`  
		Last Modified: Wed, 20 Apr 2022 13:45:04 GMT  
		Size: 22.7 MB (22747865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d8152d34419455b6bf7d8c0f2724cffc7860178bd5f7d2b0977f1f3a88ba2b`  
		Last Modified: Wed, 20 Apr 2022 22:16:07 GMT  
		Size: 2.4 MB (2366963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030a0bfd9369a7ac4c283002f40b9eff5fe55a3f7dd2ab033754f096aae7b225`  
		Last Modified: Wed, 20 Apr 2022 22:16:24 GMT  
		Size: 23.8 MB (23814893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:fd0ffe089ab133d58978ea5e51d43135e9a8c87b86be3997fd1e5b0d581cc2ee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57911076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:147cc7fd6295707399eab462793e12cbddb6d439837b2897b3c69b2125dbc6e2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:36 GMT
ADD file:5de4397c1295f7249c93907be599d96efbd9cd25909340d245ec8d1c9770f444 in / 
# Wed, 20 Apr 2022 04:29:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 09:34:48 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 20 Apr 2022 09:34:57 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 09:35:12 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:6c3e5b218d6477ff77053280968d5bdeaa5dcf16a803e917d98dd0ea8b93ac82`  
		Last Modified: Wed, 20 Apr 2022 04:36:38 GMT  
		Size: 25.9 MB (25908349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df56c08b5590c539b81f96718f5057b07ceaaf7017a28704b0f095af7166af2f`  
		Last Modified: Wed, 20 Apr 2022 09:38:39 GMT  
		Size: 2.6 MB (2641023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34f53b7c9a1d5af7034cdc60069b6b9c3b2099c676574b0de7e22085ba360dc`  
		Last Modified: Wed, 20 Apr 2022 09:38:44 GMT  
		Size: 29.4 MB (29361704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; 386

```console
$ docker pull mono@sha256:8a2f06c25415df8cc6ae7315e81ca06a9ff079a357c05caf0d1b57045ad265fa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99183370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a4588d79da86f7cab111b6c2fc82a13c1680b1134d953242a251f3c0da28b4a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:38:03 GMT
ADD file:602a25173054242f635a5a299845b7f1b56864ac5d3b8af1ae29dec3a9da119f in / 
# Wed, 20 Apr 2022 07:38:04 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:49:46 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 20 Apr 2022 12:49:55 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 12:50:19 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a13b13d818745c4d2234aab71df26e4a01bfe59f396ab62f20d156b94803650c`  
		Last Modified: Wed, 20 Apr 2022 07:45:46 GMT  
		Size: 27.8 MB (27799825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc19bd2071107b873877fbe3bf3e623d524ecd131b76d25f818ed40f8888a5ae`  
		Last Modified: Wed, 20 Apr 2022 12:53:33 GMT  
		Size: 2.8 MB (2789172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c731ec96f4a6bd8004ee92ad713c93444a1f646c970369e7c6d60ed2ffcf37b`  
		Last Modified: Wed, 20 Apr 2022 12:53:47 GMT  
		Size: 68.6 MB (68594373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:6203bc52c8d103d8b3443f587b445dc6560c72ccb9e3be3e8c362cdcaafce09e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.4 MB (60370491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e04bf5f65354fea4785a3e0189d9f0898c08bcad2e4f9aef81b0aeac97243bac`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 09:47:47 GMT
ADD file:69078e7ae6d887f7e36ae048f98f784678fbd8b7a8ec27e3c2bce0d68a47236d in / 
# Wed, 20 Apr 2022 09:47:51 GMT
CMD ["bash"]
# Thu, 21 Apr 2022 08:16:13 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 21 Apr 2022 08:17:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 21 Apr 2022 08:18:20 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1aacfa28cbcef999a852ce9c261b67f15f0ccd8450cd1dbfe7b0dc88e6b5aba2`  
		Last Modified: Wed, 20 Apr 2022 09:58:02 GMT  
		Size: 30.6 MB (30560296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de0a54d8df38d9e19040e4cc35d23ae39540f55b101c788d75b0f5bd7962f0a`  
		Last Modified: Thu, 21 Apr 2022 08:33:33 GMT  
		Size: 2.9 MB (2892565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1d68d6079e85f0ac3901f7af3c469922c3215d043be6e89e661e469915359b`  
		Last Modified: Thu, 21 Apr 2022 08:33:39 GMT  
		Size: 26.9 MB (26917630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10.0.104`

```console
$ docker pull mono@sha256:e41b67d54fb7d512ed0d1ff03444368d0bcbc6e181e6acd8595997d510f3b579
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.10.0.104` - linux; amd64

```console
$ docker pull mono@sha256:267540e87836271ff00bfad52c21dfc29f04f8686360a8c7790e959e4a5beab6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.0 MB (225005254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59e31c6453c88e8b1eadae06b24055a3c63c97bfd312dd97ca0d0d6aa3bc3358`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:48 GMT
ADD file:011a43ee23214c201afb7f3b5be592f374b89a4c71aea82ca66146bbbc31b959 in / 
# Wed, 20 Apr 2022 04:43:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 15:28:00 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 20 Apr 2022 15:28:08 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 15:28:35 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 20 Apr 2022 15:38:34 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4be315f6562fccf08fd6c749557e31e45ab6d987370e20e2c4933ddb04ddd5ff`  
		Last Modified: Wed, 20 Apr 2022 04:49:15 GMT  
		Size: 27.1 MB (27140664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c12dd5e44bf113633b7b789afce59d2c53cecb26c0693c47714e66ecd2b791b`  
		Last Modified: Wed, 20 Apr 2022 15:39:27 GMT  
		Size: 2.8 MB (2777352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf9809b5ba703db3a6b728b82e97ac17e874b7f3e1b617c6d07823e9aae072f1`  
		Last Modified: Wed, 20 Apr 2022 15:39:37 GMT  
		Size: 64.8 MB (64778853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6ff02d78da9ac75dffb18fad228a95dc17cbe7ec2e45e3c124576d1cf96730`  
		Last Modified: Wed, 20 Apr 2022 15:40:51 GMT  
		Size: 130.3 MB (130308385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; arm variant v5

```console
$ docker pull mono@sha256:c21ddc74f1ee678d26a4aba4428901c2889dc42c0737262ae205ec6dd5bb7c00
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.9 MB (180857223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d17c4501c297c80f49fd52b919d90e4d75484134cc71509d5ab04fdf40e596fb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:17:47 GMT
ADD file:5b740716d202d2f3494df5e108c0ba999125920ed9c97803fe0ccdfeba5cf518 in / 
# Wed, 20 Apr 2022 07:17:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 13:47:33 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 20 Apr 2022 13:48:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 13:48:48 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 20 Apr 2022 13:55:30 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1fc8704cfa531d4583c5d4d571b836a82c02a812dae88792c4397cf1c1770405`  
		Last Modified: Wed, 20 Apr 2022 07:33:54 GMT  
		Size: 24.9 MB (24889592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c5aa1543e8c9a4e82aa5c90d45e997347b2b2b85405e8d14879e0576d7df05a`  
		Last Modified: Wed, 20 Apr 2022 13:57:37 GMT  
		Size: 2.5 MB (2467655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:125bf149bad0edeae0dc7ad63977373207cea521e833db746a0098de085b98d6`  
		Last Modified: Wed, 20 Apr 2022 13:57:55 GMT  
		Size: 24.5 MB (24521761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6245f63551657140eed74fd21cdb79948901f1b69d7d7b036779d01667e2a59`  
		Last Modified: Wed, 20 Apr 2022 14:01:33 GMT  
		Size: 129.0 MB (128978215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; arm variant v7

```console
$ docker pull mono@sha256:2cec20e212eddef7773607ff9375f0c5d9a1096964b6af0350b0c0e1c206ba83
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.8 MB (176759115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8eda3475765acc4ffab5cc260d0a5aa6fdb589829a3e14001544cc19b9c9b929`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 13:28:26 GMT
ADD file:2a755b6e7bf01ec959b8bb848b6d46f292821a0bf08e04d565991ec4bdbea029 in / 
# Wed, 20 Apr 2022 13:28:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 22:06:40 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 20 Apr 2022 22:07:05 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 22:07:49 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 20 Apr 2022 22:14:04 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:88467ac22b4358b1b60009f6332ba9e12b7a82a36bef334d91d68dbf8b58d96f`  
		Last Modified: Wed, 20 Apr 2022 13:45:04 GMT  
		Size: 22.7 MB (22747865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d8152d34419455b6bf7d8c0f2724cffc7860178bd5f7d2b0977f1f3a88ba2b`  
		Last Modified: Wed, 20 Apr 2022 22:16:07 GMT  
		Size: 2.4 MB (2366963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030a0bfd9369a7ac4c283002f40b9eff5fe55a3f7dd2ab033754f096aae7b225`  
		Last Modified: Wed, 20 Apr 2022 22:16:24 GMT  
		Size: 23.8 MB (23814893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c213333d5cb65819a25c36d23181bfb12e6e88a9f44def07f0338f879e3726a`  
		Last Modified: Wed, 20 Apr 2022 22:20:05 GMT  
		Size: 127.8 MB (127829394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:db4ccba0ea3a15d03bce129dc7b8f8c1d17eb414d22d0ce50f04c91aa9dc8e6b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.4 MB (203357942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:542f1d2be1793e91d33d40c760fdeff6d2626a9c03e0bb060de4fc1929460c11`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:36 GMT
ADD file:5de4397c1295f7249c93907be599d96efbd9cd25909340d245ec8d1c9770f444 in / 
# Wed, 20 Apr 2022 04:29:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 09:34:48 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 20 Apr 2022 09:34:57 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 09:35:12 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 20 Apr 2022 09:37:30 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:6c3e5b218d6477ff77053280968d5bdeaa5dcf16a803e917d98dd0ea8b93ac82`  
		Last Modified: Wed, 20 Apr 2022 04:36:38 GMT  
		Size: 25.9 MB (25908349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df56c08b5590c539b81f96718f5057b07ceaaf7017a28704b0f095af7166af2f`  
		Last Modified: Wed, 20 Apr 2022 09:38:39 GMT  
		Size: 2.6 MB (2641023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34f53b7c9a1d5af7034cdc60069b6b9c3b2099c676574b0de7e22085ba360dc`  
		Last Modified: Wed, 20 Apr 2022 09:38:44 GMT  
		Size: 29.4 MB (29361704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3f7de6536f999251c110135ca6a52d08565af7071c6fe5eea96fbd6578aa58`  
		Last Modified: Wed, 20 Apr 2022 09:40:03 GMT  
		Size: 145.4 MB (145446866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; 386

```console
$ docker pull mono@sha256:3e640bbe614e2c612a0234a760239253353017f54ea632d8e70ca5007fc1129d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.6 MB (230599389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38c8b38fb0ee5f997e90812c188e9956c7ea18acf1131589a9e1d93bc640c80a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:38:03 GMT
ADD file:602a25173054242f635a5a299845b7f1b56864ac5d3b8af1ae29dec3a9da119f in / 
# Wed, 20 Apr 2022 07:38:04 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:49:46 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 20 Apr 2022 12:49:55 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 12:50:19 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 20 Apr 2022 12:52:21 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a13b13d818745c4d2234aab71df26e4a01bfe59f396ab62f20d156b94803650c`  
		Last Modified: Wed, 20 Apr 2022 07:45:46 GMT  
		Size: 27.8 MB (27799825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc19bd2071107b873877fbe3bf3e623d524ecd131b76d25f818ed40f8888a5ae`  
		Last Modified: Wed, 20 Apr 2022 12:53:33 GMT  
		Size: 2.8 MB (2789172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c731ec96f4a6bd8004ee92ad713c93444a1f646c970369e7c6d60ed2ffcf37b`  
		Last Modified: Wed, 20 Apr 2022 12:53:47 GMT  
		Size: 68.6 MB (68594373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af0ca9622588725474f2f5434ce305f02b1b9a597c878f49af99e99c444e22d`  
		Last Modified: Wed, 20 Apr 2022 12:55:04 GMT  
		Size: 131.4 MB (131416019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; ppc64le

```console
$ docker pull mono@sha256:4c88c0b5ac02dbaa91e5fe480820eb22fdc55f20bff0d7df9777d0a91922c678
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.4 MB (192387948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:387368637882df34976d77a30673f716abdd5419b3123ad8df120f22b5fcf888`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 09:47:47 GMT
ADD file:69078e7ae6d887f7e36ae048f98f784678fbd8b7a8ec27e3c2bce0d68a47236d in / 
# Wed, 20 Apr 2022 09:47:51 GMT
CMD ["bash"]
# Thu, 21 Apr 2022 08:16:13 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 21 Apr 2022 08:17:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 21 Apr 2022 08:18:20 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 21 Apr 2022 08:32:10 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1aacfa28cbcef999a852ce9c261b67f15f0ccd8450cd1dbfe7b0dc88e6b5aba2`  
		Last Modified: Wed, 20 Apr 2022 09:58:02 GMT  
		Size: 30.6 MB (30560296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de0a54d8df38d9e19040e4cc35d23ae39540f55b101c788d75b0f5bd7962f0a`  
		Last Modified: Thu, 21 Apr 2022 08:33:33 GMT  
		Size: 2.9 MB (2892565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1d68d6079e85f0ac3901f7af3c469922c3215d043be6e89e661e469915359b`  
		Last Modified: Thu, 21 Apr 2022 08:33:39 GMT  
		Size: 26.9 MB (26917630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d122d2862ed40219e98f737a6743b292bffac45b31c4f9fe88dc4d81365574e2`  
		Last Modified: Thu, 21 Apr 2022 08:35:08 GMT  
		Size: 132.0 MB (132017457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10.0.104-slim`

```console
$ docker pull mono@sha256:ff8040cc7d0ad003a0784be5d7217770d837595a8525e1fa6d3288fad7b3967d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.10.0.104-slim` - linux; amd64

```console
$ docker pull mono@sha256:b832b286c91b52d8ceb75e10c045dd0b8091eacc7dec1bf578cc93f787789094
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94696869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bac78024d85353c207f9dcab4346ac9427e1db31bba198d343bd15b9ed785115`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:48 GMT
ADD file:011a43ee23214c201afb7f3b5be592f374b89a4c71aea82ca66146bbbc31b959 in / 
# Wed, 20 Apr 2022 04:43:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 15:28:00 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 20 Apr 2022 15:28:08 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 15:28:35 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4be315f6562fccf08fd6c749557e31e45ab6d987370e20e2c4933ddb04ddd5ff`  
		Last Modified: Wed, 20 Apr 2022 04:49:15 GMT  
		Size: 27.1 MB (27140664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c12dd5e44bf113633b7b789afce59d2c53cecb26c0693c47714e66ecd2b791b`  
		Last Modified: Wed, 20 Apr 2022 15:39:27 GMT  
		Size: 2.8 MB (2777352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf9809b5ba703db3a6b728b82e97ac17e874b7f3e1b617c6d07823e9aae072f1`  
		Last Modified: Wed, 20 Apr 2022 15:39:37 GMT  
		Size: 64.8 MB (64778853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:c20dba7db17e25a0be339572fb3d52ce94d16cba9ac00d848d9c2521aa32516e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51879008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e82eef5d0fd90db316ae1e2eaede51fe23e748b0d05b2e224f14dbc82477f22`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:17:47 GMT
ADD file:5b740716d202d2f3494df5e108c0ba999125920ed9c97803fe0ccdfeba5cf518 in / 
# Wed, 20 Apr 2022 07:17:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 13:47:33 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 20 Apr 2022 13:48:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 13:48:48 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1fc8704cfa531d4583c5d4d571b836a82c02a812dae88792c4397cf1c1770405`  
		Last Modified: Wed, 20 Apr 2022 07:33:54 GMT  
		Size: 24.9 MB (24889592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c5aa1543e8c9a4e82aa5c90d45e997347b2b2b85405e8d14879e0576d7df05a`  
		Last Modified: Wed, 20 Apr 2022 13:57:37 GMT  
		Size: 2.5 MB (2467655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:125bf149bad0edeae0dc7ad63977373207cea521e833db746a0098de085b98d6`  
		Last Modified: Wed, 20 Apr 2022 13:57:55 GMT  
		Size: 24.5 MB (24521761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:6beca2f9eb9de605de516a5f5c87895701d1992d3d23b49d3093e9ee30fb527f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48929721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b85dce8f495fd90df563aba07128ceab1ede7236275f6dc501a20977712f0b1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 13:28:26 GMT
ADD file:2a755b6e7bf01ec959b8bb848b6d46f292821a0bf08e04d565991ec4bdbea029 in / 
# Wed, 20 Apr 2022 13:28:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 22:06:40 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 20 Apr 2022 22:07:05 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 22:07:49 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:88467ac22b4358b1b60009f6332ba9e12b7a82a36bef334d91d68dbf8b58d96f`  
		Last Modified: Wed, 20 Apr 2022 13:45:04 GMT  
		Size: 22.7 MB (22747865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d8152d34419455b6bf7d8c0f2724cffc7860178bd5f7d2b0977f1f3a88ba2b`  
		Last Modified: Wed, 20 Apr 2022 22:16:07 GMT  
		Size: 2.4 MB (2366963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030a0bfd9369a7ac4c283002f40b9eff5fe55a3f7dd2ab033754f096aae7b225`  
		Last Modified: Wed, 20 Apr 2022 22:16:24 GMT  
		Size: 23.8 MB (23814893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:fd0ffe089ab133d58978ea5e51d43135e9a8c87b86be3997fd1e5b0d581cc2ee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57911076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:147cc7fd6295707399eab462793e12cbddb6d439837b2897b3c69b2125dbc6e2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:36 GMT
ADD file:5de4397c1295f7249c93907be599d96efbd9cd25909340d245ec8d1c9770f444 in / 
# Wed, 20 Apr 2022 04:29:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 09:34:48 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 20 Apr 2022 09:34:57 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 09:35:12 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:6c3e5b218d6477ff77053280968d5bdeaa5dcf16a803e917d98dd0ea8b93ac82`  
		Last Modified: Wed, 20 Apr 2022 04:36:38 GMT  
		Size: 25.9 MB (25908349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df56c08b5590c539b81f96718f5057b07ceaaf7017a28704b0f095af7166af2f`  
		Last Modified: Wed, 20 Apr 2022 09:38:39 GMT  
		Size: 2.6 MB (2641023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34f53b7c9a1d5af7034cdc60069b6b9c3b2099c676574b0de7e22085ba360dc`  
		Last Modified: Wed, 20 Apr 2022 09:38:44 GMT  
		Size: 29.4 MB (29361704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; 386

```console
$ docker pull mono@sha256:8a2f06c25415df8cc6ae7315e81ca06a9ff079a357c05caf0d1b57045ad265fa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99183370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a4588d79da86f7cab111b6c2fc82a13c1680b1134d953242a251f3c0da28b4a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:38:03 GMT
ADD file:602a25173054242f635a5a299845b7f1b56864ac5d3b8af1ae29dec3a9da119f in / 
# Wed, 20 Apr 2022 07:38:04 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:49:46 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 20 Apr 2022 12:49:55 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 12:50:19 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a13b13d818745c4d2234aab71df26e4a01bfe59f396ab62f20d156b94803650c`  
		Last Modified: Wed, 20 Apr 2022 07:45:46 GMT  
		Size: 27.8 MB (27799825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc19bd2071107b873877fbe3bf3e623d524ecd131b76d25f818ed40f8888a5ae`  
		Last Modified: Wed, 20 Apr 2022 12:53:33 GMT  
		Size: 2.8 MB (2789172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c731ec96f4a6bd8004ee92ad713c93444a1f646c970369e7c6d60ed2ffcf37b`  
		Last Modified: Wed, 20 Apr 2022 12:53:47 GMT  
		Size: 68.6 MB (68594373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:6203bc52c8d103d8b3443f587b445dc6560c72ccb9e3be3e8c362cdcaafce09e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.4 MB (60370491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e04bf5f65354fea4785a3e0189d9f0898c08bcad2e4f9aef81b0aeac97243bac`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 09:47:47 GMT
ADD file:69078e7ae6d887f7e36ae048f98f784678fbd8b7a8ec27e3c2bce0d68a47236d in / 
# Wed, 20 Apr 2022 09:47:51 GMT
CMD ["bash"]
# Thu, 21 Apr 2022 08:16:13 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 21 Apr 2022 08:17:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 21 Apr 2022 08:18:20 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1aacfa28cbcef999a852ce9c261b67f15f0ccd8450cd1dbfe7b0dc88e6b5aba2`  
		Last Modified: Wed, 20 Apr 2022 09:58:02 GMT  
		Size: 30.6 MB (30560296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de0a54d8df38d9e19040e4cc35d23ae39540f55b101c788d75b0f5bd7962f0a`  
		Last Modified: Thu, 21 Apr 2022 08:33:33 GMT  
		Size: 2.9 MB (2892565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1d68d6079e85f0ac3901f7af3c469922c3215d043be6e89e661e469915359b`  
		Last Modified: Thu, 21 Apr 2022 08:33:39 GMT  
		Size: 26.9 MB (26917630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.12`

```console
$ docker pull mono@sha256:8e6aa0dc91a317d6b4ada45be67e01948c3b620226538928a4374ccea987abbc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.12` - linux; amd64

```console
$ docker pull mono@sha256:0c36486cbda2ab995af85a2e9bbe62cc56bd2cf77d030fb67c3c228c920d74cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.1 MB (236125631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a50ead981e57279bc2232fe42e0e534ddd348365a0df2aa9f7a6ea1043c1412e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:48 GMT
ADD file:011a43ee23214c201afb7f3b5be592f374b89a4c71aea82ca66146bbbc31b959 in / 
# Wed, 20 Apr 2022 04:43:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 15:27:27 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 15:27:35 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 15:27:54 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 20 Apr 2022 15:33:01 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4be315f6562fccf08fd6c749557e31e45ab6d987370e20e2c4933ddb04ddd5ff`  
		Last Modified: Wed, 20 Apr 2022 04:49:15 GMT  
		Size: 27.1 MB (27140664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20d9f7ad1a1561508daa15f30ed450e8279f8633fc277a84bd6f5b1d00ecf314`  
		Last Modified: Wed, 20 Apr 2022 15:39:01 GMT  
		Size: 2.8 MB (2777363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4214d10d224872d47c1c108360a2890678eff5f2e288cdefa4f0882ac8ff9e46`  
		Last Modified: Wed, 20 Apr 2022 15:39:10 GMT  
		Size: 64.8 MB (64759348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa0a929eb8545fe353e58ddc4af329eefbe9e50f63bbbf938d0256d77246e6a`  
		Last Modified: Wed, 20 Apr 2022 15:40:09 GMT  
		Size: 141.4 MB (141448256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12` - linux; arm variant v5

```console
$ docker pull mono@sha256:258511710254d92fe26e82049f226a7e527f0ed49778129c70646e9fc329af2a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.0 MB (191957036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac351dfd94cc0f2249f8760f8fedebcc5a814cdd11a7bef18de24f24f52c37fa`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:17:47 GMT
ADD file:5b740716d202d2f3494df5e108c0ba999125920ed9c97803fe0ccdfeba5cf518 in / 
# Wed, 20 Apr 2022 07:17:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 13:45:59 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 13:46:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 13:47:13 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 20 Apr 2022 13:52:09 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1fc8704cfa531d4583c5d4d571b836a82c02a812dae88792c4397cf1c1770405`  
		Last Modified: Wed, 20 Apr 2022 07:33:54 GMT  
		Size: 24.9 MB (24889592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de67cfe4308dcefca53d406cca104b0f4db6a1d2dda37929256a8f8761e5550a`  
		Last Modified: Wed, 20 Apr 2022 13:56:57 GMT  
		Size: 2.5 MB (2467647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641f8380b2823093df874b2b79c65d2f31452f99f5896f56a17614cbcb1dc971`  
		Last Modified: Wed, 20 Apr 2022 13:57:13 GMT  
		Size: 24.5 MB (24492891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68839de10302780399729e3999eb88f5e1ed8ca5c135b146dbb11f63aa458dfa`  
		Last Modified: Wed, 20 Apr 2022 13:59:38 GMT  
		Size: 140.1 MB (140106906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12` - linux; arm variant v7

```console
$ docker pull mono@sha256:ad3a93a04d11ffb9206df13b87aa8a10890bc78b826eef7fbbbb160387b29507
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.9 MB (187864260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c65447e8e52004d2ac80a42c301fd6f3eb5fe6898ca081f77decd51bed084fc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 13:28:26 GMT
ADD file:2a755b6e7bf01ec959b8bb848b6d46f292821a0bf08e04d565991ec4bdbea029 in / 
# Wed, 20 Apr 2022 13:28:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 22:05:17 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 22:05:41 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 22:06:24 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 20 Apr 2022 22:10:56 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:88467ac22b4358b1b60009f6332ba9e12b7a82a36bef334d91d68dbf8b58d96f`  
		Last Modified: Wed, 20 Apr 2022 13:45:04 GMT  
		Size: 22.7 MB (22747865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e27b3994c35244605adec982fe00db7376f48e5ec599c253a2465ef79124c80`  
		Last Modified: Wed, 20 Apr 2022 22:15:27 GMT  
		Size: 2.4 MB (2366878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8554905d57c581805a8fc875940e3e39baa10f0bbc841e4b1f192d1c968eafc2`  
		Last Modified: Wed, 20 Apr 2022 22:15:44 GMT  
		Size: 23.8 MB (23782556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b332d3b0da4d9e0bbb73a313bd1158fad6ed98c34ac243e90a2b37dcdac08e4`  
		Last Modified: Wed, 20 Apr 2022 22:18:18 GMT  
		Size: 139.0 MB (138966961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:617fd6f5ff9238ff8782c0b154f5fbb1e51864ad1f009da0d0c5fcd54ff179c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.5 MB (214465680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:721976153f55a700a3368032ce347eb3ae7b930fc6151b879332e0e99f1ca0cc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:36 GMT
ADD file:5de4397c1295f7249c93907be599d96efbd9cd25909340d245ec8d1c9770f444 in / 
# Wed, 20 Apr 2022 04:29:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 09:34:15 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 09:34:25 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 09:34:40 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 20 Apr 2022 09:36:17 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:6c3e5b218d6477ff77053280968d5bdeaa5dcf16a803e917d98dd0ea8b93ac82`  
		Last Modified: Wed, 20 Apr 2022 04:36:38 GMT  
		Size: 25.9 MB (25908349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5583d434a71d4775ae033dd3567325a5f5d01a34ff9f805631b17426570d60`  
		Last Modified: Wed, 20 Apr 2022 09:38:16 GMT  
		Size: 2.6 MB (2641065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1df7a4f3775402176b947b2ffb1f930879581b64904846f29bd8e5aa4000e4d`  
		Last Modified: Wed, 20 Apr 2022 09:38:20 GMT  
		Size: 29.3 MB (29318359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f80c1eac9d435a1e808ae3c8eaf8a76d9e653e54edc1090cf4c2fc47f29f6e`  
		Last Modified: Wed, 20 Apr 2022 09:39:21 GMT  
		Size: 156.6 MB (156597907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12` - linux; 386

```console
$ docker pull mono@sha256:ef781f5c402c37c294ccf7397654b6a780c16c68ab05b1ee598260446e0049b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.7 MB (241696337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:faa267e26ab7e853336277f2575154ad396b6536c3cd9e8ba22824250ccc6fbd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:38:03 GMT
ADD file:602a25173054242f635a5a299845b7f1b56864ac5d3b8af1ae29dec3a9da119f in / 
# Wed, 20 Apr 2022 07:38:04 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:49:08 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 12:49:17 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 12:49:40 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 20 Apr 2022 12:51:19 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a13b13d818745c4d2234aab71df26e4a01bfe59f396ab62f20d156b94803650c`  
		Last Modified: Wed, 20 Apr 2022 07:45:46 GMT  
		Size: 27.8 MB (27799825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc07624832ff4b064bd2b3797a6774618e27f4c3a1e24419874628eeb613e7ba`  
		Last Modified: Wed, 20 Apr 2022 12:53:02 GMT  
		Size: 2.8 MB (2789161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d6af1a94baa95c219eaba2db2fb27e299572ac8d2859e1399838abdccae784c`  
		Last Modified: Wed, 20 Apr 2022 12:53:11 GMT  
		Size: 68.6 MB (68568946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec0646bfa3d97be6f7515ad03d0cbb859adebe6cf3785cf1d36d06c8aa3f224`  
		Last Modified: Wed, 20 Apr 2022 12:54:22 GMT  
		Size: 142.5 MB (142538405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12` - linux; ppc64le

```console
$ docker pull mono@sha256:abb2d6df6d771036e5878f2d8d5f7be07336dc420c2f33f5cbcd387ff20e7215
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.6 MB (203607651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d706be5bbbd80d2cfe56b5ed3350e0a17769f9e9c5ce4ee417df1efdd40f9f5d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 09:47:47 GMT
ADD file:69078e7ae6d887f7e36ae048f98f784678fbd8b7a8ec27e3c2bce0d68a47236d in / 
# Wed, 20 Apr 2022 09:47:51 GMT
CMD ["bash"]
# Thu, 21 Apr 2022 08:14:20 GMT
ENV MONO_VERSION=6.12.0.122
# Thu, 21 Apr 2022 08:15:04 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 21 Apr 2022 08:16:01 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 21 Apr 2022 08:25:53 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1aacfa28cbcef999a852ce9c261b67f15f0ccd8450cd1dbfe7b0dc88e6b5aba2`  
		Last Modified: Wed, 20 Apr 2022 09:58:02 GMT  
		Size: 30.6 MB (30560296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b4fd6959397baa971e32512d4c0d1d094bea59e1bf9b3442d8a345c6f7cd81`  
		Last Modified: Thu, 21 Apr 2022 08:33:06 GMT  
		Size: 2.9 MB (2892563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff24986d59f2106922e32fbd04b151763111155f6440aa41d390cbab27fca8c8`  
		Last Modified: Thu, 21 Apr 2022 08:33:11 GMT  
		Size: 26.9 MB (26873691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c14de3289c90efbcb5ba56806674834ab22b34135aa29d559635cdfb7805907`  
		Last Modified: Thu, 21 Apr 2022 08:34:20 GMT  
		Size: 143.3 MB (143281101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.12-slim`

```console
$ docker pull mono@sha256:df384bda4d7d65b1fc3842d0eaa6d5bb7d188c95f274e7cc8403b002c6ec8b82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.12-slim` - linux; amd64

```console
$ docker pull mono@sha256:f0d95c21aa0a9490ae955fe78fc0f316616807db95b5790b5cd7b4391ac8568d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94677375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4291e2c603690115cbb2d33ea0dee4ab69b47aa89201a4fc53d449bd5c5e9d02`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:48 GMT
ADD file:011a43ee23214c201afb7f3b5be592f374b89a4c71aea82ca66146bbbc31b959 in / 
# Wed, 20 Apr 2022 04:43:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 15:27:27 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 15:27:35 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 15:27:54 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4be315f6562fccf08fd6c749557e31e45ab6d987370e20e2c4933ddb04ddd5ff`  
		Last Modified: Wed, 20 Apr 2022 04:49:15 GMT  
		Size: 27.1 MB (27140664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20d9f7ad1a1561508daa15f30ed450e8279f8633fc277a84bd6f5b1d00ecf314`  
		Last Modified: Wed, 20 Apr 2022 15:39:01 GMT  
		Size: 2.8 MB (2777363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4214d10d224872d47c1c108360a2890678eff5f2e288cdefa4f0882ac8ff9e46`  
		Last Modified: Wed, 20 Apr 2022 15:39:10 GMT  
		Size: 64.8 MB (64759348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:c3b087e497272a1ff39fc23bc98d4fe778bf411c3c00de946f43fe57cd6e9d50
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51850130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03bf635a6d765f56a65311bc43513ec14a0451754d992adcadcf3c7f67503ca8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:17:47 GMT
ADD file:5b740716d202d2f3494df5e108c0ba999125920ed9c97803fe0ccdfeba5cf518 in / 
# Wed, 20 Apr 2022 07:17:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 13:45:59 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 13:46:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 13:47:13 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1fc8704cfa531d4583c5d4d571b836a82c02a812dae88792c4397cf1c1770405`  
		Last Modified: Wed, 20 Apr 2022 07:33:54 GMT  
		Size: 24.9 MB (24889592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de67cfe4308dcefca53d406cca104b0f4db6a1d2dda37929256a8f8761e5550a`  
		Last Modified: Wed, 20 Apr 2022 13:56:57 GMT  
		Size: 2.5 MB (2467647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641f8380b2823093df874b2b79c65d2f31452f99f5896f56a17614cbcb1dc971`  
		Last Modified: Wed, 20 Apr 2022 13:57:13 GMT  
		Size: 24.5 MB (24492891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:faff62d5274b7437f4216c427da824165d03a1c90c7c0f79e08533937b868eee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48897299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:659c685d861a835af511fa1dc5758b62d34b1e713f3db36f2e4f3d1cc184057c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 13:28:26 GMT
ADD file:2a755b6e7bf01ec959b8bb848b6d46f292821a0bf08e04d565991ec4bdbea029 in / 
# Wed, 20 Apr 2022 13:28:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 22:05:17 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 22:05:41 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 22:06:24 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:88467ac22b4358b1b60009f6332ba9e12b7a82a36bef334d91d68dbf8b58d96f`  
		Last Modified: Wed, 20 Apr 2022 13:45:04 GMT  
		Size: 22.7 MB (22747865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e27b3994c35244605adec982fe00db7376f48e5ec599c253a2465ef79124c80`  
		Last Modified: Wed, 20 Apr 2022 22:15:27 GMT  
		Size: 2.4 MB (2366878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8554905d57c581805a8fc875940e3e39baa10f0bbc841e4b1f192d1c968eafc2`  
		Last Modified: Wed, 20 Apr 2022 22:15:44 GMT  
		Size: 23.8 MB (23782556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:0f3837c80f89d4cc61d33d11680310dd7b9170aa4a20287829db1cf4ff83169c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57867773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a03207fd5f3c9c31e878dec4d955581897e75177774ac4915f726360915f8e8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:36 GMT
ADD file:5de4397c1295f7249c93907be599d96efbd9cd25909340d245ec8d1c9770f444 in / 
# Wed, 20 Apr 2022 04:29:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 09:34:15 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 09:34:25 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 09:34:40 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:6c3e5b218d6477ff77053280968d5bdeaa5dcf16a803e917d98dd0ea8b93ac82`  
		Last Modified: Wed, 20 Apr 2022 04:36:38 GMT  
		Size: 25.9 MB (25908349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5583d434a71d4775ae033dd3567325a5f5d01a34ff9f805631b17426570d60`  
		Last Modified: Wed, 20 Apr 2022 09:38:16 GMT  
		Size: 2.6 MB (2641065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1df7a4f3775402176b947b2ffb1f930879581b64904846f29bd8e5aa4000e4d`  
		Last Modified: Wed, 20 Apr 2022 09:38:20 GMT  
		Size: 29.3 MB (29318359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12-slim` - linux; 386

```console
$ docker pull mono@sha256:a620c36d6b438c94797eaa6b17b2452369ac55ab8a59a1bcf8b4501df1eea0c5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99157932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95ff55aea4f3ffc1da74cea929a23a78ed6dc8901847098c5878018368c9da5d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:38:03 GMT
ADD file:602a25173054242f635a5a299845b7f1b56864ac5d3b8af1ae29dec3a9da119f in / 
# Wed, 20 Apr 2022 07:38:04 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:49:08 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 12:49:17 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 12:49:40 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a13b13d818745c4d2234aab71df26e4a01bfe59f396ab62f20d156b94803650c`  
		Last Modified: Wed, 20 Apr 2022 07:45:46 GMT  
		Size: 27.8 MB (27799825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc07624832ff4b064bd2b3797a6774618e27f4c3a1e24419874628eeb613e7ba`  
		Last Modified: Wed, 20 Apr 2022 12:53:02 GMT  
		Size: 2.8 MB (2789161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d6af1a94baa95c219eaba2db2fb27e299572ac8d2859e1399838abdccae784c`  
		Last Modified: Wed, 20 Apr 2022 12:53:11 GMT  
		Size: 68.6 MB (68568946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:13e28a240194ffdaa1ab1b8b10b807978db6ed7eec8e4d427b0ff2c6d38130b8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.3 MB (60326550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:806eebb6c6b16141507ab480ab6238efd982bbe9375a51cabbc00f5cd2fa62b5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 09:47:47 GMT
ADD file:69078e7ae6d887f7e36ae048f98f784678fbd8b7a8ec27e3c2bce0d68a47236d in / 
# Wed, 20 Apr 2022 09:47:51 GMT
CMD ["bash"]
# Thu, 21 Apr 2022 08:14:20 GMT
ENV MONO_VERSION=6.12.0.122
# Thu, 21 Apr 2022 08:15:04 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 21 Apr 2022 08:16:01 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1aacfa28cbcef999a852ce9c261b67f15f0ccd8450cd1dbfe7b0dc88e6b5aba2`  
		Last Modified: Wed, 20 Apr 2022 09:58:02 GMT  
		Size: 30.6 MB (30560296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b4fd6959397baa971e32512d4c0d1d094bea59e1bf9b3442d8a345c6f7cd81`  
		Last Modified: Thu, 21 Apr 2022 08:33:06 GMT  
		Size: 2.9 MB (2892563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff24986d59f2106922e32fbd04b151763111155f6440aa41d390cbab27fca8c8`  
		Last Modified: Thu, 21 Apr 2022 08:33:11 GMT  
		Size: 26.9 MB (26873691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.12.0`

```console
$ docker pull mono@sha256:8e6aa0dc91a317d6b4ada45be67e01948c3b620226538928a4374ccea987abbc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.12.0` - linux; amd64

```console
$ docker pull mono@sha256:0c36486cbda2ab995af85a2e9bbe62cc56bd2cf77d030fb67c3c228c920d74cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.1 MB (236125631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a50ead981e57279bc2232fe42e0e534ddd348365a0df2aa9f7a6ea1043c1412e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:48 GMT
ADD file:011a43ee23214c201afb7f3b5be592f374b89a4c71aea82ca66146bbbc31b959 in / 
# Wed, 20 Apr 2022 04:43:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 15:27:27 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 15:27:35 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 15:27:54 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 20 Apr 2022 15:33:01 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4be315f6562fccf08fd6c749557e31e45ab6d987370e20e2c4933ddb04ddd5ff`  
		Last Modified: Wed, 20 Apr 2022 04:49:15 GMT  
		Size: 27.1 MB (27140664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20d9f7ad1a1561508daa15f30ed450e8279f8633fc277a84bd6f5b1d00ecf314`  
		Last Modified: Wed, 20 Apr 2022 15:39:01 GMT  
		Size: 2.8 MB (2777363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4214d10d224872d47c1c108360a2890678eff5f2e288cdefa4f0882ac8ff9e46`  
		Last Modified: Wed, 20 Apr 2022 15:39:10 GMT  
		Size: 64.8 MB (64759348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa0a929eb8545fe353e58ddc4af329eefbe9e50f63bbbf938d0256d77246e6a`  
		Last Modified: Wed, 20 Apr 2022 15:40:09 GMT  
		Size: 141.4 MB (141448256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0` - linux; arm variant v5

```console
$ docker pull mono@sha256:258511710254d92fe26e82049f226a7e527f0ed49778129c70646e9fc329af2a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.0 MB (191957036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac351dfd94cc0f2249f8760f8fedebcc5a814cdd11a7bef18de24f24f52c37fa`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:17:47 GMT
ADD file:5b740716d202d2f3494df5e108c0ba999125920ed9c97803fe0ccdfeba5cf518 in / 
# Wed, 20 Apr 2022 07:17:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 13:45:59 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 13:46:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 13:47:13 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 20 Apr 2022 13:52:09 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1fc8704cfa531d4583c5d4d571b836a82c02a812dae88792c4397cf1c1770405`  
		Last Modified: Wed, 20 Apr 2022 07:33:54 GMT  
		Size: 24.9 MB (24889592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de67cfe4308dcefca53d406cca104b0f4db6a1d2dda37929256a8f8761e5550a`  
		Last Modified: Wed, 20 Apr 2022 13:56:57 GMT  
		Size: 2.5 MB (2467647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641f8380b2823093df874b2b79c65d2f31452f99f5896f56a17614cbcb1dc971`  
		Last Modified: Wed, 20 Apr 2022 13:57:13 GMT  
		Size: 24.5 MB (24492891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68839de10302780399729e3999eb88f5e1ed8ca5c135b146dbb11f63aa458dfa`  
		Last Modified: Wed, 20 Apr 2022 13:59:38 GMT  
		Size: 140.1 MB (140106906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0` - linux; arm variant v7

```console
$ docker pull mono@sha256:ad3a93a04d11ffb9206df13b87aa8a10890bc78b826eef7fbbbb160387b29507
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.9 MB (187864260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c65447e8e52004d2ac80a42c301fd6f3eb5fe6898ca081f77decd51bed084fc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 13:28:26 GMT
ADD file:2a755b6e7bf01ec959b8bb848b6d46f292821a0bf08e04d565991ec4bdbea029 in / 
# Wed, 20 Apr 2022 13:28:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 22:05:17 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 22:05:41 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 22:06:24 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 20 Apr 2022 22:10:56 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:88467ac22b4358b1b60009f6332ba9e12b7a82a36bef334d91d68dbf8b58d96f`  
		Last Modified: Wed, 20 Apr 2022 13:45:04 GMT  
		Size: 22.7 MB (22747865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e27b3994c35244605adec982fe00db7376f48e5ec599c253a2465ef79124c80`  
		Last Modified: Wed, 20 Apr 2022 22:15:27 GMT  
		Size: 2.4 MB (2366878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8554905d57c581805a8fc875940e3e39baa10f0bbc841e4b1f192d1c968eafc2`  
		Last Modified: Wed, 20 Apr 2022 22:15:44 GMT  
		Size: 23.8 MB (23782556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b332d3b0da4d9e0bbb73a313bd1158fad6ed98c34ac243e90a2b37dcdac08e4`  
		Last Modified: Wed, 20 Apr 2022 22:18:18 GMT  
		Size: 139.0 MB (138966961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:617fd6f5ff9238ff8782c0b154f5fbb1e51864ad1f009da0d0c5fcd54ff179c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.5 MB (214465680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:721976153f55a700a3368032ce347eb3ae7b930fc6151b879332e0e99f1ca0cc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:36 GMT
ADD file:5de4397c1295f7249c93907be599d96efbd9cd25909340d245ec8d1c9770f444 in / 
# Wed, 20 Apr 2022 04:29:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 09:34:15 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 09:34:25 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 09:34:40 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 20 Apr 2022 09:36:17 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:6c3e5b218d6477ff77053280968d5bdeaa5dcf16a803e917d98dd0ea8b93ac82`  
		Last Modified: Wed, 20 Apr 2022 04:36:38 GMT  
		Size: 25.9 MB (25908349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5583d434a71d4775ae033dd3567325a5f5d01a34ff9f805631b17426570d60`  
		Last Modified: Wed, 20 Apr 2022 09:38:16 GMT  
		Size: 2.6 MB (2641065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1df7a4f3775402176b947b2ffb1f930879581b64904846f29bd8e5aa4000e4d`  
		Last Modified: Wed, 20 Apr 2022 09:38:20 GMT  
		Size: 29.3 MB (29318359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f80c1eac9d435a1e808ae3c8eaf8a76d9e653e54edc1090cf4c2fc47f29f6e`  
		Last Modified: Wed, 20 Apr 2022 09:39:21 GMT  
		Size: 156.6 MB (156597907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0` - linux; 386

```console
$ docker pull mono@sha256:ef781f5c402c37c294ccf7397654b6a780c16c68ab05b1ee598260446e0049b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.7 MB (241696337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:faa267e26ab7e853336277f2575154ad396b6536c3cd9e8ba22824250ccc6fbd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:38:03 GMT
ADD file:602a25173054242f635a5a299845b7f1b56864ac5d3b8af1ae29dec3a9da119f in / 
# Wed, 20 Apr 2022 07:38:04 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:49:08 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 12:49:17 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 12:49:40 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 20 Apr 2022 12:51:19 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a13b13d818745c4d2234aab71df26e4a01bfe59f396ab62f20d156b94803650c`  
		Last Modified: Wed, 20 Apr 2022 07:45:46 GMT  
		Size: 27.8 MB (27799825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc07624832ff4b064bd2b3797a6774618e27f4c3a1e24419874628eeb613e7ba`  
		Last Modified: Wed, 20 Apr 2022 12:53:02 GMT  
		Size: 2.8 MB (2789161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d6af1a94baa95c219eaba2db2fb27e299572ac8d2859e1399838abdccae784c`  
		Last Modified: Wed, 20 Apr 2022 12:53:11 GMT  
		Size: 68.6 MB (68568946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec0646bfa3d97be6f7515ad03d0cbb859adebe6cf3785cf1d36d06c8aa3f224`  
		Last Modified: Wed, 20 Apr 2022 12:54:22 GMT  
		Size: 142.5 MB (142538405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0` - linux; ppc64le

```console
$ docker pull mono@sha256:abb2d6df6d771036e5878f2d8d5f7be07336dc420c2f33f5cbcd387ff20e7215
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.6 MB (203607651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d706be5bbbd80d2cfe56b5ed3350e0a17769f9e9c5ce4ee417df1efdd40f9f5d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 09:47:47 GMT
ADD file:69078e7ae6d887f7e36ae048f98f784678fbd8b7a8ec27e3c2bce0d68a47236d in / 
# Wed, 20 Apr 2022 09:47:51 GMT
CMD ["bash"]
# Thu, 21 Apr 2022 08:14:20 GMT
ENV MONO_VERSION=6.12.0.122
# Thu, 21 Apr 2022 08:15:04 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 21 Apr 2022 08:16:01 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 21 Apr 2022 08:25:53 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1aacfa28cbcef999a852ce9c261b67f15f0ccd8450cd1dbfe7b0dc88e6b5aba2`  
		Last Modified: Wed, 20 Apr 2022 09:58:02 GMT  
		Size: 30.6 MB (30560296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b4fd6959397baa971e32512d4c0d1d094bea59e1bf9b3442d8a345c6f7cd81`  
		Last Modified: Thu, 21 Apr 2022 08:33:06 GMT  
		Size: 2.9 MB (2892563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff24986d59f2106922e32fbd04b151763111155f6440aa41d390cbab27fca8c8`  
		Last Modified: Thu, 21 Apr 2022 08:33:11 GMT  
		Size: 26.9 MB (26873691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c14de3289c90efbcb5ba56806674834ab22b34135aa29d559635cdfb7805907`  
		Last Modified: Thu, 21 Apr 2022 08:34:20 GMT  
		Size: 143.3 MB (143281101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.12.0-slim`

```console
$ docker pull mono@sha256:df384bda4d7d65b1fc3842d0eaa6d5bb7d188c95f274e7cc8403b002c6ec8b82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.12.0-slim` - linux; amd64

```console
$ docker pull mono@sha256:f0d95c21aa0a9490ae955fe78fc0f316616807db95b5790b5cd7b4391ac8568d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94677375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4291e2c603690115cbb2d33ea0dee4ab69b47aa89201a4fc53d449bd5c5e9d02`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:48 GMT
ADD file:011a43ee23214c201afb7f3b5be592f374b89a4c71aea82ca66146bbbc31b959 in / 
# Wed, 20 Apr 2022 04:43:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 15:27:27 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 15:27:35 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 15:27:54 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4be315f6562fccf08fd6c749557e31e45ab6d987370e20e2c4933ddb04ddd5ff`  
		Last Modified: Wed, 20 Apr 2022 04:49:15 GMT  
		Size: 27.1 MB (27140664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20d9f7ad1a1561508daa15f30ed450e8279f8633fc277a84bd6f5b1d00ecf314`  
		Last Modified: Wed, 20 Apr 2022 15:39:01 GMT  
		Size: 2.8 MB (2777363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4214d10d224872d47c1c108360a2890678eff5f2e288cdefa4f0882ac8ff9e46`  
		Last Modified: Wed, 20 Apr 2022 15:39:10 GMT  
		Size: 64.8 MB (64759348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:c3b087e497272a1ff39fc23bc98d4fe778bf411c3c00de946f43fe57cd6e9d50
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51850130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03bf635a6d765f56a65311bc43513ec14a0451754d992adcadcf3c7f67503ca8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:17:47 GMT
ADD file:5b740716d202d2f3494df5e108c0ba999125920ed9c97803fe0ccdfeba5cf518 in / 
# Wed, 20 Apr 2022 07:17:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 13:45:59 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 13:46:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 13:47:13 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1fc8704cfa531d4583c5d4d571b836a82c02a812dae88792c4397cf1c1770405`  
		Last Modified: Wed, 20 Apr 2022 07:33:54 GMT  
		Size: 24.9 MB (24889592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de67cfe4308dcefca53d406cca104b0f4db6a1d2dda37929256a8f8761e5550a`  
		Last Modified: Wed, 20 Apr 2022 13:56:57 GMT  
		Size: 2.5 MB (2467647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641f8380b2823093df874b2b79c65d2f31452f99f5896f56a17614cbcb1dc971`  
		Last Modified: Wed, 20 Apr 2022 13:57:13 GMT  
		Size: 24.5 MB (24492891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:faff62d5274b7437f4216c427da824165d03a1c90c7c0f79e08533937b868eee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48897299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:659c685d861a835af511fa1dc5758b62d34b1e713f3db36f2e4f3d1cc184057c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 13:28:26 GMT
ADD file:2a755b6e7bf01ec959b8bb848b6d46f292821a0bf08e04d565991ec4bdbea029 in / 
# Wed, 20 Apr 2022 13:28:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 22:05:17 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 22:05:41 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 22:06:24 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:88467ac22b4358b1b60009f6332ba9e12b7a82a36bef334d91d68dbf8b58d96f`  
		Last Modified: Wed, 20 Apr 2022 13:45:04 GMT  
		Size: 22.7 MB (22747865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e27b3994c35244605adec982fe00db7376f48e5ec599c253a2465ef79124c80`  
		Last Modified: Wed, 20 Apr 2022 22:15:27 GMT  
		Size: 2.4 MB (2366878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8554905d57c581805a8fc875940e3e39baa10f0bbc841e4b1f192d1c968eafc2`  
		Last Modified: Wed, 20 Apr 2022 22:15:44 GMT  
		Size: 23.8 MB (23782556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:0f3837c80f89d4cc61d33d11680310dd7b9170aa4a20287829db1cf4ff83169c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57867773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a03207fd5f3c9c31e878dec4d955581897e75177774ac4915f726360915f8e8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:36 GMT
ADD file:5de4397c1295f7249c93907be599d96efbd9cd25909340d245ec8d1c9770f444 in / 
# Wed, 20 Apr 2022 04:29:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 09:34:15 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 09:34:25 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 09:34:40 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:6c3e5b218d6477ff77053280968d5bdeaa5dcf16a803e917d98dd0ea8b93ac82`  
		Last Modified: Wed, 20 Apr 2022 04:36:38 GMT  
		Size: 25.9 MB (25908349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5583d434a71d4775ae033dd3567325a5f5d01a34ff9f805631b17426570d60`  
		Last Modified: Wed, 20 Apr 2022 09:38:16 GMT  
		Size: 2.6 MB (2641065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1df7a4f3775402176b947b2ffb1f930879581b64904846f29bd8e5aa4000e4d`  
		Last Modified: Wed, 20 Apr 2022 09:38:20 GMT  
		Size: 29.3 MB (29318359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0-slim` - linux; 386

```console
$ docker pull mono@sha256:a620c36d6b438c94797eaa6b17b2452369ac55ab8a59a1bcf8b4501df1eea0c5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99157932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95ff55aea4f3ffc1da74cea929a23a78ed6dc8901847098c5878018368c9da5d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:38:03 GMT
ADD file:602a25173054242f635a5a299845b7f1b56864ac5d3b8af1ae29dec3a9da119f in / 
# Wed, 20 Apr 2022 07:38:04 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:49:08 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 12:49:17 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 12:49:40 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a13b13d818745c4d2234aab71df26e4a01bfe59f396ab62f20d156b94803650c`  
		Last Modified: Wed, 20 Apr 2022 07:45:46 GMT  
		Size: 27.8 MB (27799825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc07624832ff4b064bd2b3797a6774618e27f4c3a1e24419874628eeb613e7ba`  
		Last Modified: Wed, 20 Apr 2022 12:53:02 GMT  
		Size: 2.8 MB (2789161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d6af1a94baa95c219eaba2db2fb27e299572ac8d2859e1399838abdccae784c`  
		Last Modified: Wed, 20 Apr 2022 12:53:11 GMT  
		Size: 68.6 MB (68568946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:13e28a240194ffdaa1ab1b8b10b807978db6ed7eec8e4d427b0ff2c6d38130b8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.3 MB (60326550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:806eebb6c6b16141507ab480ab6238efd982bbe9375a51cabbc00f5cd2fa62b5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 09:47:47 GMT
ADD file:69078e7ae6d887f7e36ae048f98f784678fbd8b7a8ec27e3c2bce0d68a47236d in / 
# Wed, 20 Apr 2022 09:47:51 GMT
CMD ["bash"]
# Thu, 21 Apr 2022 08:14:20 GMT
ENV MONO_VERSION=6.12.0.122
# Thu, 21 Apr 2022 08:15:04 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 21 Apr 2022 08:16:01 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1aacfa28cbcef999a852ce9c261b67f15f0ccd8450cd1dbfe7b0dc88e6b5aba2`  
		Last Modified: Wed, 20 Apr 2022 09:58:02 GMT  
		Size: 30.6 MB (30560296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b4fd6959397baa971e32512d4c0d1d094bea59e1bf9b3442d8a345c6f7cd81`  
		Last Modified: Thu, 21 Apr 2022 08:33:06 GMT  
		Size: 2.9 MB (2892563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff24986d59f2106922e32fbd04b151763111155f6440aa41d390cbab27fca8c8`  
		Last Modified: Thu, 21 Apr 2022 08:33:11 GMT  
		Size: 26.9 MB (26873691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.12.0.122`

```console
$ docker pull mono@sha256:8e6aa0dc91a317d6b4ada45be67e01948c3b620226538928a4374ccea987abbc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.12.0.122` - linux; amd64

```console
$ docker pull mono@sha256:0c36486cbda2ab995af85a2e9bbe62cc56bd2cf77d030fb67c3c228c920d74cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.1 MB (236125631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a50ead981e57279bc2232fe42e0e534ddd348365a0df2aa9f7a6ea1043c1412e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:48 GMT
ADD file:011a43ee23214c201afb7f3b5be592f374b89a4c71aea82ca66146bbbc31b959 in / 
# Wed, 20 Apr 2022 04:43:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 15:27:27 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 15:27:35 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 15:27:54 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 20 Apr 2022 15:33:01 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4be315f6562fccf08fd6c749557e31e45ab6d987370e20e2c4933ddb04ddd5ff`  
		Last Modified: Wed, 20 Apr 2022 04:49:15 GMT  
		Size: 27.1 MB (27140664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20d9f7ad1a1561508daa15f30ed450e8279f8633fc277a84bd6f5b1d00ecf314`  
		Last Modified: Wed, 20 Apr 2022 15:39:01 GMT  
		Size: 2.8 MB (2777363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4214d10d224872d47c1c108360a2890678eff5f2e288cdefa4f0882ac8ff9e46`  
		Last Modified: Wed, 20 Apr 2022 15:39:10 GMT  
		Size: 64.8 MB (64759348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa0a929eb8545fe353e58ddc4af329eefbe9e50f63bbbf938d0256d77246e6a`  
		Last Modified: Wed, 20 Apr 2022 15:40:09 GMT  
		Size: 141.4 MB (141448256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.122` - linux; arm variant v5

```console
$ docker pull mono@sha256:258511710254d92fe26e82049f226a7e527f0ed49778129c70646e9fc329af2a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.0 MB (191957036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac351dfd94cc0f2249f8760f8fedebcc5a814cdd11a7bef18de24f24f52c37fa`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:17:47 GMT
ADD file:5b740716d202d2f3494df5e108c0ba999125920ed9c97803fe0ccdfeba5cf518 in / 
# Wed, 20 Apr 2022 07:17:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 13:45:59 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 13:46:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 13:47:13 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 20 Apr 2022 13:52:09 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1fc8704cfa531d4583c5d4d571b836a82c02a812dae88792c4397cf1c1770405`  
		Last Modified: Wed, 20 Apr 2022 07:33:54 GMT  
		Size: 24.9 MB (24889592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de67cfe4308dcefca53d406cca104b0f4db6a1d2dda37929256a8f8761e5550a`  
		Last Modified: Wed, 20 Apr 2022 13:56:57 GMT  
		Size: 2.5 MB (2467647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641f8380b2823093df874b2b79c65d2f31452f99f5896f56a17614cbcb1dc971`  
		Last Modified: Wed, 20 Apr 2022 13:57:13 GMT  
		Size: 24.5 MB (24492891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68839de10302780399729e3999eb88f5e1ed8ca5c135b146dbb11f63aa458dfa`  
		Last Modified: Wed, 20 Apr 2022 13:59:38 GMT  
		Size: 140.1 MB (140106906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.122` - linux; arm variant v7

```console
$ docker pull mono@sha256:ad3a93a04d11ffb9206df13b87aa8a10890bc78b826eef7fbbbb160387b29507
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.9 MB (187864260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c65447e8e52004d2ac80a42c301fd6f3eb5fe6898ca081f77decd51bed084fc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 13:28:26 GMT
ADD file:2a755b6e7bf01ec959b8bb848b6d46f292821a0bf08e04d565991ec4bdbea029 in / 
# Wed, 20 Apr 2022 13:28:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 22:05:17 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 22:05:41 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 22:06:24 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 20 Apr 2022 22:10:56 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:88467ac22b4358b1b60009f6332ba9e12b7a82a36bef334d91d68dbf8b58d96f`  
		Last Modified: Wed, 20 Apr 2022 13:45:04 GMT  
		Size: 22.7 MB (22747865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e27b3994c35244605adec982fe00db7376f48e5ec599c253a2465ef79124c80`  
		Last Modified: Wed, 20 Apr 2022 22:15:27 GMT  
		Size: 2.4 MB (2366878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8554905d57c581805a8fc875940e3e39baa10f0bbc841e4b1f192d1c968eafc2`  
		Last Modified: Wed, 20 Apr 2022 22:15:44 GMT  
		Size: 23.8 MB (23782556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b332d3b0da4d9e0bbb73a313bd1158fad6ed98c34ac243e90a2b37dcdac08e4`  
		Last Modified: Wed, 20 Apr 2022 22:18:18 GMT  
		Size: 139.0 MB (138966961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.122` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:617fd6f5ff9238ff8782c0b154f5fbb1e51864ad1f009da0d0c5fcd54ff179c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.5 MB (214465680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:721976153f55a700a3368032ce347eb3ae7b930fc6151b879332e0e99f1ca0cc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:36 GMT
ADD file:5de4397c1295f7249c93907be599d96efbd9cd25909340d245ec8d1c9770f444 in / 
# Wed, 20 Apr 2022 04:29:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 09:34:15 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 09:34:25 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 09:34:40 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 20 Apr 2022 09:36:17 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:6c3e5b218d6477ff77053280968d5bdeaa5dcf16a803e917d98dd0ea8b93ac82`  
		Last Modified: Wed, 20 Apr 2022 04:36:38 GMT  
		Size: 25.9 MB (25908349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5583d434a71d4775ae033dd3567325a5f5d01a34ff9f805631b17426570d60`  
		Last Modified: Wed, 20 Apr 2022 09:38:16 GMT  
		Size: 2.6 MB (2641065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1df7a4f3775402176b947b2ffb1f930879581b64904846f29bd8e5aa4000e4d`  
		Last Modified: Wed, 20 Apr 2022 09:38:20 GMT  
		Size: 29.3 MB (29318359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f80c1eac9d435a1e808ae3c8eaf8a76d9e653e54edc1090cf4c2fc47f29f6e`  
		Last Modified: Wed, 20 Apr 2022 09:39:21 GMT  
		Size: 156.6 MB (156597907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.122` - linux; 386

```console
$ docker pull mono@sha256:ef781f5c402c37c294ccf7397654b6a780c16c68ab05b1ee598260446e0049b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.7 MB (241696337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:faa267e26ab7e853336277f2575154ad396b6536c3cd9e8ba22824250ccc6fbd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:38:03 GMT
ADD file:602a25173054242f635a5a299845b7f1b56864ac5d3b8af1ae29dec3a9da119f in / 
# Wed, 20 Apr 2022 07:38:04 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:49:08 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 12:49:17 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 12:49:40 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 20 Apr 2022 12:51:19 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a13b13d818745c4d2234aab71df26e4a01bfe59f396ab62f20d156b94803650c`  
		Last Modified: Wed, 20 Apr 2022 07:45:46 GMT  
		Size: 27.8 MB (27799825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc07624832ff4b064bd2b3797a6774618e27f4c3a1e24419874628eeb613e7ba`  
		Last Modified: Wed, 20 Apr 2022 12:53:02 GMT  
		Size: 2.8 MB (2789161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d6af1a94baa95c219eaba2db2fb27e299572ac8d2859e1399838abdccae784c`  
		Last Modified: Wed, 20 Apr 2022 12:53:11 GMT  
		Size: 68.6 MB (68568946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec0646bfa3d97be6f7515ad03d0cbb859adebe6cf3785cf1d36d06c8aa3f224`  
		Last Modified: Wed, 20 Apr 2022 12:54:22 GMT  
		Size: 142.5 MB (142538405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.122` - linux; ppc64le

```console
$ docker pull mono@sha256:abb2d6df6d771036e5878f2d8d5f7be07336dc420c2f33f5cbcd387ff20e7215
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.6 MB (203607651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d706be5bbbd80d2cfe56b5ed3350e0a17769f9e9c5ce4ee417df1efdd40f9f5d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 09:47:47 GMT
ADD file:69078e7ae6d887f7e36ae048f98f784678fbd8b7a8ec27e3c2bce0d68a47236d in / 
# Wed, 20 Apr 2022 09:47:51 GMT
CMD ["bash"]
# Thu, 21 Apr 2022 08:14:20 GMT
ENV MONO_VERSION=6.12.0.122
# Thu, 21 Apr 2022 08:15:04 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 21 Apr 2022 08:16:01 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 21 Apr 2022 08:25:53 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1aacfa28cbcef999a852ce9c261b67f15f0ccd8450cd1dbfe7b0dc88e6b5aba2`  
		Last Modified: Wed, 20 Apr 2022 09:58:02 GMT  
		Size: 30.6 MB (30560296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b4fd6959397baa971e32512d4c0d1d094bea59e1bf9b3442d8a345c6f7cd81`  
		Last Modified: Thu, 21 Apr 2022 08:33:06 GMT  
		Size: 2.9 MB (2892563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff24986d59f2106922e32fbd04b151763111155f6440aa41d390cbab27fca8c8`  
		Last Modified: Thu, 21 Apr 2022 08:33:11 GMT  
		Size: 26.9 MB (26873691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c14de3289c90efbcb5ba56806674834ab22b34135aa29d559635cdfb7805907`  
		Last Modified: Thu, 21 Apr 2022 08:34:20 GMT  
		Size: 143.3 MB (143281101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.12.0.122-slim`

```console
$ docker pull mono@sha256:df384bda4d7d65b1fc3842d0eaa6d5bb7d188c95f274e7cc8403b002c6ec8b82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.12.0.122-slim` - linux; amd64

```console
$ docker pull mono@sha256:f0d95c21aa0a9490ae955fe78fc0f316616807db95b5790b5cd7b4391ac8568d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94677375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4291e2c603690115cbb2d33ea0dee4ab69b47aa89201a4fc53d449bd5c5e9d02`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:48 GMT
ADD file:011a43ee23214c201afb7f3b5be592f374b89a4c71aea82ca66146bbbc31b959 in / 
# Wed, 20 Apr 2022 04:43:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 15:27:27 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 15:27:35 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 15:27:54 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4be315f6562fccf08fd6c749557e31e45ab6d987370e20e2c4933ddb04ddd5ff`  
		Last Modified: Wed, 20 Apr 2022 04:49:15 GMT  
		Size: 27.1 MB (27140664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20d9f7ad1a1561508daa15f30ed450e8279f8633fc277a84bd6f5b1d00ecf314`  
		Last Modified: Wed, 20 Apr 2022 15:39:01 GMT  
		Size: 2.8 MB (2777363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4214d10d224872d47c1c108360a2890678eff5f2e288cdefa4f0882ac8ff9e46`  
		Last Modified: Wed, 20 Apr 2022 15:39:10 GMT  
		Size: 64.8 MB (64759348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.122-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:c3b087e497272a1ff39fc23bc98d4fe778bf411c3c00de946f43fe57cd6e9d50
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51850130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03bf635a6d765f56a65311bc43513ec14a0451754d992adcadcf3c7f67503ca8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:17:47 GMT
ADD file:5b740716d202d2f3494df5e108c0ba999125920ed9c97803fe0ccdfeba5cf518 in / 
# Wed, 20 Apr 2022 07:17:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 13:45:59 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 13:46:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 13:47:13 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1fc8704cfa531d4583c5d4d571b836a82c02a812dae88792c4397cf1c1770405`  
		Last Modified: Wed, 20 Apr 2022 07:33:54 GMT  
		Size: 24.9 MB (24889592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de67cfe4308dcefca53d406cca104b0f4db6a1d2dda37929256a8f8761e5550a`  
		Last Modified: Wed, 20 Apr 2022 13:56:57 GMT  
		Size: 2.5 MB (2467647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641f8380b2823093df874b2b79c65d2f31452f99f5896f56a17614cbcb1dc971`  
		Last Modified: Wed, 20 Apr 2022 13:57:13 GMT  
		Size: 24.5 MB (24492891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.122-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:faff62d5274b7437f4216c427da824165d03a1c90c7c0f79e08533937b868eee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48897299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:659c685d861a835af511fa1dc5758b62d34b1e713f3db36f2e4f3d1cc184057c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 13:28:26 GMT
ADD file:2a755b6e7bf01ec959b8bb848b6d46f292821a0bf08e04d565991ec4bdbea029 in / 
# Wed, 20 Apr 2022 13:28:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 22:05:17 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 22:05:41 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 22:06:24 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:88467ac22b4358b1b60009f6332ba9e12b7a82a36bef334d91d68dbf8b58d96f`  
		Last Modified: Wed, 20 Apr 2022 13:45:04 GMT  
		Size: 22.7 MB (22747865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e27b3994c35244605adec982fe00db7376f48e5ec599c253a2465ef79124c80`  
		Last Modified: Wed, 20 Apr 2022 22:15:27 GMT  
		Size: 2.4 MB (2366878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8554905d57c581805a8fc875940e3e39baa10f0bbc841e4b1f192d1c968eafc2`  
		Last Modified: Wed, 20 Apr 2022 22:15:44 GMT  
		Size: 23.8 MB (23782556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.122-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:0f3837c80f89d4cc61d33d11680310dd7b9170aa4a20287829db1cf4ff83169c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57867773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a03207fd5f3c9c31e878dec4d955581897e75177774ac4915f726360915f8e8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:36 GMT
ADD file:5de4397c1295f7249c93907be599d96efbd9cd25909340d245ec8d1c9770f444 in / 
# Wed, 20 Apr 2022 04:29:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 09:34:15 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 09:34:25 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 09:34:40 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:6c3e5b218d6477ff77053280968d5bdeaa5dcf16a803e917d98dd0ea8b93ac82`  
		Last Modified: Wed, 20 Apr 2022 04:36:38 GMT  
		Size: 25.9 MB (25908349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5583d434a71d4775ae033dd3567325a5f5d01a34ff9f805631b17426570d60`  
		Last Modified: Wed, 20 Apr 2022 09:38:16 GMT  
		Size: 2.6 MB (2641065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1df7a4f3775402176b947b2ffb1f930879581b64904846f29bd8e5aa4000e4d`  
		Last Modified: Wed, 20 Apr 2022 09:38:20 GMT  
		Size: 29.3 MB (29318359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.122-slim` - linux; 386

```console
$ docker pull mono@sha256:a620c36d6b438c94797eaa6b17b2452369ac55ab8a59a1bcf8b4501df1eea0c5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99157932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95ff55aea4f3ffc1da74cea929a23a78ed6dc8901847098c5878018368c9da5d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:38:03 GMT
ADD file:602a25173054242f635a5a299845b7f1b56864ac5d3b8af1ae29dec3a9da119f in / 
# Wed, 20 Apr 2022 07:38:04 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:49:08 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 12:49:17 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 12:49:40 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a13b13d818745c4d2234aab71df26e4a01bfe59f396ab62f20d156b94803650c`  
		Last Modified: Wed, 20 Apr 2022 07:45:46 GMT  
		Size: 27.8 MB (27799825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc07624832ff4b064bd2b3797a6774618e27f4c3a1e24419874628eeb613e7ba`  
		Last Modified: Wed, 20 Apr 2022 12:53:02 GMT  
		Size: 2.8 MB (2789161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d6af1a94baa95c219eaba2db2fb27e299572ac8d2859e1399838abdccae784c`  
		Last Modified: Wed, 20 Apr 2022 12:53:11 GMT  
		Size: 68.6 MB (68568946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.122-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:13e28a240194ffdaa1ab1b8b10b807978db6ed7eec8e4d427b0ff2c6d38130b8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.3 MB (60326550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:806eebb6c6b16141507ab480ab6238efd982bbe9375a51cabbc00f5cd2fa62b5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 09:47:47 GMT
ADD file:69078e7ae6d887f7e36ae048f98f784678fbd8b7a8ec27e3c2bce0d68a47236d in / 
# Wed, 20 Apr 2022 09:47:51 GMT
CMD ["bash"]
# Thu, 21 Apr 2022 08:14:20 GMT
ENV MONO_VERSION=6.12.0.122
# Thu, 21 Apr 2022 08:15:04 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 21 Apr 2022 08:16:01 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1aacfa28cbcef999a852ce9c261b67f15f0ccd8450cd1dbfe7b0dc88e6b5aba2`  
		Last Modified: Wed, 20 Apr 2022 09:58:02 GMT  
		Size: 30.6 MB (30560296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b4fd6959397baa971e32512d4c0d1d094bea59e1bf9b3442d8a345c6f7cd81`  
		Last Modified: Thu, 21 Apr 2022 08:33:06 GMT  
		Size: 2.9 MB (2892563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff24986d59f2106922e32fbd04b151763111155f6440aa41d390cbab27fca8c8`  
		Last Modified: Thu, 21 Apr 2022 08:33:11 GMT  
		Size: 26.9 MB (26873691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:latest`

```console
$ docker pull mono@sha256:8e6aa0dc91a317d6b4ada45be67e01948c3b620226538928a4374ccea987abbc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:latest` - linux; amd64

```console
$ docker pull mono@sha256:0c36486cbda2ab995af85a2e9bbe62cc56bd2cf77d030fb67c3c228c920d74cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.1 MB (236125631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a50ead981e57279bc2232fe42e0e534ddd348365a0df2aa9f7a6ea1043c1412e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:48 GMT
ADD file:011a43ee23214c201afb7f3b5be592f374b89a4c71aea82ca66146bbbc31b959 in / 
# Wed, 20 Apr 2022 04:43:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 15:27:27 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 15:27:35 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 15:27:54 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 20 Apr 2022 15:33:01 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4be315f6562fccf08fd6c749557e31e45ab6d987370e20e2c4933ddb04ddd5ff`  
		Last Modified: Wed, 20 Apr 2022 04:49:15 GMT  
		Size: 27.1 MB (27140664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20d9f7ad1a1561508daa15f30ed450e8279f8633fc277a84bd6f5b1d00ecf314`  
		Last Modified: Wed, 20 Apr 2022 15:39:01 GMT  
		Size: 2.8 MB (2777363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4214d10d224872d47c1c108360a2890678eff5f2e288cdefa4f0882ac8ff9e46`  
		Last Modified: Wed, 20 Apr 2022 15:39:10 GMT  
		Size: 64.8 MB (64759348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa0a929eb8545fe353e58ddc4af329eefbe9e50f63bbbf938d0256d77246e6a`  
		Last Modified: Wed, 20 Apr 2022 15:40:09 GMT  
		Size: 141.4 MB (141448256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm variant v5

```console
$ docker pull mono@sha256:258511710254d92fe26e82049f226a7e527f0ed49778129c70646e9fc329af2a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.0 MB (191957036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac351dfd94cc0f2249f8760f8fedebcc5a814cdd11a7bef18de24f24f52c37fa`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:17:47 GMT
ADD file:5b740716d202d2f3494df5e108c0ba999125920ed9c97803fe0ccdfeba5cf518 in / 
# Wed, 20 Apr 2022 07:17:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 13:45:59 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 13:46:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 13:47:13 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 20 Apr 2022 13:52:09 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1fc8704cfa531d4583c5d4d571b836a82c02a812dae88792c4397cf1c1770405`  
		Last Modified: Wed, 20 Apr 2022 07:33:54 GMT  
		Size: 24.9 MB (24889592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de67cfe4308dcefca53d406cca104b0f4db6a1d2dda37929256a8f8761e5550a`  
		Last Modified: Wed, 20 Apr 2022 13:56:57 GMT  
		Size: 2.5 MB (2467647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641f8380b2823093df874b2b79c65d2f31452f99f5896f56a17614cbcb1dc971`  
		Last Modified: Wed, 20 Apr 2022 13:57:13 GMT  
		Size: 24.5 MB (24492891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68839de10302780399729e3999eb88f5e1ed8ca5c135b146dbb11f63aa458dfa`  
		Last Modified: Wed, 20 Apr 2022 13:59:38 GMT  
		Size: 140.1 MB (140106906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm variant v7

```console
$ docker pull mono@sha256:ad3a93a04d11ffb9206df13b87aa8a10890bc78b826eef7fbbbb160387b29507
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.9 MB (187864260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c65447e8e52004d2ac80a42c301fd6f3eb5fe6898ca081f77decd51bed084fc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 13:28:26 GMT
ADD file:2a755b6e7bf01ec959b8bb848b6d46f292821a0bf08e04d565991ec4bdbea029 in / 
# Wed, 20 Apr 2022 13:28:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 22:05:17 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 22:05:41 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 22:06:24 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 20 Apr 2022 22:10:56 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:88467ac22b4358b1b60009f6332ba9e12b7a82a36bef334d91d68dbf8b58d96f`  
		Last Modified: Wed, 20 Apr 2022 13:45:04 GMT  
		Size: 22.7 MB (22747865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e27b3994c35244605adec982fe00db7376f48e5ec599c253a2465ef79124c80`  
		Last Modified: Wed, 20 Apr 2022 22:15:27 GMT  
		Size: 2.4 MB (2366878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8554905d57c581805a8fc875940e3e39baa10f0bbc841e4b1f192d1c968eafc2`  
		Last Modified: Wed, 20 Apr 2022 22:15:44 GMT  
		Size: 23.8 MB (23782556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b332d3b0da4d9e0bbb73a313bd1158fad6ed98c34ac243e90a2b37dcdac08e4`  
		Last Modified: Wed, 20 Apr 2022 22:18:18 GMT  
		Size: 139.0 MB (138966961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:617fd6f5ff9238ff8782c0b154f5fbb1e51864ad1f009da0d0c5fcd54ff179c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.5 MB (214465680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:721976153f55a700a3368032ce347eb3ae7b930fc6151b879332e0e99f1ca0cc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:36 GMT
ADD file:5de4397c1295f7249c93907be599d96efbd9cd25909340d245ec8d1c9770f444 in / 
# Wed, 20 Apr 2022 04:29:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 09:34:15 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 09:34:25 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 09:34:40 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 20 Apr 2022 09:36:17 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:6c3e5b218d6477ff77053280968d5bdeaa5dcf16a803e917d98dd0ea8b93ac82`  
		Last Modified: Wed, 20 Apr 2022 04:36:38 GMT  
		Size: 25.9 MB (25908349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5583d434a71d4775ae033dd3567325a5f5d01a34ff9f805631b17426570d60`  
		Last Modified: Wed, 20 Apr 2022 09:38:16 GMT  
		Size: 2.6 MB (2641065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1df7a4f3775402176b947b2ffb1f930879581b64904846f29bd8e5aa4000e4d`  
		Last Modified: Wed, 20 Apr 2022 09:38:20 GMT  
		Size: 29.3 MB (29318359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f80c1eac9d435a1e808ae3c8eaf8a76d9e653e54edc1090cf4c2fc47f29f6e`  
		Last Modified: Wed, 20 Apr 2022 09:39:21 GMT  
		Size: 156.6 MB (156597907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; 386

```console
$ docker pull mono@sha256:ef781f5c402c37c294ccf7397654b6a780c16c68ab05b1ee598260446e0049b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.7 MB (241696337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:faa267e26ab7e853336277f2575154ad396b6536c3cd9e8ba22824250ccc6fbd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:38:03 GMT
ADD file:602a25173054242f635a5a299845b7f1b56864ac5d3b8af1ae29dec3a9da119f in / 
# Wed, 20 Apr 2022 07:38:04 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:49:08 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 12:49:17 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 12:49:40 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 20 Apr 2022 12:51:19 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a13b13d818745c4d2234aab71df26e4a01bfe59f396ab62f20d156b94803650c`  
		Last Modified: Wed, 20 Apr 2022 07:45:46 GMT  
		Size: 27.8 MB (27799825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc07624832ff4b064bd2b3797a6774618e27f4c3a1e24419874628eeb613e7ba`  
		Last Modified: Wed, 20 Apr 2022 12:53:02 GMT  
		Size: 2.8 MB (2789161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d6af1a94baa95c219eaba2db2fb27e299572ac8d2859e1399838abdccae784c`  
		Last Modified: Wed, 20 Apr 2022 12:53:11 GMT  
		Size: 68.6 MB (68568946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec0646bfa3d97be6f7515ad03d0cbb859adebe6cf3785cf1d36d06c8aa3f224`  
		Last Modified: Wed, 20 Apr 2022 12:54:22 GMT  
		Size: 142.5 MB (142538405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; ppc64le

```console
$ docker pull mono@sha256:abb2d6df6d771036e5878f2d8d5f7be07336dc420c2f33f5cbcd387ff20e7215
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.6 MB (203607651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d706be5bbbd80d2cfe56b5ed3350e0a17769f9e9c5ce4ee417df1efdd40f9f5d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 09:47:47 GMT
ADD file:69078e7ae6d887f7e36ae048f98f784678fbd8b7a8ec27e3c2bce0d68a47236d in / 
# Wed, 20 Apr 2022 09:47:51 GMT
CMD ["bash"]
# Thu, 21 Apr 2022 08:14:20 GMT
ENV MONO_VERSION=6.12.0.122
# Thu, 21 Apr 2022 08:15:04 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 21 Apr 2022 08:16:01 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 21 Apr 2022 08:25:53 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1aacfa28cbcef999a852ce9c261b67f15f0ccd8450cd1dbfe7b0dc88e6b5aba2`  
		Last Modified: Wed, 20 Apr 2022 09:58:02 GMT  
		Size: 30.6 MB (30560296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b4fd6959397baa971e32512d4c0d1d094bea59e1bf9b3442d8a345c6f7cd81`  
		Last Modified: Thu, 21 Apr 2022 08:33:06 GMT  
		Size: 2.9 MB (2892563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff24986d59f2106922e32fbd04b151763111155f6440aa41d390cbab27fca8c8`  
		Last Modified: Thu, 21 Apr 2022 08:33:11 GMT  
		Size: 26.9 MB (26873691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c14de3289c90efbcb5ba56806674834ab22b34135aa29d559635cdfb7805907`  
		Last Modified: Thu, 21 Apr 2022 08:34:20 GMT  
		Size: 143.3 MB (143281101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:slim`

```console
$ docker pull mono@sha256:df384bda4d7d65b1fc3842d0eaa6d5bb7d188c95f274e7cc8403b002c6ec8b82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:slim` - linux; amd64

```console
$ docker pull mono@sha256:f0d95c21aa0a9490ae955fe78fc0f316616807db95b5790b5cd7b4391ac8568d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94677375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4291e2c603690115cbb2d33ea0dee4ab69b47aa89201a4fc53d449bd5c5e9d02`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:48 GMT
ADD file:011a43ee23214c201afb7f3b5be592f374b89a4c71aea82ca66146bbbc31b959 in / 
# Wed, 20 Apr 2022 04:43:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 15:27:27 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 15:27:35 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 15:27:54 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4be315f6562fccf08fd6c749557e31e45ab6d987370e20e2c4933ddb04ddd5ff`  
		Last Modified: Wed, 20 Apr 2022 04:49:15 GMT  
		Size: 27.1 MB (27140664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20d9f7ad1a1561508daa15f30ed450e8279f8633fc277a84bd6f5b1d00ecf314`  
		Last Modified: Wed, 20 Apr 2022 15:39:01 GMT  
		Size: 2.8 MB (2777363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4214d10d224872d47c1c108360a2890678eff5f2e288cdefa4f0882ac8ff9e46`  
		Last Modified: Wed, 20 Apr 2022 15:39:10 GMT  
		Size: 64.8 MB (64759348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:c3b087e497272a1ff39fc23bc98d4fe778bf411c3c00de946f43fe57cd6e9d50
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51850130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03bf635a6d765f56a65311bc43513ec14a0451754d992adcadcf3c7f67503ca8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:17:47 GMT
ADD file:5b740716d202d2f3494df5e108c0ba999125920ed9c97803fe0ccdfeba5cf518 in / 
# Wed, 20 Apr 2022 07:17:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 13:45:59 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 13:46:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 13:47:13 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1fc8704cfa531d4583c5d4d571b836a82c02a812dae88792c4397cf1c1770405`  
		Last Modified: Wed, 20 Apr 2022 07:33:54 GMT  
		Size: 24.9 MB (24889592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de67cfe4308dcefca53d406cca104b0f4db6a1d2dda37929256a8f8761e5550a`  
		Last Modified: Wed, 20 Apr 2022 13:56:57 GMT  
		Size: 2.5 MB (2467647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641f8380b2823093df874b2b79c65d2f31452f99f5896f56a17614cbcb1dc971`  
		Last Modified: Wed, 20 Apr 2022 13:57:13 GMT  
		Size: 24.5 MB (24492891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:faff62d5274b7437f4216c427da824165d03a1c90c7c0f79e08533937b868eee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48897299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:659c685d861a835af511fa1dc5758b62d34b1e713f3db36f2e4f3d1cc184057c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 13:28:26 GMT
ADD file:2a755b6e7bf01ec959b8bb848b6d46f292821a0bf08e04d565991ec4bdbea029 in / 
# Wed, 20 Apr 2022 13:28:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 22:05:17 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 22:05:41 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 22:06:24 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:88467ac22b4358b1b60009f6332ba9e12b7a82a36bef334d91d68dbf8b58d96f`  
		Last Modified: Wed, 20 Apr 2022 13:45:04 GMT  
		Size: 22.7 MB (22747865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e27b3994c35244605adec982fe00db7376f48e5ec599c253a2465ef79124c80`  
		Last Modified: Wed, 20 Apr 2022 22:15:27 GMT  
		Size: 2.4 MB (2366878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8554905d57c581805a8fc875940e3e39baa10f0bbc841e4b1f192d1c968eafc2`  
		Last Modified: Wed, 20 Apr 2022 22:15:44 GMT  
		Size: 23.8 MB (23782556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:0f3837c80f89d4cc61d33d11680310dd7b9170aa4a20287829db1cf4ff83169c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57867773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a03207fd5f3c9c31e878dec4d955581897e75177774ac4915f726360915f8e8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:36 GMT
ADD file:5de4397c1295f7249c93907be599d96efbd9cd25909340d245ec8d1c9770f444 in / 
# Wed, 20 Apr 2022 04:29:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 09:34:15 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 09:34:25 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 09:34:40 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:6c3e5b218d6477ff77053280968d5bdeaa5dcf16a803e917d98dd0ea8b93ac82`  
		Last Modified: Wed, 20 Apr 2022 04:36:38 GMT  
		Size: 25.9 MB (25908349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5583d434a71d4775ae033dd3567325a5f5d01a34ff9f805631b17426570d60`  
		Last Modified: Wed, 20 Apr 2022 09:38:16 GMT  
		Size: 2.6 MB (2641065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1df7a4f3775402176b947b2ffb1f930879581b64904846f29bd8e5aa4000e4d`  
		Last Modified: Wed, 20 Apr 2022 09:38:20 GMT  
		Size: 29.3 MB (29318359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; 386

```console
$ docker pull mono@sha256:a620c36d6b438c94797eaa6b17b2452369ac55ab8a59a1bcf8b4501df1eea0c5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99157932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95ff55aea4f3ffc1da74cea929a23a78ed6dc8901847098c5878018368c9da5d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:38:03 GMT
ADD file:602a25173054242f635a5a299845b7f1b56864ac5d3b8af1ae29dec3a9da119f in / 
# Wed, 20 Apr 2022 07:38:04 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:49:08 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 20 Apr 2022 12:49:17 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 20 Apr 2022 12:49:40 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a13b13d818745c4d2234aab71df26e4a01bfe59f396ab62f20d156b94803650c`  
		Last Modified: Wed, 20 Apr 2022 07:45:46 GMT  
		Size: 27.8 MB (27799825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc07624832ff4b064bd2b3797a6774618e27f4c3a1e24419874628eeb613e7ba`  
		Last Modified: Wed, 20 Apr 2022 12:53:02 GMT  
		Size: 2.8 MB (2789161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d6af1a94baa95c219eaba2db2fb27e299572ac8d2859e1399838abdccae784c`  
		Last Modified: Wed, 20 Apr 2022 12:53:11 GMT  
		Size: 68.6 MB (68568946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; ppc64le

```console
$ docker pull mono@sha256:13e28a240194ffdaa1ab1b8b10b807978db6ed7eec8e4d427b0ff2c6d38130b8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.3 MB (60326550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:806eebb6c6b16141507ab480ab6238efd982bbe9375a51cabbc00f5cd2fa62b5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 09:47:47 GMT
ADD file:69078e7ae6d887f7e36ae048f98f784678fbd8b7a8ec27e3c2bce0d68a47236d in / 
# Wed, 20 Apr 2022 09:47:51 GMT
CMD ["bash"]
# Thu, 21 Apr 2022 08:14:20 GMT
ENV MONO_VERSION=6.12.0.122
# Thu, 21 Apr 2022 08:15:04 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 21 Apr 2022 08:16:01 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1aacfa28cbcef999a852ce9c261b67f15f0ccd8450cd1dbfe7b0dc88e6b5aba2`  
		Last Modified: Wed, 20 Apr 2022 09:58:02 GMT  
		Size: 30.6 MB (30560296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b4fd6959397baa971e32512d4c0d1d094bea59e1bf9b3442d8a345c6f7cd81`  
		Last Modified: Thu, 21 Apr 2022 08:33:06 GMT  
		Size: 2.9 MB (2892563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff24986d59f2106922e32fbd04b151763111155f6440aa41d390cbab27fca8c8`  
		Last Modified: Thu, 21 Apr 2022 08:33:11 GMT  
		Size: 26.9 MB (26873691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
