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
$ docker pull mono@sha256:7391b3078f74b4fb71bfe3540c5390a5eed4b3811d965657f051968938e478c0
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
$ docker pull mono@sha256:436da53a1faac7a43322ebac255c97669f9f56d8b85613c47a8c62d603bfb451
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.1 MB (236118822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0363bd6b4181844fc0fe64cf89aaf499c064fe28e5df53518b050d9582253514`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:36:49 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 21 Dec 2021 02:37:06 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 02:37:36 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Dec 2021 02:45:08 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8678af474ab209c6f77514a3e861bb6e382fdd4f519efa3c08708b70676f7714`  
		Last Modified: Tue, 21 Dec 2021 02:52:42 GMT  
		Size: 2.8 MB (2767125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad55ab33cb43c5e91426eb50f5804dfaa25e4ca85d8faef05dc9894b16af2148`  
		Last Modified: Tue, 21 Dec 2021 02:52:54 GMT  
		Size: 64.8 MB (64760075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ec649bf9968b1e1c72798fc1e41260bbc80435ee4ce1e0592b19aa56ecf3ca`  
		Last Modified: Tue, 21 Dec 2021 02:54:01 GMT  
		Size: 141.4 MB (141437899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; arm variant v5

```console
$ docker pull mono@sha256:7ac5ca79c9b5e75e4e0f3bfe2b9aa70bbff7732fe99d94d54071cf51caad9585
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.9 MB (191928318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c3e96fe01b11bc7320ba93f00f68f0af7a7964d5a09d6d25b69b4382a131c93`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:51:32 GMT
ADD file:f757929225218280f26d0eca53387788343e93cc9658f5baeb58957776114579 in / 
# Tue, 21 Dec 2021 01:51:33 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:42:14 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 21 Dec 2021 03:42:48 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 03:43:35 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Dec 2021 03:48:47 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7d69cd3acec6d9e5ca88bdd718b069a7272b722048f49b6d21fbe85fc6c82560`  
		Last Modified: Tue, 21 Dec 2021 02:07:21 GMT  
		Size: 24.9 MB (24886253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9083493d202e9a9d70bb069d8ede78d5dd4a01013dfed35779a92aca045b93`  
		Last Modified: Tue, 21 Dec 2021 03:53:53 GMT  
		Size: 2.5 MB (2462568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e64cb7f034664931a2081c40c52b36a04cdd979ff44aed8df991b489266dee3`  
		Last Modified: Tue, 21 Dec 2021 03:54:10 GMT  
		Size: 24.5 MB (24493026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603e8451b8054b91d675124edf960b8e9d6a04dfb2a167c5cd5c38d670d9d189`  
		Last Modified: Tue, 21 Dec 2021 03:56:37 GMT  
		Size: 140.1 MB (140086471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; arm variant v7

```console
$ docker pull mono@sha256:42b8007b66564f9e1805b9cb16262788769a0d6178bc017943cb67f1cdd09852
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.8 MB (187845357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84f0965a3989be17ac2e2777a90aa48d8dbdea4842f795d0ca25bd9732b91c7d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:00:52 GMT
ADD file:1381e18e2847f24ebd16d8e83ad940adeff45aca2c327d4e07d7451816f29420 in / 
# Tue, 21 Dec 2021 02:00:52 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:50:08 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 21 Dec 2021 07:50:34 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 07:51:18 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Dec 2021 07:55:58 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b597e1a6bc27aa2a24a587cb687c9551dfbcfa730a11d48c5a44ff77ff6fdd75`  
		Last Modified: Tue, 21 Dec 2021 02:16:50 GMT  
		Size: 22.8 MB (22754324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf6c5f7fad1939cd9be660d18ca40d4402c8e8edb6fccb486497e7f2f7a1f72`  
		Last Modified: Tue, 21 Dec 2021 08:00:51 GMT  
		Size: 2.4 MB (2361910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c45bb2608bc2763ce62f4c08b6d3137040af4b25c52a94abfced92aaf5fee7`  
		Last Modified: Tue, 21 Dec 2021 08:01:08 GMT  
		Size: 23.8 MB (23782737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846af906bfa50c717b3f4340504b8a39511f1709951019c319d941be991cb57a`  
		Last Modified: Tue, 21 Dec 2021 08:03:41 GMT  
		Size: 138.9 MB (138946386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:9329630412680f37b655e8d0a47c1d9b3dbe3c4e1371f3c28e7279666bc6cd6f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.5 MB (214451374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11180fb2db08adf228b4d3709468115b2d40d66b874ccac4ed9a041d5e10b827`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:34 GMT
ADD file:83d9e760a84be2bd8754e31e33b3f782b44f6e7b7e02c156f519715c88c40615 in / 
# Thu, 02 Dec 2021 08:08:35 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 10:31:32 GMT
ENV MONO_VERSION=6.12.0.122
# Thu, 02 Dec 2021 10:31:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 02 Dec 2021 10:32:05 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 02 Dec 2021 10:33:50 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2a37a2e6ba8cbf21e3950cf7b2455f0af054667b6a35719fb2bd6070973bfa76`  
		Last Modified: Thu, 02 Dec 2021 08:41:37 GMT  
		Size: 25.9 MB (25923144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9881b3a1bbaf2479f58c7e7e0a008ba9dfcfd9a404b8a45f61e67b19f8a2b493`  
		Last Modified: Thu, 02 Dec 2021 10:35:43 GMT  
		Size: 2.6 MB (2634639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a63bac7bf077258f21a6462bb51b790fdfd8c75ff13922648615e0ecd2755c`  
		Last Modified: Thu, 02 Dec 2021 10:35:48 GMT  
		Size: 29.3 MB (29318432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:286d86521574d7ba2c433336ba4f2dc6bfe465c5ebf2a9b729361e3811ac1c89`  
		Last Modified: Thu, 02 Dec 2021 10:36:49 GMT  
		Size: 156.6 MB (156575159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; 386

```console
$ docker pull mono@sha256:324b2a76dcdbc9e52fc9e54df41809e830f86c065a95a0e154bfe8688fd5b8b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.9 MB (241920513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9820eafdb94e0b17dce68c576278588547a421e7817858cd8e62e1ae0c6b482`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:40:25 GMT
ADD file:9063906ecf2b5c82bf37cb574e78f61add2cd7aa8d0675647be379e30e19b6a9 in / 
# Thu, 02 Dec 2021 02:40:25 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 14:55:37 GMT
ENV MONO_VERSION=6.12.0.122
# Thu, 02 Dec 2021 14:55:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 02 Dec 2021 14:56:21 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 02 Dec 2021 14:59:07 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3b938b4b72623e9d1494d498630cd883df97fd6882fb9e0edb7af6714fce4e83`  
		Last Modified: Thu, 02 Dec 2021 02:49:02 GMT  
		Size: 27.8 MB (27804562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33df0d561cd5f2e983795fefe65289181d4ec840095931cf18b11ff6c7bf28c2`  
		Last Modified: Thu, 02 Dec 2021 15:03:01 GMT  
		Size: 2.8 MB (2781457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2ba8412a0fc14d63cab8249ab154c0f32239599e76bfd072203cc83b8a6bc4`  
		Last Modified: Thu, 02 Dec 2021 15:03:22 GMT  
		Size: 68.8 MB (68778451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4de88484565bfcbf695bf90edb1ba6a692de60b55362f113e5f5894e535ca95f`  
		Last Modified: Thu, 02 Dec 2021 15:04:49 GMT  
		Size: 142.6 MB (142556043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; ppc64le

```console
$ docker pull mono@sha256:5e278a7db6df0921e79edb66f3b8e003ed5f52ce22d92d5b136c9335c0e4ee54
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.6 MB (203586535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46e892e7d33e34077a9b4bdb2c52fbcf8deef23676b0575d4044fdbf538c24a0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:21:09 GMT
ADD file:85a8af105e3fa794598824266068cbb3c0dc66067e10e3263dab26a230458a82 in / 
# Tue, 21 Dec 2021 02:21:13 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 05:57:51 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 21 Dec 2021 05:58:36 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 05:59:19 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Dec 2021 06:04:26 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:e2c79f8e0929abda2022fed71e090d3c34c8c3fdfb2a513ede1d117020a46821`  
		Last Modified: Tue, 21 Dec 2021 02:30:19 GMT  
		Size: 30.6 MB (30562311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05689b686c6ec73e139fb223bdb96d0c2b6c18f526d0b74f571436655d64ccf0`  
		Last Modified: Tue, 21 Dec 2021 06:09:40 GMT  
		Size: 2.9 MB (2884483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74174042d484e5cc200c0a2c655bc60ad5dd9d8a165ea4907a443c4d3d7a414b`  
		Last Modified: Tue, 21 Dec 2021 06:09:45 GMT  
		Size: 26.9 MB (26873482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa471d0ae5b7ed38b2a0eb4874ad5ed176dcfdcf01beb5df800c1b0dd70972a1`  
		Last Modified: Tue, 21 Dec 2021 06:10:54 GMT  
		Size: 143.3 MB (143266259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6-slim`

```console
$ docker pull mono@sha256:3f5ae194959692b19773b78bbf549e09fee8409fc396725d26bbadac9780f305
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
$ docker pull mono@sha256:b1f160c4960056a755f78c87acbe28ab65b2090c7ce0beba9a0a347d1b34a168
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94680923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f795cebdb9ba7d4af431453595977d286d08cda538a80f67ad5e72e6901cf51`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:36:49 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 21 Dec 2021 02:37:06 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 02:37:36 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8678af474ab209c6f77514a3e861bb6e382fdd4f519efa3c08708b70676f7714`  
		Last Modified: Tue, 21 Dec 2021 02:52:42 GMT  
		Size: 2.8 MB (2767125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad55ab33cb43c5e91426eb50f5804dfaa25e4ca85d8faef05dc9894b16af2148`  
		Last Modified: Tue, 21 Dec 2021 02:52:54 GMT  
		Size: 64.8 MB (64760075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:8fd140ee635a99dc41c659aa712df53d5388c9a192bb6c8252c822b8b0330f5c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51841847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9367f423c10b12a67b18a20c893f911dd816cfa2cb80d749cb118f1f0e60f534`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:51:32 GMT
ADD file:f757929225218280f26d0eca53387788343e93cc9658f5baeb58957776114579 in / 
# Tue, 21 Dec 2021 01:51:33 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:42:14 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 21 Dec 2021 03:42:48 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 03:43:35 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7d69cd3acec6d9e5ca88bdd718b069a7272b722048f49b6d21fbe85fc6c82560`  
		Last Modified: Tue, 21 Dec 2021 02:07:21 GMT  
		Size: 24.9 MB (24886253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9083493d202e9a9d70bb069d8ede78d5dd4a01013dfed35779a92aca045b93`  
		Last Modified: Tue, 21 Dec 2021 03:53:53 GMT  
		Size: 2.5 MB (2462568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e64cb7f034664931a2081c40c52b36a04cdd979ff44aed8df991b489266dee3`  
		Last Modified: Tue, 21 Dec 2021 03:54:10 GMT  
		Size: 24.5 MB (24493026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:e279f95d27d5df508488a8074e9a28bad0160f467b1abf52c738b7fe072b0dde
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48898971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47000a347fb095bec2f3588b78876eb10e43a5a23e8ddd97bbc685d14857c728`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:00:52 GMT
ADD file:1381e18e2847f24ebd16d8e83ad940adeff45aca2c327d4e07d7451816f29420 in / 
# Tue, 21 Dec 2021 02:00:52 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:50:08 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 21 Dec 2021 07:50:34 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 07:51:18 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b597e1a6bc27aa2a24a587cb687c9551dfbcfa730a11d48c5a44ff77ff6fdd75`  
		Last Modified: Tue, 21 Dec 2021 02:16:50 GMT  
		Size: 22.8 MB (22754324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf6c5f7fad1939cd9be660d18ca40d4402c8e8edb6fccb486497e7f2f7a1f72`  
		Last Modified: Tue, 21 Dec 2021 08:00:51 GMT  
		Size: 2.4 MB (2361910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c45bb2608bc2763ce62f4c08b6d3137040af4b25c52a94abfced92aaf5fee7`  
		Last Modified: Tue, 21 Dec 2021 08:01:08 GMT  
		Size: 23.8 MB (23782737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:abd750b08116c7f7a3a04db0e669d49fcec322ff4724cce81fff8a58c101dec1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57876215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8985e0d0c74bb76657b4366297bf7ef10f1188897831bdbfc65ee14994ea211e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:34 GMT
ADD file:83d9e760a84be2bd8754e31e33b3f782b44f6e7b7e02c156f519715c88c40615 in / 
# Thu, 02 Dec 2021 08:08:35 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 10:31:32 GMT
ENV MONO_VERSION=6.12.0.122
# Thu, 02 Dec 2021 10:31:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 02 Dec 2021 10:32:05 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2a37a2e6ba8cbf21e3950cf7b2455f0af054667b6a35719fb2bd6070973bfa76`  
		Last Modified: Thu, 02 Dec 2021 08:41:37 GMT  
		Size: 25.9 MB (25923144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9881b3a1bbaf2479f58c7e7e0a008ba9dfcfd9a404b8a45f61e67b19f8a2b493`  
		Last Modified: Thu, 02 Dec 2021 10:35:43 GMT  
		Size: 2.6 MB (2634639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a63bac7bf077258f21a6462bb51b790fdfd8c75ff13922648615e0ecd2755c`  
		Last Modified: Thu, 02 Dec 2021 10:35:48 GMT  
		Size: 29.3 MB (29318432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; 386

```console
$ docker pull mono@sha256:9bb720a3e2fe2fac5af3d2868e8f635ab7de67622d1dcb87fcd9622e6e1ca5e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99364470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d552f788d57a0cc6924c3f1df81c6577715d0788660292b50b4f80a15e3d9d6`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:40:25 GMT
ADD file:9063906ecf2b5c82bf37cb574e78f61add2cd7aa8d0675647be379e30e19b6a9 in / 
# Thu, 02 Dec 2021 02:40:25 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 14:55:37 GMT
ENV MONO_VERSION=6.12.0.122
# Thu, 02 Dec 2021 14:55:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 02 Dec 2021 14:56:21 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3b938b4b72623e9d1494d498630cd883df97fd6882fb9e0edb7af6714fce4e83`  
		Last Modified: Thu, 02 Dec 2021 02:49:02 GMT  
		Size: 27.8 MB (27804562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33df0d561cd5f2e983795fefe65289181d4ec840095931cf18b11ff6c7bf28c2`  
		Last Modified: Thu, 02 Dec 2021 15:03:01 GMT  
		Size: 2.8 MB (2781457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2ba8412a0fc14d63cab8249ab154c0f32239599e76bfd072203cc83b8a6bc4`  
		Last Modified: Thu, 02 Dec 2021 15:03:22 GMT  
		Size: 68.8 MB (68778451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:dfb363f2e045a8ebea3ea09a15f42ab726bb6064b71122703eba126a13182a38
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.3 MB (60320276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e809a8a8de0af5f6974c222bdfc2adccc243dda0ef436a6ba480fb4f5edb242`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:21:09 GMT
ADD file:85a8af105e3fa794598824266068cbb3c0dc66067e10e3263dab26a230458a82 in / 
# Tue, 21 Dec 2021 02:21:13 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 05:57:51 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 21 Dec 2021 05:58:36 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 05:59:19 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:e2c79f8e0929abda2022fed71e090d3c34c8c3fdfb2a513ede1d117020a46821`  
		Last Modified: Tue, 21 Dec 2021 02:30:19 GMT  
		Size: 30.6 MB (30562311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05689b686c6ec73e139fb223bdb96d0c2b6c18f526d0b74f571436655d64ccf0`  
		Last Modified: Tue, 21 Dec 2021 06:09:40 GMT  
		Size: 2.9 MB (2884483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74174042d484e5cc200c0a2c655bc60ad5dd9d8a165ea4907a443c4d3d7a414b`  
		Last Modified: Tue, 21 Dec 2021 06:09:45 GMT  
		Size: 26.9 MB (26873482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10`

```console
$ docker pull mono@sha256:fcb033837ec25b6ee9b6ba44f09568a0169ed05b2a17bfbd221afa52f026007d
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
$ docker pull mono@sha256:4039b91d20494d8b4bc4df7a6a68cf45fe4ccd19556839149c792095d3986fde
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.0 MB (224997782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e027fe5fdba3b030c31187f7440372ee71fbb5700049e97f47c20d3c13d8cb95`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:37:47 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 21 Dec 2021 02:38:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 02:38:39 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Dec 2021 02:52:06 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d647a1e0d32e2e824bb3b1b5b4076dcd2199e92758a50c402132bbc505f00b8`  
		Last Modified: Tue, 21 Dec 2021 02:53:11 GMT  
		Size: 2.8 MB (2767086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48be8c05bbd5c6ab6ee4d43271e9ab48effe05dbe074186e31f4887aedd4ab7`  
		Last Modified: Tue, 21 Dec 2021 02:53:23 GMT  
		Size: 64.8 MB (64779430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398b7b38860914ccd2e358759883198374cb595ae1aa0367d3954a11659aef4e`  
		Last Modified: Tue, 21 Dec 2021 02:54:42 GMT  
		Size: 130.3 MB (130297543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; arm variant v5

```console
$ docker pull mono@sha256:c1252997a77c1cfd1e948caaee9276d95013d9a74889323fa294a0edea55609f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.8 MB (180835672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a69fe926479237381ca2b2b0e8a26f09bf276e9003b88943f2309e7725e77a9b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:51:32 GMT
ADD file:f757929225218280f26d0eca53387788343e93cc9658f5baeb58957776114579 in / 
# Tue, 21 Dec 2021 01:51:33 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:43:51 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 21 Dec 2021 03:44:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 03:45:07 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Dec 2021 03:52:20 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7d69cd3acec6d9e5ca88bdd718b069a7272b722048f49b6d21fbe85fc6c82560`  
		Last Modified: Tue, 21 Dec 2021 02:07:21 GMT  
		Size: 24.9 MB (24886253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b10e45599952085eea6c2aa1a83f1889e0b252f50d71b624dba51a4952db575`  
		Last Modified: Tue, 21 Dec 2021 03:54:34 GMT  
		Size: 2.5 MB (2462550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2312eccabb392075e4ae90a62be1ef1aa4a404a6b814c7bdda46b8b58061d18`  
		Last Modified: Tue, 21 Dec 2021 03:54:50 GMT  
		Size: 24.5 MB (24521836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5730be37cf73cdfd07f0f854b6154b5b3483767c1cca478d364d8b7c21a60dd`  
		Last Modified: Tue, 21 Dec 2021 03:58:30 GMT  
		Size: 129.0 MB (128965033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; arm variant v7

```console
$ docker pull mono@sha256:1d27d1945267671c3cf0495003865478b26171d9d5b3d631e84db4d6e37b2010
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.7 MB (176746630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f144e3c4c0538af28f1ffeabee52f0408275b60069ef1cdb12cc719749fa7e5b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:00:52 GMT
ADD file:1381e18e2847f24ebd16d8e83ad940adeff45aca2c327d4e07d7451816f29420 in / 
# Tue, 21 Dec 2021 02:00:52 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:51:34 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 21 Dec 2021 07:52:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 07:52:45 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Dec 2021 07:59:22 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b597e1a6bc27aa2a24a587cb687c9551dfbcfa730a11d48c5a44ff77ff6fdd75`  
		Last Modified: Tue, 21 Dec 2021 02:16:50 GMT  
		Size: 22.8 MB (22754324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a3e37eca37087e1c37e893e04e1d3e4070827d63d589a0f14b41805fbc8bee`  
		Last Modified: Tue, 21 Dec 2021 08:01:33 GMT  
		Size: 2.4 MB (2361906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c654f5074ebd647e1e9beba40fbd9953b9bf4e79d73b62a29c7b34181cd4d940`  
		Last Modified: Tue, 21 Dec 2021 08:01:49 GMT  
		Size: 23.8 MB (23814744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ef4ed79e2b307d12826fc03e9ba5438c1ed0367c5abdcd46fc085a65fccb6a`  
		Last Modified: Tue, 21 Dec 2021 08:05:32 GMT  
		Size: 127.8 MB (127815656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:488e371238f96ae52233d59dbcff4653a8351d83e479f9f4cacb12d65df7075d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.4 MB (203356329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca9ca983da493104199b13d6a3640cdbee1a08f37c1a41d72885d06dcf19db76`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:34 GMT
ADD file:83d9e760a84be2bd8754e31e33b3f782b44f6e7b7e02c156f519715c88c40615 in / 
# Thu, 02 Dec 2021 08:08:35 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 10:32:11 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 02 Dec 2021 10:32:23 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 02 Dec 2021 10:32:39 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 02 Dec 2021 10:35:00 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2a37a2e6ba8cbf21e3950cf7b2455f0af054667b6a35719fb2bd6070973bfa76`  
		Last Modified: Thu, 02 Dec 2021 08:41:37 GMT  
		Size: 25.9 MB (25923144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b221e456ebfbe9b628e3cc14fb58c185038879d3c35cbc9d00f2e7bba74f01ba`  
		Last Modified: Thu, 02 Dec 2021 10:36:07 GMT  
		Size: 2.6 MB (2634648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67c21b62aff9041a8242bc311b01af90cff481b5b09c998f08a958372bb42f1`  
		Last Modified: Thu, 02 Dec 2021 10:36:11 GMT  
		Size: 29.4 MB (29361391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14ec0ea4dd0d1785ae83dd55b0694655813a03b0f96980e50eca4fc4e326faa`  
		Last Modified: Thu, 02 Dec 2021 10:37:30 GMT  
		Size: 145.4 MB (145437146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; 386

```console
$ docker pull mono@sha256:4e1812a74500ad8fc02215dcbcf32f7102b6a1606197e834dc1146c3b0087e6c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.8 MB (230807397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:623d4c86a8b1e26ee42a0c1c39221139674aad308350f844a4be85ad316c0b67`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:40:25 GMT
ADD file:9063906ecf2b5c82bf37cb574e78f61add2cd7aa8d0675647be379e30e19b6a9 in / 
# Thu, 02 Dec 2021 02:40:25 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 14:56:29 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 02 Dec 2021 14:56:48 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 02 Dec 2021 14:57:31 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 02 Dec 2021 15:01:45 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3b938b4b72623e9d1494d498630cd883df97fd6882fb9e0edb7af6714fce4e83`  
		Last Modified: Thu, 02 Dec 2021 02:49:02 GMT  
		Size: 27.8 MB (27804562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a52ba0390c1d164a8a83a0847b99e0feb215cfdef6ed0c1858438cf69a232a2`  
		Last Modified: Thu, 02 Dec 2021 15:03:46 GMT  
		Size: 2.8 MB (2781472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cc9696e302e94355b4311371ba699c68f96855680be077154a524c14dc2bc0`  
		Last Modified: Thu, 02 Dec 2021 15:04:01 GMT  
		Size: 68.8 MB (68808039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8279d764dc51963cbb5f4aa5e2f27d664a46f9c3e0b8717f8dfe580c118a1137`  
		Last Modified: Thu, 02 Dec 2021 15:05:55 GMT  
		Size: 131.4 MB (131413324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; ppc64le

```console
$ docker pull mono@sha256:b8c7427cb3a3539b27f7d67938724ba50f203bae23ee9b23eed272d970e716d4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.4 MB (192365689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1797036260c43e1d7289c106f5d159fc8efc19cf9a43f26c912cea6c5e51033c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:21:09 GMT
ADD file:85a8af105e3fa794598824266068cbb3c0dc66067e10e3263dab26a230458a82 in / 
# Tue, 21 Dec 2021 02:21:13 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 05:59:32 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 21 Dec 2021 06:00:20 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 06:01:16 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Dec 2021 06:08:56 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:e2c79f8e0929abda2022fed71e090d3c34c8c3fdfb2a513ede1d117020a46821`  
		Last Modified: Tue, 21 Dec 2021 02:30:19 GMT  
		Size: 30.6 MB (30562311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e7d78ad87d12e9b93ae27c2f8390adb1c1d664f5b717e59f24e0fe0fec5566`  
		Last Modified: Tue, 21 Dec 2021 06:10:06 GMT  
		Size: 2.9 MB (2884503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b97bb0a865a43228d2d4b8f07914f43f1f6d87be865c5c8cc4e2f0b96feef8a8`  
		Last Modified: Tue, 21 Dec 2021 06:10:12 GMT  
		Size: 26.9 MB (26917578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d0dec152ff48daaa28be864df4bb991906bb09c587f54d49befdaef541d4b4`  
		Last Modified: Tue, 21 Dec 2021 06:11:40 GMT  
		Size: 132.0 MB (132001297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10-slim`

```console
$ docker pull mono@sha256:aa9855adef03065db8cdf6ba20e8814fe614a0ba0967d6d9e7649c4412c0f7ae
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
$ docker pull mono@sha256:da7b00ef0909ea2f04fbef70db279dae0fd9e30a25d900541c2ab90ee1a24912
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94700239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c5787617281044711602b0633cf9d4912b3797d9726bcaffffe4060a4f9b6d5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:37:47 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 21 Dec 2021 02:38:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 02:38:39 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d647a1e0d32e2e824bb3b1b5b4076dcd2199e92758a50c402132bbc505f00b8`  
		Last Modified: Tue, 21 Dec 2021 02:53:11 GMT  
		Size: 2.8 MB (2767086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48be8c05bbd5c6ab6ee4d43271e9ab48effe05dbe074186e31f4887aedd4ab7`  
		Last Modified: Tue, 21 Dec 2021 02:53:23 GMT  
		Size: 64.8 MB (64779430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:f48bdec256c01bdc5c4d2880dee2f00f4ff0c644ee9ad3652ddfbf06dfb028df
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51870639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d504c56cbe9b2fe34f71faec099b3745455d443e504424b18eb94f189e348cdc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:51:32 GMT
ADD file:f757929225218280f26d0eca53387788343e93cc9658f5baeb58957776114579 in / 
# Tue, 21 Dec 2021 01:51:33 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:43:51 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 21 Dec 2021 03:44:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 03:45:07 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7d69cd3acec6d9e5ca88bdd718b069a7272b722048f49b6d21fbe85fc6c82560`  
		Last Modified: Tue, 21 Dec 2021 02:07:21 GMT  
		Size: 24.9 MB (24886253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b10e45599952085eea6c2aa1a83f1889e0b252f50d71b624dba51a4952db575`  
		Last Modified: Tue, 21 Dec 2021 03:54:34 GMT  
		Size: 2.5 MB (2462550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2312eccabb392075e4ae90a62be1ef1aa4a404a6b814c7bdda46b8b58061d18`  
		Last Modified: Tue, 21 Dec 2021 03:54:50 GMT  
		Size: 24.5 MB (24521836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:f04f82a8388ba1e00351b7a6357e6e0786ee82f17e929061393ac2139c20b7f9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48930974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9cdb8d4c20bcb8b438d9db5f610aa15af6c3f272cd30925bee6f03422e646fa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:00:52 GMT
ADD file:1381e18e2847f24ebd16d8e83ad940adeff45aca2c327d4e07d7451816f29420 in / 
# Tue, 21 Dec 2021 02:00:52 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:51:34 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 21 Dec 2021 07:52:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 07:52:45 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b597e1a6bc27aa2a24a587cb687c9551dfbcfa730a11d48c5a44ff77ff6fdd75`  
		Last Modified: Tue, 21 Dec 2021 02:16:50 GMT  
		Size: 22.8 MB (22754324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a3e37eca37087e1c37e893e04e1d3e4070827d63d589a0f14b41805fbc8bee`  
		Last Modified: Tue, 21 Dec 2021 08:01:33 GMT  
		Size: 2.4 MB (2361906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c654f5074ebd647e1e9beba40fbd9953b9bf4e79d73b62a29c7b34181cd4d940`  
		Last Modified: Tue, 21 Dec 2021 08:01:49 GMT  
		Size: 23.8 MB (23814744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:9f8787b546c22d50b4f55f3c50117233e73cb7c77be37370e29f607db3479c0c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57919183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76dfdf29e3a643b0f29a5475f4fb04c7ee044c020c9cede2e22db91fb8fcc874`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:34 GMT
ADD file:83d9e760a84be2bd8754e31e33b3f782b44f6e7b7e02c156f519715c88c40615 in / 
# Thu, 02 Dec 2021 08:08:35 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 10:32:11 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 02 Dec 2021 10:32:23 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 02 Dec 2021 10:32:39 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2a37a2e6ba8cbf21e3950cf7b2455f0af054667b6a35719fb2bd6070973bfa76`  
		Last Modified: Thu, 02 Dec 2021 08:41:37 GMT  
		Size: 25.9 MB (25923144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b221e456ebfbe9b628e3cc14fb58c185038879d3c35cbc9d00f2e7bba74f01ba`  
		Last Modified: Thu, 02 Dec 2021 10:36:07 GMT  
		Size: 2.6 MB (2634648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67c21b62aff9041a8242bc311b01af90cff481b5b09c998f08a958372bb42f1`  
		Last Modified: Thu, 02 Dec 2021 10:36:11 GMT  
		Size: 29.4 MB (29361391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; 386

```console
$ docker pull mono@sha256:56185f066205d15d3a1d4223963b56b95ccc3465545f6d3c80f30135065e5932
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99394073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5ddeb5db82b2398b359c88b5b275d5ed36a8e1eaacd395c30a36aafe719bf76`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:40:25 GMT
ADD file:9063906ecf2b5c82bf37cb574e78f61add2cd7aa8d0675647be379e30e19b6a9 in / 
# Thu, 02 Dec 2021 02:40:25 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 14:56:29 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 02 Dec 2021 14:56:48 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 02 Dec 2021 14:57:31 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3b938b4b72623e9d1494d498630cd883df97fd6882fb9e0edb7af6714fce4e83`  
		Last Modified: Thu, 02 Dec 2021 02:49:02 GMT  
		Size: 27.8 MB (27804562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a52ba0390c1d164a8a83a0847b99e0feb215cfdef6ed0c1858438cf69a232a2`  
		Last Modified: Thu, 02 Dec 2021 15:03:46 GMT  
		Size: 2.8 MB (2781472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cc9696e302e94355b4311371ba699c68f96855680be077154a524c14dc2bc0`  
		Last Modified: Thu, 02 Dec 2021 15:04:01 GMT  
		Size: 68.8 MB (68808039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:feea4a0e048f7ed593dda7efe7abd914c6b1e5965d512813b2e87dc41bee772c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.4 MB (60364392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac07f80362ff48da2722b992eed44c0d1b6fea9e7eae7d595e7181f07a7b3a4b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:21:09 GMT
ADD file:85a8af105e3fa794598824266068cbb3c0dc66067e10e3263dab26a230458a82 in / 
# Tue, 21 Dec 2021 02:21:13 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 05:59:32 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 21 Dec 2021 06:00:20 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 06:01:16 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:e2c79f8e0929abda2022fed71e090d3c34c8c3fdfb2a513ede1d117020a46821`  
		Last Modified: Tue, 21 Dec 2021 02:30:19 GMT  
		Size: 30.6 MB (30562311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e7d78ad87d12e9b93ae27c2f8390adb1c1d664f5b717e59f24e0fe0fec5566`  
		Last Modified: Tue, 21 Dec 2021 06:10:06 GMT  
		Size: 2.9 MB (2884503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b97bb0a865a43228d2d4b8f07914f43f1f6d87be865c5c8cc4e2f0b96feef8a8`  
		Last Modified: Tue, 21 Dec 2021 06:10:12 GMT  
		Size: 26.9 MB (26917578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10.0`

```console
$ docker pull mono@sha256:fcb033837ec25b6ee9b6ba44f09568a0169ed05b2a17bfbd221afa52f026007d
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
$ docker pull mono@sha256:4039b91d20494d8b4bc4df7a6a68cf45fe4ccd19556839149c792095d3986fde
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.0 MB (224997782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e027fe5fdba3b030c31187f7440372ee71fbb5700049e97f47c20d3c13d8cb95`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:37:47 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 21 Dec 2021 02:38:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 02:38:39 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Dec 2021 02:52:06 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d647a1e0d32e2e824bb3b1b5b4076dcd2199e92758a50c402132bbc505f00b8`  
		Last Modified: Tue, 21 Dec 2021 02:53:11 GMT  
		Size: 2.8 MB (2767086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48be8c05bbd5c6ab6ee4d43271e9ab48effe05dbe074186e31f4887aedd4ab7`  
		Last Modified: Tue, 21 Dec 2021 02:53:23 GMT  
		Size: 64.8 MB (64779430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398b7b38860914ccd2e358759883198374cb595ae1aa0367d3954a11659aef4e`  
		Last Modified: Tue, 21 Dec 2021 02:54:42 GMT  
		Size: 130.3 MB (130297543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; arm variant v5

```console
$ docker pull mono@sha256:c1252997a77c1cfd1e948caaee9276d95013d9a74889323fa294a0edea55609f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.8 MB (180835672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a69fe926479237381ca2b2b0e8a26f09bf276e9003b88943f2309e7725e77a9b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:51:32 GMT
ADD file:f757929225218280f26d0eca53387788343e93cc9658f5baeb58957776114579 in / 
# Tue, 21 Dec 2021 01:51:33 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:43:51 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 21 Dec 2021 03:44:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 03:45:07 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Dec 2021 03:52:20 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7d69cd3acec6d9e5ca88bdd718b069a7272b722048f49b6d21fbe85fc6c82560`  
		Last Modified: Tue, 21 Dec 2021 02:07:21 GMT  
		Size: 24.9 MB (24886253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b10e45599952085eea6c2aa1a83f1889e0b252f50d71b624dba51a4952db575`  
		Last Modified: Tue, 21 Dec 2021 03:54:34 GMT  
		Size: 2.5 MB (2462550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2312eccabb392075e4ae90a62be1ef1aa4a404a6b814c7bdda46b8b58061d18`  
		Last Modified: Tue, 21 Dec 2021 03:54:50 GMT  
		Size: 24.5 MB (24521836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5730be37cf73cdfd07f0f854b6154b5b3483767c1cca478d364d8b7c21a60dd`  
		Last Modified: Tue, 21 Dec 2021 03:58:30 GMT  
		Size: 129.0 MB (128965033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; arm variant v7

```console
$ docker pull mono@sha256:1d27d1945267671c3cf0495003865478b26171d9d5b3d631e84db4d6e37b2010
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.7 MB (176746630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f144e3c4c0538af28f1ffeabee52f0408275b60069ef1cdb12cc719749fa7e5b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:00:52 GMT
ADD file:1381e18e2847f24ebd16d8e83ad940adeff45aca2c327d4e07d7451816f29420 in / 
# Tue, 21 Dec 2021 02:00:52 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:51:34 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 21 Dec 2021 07:52:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 07:52:45 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Dec 2021 07:59:22 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b597e1a6bc27aa2a24a587cb687c9551dfbcfa730a11d48c5a44ff77ff6fdd75`  
		Last Modified: Tue, 21 Dec 2021 02:16:50 GMT  
		Size: 22.8 MB (22754324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a3e37eca37087e1c37e893e04e1d3e4070827d63d589a0f14b41805fbc8bee`  
		Last Modified: Tue, 21 Dec 2021 08:01:33 GMT  
		Size: 2.4 MB (2361906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c654f5074ebd647e1e9beba40fbd9953b9bf4e79d73b62a29c7b34181cd4d940`  
		Last Modified: Tue, 21 Dec 2021 08:01:49 GMT  
		Size: 23.8 MB (23814744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ef4ed79e2b307d12826fc03e9ba5438c1ed0367c5abdcd46fc085a65fccb6a`  
		Last Modified: Tue, 21 Dec 2021 08:05:32 GMT  
		Size: 127.8 MB (127815656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:488e371238f96ae52233d59dbcff4653a8351d83e479f9f4cacb12d65df7075d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.4 MB (203356329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca9ca983da493104199b13d6a3640cdbee1a08f37c1a41d72885d06dcf19db76`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:34 GMT
ADD file:83d9e760a84be2bd8754e31e33b3f782b44f6e7b7e02c156f519715c88c40615 in / 
# Thu, 02 Dec 2021 08:08:35 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 10:32:11 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 02 Dec 2021 10:32:23 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 02 Dec 2021 10:32:39 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 02 Dec 2021 10:35:00 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2a37a2e6ba8cbf21e3950cf7b2455f0af054667b6a35719fb2bd6070973bfa76`  
		Last Modified: Thu, 02 Dec 2021 08:41:37 GMT  
		Size: 25.9 MB (25923144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b221e456ebfbe9b628e3cc14fb58c185038879d3c35cbc9d00f2e7bba74f01ba`  
		Last Modified: Thu, 02 Dec 2021 10:36:07 GMT  
		Size: 2.6 MB (2634648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67c21b62aff9041a8242bc311b01af90cff481b5b09c998f08a958372bb42f1`  
		Last Modified: Thu, 02 Dec 2021 10:36:11 GMT  
		Size: 29.4 MB (29361391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14ec0ea4dd0d1785ae83dd55b0694655813a03b0f96980e50eca4fc4e326faa`  
		Last Modified: Thu, 02 Dec 2021 10:37:30 GMT  
		Size: 145.4 MB (145437146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; 386

```console
$ docker pull mono@sha256:4e1812a74500ad8fc02215dcbcf32f7102b6a1606197e834dc1146c3b0087e6c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.8 MB (230807397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:623d4c86a8b1e26ee42a0c1c39221139674aad308350f844a4be85ad316c0b67`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:40:25 GMT
ADD file:9063906ecf2b5c82bf37cb574e78f61add2cd7aa8d0675647be379e30e19b6a9 in / 
# Thu, 02 Dec 2021 02:40:25 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 14:56:29 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 02 Dec 2021 14:56:48 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 02 Dec 2021 14:57:31 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 02 Dec 2021 15:01:45 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3b938b4b72623e9d1494d498630cd883df97fd6882fb9e0edb7af6714fce4e83`  
		Last Modified: Thu, 02 Dec 2021 02:49:02 GMT  
		Size: 27.8 MB (27804562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a52ba0390c1d164a8a83a0847b99e0feb215cfdef6ed0c1858438cf69a232a2`  
		Last Modified: Thu, 02 Dec 2021 15:03:46 GMT  
		Size: 2.8 MB (2781472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cc9696e302e94355b4311371ba699c68f96855680be077154a524c14dc2bc0`  
		Last Modified: Thu, 02 Dec 2021 15:04:01 GMT  
		Size: 68.8 MB (68808039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8279d764dc51963cbb5f4aa5e2f27d664a46f9c3e0b8717f8dfe580c118a1137`  
		Last Modified: Thu, 02 Dec 2021 15:05:55 GMT  
		Size: 131.4 MB (131413324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; ppc64le

```console
$ docker pull mono@sha256:b8c7427cb3a3539b27f7d67938724ba50f203bae23ee9b23eed272d970e716d4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.4 MB (192365689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1797036260c43e1d7289c106f5d159fc8efc19cf9a43f26c912cea6c5e51033c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:21:09 GMT
ADD file:85a8af105e3fa794598824266068cbb3c0dc66067e10e3263dab26a230458a82 in / 
# Tue, 21 Dec 2021 02:21:13 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 05:59:32 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 21 Dec 2021 06:00:20 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 06:01:16 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Dec 2021 06:08:56 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:e2c79f8e0929abda2022fed71e090d3c34c8c3fdfb2a513ede1d117020a46821`  
		Last Modified: Tue, 21 Dec 2021 02:30:19 GMT  
		Size: 30.6 MB (30562311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e7d78ad87d12e9b93ae27c2f8390adb1c1d664f5b717e59f24e0fe0fec5566`  
		Last Modified: Tue, 21 Dec 2021 06:10:06 GMT  
		Size: 2.9 MB (2884503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b97bb0a865a43228d2d4b8f07914f43f1f6d87be865c5c8cc4e2f0b96feef8a8`  
		Last Modified: Tue, 21 Dec 2021 06:10:12 GMT  
		Size: 26.9 MB (26917578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d0dec152ff48daaa28be864df4bb991906bb09c587f54d49befdaef541d4b4`  
		Last Modified: Tue, 21 Dec 2021 06:11:40 GMT  
		Size: 132.0 MB (132001297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10.0-slim`

```console
$ docker pull mono@sha256:aa9855adef03065db8cdf6ba20e8814fe614a0ba0967d6d9e7649c4412c0f7ae
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
$ docker pull mono@sha256:da7b00ef0909ea2f04fbef70db279dae0fd9e30a25d900541c2ab90ee1a24912
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94700239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c5787617281044711602b0633cf9d4912b3797d9726bcaffffe4060a4f9b6d5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:37:47 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 21 Dec 2021 02:38:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 02:38:39 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d647a1e0d32e2e824bb3b1b5b4076dcd2199e92758a50c402132bbc505f00b8`  
		Last Modified: Tue, 21 Dec 2021 02:53:11 GMT  
		Size: 2.8 MB (2767086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48be8c05bbd5c6ab6ee4d43271e9ab48effe05dbe074186e31f4887aedd4ab7`  
		Last Modified: Tue, 21 Dec 2021 02:53:23 GMT  
		Size: 64.8 MB (64779430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:f48bdec256c01bdc5c4d2880dee2f00f4ff0c644ee9ad3652ddfbf06dfb028df
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51870639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d504c56cbe9b2fe34f71faec099b3745455d443e504424b18eb94f189e348cdc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:51:32 GMT
ADD file:f757929225218280f26d0eca53387788343e93cc9658f5baeb58957776114579 in / 
# Tue, 21 Dec 2021 01:51:33 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:43:51 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 21 Dec 2021 03:44:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 03:45:07 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7d69cd3acec6d9e5ca88bdd718b069a7272b722048f49b6d21fbe85fc6c82560`  
		Last Modified: Tue, 21 Dec 2021 02:07:21 GMT  
		Size: 24.9 MB (24886253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b10e45599952085eea6c2aa1a83f1889e0b252f50d71b624dba51a4952db575`  
		Last Modified: Tue, 21 Dec 2021 03:54:34 GMT  
		Size: 2.5 MB (2462550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2312eccabb392075e4ae90a62be1ef1aa4a404a6b814c7bdda46b8b58061d18`  
		Last Modified: Tue, 21 Dec 2021 03:54:50 GMT  
		Size: 24.5 MB (24521836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:f04f82a8388ba1e00351b7a6357e6e0786ee82f17e929061393ac2139c20b7f9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48930974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9cdb8d4c20bcb8b438d9db5f610aa15af6c3f272cd30925bee6f03422e646fa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:00:52 GMT
ADD file:1381e18e2847f24ebd16d8e83ad940adeff45aca2c327d4e07d7451816f29420 in / 
# Tue, 21 Dec 2021 02:00:52 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:51:34 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 21 Dec 2021 07:52:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 07:52:45 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b597e1a6bc27aa2a24a587cb687c9551dfbcfa730a11d48c5a44ff77ff6fdd75`  
		Last Modified: Tue, 21 Dec 2021 02:16:50 GMT  
		Size: 22.8 MB (22754324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a3e37eca37087e1c37e893e04e1d3e4070827d63d589a0f14b41805fbc8bee`  
		Last Modified: Tue, 21 Dec 2021 08:01:33 GMT  
		Size: 2.4 MB (2361906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c654f5074ebd647e1e9beba40fbd9953b9bf4e79d73b62a29c7b34181cd4d940`  
		Last Modified: Tue, 21 Dec 2021 08:01:49 GMT  
		Size: 23.8 MB (23814744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:9f8787b546c22d50b4f55f3c50117233e73cb7c77be37370e29f607db3479c0c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57919183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76dfdf29e3a643b0f29a5475f4fb04c7ee044c020c9cede2e22db91fb8fcc874`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:34 GMT
ADD file:83d9e760a84be2bd8754e31e33b3f782b44f6e7b7e02c156f519715c88c40615 in / 
# Thu, 02 Dec 2021 08:08:35 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 10:32:11 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 02 Dec 2021 10:32:23 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 02 Dec 2021 10:32:39 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2a37a2e6ba8cbf21e3950cf7b2455f0af054667b6a35719fb2bd6070973bfa76`  
		Last Modified: Thu, 02 Dec 2021 08:41:37 GMT  
		Size: 25.9 MB (25923144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b221e456ebfbe9b628e3cc14fb58c185038879d3c35cbc9d00f2e7bba74f01ba`  
		Last Modified: Thu, 02 Dec 2021 10:36:07 GMT  
		Size: 2.6 MB (2634648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67c21b62aff9041a8242bc311b01af90cff481b5b09c998f08a958372bb42f1`  
		Last Modified: Thu, 02 Dec 2021 10:36:11 GMT  
		Size: 29.4 MB (29361391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; 386

```console
$ docker pull mono@sha256:56185f066205d15d3a1d4223963b56b95ccc3465545f6d3c80f30135065e5932
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99394073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5ddeb5db82b2398b359c88b5b275d5ed36a8e1eaacd395c30a36aafe719bf76`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:40:25 GMT
ADD file:9063906ecf2b5c82bf37cb574e78f61add2cd7aa8d0675647be379e30e19b6a9 in / 
# Thu, 02 Dec 2021 02:40:25 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 14:56:29 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 02 Dec 2021 14:56:48 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 02 Dec 2021 14:57:31 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3b938b4b72623e9d1494d498630cd883df97fd6882fb9e0edb7af6714fce4e83`  
		Last Modified: Thu, 02 Dec 2021 02:49:02 GMT  
		Size: 27.8 MB (27804562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a52ba0390c1d164a8a83a0847b99e0feb215cfdef6ed0c1858438cf69a232a2`  
		Last Modified: Thu, 02 Dec 2021 15:03:46 GMT  
		Size: 2.8 MB (2781472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cc9696e302e94355b4311371ba699c68f96855680be077154a524c14dc2bc0`  
		Last Modified: Thu, 02 Dec 2021 15:04:01 GMT  
		Size: 68.8 MB (68808039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:feea4a0e048f7ed593dda7efe7abd914c6b1e5965d512813b2e87dc41bee772c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.4 MB (60364392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac07f80362ff48da2722b992eed44c0d1b6fea9e7eae7d595e7181f07a7b3a4b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:21:09 GMT
ADD file:85a8af105e3fa794598824266068cbb3c0dc66067e10e3263dab26a230458a82 in / 
# Tue, 21 Dec 2021 02:21:13 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 05:59:32 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 21 Dec 2021 06:00:20 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 06:01:16 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:e2c79f8e0929abda2022fed71e090d3c34c8c3fdfb2a513ede1d117020a46821`  
		Last Modified: Tue, 21 Dec 2021 02:30:19 GMT  
		Size: 30.6 MB (30562311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e7d78ad87d12e9b93ae27c2f8390adb1c1d664f5b717e59f24e0fe0fec5566`  
		Last Modified: Tue, 21 Dec 2021 06:10:06 GMT  
		Size: 2.9 MB (2884503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b97bb0a865a43228d2d4b8f07914f43f1f6d87be865c5c8cc4e2f0b96feef8a8`  
		Last Modified: Tue, 21 Dec 2021 06:10:12 GMT  
		Size: 26.9 MB (26917578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10.0.104`

```console
$ docker pull mono@sha256:fcb033837ec25b6ee9b6ba44f09568a0169ed05b2a17bfbd221afa52f026007d
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
$ docker pull mono@sha256:4039b91d20494d8b4bc4df7a6a68cf45fe4ccd19556839149c792095d3986fde
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.0 MB (224997782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e027fe5fdba3b030c31187f7440372ee71fbb5700049e97f47c20d3c13d8cb95`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:37:47 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 21 Dec 2021 02:38:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 02:38:39 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Dec 2021 02:52:06 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d647a1e0d32e2e824bb3b1b5b4076dcd2199e92758a50c402132bbc505f00b8`  
		Last Modified: Tue, 21 Dec 2021 02:53:11 GMT  
		Size: 2.8 MB (2767086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48be8c05bbd5c6ab6ee4d43271e9ab48effe05dbe074186e31f4887aedd4ab7`  
		Last Modified: Tue, 21 Dec 2021 02:53:23 GMT  
		Size: 64.8 MB (64779430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398b7b38860914ccd2e358759883198374cb595ae1aa0367d3954a11659aef4e`  
		Last Modified: Tue, 21 Dec 2021 02:54:42 GMT  
		Size: 130.3 MB (130297543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; arm variant v5

```console
$ docker pull mono@sha256:c1252997a77c1cfd1e948caaee9276d95013d9a74889323fa294a0edea55609f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.8 MB (180835672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a69fe926479237381ca2b2b0e8a26f09bf276e9003b88943f2309e7725e77a9b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:51:32 GMT
ADD file:f757929225218280f26d0eca53387788343e93cc9658f5baeb58957776114579 in / 
# Tue, 21 Dec 2021 01:51:33 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:43:51 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 21 Dec 2021 03:44:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 03:45:07 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Dec 2021 03:52:20 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7d69cd3acec6d9e5ca88bdd718b069a7272b722048f49b6d21fbe85fc6c82560`  
		Last Modified: Tue, 21 Dec 2021 02:07:21 GMT  
		Size: 24.9 MB (24886253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b10e45599952085eea6c2aa1a83f1889e0b252f50d71b624dba51a4952db575`  
		Last Modified: Tue, 21 Dec 2021 03:54:34 GMT  
		Size: 2.5 MB (2462550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2312eccabb392075e4ae90a62be1ef1aa4a404a6b814c7bdda46b8b58061d18`  
		Last Modified: Tue, 21 Dec 2021 03:54:50 GMT  
		Size: 24.5 MB (24521836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5730be37cf73cdfd07f0f854b6154b5b3483767c1cca478d364d8b7c21a60dd`  
		Last Modified: Tue, 21 Dec 2021 03:58:30 GMT  
		Size: 129.0 MB (128965033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; arm variant v7

```console
$ docker pull mono@sha256:1d27d1945267671c3cf0495003865478b26171d9d5b3d631e84db4d6e37b2010
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.7 MB (176746630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f144e3c4c0538af28f1ffeabee52f0408275b60069ef1cdb12cc719749fa7e5b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:00:52 GMT
ADD file:1381e18e2847f24ebd16d8e83ad940adeff45aca2c327d4e07d7451816f29420 in / 
# Tue, 21 Dec 2021 02:00:52 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:51:34 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 21 Dec 2021 07:52:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 07:52:45 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Dec 2021 07:59:22 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b597e1a6bc27aa2a24a587cb687c9551dfbcfa730a11d48c5a44ff77ff6fdd75`  
		Last Modified: Tue, 21 Dec 2021 02:16:50 GMT  
		Size: 22.8 MB (22754324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a3e37eca37087e1c37e893e04e1d3e4070827d63d589a0f14b41805fbc8bee`  
		Last Modified: Tue, 21 Dec 2021 08:01:33 GMT  
		Size: 2.4 MB (2361906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c654f5074ebd647e1e9beba40fbd9953b9bf4e79d73b62a29c7b34181cd4d940`  
		Last Modified: Tue, 21 Dec 2021 08:01:49 GMT  
		Size: 23.8 MB (23814744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ef4ed79e2b307d12826fc03e9ba5438c1ed0367c5abdcd46fc085a65fccb6a`  
		Last Modified: Tue, 21 Dec 2021 08:05:32 GMT  
		Size: 127.8 MB (127815656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:488e371238f96ae52233d59dbcff4653a8351d83e479f9f4cacb12d65df7075d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.4 MB (203356329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca9ca983da493104199b13d6a3640cdbee1a08f37c1a41d72885d06dcf19db76`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:34 GMT
ADD file:83d9e760a84be2bd8754e31e33b3f782b44f6e7b7e02c156f519715c88c40615 in / 
# Thu, 02 Dec 2021 08:08:35 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 10:32:11 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 02 Dec 2021 10:32:23 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 02 Dec 2021 10:32:39 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 02 Dec 2021 10:35:00 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2a37a2e6ba8cbf21e3950cf7b2455f0af054667b6a35719fb2bd6070973bfa76`  
		Last Modified: Thu, 02 Dec 2021 08:41:37 GMT  
		Size: 25.9 MB (25923144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b221e456ebfbe9b628e3cc14fb58c185038879d3c35cbc9d00f2e7bba74f01ba`  
		Last Modified: Thu, 02 Dec 2021 10:36:07 GMT  
		Size: 2.6 MB (2634648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67c21b62aff9041a8242bc311b01af90cff481b5b09c998f08a958372bb42f1`  
		Last Modified: Thu, 02 Dec 2021 10:36:11 GMT  
		Size: 29.4 MB (29361391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14ec0ea4dd0d1785ae83dd55b0694655813a03b0f96980e50eca4fc4e326faa`  
		Last Modified: Thu, 02 Dec 2021 10:37:30 GMT  
		Size: 145.4 MB (145437146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; 386

```console
$ docker pull mono@sha256:4e1812a74500ad8fc02215dcbcf32f7102b6a1606197e834dc1146c3b0087e6c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.8 MB (230807397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:623d4c86a8b1e26ee42a0c1c39221139674aad308350f844a4be85ad316c0b67`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:40:25 GMT
ADD file:9063906ecf2b5c82bf37cb574e78f61add2cd7aa8d0675647be379e30e19b6a9 in / 
# Thu, 02 Dec 2021 02:40:25 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 14:56:29 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 02 Dec 2021 14:56:48 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 02 Dec 2021 14:57:31 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 02 Dec 2021 15:01:45 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3b938b4b72623e9d1494d498630cd883df97fd6882fb9e0edb7af6714fce4e83`  
		Last Modified: Thu, 02 Dec 2021 02:49:02 GMT  
		Size: 27.8 MB (27804562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a52ba0390c1d164a8a83a0847b99e0feb215cfdef6ed0c1858438cf69a232a2`  
		Last Modified: Thu, 02 Dec 2021 15:03:46 GMT  
		Size: 2.8 MB (2781472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cc9696e302e94355b4311371ba699c68f96855680be077154a524c14dc2bc0`  
		Last Modified: Thu, 02 Dec 2021 15:04:01 GMT  
		Size: 68.8 MB (68808039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8279d764dc51963cbb5f4aa5e2f27d664a46f9c3e0b8717f8dfe580c118a1137`  
		Last Modified: Thu, 02 Dec 2021 15:05:55 GMT  
		Size: 131.4 MB (131413324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; ppc64le

```console
$ docker pull mono@sha256:b8c7427cb3a3539b27f7d67938724ba50f203bae23ee9b23eed272d970e716d4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.4 MB (192365689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1797036260c43e1d7289c106f5d159fc8efc19cf9a43f26c912cea6c5e51033c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:21:09 GMT
ADD file:85a8af105e3fa794598824266068cbb3c0dc66067e10e3263dab26a230458a82 in / 
# Tue, 21 Dec 2021 02:21:13 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 05:59:32 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 21 Dec 2021 06:00:20 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 06:01:16 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Dec 2021 06:08:56 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:e2c79f8e0929abda2022fed71e090d3c34c8c3fdfb2a513ede1d117020a46821`  
		Last Modified: Tue, 21 Dec 2021 02:30:19 GMT  
		Size: 30.6 MB (30562311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e7d78ad87d12e9b93ae27c2f8390adb1c1d664f5b717e59f24e0fe0fec5566`  
		Last Modified: Tue, 21 Dec 2021 06:10:06 GMT  
		Size: 2.9 MB (2884503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b97bb0a865a43228d2d4b8f07914f43f1f6d87be865c5c8cc4e2f0b96feef8a8`  
		Last Modified: Tue, 21 Dec 2021 06:10:12 GMT  
		Size: 26.9 MB (26917578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d0dec152ff48daaa28be864df4bb991906bb09c587f54d49befdaef541d4b4`  
		Last Modified: Tue, 21 Dec 2021 06:11:40 GMT  
		Size: 132.0 MB (132001297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10.0.104-slim`

```console
$ docker pull mono@sha256:aa9855adef03065db8cdf6ba20e8814fe614a0ba0967d6d9e7649c4412c0f7ae
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
$ docker pull mono@sha256:da7b00ef0909ea2f04fbef70db279dae0fd9e30a25d900541c2ab90ee1a24912
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94700239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c5787617281044711602b0633cf9d4912b3797d9726bcaffffe4060a4f9b6d5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:37:47 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 21 Dec 2021 02:38:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 02:38:39 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d647a1e0d32e2e824bb3b1b5b4076dcd2199e92758a50c402132bbc505f00b8`  
		Last Modified: Tue, 21 Dec 2021 02:53:11 GMT  
		Size: 2.8 MB (2767086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48be8c05bbd5c6ab6ee4d43271e9ab48effe05dbe074186e31f4887aedd4ab7`  
		Last Modified: Tue, 21 Dec 2021 02:53:23 GMT  
		Size: 64.8 MB (64779430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:f48bdec256c01bdc5c4d2880dee2f00f4ff0c644ee9ad3652ddfbf06dfb028df
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51870639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d504c56cbe9b2fe34f71faec099b3745455d443e504424b18eb94f189e348cdc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:51:32 GMT
ADD file:f757929225218280f26d0eca53387788343e93cc9658f5baeb58957776114579 in / 
# Tue, 21 Dec 2021 01:51:33 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:43:51 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 21 Dec 2021 03:44:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 03:45:07 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7d69cd3acec6d9e5ca88bdd718b069a7272b722048f49b6d21fbe85fc6c82560`  
		Last Modified: Tue, 21 Dec 2021 02:07:21 GMT  
		Size: 24.9 MB (24886253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b10e45599952085eea6c2aa1a83f1889e0b252f50d71b624dba51a4952db575`  
		Last Modified: Tue, 21 Dec 2021 03:54:34 GMT  
		Size: 2.5 MB (2462550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2312eccabb392075e4ae90a62be1ef1aa4a404a6b814c7bdda46b8b58061d18`  
		Last Modified: Tue, 21 Dec 2021 03:54:50 GMT  
		Size: 24.5 MB (24521836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:f04f82a8388ba1e00351b7a6357e6e0786ee82f17e929061393ac2139c20b7f9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48930974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9cdb8d4c20bcb8b438d9db5f610aa15af6c3f272cd30925bee6f03422e646fa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:00:52 GMT
ADD file:1381e18e2847f24ebd16d8e83ad940adeff45aca2c327d4e07d7451816f29420 in / 
# Tue, 21 Dec 2021 02:00:52 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:51:34 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 21 Dec 2021 07:52:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 07:52:45 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b597e1a6bc27aa2a24a587cb687c9551dfbcfa730a11d48c5a44ff77ff6fdd75`  
		Last Modified: Tue, 21 Dec 2021 02:16:50 GMT  
		Size: 22.8 MB (22754324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a3e37eca37087e1c37e893e04e1d3e4070827d63d589a0f14b41805fbc8bee`  
		Last Modified: Tue, 21 Dec 2021 08:01:33 GMT  
		Size: 2.4 MB (2361906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c654f5074ebd647e1e9beba40fbd9953b9bf4e79d73b62a29c7b34181cd4d940`  
		Last Modified: Tue, 21 Dec 2021 08:01:49 GMT  
		Size: 23.8 MB (23814744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:9f8787b546c22d50b4f55f3c50117233e73cb7c77be37370e29f607db3479c0c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57919183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76dfdf29e3a643b0f29a5475f4fb04c7ee044c020c9cede2e22db91fb8fcc874`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:34 GMT
ADD file:83d9e760a84be2bd8754e31e33b3f782b44f6e7b7e02c156f519715c88c40615 in / 
# Thu, 02 Dec 2021 08:08:35 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 10:32:11 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 02 Dec 2021 10:32:23 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 02 Dec 2021 10:32:39 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2a37a2e6ba8cbf21e3950cf7b2455f0af054667b6a35719fb2bd6070973bfa76`  
		Last Modified: Thu, 02 Dec 2021 08:41:37 GMT  
		Size: 25.9 MB (25923144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b221e456ebfbe9b628e3cc14fb58c185038879d3c35cbc9d00f2e7bba74f01ba`  
		Last Modified: Thu, 02 Dec 2021 10:36:07 GMT  
		Size: 2.6 MB (2634648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67c21b62aff9041a8242bc311b01af90cff481b5b09c998f08a958372bb42f1`  
		Last Modified: Thu, 02 Dec 2021 10:36:11 GMT  
		Size: 29.4 MB (29361391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; 386

```console
$ docker pull mono@sha256:56185f066205d15d3a1d4223963b56b95ccc3465545f6d3c80f30135065e5932
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99394073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5ddeb5db82b2398b359c88b5b275d5ed36a8e1eaacd395c30a36aafe719bf76`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:40:25 GMT
ADD file:9063906ecf2b5c82bf37cb574e78f61add2cd7aa8d0675647be379e30e19b6a9 in / 
# Thu, 02 Dec 2021 02:40:25 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 14:56:29 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 02 Dec 2021 14:56:48 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 02 Dec 2021 14:57:31 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3b938b4b72623e9d1494d498630cd883df97fd6882fb9e0edb7af6714fce4e83`  
		Last Modified: Thu, 02 Dec 2021 02:49:02 GMT  
		Size: 27.8 MB (27804562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a52ba0390c1d164a8a83a0847b99e0feb215cfdef6ed0c1858438cf69a232a2`  
		Last Modified: Thu, 02 Dec 2021 15:03:46 GMT  
		Size: 2.8 MB (2781472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cc9696e302e94355b4311371ba699c68f96855680be077154a524c14dc2bc0`  
		Last Modified: Thu, 02 Dec 2021 15:04:01 GMT  
		Size: 68.8 MB (68808039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:feea4a0e048f7ed593dda7efe7abd914c6b1e5965d512813b2e87dc41bee772c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.4 MB (60364392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac07f80362ff48da2722b992eed44c0d1b6fea9e7eae7d595e7181f07a7b3a4b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:21:09 GMT
ADD file:85a8af105e3fa794598824266068cbb3c0dc66067e10e3263dab26a230458a82 in / 
# Tue, 21 Dec 2021 02:21:13 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 05:59:32 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 21 Dec 2021 06:00:20 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 06:01:16 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:e2c79f8e0929abda2022fed71e090d3c34c8c3fdfb2a513ede1d117020a46821`  
		Last Modified: Tue, 21 Dec 2021 02:30:19 GMT  
		Size: 30.6 MB (30562311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e7d78ad87d12e9b93ae27c2f8390adb1c1d664f5b717e59f24e0fe0fec5566`  
		Last Modified: Tue, 21 Dec 2021 06:10:06 GMT  
		Size: 2.9 MB (2884503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b97bb0a865a43228d2d4b8f07914f43f1f6d87be865c5c8cc4e2f0b96feef8a8`  
		Last Modified: Tue, 21 Dec 2021 06:10:12 GMT  
		Size: 26.9 MB (26917578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.12`

```console
$ docker pull mono@sha256:7391b3078f74b4fb71bfe3540c5390a5eed4b3811d965657f051968938e478c0
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
$ docker pull mono@sha256:436da53a1faac7a43322ebac255c97669f9f56d8b85613c47a8c62d603bfb451
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.1 MB (236118822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0363bd6b4181844fc0fe64cf89aaf499c064fe28e5df53518b050d9582253514`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:36:49 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 21 Dec 2021 02:37:06 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 02:37:36 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Dec 2021 02:45:08 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8678af474ab209c6f77514a3e861bb6e382fdd4f519efa3c08708b70676f7714`  
		Last Modified: Tue, 21 Dec 2021 02:52:42 GMT  
		Size: 2.8 MB (2767125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad55ab33cb43c5e91426eb50f5804dfaa25e4ca85d8faef05dc9894b16af2148`  
		Last Modified: Tue, 21 Dec 2021 02:52:54 GMT  
		Size: 64.8 MB (64760075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ec649bf9968b1e1c72798fc1e41260bbc80435ee4ce1e0592b19aa56ecf3ca`  
		Last Modified: Tue, 21 Dec 2021 02:54:01 GMT  
		Size: 141.4 MB (141437899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12` - linux; arm variant v5

```console
$ docker pull mono@sha256:7ac5ca79c9b5e75e4e0f3bfe2b9aa70bbff7732fe99d94d54071cf51caad9585
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.9 MB (191928318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c3e96fe01b11bc7320ba93f00f68f0af7a7964d5a09d6d25b69b4382a131c93`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:51:32 GMT
ADD file:f757929225218280f26d0eca53387788343e93cc9658f5baeb58957776114579 in / 
# Tue, 21 Dec 2021 01:51:33 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:42:14 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 21 Dec 2021 03:42:48 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 03:43:35 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Dec 2021 03:48:47 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7d69cd3acec6d9e5ca88bdd718b069a7272b722048f49b6d21fbe85fc6c82560`  
		Last Modified: Tue, 21 Dec 2021 02:07:21 GMT  
		Size: 24.9 MB (24886253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9083493d202e9a9d70bb069d8ede78d5dd4a01013dfed35779a92aca045b93`  
		Last Modified: Tue, 21 Dec 2021 03:53:53 GMT  
		Size: 2.5 MB (2462568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e64cb7f034664931a2081c40c52b36a04cdd979ff44aed8df991b489266dee3`  
		Last Modified: Tue, 21 Dec 2021 03:54:10 GMT  
		Size: 24.5 MB (24493026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603e8451b8054b91d675124edf960b8e9d6a04dfb2a167c5cd5c38d670d9d189`  
		Last Modified: Tue, 21 Dec 2021 03:56:37 GMT  
		Size: 140.1 MB (140086471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12` - linux; arm variant v7

```console
$ docker pull mono@sha256:42b8007b66564f9e1805b9cb16262788769a0d6178bc017943cb67f1cdd09852
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.8 MB (187845357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84f0965a3989be17ac2e2777a90aa48d8dbdea4842f795d0ca25bd9732b91c7d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:00:52 GMT
ADD file:1381e18e2847f24ebd16d8e83ad940adeff45aca2c327d4e07d7451816f29420 in / 
# Tue, 21 Dec 2021 02:00:52 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:50:08 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 21 Dec 2021 07:50:34 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 07:51:18 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Dec 2021 07:55:58 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b597e1a6bc27aa2a24a587cb687c9551dfbcfa730a11d48c5a44ff77ff6fdd75`  
		Last Modified: Tue, 21 Dec 2021 02:16:50 GMT  
		Size: 22.8 MB (22754324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf6c5f7fad1939cd9be660d18ca40d4402c8e8edb6fccb486497e7f2f7a1f72`  
		Last Modified: Tue, 21 Dec 2021 08:00:51 GMT  
		Size: 2.4 MB (2361910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c45bb2608bc2763ce62f4c08b6d3137040af4b25c52a94abfced92aaf5fee7`  
		Last Modified: Tue, 21 Dec 2021 08:01:08 GMT  
		Size: 23.8 MB (23782737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846af906bfa50c717b3f4340504b8a39511f1709951019c319d941be991cb57a`  
		Last Modified: Tue, 21 Dec 2021 08:03:41 GMT  
		Size: 138.9 MB (138946386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:9329630412680f37b655e8d0a47c1d9b3dbe3c4e1371f3c28e7279666bc6cd6f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.5 MB (214451374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11180fb2db08adf228b4d3709468115b2d40d66b874ccac4ed9a041d5e10b827`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:34 GMT
ADD file:83d9e760a84be2bd8754e31e33b3f782b44f6e7b7e02c156f519715c88c40615 in / 
# Thu, 02 Dec 2021 08:08:35 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 10:31:32 GMT
ENV MONO_VERSION=6.12.0.122
# Thu, 02 Dec 2021 10:31:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 02 Dec 2021 10:32:05 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 02 Dec 2021 10:33:50 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2a37a2e6ba8cbf21e3950cf7b2455f0af054667b6a35719fb2bd6070973bfa76`  
		Last Modified: Thu, 02 Dec 2021 08:41:37 GMT  
		Size: 25.9 MB (25923144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9881b3a1bbaf2479f58c7e7e0a008ba9dfcfd9a404b8a45f61e67b19f8a2b493`  
		Last Modified: Thu, 02 Dec 2021 10:35:43 GMT  
		Size: 2.6 MB (2634639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a63bac7bf077258f21a6462bb51b790fdfd8c75ff13922648615e0ecd2755c`  
		Last Modified: Thu, 02 Dec 2021 10:35:48 GMT  
		Size: 29.3 MB (29318432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:286d86521574d7ba2c433336ba4f2dc6bfe465c5ebf2a9b729361e3811ac1c89`  
		Last Modified: Thu, 02 Dec 2021 10:36:49 GMT  
		Size: 156.6 MB (156575159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12` - linux; 386

```console
$ docker pull mono@sha256:324b2a76dcdbc9e52fc9e54df41809e830f86c065a95a0e154bfe8688fd5b8b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.9 MB (241920513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9820eafdb94e0b17dce68c576278588547a421e7817858cd8e62e1ae0c6b482`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:40:25 GMT
ADD file:9063906ecf2b5c82bf37cb574e78f61add2cd7aa8d0675647be379e30e19b6a9 in / 
# Thu, 02 Dec 2021 02:40:25 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 14:55:37 GMT
ENV MONO_VERSION=6.12.0.122
# Thu, 02 Dec 2021 14:55:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 02 Dec 2021 14:56:21 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 02 Dec 2021 14:59:07 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3b938b4b72623e9d1494d498630cd883df97fd6882fb9e0edb7af6714fce4e83`  
		Last Modified: Thu, 02 Dec 2021 02:49:02 GMT  
		Size: 27.8 MB (27804562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33df0d561cd5f2e983795fefe65289181d4ec840095931cf18b11ff6c7bf28c2`  
		Last Modified: Thu, 02 Dec 2021 15:03:01 GMT  
		Size: 2.8 MB (2781457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2ba8412a0fc14d63cab8249ab154c0f32239599e76bfd072203cc83b8a6bc4`  
		Last Modified: Thu, 02 Dec 2021 15:03:22 GMT  
		Size: 68.8 MB (68778451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4de88484565bfcbf695bf90edb1ba6a692de60b55362f113e5f5894e535ca95f`  
		Last Modified: Thu, 02 Dec 2021 15:04:49 GMT  
		Size: 142.6 MB (142556043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12` - linux; ppc64le

```console
$ docker pull mono@sha256:5e278a7db6df0921e79edb66f3b8e003ed5f52ce22d92d5b136c9335c0e4ee54
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.6 MB (203586535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46e892e7d33e34077a9b4bdb2c52fbcf8deef23676b0575d4044fdbf538c24a0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:21:09 GMT
ADD file:85a8af105e3fa794598824266068cbb3c0dc66067e10e3263dab26a230458a82 in / 
# Tue, 21 Dec 2021 02:21:13 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 05:57:51 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 21 Dec 2021 05:58:36 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 05:59:19 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Dec 2021 06:04:26 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:e2c79f8e0929abda2022fed71e090d3c34c8c3fdfb2a513ede1d117020a46821`  
		Last Modified: Tue, 21 Dec 2021 02:30:19 GMT  
		Size: 30.6 MB (30562311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05689b686c6ec73e139fb223bdb96d0c2b6c18f526d0b74f571436655d64ccf0`  
		Last Modified: Tue, 21 Dec 2021 06:09:40 GMT  
		Size: 2.9 MB (2884483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74174042d484e5cc200c0a2c655bc60ad5dd9d8a165ea4907a443c4d3d7a414b`  
		Last Modified: Tue, 21 Dec 2021 06:09:45 GMT  
		Size: 26.9 MB (26873482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa471d0ae5b7ed38b2a0eb4874ad5ed176dcfdcf01beb5df800c1b0dd70972a1`  
		Last Modified: Tue, 21 Dec 2021 06:10:54 GMT  
		Size: 143.3 MB (143266259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.12-slim`

```console
$ docker pull mono@sha256:3f5ae194959692b19773b78bbf549e09fee8409fc396725d26bbadac9780f305
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
$ docker pull mono@sha256:b1f160c4960056a755f78c87acbe28ab65b2090c7ce0beba9a0a347d1b34a168
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94680923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f795cebdb9ba7d4af431453595977d286d08cda538a80f67ad5e72e6901cf51`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:36:49 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 21 Dec 2021 02:37:06 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 02:37:36 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8678af474ab209c6f77514a3e861bb6e382fdd4f519efa3c08708b70676f7714`  
		Last Modified: Tue, 21 Dec 2021 02:52:42 GMT  
		Size: 2.8 MB (2767125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad55ab33cb43c5e91426eb50f5804dfaa25e4ca85d8faef05dc9894b16af2148`  
		Last Modified: Tue, 21 Dec 2021 02:52:54 GMT  
		Size: 64.8 MB (64760075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:8fd140ee635a99dc41c659aa712df53d5388c9a192bb6c8252c822b8b0330f5c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51841847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9367f423c10b12a67b18a20c893f911dd816cfa2cb80d749cb118f1f0e60f534`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:51:32 GMT
ADD file:f757929225218280f26d0eca53387788343e93cc9658f5baeb58957776114579 in / 
# Tue, 21 Dec 2021 01:51:33 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:42:14 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 21 Dec 2021 03:42:48 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 03:43:35 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7d69cd3acec6d9e5ca88bdd718b069a7272b722048f49b6d21fbe85fc6c82560`  
		Last Modified: Tue, 21 Dec 2021 02:07:21 GMT  
		Size: 24.9 MB (24886253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9083493d202e9a9d70bb069d8ede78d5dd4a01013dfed35779a92aca045b93`  
		Last Modified: Tue, 21 Dec 2021 03:53:53 GMT  
		Size: 2.5 MB (2462568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e64cb7f034664931a2081c40c52b36a04cdd979ff44aed8df991b489266dee3`  
		Last Modified: Tue, 21 Dec 2021 03:54:10 GMT  
		Size: 24.5 MB (24493026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:e279f95d27d5df508488a8074e9a28bad0160f467b1abf52c738b7fe072b0dde
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48898971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47000a347fb095bec2f3588b78876eb10e43a5a23e8ddd97bbc685d14857c728`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:00:52 GMT
ADD file:1381e18e2847f24ebd16d8e83ad940adeff45aca2c327d4e07d7451816f29420 in / 
# Tue, 21 Dec 2021 02:00:52 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:50:08 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 21 Dec 2021 07:50:34 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 07:51:18 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b597e1a6bc27aa2a24a587cb687c9551dfbcfa730a11d48c5a44ff77ff6fdd75`  
		Last Modified: Tue, 21 Dec 2021 02:16:50 GMT  
		Size: 22.8 MB (22754324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf6c5f7fad1939cd9be660d18ca40d4402c8e8edb6fccb486497e7f2f7a1f72`  
		Last Modified: Tue, 21 Dec 2021 08:00:51 GMT  
		Size: 2.4 MB (2361910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c45bb2608bc2763ce62f4c08b6d3137040af4b25c52a94abfced92aaf5fee7`  
		Last Modified: Tue, 21 Dec 2021 08:01:08 GMT  
		Size: 23.8 MB (23782737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:abd750b08116c7f7a3a04db0e669d49fcec322ff4724cce81fff8a58c101dec1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57876215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8985e0d0c74bb76657b4366297bf7ef10f1188897831bdbfc65ee14994ea211e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:34 GMT
ADD file:83d9e760a84be2bd8754e31e33b3f782b44f6e7b7e02c156f519715c88c40615 in / 
# Thu, 02 Dec 2021 08:08:35 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 10:31:32 GMT
ENV MONO_VERSION=6.12.0.122
# Thu, 02 Dec 2021 10:31:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 02 Dec 2021 10:32:05 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2a37a2e6ba8cbf21e3950cf7b2455f0af054667b6a35719fb2bd6070973bfa76`  
		Last Modified: Thu, 02 Dec 2021 08:41:37 GMT  
		Size: 25.9 MB (25923144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9881b3a1bbaf2479f58c7e7e0a008ba9dfcfd9a404b8a45f61e67b19f8a2b493`  
		Last Modified: Thu, 02 Dec 2021 10:35:43 GMT  
		Size: 2.6 MB (2634639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a63bac7bf077258f21a6462bb51b790fdfd8c75ff13922648615e0ecd2755c`  
		Last Modified: Thu, 02 Dec 2021 10:35:48 GMT  
		Size: 29.3 MB (29318432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12-slim` - linux; 386

```console
$ docker pull mono@sha256:9bb720a3e2fe2fac5af3d2868e8f635ab7de67622d1dcb87fcd9622e6e1ca5e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99364470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d552f788d57a0cc6924c3f1df81c6577715d0788660292b50b4f80a15e3d9d6`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:40:25 GMT
ADD file:9063906ecf2b5c82bf37cb574e78f61add2cd7aa8d0675647be379e30e19b6a9 in / 
# Thu, 02 Dec 2021 02:40:25 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 14:55:37 GMT
ENV MONO_VERSION=6.12.0.122
# Thu, 02 Dec 2021 14:55:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 02 Dec 2021 14:56:21 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3b938b4b72623e9d1494d498630cd883df97fd6882fb9e0edb7af6714fce4e83`  
		Last Modified: Thu, 02 Dec 2021 02:49:02 GMT  
		Size: 27.8 MB (27804562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33df0d561cd5f2e983795fefe65289181d4ec840095931cf18b11ff6c7bf28c2`  
		Last Modified: Thu, 02 Dec 2021 15:03:01 GMT  
		Size: 2.8 MB (2781457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2ba8412a0fc14d63cab8249ab154c0f32239599e76bfd072203cc83b8a6bc4`  
		Last Modified: Thu, 02 Dec 2021 15:03:22 GMT  
		Size: 68.8 MB (68778451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:dfb363f2e045a8ebea3ea09a15f42ab726bb6064b71122703eba126a13182a38
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.3 MB (60320276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e809a8a8de0af5f6974c222bdfc2adccc243dda0ef436a6ba480fb4f5edb242`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:21:09 GMT
ADD file:85a8af105e3fa794598824266068cbb3c0dc66067e10e3263dab26a230458a82 in / 
# Tue, 21 Dec 2021 02:21:13 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 05:57:51 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 21 Dec 2021 05:58:36 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 05:59:19 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:e2c79f8e0929abda2022fed71e090d3c34c8c3fdfb2a513ede1d117020a46821`  
		Last Modified: Tue, 21 Dec 2021 02:30:19 GMT  
		Size: 30.6 MB (30562311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05689b686c6ec73e139fb223bdb96d0c2b6c18f526d0b74f571436655d64ccf0`  
		Last Modified: Tue, 21 Dec 2021 06:09:40 GMT  
		Size: 2.9 MB (2884483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74174042d484e5cc200c0a2c655bc60ad5dd9d8a165ea4907a443c4d3d7a414b`  
		Last Modified: Tue, 21 Dec 2021 06:09:45 GMT  
		Size: 26.9 MB (26873482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.12.0`

```console
$ docker pull mono@sha256:7391b3078f74b4fb71bfe3540c5390a5eed4b3811d965657f051968938e478c0
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
$ docker pull mono@sha256:436da53a1faac7a43322ebac255c97669f9f56d8b85613c47a8c62d603bfb451
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.1 MB (236118822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0363bd6b4181844fc0fe64cf89aaf499c064fe28e5df53518b050d9582253514`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:36:49 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 21 Dec 2021 02:37:06 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 02:37:36 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Dec 2021 02:45:08 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8678af474ab209c6f77514a3e861bb6e382fdd4f519efa3c08708b70676f7714`  
		Last Modified: Tue, 21 Dec 2021 02:52:42 GMT  
		Size: 2.8 MB (2767125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad55ab33cb43c5e91426eb50f5804dfaa25e4ca85d8faef05dc9894b16af2148`  
		Last Modified: Tue, 21 Dec 2021 02:52:54 GMT  
		Size: 64.8 MB (64760075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ec649bf9968b1e1c72798fc1e41260bbc80435ee4ce1e0592b19aa56ecf3ca`  
		Last Modified: Tue, 21 Dec 2021 02:54:01 GMT  
		Size: 141.4 MB (141437899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0` - linux; arm variant v5

```console
$ docker pull mono@sha256:7ac5ca79c9b5e75e4e0f3bfe2b9aa70bbff7732fe99d94d54071cf51caad9585
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.9 MB (191928318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c3e96fe01b11bc7320ba93f00f68f0af7a7964d5a09d6d25b69b4382a131c93`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:51:32 GMT
ADD file:f757929225218280f26d0eca53387788343e93cc9658f5baeb58957776114579 in / 
# Tue, 21 Dec 2021 01:51:33 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:42:14 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 21 Dec 2021 03:42:48 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 03:43:35 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Dec 2021 03:48:47 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7d69cd3acec6d9e5ca88bdd718b069a7272b722048f49b6d21fbe85fc6c82560`  
		Last Modified: Tue, 21 Dec 2021 02:07:21 GMT  
		Size: 24.9 MB (24886253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9083493d202e9a9d70bb069d8ede78d5dd4a01013dfed35779a92aca045b93`  
		Last Modified: Tue, 21 Dec 2021 03:53:53 GMT  
		Size: 2.5 MB (2462568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e64cb7f034664931a2081c40c52b36a04cdd979ff44aed8df991b489266dee3`  
		Last Modified: Tue, 21 Dec 2021 03:54:10 GMT  
		Size: 24.5 MB (24493026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603e8451b8054b91d675124edf960b8e9d6a04dfb2a167c5cd5c38d670d9d189`  
		Last Modified: Tue, 21 Dec 2021 03:56:37 GMT  
		Size: 140.1 MB (140086471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0` - linux; arm variant v7

```console
$ docker pull mono@sha256:42b8007b66564f9e1805b9cb16262788769a0d6178bc017943cb67f1cdd09852
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.8 MB (187845357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84f0965a3989be17ac2e2777a90aa48d8dbdea4842f795d0ca25bd9732b91c7d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:00:52 GMT
ADD file:1381e18e2847f24ebd16d8e83ad940adeff45aca2c327d4e07d7451816f29420 in / 
# Tue, 21 Dec 2021 02:00:52 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:50:08 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 21 Dec 2021 07:50:34 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 07:51:18 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Dec 2021 07:55:58 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b597e1a6bc27aa2a24a587cb687c9551dfbcfa730a11d48c5a44ff77ff6fdd75`  
		Last Modified: Tue, 21 Dec 2021 02:16:50 GMT  
		Size: 22.8 MB (22754324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf6c5f7fad1939cd9be660d18ca40d4402c8e8edb6fccb486497e7f2f7a1f72`  
		Last Modified: Tue, 21 Dec 2021 08:00:51 GMT  
		Size: 2.4 MB (2361910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c45bb2608bc2763ce62f4c08b6d3137040af4b25c52a94abfced92aaf5fee7`  
		Last Modified: Tue, 21 Dec 2021 08:01:08 GMT  
		Size: 23.8 MB (23782737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846af906bfa50c717b3f4340504b8a39511f1709951019c319d941be991cb57a`  
		Last Modified: Tue, 21 Dec 2021 08:03:41 GMT  
		Size: 138.9 MB (138946386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:9329630412680f37b655e8d0a47c1d9b3dbe3c4e1371f3c28e7279666bc6cd6f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.5 MB (214451374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11180fb2db08adf228b4d3709468115b2d40d66b874ccac4ed9a041d5e10b827`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:34 GMT
ADD file:83d9e760a84be2bd8754e31e33b3f782b44f6e7b7e02c156f519715c88c40615 in / 
# Thu, 02 Dec 2021 08:08:35 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 10:31:32 GMT
ENV MONO_VERSION=6.12.0.122
# Thu, 02 Dec 2021 10:31:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 02 Dec 2021 10:32:05 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 02 Dec 2021 10:33:50 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2a37a2e6ba8cbf21e3950cf7b2455f0af054667b6a35719fb2bd6070973bfa76`  
		Last Modified: Thu, 02 Dec 2021 08:41:37 GMT  
		Size: 25.9 MB (25923144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9881b3a1bbaf2479f58c7e7e0a008ba9dfcfd9a404b8a45f61e67b19f8a2b493`  
		Last Modified: Thu, 02 Dec 2021 10:35:43 GMT  
		Size: 2.6 MB (2634639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a63bac7bf077258f21a6462bb51b790fdfd8c75ff13922648615e0ecd2755c`  
		Last Modified: Thu, 02 Dec 2021 10:35:48 GMT  
		Size: 29.3 MB (29318432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:286d86521574d7ba2c433336ba4f2dc6bfe465c5ebf2a9b729361e3811ac1c89`  
		Last Modified: Thu, 02 Dec 2021 10:36:49 GMT  
		Size: 156.6 MB (156575159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0` - linux; 386

```console
$ docker pull mono@sha256:324b2a76dcdbc9e52fc9e54df41809e830f86c065a95a0e154bfe8688fd5b8b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.9 MB (241920513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9820eafdb94e0b17dce68c576278588547a421e7817858cd8e62e1ae0c6b482`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:40:25 GMT
ADD file:9063906ecf2b5c82bf37cb574e78f61add2cd7aa8d0675647be379e30e19b6a9 in / 
# Thu, 02 Dec 2021 02:40:25 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 14:55:37 GMT
ENV MONO_VERSION=6.12.0.122
# Thu, 02 Dec 2021 14:55:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 02 Dec 2021 14:56:21 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 02 Dec 2021 14:59:07 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3b938b4b72623e9d1494d498630cd883df97fd6882fb9e0edb7af6714fce4e83`  
		Last Modified: Thu, 02 Dec 2021 02:49:02 GMT  
		Size: 27.8 MB (27804562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33df0d561cd5f2e983795fefe65289181d4ec840095931cf18b11ff6c7bf28c2`  
		Last Modified: Thu, 02 Dec 2021 15:03:01 GMT  
		Size: 2.8 MB (2781457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2ba8412a0fc14d63cab8249ab154c0f32239599e76bfd072203cc83b8a6bc4`  
		Last Modified: Thu, 02 Dec 2021 15:03:22 GMT  
		Size: 68.8 MB (68778451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4de88484565bfcbf695bf90edb1ba6a692de60b55362f113e5f5894e535ca95f`  
		Last Modified: Thu, 02 Dec 2021 15:04:49 GMT  
		Size: 142.6 MB (142556043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0` - linux; ppc64le

```console
$ docker pull mono@sha256:5e278a7db6df0921e79edb66f3b8e003ed5f52ce22d92d5b136c9335c0e4ee54
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.6 MB (203586535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46e892e7d33e34077a9b4bdb2c52fbcf8deef23676b0575d4044fdbf538c24a0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:21:09 GMT
ADD file:85a8af105e3fa794598824266068cbb3c0dc66067e10e3263dab26a230458a82 in / 
# Tue, 21 Dec 2021 02:21:13 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 05:57:51 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 21 Dec 2021 05:58:36 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 05:59:19 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Dec 2021 06:04:26 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:e2c79f8e0929abda2022fed71e090d3c34c8c3fdfb2a513ede1d117020a46821`  
		Last Modified: Tue, 21 Dec 2021 02:30:19 GMT  
		Size: 30.6 MB (30562311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05689b686c6ec73e139fb223bdb96d0c2b6c18f526d0b74f571436655d64ccf0`  
		Last Modified: Tue, 21 Dec 2021 06:09:40 GMT  
		Size: 2.9 MB (2884483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74174042d484e5cc200c0a2c655bc60ad5dd9d8a165ea4907a443c4d3d7a414b`  
		Last Modified: Tue, 21 Dec 2021 06:09:45 GMT  
		Size: 26.9 MB (26873482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa471d0ae5b7ed38b2a0eb4874ad5ed176dcfdcf01beb5df800c1b0dd70972a1`  
		Last Modified: Tue, 21 Dec 2021 06:10:54 GMT  
		Size: 143.3 MB (143266259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.12.0-slim`

```console
$ docker pull mono@sha256:3f5ae194959692b19773b78bbf549e09fee8409fc396725d26bbadac9780f305
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
$ docker pull mono@sha256:b1f160c4960056a755f78c87acbe28ab65b2090c7ce0beba9a0a347d1b34a168
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94680923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f795cebdb9ba7d4af431453595977d286d08cda538a80f67ad5e72e6901cf51`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:36:49 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 21 Dec 2021 02:37:06 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 02:37:36 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8678af474ab209c6f77514a3e861bb6e382fdd4f519efa3c08708b70676f7714`  
		Last Modified: Tue, 21 Dec 2021 02:52:42 GMT  
		Size: 2.8 MB (2767125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad55ab33cb43c5e91426eb50f5804dfaa25e4ca85d8faef05dc9894b16af2148`  
		Last Modified: Tue, 21 Dec 2021 02:52:54 GMT  
		Size: 64.8 MB (64760075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:8fd140ee635a99dc41c659aa712df53d5388c9a192bb6c8252c822b8b0330f5c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51841847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9367f423c10b12a67b18a20c893f911dd816cfa2cb80d749cb118f1f0e60f534`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:51:32 GMT
ADD file:f757929225218280f26d0eca53387788343e93cc9658f5baeb58957776114579 in / 
# Tue, 21 Dec 2021 01:51:33 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:42:14 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 21 Dec 2021 03:42:48 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 03:43:35 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7d69cd3acec6d9e5ca88bdd718b069a7272b722048f49b6d21fbe85fc6c82560`  
		Last Modified: Tue, 21 Dec 2021 02:07:21 GMT  
		Size: 24.9 MB (24886253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9083493d202e9a9d70bb069d8ede78d5dd4a01013dfed35779a92aca045b93`  
		Last Modified: Tue, 21 Dec 2021 03:53:53 GMT  
		Size: 2.5 MB (2462568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e64cb7f034664931a2081c40c52b36a04cdd979ff44aed8df991b489266dee3`  
		Last Modified: Tue, 21 Dec 2021 03:54:10 GMT  
		Size: 24.5 MB (24493026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:e279f95d27d5df508488a8074e9a28bad0160f467b1abf52c738b7fe072b0dde
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48898971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47000a347fb095bec2f3588b78876eb10e43a5a23e8ddd97bbc685d14857c728`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:00:52 GMT
ADD file:1381e18e2847f24ebd16d8e83ad940adeff45aca2c327d4e07d7451816f29420 in / 
# Tue, 21 Dec 2021 02:00:52 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:50:08 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 21 Dec 2021 07:50:34 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 07:51:18 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b597e1a6bc27aa2a24a587cb687c9551dfbcfa730a11d48c5a44ff77ff6fdd75`  
		Last Modified: Tue, 21 Dec 2021 02:16:50 GMT  
		Size: 22.8 MB (22754324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf6c5f7fad1939cd9be660d18ca40d4402c8e8edb6fccb486497e7f2f7a1f72`  
		Last Modified: Tue, 21 Dec 2021 08:00:51 GMT  
		Size: 2.4 MB (2361910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c45bb2608bc2763ce62f4c08b6d3137040af4b25c52a94abfced92aaf5fee7`  
		Last Modified: Tue, 21 Dec 2021 08:01:08 GMT  
		Size: 23.8 MB (23782737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:abd750b08116c7f7a3a04db0e669d49fcec322ff4724cce81fff8a58c101dec1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57876215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8985e0d0c74bb76657b4366297bf7ef10f1188897831bdbfc65ee14994ea211e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:34 GMT
ADD file:83d9e760a84be2bd8754e31e33b3f782b44f6e7b7e02c156f519715c88c40615 in / 
# Thu, 02 Dec 2021 08:08:35 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 10:31:32 GMT
ENV MONO_VERSION=6.12.0.122
# Thu, 02 Dec 2021 10:31:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 02 Dec 2021 10:32:05 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2a37a2e6ba8cbf21e3950cf7b2455f0af054667b6a35719fb2bd6070973bfa76`  
		Last Modified: Thu, 02 Dec 2021 08:41:37 GMT  
		Size: 25.9 MB (25923144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9881b3a1bbaf2479f58c7e7e0a008ba9dfcfd9a404b8a45f61e67b19f8a2b493`  
		Last Modified: Thu, 02 Dec 2021 10:35:43 GMT  
		Size: 2.6 MB (2634639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a63bac7bf077258f21a6462bb51b790fdfd8c75ff13922648615e0ecd2755c`  
		Last Modified: Thu, 02 Dec 2021 10:35:48 GMT  
		Size: 29.3 MB (29318432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0-slim` - linux; 386

```console
$ docker pull mono@sha256:9bb720a3e2fe2fac5af3d2868e8f635ab7de67622d1dcb87fcd9622e6e1ca5e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99364470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d552f788d57a0cc6924c3f1df81c6577715d0788660292b50b4f80a15e3d9d6`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:40:25 GMT
ADD file:9063906ecf2b5c82bf37cb574e78f61add2cd7aa8d0675647be379e30e19b6a9 in / 
# Thu, 02 Dec 2021 02:40:25 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 14:55:37 GMT
ENV MONO_VERSION=6.12.0.122
# Thu, 02 Dec 2021 14:55:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 02 Dec 2021 14:56:21 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3b938b4b72623e9d1494d498630cd883df97fd6882fb9e0edb7af6714fce4e83`  
		Last Modified: Thu, 02 Dec 2021 02:49:02 GMT  
		Size: 27.8 MB (27804562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33df0d561cd5f2e983795fefe65289181d4ec840095931cf18b11ff6c7bf28c2`  
		Last Modified: Thu, 02 Dec 2021 15:03:01 GMT  
		Size: 2.8 MB (2781457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2ba8412a0fc14d63cab8249ab154c0f32239599e76bfd072203cc83b8a6bc4`  
		Last Modified: Thu, 02 Dec 2021 15:03:22 GMT  
		Size: 68.8 MB (68778451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:dfb363f2e045a8ebea3ea09a15f42ab726bb6064b71122703eba126a13182a38
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.3 MB (60320276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e809a8a8de0af5f6974c222bdfc2adccc243dda0ef436a6ba480fb4f5edb242`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:21:09 GMT
ADD file:85a8af105e3fa794598824266068cbb3c0dc66067e10e3263dab26a230458a82 in / 
# Tue, 21 Dec 2021 02:21:13 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 05:57:51 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 21 Dec 2021 05:58:36 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 05:59:19 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:e2c79f8e0929abda2022fed71e090d3c34c8c3fdfb2a513ede1d117020a46821`  
		Last Modified: Tue, 21 Dec 2021 02:30:19 GMT  
		Size: 30.6 MB (30562311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05689b686c6ec73e139fb223bdb96d0c2b6c18f526d0b74f571436655d64ccf0`  
		Last Modified: Tue, 21 Dec 2021 06:09:40 GMT  
		Size: 2.9 MB (2884483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74174042d484e5cc200c0a2c655bc60ad5dd9d8a165ea4907a443c4d3d7a414b`  
		Last Modified: Tue, 21 Dec 2021 06:09:45 GMT  
		Size: 26.9 MB (26873482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.12.0.122`

```console
$ docker pull mono@sha256:7391b3078f74b4fb71bfe3540c5390a5eed4b3811d965657f051968938e478c0
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
$ docker pull mono@sha256:436da53a1faac7a43322ebac255c97669f9f56d8b85613c47a8c62d603bfb451
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.1 MB (236118822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0363bd6b4181844fc0fe64cf89aaf499c064fe28e5df53518b050d9582253514`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:36:49 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 21 Dec 2021 02:37:06 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 02:37:36 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Dec 2021 02:45:08 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8678af474ab209c6f77514a3e861bb6e382fdd4f519efa3c08708b70676f7714`  
		Last Modified: Tue, 21 Dec 2021 02:52:42 GMT  
		Size: 2.8 MB (2767125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad55ab33cb43c5e91426eb50f5804dfaa25e4ca85d8faef05dc9894b16af2148`  
		Last Modified: Tue, 21 Dec 2021 02:52:54 GMT  
		Size: 64.8 MB (64760075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ec649bf9968b1e1c72798fc1e41260bbc80435ee4ce1e0592b19aa56ecf3ca`  
		Last Modified: Tue, 21 Dec 2021 02:54:01 GMT  
		Size: 141.4 MB (141437899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.122` - linux; arm variant v5

```console
$ docker pull mono@sha256:7ac5ca79c9b5e75e4e0f3bfe2b9aa70bbff7732fe99d94d54071cf51caad9585
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.9 MB (191928318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c3e96fe01b11bc7320ba93f00f68f0af7a7964d5a09d6d25b69b4382a131c93`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:51:32 GMT
ADD file:f757929225218280f26d0eca53387788343e93cc9658f5baeb58957776114579 in / 
# Tue, 21 Dec 2021 01:51:33 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:42:14 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 21 Dec 2021 03:42:48 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 03:43:35 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Dec 2021 03:48:47 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7d69cd3acec6d9e5ca88bdd718b069a7272b722048f49b6d21fbe85fc6c82560`  
		Last Modified: Tue, 21 Dec 2021 02:07:21 GMT  
		Size: 24.9 MB (24886253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9083493d202e9a9d70bb069d8ede78d5dd4a01013dfed35779a92aca045b93`  
		Last Modified: Tue, 21 Dec 2021 03:53:53 GMT  
		Size: 2.5 MB (2462568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e64cb7f034664931a2081c40c52b36a04cdd979ff44aed8df991b489266dee3`  
		Last Modified: Tue, 21 Dec 2021 03:54:10 GMT  
		Size: 24.5 MB (24493026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603e8451b8054b91d675124edf960b8e9d6a04dfb2a167c5cd5c38d670d9d189`  
		Last Modified: Tue, 21 Dec 2021 03:56:37 GMT  
		Size: 140.1 MB (140086471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.122` - linux; arm variant v7

```console
$ docker pull mono@sha256:42b8007b66564f9e1805b9cb16262788769a0d6178bc017943cb67f1cdd09852
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.8 MB (187845357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84f0965a3989be17ac2e2777a90aa48d8dbdea4842f795d0ca25bd9732b91c7d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:00:52 GMT
ADD file:1381e18e2847f24ebd16d8e83ad940adeff45aca2c327d4e07d7451816f29420 in / 
# Tue, 21 Dec 2021 02:00:52 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:50:08 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 21 Dec 2021 07:50:34 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 07:51:18 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Dec 2021 07:55:58 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b597e1a6bc27aa2a24a587cb687c9551dfbcfa730a11d48c5a44ff77ff6fdd75`  
		Last Modified: Tue, 21 Dec 2021 02:16:50 GMT  
		Size: 22.8 MB (22754324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf6c5f7fad1939cd9be660d18ca40d4402c8e8edb6fccb486497e7f2f7a1f72`  
		Last Modified: Tue, 21 Dec 2021 08:00:51 GMT  
		Size: 2.4 MB (2361910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c45bb2608bc2763ce62f4c08b6d3137040af4b25c52a94abfced92aaf5fee7`  
		Last Modified: Tue, 21 Dec 2021 08:01:08 GMT  
		Size: 23.8 MB (23782737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846af906bfa50c717b3f4340504b8a39511f1709951019c319d941be991cb57a`  
		Last Modified: Tue, 21 Dec 2021 08:03:41 GMT  
		Size: 138.9 MB (138946386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.122` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:9329630412680f37b655e8d0a47c1d9b3dbe3c4e1371f3c28e7279666bc6cd6f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.5 MB (214451374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11180fb2db08adf228b4d3709468115b2d40d66b874ccac4ed9a041d5e10b827`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:34 GMT
ADD file:83d9e760a84be2bd8754e31e33b3f782b44f6e7b7e02c156f519715c88c40615 in / 
# Thu, 02 Dec 2021 08:08:35 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 10:31:32 GMT
ENV MONO_VERSION=6.12.0.122
# Thu, 02 Dec 2021 10:31:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 02 Dec 2021 10:32:05 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 02 Dec 2021 10:33:50 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2a37a2e6ba8cbf21e3950cf7b2455f0af054667b6a35719fb2bd6070973bfa76`  
		Last Modified: Thu, 02 Dec 2021 08:41:37 GMT  
		Size: 25.9 MB (25923144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9881b3a1bbaf2479f58c7e7e0a008ba9dfcfd9a404b8a45f61e67b19f8a2b493`  
		Last Modified: Thu, 02 Dec 2021 10:35:43 GMT  
		Size: 2.6 MB (2634639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a63bac7bf077258f21a6462bb51b790fdfd8c75ff13922648615e0ecd2755c`  
		Last Modified: Thu, 02 Dec 2021 10:35:48 GMT  
		Size: 29.3 MB (29318432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:286d86521574d7ba2c433336ba4f2dc6bfe465c5ebf2a9b729361e3811ac1c89`  
		Last Modified: Thu, 02 Dec 2021 10:36:49 GMT  
		Size: 156.6 MB (156575159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.122` - linux; 386

```console
$ docker pull mono@sha256:324b2a76dcdbc9e52fc9e54df41809e830f86c065a95a0e154bfe8688fd5b8b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.9 MB (241920513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9820eafdb94e0b17dce68c576278588547a421e7817858cd8e62e1ae0c6b482`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:40:25 GMT
ADD file:9063906ecf2b5c82bf37cb574e78f61add2cd7aa8d0675647be379e30e19b6a9 in / 
# Thu, 02 Dec 2021 02:40:25 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 14:55:37 GMT
ENV MONO_VERSION=6.12.0.122
# Thu, 02 Dec 2021 14:55:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 02 Dec 2021 14:56:21 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 02 Dec 2021 14:59:07 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3b938b4b72623e9d1494d498630cd883df97fd6882fb9e0edb7af6714fce4e83`  
		Last Modified: Thu, 02 Dec 2021 02:49:02 GMT  
		Size: 27.8 MB (27804562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33df0d561cd5f2e983795fefe65289181d4ec840095931cf18b11ff6c7bf28c2`  
		Last Modified: Thu, 02 Dec 2021 15:03:01 GMT  
		Size: 2.8 MB (2781457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2ba8412a0fc14d63cab8249ab154c0f32239599e76bfd072203cc83b8a6bc4`  
		Last Modified: Thu, 02 Dec 2021 15:03:22 GMT  
		Size: 68.8 MB (68778451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4de88484565bfcbf695bf90edb1ba6a692de60b55362f113e5f5894e535ca95f`  
		Last Modified: Thu, 02 Dec 2021 15:04:49 GMT  
		Size: 142.6 MB (142556043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.122` - linux; ppc64le

```console
$ docker pull mono@sha256:5e278a7db6df0921e79edb66f3b8e003ed5f52ce22d92d5b136c9335c0e4ee54
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.6 MB (203586535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46e892e7d33e34077a9b4bdb2c52fbcf8deef23676b0575d4044fdbf538c24a0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:21:09 GMT
ADD file:85a8af105e3fa794598824266068cbb3c0dc66067e10e3263dab26a230458a82 in / 
# Tue, 21 Dec 2021 02:21:13 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 05:57:51 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 21 Dec 2021 05:58:36 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 05:59:19 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Dec 2021 06:04:26 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:e2c79f8e0929abda2022fed71e090d3c34c8c3fdfb2a513ede1d117020a46821`  
		Last Modified: Tue, 21 Dec 2021 02:30:19 GMT  
		Size: 30.6 MB (30562311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05689b686c6ec73e139fb223bdb96d0c2b6c18f526d0b74f571436655d64ccf0`  
		Last Modified: Tue, 21 Dec 2021 06:09:40 GMT  
		Size: 2.9 MB (2884483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74174042d484e5cc200c0a2c655bc60ad5dd9d8a165ea4907a443c4d3d7a414b`  
		Last Modified: Tue, 21 Dec 2021 06:09:45 GMT  
		Size: 26.9 MB (26873482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa471d0ae5b7ed38b2a0eb4874ad5ed176dcfdcf01beb5df800c1b0dd70972a1`  
		Last Modified: Tue, 21 Dec 2021 06:10:54 GMT  
		Size: 143.3 MB (143266259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.12.0.122-slim`

```console
$ docker pull mono@sha256:3f5ae194959692b19773b78bbf549e09fee8409fc396725d26bbadac9780f305
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
$ docker pull mono@sha256:b1f160c4960056a755f78c87acbe28ab65b2090c7ce0beba9a0a347d1b34a168
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94680923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f795cebdb9ba7d4af431453595977d286d08cda538a80f67ad5e72e6901cf51`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:36:49 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 21 Dec 2021 02:37:06 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 02:37:36 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8678af474ab209c6f77514a3e861bb6e382fdd4f519efa3c08708b70676f7714`  
		Last Modified: Tue, 21 Dec 2021 02:52:42 GMT  
		Size: 2.8 MB (2767125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad55ab33cb43c5e91426eb50f5804dfaa25e4ca85d8faef05dc9894b16af2148`  
		Last Modified: Tue, 21 Dec 2021 02:52:54 GMT  
		Size: 64.8 MB (64760075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.122-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:8fd140ee635a99dc41c659aa712df53d5388c9a192bb6c8252c822b8b0330f5c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51841847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9367f423c10b12a67b18a20c893f911dd816cfa2cb80d749cb118f1f0e60f534`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:51:32 GMT
ADD file:f757929225218280f26d0eca53387788343e93cc9658f5baeb58957776114579 in / 
# Tue, 21 Dec 2021 01:51:33 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:42:14 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 21 Dec 2021 03:42:48 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 03:43:35 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7d69cd3acec6d9e5ca88bdd718b069a7272b722048f49b6d21fbe85fc6c82560`  
		Last Modified: Tue, 21 Dec 2021 02:07:21 GMT  
		Size: 24.9 MB (24886253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9083493d202e9a9d70bb069d8ede78d5dd4a01013dfed35779a92aca045b93`  
		Last Modified: Tue, 21 Dec 2021 03:53:53 GMT  
		Size: 2.5 MB (2462568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e64cb7f034664931a2081c40c52b36a04cdd979ff44aed8df991b489266dee3`  
		Last Modified: Tue, 21 Dec 2021 03:54:10 GMT  
		Size: 24.5 MB (24493026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.122-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:e279f95d27d5df508488a8074e9a28bad0160f467b1abf52c738b7fe072b0dde
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48898971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47000a347fb095bec2f3588b78876eb10e43a5a23e8ddd97bbc685d14857c728`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:00:52 GMT
ADD file:1381e18e2847f24ebd16d8e83ad940adeff45aca2c327d4e07d7451816f29420 in / 
# Tue, 21 Dec 2021 02:00:52 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:50:08 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 21 Dec 2021 07:50:34 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 07:51:18 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b597e1a6bc27aa2a24a587cb687c9551dfbcfa730a11d48c5a44ff77ff6fdd75`  
		Last Modified: Tue, 21 Dec 2021 02:16:50 GMT  
		Size: 22.8 MB (22754324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf6c5f7fad1939cd9be660d18ca40d4402c8e8edb6fccb486497e7f2f7a1f72`  
		Last Modified: Tue, 21 Dec 2021 08:00:51 GMT  
		Size: 2.4 MB (2361910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c45bb2608bc2763ce62f4c08b6d3137040af4b25c52a94abfced92aaf5fee7`  
		Last Modified: Tue, 21 Dec 2021 08:01:08 GMT  
		Size: 23.8 MB (23782737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.122-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:abd750b08116c7f7a3a04db0e669d49fcec322ff4724cce81fff8a58c101dec1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57876215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8985e0d0c74bb76657b4366297bf7ef10f1188897831bdbfc65ee14994ea211e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:34 GMT
ADD file:83d9e760a84be2bd8754e31e33b3f782b44f6e7b7e02c156f519715c88c40615 in / 
# Thu, 02 Dec 2021 08:08:35 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 10:31:32 GMT
ENV MONO_VERSION=6.12.0.122
# Thu, 02 Dec 2021 10:31:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 02 Dec 2021 10:32:05 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2a37a2e6ba8cbf21e3950cf7b2455f0af054667b6a35719fb2bd6070973bfa76`  
		Last Modified: Thu, 02 Dec 2021 08:41:37 GMT  
		Size: 25.9 MB (25923144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9881b3a1bbaf2479f58c7e7e0a008ba9dfcfd9a404b8a45f61e67b19f8a2b493`  
		Last Modified: Thu, 02 Dec 2021 10:35:43 GMT  
		Size: 2.6 MB (2634639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a63bac7bf077258f21a6462bb51b790fdfd8c75ff13922648615e0ecd2755c`  
		Last Modified: Thu, 02 Dec 2021 10:35:48 GMT  
		Size: 29.3 MB (29318432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.122-slim` - linux; 386

```console
$ docker pull mono@sha256:9bb720a3e2fe2fac5af3d2868e8f635ab7de67622d1dcb87fcd9622e6e1ca5e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99364470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d552f788d57a0cc6924c3f1df81c6577715d0788660292b50b4f80a15e3d9d6`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:40:25 GMT
ADD file:9063906ecf2b5c82bf37cb574e78f61add2cd7aa8d0675647be379e30e19b6a9 in / 
# Thu, 02 Dec 2021 02:40:25 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 14:55:37 GMT
ENV MONO_VERSION=6.12.0.122
# Thu, 02 Dec 2021 14:55:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 02 Dec 2021 14:56:21 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3b938b4b72623e9d1494d498630cd883df97fd6882fb9e0edb7af6714fce4e83`  
		Last Modified: Thu, 02 Dec 2021 02:49:02 GMT  
		Size: 27.8 MB (27804562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33df0d561cd5f2e983795fefe65289181d4ec840095931cf18b11ff6c7bf28c2`  
		Last Modified: Thu, 02 Dec 2021 15:03:01 GMT  
		Size: 2.8 MB (2781457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2ba8412a0fc14d63cab8249ab154c0f32239599e76bfd072203cc83b8a6bc4`  
		Last Modified: Thu, 02 Dec 2021 15:03:22 GMT  
		Size: 68.8 MB (68778451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.122-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:dfb363f2e045a8ebea3ea09a15f42ab726bb6064b71122703eba126a13182a38
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.3 MB (60320276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e809a8a8de0af5f6974c222bdfc2adccc243dda0ef436a6ba480fb4f5edb242`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:21:09 GMT
ADD file:85a8af105e3fa794598824266068cbb3c0dc66067e10e3263dab26a230458a82 in / 
# Tue, 21 Dec 2021 02:21:13 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 05:57:51 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 21 Dec 2021 05:58:36 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 05:59:19 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:e2c79f8e0929abda2022fed71e090d3c34c8c3fdfb2a513ede1d117020a46821`  
		Last Modified: Tue, 21 Dec 2021 02:30:19 GMT  
		Size: 30.6 MB (30562311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05689b686c6ec73e139fb223bdb96d0c2b6c18f526d0b74f571436655d64ccf0`  
		Last Modified: Tue, 21 Dec 2021 06:09:40 GMT  
		Size: 2.9 MB (2884483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74174042d484e5cc200c0a2c655bc60ad5dd9d8a165ea4907a443c4d3d7a414b`  
		Last Modified: Tue, 21 Dec 2021 06:09:45 GMT  
		Size: 26.9 MB (26873482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:latest`

```console
$ docker pull mono@sha256:7391b3078f74b4fb71bfe3540c5390a5eed4b3811d965657f051968938e478c0
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
$ docker pull mono@sha256:436da53a1faac7a43322ebac255c97669f9f56d8b85613c47a8c62d603bfb451
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.1 MB (236118822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0363bd6b4181844fc0fe64cf89aaf499c064fe28e5df53518b050d9582253514`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:36:49 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 21 Dec 2021 02:37:06 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 02:37:36 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Dec 2021 02:45:08 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8678af474ab209c6f77514a3e861bb6e382fdd4f519efa3c08708b70676f7714`  
		Last Modified: Tue, 21 Dec 2021 02:52:42 GMT  
		Size: 2.8 MB (2767125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad55ab33cb43c5e91426eb50f5804dfaa25e4ca85d8faef05dc9894b16af2148`  
		Last Modified: Tue, 21 Dec 2021 02:52:54 GMT  
		Size: 64.8 MB (64760075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ec649bf9968b1e1c72798fc1e41260bbc80435ee4ce1e0592b19aa56ecf3ca`  
		Last Modified: Tue, 21 Dec 2021 02:54:01 GMT  
		Size: 141.4 MB (141437899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm variant v5

```console
$ docker pull mono@sha256:7ac5ca79c9b5e75e4e0f3bfe2b9aa70bbff7732fe99d94d54071cf51caad9585
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.9 MB (191928318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c3e96fe01b11bc7320ba93f00f68f0af7a7964d5a09d6d25b69b4382a131c93`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:51:32 GMT
ADD file:f757929225218280f26d0eca53387788343e93cc9658f5baeb58957776114579 in / 
# Tue, 21 Dec 2021 01:51:33 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:42:14 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 21 Dec 2021 03:42:48 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 03:43:35 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Dec 2021 03:48:47 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7d69cd3acec6d9e5ca88bdd718b069a7272b722048f49b6d21fbe85fc6c82560`  
		Last Modified: Tue, 21 Dec 2021 02:07:21 GMT  
		Size: 24.9 MB (24886253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9083493d202e9a9d70bb069d8ede78d5dd4a01013dfed35779a92aca045b93`  
		Last Modified: Tue, 21 Dec 2021 03:53:53 GMT  
		Size: 2.5 MB (2462568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e64cb7f034664931a2081c40c52b36a04cdd979ff44aed8df991b489266dee3`  
		Last Modified: Tue, 21 Dec 2021 03:54:10 GMT  
		Size: 24.5 MB (24493026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603e8451b8054b91d675124edf960b8e9d6a04dfb2a167c5cd5c38d670d9d189`  
		Last Modified: Tue, 21 Dec 2021 03:56:37 GMT  
		Size: 140.1 MB (140086471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm variant v7

```console
$ docker pull mono@sha256:42b8007b66564f9e1805b9cb16262788769a0d6178bc017943cb67f1cdd09852
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.8 MB (187845357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84f0965a3989be17ac2e2777a90aa48d8dbdea4842f795d0ca25bd9732b91c7d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:00:52 GMT
ADD file:1381e18e2847f24ebd16d8e83ad940adeff45aca2c327d4e07d7451816f29420 in / 
# Tue, 21 Dec 2021 02:00:52 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:50:08 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 21 Dec 2021 07:50:34 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 07:51:18 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Dec 2021 07:55:58 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b597e1a6bc27aa2a24a587cb687c9551dfbcfa730a11d48c5a44ff77ff6fdd75`  
		Last Modified: Tue, 21 Dec 2021 02:16:50 GMT  
		Size: 22.8 MB (22754324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf6c5f7fad1939cd9be660d18ca40d4402c8e8edb6fccb486497e7f2f7a1f72`  
		Last Modified: Tue, 21 Dec 2021 08:00:51 GMT  
		Size: 2.4 MB (2361910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c45bb2608bc2763ce62f4c08b6d3137040af4b25c52a94abfced92aaf5fee7`  
		Last Modified: Tue, 21 Dec 2021 08:01:08 GMT  
		Size: 23.8 MB (23782737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846af906bfa50c717b3f4340504b8a39511f1709951019c319d941be991cb57a`  
		Last Modified: Tue, 21 Dec 2021 08:03:41 GMT  
		Size: 138.9 MB (138946386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:9329630412680f37b655e8d0a47c1d9b3dbe3c4e1371f3c28e7279666bc6cd6f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.5 MB (214451374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11180fb2db08adf228b4d3709468115b2d40d66b874ccac4ed9a041d5e10b827`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:34 GMT
ADD file:83d9e760a84be2bd8754e31e33b3f782b44f6e7b7e02c156f519715c88c40615 in / 
# Thu, 02 Dec 2021 08:08:35 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 10:31:32 GMT
ENV MONO_VERSION=6.12.0.122
# Thu, 02 Dec 2021 10:31:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 02 Dec 2021 10:32:05 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 02 Dec 2021 10:33:50 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2a37a2e6ba8cbf21e3950cf7b2455f0af054667b6a35719fb2bd6070973bfa76`  
		Last Modified: Thu, 02 Dec 2021 08:41:37 GMT  
		Size: 25.9 MB (25923144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9881b3a1bbaf2479f58c7e7e0a008ba9dfcfd9a404b8a45f61e67b19f8a2b493`  
		Last Modified: Thu, 02 Dec 2021 10:35:43 GMT  
		Size: 2.6 MB (2634639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a63bac7bf077258f21a6462bb51b790fdfd8c75ff13922648615e0ecd2755c`  
		Last Modified: Thu, 02 Dec 2021 10:35:48 GMT  
		Size: 29.3 MB (29318432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:286d86521574d7ba2c433336ba4f2dc6bfe465c5ebf2a9b729361e3811ac1c89`  
		Last Modified: Thu, 02 Dec 2021 10:36:49 GMT  
		Size: 156.6 MB (156575159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; 386

```console
$ docker pull mono@sha256:324b2a76dcdbc9e52fc9e54df41809e830f86c065a95a0e154bfe8688fd5b8b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.9 MB (241920513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9820eafdb94e0b17dce68c576278588547a421e7817858cd8e62e1ae0c6b482`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:40:25 GMT
ADD file:9063906ecf2b5c82bf37cb574e78f61add2cd7aa8d0675647be379e30e19b6a9 in / 
# Thu, 02 Dec 2021 02:40:25 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 14:55:37 GMT
ENV MONO_VERSION=6.12.0.122
# Thu, 02 Dec 2021 14:55:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 02 Dec 2021 14:56:21 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 02 Dec 2021 14:59:07 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3b938b4b72623e9d1494d498630cd883df97fd6882fb9e0edb7af6714fce4e83`  
		Last Modified: Thu, 02 Dec 2021 02:49:02 GMT  
		Size: 27.8 MB (27804562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33df0d561cd5f2e983795fefe65289181d4ec840095931cf18b11ff6c7bf28c2`  
		Last Modified: Thu, 02 Dec 2021 15:03:01 GMT  
		Size: 2.8 MB (2781457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2ba8412a0fc14d63cab8249ab154c0f32239599e76bfd072203cc83b8a6bc4`  
		Last Modified: Thu, 02 Dec 2021 15:03:22 GMT  
		Size: 68.8 MB (68778451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4de88484565bfcbf695bf90edb1ba6a692de60b55362f113e5f5894e535ca95f`  
		Last Modified: Thu, 02 Dec 2021 15:04:49 GMT  
		Size: 142.6 MB (142556043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; ppc64le

```console
$ docker pull mono@sha256:5e278a7db6df0921e79edb66f3b8e003ed5f52ce22d92d5b136c9335c0e4ee54
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.6 MB (203586535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46e892e7d33e34077a9b4bdb2c52fbcf8deef23676b0575d4044fdbf538c24a0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:21:09 GMT
ADD file:85a8af105e3fa794598824266068cbb3c0dc66067e10e3263dab26a230458a82 in / 
# Tue, 21 Dec 2021 02:21:13 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 05:57:51 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 21 Dec 2021 05:58:36 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 05:59:19 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Dec 2021 06:04:26 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:e2c79f8e0929abda2022fed71e090d3c34c8c3fdfb2a513ede1d117020a46821`  
		Last Modified: Tue, 21 Dec 2021 02:30:19 GMT  
		Size: 30.6 MB (30562311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05689b686c6ec73e139fb223bdb96d0c2b6c18f526d0b74f571436655d64ccf0`  
		Last Modified: Tue, 21 Dec 2021 06:09:40 GMT  
		Size: 2.9 MB (2884483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74174042d484e5cc200c0a2c655bc60ad5dd9d8a165ea4907a443c4d3d7a414b`  
		Last Modified: Tue, 21 Dec 2021 06:09:45 GMT  
		Size: 26.9 MB (26873482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa471d0ae5b7ed38b2a0eb4874ad5ed176dcfdcf01beb5df800c1b0dd70972a1`  
		Last Modified: Tue, 21 Dec 2021 06:10:54 GMT  
		Size: 143.3 MB (143266259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:slim`

```console
$ docker pull mono@sha256:3f5ae194959692b19773b78bbf549e09fee8409fc396725d26bbadac9780f305
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
$ docker pull mono@sha256:b1f160c4960056a755f78c87acbe28ab65b2090c7ce0beba9a0a347d1b34a168
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94680923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f795cebdb9ba7d4af431453595977d286d08cda538a80f67ad5e72e6901cf51`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:36:49 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 21 Dec 2021 02:37:06 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 02:37:36 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8678af474ab209c6f77514a3e861bb6e382fdd4f519efa3c08708b70676f7714`  
		Last Modified: Tue, 21 Dec 2021 02:52:42 GMT  
		Size: 2.8 MB (2767125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad55ab33cb43c5e91426eb50f5804dfaa25e4ca85d8faef05dc9894b16af2148`  
		Last Modified: Tue, 21 Dec 2021 02:52:54 GMT  
		Size: 64.8 MB (64760075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:8fd140ee635a99dc41c659aa712df53d5388c9a192bb6c8252c822b8b0330f5c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51841847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9367f423c10b12a67b18a20c893f911dd816cfa2cb80d749cb118f1f0e60f534`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:51:32 GMT
ADD file:f757929225218280f26d0eca53387788343e93cc9658f5baeb58957776114579 in / 
# Tue, 21 Dec 2021 01:51:33 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:42:14 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 21 Dec 2021 03:42:48 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 03:43:35 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7d69cd3acec6d9e5ca88bdd718b069a7272b722048f49b6d21fbe85fc6c82560`  
		Last Modified: Tue, 21 Dec 2021 02:07:21 GMT  
		Size: 24.9 MB (24886253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9083493d202e9a9d70bb069d8ede78d5dd4a01013dfed35779a92aca045b93`  
		Last Modified: Tue, 21 Dec 2021 03:53:53 GMT  
		Size: 2.5 MB (2462568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e64cb7f034664931a2081c40c52b36a04cdd979ff44aed8df991b489266dee3`  
		Last Modified: Tue, 21 Dec 2021 03:54:10 GMT  
		Size: 24.5 MB (24493026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:e279f95d27d5df508488a8074e9a28bad0160f467b1abf52c738b7fe072b0dde
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48898971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47000a347fb095bec2f3588b78876eb10e43a5a23e8ddd97bbc685d14857c728`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:00:52 GMT
ADD file:1381e18e2847f24ebd16d8e83ad940adeff45aca2c327d4e07d7451816f29420 in / 
# Tue, 21 Dec 2021 02:00:52 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:50:08 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 21 Dec 2021 07:50:34 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 07:51:18 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b597e1a6bc27aa2a24a587cb687c9551dfbcfa730a11d48c5a44ff77ff6fdd75`  
		Last Modified: Tue, 21 Dec 2021 02:16:50 GMT  
		Size: 22.8 MB (22754324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf6c5f7fad1939cd9be660d18ca40d4402c8e8edb6fccb486497e7f2f7a1f72`  
		Last Modified: Tue, 21 Dec 2021 08:00:51 GMT  
		Size: 2.4 MB (2361910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c45bb2608bc2763ce62f4c08b6d3137040af4b25c52a94abfced92aaf5fee7`  
		Last Modified: Tue, 21 Dec 2021 08:01:08 GMT  
		Size: 23.8 MB (23782737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:abd750b08116c7f7a3a04db0e669d49fcec322ff4724cce81fff8a58c101dec1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57876215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8985e0d0c74bb76657b4366297bf7ef10f1188897831bdbfc65ee14994ea211e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:34 GMT
ADD file:83d9e760a84be2bd8754e31e33b3f782b44f6e7b7e02c156f519715c88c40615 in / 
# Thu, 02 Dec 2021 08:08:35 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 10:31:32 GMT
ENV MONO_VERSION=6.12.0.122
# Thu, 02 Dec 2021 10:31:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 02 Dec 2021 10:32:05 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2a37a2e6ba8cbf21e3950cf7b2455f0af054667b6a35719fb2bd6070973bfa76`  
		Last Modified: Thu, 02 Dec 2021 08:41:37 GMT  
		Size: 25.9 MB (25923144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9881b3a1bbaf2479f58c7e7e0a008ba9dfcfd9a404b8a45f61e67b19f8a2b493`  
		Last Modified: Thu, 02 Dec 2021 10:35:43 GMT  
		Size: 2.6 MB (2634639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a63bac7bf077258f21a6462bb51b790fdfd8c75ff13922648615e0ecd2755c`  
		Last Modified: Thu, 02 Dec 2021 10:35:48 GMT  
		Size: 29.3 MB (29318432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; 386

```console
$ docker pull mono@sha256:9bb720a3e2fe2fac5af3d2868e8f635ab7de67622d1dcb87fcd9622e6e1ca5e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99364470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d552f788d57a0cc6924c3f1df81c6577715d0788660292b50b4f80a15e3d9d6`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:40:25 GMT
ADD file:9063906ecf2b5c82bf37cb574e78f61add2cd7aa8d0675647be379e30e19b6a9 in / 
# Thu, 02 Dec 2021 02:40:25 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 14:55:37 GMT
ENV MONO_VERSION=6.12.0.122
# Thu, 02 Dec 2021 14:55:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 02 Dec 2021 14:56:21 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3b938b4b72623e9d1494d498630cd883df97fd6882fb9e0edb7af6714fce4e83`  
		Last Modified: Thu, 02 Dec 2021 02:49:02 GMT  
		Size: 27.8 MB (27804562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33df0d561cd5f2e983795fefe65289181d4ec840095931cf18b11ff6c7bf28c2`  
		Last Modified: Thu, 02 Dec 2021 15:03:01 GMT  
		Size: 2.8 MB (2781457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2ba8412a0fc14d63cab8249ab154c0f32239599e76bfd072203cc83b8a6bc4`  
		Last Modified: Thu, 02 Dec 2021 15:03:22 GMT  
		Size: 68.8 MB (68778451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; ppc64le

```console
$ docker pull mono@sha256:dfb363f2e045a8ebea3ea09a15f42ab726bb6064b71122703eba126a13182a38
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.3 MB (60320276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e809a8a8de0af5f6974c222bdfc2adccc243dda0ef436a6ba480fb4f5edb242`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:21:09 GMT
ADD file:85a8af105e3fa794598824266068cbb3c0dc66067e10e3263dab26a230458a82 in / 
# Tue, 21 Dec 2021 02:21:13 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 05:57:51 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 21 Dec 2021 05:58:36 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Dec 2021 05:59:19 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:e2c79f8e0929abda2022fed71e090d3c34c8c3fdfb2a513ede1d117020a46821`  
		Last Modified: Tue, 21 Dec 2021 02:30:19 GMT  
		Size: 30.6 MB (30562311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05689b686c6ec73e139fb223bdb96d0c2b6c18f526d0b74f571436655d64ccf0`  
		Last Modified: Tue, 21 Dec 2021 06:09:40 GMT  
		Size: 2.9 MB (2884483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74174042d484e5cc200c0a2c655bc60ad5dd9d8a165ea4907a443c4d3d7a414b`  
		Last Modified: Tue, 21 Dec 2021 06:09:45 GMT  
		Size: 26.9 MB (26873482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
