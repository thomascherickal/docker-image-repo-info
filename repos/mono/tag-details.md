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
-	[`mono:6.6`](#mono66)
-	[`mono:6.6.0`](#mono660)
-	[`mono:6.6.0.161`](#mono660161)
-	[`mono:6.6.0.161-slim`](#mono660161-slim)
-	[`mono:6.6.0-slim`](#mono660-slim)
-	[`mono:6.6-slim`](#mono66-slim)
-	[`mono:6.8`](#mono68)
-	[`mono:6.8.0`](#mono680)
-	[`mono:6.8.0.96`](#mono68096)
-	[`mono:6.8.0.96-slim`](#mono68096-slim)
-	[`mono:6.8.0-slim`](#mono680-slim)
-	[`mono:6.8-slim`](#mono68-slim)
-	[`mono:6-slim`](#mono6-slim)
-	[`mono:latest`](#monolatest)
-	[`mono:slim`](#monoslim)

## `mono:5`

```console
$ docker pull mono@sha256:d6565a59b4c4f4186cb3fa83001f333795b7963c8efb8246244d6524b11a7bd0
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
$ docker pull mono@sha256:a6bd33eaec46ce447d3d114fa7d87c1a161ce421bcd9a615d2e3bd79c1b27179
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.3 MB (218273053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d615e447a74530b87923b510fdf27472388004dc17c20dc13b0efb913b52ef96`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:23:03 GMT
ADD file:08ea1ff3fcd4efc24ab4f262cfa24e55e65844f6858e41a46fe0635d247f174d in / 
# Thu, 23 Apr 2020 00:23:03 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:50:05 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 23 Apr 2020 01:50:15 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Apr 2020 01:50:43 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 23 Apr 2020 02:18:39 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b248fa9f6d2ae427ad7f00de3537ab256ae7eb413565f8be0773ee9b86ef57d4`  
		Last Modified: Thu, 23 Apr 2020 00:27:46 GMT  
		Size: 22.5 MB (22513488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb8a90fcd30243429ccde1f9410482825b3cf605a11a43283d700d5d0d2c19d`  
		Last Modified: Thu, 23 Apr 2020 02:19:53 GMT  
		Size: 244.5 KB (244486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc60b582667e2deb99365fcd66c622deb3a30e7320b51aa6bed522cc774124d2`  
		Last Modified: Thu, 23 Apr 2020 02:20:08 GMT  
		Size: 55.5 MB (55520441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372424f3138cf973f4a1e505b9f65ee657ae72dc6d20e6a766e17371c8ba4be6`  
		Last Modified: Thu, 23 Apr 2020 02:22:31 GMT  
		Size: 140.0 MB (139994638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5` - linux; arm variant v5

```console
$ docker pull mono@sha256:d0990a67b741ecd468b423fd6b1a5d68565ea9834c7d66e515c359a8aa3ce409
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.9 MB (170947359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:777794083d01b9f8fbae94cc586fb12b4bbc22626fd8c6b723efefb205c154a4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 22:42:50 GMT
ADD file:4d807a3f2b10f72f31b43691d51a75c26c3898b53e775bfc4bc3d08720448371 in / 
# Thu, 14 May 2020 22:42:52 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:10:37 GMT
ENV MONO_VERSION=5.20.1.34
# Fri, 15 May 2020 04:10:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 04:11:48 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 15 May 2020 04:21:06 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8c1954048f7e4cb30320daf180f1197d278a905c20d04ff10b32f11b35b7757c`  
		Last Modified: Thu, 14 May 2020 22:50:57 GMT  
		Size: 21.2 MB (21197082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27f57444326b25b6adc5b706cae418e27ec6f1b33168ae52de8b29dbda24346`  
		Last Modified: Fri, 15 May 2020 04:22:28 GMT  
		Size: 244.5 KB (244528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca922f93721ff7b288af2ce3db01ffa707171df5bf83ae4a8b3c1df3e1da789c`  
		Last Modified: Fri, 15 May 2020 04:22:38 GMT  
		Size: 24.3 MB (24265046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa278c7d38f0acb13496d32aa240b1c3f308e3074535fce5a4e408cc597db82e`  
		Last Modified: Fri, 15 May 2020 04:25:26 GMT  
		Size: 125.2 MB (125240703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5` - linux; arm variant v7

```console
$ docker pull mono@sha256:320363b03bb1b63a9f73c0697b037ce63105ad07f43475c2e9dfd7bba2494e55
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.0 MB (166993175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ef6afc7eee71102b7bcfb81647a5f4d77246cb6153438c04acbf86a0ccbb52c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:19:24 GMT
ADD file:aac27626ed8520bcfd1f03f5b7aa780a4e94978b86afcc507994a8c240953561 in / 
# Wed, 13 May 2020 21:19:26 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:29:08 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 14 May 2020 00:29:28 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:30:19 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 00:42:07 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:307a7e70a6dd41fc81298d6cb2641ebfa8e7bc00b0b27f30f6559f9976a46f1e`  
		Last Modified: Wed, 13 May 2020 21:28:39 GMT  
		Size: 19.3 MB (19298476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896601cb6b4c7cbbe19d0fd80b06e911dc10440fb462364fd269f6ad65b0d878`  
		Last Modified: Thu, 14 May 2020 00:43:20 GMT  
		Size: 244.5 KB (244507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b4e2a9f08b6cddb26653d50b851091a16aa70f85f865b82163f3eda8e29c7ab`  
		Last Modified: Thu, 14 May 2020 00:43:28 GMT  
		Size: 23.6 MB (23562080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c1a825a4dc7639b1e0a16540803a3d7dc497f63ae2e90d1e6a3da65198b782`  
		Last Modified: Thu, 14 May 2020 00:46:07 GMT  
		Size: 123.9 MB (123888112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:9bca20bae5bd3bf6bb5c30818f5ea5a77d1daa278294cf13a82e71192cf0065f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.8 MB (187800654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4471b1413db5322bf5b1095e84d357398cd0203132af181d1455975ed6bb6c45`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:48:17 GMT
ADD file:53d95477395267e3c1059f1101e29a7d4b0fcb2bb52351542f4ac065ccb0b973 in / 
# Wed, 13 May 2020 21:48:19 GMT
CMD ["bash"]
# Thu, 14 May 2020 02:03:31 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 14 May 2020 02:03:53 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 02:04:38 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 02:14:12 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1d8af20f9b50479a890734605435a9de85d69f19b65d29c9c92f43eea2463979`  
		Last Modified: Wed, 13 May 2020 21:56:26 GMT  
		Size: 20.4 MB (20370044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7664f3bea1034c7adfeffc0216ecb4daf47c72f70db51b311a99e7a5234018e`  
		Last Modified: Thu, 14 May 2020 02:15:25 GMT  
		Size: 244.4 KB (244356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c750bc6b6bd8c0e33ee1a45079f8a7e94ad41994a1338e35987e616d46642b8`  
		Last Modified: Thu, 14 May 2020 02:15:34 GMT  
		Size: 28.2 MB (28157301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab507e719776f5ab0d3d35740a189c539a15f0133e7a5008748c8989329943ed`  
		Last Modified: Thu, 14 May 2020 02:18:19 GMT  
		Size: 139.0 MB (139028953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5` - linux; 386

```console
$ docker pull mono@sha256:b28775f3fe4b34e719abe27abd1b63b633e6c1cd00dd06a1f129a408dce60ffa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.8 MB (227783755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42e561300d8198e0c77b6aee4f0990f8c383a633334b3098faf2eb8044008b8b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:42:40 GMT
ADD file:39f8a4c4274f123e2c0a2ef48ac1a111bcc59fda68f3946ab5d644f480fab499 in / 
# Wed, 13 May 2020 21:42:41 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:36:29 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 14 May 2020 00:36:42 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:37:27 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 00:46:23 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1fa825514fac4b3d9226a943b4954a2efb197db27c0c1c5019bf4a5f7529746e`  
		Last Modified: Wed, 13 May 2020 21:50:17 GMT  
		Size: 23.1 MB (23141460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f915ceb93db6764fe0575ee0432a41ae86c2d604b523984aed9d78d5c1234d0f`  
		Last Modified: Thu, 14 May 2020 00:47:39 GMT  
		Size: 244.5 KB (244474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8679a891a2319ab8cd948aec3e70379d339b63d0233de8ee99d38dd0ff0a27f9`  
		Last Modified: Thu, 14 May 2020 00:47:55 GMT  
		Size: 58.6 MB (58557356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8c83ce38d25359d8ed294348233e5ac1ca3189dc7833fcff28951d47a4ca8f2`  
		Last Modified: Thu, 14 May 2020 00:51:37 GMT  
		Size: 145.8 MB (145840465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5` - linux; ppc64le

```console
$ docker pull mono@sha256:520a7be6cca5031ab382cf6d12cfe9a4c0f7b66746bef679cdb6bb4979d62d07
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.3 MB (173291523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3053d7df0e823d1a61dda1cda08a385d28e0adbea568b51885bed8c2be7e1c34`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:42:09 GMT
ADD file:341dbc564992a44e81b3a4f399f7de14d7340a45b73c577edb78e16da2c14584 in / 
# Wed, 13 May 2020 22:42:12 GMT
CMD ["bash"]
# Thu, 14 May 2020 01:50:04 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 14 May 2020 01:50:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 01:51:55 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 02:10:11 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3b6ae894780534c0f99588e9cce4beb8fb7884b4578e6206b72f2db75116bb1c`  
		Last Modified: Wed, 13 May 2020 23:02:51 GMT  
		Size: 22.8 MB (22785361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f1dc144d71ebf5bd6087036a8c8f775c55db152b26a34c40ca01b3f46e2372`  
		Last Modified: Thu, 14 May 2020 02:11:55 GMT  
		Size: 244.5 KB (244492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc7b3ed156debf9afe549ded8235a14506c726d42c634573aea54f25e12ff092`  
		Last Modified: Thu, 14 May 2020 02:12:12 GMT  
		Size: 24.6 MB (24638890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121b739b2a59d878c4cef1c4717163d4bbb0bf8c4cb15dca30da5668c013b86e`  
		Last Modified: Thu, 14 May 2020 02:16:47 GMT  
		Size: 125.6 MB (125622780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.20`

```console
$ docker pull mono@sha256:d6565a59b4c4f4186cb3fa83001f333795b7963c8efb8246244d6524b11a7bd0
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
$ docker pull mono@sha256:a6bd33eaec46ce447d3d114fa7d87c1a161ce421bcd9a615d2e3bd79c1b27179
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.3 MB (218273053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d615e447a74530b87923b510fdf27472388004dc17c20dc13b0efb913b52ef96`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:23:03 GMT
ADD file:08ea1ff3fcd4efc24ab4f262cfa24e55e65844f6858e41a46fe0635d247f174d in / 
# Thu, 23 Apr 2020 00:23:03 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:50:05 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 23 Apr 2020 01:50:15 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Apr 2020 01:50:43 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 23 Apr 2020 02:18:39 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b248fa9f6d2ae427ad7f00de3537ab256ae7eb413565f8be0773ee9b86ef57d4`  
		Last Modified: Thu, 23 Apr 2020 00:27:46 GMT  
		Size: 22.5 MB (22513488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb8a90fcd30243429ccde1f9410482825b3cf605a11a43283d700d5d0d2c19d`  
		Last Modified: Thu, 23 Apr 2020 02:19:53 GMT  
		Size: 244.5 KB (244486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc60b582667e2deb99365fcd66c622deb3a30e7320b51aa6bed522cc774124d2`  
		Last Modified: Thu, 23 Apr 2020 02:20:08 GMT  
		Size: 55.5 MB (55520441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372424f3138cf973f4a1e505b9f65ee657ae72dc6d20e6a766e17371c8ba4be6`  
		Last Modified: Thu, 23 Apr 2020 02:22:31 GMT  
		Size: 140.0 MB (139994638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20` - linux; arm variant v5

```console
$ docker pull mono@sha256:d0990a67b741ecd468b423fd6b1a5d68565ea9834c7d66e515c359a8aa3ce409
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.9 MB (170947359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:777794083d01b9f8fbae94cc586fb12b4bbc22626fd8c6b723efefb205c154a4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 22:42:50 GMT
ADD file:4d807a3f2b10f72f31b43691d51a75c26c3898b53e775bfc4bc3d08720448371 in / 
# Thu, 14 May 2020 22:42:52 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:10:37 GMT
ENV MONO_VERSION=5.20.1.34
# Fri, 15 May 2020 04:10:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 04:11:48 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 15 May 2020 04:21:06 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8c1954048f7e4cb30320daf180f1197d278a905c20d04ff10b32f11b35b7757c`  
		Last Modified: Thu, 14 May 2020 22:50:57 GMT  
		Size: 21.2 MB (21197082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27f57444326b25b6adc5b706cae418e27ec6f1b33168ae52de8b29dbda24346`  
		Last Modified: Fri, 15 May 2020 04:22:28 GMT  
		Size: 244.5 KB (244528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca922f93721ff7b288af2ce3db01ffa707171df5bf83ae4a8b3c1df3e1da789c`  
		Last Modified: Fri, 15 May 2020 04:22:38 GMT  
		Size: 24.3 MB (24265046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa278c7d38f0acb13496d32aa240b1c3f308e3074535fce5a4e408cc597db82e`  
		Last Modified: Fri, 15 May 2020 04:25:26 GMT  
		Size: 125.2 MB (125240703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20` - linux; arm variant v7

```console
$ docker pull mono@sha256:320363b03bb1b63a9f73c0697b037ce63105ad07f43475c2e9dfd7bba2494e55
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.0 MB (166993175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ef6afc7eee71102b7bcfb81647a5f4d77246cb6153438c04acbf86a0ccbb52c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:19:24 GMT
ADD file:aac27626ed8520bcfd1f03f5b7aa780a4e94978b86afcc507994a8c240953561 in / 
# Wed, 13 May 2020 21:19:26 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:29:08 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 14 May 2020 00:29:28 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:30:19 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 00:42:07 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:307a7e70a6dd41fc81298d6cb2641ebfa8e7bc00b0b27f30f6559f9976a46f1e`  
		Last Modified: Wed, 13 May 2020 21:28:39 GMT  
		Size: 19.3 MB (19298476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896601cb6b4c7cbbe19d0fd80b06e911dc10440fb462364fd269f6ad65b0d878`  
		Last Modified: Thu, 14 May 2020 00:43:20 GMT  
		Size: 244.5 KB (244507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b4e2a9f08b6cddb26653d50b851091a16aa70f85f865b82163f3eda8e29c7ab`  
		Last Modified: Thu, 14 May 2020 00:43:28 GMT  
		Size: 23.6 MB (23562080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c1a825a4dc7639b1e0a16540803a3d7dc497f63ae2e90d1e6a3da65198b782`  
		Last Modified: Thu, 14 May 2020 00:46:07 GMT  
		Size: 123.9 MB (123888112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:9bca20bae5bd3bf6bb5c30818f5ea5a77d1daa278294cf13a82e71192cf0065f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.8 MB (187800654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4471b1413db5322bf5b1095e84d357398cd0203132af181d1455975ed6bb6c45`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:48:17 GMT
ADD file:53d95477395267e3c1059f1101e29a7d4b0fcb2bb52351542f4ac065ccb0b973 in / 
# Wed, 13 May 2020 21:48:19 GMT
CMD ["bash"]
# Thu, 14 May 2020 02:03:31 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 14 May 2020 02:03:53 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 02:04:38 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 02:14:12 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1d8af20f9b50479a890734605435a9de85d69f19b65d29c9c92f43eea2463979`  
		Last Modified: Wed, 13 May 2020 21:56:26 GMT  
		Size: 20.4 MB (20370044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7664f3bea1034c7adfeffc0216ecb4daf47c72f70db51b311a99e7a5234018e`  
		Last Modified: Thu, 14 May 2020 02:15:25 GMT  
		Size: 244.4 KB (244356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c750bc6b6bd8c0e33ee1a45079f8a7e94ad41994a1338e35987e616d46642b8`  
		Last Modified: Thu, 14 May 2020 02:15:34 GMT  
		Size: 28.2 MB (28157301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab507e719776f5ab0d3d35740a189c539a15f0133e7a5008748c8989329943ed`  
		Last Modified: Thu, 14 May 2020 02:18:19 GMT  
		Size: 139.0 MB (139028953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20` - linux; 386

```console
$ docker pull mono@sha256:b28775f3fe4b34e719abe27abd1b63b633e6c1cd00dd06a1f129a408dce60ffa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.8 MB (227783755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42e561300d8198e0c77b6aee4f0990f8c383a633334b3098faf2eb8044008b8b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:42:40 GMT
ADD file:39f8a4c4274f123e2c0a2ef48ac1a111bcc59fda68f3946ab5d644f480fab499 in / 
# Wed, 13 May 2020 21:42:41 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:36:29 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 14 May 2020 00:36:42 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:37:27 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 00:46:23 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1fa825514fac4b3d9226a943b4954a2efb197db27c0c1c5019bf4a5f7529746e`  
		Last Modified: Wed, 13 May 2020 21:50:17 GMT  
		Size: 23.1 MB (23141460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f915ceb93db6764fe0575ee0432a41ae86c2d604b523984aed9d78d5c1234d0f`  
		Last Modified: Thu, 14 May 2020 00:47:39 GMT  
		Size: 244.5 KB (244474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8679a891a2319ab8cd948aec3e70379d339b63d0233de8ee99d38dd0ff0a27f9`  
		Last Modified: Thu, 14 May 2020 00:47:55 GMT  
		Size: 58.6 MB (58557356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8c83ce38d25359d8ed294348233e5ac1ca3189dc7833fcff28951d47a4ca8f2`  
		Last Modified: Thu, 14 May 2020 00:51:37 GMT  
		Size: 145.8 MB (145840465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20` - linux; ppc64le

```console
$ docker pull mono@sha256:520a7be6cca5031ab382cf6d12cfe9a4c0f7b66746bef679cdb6bb4979d62d07
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.3 MB (173291523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3053d7df0e823d1a61dda1cda08a385d28e0adbea568b51885bed8c2be7e1c34`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:42:09 GMT
ADD file:341dbc564992a44e81b3a4f399f7de14d7340a45b73c577edb78e16da2c14584 in / 
# Wed, 13 May 2020 22:42:12 GMT
CMD ["bash"]
# Thu, 14 May 2020 01:50:04 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 14 May 2020 01:50:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 01:51:55 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 02:10:11 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3b6ae894780534c0f99588e9cce4beb8fb7884b4578e6206b72f2db75116bb1c`  
		Last Modified: Wed, 13 May 2020 23:02:51 GMT  
		Size: 22.8 MB (22785361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f1dc144d71ebf5bd6087036a8c8f775c55db152b26a34c40ca01b3f46e2372`  
		Last Modified: Thu, 14 May 2020 02:11:55 GMT  
		Size: 244.5 KB (244492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc7b3ed156debf9afe549ded8235a14506c726d42c634573aea54f25e12ff092`  
		Last Modified: Thu, 14 May 2020 02:12:12 GMT  
		Size: 24.6 MB (24638890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121b739b2a59d878c4cef1c4717163d4bbb0bf8c4cb15dca30da5668c013b86e`  
		Last Modified: Thu, 14 May 2020 02:16:47 GMT  
		Size: 125.6 MB (125622780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.20.1`

```console
$ docker pull mono@sha256:d6565a59b4c4f4186cb3fa83001f333795b7963c8efb8246244d6524b11a7bd0
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
$ docker pull mono@sha256:a6bd33eaec46ce447d3d114fa7d87c1a161ce421bcd9a615d2e3bd79c1b27179
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.3 MB (218273053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d615e447a74530b87923b510fdf27472388004dc17c20dc13b0efb913b52ef96`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:23:03 GMT
ADD file:08ea1ff3fcd4efc24ab4f262cfa24e55e65844f6858e41a46fe0635d247f174d in / 
# Thu, 23 Apr 2020 00:23:03 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:50:05 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 23 Apr 2020 01:50:15 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Apr 2020 01:50:43 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 23 Apr 2020 02:18:39 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b248fa9f6d2ae427ad7f00de3537ab256ae7eb413565f8be0773ee9b86ef57d4`  
		Last Modified: Thu, 23 Apr 2020 00:27:46 GMT  
		Size: 22.5 MB (22513488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb8a90fcd30243429ccde1f9410482825b3cf605a11a43283d700d5d0d2c19d`  
		Last Modified: Thu, 23 Apr 2020 02:19:53 GMT  
		Size: 244.5 KB (244486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc60b582667e2deb99365fcd66c622deb3a30e7320b51aa6bed522cc774124d2`  
		Last Modified: Thu, 23 Apr 2020 02:20:08 GMT  
		Size: 55.5 MB (55520441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372424f3138cf973f4a1e505b9f65ee657ae72dc6d20e6a766e17371c8ba4be6`  
		Last Modified: Thu, 23 Apr 2020 02:22:31 GMT  
		Size: 140.0 MB (139994638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1` - linux; arm variant v5

```console
$ docker pull mono@sha256:d0990a67b741ecd468b423fd6b1a5d68565ea9834c7d66e515c359a8aa3ce409
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.9 MB (170947359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:777794083d01b9f8fbae94cc586fb12b4bbc22626fd8c6b723efefb205c154a4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 22:42:50 GMT
ADD file:4d807a3f2b10f72f31b43691d51a75c26c3898b53e775bfc4bc3d08720448371 in / 
# Thu, 14 May 2020 22:42:52 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:10:37 GMT
ENV MONO_VERSION=5.20.1.34
# Fri, 15 May 2020 04:10:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 04:11:48 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 15 May 2020 04:21:06 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8c1954048f7e4cb30320daf180f1197d278a905c20d04ff10b32f11b35b7757c`  
		Last Modified: Thu, 14 May 2020 22:50:57 GMT  
		Size: 21.2 MB (21197082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27f57444326b25b6adc5b706cae418e27ec6f1b33168ae52de8b29dbda24346`  
		Last Modified: Fri, 15 May 2020 04:22:28 GMT  
		Size: 244.5 KB (244528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca922f93721ff7b288af2ce3db01ffa707171df5bf83ae4a8b3c1df3e1da789c`  
		Last Modified: Fri, 15 May 2020 04:22:38 GMT  
		Size: 24.3 MB (24265046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa278c7d38f0acb13496d32aa240b1c3f308e3074535fce5a4e408cc597db82e`  
		Last Modified: Fri, 15 May 2020 04:25:26 GMT  
		Size: 125.2 MB (125240703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1` - linux; arm variant v7

```console
$ docker pull mono@sha256:320363b03bb1b63a9f73c0697b037ce63105ad07f43475c2e9dfd7bba2494e55
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.0 MB (166993175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ef6afc7eee71102b7bcfb81647a5f4d77246cb6153438c04acbf86a0ccbb52c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:19:24 GMT
ADD file:aac27626ed8520bcfd1f03f5b7aa780a4e94978b86afcc507994a8c240953561 in / 
# Wed, 13 May 2020 21:19:26 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:29:08 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 14 May 2020 00:29:28 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:30:19 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 00:42:07 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:307a7e70a6dd41fc81298d6cb2641ebfa8e7bc00b0b27f30f6559f9976a46f1e`  
		Last Modified: Wed, 13 May 2020 21:28:39 GMT  
		Size: 19.3 MB (19298476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896601cb6b4c7cbbe19d0fd80b06e911dc10440fb462364fd269f6ad65b0d878`  
		Last Modified: Thu, 14 May 2020 00:43:20 GMT  
		Size: 244.5 KB (244507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b4e2a9f08b6cddb26653d50b851091a16aa70f85f865b82163f3eda8e29c7ab`  
		Last Modified: Thu, 14 May 2020 00:43:28 GMT  
		Size: 23.6 MB (23562080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c1a825a4dc7639b1e0a16540803a3d7dc497f63ae2e90d1e6a3da65198b782`  
		Last Modified: Thu, 14 May 2020 00:46:07 GMT  
		Size: 123.9 MB (123888112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:9bca20bae5bd3bf6bb5c30818f5ea5a77d1daa278294cf13a82e71192cf0065f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.8 MB (187800654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4471b1413db5322bf5b1095e84d357398cd0203132af181d1455975ed6bb6c45`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:48:17 GMT
ADD file:53d95477395267e3c1059f1101e29a7d4b0fcb2bb52351542f4ac065ccb0b973 in / 
# Wed, 13 May 2020 21:48:19 GMT
CMD ["bash"]
# Thu, 14 May 2020 02:03:31 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 14 May 2020 02:03:53 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 02:04:38 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 02:14:12 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1d8af20f9b50479a890734605435a9de85d69f19b65d29c9c92f43eea2463979`  
		Last Modified: Wed, 13 May 2020 21:56:26 GMT  
		Size: 20.4 MB (20370044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7664f3bea1034c7adfeffc0216ecb4daf47c72f70db51b311a99e7a5234018e`  
		Last Modified: Thu, 14 May 2020 02:15:25 GMT  
		Size: 244.4 KB (244356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c750bc6b6bd8c0e33ee1a45079f8a7e94ad41994a1338e35987e616d46642b8`  
		Last Modified: Thu, 14 May 2020 02:15:34 GMT  
		Size: 28.2 MB (28157301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab507e719776f5ab0d3d35740a189c539a15f0133e7a5008748c8989329943ed`  
		Last Modified: Thu, 14 May 2020 02:18:19 GMT  
		Size: 139.0 MB (139028953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1` - linux; 386

```console
$ docker pull mono@sha256:b28775f3fe4b34e719abe27abd1b63b633e6c1cd00dd06a1f129a408dce60ffa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.8 MB (227783755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42e561300d8198e0c77b6aee4f0990f8c383a633334b3098faf2eb8044008b8b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:42:40 GMT
ADD file:39f8a4c4274f123e2c0a2ef48ac1a111bcc59fda68f3946ab5d644f480fab499 in / 
# Wed, 13 May 2020 21:42:41 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:36:29 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 14 May 2020 00:36:42 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:37:27 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 00:46:23 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1fa825514fac4b3d9226a943b4954a2efb197db27c0c1c5019bf4a5f7529746e`  
		Last Modified: Wed, 13 May 2020 21:50:17 GMT  
		Size: 23.1 MB (23141460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f915ceb93db6764fe0575ee0432a41ae86c2d604b523984aed9d78d5c1234d0f`  
		Last Modified: Thu, 14 May 2020 00:47:39 GMT  
		Size: 244.5 KB (244474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8679a891a2319ab8cd948aec3e70379d339b63d0233de8ee99d38dd0ff0a27f9`  
		Last Modified: Thu, 14 May 2020 00:47:55 GMT  
		Size: 58.6 MB (58557356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8c83ce38d25359d8ed294348233e5ac1ca3189dc7833fcff28951d47a4ca8f2`  
		Last Modified: Thu, 14 May 2020 00:51:37 GMT  
		Size: 145.8 MB (145840465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1` - linux; ppc64le

```console
$ docker pull mono@sha256:520a7be6cca5031ab382cf6d12cfe9a4c0f7b66746bef679cdb6bb4979d62d07
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.3 MB (173291523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3053d7df0e823d1a61dda1cda08a385d28e0adbea568b51885bed8c2be7e1c34`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:42:09 GMT
ADD file:341dbc564992a44e81b3a4f399f7de14d7340a45b73c577edb78e16da2c14584 in / 
# Wed, 13 May 2020 22:42:12 GMT
CMD ["bash"]
# Thu, 14 May 2020 01:50:04 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 14 May 2020 01:50:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 01:51:55 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 02:10:11 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3b6ae894780534c0f99588e9cce4beb8fb7884b4578e6206b72f2db75116bb1c`  
		Last Modified: Wed, 13 May 2020 23:02:51 GMT  
		Size: 22.8 MB (22785361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f1dc144d71ebf5bd6087036a8c8f775c55db152b26a34c40ca01b3f46e2372`  
		Last Modified: Thu, 14 May 2020 02:11:55 GMT  
		Size: 244.5 KB (244492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc7b3ed156debf9afe549ded8235a14506c726d42c634573aea54f25e12ff092`  
		Last Modified: Thu, 14 May 2020 02:12:12 GMT  
		Size: 24.6 MB (24638890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121b739b2a59d878c4cef1c4717163d4bbb0bf8c4cb15dca30da5668c013b86e`  
		Last Modified: Thu, 14 May 2020 02:16:47 GMT  
		Size: 125.6 MB (125622780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.20.1.34`

```console
$ docker pull mono@sha256:d6565a59b4c4f4186cb3fa83001f333795b7963c8efb8246244d6524b11a7bd0
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
$ docker pull mono@sha256:a6bd33eaec46ce447d3d114fa7d87c1a161ce421bcd9a615d2e3bd79c1b27179
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.3 MB (218273053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d615e447a74530b87923b510fdf27472388004dc17c20dc13b0efb913b52ef96`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:23:03 GMT
ADD file:08ea1ff3fcd4efc24ab4f262cfa24e55e65844f6858e41a46fe0635d247f174d in / 
# Thu, 23 Apr 2020 00:23:03 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:50:05 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 23 Apr 2020 01:50:15 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Apr 2020 01:50:43 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 23 Apr 2020 02:18:39 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b248fa9f6d2ae427ad7f00de3537ab256ae7eb413565f8be0773ee9b86ef57d4`  
		Last Modified: Thu, 23 Apr 2020 00:27:46 GMT  
		Size: 22.5 MB (22513488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb8a90fcd30243429ccde1f9410482825b3cf605a11a43283d700d5d0d2c19d`  
		Last Modified: Thu, 23 Apr 2020 02:19:53 GMT  
		Size: 244.5 KB (244486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc60b582667e2deb99365fcd66c622deb3a30e7320b51aa6bed522cc774124d2`  
		Last Modified: Thu, 23 Apr 2020 02:20:08 GMT  
		Size: 55.5 MB (55520441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372424f3138cf973f4a1e505b9f65ee657ae72dc6d20e6a766e17371c8ba4be6`  
		Last Modified: Thu, 23 Apr 2020 02:22:31 GMT  
		Size: 140.0 MB (139994638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1.34` - linux; arm variant v5

```console
$ docker pull mono@sha256:d0990a67b741ecd468b423fd6b1a5d68565ea9834c7d66e515c359a8aa3ce409
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.9 MB (170947359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:777794083d01b9f8fbae94cc586fb12b4bbc22626fd8c6b723efefb205c154a4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 22:42:50 GMT
ADD file:4d807a3f2b10f72f31b43691d51a75c26c3898b53e775bfc4bc3d08720448371 in / 
# Thu, 14 May 2020 22:42:52 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:10:37 GMT
ENV MONO_VERSION=5.20.1.34
# Fri, 15 May 2020 04:10:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 04:11:48 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 15 May 2020 04:21:06 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8c1954048f7e4cb30320daf180f1197d278a905c20d04ff10b32f11b35b7757c`  
		Last Modified: Thu, 14 May 2020 22:50:57 GMT  
		Size: 21.2 MB (21197082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27f57444326b25b6adc5b706cae418e27ec6f1b33168ae52de8b29dbda24346`  
		Last Modified: Fri, 15 May 2020 04:22:28 GMT  
		Size: 244.5 KB (244528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca922f93721ff7b288af2ce3db01ffa707171df5bf83ae4a8b3c1df3e1da789c`  
		Last Modified: Fri, 15 May 2020 04:22:38 GMT  
		Size: 24.3 MB (24265046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa278c7d38f0acb13496d32aa240b1c3f308e3074535fce5a4e408cc597db82e`  
		Last Modified: Fri, 15 May 2020 04:25:26 GMT  
		Size: 125.2 MB (125240703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1.34` - linux; arm variant v7

```console
$ docker pull mono@sha256:320363b03bb1b63a9f73c0697b037ce63105ad07f43475c2e9dfd7bba2494e55
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.0 MB (166993175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ef6afc7eee71102b7bcfb81647a5f4d77246cb6153438c04acbf86a0ccbb52c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:19:24 GMT
ADD file:aac27626ed8520bcfd1f03f5b7aa780a4e94978b86afcc507994a8c240953561 in / 
# Wed, 13 May 2020 21:19:26 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:29:08 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 14 May 2020 00:29:28 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:30:19 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 00:42:07 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:307a7e70a6dd41fc81298d6cb2641ebfa8e7bc00b0b27f30f6559f9976a46f1e`  
		Last Modified: Wed, 13 May 2020 21:28:39 GMT  
		Size: 19.3 MB (19298476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896601cb6b4c7cbbe19d0fd80b06e911dc10440fb462364fd269f6ad65b0d878`  
		Last Modified: Thu, 14 May 2020 00:43:20 GMT  
		Size: 244.5 KB (244507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b4e2a9f08b6cddb26653d50b851091a16aa70f85f865b82163f3eda8e29c7ab`  
		Last Modified: Thu, 14 May 2020 00:43:28 GMT  
		Size: 23.6 MB (23562080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c1a825a4dc7639b1e0a16540803a3d7dc497f63ae2e90d1e6a3da65198b782`  
		Last Modified: Thu, 14 May 2020 00:46:07 GMT  
		Size: 123.9 MB (123888112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1.34` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:9bca20bae5bd3bf6bb5c30818f5ea5a77d1daa278294cf13a82e71192cf0065f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.8 MB (187800654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4471b1413db5322bf5b1095e84d357398cd0203132af181d1455975ed6bb6c45`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:48:17 GMT
ADD file:53d95477395267e3c1059f1101e29a7d4b0fcb2bb52351542f4ac065ccb0b973 in / 
# Wed, 13 May 2020 21:48:19 GMT
CMD ["bash"]
# Thu, 14 May 2020 02:03:31 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 14 May 2020 02:03:53 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 02:04:38 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 02:14:12 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1d8af20f9b50479a890734605435a9de85d69f19b65d29c9c92f43eea2463979`  
		Last Modified: Wed, 13 May 2020 21:56:26 GMT  
		Size: 20.4 MB (20370044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7664f3bea1034c7adfeffc0216ecb4daf47c72f70db51b311a99e7a5234018e`  
		Last Modified: Thu, 14 May 2020 02:15:25 GMT  
		Size: 244.4 KB (244356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c750bc6b6bd8c0e33ee1a45079f8a7e94ad41994a1338e35987e616d46642b8`  
		Last Modified: Thu, 14 May 2020 02:15:34 GMT  
		Size: 28.2 MB (28157301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab507e719776f5ab0d3d35740a189c539a15f0133e7a5008748c8989329943ed`  
		Last Modified: Thu, 14 May 2020 02:18:19 GMT  
		Size: 139.0 MB (139028953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1.34` - linux; 386

```console
$ docker pull mono@sha256:b28775f3fe4b34e719abe27abd1b63b633e6c1cd00dd06a1f129a408dce60ffa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.8 MB (227783755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42e561300d8198e0c77b6aee4f0990f8c383a633334b3098faf2eb8044008b8b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:42:40 GMT
ADD file:39f8a4c4274f123e2c0a2ef48ac1a111bcc59fda68f3946ab5d644f480fab499 in / 
# Wed, 13 May 2020 21:42:41 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:36:29 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 14 May 2020 00:36:42 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:37:27 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 00:46:23 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1fa825514fac4b3d9226a943b4954a2efb197db27c0c1c5019bf4a5f7529746e`  
		Last Modified: Wed, 13 May 2020 21:50:17 GMT  
		Size: 23.1 MB (23141460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f915ceb93db6764fe0575ee0432a41ae86c2d604b523984aed9d78d5c1234d0f`  
		Last Modified: Thu, 14 May 2020 00:47:39 GMT  
		Size: 244.5 KB (244474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8679a891a2319ab8cd948aec3e70379d339b63d0233de8ee99d38dd0ff0a27f9`  
		Last Modified: Thu, 14 May 2020 00:47:55 GMT  
		Size: 58.6 MB (58557356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8c83ce38d25359d8ed294348233e5ac1ca3189dc7833fcff28951d47a4ca8f2`  
		Last Modified: Thu, 14 May 2020 00:51:37 GMT  
		Size: 145.8 MB (145840465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1.34` - linux; ppc64le

```console
$ docker pull mono@sha256:520a7be6cca5031ab382cf6d12cfe9a4c0f7b66746bef679cdb6bb4979d62d07
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.3 MB (173291523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3053d7df0e823d1a61dda1cda08a385d28e0adbea568b51885bed8c2be7e1c34`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:42:09 GMT
ADD file:341dbc564992a44e81b3a4f399f7de14d7340a45b73c577edb78e16da2c14584 in / 
# Wed, 13 May 2020 22:42:12 GMT
CMD ["bash"]
# Thu, 14 May 2020 01:50:04 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 14 May 2020 01:50:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 01:51:55 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 02:10:11 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3b6ae894780534c0f99588e9cce4beb8fb7884b4578e6206b72f2db75116bb1c`  
		Last Modified: Wed, 13 May 2020 23:02:51 GMT  
		Size: 22.8 MB (22785361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f1dc144d71ebf5bd6087036a8c8f775c55db152b26a34c40ca01b3f46e2372`  
		Last Modified: Thu, 14 May 2020 02:11:55 GMT  
		Size: 244.5 KB (244492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc7b3ed156debf9afe549ded8235a14506c726d42c634573aea54f25e12ff092`  
		Last Modified: Thu, 14 May 2020 02:12:12 GMT  
		Size: 24.6 MB (24638890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121b739b2a59d878c4cef1c4717163d4bbb0bf8c4cb15dca30da5668c013b86e`  
		Last Modified: Thu, 14 May 2020 02:16:47 GMT  
		Size: 125.6 MB (125622780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.20.1.34-slim`

```console
$ docker pull mono@sha256:baed01710cdf1d3ed52eaa00aa4035b80082a6a6256836c1ff88db42c25cdb9d
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
$ docker pull mono@sha256:a67c4cfdbe2cbfd691b5e0506c6d7c3f63e27f09611f7553437ee8be0c1540d4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78278415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bfd262ac923bb4f9148617aa8498c5ab8c4aa833de4b7c30ea774331686612e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:23:03 GMT
ADD file:08ea1ff3fcd4efc24ab4f262cfa24e55e65844f6858e41a46fe0635d247f174d in / 
# Thu, 23 Apr 2020 00:23:03 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:50:05 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 23 Apr 2020 01:50:15 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Apr 2020 01:50:43 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b248fa9f6d2ae427ad7f00de3537ab256ae7eb413565f8be0773ee9b86ef57d4`  
		Last Modified: Thu, 23 Apr 2020 00:27:46 GMT  
		Size: 22.5 MB (22513488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb8a90fcd30243429ccde1f9410482825b3cf605a11a43283d700d5d0d2c19d`  
		Last Modified: Thu, 23 Apr 2020 02:19:53 GMT  
		Size: 244.5 KB (244486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc60b582667e2deb99365fcd66c622deb3a30e7320b51aa6bed522cc774124d2`  
		Last Modified: Thu, 23 Apr 2020 02:20:08 GMT  
		Size: 55.5 MB (55520441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1.34-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:2310d3d6267b9953c7c1e9246d65b092834df4f109a3e1e05210bc26ac9cc81c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.7 MB (45706656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:496109827bf18819213d5b47184b51d13344664af24925b3e975a9554cca18ff`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 22:42:50 GMT
ADD file:4d807a3f2b10f72f31b43691d51a75c26c3898b53e775bfc4bc3d08720448371 in / 
# Thu, 14 May 2020 22:42:52 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:10:37 GMT
ENV MONO_VERSION=5.20.1.34
# Fri, 15 May 2020 04:10:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 04:11:48 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8c1954048f7e4cb30320daf180f1197d278a905c20d04ff10b32f11b35b7757c`  
		Last Modified: Thu, 14 May 2020 22:50:57 GMT  
		Size: 21.2 MB (21197082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27f57444326b25b6adc5b706cae418e27ec6f1b33168ae52de8b29dbda24346`  
		Last Modified: Fri, 15 May 2020 04:22:28 GMT  
		Size: 244.5 KB (244528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca922f93721ff7b288af2ce3db01ffa707171df5bf83ae4a8b3c1df3e1da789c`  
		Last Modified: Fri, 15 May 2020 04:22:38 GMT  
		Size: 24.3 MB (24265046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1.34-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:434173f3eea1e1ba04eb71d0e55c471952da67b323ed3f91ee7ea673e36d2d94
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43105063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd793e4cb8a7142b1b6735b42ab1cf3da33103e53e192c66c57c495aaa9eac80`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:19:24 GMT
ADD file:aac27626ed8520bcfd1f03f5b7aa780a4e94978b86afcc507994a8c240953561 in / 
# Wed, 13 May 2020 21:19:26 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:29:08 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 14 May 2020 00:29:28 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:30:19 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:307a7e70a6dd41fc81298d6cb2641ebfa8e7bc00b0b27f30f6559f9976a46f1e`  
		Last Modified: Wed, 13 May 2020 21:28:39 GMT  
		Size: 19.3 MB (19298476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896601cb6b4c7cbbe19d0fd80b06e911dc10440fb462364fd269f6ad65b0d878`  
		Last Modified: Thu, 14 May 2020 00:43:20 GMT  
		Size: 244.5 KB (244507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b4e2a9f08b6cddb26653d50b851091a16aa70f85f865b82163f3eda8e29c7ab`  
		Last Modified: Thu, 14 May 2020 00:43:28 GMT  
		Size: 23.6 MB (23562080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1.34-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:4eafdba106027bbd748ab01b58d3f87e0b2eebfc080c28b8b2a2d058eaa9e97e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48771701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07387acae610806e811268fe2c83177e416bf4fb94cf1f4848183b3e85982fae`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:48:17 GMT
ADD file:53d95477395267e3c1059f1101e29a7d4b0fcb2bb52351542f4ac065ccb0b973 in / 
# Wed, 13 May 2020 21:48:19 GMT
CMD ["bash"]
# Thu, 14 May 2020 02:03:31 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 14 May 2020 02:03:53 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 02:04:38 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1d8af20f9b50479a890734605435a9de85d69f19b65d29c9c92f43eea2463979`  
		Last Modified: Wed, 13 May 2020 21:56:26 GMT  
		Size: 20.4 MB (20370044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7664f3bea1034c7adfeffc0216ecb4daf47c72f70db51b311a99e7a5234018e`  
		Last Modified: Thu, 14 May 2020 02:15:25 GMT  
		Size: 244.4 KB (244356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c750bc6b6bd8c0e33ee1a45079f8a7e94ad41994a1338e35987e616d46642b8`  
		Last Modified: Thu, 14 May 2020 02:15:34 GMT  
		Size: 28.2 MB (28157301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1.34-slim` - linux; 386

```console
$ docker pull mono@sha256:4eedd0160a1082fd7a646e7f8492c3d464e673f13c2de5306be27a915e74c232
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81943290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0efb3cfe06d5aa360834e7361d319c8589b6d5d2f55816151e0b8c68e3f8cc0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:42:40 GMT
ADD file:39f8a4c4274f123e2c0a2ef48ac1a111bcc59fda68f3946ab5d644f480fab499 in / 
# Wed, 13 May 2020 21:42:41 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:36:29 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 14 May 2020 00:36:42 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:37:27 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1fa825514fac4b3d9226a943b4954a2efb197db27c0c1c5019bf4a5f7529746e`  
		Last Modified: Wed, 13 May 2020 21:50:17 GMT  
		Size: 23.1 MB (23141460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f915ceb93db6764fe0575ee0432a41ae86c2d604b523984aed9d78d5c1234d0f`  
		Last Modified: Thu, 14 May 2020 00:47:39 GMT  
		Size: 244.5 KB (244474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8679a891a2319ab8cd948aec3e70379d339b63d0233de8ee99d38dd0ff0a27f9`  
		Last Modified: Thu, 14 May 2020 00:47:55 GMT  
		Size: 58.6 MB (58557356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1.34-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:bb95612257eeef3bdeda1eb6ec5b729e68c3641c64daca4c43e9a096738f48ab
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.7 MB (47668743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96e062ad47c88c3e2daed7608ea87a8a2796b863474c47f3e7fcae8d5d8e5cd3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:42:09 GMT
ADD file:341dbc564992a44e81b3a4f399f7de14d7340a45b73c577edb78e16da2c14584 in / 
# Wed, 13 May 2020 22:42:12 GMT
CMD ["bash"]
# Thu, 14 May 2020 01:50:04 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 14 May 2020 01:50:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 01:51:55 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3b6ae894780534c0f99588e9cce4beb8fb7884b4578e6206b72f2db75116bb1c`  
		Last Modified: Wed, 13 May 2020 23:02:51 GMT  
		Size: 22.8 MB (22785361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f1dc144d71ebf5bd6087036a8c8f775c55db152b26a34c40ca01b3f46e2372`  
		Last Modified: Thu, 14 May 2020 02:11:55 GMT  
		Size: 244.5 KB (244492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc7b3ed156debf9afe549ded8235a14506c726d42c634573aea54f25e12ff092`  
		Last Modified: Thu, 14 May 2020 02:12:12 GMT  
		Size: 24.6 MB (24638890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.20.1-slim`

```console
$ docker pull mono@sha256:baed01710cdf1d3ed52eaa00aa4035b80082a6a6256836c1ff88db42c25cdb9d
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
$ docker pull mono@sha256:a67c4cfdbe2cbfd691b5e0506c6d7c3f63e27f09611f7553437ee8be0c1540d4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78278415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bfd262ac923bb4f9148617aa8498c5ab8c4aa833de4b7c30ea774331686612e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:23:03 GMT
ADD file:08ea1ff3fcd4efc24ab4f262cfa24e55e65844f6858e41a46fe0635d247f174d in / 
# Thu, 23 Apr 2020 00:23:03 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:50:05 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 23 Apr 2020 01:50:15 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Apr 2020 01:50:43 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b248fa9f6d2ae427ad7f00de3537ab256ae7eb413565f8be0773ee9b86ef57d4`  
		Last Modified: Thu, 23 Apr 2020 00:27:46 GMT  
		Size: 22.5 MB (22513488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb8a90fcd30243429ccde1f9410482825b3cf605a11a43283d700d5d0d2c19d`  
		Last Modified: Thu, 23 Apr 2020 02:19:53 GMT  
		Size: 244.5 KB (244486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc60b582667e2deb99365fcd66c622deb3a30e7320b51aa6bed522cc774124d2`  
		Last Modified: Thu, 23 Apr 2020 02:20:08 GMT  
		Size: 55.5 MB (55520441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:2310d3d6267b9953c7c1e9246d65b092834df4f109a3e1e05210bc26ac9cc81c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.7 MB (45706656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:496109827bf18819213d5b47184b51d13344664af24925b3e975a9554cca18ff`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 22:42:50 GMT
ADD file:4d807a3f2b10f72f31b43691d51a75c26c3898b53e775bfc4bc3d08720448371 in / 
# Thu, 14 May 2020 22:42:52 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:10:37 GMT
ENV MONO_VERSION=5.20.1.34
# Fri, 15 May 2020 04:10:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 04:11:48 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8c1954048f7e4cb30320daf180f1197d278a905c20d04ff10b32f11b35b7757c`  
		Last Modified: Thu, 14 May 2020 22:50:57 GMT  
		Size: 21.2 MB (21197082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27f57444326b25b6adc5b706cae418e27ec6f1b33168ae52de8b29dbda24346`  
		Last Modified: Fri, 15 May 2020 04:22:28 GMT  
		Size: 244.5 KB (244528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca922f93721ff7b288af2ce3db01ffa707171df5bf83ae4a8b3c1df3e1da789c`  
		Last Modified: Fri, 15 May 2020 04:22:38 GMT  
		Size: 24.3 MB (24265046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:434173f3eea1e1ba04eb71d0e55c471952da67b323ed3f91ee7ea673e36d2d94
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43105063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd793e4cb8a7142b1b6735b42ab1cf3da33103e53e192c66c57c495aaa9eac80`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:19:24 GMT
ADD file:aac27626ed8520bcfd1f03f5b7aa780a4e94978b86afcc507994a8c240953561 in / 
# Wed, 13 May 2020 21:19:26 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:29:08 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 14 May 2020 00:29:28 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:30:19 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:307a7e70a6dd41fc81298d6cb2641ebfa8e7bc00b0b27f30f6559f9976a46f1e`  
		Last Modified: Wed, 13 May 2020 21:28:39 GMT  
		Size: 19.3 MB (19298476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896601cb6b4c7cbbe19d0fd80b06e911dc10440fb462364fd269f6ad65b0d878`  
		Last Modified: Thu, 14 May 2020 00:43:20 GMT  
		Size: 244.5 KB (244507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b4e2a9f08b6cddb26653d50b851091a16aa70f85f865b82163f3eda8e29c7ab`  
		Last Modified: Thu, 14 May 2020 00:43:28 GMT  
		Size: 23.6 MB (23562080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:4eafdba106027bbd748ab01b58d3f87e0b2eebfc080c28b8b2a2d058eaa9e97e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48771701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07387acae610806e811268fe2c83177e416bf4fb94cf1f4848183b3e85982fae`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:48:17 GMT
ADD file:53d95477395267e3c1059f1101e29a7d4b0fcb2bb52351542f4ac065ccb0b973 in / 
# Wed, 13 May 2020 21:48:19 GMT
CMD ["bash"]
# Thu, 14 May 2020 02:03:31 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 14 May 2020 02:03:53 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 02:04:38 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1d8af20f9b50479a890734605435a9de85d69f19b65d29c9c92f43eea2463979`  
		Last Modified: Wed, 13 May 2020 21:56:26 GMT  
		Size: 20.4 MB (20370044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7664f3bea1034c7adfeffc0216ecb4daf47c72f70db51b311a99e7a5234018e`  
		Last Modified: Thu, 14 May 2020 02:15:25 GMT  
		Size: 244.4 KB (244356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c750bc6b6bd8c0e33ee1a45079f8a7e94ad41994a1338e35987e616d46642b8`  
		Last Modified: Thu, 14 May 2020 02:15:34 GMT  
		Size: 28.2 MB (28157301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1-slim` - linux; 386

```console
$ docker pull mono@sha256:4eedd0160a1082fd7a646e7f8492c3d464e673f13c2de5306be27a915e74c232
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81943290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0efb3cfe06d5aa360834e7361d319c8589b6d5d2f55816151e0b8c68e3f8cc0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:42:40 GMT
ADD file:39f8a4c4274f123e2c0a2ef48ac1a111bcc59fda68f3946ab5d644f480fab499 in / 
# Wed, 13 May 2020 21:42:41 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:36:29 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 14 May 2020 00:36:42 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:37:27 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1fa825514fac4b3d9226a943b4954a2efb197db27c0c1c5019bf4a5f7529746e`  
		Last Modified: Wed, 13 May 2020 21:50:17 GMT  
		Size: 23.1 MB (23141460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f915ceb93db6764fe0575ee0432a41ae86c2d604b523984aed9d78d5c1234d0f`  
		Last Modified: Thu, 14 May 2020 00:47:39 GMT  
		Size: 244.5 KB (244474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8679a891a2319ab8cd948aec3e70379d339b63d0233de8ee99d38dd0ff0a27f9`  
		Last Modified: Thu, 14 May 2020 00:47:55 GMT  
		Size: 58.6 MB (58557356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:bb95612257eeef3bdeda1eb6ec5b729e68c3641c64daca4c43e9a096738f48ab
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.7 MB (47668743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96e062ad47c88c3e2daed7608ea87a8a2796b863474c47f3e7fcae8d5d8e5cd3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:42:09 GMT
ADD file:341dbc564992a44e81b3a4f399f7de14d7340a45b73c577edb78e16da2c14584 in / 
# Wed, 13 May 2020 22:42:12 GMT
CMD ["bash"]
# Thu, 14 May 2020 01:50:04 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 14 May 2020 01:50:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 01:51:55 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3b6ae894780534c0f99588e9cce4beb8fb7884b4578e6206b72f2db75116bb1c`  
		Last Modified: Wed, 13 May 2020 23:02:51 GMT  
		Size: 22.8 MB (22785361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f1dc144d71ebf5bd6087036a8c8f775c55db152b26a34c40ca01b3f46e2372`  
		Last Modified: Thu, 14 May 2020 02:11:55 GMT  
		Size: 244.5 KB (244492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc7b3ed156debf9afe549ded8235a14506c726d42c634573aea54f25e12ff092`  
		Last Modified: Thu, 14 May 2020 02:12:12 GMT  
		Size: 24.6 MB (24638890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.20-slim`

```console
$ docker pull mono@sha256:baed01710cdf1d3ed52eaa00aa4035b80082a6a6256836c1ff88db42c25cdb9d
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
$ docker pull mono@sha256:a67c4cfdbe2cbfd691b5e0506c6d7c3f63e27f09611f7553437ee8be0c1540d4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78278415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bfd262ac923bb4f9148617aa8498c5ab8c4aa833de4b7c30ea774331686612e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:23:03 GMT
ADD file:08ea1ff3fcd4efc24ab4f262cfa24e55e65844f6858e41a46fe0635d247f174d in / 
# Thu, 23 Apr 2020 00:23:03 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:50:05 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 23 Apr 2020 01:50:15 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Apr 2020 01:50:43 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b248fa9f6d2ae427ad7f00de3537ab256ae7eb413565f8be0773ee9b86ef57d4`  
		Last Modified: Thu, 23 Apr 2020 00:27:46 GMT  
		Size: 22.5 MB (22513488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb8a90fcd30243429ccde1f9410482825b3cf605a11a43283d700d5d0d2c19d`  
		Last Modified: Thu, 23 Apr 2020 02:19:53 GMT  
		Size: 244.5 KB (244486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc60b582667e2deb99365fcd66c622deb3a30e7320b51aa6bed522cc774124d2`  
		Last Modified: Thu, 23 Apr 2020 02:20:08 GMT  
		Size: 55.5 MB (55520441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:2310d3d6267b9953c7c1e9246d65b092834df4f109a3e1e05210bc26ac9cc81c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.7 MB (45706656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:496109827bf18819213d5b47184b51d13344664af24925b3e975a9554cca18ff`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 22:42:50 GMT
ADD file:4d807a3f2b10f72f31b43691d51a75c26c3898b53e775bfc4bc3d08720448371 in / 
# Thu, 14 May 2020 22:42:52 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:10:37 GMT
ENV MONO_VERSION=5.20.1.34
# Fri, 15 May 2020 04:10:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 04:11:48 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8c1954048f7e4cb30320daf180f1197d278a905c20d04ff10b32f11b35b7757c`  
		Last Modified: Thu, 14 May 2020 22:50:57 GMT  
		Size: 21.2 MB (21197082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27f57444326b25b6adc5b706cae418e27ec6f1b33168ae52de8b29dbda24346`  
		Last Modified: Fri, 15 May 2020 04:22:28 GMT  
		Size: 244.5 KB (244528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca922f93721ff7b288af2ce3db01ffa707171df5bf83ae4a8b3c1df3e1da789c`  
		Last Modified: Fri, 15 May 2020 04:22:38 GMT  
		Size: 24.3 MB (24265046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:434173f3eea1e1ba04eb71d0e55c471952da67b323ed3f91ee7ea673e36d2d94
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43105063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd793e4cb8a7142b1b6735b42ab1cf3da33103e53e192c66c57c495aaa9eac80`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:19:24 GMT
ADD file:aac27626ed8520bcfd1f03f5b7aa780a4e94978b86afcc507994a8c240953561 in / 
# Wed, 13 May 2020 21:19:26 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:29:08 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 14 May 2020 00:29:28 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:30:19 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:307a7e70a6dd41fc81298d6cb2641ebfa8e7bc00b0b27f30f6559f9976a46f1e`  
		Last Modified: Wed, 13 May 2020 21:28:39 GMT  
		Size: 19.3 MB (19298476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896601cb6b4c7cbbe19d0fd80b06e911dc10440fb462364fd269f6ad65b0d878`  
		Last Modified: Thu, 14 May 2020 00:43:20 GMT  
		Size: 244.5 KB (244507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b4e2a9f08b6cddb26653d50b851091a16aa70f85f865b82163f3eda8e29c7ab`  
		Last Modified: Thu, 14 May 2020 00:43:28 GMT  
		Size: 23.6 MB (23562080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:4eafdba106027bbd748ab01b58d3f87e0b2eebfc080c28b8b2a2d058eaa9e97e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48771701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07387acae610806e811268fe2c83177e416bf4fb94cf1f4848183b3e85982fae`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:48:17 GMT
ADD file:53d95477395267e3c1059f1101e29a7d4b0fcb2bb52351542f4ac065ccb0b973 in / 
# Wed, 13 May 2020 21:48:19 GMT
CMD ["bash"]
# Thu, 14 May 2020 02:03:31 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 14 May 2020 02:03:53 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 02:04:38 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1d8af20f9b50479a890734605435a9de85d69f19b65d29c9c92f43eea2463979`  
		Last Modified: Wed, 13 May 2020 21:56:26 GMT  
		Size: 20.4 MB (20370044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7664f3bea1034c7adfeffc0216ecb4daf47c72f70db51b311a99e7a5234018e`  
		Last Modified: Thu, 14 May 2020 02:15:25 GMT  
		Size: 244.4 KB (244356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c750bc6b6bd8c0e33ee1a45079f8a7e94ad41994a1338e35987e616d46642b8`  
		Last Modified: Thu, 14 May 2020 02:15:34 GMT  
		Size: 28.2 MB (28157301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20-slim` - linux; 386

```console
$ docker pull mono@sha256:4eedd0160a1082fd7a646e7f8492c3d464e673f13c2de5306be27a915e74c232
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81943290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0efb3cfe06d5aa360834e7361d319c8589b6d5d2f55816151e0b8c68e3f8cc0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:42:40 GMT
ADD file:39f8a4c4274f123e2c0a2ef48ac1a111bcc59fda68f3946ab5d644f480fab499 in / 
# Wed, 13 May 2020 21:42:41 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:36:29 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 14 May 2020 00:36:42 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:37:27 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1fa825514fac4b3d9226a943b4954a2efb197db27c0c1c5019bf4a5f7529746e`  
		Last Modified: Wed, 13 May 2020 21:50:17 GMT  
		Size: 23.1 MB (23141460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f915ceb93db6764fe0575ee0432a41ae86c2d604b523984aed9d78d5c1234d0f`  
		Last Modified: Thu, 14 May 2020 00:47:39 GMT  
		Size: 244.5 KB (244474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8679a891a2319ab8cd948aec3e70379d339b63d0233de8ee99d38dd0ff0a27f9`  
		Last Modified: Thu, 14 May 2020 00:47:55 GMT  
		Size: 58.6 MB (58557356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:bb95612257eeef3bdeda1eb6ec5b729e68c3641c64daca4c43e9a096738f48ab
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.7 MB (47668743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96e062ad47c88c3e2daed7608ea87a8a2796b863474c47f3e7fcae8d5d8e5cd3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:42:09 GMT
ADD file:341dbc564992a44e81b3a4f399f7de14d7340a45b73c577edb78e16da2c14584 in / 
# Wed, 13 May 2020 22:42:12 GMT
CMD ["bash"]
# Thu, 14 May 2020 01:50:04 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 14 May 2020 01:50:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 01:51:55 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3b6ae894780534c0f99588e9cce4beb8fb7884b4578e6206b72f2db75116bb1c`  
		Last Modified: Wed, 13 May 2020 23:02:51 GMT  
		Size: 22.8 MB (22785361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f1dc144d71ebf5bd6087036a8c8f775c55db152b26a34c40ca01b3f46e2372`  
		Last Modified: Thu, 14 May 2020 02:11:55 GMT  
		Size: 244.5 KB (244492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc7b3ed156debf9afe549ded8235a14506c726d42c634573aea54f25e12ff092`  
		Last Modified: Thu, 14 May 2020 02:12:12 GMT  
		Size: 24.6 MB (24638890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5-slim`

```console
$ docker pull mono@sha256:baed01710cdf1d3ed52eaa00aa4035b80082a6a6256836c1ff88db42c25cdb9d
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
$ docker pull mono@sha256:a67c4cfdbe2cbfd691b5e0506c6d7c3f63e27f09611f7553437ee8be0c1540d4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78278415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bfd262ac923bb4f9148617aa8498c5ab8c4aa833de4b7c30ea774331686612e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:23:03 GMT
ADD file:08ea1ff3fcd4efc24ab4f262cfa24e55e65844f6858e41a46fe0635d247f174d in / 
# Thu, 23 Apr 2020 00:23:03 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:50:05 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 23 Apr 2020 01:50:15 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Apr 2020 01:50:43 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b248fa9f6d2ae427ad7f00de3537ab256ae7eb413565f8be0773ee9b86ef57d4`  
		Last Modified: Thu, 23 Apr 2020 00:27:46 GMT  
		Size: 22.5 MB (22513488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb8a90fcd30243429ccde1f9410482825b3cf605a11a43283d700d5d0d2c19d`  
		Last Modified: Thu, 23 Apr 2020 02:19:53 GMT  
		Size: 244.5 KB (244486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc60b582667e2deb99365fcd66c622deb3a30e7320b51aa6bed522cc774124d2`  
		Last Modified: Thu, 23 Apr 2020 02:20:08 GMT  
		Size: 55.5 MB (55520441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:2310d3d6267b9953c7c1e9246d65b092834df4f109a3e1e05210bc26ac9cc81c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.7 MB (45706656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:496109827bf18819213d5b47184b51d13344664af24925b3e975a9554cca18ff`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 22:42:50 GMT
ADD file:4d807a3f2b10f72f31b43691d51a75c26c3898b53e775bfc4bc3d08720448371 in / 
# Thu, 14 May 2020 22:42:52 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:10:37 GMT
ENV MONO_VERSION=5.20.1.34
# Fri, 15 May 2020 04:10:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 04:11:48 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8c1954048f7e4cb30320daf180f1197d278a905c20d04ff10b32f11b35b7757c`  
		Last Modified: Thu, 14 May 2020 22:50:57 GMT  
		Size: 21.2 MB (21197082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27f57444326b25b6adc5b706cae418e27ec6f1b33168ae52de8b29dbda24346`  
		Last Modified: Fri, 15 May 2020 04:22:28 GMT  
		Size: 244.5 KB (244528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca922f93721ff7b288af2ce3db01ffa707171df5bf83ae4a8b3c1df3e1da789c`  
		Last Modified: Fri, 15 May 2020 04:22:38 GMT  
		Size: 24.3 MB (24265046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:434173f3eea1e1ba04eb71d0e55c471952da67b323ed3f91ee7ea673e36d2d94
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43105063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd793e4cb8a7142b1b6735b42ab1cf3da33103e53e192c66c57c495aaa9eac80`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:19:24 GMT
ADD file:aac27626ed8520bcfd1f03f5b7aa780a4e94978b86afcc507994a8c240953561 in / 
# Wed, 13 May 2020 21:19:26 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:29:08 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 14 May 2020 00:29:28 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:30:19 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:307a7e70a6dd41fc81298d6cb2641ebfa8e7bc00b0b27f30f6559f9976a46f1e`  
		Last Modified: Wed, 13 May 2020 21:28:39 GMT  
		Size: 19.3 MB (19298476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896601cb6b4c7cbbe19d0fd80b06e911dc10440fb462364fd269f6ad65b0d878`  
		Last Modified: Thu, 14 May 2020 00:43:20 GMT  
		Size: 244.5 KB (244507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b4e2a9f08b6cddb26653d50b851091a16aa70f85f865b82163f3eda8e29c7ab`  
		Last Modified: Thu, 14 May 2020 00:43:28 GMT  
		Size: 23.6 MB (23562080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:4eafdba106027bbd748ab01b58d3f87e0b2eebfc080c28b8b2a2d058eaa9e97e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48771701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07387acae610806e811268fe2c83177e416bf4fb94cf1f4848183b3e85982fae`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:48:17 GMT
ADD file:53d95477395267e3c1059f1101e29a7d4b0fcb2bb52351542f4ac065ccb0b973 in / 
# Wed, 13 May 2020 21:48:19 GMT
CMD ["bash"]
# Thu, 14 May 2020 02:03:31 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 14 May 2020 02:03:53 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 02:04:38 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1d8af20f9b50479a890734605435a9de85d69f19b65d29c9c92f43eea2463979`  
		Last Modified: Wed, 13 May 2020 21:56:26 GMT  
		Size: 20.4 MB (20370044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7664f3bea1034c7adfeffc0216ecb4daf47c72f70db51b311a99e7a5234018e`  
		Last Modified: Thu, 14 May 2020 02:15:25 GMT  
		Size: 244.4 KB (244356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c750bc6b6bd8c0e33ee1a45079f8a7e94ad41994a1338e35987e616d46642b8`  
		Last Modified: Thu, 14 May 2020 02:15:34 GMT  
		Size: 28.2 MB (28157301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5-slim` - linux; 386

```console
$ docker pull mono@sha256:4eedd0160a1082fd7a646e7f8492c3d464e673f13c2de5306be27a915e74c232
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81943290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0efb3cfe06d5aa360834e7361d319c8589b6d5d2f55816151e0b8c68e3f8cc0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:42:40 GMT
ADD file:39f8a4c4274f123e2c0a2ef48ac1a111bcc59fda68f3946ab5d644f480fab499 in / 
# Wed, 13 May 2020 21:42:41 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:36:29 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 14 May 2020 00:36:42 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:37:27 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1fa825514fac4b3d9226a943b4954a2efb197db27c0c1c5019bf4a5f7529746e`  
		Last Modified: Wed, 13 May 2020 21:50:17 GMT  
		Size: 23.1 MB (23141460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f915ceb93db6764fe0575ee0432a41ae86c2d604b523984aed9d78d5c1234d0f`  
		Last Modified: Thu, 14 May 2020 00:47:39 GMT  
		Size: 244.5 KB (244474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8679a891a2319ab8cd948aec3e70379d339b63d0233de8ee99d38dd0ff0a27f9`  
		Last Modified: Thu, 14 May 2020 00:47:55 GMT  
		Size: 58.6 MB (58557356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:bb95612257eeef3bdeda1eb6ec5b729e68c3641c64daca4c43e9a096738f48ab
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.7 MB (47668743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96e062ad47c88c3e2daed7608ea87a8a2796b863474c47f3e7fcae8d5d8e5cd3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:42:09 GMT
ADD file:341dbc564992a44e81b3a4f399f7de14d7340a45b73c577edb78e16da2c14584 in / 
# Wed, 13 May 2020 22:42:12 GMT
CMD ["bash"]
# Thu, 14 May 2020 01:50:04 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 14 May 2020 01:50:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 01:51:55 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3b6ae894780534c0f99588e9cce4beb8fb7884b4578e6206b72f2db75116bb1c`  
		Last Modified: Wed, 13 May 2020 23:02:51 GMT  
		Size: 22.8 MB (22785361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f1dc144d71ebf5bd6087036a8c8f775c55db152b26a34c40ca01b3f46e2372`  
		Last Modified: Thu, 14 May 2020 02:11:55 GMT  
		Size: 244.5 KB (244492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc7b3ed156debf9afe549ded8235a14506c726d42c634573aea54f25e12ff092`  
		Last Modified: Thu, 14 May 2020 02:12:12 GMT  
		Size: 24.6 MB (24638890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6`

```console
$ docker pull mono@sha256:77e66aca06ed4914a850ce5a590698acdc7c2f71a197b4428a0a6fe145bb0027
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
$ docker pull mono@sha256:2351a2ba6c2228ecac8696680f65e49607432bb7fd6c0494fd254060c48f6a02
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.1 MB (235136555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59599093bfc20b4291b6019e7cd8bd648dab8dc3c341bc26001f807264ac44dc`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:23:03 GMT
ADD file:08ea1ff3fcd4efc24ab4f262cfa24e55e65844f6858e41a46fe0635d247f174d in / 
# Thu, 23 Apr 2020 00:23:03 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:48:15 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 23 Apr 2020 01:48:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Apr 2020 01:48:58 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 23 Apr 2020 01:59:28 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b248fa9f6d2ae427ad7f00de3537ab256ae7eb413565f8be0773ee9b86ef57d4`  
		Last Modified: Thu, 23 Apr 2020 00:27:46 GMT  
		Size: 22.5 MB (22513488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5f98f65ba396764fe9568783d5a5c15abaed85471ba915f7533777d9ee788d`  
		Last Modified: Thu, 23 Apr 2020 02:19:07 GMT  
		Size: 244.5 KB (244473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06df397516278d03ee36a7c24249bc8b0b57b23701952818c89538b9856c1ffb`  
		Last Modified: Thu, 23 Apr 2020 02:19:25 GMT  
		Size: 64.6 MB (64584374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e83f8e35ba5681f2772165e09a403fab75e2cb54d9c6166e85301ad905d258`  
		Last Modified: Thu, 23 Apr 2020 02:20:55 GMT  
		Size: 147.8 MB (147794220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; arm variant v5

```console
$ docker pull mono@sha256:5be1950fc69cdd2737286151d13e08b8a810ce402c4e961abec76247ef5d87f5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.7 MB (176701525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7285a10f55436a04b15962a4fe25b96046a348c1a02a15aa64d07e2369f2ed5`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 22:42:50 GMT
ADD file:4d807a3f2b10f72f31b43691d51a75c26c3898b53e775bfc4bc3d08720448371 in / 
# Thu, 14 May 2020 22:42:52 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:07:32 GMT
ENV MONO_VERSION=6.8.0.96
# Fri, 15 May 2020 04:07:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 04:08:51 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 15 May 2020 04:14:47 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8c1954048f7e4cb30320daf180f1197d278a905c20d04ff10b32f11b35b7757c`  
		Last Modified: Thu, 14 May 2020 22:50:57 GMT  
		Size: 21.2 MB (21197082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7009fb73261c04c568d9dd5c1b839a02f5d97fea7f8c21705c8091eb1b6b5b6d`  
		Last Modified: Fri, 15 May 2020 04:21:54 GMT  
		Size: 244.5 KB (244519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b237016212e8e87ef0d32354521bfb76ce82ce991d8c6cc90ee0dcd82cc0392e`  
		Last Modified: Fri, 15 May 2020 04:22:04 GMT  
		Size: 25.4 MB (25368245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f7186fdafac062d1af6c86d4fca2df0b62f320aec72fcbbd7b8cb4d6fcf467`  
		Last Modified: Fri, 15 May 2020 04:23:35 GMT  
		Size: 129.9 MB (129891679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; arm variant v7

```console
$ docker pull mono@sha256:55ef6d96d85e1d0e3aca832b8c2a7a0b7da50bffa2dacf77542fbd7aff27a559
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.7 MB (172707764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc9acd8a77a391a80d27014968c3dfe08186f34930cc569f44c35d2a7a09b22c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:19:24 GMT
ADD file:aac27626ed8520bcfd1f03f5b7aa780a4e94978b86afcc507994a8c240953561 in / 
# Wed, 13 May 2020 21:19:26 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:26:29 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 14 May 2020 00:26:48 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:27:40 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 00:33:55 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:307a7e70a6dd41fc81298d6cb2641ebfa8e7bc00b0b27f30f6559f9976a46f1e`  
		Last Modified: Wed, 13 May 2020 21:28:39 GMT  
		Size: 19.3 MB (19298476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91631fd0b2baefb452095603fc22b8be62f3657d1ae76086f6318c48f36cae25`  
		Last Modified: Thu, 14 May 2020 00:42:46 GMT  
		Size: 244.5 KB (244516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707e4565b23eaef80b85f8caf65db746d521af83f33888a710630ea91c60de18`  
		Last Modified: Thu, 14 May 2020 00:42:55 GMT  
		Size: 24.6 MB (24608714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a42be730e2ad23f35deb8b93a0913d13edb02be20a73fa837770d36acbbf74`  
		Last Modified: Thu, 14 May 2020 00:44:20 GMT  
		Size: 128.6 MB (128556058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:cbc1409b11ea1fd492744b6396ef5a9afa4bd427de25d89ea8406fbd9189d0a7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.7 MB (194747627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:939138ef9b9d3ec1af2baae95869f7cf8c66020511a3bb70138be5e5dd8450f2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:48:17 GMT
ADD file:53d95477395267e3c1059f1101e29a7d4b0fcb2bb52351542f4ac065ccb0b973 in / 
# Wed, 13 May 2020 21:48:19 GMT
CMD ["bash"]
# Thu, 14 May 2020 02:00:25 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 14 May 2020 02:00:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 02:01:47 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 02:07:30 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1d8af20f9b50479a890734605435a9de85d69f19b65d29c9c92f43eea2463979`  
		Last Modified: Wed, 13 May 2020 21:56:26 GMT  
		Size: 20.4 MB (20370044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5f88aa673180f3a9e54d2d3fc9c67565c9545d3072c1a42eee0eda3192c039`  
		Last Modified: Thu, 14 May 2020 02:14:51 GMT  
		Size: 244.4 KB (244366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5622468da1cdc4403ec0072a3093de5483f907e82f7e7493e9bcf66765d2367`  
		Last Modified: Thu, 14 May 2020 02:14:59 GMT  
		Size: 29.4 MB (29419827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a79b7e06bf892f3f0e1c21e1bdc62517abc6fd4fd31a2f0be27e369398f2d0ca`  
		Last Modified: Thu, 14 May 2020 02:16:28 GMT  
		Size: 144.7 MB (144713390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; 386

```console
$ docker pull mono@sha256:91becebb427753ead531605be391b0528b1b8176f46762f3fb896b58fbf493f5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.5 MB (243509833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d912f07467de168fbaadffea2b2be97d24f40de4675c1ef98b3b7c70f274b9c5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:42:40 GMT
ADD file:39f8a4c4274f123e2c0a2ef48ac1a111bcc59fda68f3946ab5d644f480fab499 in / 
# Wed, 13 May 2020 21:42:41 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:33:55 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 14 May 2020 00:34:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:34:57 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 00:40:29 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1fa825514fac4b3d9226a943b4954a2efb197db27c0c1c5019bf4a5f7529746e`  
		Last Modified: Wed, 13 May 2020 21:50:17 GMT  
		Size: 23.1 MB (23141460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eac1a2c3c2e8b2376318177cabaab6efa4884e4a1262be8019864dd8d79b02d`  
		Last Modified: Thu, 14 May 2020 00:46:50 GMT  
		Size: 244.5 KB (244476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0517e1b7f3b81bc5e21be055d429fe5465bebb94609a0824c5064f1c2198ea92`  
		Last Modified: Thu, 14 May 2020 00:47:08 GMT  
		Size: 68.6 MB (68630757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b33be2fe9551abfc1002c4bad0c8ce971f275c3ca146936540551c5776b4fd4`  
		Last Modified: Thu, 14 May 2020 00:49:07 GMT  
		Size: 151.5 MB (151493140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; ppc64le

```console
$ docker pull mono@sha256:28211181008fc8a25dbc12b5f75fd4857e92af22ee4716fd13064027ba80c113
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.0 MB (178995744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcbdcf050885aeb282b85d9942bee597145d594577643da02a09cb638cd2edb9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:42:09 GMT
ADD file:341dbc564992a44e81b3a4f399f7de14d7340a45b73c577edb78e16da2c14584 in / 
# Wed, 13 May 2020 22:42:12 GMT
CMD ["bash"]
# Thu, 14 May 2020 01:44:38 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 14 May 2020 01:45:44 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 01:47:00 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 01:57:53 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3b6ae894780534c0f99588e9cce4beb8fb7884b4578e6206b72f2db75116bb1c`  
		Last Modified: Wed, 13 May 2020 23:02:51 GMT  
		Size: 22.8 MB (22785361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0d85174db6ce48c895d3bbf3f847e1cba986fc66e705bd86bb13e3fbf73286`  
		Last Modified: Thu, 14 May 2020 02:10:48 GMT  
		Size: 244.5 KB (244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6124cc55d37923fca85643397621b030dae64f93ddf2c45ed9704bf9e9e5d141`  
		Last Modified: Thu, 14 May 2020 02:11:06 GMT  
		Size: 25.8 MB (25775347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64bc6db4438da29e772ebf533c91b52b035c322c12bf45899c0cbcff8a42ba24`  
		Last Modified: Thu, 14 May 2020 02:13:51 GMT  
		Size: 130.2 MB (130190503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.6`

```console
$ docker pull mono@sha256:a15362b5a7bda5bc2e7d0633e029cdfaa22f424674688850f78581aa2d0a8e64
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
$ docker pull mono@sha256:3ea2f2740b1f0ff78b3a90eb8ff531a9763c181158b7c329f97ea04e8d213dec
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.0 MB (233037465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53213d4543a9b55852762487dcc6eca75d1a42efa19c79750579e082c5a2b536`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:23:03 GMT
ADD file:08ea1ff3fcd4efc24ab4f262cfa24e55e65844f6858e41a46fe0635d247f174d in / 
# Thu, 23 Apr 2020 00:23:03 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:49:10 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 23 Apr 2020 01:49:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Apr 2020 01:49:54 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 23 Apr 2020 02:08:52 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b248fa9f6d2ae427ad7f00de3537ab256ae7eb413565f8be0773ee9b86ef57d4`  
		Last Modified: Thu, 23 Apr 2020 00:27:46 GMT  
		Size: 22.5 MB (22513488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485f7d13fbf11ea37b0afce7d19a2618fdef52ce09eeed3be5d6c2cba3ff89bc`  
		Last Modified: Thu, 23 Apr 2020 02:19:31 GMT  
		Size: 244.5 KB (244478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a4778f199830e07df7630da3469e683d4db678333a3b3d661eaadaf4866f90`  
		Last Modified: Thu, 23 Apr 2020 02:19:48 GMT  
		Size: 63.0 MB (62971564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8309b0c95463c87a0e326685c37fc42adbe87d5e1da3032cd92d8e56c50c6440`  
		Last Modified: Thu, 23 Apr 2020 02:21:38 GMT  
		Size: 147.3 MB (147307935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6` - linux; arm variant v5

```console
$ docker pull mono@sha256:f3807669d504f8b88ae732bd6f8ac7cdac47eb3846b9c0b101f2d8803121b96e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.5 MB (176504642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3f271d96ba92201aaaa39ee3f7087ca34adb53b432460f9b861b11e07ae9297`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 22:42:50 GMT
ADD file:4d807a3f2b10f72f31b43691d51a75c26c3898b53e775bfc4bc3d08720448371 in / 
# Thu, 14 May 2020 22:42:52 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:09:05 GMT
ENV MONO_VERSION=6.6.0.161
# Fri, 15 May 2020 04:09:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 04:10:18 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 15 May 2020 04:17:54 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8c1954048f7e4cb30320daf180f1197d278a905c20d04ff10b32f11b35b7757c`  
		Last Modified: Thu, 14 May 2020 22:50:57 GMT  
		Size: 21.2 MB (21197082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e964c01e015bfb89fdb3e72b98f7ff67658939e38fb7ece25a29bcbb3082fe30`  
		Last Modified: Fri, 15 May 2020 04:22:13 GMT  
		Size: 244.5 KB (244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2e95a1ec1e22ad6830069d161ad74d7ea8b905748f4762cb117bbd0a207e47`  
		Last Modified: Fri, 15 May 2020 04:22:23 GMT  
		Size: 25.4 MB (25415001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1960b29e22a1fbf8eff093c13a84e979e62692b108cf5d5caced120ac28f4783`  
		Last Modified: Fri, 15 May 2020 04:24:33 GMT  
		Size: 129.6 MB (129648026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6` - linux; arm variant v7

```console
$ docker pull mono@sha256:55cd43afcfa894c9229f88632194080eb7c6c59e66cab9f389ce2cd72b31b53a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.5 MB (172507612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fed5f41cfca4aefe3261e6c7b988ecd45ff10da7201eda8152a78f90160084a3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:19:24 GMT
ADD file:aac27626ed8520bcfd1f03f5b7aa780a4e94978b86afcc507994a8c240953561 in / 
# Wed, 13 May 2020 21:19:26 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:27:48 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 14 May 2020 00:28:08 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:29:00 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 00:38:07 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:307a7e70a6dd41fc81298d6cb2641ebfa8e7bc00b0b27f30f6559f9976a46f1e`  
		Last Modified: Wed, 13 May 2020 21:28:39 GMT  
		Size: 19.3 MB (19298476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9121d426ba6b2669d1e4a4ee3c9060b0cfc6fded57610512fc7818bd31efc9`  
		Last Modified: Thu, 14 May 2020 00:43:03 GMT  
		Size: 244.5 KB (244535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61917c719f7757620481cf5c7275ab522044d462e7fffb609c8144d02290709b`  
		Last Modified: Thu, 14 May 2020 00:43:12 GMT  
		Size: 24.6 MB (24648559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cea1db341dd50dd87ea55a37b5d24d7c44260690be6f29622105e8ed87fc458`  
		Last Modified: Thu, 14 May 2020 00:45:13 GMT  
		Size: 128.3 MB (128316042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:33758ec3af3790e745b7e45999695d8443fcf2612a94e53a5ac87aa39f07c1b3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.4 MB (194394846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e92735237db17e218404d819ff036271ab8e952020efe6189897eced3703c5f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:48:17 GMT
ADD file:53d95477395267e3c1059f1101e29a7d4b0fcb2bb52351542f4ac065ccb0b973 in / 
# Wed, 13 May 2020 21:48:19 GMT
CMD ["bash"]
# Thu, 14 May 2020 02:01:58 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 14 May 2020 02:02:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 02:03:19 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 02:10:56 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1d8af20f9b50479a890734605435a9de85d69f19b65d29c9c92f43eea2463979`  
		Last Modified: Wed, 13 May 2020 21:56:26 GMT  
		Size: 20.4 MB (20370044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2377cccc819b93b6367c694d4531f6d0f256636a62effd3f8592bd961c6c21fa`  
		Last Modified: Thu, 14 May 2020 02:15:09 GMT  
		Size: 244.4 KB (244352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb8d9c0ce16dd2186df4ffb514e93303927dd9ad10d5cf79fba2a002b028038`  
		Last Modified: Thu, 14 May 2020 02:15:18 GMT  
		Size: 29.4 MB (29438964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0b27b22e2c8f7c9df478480fac8f22e6f7395c3dbe28c8be650790fa8386a9`  
		Last Modified: Thu, 14 May 2020 02:17:24 GMT  
		Size: 144.3 MB (144341486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6` - linux; 386

```console
$ docker pull mono@sha256:87935bbcdb147f4791ae4d6165adad2ad217ef7e2d63505bd6f92f19c1902551
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.3 MB (241295007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad8575f54d705024e8d6be88215703f77757dfa8d25bdff895034b446080daeb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:42:40 GMT
ADD file:39f8a4c4274f123e2c0a2ef48ac1a111bcc59fda68f3946ab5d644f480fab499 in / 
# Wed, 13 May 2020 21:42:41 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:35:12 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 14 May 2020 00:35:31 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:36:22 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 00:43:35 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1fa825514fac4b3d9226a943b4954a2efb197db27c0c1c5019bf4a5f7529746e`  
		Last Modified: Wed, 13 May 2020 21:50:17 GMT  
		Size: 23.1 MB (23141460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43163d1e26ca7bae351b647978e6e525a5f6d5979bd3fdf9ec4cc8c55f85d3a8`  
		Last Modified: Thu, 14 May 2020 00:47:14 GMT  
		Size: 244.5 KB (244483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb7945cfea3f1977c9997db158a1e3e46a16bb70d2580c4591d401940b1786e`  
		Last Modified: Thu, 14 May 2020 00:47:32 GMT  
		Size: 66.7 MB (66747691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29209c32232d73b1849a9cf914409550c9d9d675516366e9091d2097ef8225e5`  
		Last Modified: Thu, 14 May 2020 00:50:11 GMT  
		Size: 151.2 MB (151161373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6` - linux; ppc64le

```console
$ docker pull mono@sha256:efa950ab81f35184991cc64c555e369e358341729408493f4e6e917a9666dc50
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.8 MB (178799782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:effa94527570c1c067f88bc7de296edd263537d5abe9bcec4ca0010ca6c55462`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:42:09 GMT
ADD file:341dbc564992a44e81b3a4f399f7de14d7340a45b73c577edb78e16da2c14584 in / 
# Wed, 13 May 2020 22:42:12 GMT
CMD ["bash"]
# Thu, 14 May 2020 01:47:21 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 14 May 2020 01:48:31 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 01:49:49 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 02:04:18 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3b6ae894780534c0f99588e9cce4beb8fb7884b4578e6206b72f2db75116bb1c`  
		Last Modified: Wed, 13 May 2020 23:02:51 GMT  
		Size: 22.8 MB (22785361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f954c6ba09f38f1b2c8c4a6b3d1d478763bccd68a9038c72437436ac2092cad`  
		Last Modified: Thu, 14 May 2020 02:11:22 GMT  
		Size: 244.6 KB (244550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8516e67eac3bdcee3a32e15d6d71edfb984e8c59ad0c98f7a6c7b015218f85da`  
		Last Modified: Thu, 14 May 2020 02:11:43 GMT  
		Size: 25.8 MB (25827650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab0d035f0a9e245ea6a10deaaf47a7697acc1800bdaf8eafc7c263a467d07f1`  
		Last Modified: Thu, 14 May 2020 02:15:35 GMT  
		Size: 129.9 MB (129942221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.6.0`

```console
$ docker pull mono@sha256:a15362b5a7bda5bc2e7d0633e029cdfaa22f424674688850f78581aa2d0a8e64
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
$ docker pull mono@sha256:3ea2f2740b1f0ff78b3a90eb8ff531a9763c181158b7c329f97ea04e8d213dec
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.0 MB (233037465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53213d4543a9b55852762487dcc6eca75d1a42efa19c79750579e082c5a2b536`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:23:03 GMT
ADD file:08ea1ff3fcd4efc24ab4f262cfa24e55e65844f6858e41a46fe0635d247f174d in / 
# Thu, 23 Apr 2020 00:23:03 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:49:10 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 23 Apr 2020 01:49:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Apr 2020 01:49:54 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 23 Apr 2020 02:08:52 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b248fa9f6d2ae427ad7f00de3537ab256ae7eb413565f8be0773ee9b86ef57d4`  
		Last Modified: Thu, 23 Apr 2020 00:27:46 GMT  
		Size: 22.5 MB (22513488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485f7d13fbf11ea37b0afce7d19a2618fdef52ce09eeed3be5d6c2cba3ff89bc`  
		Last Modified: Thu, 23 Apr 2020 02:19:31 GMT  
		Size: 244.5 KB (244478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a4778f199830e07df7630da3469e683d4db678333a3b3d661eaadaf4866f90`  
		Last Modified: Thu, 23 Apr 2020 02:19:48 GMT  
		Size: 63.0 MB (62971564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8309b0c95463c87a0e326685c37fc42adbe87d5e1da3032cd92d8e56c50c6440`  
		Last Modified: Thu, 23 Apr 2020 02:21:38 GMT  
		Size: 147.3 MB (147307935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0` - linux; arm variant v5

```console
$ docker pull mono@sha256:f3807669d504f8b88ae732bd6f8ac7cdac47eb3846b9c0b101f2d8803121b96e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.5 MB (176504642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3f271d96ba92201aaaa39ee3f7087ca34adb53b432460f9b861b11e07ae9297`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 22:42:50 GMT
ADD file:4d807a3f2b10f72f31b43691d51a75c26c3898b53e775bfc4bc3d08720448371 in / 
# Thu, 14 May 2020 22:42:52 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:09:05 GMT
ENV MONO_VERSION=6.6.0.161
# Fri, 15 May 2020 04:09:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 04:10:18 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 15 May 2020 04:17:54 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8c1954048f7e4cb30320daf180f1197d278a905c20d04ff10b32f11b35b7757c`  
		Last Modified: Thu, 14 May 2020 22:50:57 GMT  
		Size: 21.2 MB (21197082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e964c01e015bfb89fdb3e72b98f7ff67658939e38fb7ece25a29bcbb3082fe30`  
		Last Modified: Fri, 15 May 2020 04:22:13 GMT  
		Size: 244.5 KB (244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2e95a1ec1e22ad6830069d161ad74d7ea8b905748f4762cb117bbd0a207e47`  
		Last Modified: Fri, 15 May 2020 04:22:23 GMT  
		Size: 25.4 MB (25415001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1960b29e22a1fbf8eff093c13a84e979e62692b108cf5d5caced120ac28f4783`  
		Last Modified: Fri, 15 May 2020 04:24:33 GMT  
		Size: 129.6 MB (129648026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0` - linux; arm variant v7

```console
$ docker pull mono@sha256:55cd43afcfa894c9229f88632194080eb7c6c59e66cab9f389ce2cd72b31b53a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.5 MB (172507612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fed5f41cfca4aefe3261e6c7b988ecd45ff10da7201eda8152a78f90160084a3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:19:24 GMT
ADD file:aac27626ed8520bcfd1f03f5b7aa780a4e94978b86afcc507994a8c240953561 in / 
# Wed, 13 May 2020 21:19:26 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:27:48 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 14 May 2020 00:28:08 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:29:00 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 00:38:07 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:307a7e70a6dd41fc81298d6cb2641ebfa8e7bc00b0b27f30f6559f9976a46f1e`  
		Last Modified: Wed, 13 May 2020 21:28:39 GMT  
		Size: 19.3 MB (19298476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9121d426ba6b2669d1e4a4ee3c9060b0cfc6fded57610512fc7818bd31efc9`  
		Last Modified: Thu, 14 May 2020 00:43:03 GMT  
		Size: 244.5 KB (244535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61917c719f7757620481cf5c7275ab522044d462e7fffb609c8144d02290709b`  
		Last Modified: Thu, 14 May 2020 00:43:12 GMT  
		Size: 24.6 MB (24648559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cea1db341dd50dd87ea55a37b5d24d7c44260690be6f29622105e8ed87fc458`  
		Last Modified: Thu, 14 May 2020 00:45:13 GMT  
		Size: 128.3 MB (128316042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:33758ec3af3790e745b7e45999695d8443fcf2612a94e53a5ac87aa39f07c1b3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.4 MB (194394846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e92735237db17e218404d819ff036271ab8e952020efe6189897eced3703c5f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:48:17 GMT
ADD file:53d95477395267e3c1059f1101e29a7d4b0fcb2bb52351542f4ac065ccb0b973 in / 
# Wed, 13 May 2020 21:48:19 GMT
CMD ["bash"]
# Thu, 14 May 2020 02:01:58 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 14 May 2020 02:02:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 02:03:19 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 02:10:56 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1d8af20f9b50479a890734605435a9de85d69f19b65d29c9c92f43eea2463979`  
		Last Modified: Wed, 13 May 2020 21:56:26 GMT  
		Size: 20.4 MB (20370044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2377cccc819b93b6367c694d4531f6d0f256636a62effd3f8592bd961c6c21fa`  
		Last Modified: Thu, 14 May 2020 02:15:09 GMT  
		Size: 244.4 KB (244352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb8d9c0ce16dd2186df4ffb514e93303927dd9ad10d5cf79fba2a002b028038`  
		Last Modified: Thu, 14 May 2020 02:15:18 GMT  
		Size: 29.4 MB (29438964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0b27b22e2c8f7c9df478480fac8f22e6f7395c3dbe28c8be650790fa8386a9`  
		Last Modified: Thu, 14 May 2020 02:17:24 GMT  
		Size: 144.3 MB (144341486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0` - linux; 386

```console
$ docker pull mono@sha256:87935bbcdb147f4791ae4d6165adad2ad217ef7e2d63505bd6f92f19c1902551
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.3 MB (241295007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad8575f54d705024e8d6be88215703f77757dfa8d25bdff895034b446080daeb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:42:40 GMT
ADD file:39f8a4c4274f123e2c0a2ef48ac1a111bcc59fda68f3946ab5d644f480fab499 in / 
# Wed, 13 May 2020 21:42:41 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:35:12 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 14 May 2020 00:35:31 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:36:22 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 00:43:35 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1fa825514fac4b3d9226a943b4954a2efb197db27c0c1c5019bf4a5f7529746e`  
		Last Modified: Wed, 13 May 2020 21:50:17 GMT  
		Size: 23.1 MB (23141460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43163d1e26ca7bae351b647978e6e525a5f6d5979bd3fdf9ec4cc8c55f85d3a8`  
		Last Modified: Thu, 14 May 2020 00:47:14 GMT  
		Size: 244.5 KB (244483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb7945cfea3f1977c9997db158a1e3e46a16bb70d2580c4591d401940b1786e`  
		Last Modified: Thu, 14 May 2020 00:47:32 GMT  
		Size: 66.7 MB (66747691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29209c32232d73b1849a9cf914409550c9d9d675516366e9091d2097ef8225e5`  
		Last Modified: Thu, 14 May 2020 00:50:11 GMT  
		Size: 151.2 MB (151161373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0` - linux; ppc64le

```console
$ docker pull mono@sha256:efa950ab81f35184991cc64c555e369e358341729408493f4e6e917a9666dc50
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.8 MB (178799782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:effa94527570c1c067f88bc7de296edd263537d5abe9bcec4ca0010ca6c55462`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:42:09 GMT
ADD file:341dbc564992a44e81b3a4f399f7de14d7340a45b73c577edb78e16da2c14584 in / 
# Wed, 13 May 2020 22:42:12 GMT
CMD ["bash"]
# Thu, 14 May 2020 01:47:21 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 14 May 2020 01:48:31 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 01:49:49 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 02:04:18 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3b6ae894780534c0f99588e9cce4beb8fb7884b4578e6206b72f2db75116bb1c`  
		Last Modified: Wed, 13 May 2020 23:02:51 GMT  
		Size: 22.8 MB (22785361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f954c6ba09f38f1b2c8c4a6b3d1d478763bccd68a9038c72437436ac2092cad`  
		Last Modified: Thu, 14 May 2020 02:11:22 GMT  
		Size: 244.6 KB (244550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8516e67eac3bdcee3a32e15d6d71edfb984e8c59ad0c98f7a6c7b015218f85da`  
		Last Modified: Thu, 14 May 2020 02:11:43 GMT  
		Size: 25.8 MB (25827650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab0d035f0a9e245ea6a10deaaf47a7697acc1800bdaf8eafc7c263a467d07f1`  
		Last Modified: Thu, 14 May 2020 02:15:35 GMT  
		Size: 129.9 MB (129942221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.6.0.161`

```console
$ docker pull mono@sha256:a15362b5a7bda5bc2e7d0633e029cdfaa22f424674688850f78581aa2d0a8e64
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
$ docker pull mono@sha256:3ea2f2740b1f0ff78b3a90eb8ff531a9763c181158b7c329f97ea04e8d213dec
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.0 MB (233037465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53213d4543a9b55852762487dcc6eca75d1a42efa19c79750579e082c5a2b536`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:23:03 GMT
ADD file:08ea1ff3fcd4efc24ab4f262cfa24e55e65844f6858e41a46fe0635d247f174d in / 
# Thu, 23 Apr 2020 00:23:03 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:49:10 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 23 Apr 2020 01:49:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Apr 2020 01:49:54 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 23 Apr 2020 02:08:52 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b248fa9f6d2ae427ad7f00de3537ab256ae7eb413565f8be0773ee9b86ef57d4`  
		Last Modified: Thu, 23 Apr 2020 00:27:46 GMT  
		Size: 22.5 MB (22513488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485f7d13fbf11ea37b0afce7d19a2618fdef52ce09eeed3be5d6c2cba3ff89bc`  
		Last Modified: Thu, 23 Apr 2020 02:19:31 GMT  
		Size: 244.5 KB (244478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a4778f199830e07df7630da3469e683d4db678333a3b3d661eaadaf4866f90`  
		Last Modified: Thu, 23 Apr 2020 02:19:48 GMT  
		Size: 63.0 MB (62971564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8309b0c95463c87a0e326685c37fc42adbe87d5e1da3032cd92d8e56c50c6440`  
		Last Modified: Thu, 23 Apr 2020 02:21:38 GMT  
		Size: 147.3 MB (147307935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0.161` - linux; arm variant v5

```console
$ docker pull mono@sha256:f3807669d504f8b88ae732bd6f8ac7cdac47eb3846b9c0b101f2d8803121b96e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.5 MB (176504642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3f271d96ba92201aaaa39ee3f7087ca34adb53b432460f9b861b11e07ae9297`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 22:42:50 GMT
ADD file:4d807a3f2b10f72f31b43691d51a75c26c3898b53e775bfc4bc3d08720448371 in / 
# Thu, 14 May 2020 22:42:52 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:09:05 GMT
ENV MONO_VERSION=6.6.0.161
# Fri, 15 May 2020 04:09:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 04:10:18 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 15 May 2020 04:17:54 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8c1954048f7e4cb30320daf180f1197d278a905c20d04ff10b32f11b35b7757c`  
		Last Modified: Thu, 14 May 2020 22:50:57 GMT  
		Size: 21.2 MB (21197082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e964c01e015bfb89fdb3e72b98f7ff67658939e38fb7ece25a29bcbb3082fe30`  
		Last Modified: Fri, 15 May 2020 04:22:13 GMT  
		Size: 244.5 KB (244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2e95a1ec1e22ad6830069d161ad74d7ea8b905748f4762cb117bbd0a207e47`  
		Last Modified: Fri, 15 May 2020 04:22:23 GMT  
		Size: 25.4 MB (25415001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1960b29e22a1fbf8eff093c13a84e979e62692b108cf5d5caced120ac28f4783`  
		Last Modified: Fri, 15 May 2020 04:24:33 GMT  
		Size: 129.6 MB (129648026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0.161` - linux; arm variant v7

```console
$ docker pull mono@sha256:55cd43afcfa894c9229f88632194080eb7c6c59e66cab9f389ce2cd72b31b53a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.5 MB (172507612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fed5f41cfca4aefe3261e6c7b988ecd45ff10da7201eda8152a78f90160084a3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:19:24 GMT
ADD file:aac27626ed8520bcfd1f03f5b7aa780a4e94978b86afcc507994a8c240953561 in / 
# Wed, 13 May 2020 21:19:26 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:27:48 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 14 May 2020 00:28:08 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:29:00 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 00:38:07 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:307a7e70a6dd41fc81298d6cb2641ebfa8e7bc00b0b27f30f6559f9976a46f1e`  
		Last Modified: Wed, 13 May 2020 21:28:39 GMT  
		Size: 19.3 MB (19298476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9121d426ba6b2669d1e4a4ee3c9060b0cfc6fded57610512fc7818bd31efc9`  
		Last Modified: Thu, 14 May 2020 00:43:03 GMT  
		Size: 244.5 KB (244535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61917c719f7757620481cf5c7275ab522044d462e7fffb609c8144d02290709b`  
		Last Modified: Thu, 14 May 2020 00:43:12 GMT  
		Size: 24.6 MB (24648559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cea1db341dd50dd87ea55a37b5d24d7c44260690be6f29622105e8ed87fc458`  
		Last Modified: Thu, 14 May 2020 00:45:13 GMT  
		Size: 128.3 MB (128316042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0.161` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:33758ec3af3790e745b7e45999695d8443fcf2612a94e53a5ac87aa39f07c1b3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.4 MB (194394846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e92735237db17e218404d819ff036271ab8e952020efe6189897eced3703c5f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:48:17 GMT
ADD file:53d95477395267e3c1059f1101e29a7d4b0fcb2bb52351542f4ac065ccb0b973 in / 
# Wed, 13 May 2020 21:48:19 GMT
CMD ["bash"]
# Thu, 14 May 2020 02:01:58 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 14 May 2020 02:02:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 02:03:19 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 02:10:56 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1d8af20f9b50479a890734605435a9de85d69f19b65d29c9c92f43eea2463979`  
		Last Modified: Wed, 13 May 2020 21:56:26 GMT  
		Size: 20.4 MB (20370044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2377cccc819b93b6367c694d4531f6d0f256636a62effd3f8592bd961c6c21fa`  
		Last Modified: Thu, 14 May 2020 02:15:09 GMT  
		Size: 244.4 KB (244352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb8d9c0ce16dd2186df4ffb514e93303927dd9ad10d5cf79fba2a002b028038`  
		Last Modified: Thu, 14 May 2020 02:15:18 GMT  
		Size: 29.4 MB (29438964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0b27b22e2c8f7c9df478480fac8f22e6f7395c3dbe28c8be650790fa8386a9`  
		Last Modified: Thu, 14 May 2020 02:17:24 GMT  
		Size: 144.3 MB (144341486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0.161` - linux; 386

```console
$ docker pull mono@sha256:87935bbcdb147f4791ae4d6165adad2ad217ef7e2d63505bd6f92f19c1902551
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.3 MB (241295007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad8575f54d705024e8d6be88215703f77757dfa8d25bdff895034b446080daeb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:42:40 GMT
ADD file:39f8a4c4274f123e2c0a2ef48ac1a111bcc59fda68f3946ab5d644f480fab499 in / 
# Wed, 13 May 2020 21:42:41 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:35:12 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 14 May 2020 00:35:31 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:36:22 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 00:43:35 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1fa825514fac4b3d9226a943b4954a2efb197db27c0c1c5019bf4a5f7529746e`  
		Last Modified: Wed, 13 May 2020 21:50:17 GMT  
		Size: 23.1 MB (23141460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43163d1e26ca7bae351b647978e6e525a5f6d5979bd3fdf9ec4cc8c55f85d3a8`  
		Last Modified: Thu, 14 May 2020 00:47:14 GMT  
		Size: 244.5 KB (244483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb7945cfea3f1977c9997db158a1e3e46a16bb70d2580c4591d401940b1786e`  
		Last Modified: Thu, 14 May 2020 00:47:32 GMT  
		Size: 66.7 MB (66747691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29209c32232d73b1849a9cf914409550c9d9d675516366e9091d2097ef8225e5`  
		Last Modified: Thu, 14 May 2020 00:50:11 GMT  
		Size: 151.2 MB (151161373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0.161` - linux; ppc64le

```console
$ docker pull mono@sha256:efa950ab81f35184991cc64c555e369e358341729408493f4e6e917a9666dc50
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.8 MB (178799782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:effa94527570c1c067f88bc7de296edd263537d5abe9bcec4ca0010ca6c55462`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:42:09 GMT
ADD file:341dbc564992a44e81b3a4f399f7de14d7340a45b73c577edb78e16da2c14584 in / 
# Wed, 13 May 2020 22:42:12 GMT
CMD ["bash"]
# Thu, 14 May 2020 01:47:21 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 14 May 2020 01:48:31 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 01:49:49 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 02:04:18 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3b6ae894780534c0f99588e9cce4beb8fb7884b4578e6206b72f2db75116bb1c`  
		Last Modified: Wed, 13 May 2020 23:02:51 GMT  
		Size: 22.8 MB (22785361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f954c6ba09f38f1b2c8c4a6b3d1d478763bccd68a9038c72437436ac2092cad`  
		Last Modified: Thu, 14 May 2020 02:11:22 GMT  
		Size: 244.6 KB (244550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8516e67eac3bdcee3a32e15d6d71edfb984e8c59ad0c98f7a6c7b015218f85da`  
		Last Modified: Thu, 14 May 2020 02:11:43 GMT  
		Size: 25.8 MB (25827650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab0d035f0a9e245ea6a10deaaf47a7697acc1800bdaf8eafc7c263a467d07f1`  
		Last Modified: Thu, 14 May 2020 02:15:35 GMT  
		Size: 129.9 MB (129942221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.6.0.161-slim`

```console
$ docker pull mono@sha256:9fb10f64ea980e0c3a7d27488c75e4c91bff8660fc519dc5887311bd10b17c9a
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
$ docker pull mono@sha256:e03c444502022dd73573d892596a6bb4cab789a4f66a61e9ee6dffd8ff9ef1c5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.7 MB (85729530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fa672f39c92e71df557f447a2ab1ebfcf309747e3f6f883f2ccf571ac14d999`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:23:03 GMT
ADD file:08ea1ff3fcd4efc24ab4f262cfa24e55e65844f6858e41a46fe0635d247f174d in / 
# Thu, 23 Apr 2020 00:23:03 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:49:10 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 23 Apr 2020 01:49:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Apr 2020 01:49:54 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b248fa9f6d2ae427ad7f00de3537ab256ae7eb413565f8be0773ee9b86ef57d4`  
		Last Modified: Thu, 23 Apr 2020 00:27:46 GMT  
		Size: 22.5 MB (22513488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485f7d13fbf11ea37b0afce7d19a2618fdef52ce09eeed3be5d6c2cba3ff89bc`  
		Last Modified: Thu, 23 Apr 2020 02:19:31 GMT  
		Size: 244.5 KB (244478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a4778f199830e07df7630da3469e683d4db678333a3b3d661eaadaf4866f90`  
		Last Modified: Thu, 23 Apr 2020 02:19:48 GMT  
		Size: 63.0 MB (62971564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0.161-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:41d695b38491b1206c44e7add06393bac07434a32edd1e3f8edc4d855878fc16
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46856616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc846d0fc08a43fbf49f1b11aeddcf98fbb07227a218782a032113b042488f01`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 22:42:50 GMT
ADD file:4d807a3f2b10f72f31b43691d51a75c26c3898b53e775bfc4bc3d08720448371 in / 
# Thu, 14 May 2020 22:42:52 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:09:05 GMT
ENV MONO_VERSION=6.6.0.161
# Fri, 15 May 2020 04:09:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 04:10:18 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8c1954048f7e4cb30320daf180f1197d278a905c20d04ff10b32f11b35b7757c`  
		Last Modified: Thu, 14 May 2020 22:50:57 GMT  
		Size: 21.2 MB (21197082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e964c01e015bfb89fdb3e72b98f7ff67658939e38fb7ece25a29bcbb3082fe30`  
		Last Modified: Fri, 15 May 2020 04:22:13 GMT  
		Size: 244.5 KB (244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2e95a1ec1e22ad6830069d161ad74d7ea8b905748f4762cb117bbd0a207e47`  
		Last Modified: Fri, 15 May 2020 04:22:23 GMT  
		Size: 25.4 MB (25415001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0.161-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:15ed5f9bc060975b061446059a1dc1ca7e6605c5baaed855eb1c66328d765095
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44191570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51da61aca945ec4b12db96ecb19125c0c35f45c1a6200d14eef21a5e2a59c159`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:19:24 GMT
ADD file:aac27626ed8520bcfd1f03f5b7aa780a4e94978b86afcc507994a8c240953561 in / 
# Wed, 13 May 2020 21:19:26 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:27:48 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 14 May 2020 00:28:08 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:29:00 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:307a7e70a6dd41fc81298d6cb2641ebfa8e7bc00b0b27f30f6559f9976a46f1e`  
		Last Modified: Wed, 13 May 2020 21:28:39 GMT  
		Size: 19.3 MB (19298476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9121d426ba6b2669d1e4a4ee3c9060b0cfc6fded57610512fc7818bd31efc9`  
		Last Modified: Thu, 14 May 2020 00:43:03 GMT  
		Size: 244.5 KB (244535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61917c719f7757620481cf5c7275ab522044d462e7fffb609c8144d02290709b`  
		Last Modified: Thu, 14 May 2020 00:43:12 GMT  
		Size: 24.6 MB (24648559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0.161-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:f5c151197464621e2d06dc4abced8ee231ca8112395954e58566df29ecaa08a5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50053360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d165094a4d3c18123e7b99966e3136748b491a25be3452b0f7479cd8a705bd59`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:48:17 GMT
ADD file:53d95477395267e3c1059f1101e29a7d4b0fcb2bb52351542f4ac065ccb0b973 in / 
# Wed, 13 May 2020 21:48:19 GMT
CMD ["bash"]
# Thu, 14 May 2020 02:01:58 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 14 May 2020 02:02:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 02:03:19 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1d8af20f9b50479a890734605435a9de85d69f19b65d29c9c92f43eea2463979`  
		Last Modified: Wed, 13 May 2020 21:56:26 GMT  
		Size: 20.4 MB (20370044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2377cccc819b93b6367c694d4531f6d0f256636a62effd3f8592bd961c6c21fa`  
		Last Modified: Thu, 14 May 2020 02:15:09 GMT  
		Size: 244.4 KB (244352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb8d9c0ce16dd2186df4ffb514e93303927dd9ad10d5cf79fba2a002b028038`  
		Last Modified: Thu, 14 May 2020 02:15:18 GMT  
		Size: 29.4 MB (29438964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0.161-slim` - linux; 386

```console
$ docker pull mono@sha256:ca713191841be2d2466e3de2935b029654098d4665f1971b5f798d9c90399db6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.1 MB (90133634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0721b64bc41ed06778c68a6d8cf96fb6aa638ca8230fc321beccb3262a401c22`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:42:40 GMT
ADD file:39f8a4c4274f123e2c0a2ef48ac1a111bcc59fda68f3946ab5d644f480fab499 in / 
# Wed, 13 May 2020 21:42:41 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:35:12 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 14 May 2020 00:35:31 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:36:22 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1fa825514fac4b3d9226a943b4954a2efb197db27c0c1c5019bf4a5f7529746e`  
		Last Modified: Wed, 13 May 2020 21:50:17 GMT  
		Size: 23.1 MB (23141460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43163d1e26ca7bae351b647978e6e525a5f6d5979bd3fdf9ec4cc8c55f85d3a8`  
		Last Modified: Thu, 14 May 2020 00:47:14 GMT  
		Size: 244.5 KB (244483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb7945cfea3f1977c9997db158a1e3e46a16bb70d2580c4591d401940b1786e`  
		Last Modified: Thu, 14 May 2020 00:47:32 GMT  
		Size: 66.7 MB (66747691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0.161-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:157b8a5afb302460dbc1638960a65143b725a26452b335da2e22ab7daceb9970
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48857561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52b53ad1ac1fc995b389ae4afa95de28f2255f8dc4ce8b038035f48a5af1da63`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:42:09 GMT
ADD file:341dbc564992a44e81b3a4f399f7de14d7340a45b73c577edb78e16da2c14584 in / 
# Wed, 13 May 2020 22:42:12 GMT
CMD ["bash"]
# Thu, 14 May 2020 01:47:21 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 14 May 2020 01:48:31 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 01:49:49 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3b6ae894780534c0f99588e9cce4beb8fb7884b4578e6206b72f2db75116bb1c`  
		Last Modified: Wed, 13 May 2020 23:02:51 GMT  
		Size: 22.8 MB (22785361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f954c6ba09f38f1b2c8c4a6b3d1d478763bccd68a9038c72437436ac2092cad`  
		Last Modified: Thu, 14 May 2020 02:11:22 GMT  
		Size: 244.6 KB (244550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8516e67eac3bdcee3a32e15d6d71edfb984e8c59ad0c98f7a6c7b015218f85da`  
		Last Modified: Thu, 14 May 2020 02:11:43 GMT  
		Size: 25.8 MB (25827650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.6.0-slim`

```console
$ docker pull mono@sha256:9fb10f64ea980e0c3a7d27488c75e4c91bff8660fc519dc5887311bd10b17c9a
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
$ docker pull mono@sha256:e03c444502022dd73573d892596a6bb4cab789a4f66a61e9ee6dffd8ff9ef1c5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.7 MB (85729530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fa672f39c92e71df557f447a2ab1ebfcf309747e3f6f883f2ccf571ac14d999`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:23:03 GMT
ADD file:08ea1ff3fcd4efc24ab4f262cfa24e55e65844f6858e41a46fe0635d247f174d in / 
# Thu, 23 Apr 2020 00:23:03 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:49:10 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 23 Apr 2020 01:49:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Apr 2020 01:49:54 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b248fa9f6d2ae427ad7f00de3537ab256ae7eb413565f8be0773ee9b86ef57d4`  
		Last Modified: Thu, 23 Apr 2020 00:27:46 GMT  
		Size: 22.5 MB (22513488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485f7d13fbf11ea37b0afce7d19a2618fdef52ce09eeed3be5d6c2cba3ff89bc`  
		Last Modified: Thu, 23 Apr 2020 02:19:31 GMT  
		Size: 244.5 KB (244478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a4778f199830e07df7630da3469e683d4db678333a3b3d661eaadaf4866f90`  
		Last Modified: Thu, 23 Apr 2020 02:19:48 GMT  
		Size: 63.0 MB (62971564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:41d695b38491b1206c44e7add06393bac07434a32edd1e3f8edc4d855878fc16
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46856616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc846d0fc08a43fbf49f1b11aeddcf98fbb07227a218782a032113b042488f01`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 22:42:50 GMT
ADD file:4d807a3f2b10f72f31b43691d51a75c26c3898b53e775bfc4bc3d08720448371 in / 
# Thu, 14 May 2020 22:42:52 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:09:05 GMT
ENV MONO_VERSION=6.6.0.161
# Fri, 15 May 2020 04:09:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 04:10:18 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8c1954048f7e4cb30320daf180f1197d278a905c20d04ff10b32f11b35b7757c`  
		Last Modified: Thu, 14 May 2020 22:50:57 GMT  
		Size: 21.2 MB (21197082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e964c01e015bfb89fdb3e72b98f7ff67658939e38fb7ece25a29bcbb3082fe30`  
		Last Modified: Fri, 15 May 2020 04:22:13 GMT  
		Size: 244.5 KB (244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2e95a1ec1e22ad6830069d161ad74d7ea8b905748f4762cb117bbd0a207e47`  
		Last Modified: Fri, 15 May 2020 04:22:23 GMT  
		Size: 25.4 MB (25415001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:15ed5f9bc060975b061446059a1dc1ca7e6605c5baaed855eb1c66328d765095
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44191570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51da61aca945ec4b12db96ecb19125c0c35f45c1a6200d14eef21a5e2a59c159`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:19:24 GMT
ADD file:aac27626ed8520bcfd1f03f5b7aa780a4e94978b86afcc507994a8c240953561 in / 
# Wed, 13 May 2020 21:19:26 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:27:48 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 14 May 2020 00:28:08 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:29:00 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:307a7e70a6dd41fc81298d6cb2641ebfa8e7bc00b0b27f30f6559f9976a46f1e`  
		Last Modified: Wed, 13 May 2020 21:28:39 GMT  
		Size: 19.3 MB (19298476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9121d426ba6b2669d1e4a4ee3c9060b0cfc6fded57610512fc7818bd31efc9`  
		Last Modified: Thu, 14 May 2020 00:43:03 GMT  
		Size: 244.5 KB (244535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61917c719f7757620481cf5c7275ab522044d462e7fffb609c8144d02290709b`  
		Last Modified: Thu, 14 May 2020 00:43:12 GMT  
		Size: 24.6 MB (24648559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:f5c151197464621e2d06dc4abced8ee231ca8112395954e58566df29ecaa08a5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50053360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d165094a4d3c18123e7b99966e3136748b491a25be3452b0f7479cd8a705bd59`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:48:17 GMT
ADD file:53d95477395267e3c1059f1101e29a7d4b0fcb2bb52351542f4ac065ccb0b973 in / 
# Wed, 13 May 2020 21:48:19 GMT
CMD ["bash"]
# Thu, 14 May 2020 02:01:58 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 14 May 2020 02:02:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 02:03:19 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1d8af20f9b50479a890734605435a9de85d69f19b65d29c9c92f43eea2463979`  
		Last Modified: Wed, 13 May 2020 21:56:26 GMT  
		Size: 20.4 MB (20370044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2377cccc819b93b6367c694d4531f6d0f256636a62effd3f8592bd961c6c21fa`  
		Last Modified: Thu, 14 May 2020 02:15:09 GMT  
		Size: 244.4 KB (244352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb8d9c0ce16dd2186df4ffb514e93303927dd9ad10d5cf79fba2a002b028038`  
		Last Modified: Thu, 14 May 2020 02:15:18 GMT  
		Size: 29.4 MB (29438964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0-slim` - linux; 386

```console
$ docker pull mono@sha256:ca713191841be2d2466e3de2935b029654098d4665f1971b5f798d9c90399db6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.1 MB (90133634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0721b64bc41ed06778c68a6d8cf96fb6aa638ca8230fc321beccb3262a401c22`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:42:40 GMT
ADD file:39f8a4c4274f123e2c0a2ef48ac1a111bcc59fda68f3946ab5d644f480fab499 in / 
# Wed, 13 May 2020 21:42:41 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:35:12 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 14 May 2020 00:35:31 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:36:22 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1fa825514fac4b3d9226a943b4954a2efb197db27c0c1c5019bf4a5f7529746e`  
		Last Modified: Wed, 13 May 2020 21:50:17 GMT  
		Size: 23.1 MB (23141460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43163d1e26ca7bae351b647978e6e525a5f6d5979bd3fdf9ec4cc8c55f85d3a8`  
		Last Modified: Thu, 14 May 2020 00:47:14 GMT  
		Size: 244.5 KB (244483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb7945cfea3f1977c9997db158a1e3e46a16bb70d2580c4591d401940b1786e`  
		Last Modified: Thu, 14 May 2020 00:47:32 GMT  
		Size: 66.7 MB (66747691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:157b8a5afb302460dbc1638960a65143b725a26452b335da2e22ab7daceb9970
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48857561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52b53ad1ac1fc995b389ae4afa95de28f2255f8dc4ce8b038035f48a5af1da63`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:42:09 GMT
ADD file:341dbc564992a44e81b3a4f399f7de14d7340a45b73c577edb78e16da2c14584 in / 
# Wed, 13 May 2020 22:42:12 GMT
CMD ["bash"]
# Thu, 14 May 2020 01:47:21 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 14 May 2020 01:48:31 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 01:49:49 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3b6ae894780534c0f99588e9cce4beb8fb7884b4578e6206b72f2db75116bb1c`  
		Last Modified: Wed, 13 May 2020 23:02:51 GMT  
		Size: 22.8 MB (22785361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f954c6ba09f38f1b2c8c4a6b3d1d478763bccd68a9038c72437436ac2092cad`  
		Last Modified: Thu, 14 May 2020 02:11:22 GMT  
		Size: 244.6 KB (244550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8516e67eac3bdcee3a32e15d6d71edfb984e8c59ad0c98f7a6c7b015218f85da`  
		Last Modified: Thu, 14 May 2020 02:11:43 GMT  
		Size: 25.8 MB (25827650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.6-slim`

```console
$ docker pull mono@sha256:9fb10f64ea980e0c3a7d27488c75e4c91bff8660fc519dc5887311bd10b17c9a
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
$ docker pull mono@sha256:e03c444502022dd73573d892596a6bb4cab789a4f66a61e9ee6dffd8ff9ef1c5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.7 MB (85729530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fa672f39c92e71df557f447a2ab1ebfcf309747e3f6f883f2ccf571ac14d999`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:23:03 GMT
ADD file:08ea1ff3fcd4efc24ab4f262cfa24e55e65844f6858e41a46fe0635d247f174d in / 
# Thu, 23 Apr 2020 00:23:03 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:49:10 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 23 Apr 2020 01:49:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Apr 2020 01:49:54 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b248fa9f6d2ae427ad7f00de3537ab256ae7eb413565f8be0773ee9b86ef57d4`  
		Last Modified: Thu, 23 Apr 2020 00:27:46 GMT  
		Size: 22.5 MB (22513488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485f7d13fbf11ea37b0afce7d19a2618fdef52ce09eeed3be5d6c2cba3ff89bc`  
		Last Modified: Thu, 23 Apr 2020 02:19:31 GMT  
		Size: 244.5 KB (244478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a4778f199830e07df7630da3469e683d4db678333a3b3d661eaadaf4866f90`  
		Last Modified: Thu, 23 Apr 2020 02:19:48 GMT  
		Size: 63.0 MB (62971564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:41d695b38491b1206c44e7add06393bac07434a32edd1e3f8edc4d855878fc16
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46856616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc846d0fc08a43fbf49f1b11aeddcf98fbb07227a218782a032113b042488f01`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 22:42:50 GMT
ADD file:4d807a3f2b10f72f31b43691d51a75c26c3898b53e775bfc4bc3d08720448371 in / 
# Thu, 14 May 2020 22:42:52 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:09:05 GMT
ENV MONO_VERSION=6.6.0.161
# Fri, 15 May 2020 04:09:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 04:10:18 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8c1954048f7e4cb30320daf180f1197d278a905c20d04ff10b32f11b35b7757c`  
		Last Modified: Thu, 14 May 2020 22:50:57 GMT  
		Size: 21.2 MB (21197082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e964c01e015bfb89fdb3e72b98f7ff67658939e38fb7ece25a29bcbb3082fe30`  
		Last Modified: Fri, 15 May 2020 04:22:13 GMT  
		Size: 244.5 KB (244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2e95a1ec1e22ad6830069d161ad74d7ea8b905748f4762cb117bbd0a207e47`  
		Last Modified: Fri, 15 May 2020 04:22:23 GMT  
		Size: 25.4 MB (25415001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:15ed5f9bc060975b061446059a1dc1ca7e6605c5baaed855eb1c66328d765095
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44191570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51da61aca945ec4b12db96ecb19125c0c35f45c1a6200d14eef21a5e2a59c159`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:19:24 GMT
ADD file:aac27626ed8520bcfd1f03f5b7aa780a4e94978b86afcc507994a8c240953561 in / 
# Wed, 13 May 2020 21:19:26 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:27:48 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 14 May 2020 00:28:08 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:29:00 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:307a7e70a6dd41fc81298d6cb2641ebfa8e7bc00b0b27f30f6559f9976a46f1e`  
		Last Modified: Wed, 13 May 2020 21:28:39 GMT  
		Size: 19.3 MB (19298476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9121d426ba6b2669d1e4a4ee3c9060b0cfc6fded57610512fc7818bd31efc9`  
		Last Modified: Thu, 14 May 2020 00:43:03 GMT  
		Size: 244.5 KB (244535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61917c719f7757620481cf5c7275ab522044d462e7fffb609c8144d02290709b`  
		Last Modified: Thu, 14 May 2020 00:43:12 GMT  
		Size: 24.6 MB (24648559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:f5c151197464621e2d06dc4abced8ee231ca8112395954e58566df29ecaa08a5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50053360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d165094a4d3c18123e7b99966e3136748b491a25be3452b0f7479cd8a705bd59`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:48:17 GMT
ADD file:53d95477395267e3c1059f1101e29a7d4b0fcb2bb52351542f4ac065ccb0b973 in / 
# Wed, 13 May 2020 21:48:19 GMT
CMD ["bash"]
# Thu, 14 May 2020 02:01:58 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 14 May 2020 02:02:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 02:03:19 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1d8af20f9b50479a890734605435a9de85d69f19b65d29c9c92f43eea2463979`  
		Last Modified: Wed, 13 May 2020 21:56:26 GMT  
		Size: 20.4 MB (20370044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2377cccc819b93b6367c694d4531f6d0f256636a62effd3f8592bd961c6c21fa`  
		Last Modified: Thu, 14 May 2020 02:15:09 GMT  
		Size: 244.4 KB (244352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb8d9c0ce16dd2186df4ffb514e93303927dd9ad10d5cf79fba2a002b028038`  
		Last Modified: Thu, 14 May 2020 02:15:18 GMT  
		Size: 29.4 MB (29438964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6-slim` - linux; 386

```console
$ docker pull mono@sha256:ca713191841be2d2466e3de2935b029654098d4665f1971b5f798d9c90399db6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.1 MB (90133634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0721b64bc41ed06778c68a6d8cf96fb6aa638ca8230fc321beccb3262a401c22`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:42:40 GMT
ADD file:39f8a4c4274f123e2c0a2ef48ac1a111bcc59fda68f3946ab5d644f480fab499 in / 
# Wed, 13 May 2020 21:42:41 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:35:12 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 14 May 2020 00:35:31 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:36:22 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1fa825514fac4b3d9226a943b4954a2efb197db27c0c1c5019bf4a5f7529746e`  
		Last Modified: Wed, 13 May 2020 21:50:17 GMT  
		Size: 23.1 MB (23141460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43163d1e26ca7bae351b647978e6e525a5f6d5979bd3fdf9ec4cc8c55f85d3a8`  
		Last Modified: Thu, 14 May 2020 00:47:14 GMT  
		Size: 244.5 KB (244483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb7945cfea3f1977c9997db158a1e3e46a16bb70d2580c4591d401940b1786e`  
		Last Modified: Thu, 14 May 2020 00:47:32 GMT  
		Size: 66.7 MB (66747691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:157b8a5afb302460dbc1638960a65143b725a26452b335da2e22ab7daceb9970
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48857561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52b53ad1ac1fc995b389ae4afa95de28f2255f8dc4ce8b038035f48a5af1da63`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:42:09 GMT
ADD file:341dbc564992a44e81b3a4f399f7de14d7340a45b73c577edb78e16da2c14584 in / 
# Wed, 13 May 2020 22:42:12 GMT
CMD ["bash"]
# Thu, 14 May 2020 01:47:21 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 14 May 2020 01:48:31 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 01:49:49 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3b6ae894780534c0f99588e9cce4beb8fb7884b4578e6206b72f2db75116bb1c`  
		Last Modified: Wed, 13 May 2020 23:02:51 GMT  
		Size: 22.8 MB (22785361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f954c6ba09f38f1b2c8c4a6b3d1d478763bccd68a9038c72437436ac2092cad`  
		Last Modified: Thu, 14 May 2020 02:11:22 GMT  
		Size: 244.6 KB (244550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8516e67eac3bdcee3a32e15d6d71edfb984e8c59ad0c98f7a6c7b015218f85da`  
		Last Modified: Thu, 14 May 2020 02:11:43 GMT  
		Size: 25.8 MB (25827650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.8`

```console
$ docker pull mono@sha256:77e66aca06ed4914a850ce5a590698acdc7c2f71a197b4428a0a6fe145bb0027
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.8` - linux; amd64

```console
$ docker pull mono@sha256:2351a2ba6c2228ecac8696680f65e49607432bb7fd6c0494fd254060c48f6a02
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.1 MB (235136555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59599093bfc20b4291b6019e7cd8bd648dab8dc3c341bc26001f807264ac44dc`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:23:03 GMT
ADD file:08ea1ff3fcd4efc24ab4f262cfa24e55e65844f6858e41a46fe0635d247f174d in / 
# Thu, 23 Apr 2020 00:23:03 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:48:15 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 23 Apr 2020 01:48:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Apr 2020 01:48:58 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 23 Apr 2020 01:59:28 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b248fa9f6d2ae427ad7f00de3537ab256ae7eb413565f8be0773ee9b86ef57d4`  
		Last Modified: Thu, 23 Apr 2020 00:27:46 GMT  
		Size: 22.5 MB (22513488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5f98f65ba396764fe9568783d5a5c15abaed85471ba915f7533777d9ee788d`  
		Last Modified: Thu, 23 Apr 2020 02:19:07 GMT  
		Size: 244.5 KB (244473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06df397516278d03ee36a7c24249bc8b0b57b23701952818c89538b9856c1ffb`  
		Last Modified: Thu, 23 Apr 2020 02:19:25 GMT  
		Size: 64.6 MB (64584374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e83f8e35ba5681f2772165e09a403fab75e2cb54d9c6166e85301ad905d258`  
		Last Modified: Thu, 23 Apr 2020 02:20:55 GMT  
		Size: 147.8 MB (147794220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8` - linux; arm variant v5

```console
$ docker pull mono@sha256:5be1950fc69cdd2737286151d13e08b8a810ce402c4e961abec76247ef5d87f5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.7 MB (176701525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7285a10f55436a04b15962a4fe25b96046a348c1a02a15aa64d07e2369f2ed5`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 22:42:50 GMT
ADD file:4d807a3f2b10f72f31b43691d51a75c26c3898b53e775bfc4bc3d08720448371 in / 
# Thu, 14 May 2020 22:42:52 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:07:32 GMT
ENV MONO_VERSION=6.8.0.96
# Fri, 15 May 2020 04:07:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 04:08:51 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 15 May 2020 04:14:47 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8c1954048f7e4cb30320daf180f1197d278a905c20d04ff10b32f11b35b7757c`  
		Last Modified: Thu, 14 May 2020 22:50:57 GMT  
		Size: 21.2 MB (21197082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7009fb73261c04c568d9dd5c1b839a02f5d97fea7f8c21705c8091eb1b6b5b6d`  
		Last Modified: Fri, 15 May 2020 04:21:54 GMT  
		Size: 244.5 KB (244519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b237016212e8e87ef0d32354521bfb76ce82ce991d8c6cc90ee0dcd82cc0392e`  
		Last Modified: Fri, 15 May 2020 04:22:04 GMT  
		Size: 25.4 MB (25368245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f7186fdafac062d1af6c86d4fca2df0b62f320aec72fcbbd7b8cb4d6fcf467`  
		Last Modified: Fri, 15 May 2020 04:23:35 GMT  
		Size: 129.9 MB (129891679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8` - linux; arm variant v7

```console
$ docker pull mono@sha256:55ef6d96d85e1d0e3aca832b8c2a7a0b7da50bffa2dacf77542fbd7aff27a559
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.7 MB (172707764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc9acd8a77a391a80d27014968c3dfe08186f34930cc569f44c35d2a7a09b22c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:19:24 GMT
ADD file:aac27626ed8520bcfd1f03f5b7aa780a4e94978b86afcc507994a8c240953561 in / 
# Wed, 13 May 2020 21:19:26 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:26:29 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 14 May 2020 00:26:48 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:27:40 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 00:33:55 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:307a7e70a6dd41fc81298d6cb2641ebfa8e7bc00b0b27f30f6559f9976a46f1e`  
		Last Modified: Wed, 13 May 2020 21:28:39 GMT  
		Size: 19.3 MB (19298476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91631fd0b2baefb452095603fc22b8be62f3657d1ae76086f6318c48f36cae25`  
		Last Modified: Thu, 14 May 2020 00:42:46 GMT  
		Size: 244.5 KB (244516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707e4565b23eaef80b85f8caf65db746d521af83f33888a710630ea91c60de18`  
		Last Modified: Thu, 14 May 2020 00:42:55 GMT  
		Size: 24.6 MB (24608714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a42be730e2ad23f35deb8b93a0913d13edb02be20a73fa837770d36acbbf74`  
		Last Modified: Thu, 14 May 2020 00:44:20 GMT  
		Size: 128.6 MB (128556058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:cbc1409b11ea1fd492744b6396ef5a9afa4bd427de25d89ea8406fbd9189d0a7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.7 MB (194747627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:939138ef9b9d3ec1af2baae95869f7cf8c66020511a3bb70138be5e5dd8450f2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:48:17 GMT
ADD file:53d95477395267e3c1059f1101e29a7d4b0fcb2bb52351542f4ac065ccb0b973 in / 
# Wed, 13 May 2020 21:48:19 GMT
CMD ["bash"]
# Thu, 14 May 2020 02:00:25 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 14 May 2020 02:00:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 02:01:47 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 02:07:30 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1d8af20f9b50479a890734605435a9de85d69f19b65d29c9c92f43eea2463979`  
		Last Modified: Wed, 13 May 2020 21:56:26 GMT  
		Size: 20.4 MB (20370044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5f88aa673180f3a9e54d2d3fc9c67565c9545d3072c1a42eee0eda3192c039`  
		Last Modified: Thu, 14 May 2020 02:14:51 GMT  
		Size: 244.4 KB (244366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5622468da1cdc4403ec0072a3093de5483f907e82f7e7493e9bcf66765d2367`  
		Last Modified: Thu, 14 May 2020 02:14:59 GMT  
		Size: 29.4 MB (29419827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a79b7e06bf892f3f0e1c21e1bdc62517abc6fd4fd31a2f0be27e369398f2d0ca`  
		Last Modified: Thu, 14 May 2020 02:16:28 GMT  
		Size: 144.7 MB (144713390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8` - linux; 386

```console
$ docker pull mono@sha256:91becebb427753ead531605be391b0528b1b8176f46762f3fb896b58fbf493f5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.5 MB (243509833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d912f07467de168fbaadffea2b2be97d24f40de4675c1ef98b3b7c70f274b9c5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:42:40 GMT
ADD file:39f8a4c4274f123e2c0a2ef48ac1a111bcc59fda68f3946ab5d644f480fab499 in / 
# Wed, 13 May 2020 21:42:41 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:33:55 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 14 May 2020 00:34:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:34:57 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 00:40:29 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1fa825514fac4b3d9226a943b4954a2efb197db27c0c1c5019bf4a5f7529746e`  
		Last Modified: Wed, 13 May 2020 21:50:17 GMT  
		Size: 23.1 MB (23141460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eac1a2c3c2e8b2376318177cabaab6efa4884e4a1262be8019864dd8d79b02d`  
		Last Modified: Thu, 14 May 2020 00:46:50 GMT  
		Size: 244.5 KB (244476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0517e1b7f3b81bc5e21be055d429fe5465bebb94609a0824c5064f1c2198ea92`  
		Last Modified: Thu, 14 May 2020 00:47:08 GMT  
		Size: 68.6 MB (68630757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b33be2fe9551abfc1002c4bad0c8ce971f275c3ca146936540551c5776b4fd4`  
		Last Modified: Thu, 14 May 2020 00:49:07 GMT  
		Size: 151.5 MB (151493140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8` - linux; ppc64le

```console
$ docker pull mono@sha256:28211181008fc8a25dbc12b5f75fd4857e92af22ee4716fd13064027ba80c113
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.0 MB (178995744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcbdcf050885aeb282b85d9942bee597145d594577643da02a09cb638cd2edb9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:42:09 GMT
ADD file:341dbc564992a44e81b3a4f399f7de14d7340a45b73c577edb78e16da2c14584 in / 
# Wed, 13 May 2020 22:42:12 GMT
CMD ["bash"]
# Thu, 14 May 2020 01:44:38 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 14 May 2020 01:45:44 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 01:47:00 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 01:57:53 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3b6ae894780534c0f99588e9cce4beb8fb7884b4578e6206b72f2db75116bb1c`  
		Last Modified: Wed, 13 May 2020 23:02:51 GMT  
		Size: 22.8 MB (22785361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0d85174db6ce48c895d3bbf3f847e1cba986fc66e705bd86bb13e3fbf73286`  
		Last Modified: Thu, 14 May 2020 02:10:48 GMT  
		Size: 244.5 KB (244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6124cc55d37923fca85643397621b030dae64f93ddf2c45ed9704bf9e9e5d141`  
		Last Modified: Thu, 14 May 2020 02:11:06 GMT  
		Size: 25.8 MB (25775347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64bc6db4438da29e772ebf533c91b52b035c322c12bf45899c0cbcff8a42ba24`  
		Last Modified: Thu, 14 May 2020 02:13:51 GMT  
		Size: 130.2 MB (130190503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.8.0`

```console
$ docker pull mono@sha256:77e66aca06ed4914a850ce5a590698acdc7c2f71a197b4428a0a6fe145bb0027
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.8.0` - linux; amd64

```console
$ docker pull mono@sha256:2351a2ba6c2228ecac8696680f65e49607432bb7fd6c0494fd254060c48f6a02
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.1 MB (235136555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59599093bfc20b4291b6019e7cd8bd648dab8dc3c341bc26001f807264ac44dc`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:23:03 GMT
ADD file:08ea1ff3fcd4efc24ab4f262cfa24e55e65844f6858e41a46fe0635d247f174d in / 
# Thu, 23 Apr 2020 00:23:03 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:48:15 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 23 Apr 2020 01:48:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Apr 2020 01:48:58 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 23 Apr 2020 01:59:28 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b248fa9f6d2ae427ad7f00de3537ab256ae7eb413565f8be0773ee9b86ef57d4`  
		Last Modified: Thu, 23 Apr 2020 00:27:46 GMT  
		Size: 22.5 MB (22513488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5f98f65ba396764fe9568783d5a5c15abaed85471ba915f7533777d9ee788d`  
		Last Modified: Thu, 23 Apr 2020 02:19:07 GMT  
		Size: 244.5 KB (244473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06df397516278d03ee36a7c24249bc8b0b57b23701952818c89538b9856c1ffb`  
		Last Modified: Thu, 23 Apr 2020 02:19:25 GMT  
		Size: 64.6 MB (64584374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e83f8e35ba5681f2772165e09a403fab75e2cb54d9c6166e85301ad905d258`  
		Last Modified: Thu, 23 Apr 2020 02:20:55 GMT  
		Size: 147.8 MB (147794220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0` - linux; arm variant v5

```console
$ docker pull mono@sha256:5be1950fc69cdd2737286151d13e08b8a810ce402c4e961abec76247ef5d87f5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.7 MB (176701525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7285a10f55436a04b15962a4fe25b96046a348c1a02a15aa64d07e2369f2ed5`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 22:42:50 GMT
ADD file:4d807a3f2b10f72f31b43691d51a75c26c3898b53e775bfc4bc3d08720448371 in / 
# Thu, 14 May 2020 22:42:52 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:07:32 GMT
ENV MONO_VERSION=6.8.0.96
# Fri, 15 May 2020 04:07:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 04:08:51 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 15 May 2020 04:14:47 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8c1954048f7e4cb30320daf180f1197d278a905c20d04ff10b32f11b35b7757c`  
		Last Modified: Thu, 14 May 2020 22:50:57 GMT  
		Size: 21.2 MB (21197082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7009fb73261c04c568d9dd5c1b839a02f5d97fea7f8c21705c8091eb1b6b5b6d`  
		Last Modified: Fri, 15 May 2020 04:21:54 GMT  
		Size: 244.5 KB (244519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b237016212e8e87ef0d32354521bfb76ce82ce991d8c6cc90ee0dcd82cc0392e`  
		Last Modified: Fri, 15 May 2020 04:22:04 GMT  
		Size: 25.4 MB (25368245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f7186fdafac062d1af6c86d4fca2df0b62f320aec72fcbbd7b8cb4d6fcf467`  
		Last Modified: Fri, 15 May 2020 04:23:35 GMT  
		Size: 129.9 MB (129891679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0` - linux; arm variant v7

```console
$ docker pull mono@sha256:55ef6d96d85e1d0e3aca832b8c2a7a0b7da50bffa2dacf77542fbd7aff27a559
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.7 MB (172707764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc9acd8a77a391a80d27014968c3dfe08186f34930cc569f44c35d2a7a09b22c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:19:24 GMT
ADD file:aac27626ed8520bcfd1f03f5b7aa780a4e94978b86afcc507994a8c240953561 in / 
# Wed, 13 May 2020 21:19:26 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:26:29 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 14 May 2020 00:26:48 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:27:40 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 00:33:55 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:307a7e70a6dd41fc81298d6cb2641ebfa8e7bc00b0b27f30f6559f9976a46f1e`  
		Last Modified: Wed, 13 May 2020 21:28:39 GMT  
		Size: 19.3 MB (19298476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91631fd0b2baefb452095603fc22b8be62f3657d1ae76086f6318c48f36cae25`  
		Last Modified: Thu, 14 May 2020 00:42:46 GMT  
		Size: 244.5 KB (244516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707e4565b23eaef80b85f8caf65db746d521af83f33888a710630ea91c60de18`  
		Last Modified: Thu, 14 May 2020 00:42:55 GMT  
		Size: 24.6 MB (24608714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a42be730e2ad23f35deb8b93a0913d13edb02be20a73fa837770d36acbbf74`  
		Last Modified: Thu, 14 May 2020 00:44:20 GMT  
		Size: 128.6 MB (128556058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:cbc1409b11ea1fd492744b6396ef5a9afa4bd427de25d89ea8406fbd9189d0a7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.7 MB (194747627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:939138ef9b9d3ec1af2baae95869f7cf8c66020511a3bb70138be5e5dd8450f2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:48:17 GMT
ADD file:53d95477395267e3c1059f1101e29a7d4b0fcb2bb52351542f4ac065ccb0b973 in / 
# Wed, 13 May 2020 21:48:19 GMT
CMD ["bash"]
# Thu, 14 May 2020 02:00:25 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 14 May 2020 02:00:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 02:01:47 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 02:07:30 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1d8af20f9b50479a890734605435a9de85d69f19b65d29c9c92f43eea2463979`  
		Last Modified: Wed, 13 May 2020 21:56:26 GMT  
		Size: 20.4 MB (20370044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5f88aa673180f3a9e54d2d3fc9c67565c9545d3072c1a42eee0eda3192c039`  
		Last Modified: Thu, 14 May 2020 02:14:51 GMT  
		Size: 244.4 KB (244366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5622468da1cdc4403ec0072a3093de5483f907e82f7e7493e9bcf66765d2367`  
		Last Modified: Thu, 14 May 2020 02:14:59 GMT  
		Size: 29.4 MB (29419827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a79b7e06bf892f3f0e1c21e1bdc62517abc6fd4fd31a2f0be27e369398f2d0ca`  
		Last Modified: Thu, 14 May 2020 02:16:28 GMT  
		Size: 144.7 MB (144713390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0` - linux; 386

```console
$ docker pull mono@sha256:91becebb427753ead531605be391b0528b1b8176f46762f3fb896b58fbf493f5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.5 MB (243509833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d912f07467de168fbaadffea2b2be97d24f40de4675c1ef98b3b7c70f274b9c5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:42:40 GMT
ADD file:39f8a4c4274f123e2c0a2ef48ac1a111bcc59fda68f3946ab5d644f480fab499 in / 
# Wed, 13 May 2020 21:42:41 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:33:55 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 14 May 2020 00:34:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:34:57 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 00:40:29 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1fa825514fac4b3d9226a943b4954a2efb197db27c0c1c5019bf4a5f7529746e`  
		Last Modified: Wed, 13 May 2020 21:50:17 GMT  
		Size: 23.1 MB (23141460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eac1a2c3c2e8b2376318177cabaab6efa4884e4a1262be8019864dd8d79b02d`  
		Last Modified: Thu, 14 May 2020 00:46:50 GMT  
		Size: 244.5 KB (244476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0517e1b7f3b81bc5e21be055d429fe5465bebb94609a0824c5064f1c2198ea92`  
		Last Modified: Thu, 14 May 2020 00:47:08 GMT  
		Size: 68.6 MB (68630757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b33be2fe9551abfc1002c4bad0c8ce971f275c3ca146936540551c5776b4fd4`  
		Last Modified: Thu, 14 May 2020 00:49:07 GMT  
		Size: 151.5 MB (151493140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0` - linux; ppc64le

```console
$ docker pull mono@sha256:28211181008fc8a25dbc12b5f75fd4857e92af22ee4716fd13064027ba80c113
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.0 MB (178995744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcbdcf050885aeb282b85d9942bee597145d594577643da02a09cb638cd2edb9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:42:09 GMT
ADD file:341dbc564992a44e81b3a4f399f7de14d7340a45b73c577edb78e16da2c14584 in / 
# Wed, 13 May 2020 22:42:12 GMT
CMD ["bash"]
# Thu, 14 May 2020 01:44:38 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 14 May 2020 01:45:44 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 01:47:00 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 01:57:53 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3b6ae894780534c0f99588e9cce4beb8fb7884b4578e6206b72f2db75116bb1c`  
		Last Modified: Wed, 13 May 2020 23:02:51 GMT  
		Size: 22.8 MB (22785361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0d85174db6ce48c895d3bbf3f847e1cba986fc66e705bd86bb13e3fbf73286`  
		Last Modified: Thu, 14 May 2020 02:10:48 GMT  
		Size: 244.5 KB (244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6124cc55d37923fca85643397621b030dae64f93ddf2c45ed9704bf9e9e5d141`  
		Last Modified: Thu, 14 May 2020 02:11:06 GMT  
		Size: 25.8 MB (25775347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64bc6db4438da29e772ebf533c91b52b035c322c12bf45899c0cbcff8a42ba24`  
		Last Modified: Thu, 14 May 2020 02:13:51 GMT  
		Size: 130.2 MB (130190503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.8.0.96`

```console
$ docker pull mono@sha256:77e66aca06ed4914a850ce5a590698acdc7c2f71a197b4428a0a6fe145bb0027
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.8.0.96` - linux; amd64

```console
$ docker pull mono@sha256:2351a2ba6c2228ecac8696680f65e49607432bb7fd6c0494fd254060c48f6a02
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.1 MB (235136555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59599093bfc20b4291b6019e7cd8bd648dab8dc3c341bc26001f807264ac44dc`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:23:03 GMT
ADD file:08ea1ff3fcd4efc24ab4f262cfa24e55e65844f6858e41a46fe0635d247f174d in / 
# Thu, 23 Apr 2020 00:23:03 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:48:15 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 23 Apr 2020 01:48:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Apr 2020 01:48:58 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 23 Apr 2020 01:59:28 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b248fa9f6d2ae427ad7f00de3537ab256ae7eb413565f8be0773ee9b86ef57d4`  
		Last Modified: Thu, 23 Apr 2020 00:27:46 GMT  
		Size: 22.5 MB (22513488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5f98f65ba396764fe9568783d5a5c15abaed85471ba915f7533777d9ee788d`  
		Last Modified: Thu, 23 Apr 2020 02:19:07 GMT  
		Size: 244.5 KB (244473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06df397516278d03ee36a7c24249bc8b0b57b23701952818c89538b9856c1ffb`  
		Last Modified: Thu, 23 Apr 2020 02:19:25 GMT  
		Size: 64.6 MB (64584374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e83f8e35ba5681f2772165e09a403fab75e2cb54d9c6166e85301ad905d258`  
		Last Modified: Thu, 23 Apr 2020 02:20:55 GMT  
		Size: 147.8 MB (147794220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.96` - linux; arm variant v5

```console
$ docker pull mono@sha256:5be1950fc69cdd2737286151d13e08b8a810ce402c4e961abec76247ef5d87f5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.7 MB (176701525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7285a10f55436a04b15962a4fe25b96046a348c1a02a15aa64d07e2369f2ed5`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 22:42:50 GMT
ADD file:4d807a3f2b10f72f31b43691d51a75c26c3898b53e775bfc4bc3d08720448371 in / 
# Thu, 14 May 2020 22:42:52 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:07:32 GMT
ENV MONO_VERSION=6.8.0.96
# Fri, 15 May 2020 04:07:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 04:08:51 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 15 May 2020 04:14:47 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8c1954048f7e4cb30320daf180f1197d278a905c20d04ff10b32f11b35b7757c`  
		Last Modified: Thu, 14 May 2020 22:50:57 GMT  
		Size: 21.2 MB (21197082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7009fb73261c04c568d9dd5c1b839a02f5d97fea7f8c21705c8091eb1b6b5b6d`  
		Last Modified: Fri, 15 May 2020 04:21:54 GMT  
		Size: 244.5 KB (244519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b237016212e8e87ef0d32354521bfb76ce82ce991d8c6cc90ee0dcd82cc0392e`  
		Last Modified: Fri, 15 May 2020 04:22:04 GMT  
		Size: 25.4 MB (25368245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f7186fdafac062d1af6c86d4fca2df0b62f320aec72fcbbd7b8cb4d6fcf467`  
		Last Modified: Fri, 15 May 2020 04:23:35 GMT  
		Size: 129.9 MB (129891679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.96` - linux; arm variant v7

```console
$ docker pull mono@sha256:55ef6d96d85e1d0e3aca832b8c2a7a0b7da50bffa2dacf77542fbd7aff27a559
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.7 MB (172707764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc9acd8a77a391a80d27014968c3dfe08186f34930cc569f44c35d2a7a09b22c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:19:24 GMT
ADD file:aac27626ed8520bcfd1f03f5b7aa780a4e94978b86afcc507994a8c240953561 in / 
# Wed, 13 May 2020 21:19:26 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:26:29 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 14 May 2020 00:26:48 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:27:40 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 00:33:55 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:307a7e70a6dd41fc81298d6cb2641ebfa8e7bc00b0b27f30f6559f9976a46f1e`  
		Last Modified: Wed, 13 May 2020 21:28:39 GMT  
		Size: 19.3 MB (19298476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91631fd0b2baefb452095603fc22b8be62f3657d1ae76086f6318c48f36cae25`  
		Last Modified: Thu, 14 May 2020 00:42:46 GMT  
		Size: 244.5 KB (244516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707e4565b23eaef80b85f8caf65db746d521af83f33888a710630ea91c60de18`  
		Last Modified: Thu, 14 May 2020 00:42:55 GMT  
		Size: 24.6 MB (24608714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a42be730e2ad23f35deb8b93a0913d13edb02be20a73fa837770d36acbbf74`  
		Last Modified: Thu, 14 May 2020 00:44:20 GMT  
		Size: 128.6 MB (128556058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.96` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:cbc1409b11ea1fd492744b6396ef5a9afa4bd427de25d89ea8406fbd9189d0a7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.7 MB (194747627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:939138ef9b9d3ec1af2baae95869f7cf8c66020511a3bb70138be5e5dd8450f2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:48:17 GMT
ADD file:53d95477395267e3c1059f1101e29a7d4b0fcb2bb52351542f4ac065ccb0b973 in / 
# Wed, 13 May 2020 21:48:19 GMT
CMD ["bash"]
# Thu, 14 May 2020 02:00:25 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 14 May 2020 02:00:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 02:01:47 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 02:07:30 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1d8af20f9b50479a890734605435a9de85d69f19b65d29c9c92f43eea2463979`  
		Last Modified: Wed, 13 May 2020 21:56:26 GMT  
		Size: 20.4 MB (20370044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5f88aa673180f3a9e54d2d3fc9c67565c9545d3072c1a42eee0eda3192c039`  
		Last Modified: Thu, 14 May 2020 02:14:51 GMT  
		Size: 244.4 KB (244366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5622468da1cdc4403ec0072a3093de5483f907e82f7e7493e9bcf66765d2367`  
		Last Modified: Thu, 14 May 2020 02:14:59 GMT  
		Size: 29.4 MB (29419827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a79b7e06bf892f3f0e1c21e1bdc62517abc6fd4fd31a2f0be27e369398f2d0ca`  
		Last Modified: Thu, 14 May 2020 02:16:28 GMT  
		Size: 144.7 MB (144713390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.96` - linux; 386

```console
$ docker pull mono@sha256:91becebb427753ead531605be391b0528b1b8176f46762f3fb896b58fbf493f5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.5 MB (243509833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d912f07467de168fbaadffea2b2be97d24f40de4675c1ef98b3b7c70f274b9c5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:42:40 GMT
ADD file:39f8a4c4274f123e2c0a2ef48ac1a111bcc59fda68f3946ab5d644f480fab499 in / 
# Wed, 13 May 2020 21:42:41 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:33:55 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 14 May 2020 00:34:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:34:57 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 00:40:29 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1fa825514fac4b3d9226a943b4954a2efb197db27c0c1c5019bf4a5f7529746e`  
		Last Modified: Wed, 13 May 2020 21:50:17 GMT  
		Size: 23.1 MB (23141460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eac1a2c3c2e8b2376318177cabaab6efa4884e4a1262be8019864dd8d79b02d`  
		Last Modified: Thu, 14 May 2020 00:46:50 GMT  
		Size: 244.5 KB (244476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0517e1b7f3b81bc5e21be055d429fe5465bebb94609a0824c5064f1c2198ea92`  
		Last Modified: Thu, 14 May 2020 00:47:08 GMT  
		Size: 68.6 MB (68630757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b33be2fe9551abfc1002c4bad0c8ce971f275c3ca146936540551c5776b4fd4`  
		Last Modified: Thu, 14 May 2020 00:49:07 GMT  
		Size: 151.5 MB (151493140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.96` - linux; ppc64le

```console
$ docker pull mono@sha256:28211181008fc8a25dbc12b5f75fd4857e92af22ee4716fd13064027ba80c113
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.0 MB (178995744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcbdcf050885aeb282b85d9942bee597145d594577643da02a09cb638cd2edb9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:42:09 GMT
ADD file:341dbc564992a44e81b3a4f399f7de14d7340a45b73c577edb78e16da2c14584 in / 
# Wed, 13 May 2020 22:42:12 GMT
CMD ["bash"]
# Thu, 14 May 2020 01:44:38 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 14 May 2020 01:45:44 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 01:47:00 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 01:57:53 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3b6ae894780534c0f99588e9cce4beb8fb7884b4578e6206b72f2db75116bb1c`  
		Last Modified: Wed, 13 May 2020 23:02:51 GMT  
		Size: 22.8 MB (22785361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0d85174db6ce48c895d3bbf3f847e1cba986fc66e705bd86bb13e3fbf73286`  
		Last Modified: Thu, 14 May 2020 02:10:48 GMT  
		Size: 244.5 KB (244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6124cc55d37923fca85643397621b030dae64f93ddf2c45ed9704bf9e9e5d141`  
		Last Modified: Thu, 14 May 2020 02:11:06 GMT  
		Size: 25.8 MB (25775347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64bc6db4438da29e772ebf533c91b52b035c322c12bf45899c0cbcff8a42ba24`  
		Last Modified: Thu, 14 May 2020 02:13:51 GMT  
		Size: 130.2 MB (130190503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.8.0.96-slim`

```console
$ docker pull mono@sha256:7db549a1569b8cda022b582142b50bf26fad154f7d1ae0274c9287142bb656bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.8.0.96-slim` - linux; amd64

```console
$ docker pull mono@sha256:dea2a84843d47ee855a58ca9291c5838d5f13a703074e85ce81a2b324675a091
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.3 MB (87342335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b522d57eded02abb2b3358f68714c4c066951809e1257fee584c4f22ad8347f8`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:23:03 GMT
ADD file:08ea1ff3fcd4efc24ab4f262cfa24e55e65844f6858e41a46fe0635d247f174d in / 
# Thu, 23 Apr 2020 00:23:03 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:48:15 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 23 Apr 2020 01:48:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Apr 2020 01:48:58 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b248fa9f6d2ae427ad7f00de3537ab256ae7eb413565f8be0773ee9b86ef57d4`  
		Last Modified: Thu, 23 Apr 2020 00:27:46 GMT  
		Size: 22.5 MB (22513488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5f98f65ba396764fe9568783d5a5c15abaed85471ba915f7533777d9ee788d`  
		Last Modified: Thu, 23 Apr 2020 02:19:07 GMT  
		Size: 244.5 KB (244473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06df397516278d03ee36a7c24249bc8b0b57b23701952818c89538b9856c1ffb`  
		Last Modified: Thu, 23 Apr 2020 02:19:25 GMT  
		Size: 64.6 MB (64584374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.96-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:d9c9e91dff7bbf016ee6a8f1f38041efdcf168a14ce7e2d16153ab428aeb97f6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.8 MB (46809846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b23a07406039b0f5272713478c0818cd62f58444e5e8fd5056ddd9a98f926a5`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 22:42:50 GMT
ADD file:4d807a3f2b10f72f31b43691d51a75c26c3898b53e775bfc4bc3d08720448371 in / 
# Thu, 14 May 2020 22:42:52 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:07:32 GMT
ENV MONO_VERSION=6.8.0.96
# Fri, 15 May 2020 04:07:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 04:08:51 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8c1954048f7e4cb30320daf180f1197d278a905c20d04ff10b32f11b35b7757c`  
		Last Modified: Thu, 14 May 2020 22:50:57 GMT  
		Size: 21.2 MB (21197082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7009fb73261c04c568d9dd5c1b839a02f5d97fea7f8c21705c8091eb1b6b5b6d`  
		Last Modified: Fri, 15 May 2020 04:21:54 GMT  
		Size: 244.5 KB (244519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b237016212e8e87ef0d32354521bfb76ce82ce991d8c6cc90ee0dcd82cc0392e`  
		Last Modified: Fri, 15 May 2020 04:22:04 GMT  
		Size: 25.4 MB (25368245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.96-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:a9945c4918d9c5c5ef26c826070dd74dbba790c4c401d8b6e12765ff40c280b8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44151706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd612c76d4392d6d518734ad46937b42ba37d4a772ab5addeacd13e90426149f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:19:24 GMT
ADD file:aac27626ed8520bcfd1f03f5b7aa780a4e94978b86afcc507994a8c240953561 in / 
# Wed, 13 May 2020 21:19:26 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:26:29 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 14 May 2020 00:26:48 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:27:40 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:307a7e70a6dd41fc81298d6cb2641ebfa8e7bc00b0b27f30f6559f9976a46f1e`  
		Last Modified: Wed, 13 May 2020 21:28:39 GMT  
		Size: 19.3 MB (19298476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91631fd0b2baefb452095603fc22b8be62f3657d1ae76086f6318c48f36cae25`  
		Last Modified: Thu, 14 May 2020 00:42:46 GMT  
		Size: 244.5 KB (244516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707e4565b23eaef80b85f8caf65db746d521af83f33888a710630ea91c60de18`  
		Last Modified: Thu, 14 May 2020 00:42:55 GMT  
		Size: 24.6 MB (24608714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.96-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:dc740734bf8260becbc80172fef0b0b8f06f8d330bf408430f2d87ca6481c17e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.0 MB (50034237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af66e09fed339b7fec7b623551585fc2c456c9924f2b63157140a614ce76be09`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:48:17 GMT
ADD file:53d95477395267e3c1059f1101e29a7d4b0fcb2bb52351542f4ac065ccb0b973 in / 
# Wed, 13 May 2020 21:48:19 GMT
CMD ["bash"]
# Thu, 14 May 2020 02:00:25 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 14 May 2020 02:00:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 02:01:47 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1d8af20f9b50479a890734605435a9de85d69f19b65d29c9c92f43eea2463979`  
		Last Modified: Wed, 13 May 2020 21:56:26 GMT  
		Size: 20.4 MB (20370044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5f88aa673180f3a9e54d2d3fc9c67565c9545d3072c1a42eee0eda3192c039`  
		Last Modified: Thu, 14 May 2020 02:14:51 GMT  
		Size: 244.4 KB (244366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5622468da1cdc4403ec0072a3093de5483f907e82f7e7493e9bcf66765d2367`  
		Last Modified: Thu, 14 May 2020 02:14:59 GMT  
		Size: 29.4 MB (29419827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.96-slim` - linux; 386

```console
$ docker pull mono@sha256:8b4deead0eb0a51cde3756c66f5df00ec37266e817d09f563304a477f3b56389
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.0 MB (92016693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7487028e54085f98df2000d073d14ffe16aa3465c0b6d8d07e3a14b8971427b9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:42:40 GMT
ADD file:39f8a4c4274f123e2c0a2ef48ac1a111bcc59fda68f3946ab5d644f480fab499 in / 
# Wed, 13 May 2020 21:42:41 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:33:55 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 14 May 2020 00:34:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:34:57 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1fa825514fac4b3d9226a943b4954a2efb197db27c0c1c5019bf4a5f7529746e`  
		Last Modified: Wed, 13 May 2020 21:50:17 GMT  
		Size: 23.1 MB (23141460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eac1a2c3c2e8b2376318177cabaab6efa4884e4a1262be8019864dd8d79b02d`  
		Last Modified: Thu, 14 May 2020 00:46:50 GMT  
		Size: 244.5 KB (244476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0517e1b7f3b81bc5e21be055d429fe5465bebb94609a0824c5064f1c2198ea92`  
		Last Modified: Thu, 14 May 2020 00:47:08 GMT  
		Size: 68.6 MB (68630757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.96-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:287a89353e5f4c7b3c9eb7880aaec9f53aba0c26dab0a01a9b1fc1d544978838
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48805241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:985a1f4dd9acf9434dfb803b92594e8ea0ffe7685c067b73f0ef27d05e9271b6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:42:09 GMT
ADD file:341dbc564992a44e81b3a4f399f7de14d7340a45b73c577edb78e16da2c14584 in / 
# Wed, 13 May 2020 22:42:12 GMT
CMD ["bash"]
# Thu, 14 May 2020 01:44:38 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 14 May 2020 01:45:44 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 01:47:00 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3b6ae894780534c0f99588e9cce4beb8fb7884b4578e6206b72f2db75116bb1c`  
		Last Modified: Wed, 13 May 2020 23:02:51 GMT  
		Size: 22.8 MB (22785361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0d85174db6ce48c895d3bbf3f847e1cba986fc66e705bd86bb13e3fbf73286`  
		Last Modified: Thu, 14 May 2020 02:10:48 GMT  
		Size: 244.5 KB (244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6124cc55d37923fca85643397621b030dae64f93ddf2c45ed9704bf9e9e5d141`  
		Last Modified: Thu, 14 May 2020 02:11:06 GMT  
		Size: 25.8 MB (25775347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.8.0-slim`

```console
$ docker pull mono@sha256:7db549a1569b8cda022b582142b50bf26fad154f7d1ae0274c9287142bb656bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.8.0-slim` - linux; amd64

```console
$ docker pull mono@sha256:dea2a84843d47ee855a58ca9291c5838d5f13a703074e85ce81a2b324675a091
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.3 MB (87342335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b522d57eded02abb2b3358f68714c4c066951809e1257fee584c4f22ad8347f8`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:23:03 GMT
ADD file:08ea1ff3fcd4efc24ab4f262cfa24e55e65844f6858e41a46fe0635d247f174d in / 
# Thu, 23 Apr 2020 00:23:03 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:48:15 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 23 Apr 2020 01:48:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Apr 2020 01:48:58 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b248fa9f6d2ae427ad7f00de3537ab256ae7eb413565f8be0773ee9b86ef57d4`  
		Last Modified: Thu, 23 Apr 2020 00:27:46 GMT  
		Size: 22.5 MB (22513488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5f98f65ba396764fe9568783d5a5c15abaed85471ba915f7533777d9ee788d`  
		Last Modified: Thu, 23 Apr 2020 02:19:07 GMT  
		Size: 244.5 KB (244473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06df397516278d03ee36a7c24249bc8b0b57b23701952818c89538b9856c1ffb`  
		Last Modified: Thu, 23 Apr 2020 02:19:25 GMT  
		Size: 64.6 MB (64584374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:d9c9e91dff7bbf016ee6a8f1f38041efdcf168a14ce7e2d16153ab428aeb97f6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.8 MB (46809846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b23a07406039b0f5272713478c0818cd62f58444e5e8fd5056ddd9a98f926a5`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 22:42:50 GMT
ADD file:4d807a3f2b10f72f31b43691d51a75c26c3898b53e775bfc4bc3d08720448371 in / 
# Thu, 14 May 2020 22:42:52 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:07:32 GMT
ENV MONO_VERSION=6.8.0.96
# Fri, 15 May 2020 04:07:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 04:08:51 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8c1954048f7e4cb30320daf180f1197d278a905c20d04ff10b32f11b35b7757c`  
		Last Modified: Thu, 14 May 2020 22:50:57 GMT  
		Size: 21.2 MB (21197082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7009fb73261c04c568d9dd5c1b839a02f5d97fea7f8c21705c8091eb1b6b5b6d`  
		Last Modified: Fri, 15 May 2020 04:21:54 GMT  
		Size: 244.5 KB (244519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b237016212e8e87ef0d32354521bfb76ce82ce991d8c6cc90ee0dcd82cc0392e`  
		Last Modified: Fri, 15 May 2020 04:22:04 GMT  
		Size: 25.4 MB (25368245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:a9945c4918d9c5c5ef26c826070dd74dbba790c4c401d8b6e12765ff40c280b8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44151706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd612c76d4392d6d518734ad46937b42ba37d4a772ab5addeacd13e90426149f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:19:24 GMT
ADD file:aac27626ed8520bcfd1f03f5b7aa780a4e94978b86afcc507994a8c240953561 in / 
# Wed, 13 May 2020 21:19:26 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:26:29 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 14 May 2020 00:26:48 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:27:40 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:307a7e70a6dd41fc81298d6cb2641ebfa8e7bc00b0b27f30f6559f9976a46f1e`  
		Last Modified: Wed, 13 May 2020 21:28:39 GMT  
		Size: 19.3 MB (19298476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91631fd0b2baefb452095603fc22b8be62f3657d1ae76086f6318c48f36cae25`  
		Last Modified: Thu, 14 May 2020 00:42:46 GMT  
		Size: 244.5 KB (244516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707e4565b23eaef80b85f8caf65db746d521af83f33888a710630ea91c60de18`  
		Last Modified: Thu, 14 May 2020 00:42:55 GMT  
		Size: 24.6 MB (24608714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:dc740734bf8260becbc80172fef0b0b8f06f8d330bf408430f2d87ca6481c17e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.0 MB (50034237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af66e09fed339b7fec7b623551585fc2c456c9924f2b63157140a614ce76be09`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:48:17 GMT
ADD file:53d95477395267e3c1059f1101e29a7d4b0fcb2bb52351542f4ac065ccb0b973 in / 
# Wed, 13 May 2020 21:48:19 GMT
CMD ["bash"]
# Thu, 14 May 2020 02:00:25 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 14 May 2020 02:00:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 02:01:47 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1d8af20f9b50479a890734605435a9de85d69f19b65d29c9c92f43eea2463979`  
		Last Modified: Wed, 13 May 2020 21:56:26 GMT  
		Size: 20.4 MB (20370044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5f88aa673180f3a9e54d2d3fc9c67565c9545d3072c1a42eee0eda3192c039`  
		Last Modified: Thu, 14 May 2020 02:14:51 GMT  
		Size: 244.4 KB (244366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5622468da1cdc4403ec0072a3093de5483f907e82f7e7493e9bcf66765d2367`  
		Last Modified: Thu, 14 May 2020 02:14:59 GMT  
		Size: 29.4 MB (29419827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0-slim` - linux; 386

```console
$ docker pull mono@sha256:8b4deead0eb0a51cde3756c66f5df00ec37266e817d09f563304a477f3b56389
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.0 MB (92016693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7487028e54085f98df2000d073d14ffe16aa3465c0b6d8d07e3a14b8971427b9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:42:40 GMT
ADD file:39f8a4c4274f123e2c0a2ef48ac1a111bcc59fda68f3946ab5d644f480fab499 in / 
# Wed, 13 May 2020 21:42:41 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:33:55 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 14 May 2020 00:34:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:34:57 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1fa825514fac4b3d9226a943b4954a2efb197db27c0c1c5019bf4a5f7529746e`  
		Last Modified: Wed, 13 May 2020 21:50:17 GMT  
		Size: 23.1 MB (23141460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eac1a2c3c2e8b2376318177cabaab6efa4884e4a1262be8019864dd8d79b02d`  
		Last Modified: Thu, 14 May 2020 00:46:50 GMT  
		Size: 244.5 KB (244476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0517e1b7f3b81bc5e21be055d429fe5465bebb94609a0824c5064f1c2198ea92`  
		Last Modified: Thu, 14 May 2020 00:47:08 GMT  
		Size: 68.6 MB (68630757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:287a89353e5f4c7b3c9eb7880aaec9f53aba0c26dab0a01a9b1fc1d544978838
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48805241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:985a1f4dd9acf9434dfb803b92594e8ea0ffe7685c067b73f0ef27d05e9271b6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:42:09 GMT
ADD file:341dbc564992a44e81b3a4f399f7de14d7340a45b73c577edb78e16da2c14584 in / 
# Wed, 13 May 2020 22:42:12 GMT
CMD ["bash"]
# Thu, 14 May 2020 01:44:38 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 14 May 2020 01:45:44 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 01:47:00 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3b6ae894780534c0f99588e9cce4beb8fb7884b4578e6206b72f2db75116bb1c`  
		Last Modified: Wed, 13 May 2020 23:02:51 GMT  
		Size: 22.8 MB (22785361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0d85174db6ce48c895d3bbf3f847e1cba986fc66e705bd86bb13e3fbf73286`  
		Last Modified: Thu, 14 May 2020 02:10:48 GMT  
		Size: 244.5 KB (244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6124cc55d37923fca85643397621b030dae64f93ddf2c45ed9704bf9e9e5d141`  
		Last Modified: Thu, 14 May 2020 02:11:06 GMT  
		Size: 25.8 MB (25775347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.8-slim`

```console
$ docker pull mono@sha256:7db549a1569b8cda022b582142b50bf26fad154f7d1ae0274c9287142bb656bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.8-slim` - linux; amd64

```console
$ docker pull mono@sha256:dea2a84843d47ee855a58ca9291c5838d5f13a703074e85ce81a2b324675a091
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.3 MB (87342335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b522d57eded02abb2b3358f68714c4c066951809e1257fee584c4f22ad8347f8`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:23:03 GMT
ADD file:08ea1ff3fcd4efc24ab4f262cfa24e55e65844f6858e41a46fe0635d247f174d in / 
# Thu, 23 Apr 2020 00:23:03 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:48:15 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 23 Apr 2020 01:48:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Apr 2020 01:48:58 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b248fa9f6d2ae427ad7f00de3537ab256ae7eb413565f8be0773ee9b86ef57d4`  
		Last Modified: Thu, 23 Apr 2020 00:27:46 GMT  
		Size: 22.5 MB (22513488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5f98f65ba396764fe9568783d5a5c15abaed85471ba915f7533777d9ee788d`  
		Last Modified: Thu, 23 Apr 2020 02:19:07 GMT  
		Size: 244.5 KB (244473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06df397516278d03ee36a7c24249bc8b0b57b23701952818c89538b9856c1ffb`  
		Last Modified: Thu, 23 Apr 2020 02:19:25 GMT  
		Size: 64.6 MB (64584374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:d9c9e91dff7bbf016ee6a8f1f38041efdcf168a14ce7e2d16153ab428aeb97f6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.8 MB (46809846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b23a07406039b0f5272713478c0818cd62f58444e5e8fd5056ddd9a98f926a5`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 22:42:50 GMT
ADD file:4d807a3f2b10f72f31b43691d51a75c26c3898b53e775bfc4bc3d08720448371 in / 
# Thu, 14 May 2020 22:42:52 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:07:32 GMT
ENV MONO_VERSION=6.8.0.96
# Fri, 15 May 2020 04:07:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 04:08:51 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8c1954048f7e4cb30320daf180f1197d278a905c20d04ff10b32f11b35b7757c`  
		Last Modified: Thu, 14 May 2020 22:50:57 GMT  
		Size: 21.2 MB (21197082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7009fb73261c04c568d9dd5c1b839a02f5d97fea7f8c21705c8091eb1b6b5b6d`  
		Last Modified: Fri, 15 May 2020 04:21:54 GMT  
		Size: 244.5 KB (244519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b237016212e8e87ef0d32354521bfb76ce82ce991d8c6cc90ee0dcd82cc0392e`  
		Last Modified: Fri, 15 May 2020 04:22:04 GMT  
		Size: 25.4 MB (25368245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:a9945c4918d9c5c5ef26c826070dd74dbba790c4c401d8b6e12765ff40c280b8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44151706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd612c76d4392d6d518734ad46937b42ba37d4a772ab5addeacd13e90426149f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:19:24 GMT
ADD file:aac27626ed8520bcfd1f03f5b7aa780a4e94978b86afcc507994a8c240953561 in / 
# Wed, 13 May 2020 21:19:26 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:26:29 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 14 May 2020 00:26:48 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:27:40 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:307a7e70a6dd41fc81298d6cb2641ebfa8e7bc00b0b27f30f6559f9976a46f1e`  
		Last Modified: Wed, 13 May 2020 21:28:39 GMT  
		Size: 19.3 MB (19298476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91631fd0b2baefb452095603fc22b8be62f3657d1ae76086f6318c48f36cae25`  
		Last Modified: Thu, 14 May 2020 00:42:46 GMT  
		Size: 244.5 KB (244516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707e4565b23eaef80b85f8caf65db746d521af83f33888a710630ea91c60de18`  
		Last Modified: Thu, 14 May 2020 00:42:55 GMT  
		Size: 24.6 MB (24608714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:dc740734bf8260becbc80172fef0b0b8f06f8d330bf408430f2d87ca6481c17e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.0 MB (50034237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af66e09fed339b7fec7b623551585fc2c456c9924f2b63157140a614ce76be09`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:48:17 GMT
ADD file:53d95477395267e3c1059f1101e29a7d4b0fcb2bb52351542f4ac065ccb0b973 in / 
# Wed, 13 May 2020 21:48:19 GMT
CMD ["bash"]
# Thu, 14 May 2020 02:00:25 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 14 May 2020 02:00:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 02:01:47 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1d8af20f9b50479a890734605435a9de85d69f19b65d29c9c92f43eea2463979`  
		Last Modified: Wed, 13 May 2020 21:56:26 GMT  
		Size: 20.4 MB (20370044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5f88aa673180f3a9e54d2d3fc9c67565c9545d3072c1a42eee0eda3192c039`  
		Last Modified: Thu, 14 May 2020 02:14:51 GMT  
		Size: 244.4 KB (244366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5622468da1cdc4403ec0072a3093de5483f907e82f7e7493e9bcf66765d2367`  
		Last Modified: Thu, 14 May 2020 02:14:59 GMT  
		Size: 29.4 MB (29419827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8-slim` - linux; 386

```console
$ docker pull mono@sha256:8b4deead0eb0a51cde3756c66f5df00ec37266e817d09f563304a477f3b56389
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.0 MB (92016693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7487028e54085f98df2000d073d14ffe16aa3465c0b6d8d07e3a14b8971427b9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:42:40 GMT
ADD file:39f8a4c4274f123e2c0a2ef48ac1a111bcc59fda68f3946ab5d644f480fab499 in / 
# Wed, 13 May 2020 21:42:41 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:33:55 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 14 May 2020 00:34:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:34:57 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1fa825514fac4b3d9226a943b4954a2efb197db27c0c1c5019bf4a5f7529746e`  
		Last Modified: Wed, 13 May 2020 21:50:17 GMT  
		Size: 23.1 MB (23141460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eac1a2c3c2e8b2376318177cabaab6efa4884e4a1262be8019864dd8d79b02d`  
		Last Modified: Thu, 14 May 2020 00:46:50 GMT  
		Size: 244.5 KB (244476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0517e1b7f3b81bc5e21be055d429fe5465bebb94609a0824c5064f1c2198ea92`  
		Last Modified: Thu, 14 May 2020 00:47:08 GMT  
		Size: 68.6 MB (68630757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:287a89353e5f4c7b3c9eb7880aaec9f53aba0c26dab0a01a9b1fc1d544978838
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48805241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:985a1f4dd9acf9434dfb803b92594e8ea0ffe7685c067b73f0ef27d05e9271b6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:42:09 GMT
ADD file:341dbc564992a44e81b3a4f399f7de14d7340a45b73c577edb78e16da2c14584 in / 
# Wed, 13 May 2020 22:42:12 GMT
CMD ["bash"]
# Thu, 14 May 2020 01:44:38 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 14 May 2020 01:45:44 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 01:47:00 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3b6ae894780534c0f99588e9cce4beb8fb7884b4578e6206b72f2db75116bb1c`  
		Last Modified: Wed, 13 May 2020 23:02:51 GMT  
		Size: 22.8 MB (22785361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0d85174db6ce48c895d3bbf3f847e1cba986fc66e705bd86bb13e3fbf73286`  
		Last Modified: Thu, 14 May 2020 02:10:48 GMT  
		Size: 244.5 KB (244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6124cc55d37923fca85643397621b030dae64f93ddf2c45ed9704bf9e9e5d141`  
		Last Modified: Thu, 14 May 2020 02:11:06 GMT  
		Size: 25.8 MB (25775347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6-slim`

```console
$ docker pull mono@sha256:7db549a1569b8cda022b582142b50bf26fad154f7d1ae0274c9287142bb656bb
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
$ docker pull mono@sha256:dea2a84843d47ee855a58ca9291c5838d5f13a703074e85ce81a2b324675a091
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.3 MB (87342335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b522d57eded02abb2b3358f68714c4c066951809e1257fee584c4f22ad8347f8`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:23:03 GMT
ADD file:08ea1ff3fcd4efc24ab4f262cfa24e55e65844f6858e41a46fe0635d247f174d in / 
# Thu, 23 Apr 2020 00:23:03 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:48:15 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 23 Apr 2020 01:48:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Apr 2020 01:48:58 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b248fa9f6d2ae427ad7f00de3537ab256ae7eb413565f8be0773ee9b86ef57d4`  
		Last Modified: Thu, 23 Apr 2020 00:27:46 GMT  
		Size: 22.5 MB (22513488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5f98f65ba396764fe9568783d5a5c15abaed85471ba915f7533777d9ee788d`  
		Last Modified: Thu, 23 Apr 2020 02:19:07 GMT  
		Size: 244.5 KB (244473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06df397516278d03ee36a7c24249bc8b0b57b23701952818c89538b9856c1ffb`  
		Last Modified: Thu, 23 Apr 2020 02:19:25 GMT  
		Size: 64.6 MB (64584374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:d9c9e91dff7bbf016ee6a8f1f38041efdcf168a14ce7e2d16153ab428aeb97f6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.8 MB (46809846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b23a07406039b0f5272713478c0818cd62f58444e5e8fd5056ddd9a98f926a5`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 22:42:50 GMT
ADD file:4d807a3f2b10f72f31b43691d51a75c26c3898b53e775bfc4bc3d08720448371 in / 
# Thu, 14 May 2020 22:42:52 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:07:32 GMT
ENV MONO_VERSION=6.8.0.96
# Fri, 15 May 2020 04:07:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 04:08:51 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8c1954048f7e4cb30320daf180f1197d278a905c20d04ff10b32f11b35b7757c`  
		Last Modified: Thu, 14 May 2020 22:50:57 GMT  
		Size: 21.2 MB (21197082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7009fb73261c04c568d9dd5c1b839a02f5d97fea7f8c21705c8091eb1b6b5b6d`  
		Last Modified: Fri, 15 May 2020 04:21:54 GMT  
		Size: 244.5 KB (244519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b237016212e8e87ef0d32354521bfb76ce82ce991d8c6cc90ee0dcd82cc0392e`  
		Last Modified: Fri, 15 May 2020 04:22:04 GMT  
		Size: 25.4 MB (25368245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:a9945c4918d9c5c5ef26c826070dd74dbba790c4c401d8b6e12765ff40c280b8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44151706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd612c76d4392d6d518734ad46937b42ba37d4a772ab5addeacd13e90426149f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:19:24 GMT
ADD file:aac27626ed8520bcfd1f03f5b7aa780a4e94978b86afcc507994a8c240953561 in / 
# Wed, 13 May 2020 21:19:26 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:26:29 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 14 May 2020 00:26:48 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:27:40 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:307a7e70a6dd41fc81298d6cb2641ebfa8e7bc00b0b27f30f6559f9976a46f1e`  
		Last Modified: Wed, 13 May 2020 21:28:39 GMT  
		Size: 19.3 MB (19298476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91631fd0b2baefb452095603fc22b8be62f3657d1ae76086f6318c48f36cae25`  
		Last Modified: Thu, 14 May 2020 00:42:46 GMT  
		Size: 244.5 KB (244516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707e4565b23eaef80b85f8caf65db746d521af83f33888a710630ea91c60de18`  
		Last Modified: Thu, 14 May 2020 00:42:55 GMT  
		Size: 24.6 MB (24608714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:dc740734bf8260becbc80172fef0b0b8f06f8d330bf408430f2d87ca6481c17e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.0 MB (50034237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af66e09fed339b7fec7b623551585fc2c456c9924f2b63157140a614ce76be09`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:48:17 GMT
ADD file:53d95477395267e3c1059f1101e29a7d4b0fcb2bb52351542f4ac065ccb0b973 in / 
# Wed, 13 May 2020 21:48:19 GMT
CMD ["bash"]
# Thu, 14 May 2020 02:00:25 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 14 May 2020 02:00:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 02:01:47 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1d8af20f9b50479a890734605435a9de85d69f19b65d29c9c92f43eea2463979`  
		Last Modified: Wed, 13 May 2020 21:56:26 GMT  
		Size: 20.4 MB (20370044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5f88aa673180f3a9e54d2d3fc9c67565c9545d3072c1a42eee0eda3192c039`  
		Last Modified: Thu, 14 May 2020 02:14:51 GMT  
		Size: 244.4 KB (244366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5622468da1cdc4403ec0072a3093de5483f907e82f7e7493e9bcf66765d2367`  
		Last Modified: Thu, 14 May 2020 02:14:59 GMT  
		Size: 29.4 MB (29419827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; 386

```console
$ docker pull mono@sha256:8b4deead0eb0a51cde3756c66f5df00ec37266e817d09f563304a477f3b56389
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.0 MB (92016693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7487028e54085f98df2000d073d14ffe16aa3465c0b6d8d07e3a14b8971427b9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:42:40 GMT
ADD file:39f8a4c4274f123e2c0a2ef48ac1a111bcc59fda68f3946ab5d644f480fab499 in / 
# Wed, 13 May 2020 21:42:41 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:33:55 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 14 May 2020 00:34:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:34:57 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1fa825514fac4b3d9226a943b4954a2efb197db27c0c1c5019bf4a5f7529746e`  
		Last Modified: Wed, 13 May 2020 21:50:17 GMT  
		Size: 23.1 MB (23141460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eac1a2c3c2e8b2376318177cabaab6efa4884e4a1262be8019864dd8d79b02d`  
		Last Modified: Thu, 14 May 2020 00:46:50 GMT  
		Size: 244.5 KB (244476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0517e1b7f3b81bc5e21be055d429fe5465bebb94609a0824c5064f1c2198ea92`  
		Last Modified: Thu, 14 May 2020 00:47:08 GMT  
		Size: 68.6 MB (68630757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:287a89353e5f4c7b3c9eb7880aaec9f53aba0c26dab0a01a9b1fc1d544978838
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48805241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:985a1f4dd9acf9434dfb803b92594e8ea0ffe7685c067b73f0ef27d05e9271b6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:42:09 GMT
ADD file:341dbc564992a44e81b3a4f399f7de14d7340a45b73c577edb78e16da2c14584 in / 
# Wed, 13 May 2020 22:42:12 GMT
CMD ["bash"]
# Thu, 14 May 2020 01:44:38 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 14 May 2020 01:45:44 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 01:47:00 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3b6ae894780534c0f99588e9cce4beb8fb7884b4578e6206b72f2db75116bb1c`  
		Last Modified: Wed, 13 May 2020 23:02:51 GMT  
		Size: 22.8 MB (22785361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0d85174db6ce48c895d3bbf3f847e1cba986fc66e705bd86bb13e3fbf73286`  
		Last Modified: Thu, 14 May 2020 02:10:48 GMT  
		Size: 244.5 KB (244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6124cc55d37923fca85643397621b030dae64f93ddf2c45ed9704bf9e9e5d141`  
		Last Modified: Thu, 14 May 2020 02:11:06 GMT  
		Size: 25.8 MB (25775347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:latest`

```console
$ docker pull mono@sha256:77e66aca06ed4914a850ce5a590698acdc7c2f71a197b4428a0a6fe145bb0027
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
$ docker pull mono@sha256:2351a2ba6c2228ecac8696680f65e49607432bb7fd6c0494fd254060c48f6a02
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.1 MB (235136555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59599093bfc20b4291b6019e7cd8bd648dab8dc3c341bc26001f807264ac44dc`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:23:03 GMT
ADD file:08ea1ff3fcd4efc24ab4f262cfa24e55e65844f6858e41a46fe0635d247f174d in / 
# Thu, 23 Apr 2020 00:23:03 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:48:15 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 23 Apr 2020 01:48:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Apr 2020 01:48:58 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 23 Apr 2020 01:59:28 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b248fa9f6d2ae427ad7f00de3537ab256ae7eb413565f8be0773ee9b86ef57d4`  
		Last Modified: Thu, 23 Apr 2020 00:27:46 GMT  
		Size: 22.5 MB (22513488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5f98f65ba396764fe9568783d5a5c15abaed85471ba915f7533777d9ee788d`  
		Last Modified: Thu, 23 Apr 2020 02:19:07 GMT  
		Size: 244.5 KB (244473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06df397516278d03ee36a7c24249bc8b0b57b23701952818c89538b9856c1ffb`  
		Last Modified: Thu, 23 Apr 2020 02:19:25 GMT  
		Size: 64.6 MB (64584374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e83f8e35ba5681f2772165e09a403fab75e2cb54d9c6166e85301ad905d258`  
		Last Modified: Thu, 23 Apr 2020 02:20:55 GMT  
		Size: 147.8 MB (147794220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm variant v5

```console
$ docker pull mono@sha256:5be1950fc69cdd2737286151d13e08b8a810ce402c4e961abec76247ef5d87f5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.7 MB (176701525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7285a10f55436a04b15962a4fe25b96046a348c1a02a15aa64d07e2369f2ed5`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 22:42:50 GMT
ADD file:4d807a3f2b10f72f31b43691d51a75c26c3898b53e775bfc4bc3d08720448371 in / 
# Thu, 14 May 2020 22:42:52 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:07:32 GMT
ENV MONO_VERSION=6.8.0.96
# Fri, 15 May 2020 04:07:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 04:08:51 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 15 May 2020 04:14:47 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8c1954048f7e4cb30320daf180f1197d278a905c20d04ff10b32f11b35b7757c`  
		Last Modified: Thu, 14 May 2020 22:50:57 GMT  
		Size: 21.2 MB (21197082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7009fb73261c04c568d9dd5c1b839a02f5d97fea7f8c21705c8091eb1b6b5b6d`  
		Last Modified: Fri, 15 May 2020 04:21:54 GMT  
		Size: 244.5 KB (244519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b237016212e8e87ef0d32354521bfb76ce82ce991d8c6cc90ee0dcd82cc0392e`  
		Last Modified: Fri, 15 May 2020 04:22:04 GMT  
		Size: 25.4 MB (25368245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f7186fdafac062d1af6c86d4fca2df0b62f320aec72fcbbd7b8cb4d6fcf467`  
		Last Modified: Fri, 15 May 2020 04:23:35 GMT  
		Size: 129.9 MB (129891679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm variant v7

```console
$ docker pull mono@sha256:55ef6d96d85e1d0e3aca832b8c2a7a0b7da50bffa2dacf77542fbd7aff27a559
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.7 MB (172707764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc9acd8a77a391a80d27014968c3dfe08186f34930cc569f44c35d2a7a09b22c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:19:24 GMT
ADD file:aac27626ed8520bcfd1f03f5b7aa780a4e94978b86afcc507994a8c240953561 in / 
# Wed, 13 May 2020 21:19:26 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:26:29 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 14 May 2020 00:26:48 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:27:40 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 00:33:55 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:307a7e70a6dd41fc81298d6cb2641ebfa8e7bc00b0b27f30f6559f9976a46f1e`  
		Last Modified: Wed, 13 May 2020 21:28:39 GMT  
		Size: 19.3 MB (19298476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91631fd0b2baefb452095603fc22b8be62f3657d1ae76086f6318c48f36cae25`  
		Last Modified: Thu, 14 May 2020 00:42:46 GMT  
		Size: 244.5 KB (244516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707e4565b23eaef80b85f8caf65db746d521af83f33888a710630ea91c60de18`  
		Last Modified: Thu, 14 May 2020 00:42:55 GMT  
		Size: 24.6 MB (24608714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a42be730e2ad23f35deb8b93a0913d13edb02be20a73fa837770d36acbbf74`  
		Last Modified: Thu, 14 May 2020 00:44:20 GMT  
		Size: 128.6 MB (128556058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:cbc1409b11ea1fd492744b6396ef5a9afa4bd427de25d89ea8406fbd9189d0a7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.7 MB (194747627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:939138ef9b9d3ec1af2baae95869f7cf8c66020511a3bb70138be5e5dd8450f2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:48:17 GMT
ADD file:53d95477395267e3c1059f1101e29a7d4b0fcb2bb52351542f4ac065ccb0b973 in / 
# Wed, 13 May 2020 21:48:19 GMT
CMD ["bash"]
# Thu, 14 May 2020 02:00:25 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 14 May 2020 02:00:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 02:01:47 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 02:07:30 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1d8af20f9b50479a890734605435a9de85d69f19b65d29c9c92f43eea2463979`  
		Last Modified: Wed, 13 May 2020 21:56:26 GMT  
		Size: 20.4 MB (20370044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5f88aa673180f3a9e54d2d3fc9c67565c9545d3072c1a42eee0eda3192c039`  
		Last Modified: Thu, 14 May 2020 02:14:51 GMT  
		Size: 244.4 KB (244366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5622468da1cdc4403ec0072a3093de5483f907e82f7e7493e9bcf66765d2367`  
		Last Modified: Thu, 14 May 2020 02:14:59 GMT  
		Size: 29.4 MB (29419827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a79b7e06bf892f3f0e1c21e1bdc62517abc6fd4fd31a2f0be27e369398f2d0ca`  
		Last Modified: Thu, 14 May 2020 02:16:28 GMT  
		Size: 144.7 MB (144713390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; 386

```console
$ docker pull mono@sha256:91becebb427753ead531605be391b0528b1b8176f46762f3fb896b58fbf493f5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.5 MB (243509833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d912f07467de168fbaadffea2b2be97d24f40de4675c1ef98b3b7c70f274b9c5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:42:40 GMT
ADD file:39f8a4c4274f123e2c0a2ef48ac1a111bcc59fda68f3946ab5d644f480fab499 in / 
# Wed, 13 May 2020 21:42:41 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:33:55 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 14 May 2020 00:34:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:34:57 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 00:40:29 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1fa825514fac4b3d9226a943b4954a2efb197db27c0c1c5019bf4a5f7529746e`  
		Last Modified: Wed, 13 May 2020 21:50:17 GMT  
		Size: 23.1 MB (23141460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eac1a2c3c2e8b2376318177cabaab6efa4884e4a1262be8019864dd8d79b02d`  
		Last Modified: Thu, 14 May 2020 00:46:50 GMT  
		Size: 244.5 KB (244476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0517e1b7f3b81bc5e21be055d429fe5465bebb94609a0824c5064f1c2198ea92`  
		Last Modified: Thu, 14 May 2020 00:47:08 GMT  
		Size: 68.6 MB (68630757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b33be2fe9551abfc1002c4bad0c8ce971f275c3ca146936540551c5776b4fd4`  
		Last Modified: Thu, 14 May 2020 00:49:07 GMT  
		Size: 151.5 MB (151493140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; ppc64le

```console
$ docker pull mono@sha256:28211181008fc8a25dbc12b5f75fd4857e92af22ee4716fd13064027ba80c113
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.0 MB (178995744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcbdcf050885aeb282b85d9942bee597145d594577643da02a09cb638cd2edb9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:42:09 GMT
ADD file:341dbc564992a44e81b3a4f399f7de14d7340a45b73c577edb78e16da2c14584 in / 
# Wed, 13 May 2020 22:42:12 GMT
CMD ["bash"]
# Thu, 14 May 2020 01:44:38 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 14 May 2020 01:45:44 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 01:47:00 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 14 May 2020 01:57:53 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3b6ae894780534c0f99588e9cce4beb8fb7884b4578e6206b72f2db75116bb1c`  
		Last Modified: Wed, 13 May 2020 23:02:51 GMT  
		Size: 22.8 MB (22785361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0d85174db6ce48c895d3bbf3f847e1cba986fc66e705bd86bb13e3fbf73286`  
		Last Modified: Thu, 14 May 2020 02:10:48 GMT  
		Size: 244.5 KB (244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6124cc55d37923fca85643397621b030dae64f93ddf2c45ed9704bf9e9e5d141`  
		Last Modified: Thu, 14 May 2020 02:11:06 GMT  
		Size: 25.8 MB (25775347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64bc6db4438da29e772ebf533c91b52b035c322c12bf45899c0cbcff8a42ba24`  
		Last Modified: Thu, 14 May 2020 02:13:51 GMT  
		Size: 130.2 MB (130190503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:slim`

```console
$ docker pull mono@sha256:7db549a1569b8cda022b582142b50bf26fad154f7d1ae0274c9287142bb656bb
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
$ docker pull mono@sha256:dea2a84843d47ee855a58ca9291c5838d5f13a703074e85ce81a2b324675a091
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.3 MB (87342335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b522d57eded02abb2b3358f68714c4c066951809e1257fee584c4f22ad8347f8`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:23:03 GMT
ADD file:08ea1ff3fcd4efc24ab4f262cfa24e55e65844f6858e41a46fe0635d247f174d in / 
# Thu, 23 Apr 2020 00:23:03 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:48:15 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 23 Apr 2020 01:48:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Apr 2020 01:48:58 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b248fa9f6d2ae427ad7f00de3537ab256ae7eb413565f8be0773ee9b86ef57d4`  
		Last Modified: Thu, 23 Apr 2020 00:27:46 GMT  
		Size: 22.5 MB (22513488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5f98f65ba396764fe9568783d5a5c15abaed85471ba915f7533777d9ee788d`  
		Last Modified: Thu, 23 Apr 2020 02:19:07 GMT  
		Size: 244.5 KB (244473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06df397516278d03ee36a7c24249bc8b0b57b23701952818c89538b9856c1ffb`  
		Last Modified: Thu, 23 Apr 2020 02:19:25 GMT  
		Size: 64.6 MB (64584374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:d9c9e91dff7bbf016ee6a8f1f38041efdcf168a14ce7e2d16153ab428aeb97f6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.8 MB (46809846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b23a07406039b0f5272713478c0818cd62f58444e5e8fd5056ddd9a98f926a5`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 22:42:50 GMT
ADD file:4d807a3f2b10f72f31b43691d51a75c26c3898b53e775bfc4bc3d08720448371 in / 
# Thu, 14 May 2020 22:42:52 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:07:32 GMT
ENV MONO_VERSION=6.8.0.96
# Fri, 15 May 2020 04:07:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 04:08:51 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8c1954048f7e4cb30320daf180f1197d278a905c20d04ff10b32f11b35b7757c`  
		Last Modified: Thu, 14 May 2020 22:50:57 GMT  
		Size: 21.2 MB (21197082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7009fb73261c04c568d9dd5c1b839a02f5d97fea7f8c21705c8091eb1b6b5b6d`  
		Last Modified: Fri, 15 May 2020 04:21:54 GMT  
		Size: 244.5 KB (244519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b237016212e8e87ef0d32354521bfb76ce82ce991d8c6cc90ee0dcd82cc0392e`  
		Last Modified: Fri, 15 May 2020 04:22:04 GMT  
		Size: 25.4 MB (25368245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:a9945c4918d9c5c5ef26c826070dd74dbba790c4c401d8b6e12765ff40c280b8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44151706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd612c76d4392d6d518734ad46937b42ba37d4a772ab5addeacd13e90426149f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:19:24 GMT
ADD file:aac27626ed8520bcfd1f03f5b7aa780a4e94978b86afcc507994a8c240953561 in / 
# Wed, 13 May 2020 21:19:26 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:26:29 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 14 May 2020 00:26:48 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:27:40 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:307a7e70a6dd41fc81298d6cb2641ebfa8e7bc00b0b27f30f6559f9976a46f1e`  
		Last Modified: Wed, 13 May 2020 21:28:39 GMT  
		Size: 19.3 MB (19298476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91631fd0b2baefb452095603fc22b8be62f3657d1ae76086f6318c48f36cae25`  
		Last Modified: Thu, 14 May 2020 00:42:46 GMT  
		Size: 244.5 KB (244516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707e4565b23eaef80b85f8caf65db746d521af83f33888a710630ea91c60de18`  
		Last Modified: Thu, 14 May 2020 00:42:55 GMT  
		Size: 24.6 MB (24608714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:dc740734bf8260becbc80172fef0b0b8f06f8d330bf408430f2d87ca6481c17e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.0 MB (50034237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af66e09fed339b7fec7b623551585fc2c456c9924f2b63157140a614ce76be09`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:48:17 GMT
ADD file:53d95477395267e3c1059f1101e29a7d4b0fcb2bb52351542f4ac065ccb0b973 in / 
# Wed, 13 May 2020 21:48:19 GMT
CMD ["bash"]
# Thu, 14 May 2020 02:00:25 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 14 May 2020 02:00:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 02:01:47 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1d8af20f9b50479a890734605435a9de85d69f19b65d29c9c92f43eea2463979`  
		Last Modified: Wed, 13 May 2020 21:56:26 GMT  
		Size: 20.4 MB (20370044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5f88aa673180f3a9e54d2d3fc9c67565c9545d3072c1a42eee0eda3192c039`  
		Last Modified: Thu, 14 May 2020 02:14:51 GMT  
		Size: 244.4 KB (244366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5622468da1cdc4403ec0072a3093de5483f907e82f7e7493e9bcf66765d2367`  
		Last Modified: Thu, 14 May 2020 02:14:59 GMT  
		Size: 29.4 MB (29419827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; 386

```console
$ docker pull mono@sha256:8b4deead0eb0a51cde3756c66f5df00ec37266e817d09f563304a477f3b56389
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.0 MB (92016693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7487028e54085f98df2000d073d14ffe16aa3465c0b6d8d07e3a14b8971427b9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:42:40 GMT
ADD file:39f8a4c4274f123e2c0a2ef48ac1a111bcc59fda68f3946ab5d644f480fab499 in / 
# Wed, 13 May 2020 21:42:41 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:33:55 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 14 May 2020 00:34:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 00:34:57 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:1fa825514fac4b3d9226a943b4954a2efb197db27c0c1c5019bf4a5f7529746e`  
		Last Modified: Wed, 13 May 2020 21:50:17 GMT  
		Size: 23.1 MB (23141460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eac1a2c3c2e8b2376318177cabaab6efa4884e4a1262be8019864dd8d79b02d`  
		Last Modified: Thu, 14 May 2020 00:46:50 GMT  
		Size: 244.5 KB (244476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0517e1b7f3b81bc5e21be055d429fe5465bebb94609a0824c5064f1c2198ea92`  
		Last Modified: Thu, 14 May 2020 00:47:08 GMT  
		Size: 68.6 MB (68630757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; ppc64le

```console
$ docker pull mono@sha256:287a89353e5f4c7b3c9eb7880aaec9f53aba0c26dab0a01a9b1fc1d544978838
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48805241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:985a1f4dd9acf9434dfb803b92594e8ea0ffe7685c067b73f0ef27d05e9271b6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:42:09 GMT
ADD file:341dbc564992a44e81b3a4f399f7de14d7340a45b73c577edb78e16da2c14584 in / 
# Wed, 13 May 2020 22:42:12 GMT
CMD ["bash"]
# Thu, 14 May 2020 01:44:38 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 14 May 2020 01:45:44 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 14 May 2020 01:47:00 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3b6ae894780534c0f99588e9cce4beb8fb7884b4578e6206b72f2db75116bb1c`  
		Last Modified: Wed, 13 May 2020 23:02:51 GMT  
		Size: 22.8 MB (22785361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0d85174db6ce48c895d3bbf3f847e1cba986fc66e705bd86bb13e3fbf73286`  
		Last Modified: Thu, 14 May 2020 02:10:48 GMT  
		Size: 244.5 KB (244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6124cc55d37923fca85643397621b030dae64f93ddf2c45ed9704bf9e9e5d141`  
		Last Modified: Thu, 14 May 2020 02:11:06 GMT  
		Size: 25.8 MB (25775347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
