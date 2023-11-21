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
-	[`mono:6.12.0.182`](#mono6120182)
-	[`mono:6.12.0.182-slim`](#mono6120182-slim)
-	[`mono:latest`](#monolatest)
-	[`mono:slim`](#monoslim)

## `mono:6`

```console
$ docker pull mono@sha256:4abe0c2a97bd2cbd2a9ae115a02e685c54f7beab3ecd69532a33ea87f975c579
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
$ docker pull mono@sha256:d4b666878534b77724463e1a48ca0ed272f4ef2e4e57898dfd811089cf5b4c64
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.7 MB (254675607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf33e8f095a74d2e08dbd1cf9dab91f0e023164ed4b29cbcd15e83ea70a08b27`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:33 GMT
ADD file:29d3eb64d192a97184f2aa169407b58e969b06268c6372b49eefb72bcadb6e99 in / 
# Wed, 01 Nov 2023 00:21:34 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 05:01:16 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 01 Nov 2023 05:01:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Nov 2023 05:01:52 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 01 Nov 2023 05:04:26 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:113c6ad4754853f4a2ae632cff7d90eba9145cca0bd6fa4d60aa432bd26be6c7`  
		Last Modified: Wed, 01 Nov 2023 00:26:56 GMT  
		Size: 27.2 MB (27187422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018432e3f09706360a65c7c08b2f2e1997ee3e264599f9ee23b8ae9320814895`  
		Last Modified: Wed, 01 Nov 2023 05:09:53 GMT  
		Size: 2.8 MB (2780992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a7b7f1fcc5fc6bd617d375dabccb96b0eeecd3c1fc72440733884fa4bdc1503`  
		Last Modified: Wed, 01 Nov 2023 05:10:01 GMT  
		Size: 64.8 MB (64774577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6182d0a19d1676c36f4c3b2b64551e3f963466bf61976f0855369b05cc0b5266`  
		Last Modified: Wed, 01 Nov 2023 05:10:57 GMT  
		Size: 159.9 MB (159932616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; arm variant v5

```console
$ docker pull mono@sha256:dea4d3a6cf8d83cd0b747ac36b0b7a279de919c38227c259e8f0dd933ad99d3d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.9 MB (192868079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52646a30a3e2966b0a92b143b872a725a0eaa3c003a2b6c3030454d2f5f26220`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:49:37 GMT
ADD file:2ed7ca0d45c68b46a10ae186e8a03f98e72cadfeed17105668f53adf14d31e1f in / 
# Tue, 02 Aug 2022 00:49:38 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 07:17:55 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 01 Mar 2023 07:18:17 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Mar 2023 07:18:42 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 01 Mar 2023 07:20:53 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:187ecffbd1e0eae5de6567dff32bd58f28623635657779760c9d9539d6b7cc59`  
		Last Modified: Tue, 02 Aug 2022 00:57:06 GMT  
		Size: 24.9 MB (24889750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6702eef9c7d9ec6ede2c5f9a15a047b314ccc9140f25694f337c0127478bb25b`  
		Last Modified: Wed, 01 Mar 2023 07:23:12 GMT  
		Size: 2.5 MB (2467715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3781ed66d8db4f1e7c7b6323f62af11c65550a10f339ad7c0fb68f9467f8026d`  
		Last Modified: Wed, 01 Mar 2023 07:23:17 GMT  
		Size: 24.5 MB (24503499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f32f45a77bbef0505ff02ad954c1ce25d1cb8f5b668bbd7c73fa538966d0c0b`  
		Last Modified: Wed, 01 Mar 2023 07:24:21 GMT  
		Size: 141.0 MB (141007115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; arm variant v7

```console
$ docker pull mono@sha256:26c6610167b65aa65e842af4393ce1249efd17ef94a7d18e50dac8ec377d49cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.0 MB (189020371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26a526a0911129c09ef96bb6133ec8377df09020139dd8e1a9cfdc10ea46154a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 03:58:22 GMT
ADD file:407ef80699946b8a8560ae436dfc9ca6148067b3012c02b4cb4e54d6d0aca674 in / 
# Tue, 21 Nov 2023 03:58:22 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:14:47 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 21 Nov 2023 08:14:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Nov 2023 08:15:23 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Nov 2023 08:18:03 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d0b016a8027330736e9ca5c23b846a6a9c1eb0a32da6459047c95d22e9544cb7`  
		Last Modified: Tue, 21 Nov 2023 04:03:19 GMT  
		Size: 22.8 MB (22795884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2ab0cc04bbb4f3bd67f5ec694c4008bc3ac663112b267579b7329a492fc8f5`  
		Last Modified: Tue, 21 Nov 2023 08:20:35 GMT  
		Size: 2.4 MB (2370798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d12568a4ad10f5f80b54205380b845267c3ea411300837fe9faa9d56e0d73c4`  
		Last Modified: Tue, 21 Nov 2023 08:20:40 GMT  
		Size: 23.8 MB (23791217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65c029d99d34a3640b09029fcf63907253204fc8737758d0d95e19c924cc1413`  
		Last Modified: Tue, 21 Nov 2023 08:21:33 GMT  
		Size: 140.1 MB (140062472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:dbea7c6015e69ec89dde16e4a20bae61c77f464c82e42e1e21b7970c0344782e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.4 MB (216406658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29846055156fd6a82b9238f73926c1685a42c5d83cd25fa845ef60855b49cd11`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:34 GMT
ADD file:475e94b9a8f65c7cd4d4156af31e83190240ff35d8038f3fa86ad124d4d5d299 in / 
# Tue, 21 Nov 2023 06:27:35 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:50:59 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 21 Nov 2023 08:51:07 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Nov 2023 08:51:26 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Nov 2023 08:52:56 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:78b429e3efdd9f2b163abf0bca6b1462a25b1c5eddc1dd47f5d3445c6413cfa1`  
		Last Modified: Tue, 21 Nov 2023 06:31:45 GMT  
		Size: 26.0 MB (25967796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb5e1161766d0ff99d8c403407e1f624d50aaf500c2caf00c308fa65fd4d1184`  
		Last Modified: Tue, 21 Nov 2023 08:55:09 GMT  
		Size: 2.6 MB (2645901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b10043d7baec43e46ab0e0715597f3d283d2f0a778c399784ae85bd2cadbbe`  
		Last Modified: Tue, 21 Nov 2023 08:55:13 GMT  
		Size: 29.5 MB (29545201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ba77b4c4b8d91f24be23f4fc7919b9d5c36ccca4b44c92f079989544b8095c`  
		Last Modified: Tue, 21 Nov 2023 08:55:58 GMT  
		Size: 158.2 MB (158247760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; 386

```console
$ docker pull mono@sha256:d54444ae4601e0badb94b98065160fc1a920d03f21d1c19d739845940929f88f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.6 MB (259559841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:143d59a7ac07f028ecb6dbebc5cfd6927673b6e0441d44b4317abf0bed0d145a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:39 GMT
ADD file:f016ddd8ef89ed2b1825b3df9abc595f7e774f9a607e3481272e622153b57aaf in / 
# Wed, 01 Nov 2023 00:39:40 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 09:34:07 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 01 Nov 2023 09:34:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Nov 2023 09:34:47 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 01 Nov 2023 09:37:01 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:36a7e611445c645573e630ead3c9d0a62139e195288b4e02b8a4dba6e0118b73`  
		Last Modified: Wed, 01 Nov 2023 00:45:00 GMT  
		Size: 27.8 MB (27846916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd0850558d4dd4cda278293930bdaa50e81cd25ab9eb55d766180c0aa1b1f59`  
		Last Modified: Wed, 01 Nov 2023 09:38:31 GMT  
		Size: 2.8 MB (2792539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cd462825126104e75cad134113d9c3120e9b4740eab8bb07a26b82826b51451`  
		Last Modified: Wed, 01 Nov 2023 09:38:45 GMT  
		Size: 68.8 MB (68800612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c56b1989d422bad3403fc2962148dfbcdf1737a8059c285e5883ce1c40872412`  
		Last Modified: Wed, 01 Nov 2023 09:40:00 GMT  
		Size: 160.1 MB (160119774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; ppc64le

```console
$ docker pull mono@sha256:fbfb5b60906856f25cc0ffb3ed273fa5da089aed24eab6afb049cc150c221768
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.7 MB (221654331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45a10e5a16545c25df57d5cf1f034acbb78fb5a3c968378416dc576fa88386ef`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:04 GMT
ADD file:6d33ba25d3625e5f445fc2183b60c64e2cbc780cb541d7f8ac76ce193b311d13 in / 
# Tue, 02 Aug 2022 01:18:06 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 02:07:46 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 03 Aug 2022 02:08:06 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 03 Aug 2022 02:08:41 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 03 Aug 2022 02:11:40 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:fc8842eebb7ccaf249b2bb2d6a3878fffdae26c9db8f23b393c7f76a6249d2f6`  
		Last Modified: Tue, 02 Aug 2022 01:25:45 GMT  
		Size: 30.6 MB (30560308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1100971c8a3b3eb42c6e22a4c25f405143f007bda60d16697d49b333925b4d84`  
		Last Modified: Wed, 03 Aug 2022 02:15:13 GMT  
		Size: 2.9 MB (2892658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:390f883f1594b5d2d40b7ba4dc50f375439dd1611f38f0c3d071a38bf2ac62cd`  
		Last Modified: Wed, 03 Aug 2022 02:15:27 GMT  
		Size: 41.9 MB (41897345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae94af697c95b6bf75033b813f19ec72f68da49a681d5ce7078753923129147`  
		Last Modified: Wed, 03 Aug 2022 02:16:58 GMT  
		Size: 146.3 MB (146304020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6-slim`

```console
$ docker pull mono@sha256:4ee2372e0eab5a1051a61f031a9d6f540ed74cba380afc523c9b31f20eba3b19
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
$ docker pull mono@sha256:3e33848de2b17f18b2ffbfbb6c62dddff99d8150e2a4ccf699bda9fdf2898f7b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94742991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:217398809241e0b3afff0a94ae94d93b7722c12f15c7abd1e6e1f0760d2203f9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:33 GMT
ADD file:29d3eb64d192a97184f2aa169407b58e969b06268c6372b49eefb72bcadb6e99 in / 
# Wed, 01 Nov 2023 00:21:34 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 05:01:16 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 01 Nov 2023 05:01:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Nov 2023 05:01:52 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:113c6ad4754853f4a2ae632cff7d90eba9145cca0bd6fa4d60aa432bd26be6c7`  
		Last Modified: Wed, 01 Nov 2023 00:26:56 GMT  
		Size: 27.2 MB (27187422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018432e3f09706360a65c7c08b2f2e1997ee3e264599f9ee23b8ae9320814895`  
		Last Modified: Wed, 01 Nov 2023 05:09:53 GMT  
		Size: 2.8 MB (2780992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a7b7f1fcc5fc6bd617d375dabccb96b0eeecd3c1fc72440733884fa4bdc1503`  
		Last Modified: Wed, 01 Nov 2023 05:10:01 GMT  
		Size: 64.8 MB (64774577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:f7c133539fa6a4add7484e9c93bc9b62ec32236d4b619f320c20b3248fb4739a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51860964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe52652f149ceedc89ed0c0f70985fcd898b6cd5cc98aa6f99f9ca06fd83046c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:49:37 GMT
ADD file:2ed7ca0d45c68b46a10ae186e8a03f98e72cadfeed17105668f53adf14d31e1f in / 
# Tue, 02 Aug 2022 00:49:38 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 07:17:55 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 01 Mar 2023 07:18:17 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Mar 2023 07:18:42 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:187ecffbd1e0eae5de6567dff32bd58f28623635657779760c9d9539d6b7cc59`  
		Last Modified: Tue, 02 Aug 2022 00:57:06 GMT  
		Size: 24.9 MB (24889750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6702eef9c7d9ec6ede2c5f9a15a047b314ccc9140f25694f337c0127478bb25b`  
		Last Modified: Wed, 01 Mar 2023 07:23:12 GMT  
		Size: 2.5 MB (2467715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3781ed66d8db4f1e7c7b6323f62af11c65550a10f339ad7c0fb68f9467f8026d`  
		Last Modified: Wed, 01 Mar 2023 07:23:17 GMT  
		Size: 24.5 MB (24503499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:5e8757a56832dbc6da018fcfaadf6ff1b6b658b619904346d79bd6dfa424e13d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48957899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec15648cad0f6cf0b22ae385f4806e7f6381f7740b9a0ff446655344513f454f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 03:58:22 GMT
ADD file:407ef80699946b8a8560ae436dfc9ca6148067b3012c02b4cb4e54d6d0aca674 in / 
# Tue, 21 Nov 2023 03:58:22 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:14:47 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 21 Nov 2023 08:14:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Nov 2023 08:15:23 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d0b016a8027330736e9ca5c23b846a6a9c1eb0a32da6459047c95d22e9544cb7`  
		Last Modified: Tue, 21 Nov 2023 04:03:19 GMT  
		Size: 22.8 MB (22795884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2ab0cc04bbb4f3bd67f5ec694c4008bc3ac663112b267579b7329a492fc8f5`  
		Last Modified: Tue, 21 Nov 2023 08:20:35 GMT  
		Size: 2.4 MB (2370798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d12568a4ad10f5f80b54205380b845267c3ea411300837fe9faa9d56e0d73c4`  
		Last Modified: Tue, 21 Nov 2023 08:20:40 GMT  
		Size: 23.8 MB (23791217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:c213688b7ba872a8b663c3a357748701d05bf4a34f8d8577211b43e19bb5a34f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.2 MB (58158898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:394752f8a02fce0133c215e5d4432e3507157d364fb9a64e5d2cb3f666fc8014`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:34 GMT
ADD file:475e94b9a8f65c7cd4d4156af31e83190240ff35d8038f3fa86ad124d4d5d299 in / 
# Tue, 21 Nov 2023 06:27:35 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:50:59 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 21 Nov 2023 08:51:07 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Nov 2023 08:51:26 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:78b429e3efdd9f2b163abf0bca6b1462a25b1c5eddc1dd47f5d3445c6413cfa1`  
		Last Modified: Tue, 21 Nov 2023 06:31:45 GMT  
		Size: 26.0 MB (25967796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb5e1161766d0ff99d8c403407e1f624d50aaf500c2caf00c308fa65fd4d1184`  
		Last Modified: Tue, 21 Nov 2023 08:55:09 GMT  
		Size: 2.6 MB (2645901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b10043d7baec43e46ab0e0715597f3d283d2f0a778c399784ae85bd2cadbbe`  
		Last Modified: Tue, 21 Nov 2023 08:55:13 GMT  
		Size: 29.5 MB (29545201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; 386

```console
$ docker pull mono@sha256:599faf3f778e3c5527c6b2884f09cdcbb76e8d4141ff225f16bccaf33eb4262e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99440067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9ea66b266996c0a54d4e901d02fb701aec85b8982405cf787fc22eeb621a04d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:39 GMT
ADD file:f016ddd8ef89ed2b1825b3df9abc595f7e774f9a607e3481272e622153b57aaf in / 
# Wed, 01 Nov 2023 00:39:40 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 09:34:07 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 01 Nov 2023 09:34:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Nov 2023 09:34:47 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:36a7e611445c645573e630ead3c9d0a62139e195288b4e02b8a4dba6e0118b73`  
		Last Modified: Wed, 01 Nov 2023 00:45:00 GMT  
		Size: 27.8 MB (27846916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd0850558d4dd4cda278293930bdaa50e81cd25ab9eb55d766180c0aa1b1f59`  
		Last Modified: Wed, 01 Nov 2023 09:38:31 GMT  
		Size: 2.8 MB (2792539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cd462825126104e75cad134113d9c3120e9b4740eab8bb07a26b82826b51451`  
		Last Modified: Wed, 01 Nov 2023 09:38:45 GMT  
		Size: 68.8 MB (68800612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:b83383e51874bbee097571b303be3299c87d7da8c4c6b0f4e067cfaa552ad925
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75350311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c28d9c810a28445dd3b5767c5be8a3a5c5f459f859498e49f59bb419b735510`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:04 GMT
ADD file:6d33ba25d3625e5f445fc2183b60c64e2cbc780cb541d7f8ac76ce193b311d13 in / 
# Tue, 02 Aug 2022 01:18:06 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 02:07:46 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 03 Aug 2022 02:08:06 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 03 Aug 2022 02:08:41 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:fc8842eebb7ccaf249b2bb2d6a3878fffdae26c9db8f23b393c7f76a6249d2f6`  
		Last Modified: Tue, 02 Aug 2022 01:25:45 GMT  
		Size: 30.6 MB (30560308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1100971c8a3b3eb42c6e22a4c25f405143f007bda60d16697d49b333925b4d84`  
		Last Modified: Wed, 03 Aug 2022 02:15:13 GMT  
		Size: 2.9 MB (2892658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:390f883f1594b5d2d40b7ba4dc50f375439dd1611f38f0c3d071a38bf2ac62cd`  
		Last Modified: Wed, 03 Aug 2022 02:15:27 GMT  
		Size: 41.9 MB (41897345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10`

```console
$ docker pull mono@sha256:c61c97c26f6f997de3073d1b33bf9cbbaf2c4e8d678806a30c4358d7edf63693
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
$ docker pull mono@sha256:088544cff1ba3e43115fb989479bd9b429f8cec1b783f47ef0544b72e6982db8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.1 MB (225080049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23d6552d29f3abcbc35457990eb489a9c1a6e33a626212398ebacbf7be2f70c9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:33 GMT
ADD file:29d3eb64d192a97184f2aa169407b58e969b06268c6372b49eefb72bcadb6e99 in / 
# Wed, 01 Nov 2023 00:21:34 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 05:01:57 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 01 Nov 2023 05:02:05 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Nov 2023 05:02:30 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 01 Nov 2023 05:09:36 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:113c6ad4754853f4a2ae632cff7d90eba9145cca0bd6fa4d60aa432bd26be6c7`  
		Last Modified: Wed, 01 Nov 2023 00:26:56 GMT  
		Size: 27.2 MB (27187422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce1bd567401672434bad3cc050dbcca8eb38f5c62353edf0be2511a9c392b2c`  
		Last Modified: Wed, 01 Nov 2023 05:10:16 GMT  
		Size: 2.8 MB (2781004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc889d221e45f4a1537b9fd04532bd1fc2b3b0ae20ce2c3f887dfe02ed969df`  
		Last Modified: Wed, 01 Nov 2023 05:10:24 GMT  
		Size: 64.8 MB (64780530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec75df573a6069093bca81532c42e67e5b9f1cd0e0506e48c2ef7d4afa21c00e`  
		Last Modified: Wed, 01 Nov 2023 05:11:28 GMT  
		Size: 130.3 MB (130331093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; arm variant v5

```console
$ docker pull mono@sha256:5fd28ff75f47e10162fa8359e3457ed77e6a13c9eb64585df39efdf63e70a1a1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.9 MB (180861329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efa9d1dae1421f12f6f7eecf8cfaac5d7da3f6b99f6874365ce2f2f5fc9d9662`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:49:37 GMT
ADD file:2ed7ca0d45c68b46a10ae186e8a03f98e72cadfeed17105668f53adf14d31e1f in / 
# Tue, 02 Aug 2022 00:49:38 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 07:18:54 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 01 Mar 2023 07:19:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Mar 2023 07:19:22 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 01 Mar 2023 07:22:13 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:187ecffbd1e0eae5de6567dff32bd58f28623635657779760c9d9539d6b7cc59`  
		Last Modified: Tue, 02 Aug 2022 00:57:06 GMT  
		Size: 24.9 MB (24889750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb25ee9d7e5ee2ba3d5fe6104206a45f2c5c425365a535e0aaac7bb9bd71034e`  
		Last Modified: Wed, 01 Mar 2023 07:23:36 GMT  
		Size: 2.5 MB (2467730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b5b10e99353e19dd9c56deed1fd46d8ffc3c3eb2ad78b8d36ac029a085764e`  
		Last Modified: Wed, 01 Mar 2023 07:23:40 GMT  
		Size: 24.5 MB (24521836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75576104ae9839169a1957af7269a139e0be7d50d8cef2a4fe4011b528926e18`  
		Last Modified: Wed, 01 Mar 2023 07:25:04 GMT  
		Size: 129.0 MB (128982013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; arm variant v7

```console
$ docker pull mono@sha256:fad5d37b9e7772d99c00cd5a30b156b4502dfc9c3a69b2a7290d1fa1180adafb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.8 MB (176808297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fef433b8708da3b8c109fb467e2269cda8731dc543827e9d32cb52f7b6be799`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 03:58:22 GMT
ADD file:407ef80699946b8a8560ae436dfc9ca6148067b3012c02b4cb4e54d6d0aca674 in / 
# Tue, 21 Nov 2023 03:58:22 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:15:28 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 21 Nov 2023 08:15:37 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Nov 2023 08:16:00 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Nov 2023 08:20:09 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d0b016a8027330736e9ca5c23b846a6a9c1eb0a32da6459047c95d22e9544cb7`  
		Last Modified: Tue, 21 Nov 2023 04:03:19 GMT  
		Size: 22.8 MB (22795884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354a94df70d4e7e46b42c1937a573d21ba53d8ee384e3950ba4177ec7b5442c7`  
		Last Modified: Tue, 21 Nov 2023 08:20:53 GMT  
		Size: 2.4 MB (2370779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9330c159bf0d14284d9e46e04b57428e1471f7e5e84343b8dca26138f52d5a5e`  
		Last Modified: Tue, 21 Nov 2023 08:20:59 GMT  
		Size: 23.8 MB (23816041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8cc10095ce3fe4292acef0ffc63f8cdec520e66aeb8fea215f4a4b734a9ba96`  
		Last Modified: Tue, 21 Nov 2023 08:22:09 GMT  
		Size: 127.8 MB (127825593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:d78448d09a4eeb6a3a47bbc370579bc895b933ddd6a8bccba058af7340382321
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.7 MB (203694658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57f4204153e548f97b1f01a568f568e1173830483f0d086894bd8070e9779b69`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:34 GMT
ADD file:475e94b9a8f65c7cd4d4156af31e83190240ff35d8038f3fa86ad124d4d5d299 in / 
# Tue, 21 Nov 2023 06:27:35 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:51:33 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 21 Nov 2023 08:51:40 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Nov 2023 08:51:59 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Nov 2023 08:54:42 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:78b429e3efdd9f2b163abf0bca6b1462a25b1c5eddc1dd47f5d3445c6413cfa1`  
		Last Modified: Tue, 21 Nov 2023 06:31:45 GMT  
		Size: 26.0 MB (25967796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba61a6960570324786833e88006201960f3b39419902df3c5d72ee859ed1963`  
		Last Modified: Tue, 21 Nov 2023 08:55:27 GMT  
		Size: 2.6 MB (2645887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4dfdc89451aa2b2d34a467dcbb81dea87ba3c921d5535212ff10e6339a11f49`  
		Last Modified: Tue, 21 Nov 2023 08:55:30 GMT  
		Size: 29.6 MB (29575317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45897c882cde9d30f02104690f4c3d38fbbe2a61d9efdbed4a8400996f5fc7d7`  
		Last Modified: Tue, 21 Nov 2023 08:56:29 GMT  
		Size: 145.5 MB (145505658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; 386

```console
$ docker pull mono@sha256:b414eb29727dd814a1446707b990c5f2ae04ca33bd48388d2c6b3abab8918a54
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.9 MB (230903961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4153c0670bf89b1b7b982e398d954f5df80c7aaa90641ff7d3f153fed0e8107b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:39 GMT
ADD file:f016ddd8ef89ed2b1825b3df9abc595f7e774f9a607e3481272e622153b57aaf in / 
# Wed, 01 Nov 2023 00:39:40 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 09:34:55 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 01 Nov 2023 09:35:06 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Nov 2023 09:35:34 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 01 Nov 2023 09:38:12 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:36a7e611445c645573e630ead3c9d0a62139e195288b4e02b8a4dba6e0118b73`  
		Last Modified: Wed, 01 Nov 2023 00:45:00 GMT  
		Size: 27.8 MB (27846916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0121fb994873373d1332a70d7aff083930bda8f4874fa6e98379bf39abd5f3b8`  
		Last Modified: Wed, 01 Nov 2023 09:39:00 GMT  
		Size: 2.8 MB (2792538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f19fd2bd2e7c03f8ebdf16da322ba6e84ebc1029bdf08b25a80ca00e46d68c`  
		Last Modified: Wed, 01 Nov 2023 09:39:14 GMT  
		Size: 68.8 MB (68809985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd68142980e47041e12b1331253de545f54139dad1f3044c4ccf7d293a3f62b3`  
		Last Modified: Wed, 01 Nov 2023 09:40:45 GMT  
		Size: 131.5 MB (131454522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; ppc64le

```console
$ docker pull mono@sha256:6126f0b2219e750b391e2e0d63ac7a2df863d9e2356c43fba06fee0708676038
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **209.7 MB (209715776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e4e952c22c47db9a79c5ca425c7de3d576d719e2042713424b88a3dae8e5129`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:04 GMT
ADD file:6d33ba25d3625e5f445fc2183b60c64e2cbc780cb541d7f8ac76ce193b311d13 in / 
# Tue, 02 Aug 2022 01:18:06 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 02:08:58 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 03 Aug 2022 02:09:16 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 03 Aug 2022 02:09:49 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 03 Aug 2022 02:14:18 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:fc8842eebb7ccaf249b2bb2d6a3878fffdae26c9db8f23b393c7f76a6249d2f6`  
		Last Modified: Tue, 02 Aug 2022 01:25:45 GMT  
		Size: 30.6 MB (30560308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0b96bc274eefbc8d34a02735b6f704f29aaf7e6c4095edb588a74c1ffb2825`  
		Last Modified: Wed, 03 Aug 2022 02:15:49 GMT  
		Size: 2.9 MB (2892610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f103eac188d225f1b73fa0b0d6a3f2560c7fc46d7ec0f0e7e7a07330eb1ff0`  
		Last Modified: Wed, 03 Aug 2022 02:16:04 GMT  
		Size: 41.8 MB (41839360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a64f5c66cdaf23afe83539fd8177bddc2e783d6ca6ee6eb3cabd08a6a5c375`  
		Last Modified: Wed, 03 Aug 2022 02:17:54 GMT  
		Size: 134.4 MB (134423498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10-slim`

```console
$ docker pull mono@sha256:e0db64c5bcfeb8be85eab1732dca2c1feef667b8e4585057565d8389bf4f0ec5
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
$ docker pull mono@sha256:1abb60d3f90dfb5db58253226fff17b5826a8b0506e63a99e4be9803a088946e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94748956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8367d629ccfdb27d24cb1141138c6ff1c74ba6f524f18e67870a48c962f480d5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:33 GMT
ADD file:29d3eb64d192a97184f2aa169407b58e969b06268c6372b49eefb72bcadb6e99 in / 
# Wed, 01 Nov 2023 00:21:34 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 05:01:57 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 01 Nov 2023 05:02:05 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Nov 2023 05:02:30 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:113c6ad4754853f4a2ae632cff7d90eba9145cca0bd6fa4d60aa432bd26be6c7`  
		Last Modified: Wed, 01 Nov 2023 00:26:56 GMT  
		Size: 27.2 MB (27187422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce1bd567401672434bad3cc050dbcca8eb38f5c62353edf0be2511a9c392b2c`  
		Last Modified: Wed, 01 Nov 2023 05:10:16 GMT  
		Size: 2.8 MB (2781004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc889d221e45f4a1537b9fd04532bd1fc2b3b0ae20ce2c3f887dfe02ed969df`  
		Last Modified: Wed, 01 Nov 2023 05:10:24 GMT  
		Size: 64.8 MB (64780530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:9d52e2f9db76c24f9964eec255de917d7a05b180e6e45f98545846b130400ab6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51879316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccac5ddbcee195ea38a9828f45d157f2ef674624fb9a6a2d5529fc2f8e6b736a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:49:37 GMT
ADD file:2ed7ca0d45c68b46a10ae186e8a03f98e72cadfeed17105668f53adf14d31e1f in / 
# Tue, 02 Aug 2022 00:49:38 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 07:18:54 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 01 Mar 2023 07:19:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Mar 2023 07:19:22 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:187ecffbd1e0eae5de6567dff32bd58f28623635657779760c9d9539d6b7cc59`  
		Last Modified: Tue, 02 Aug 2022 00:57:06 GMT  
		Size: 24.9 MB (24889750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb25ee9d7e5ee2ba3d5fe6104206a45f2c5c425365a535e0aaac7bb9bd71034e`  
		Last Modified: Wed, 01 Mar 2023 07:23:36 GMT  
		Size: 2.5 MB (2467730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b5b10e99353e19dd9c56deed1fd46d8ffc3c3eb2ad78b8d36ac029a085764e`  
		Last Modified: Wed, 01 Mar 2023 07:23:40 GMT  
		Size: 24.5 MB (24521836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:6244f4148355ef7762cdd6fa0a825a4427f77fe830ccf680a3c4b2d169c243a5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48982704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7832d532ed0d3a9a7baa0bd09aebae67770df5cd6714588618f5e38eba5dd36`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 03:58:22 GMT
ADD file:407ef80699946b8a8560ae436dfc9ca6148067b3012c02b4cb4e54d6d0aca674 in / 
# Tue, 21 Nov 2023 03:58:22 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:15:28 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 21 Nov 2023 08:15:37 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Nov 2023 08:16:00 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d0b016a8027330736e9ca5c23b846a6a9c1eb0a32da6459047c95d22e9544cb7`  
		Last Modified: Tue, 21 Nov 2023 04:03:19 GMT  
		Size: 22.8 MB (22795884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354a94df70d4e7e46b42c1937a573d21ba53d8ee384e3950ba4177ec7b5442c7`  
		Last Modified: Tue, 21 Nov 2023 08:20:53 GMT  
		Size: 2.4 MB (2370779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9330c159bf0d14284d9e46e04b57428e1471f7e5e84343b8dca26138f52d5a5e`  
		Last Modified: Tue, 21 Nov 2023 08:20:59 GMT  
		Size: 23.8 MB (23816041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:a47dc78a5b55cc23cb2825635b4e005834682ebcfa5afd2f334e8e0e2bf51077
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.2 MB (58189000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4563ac6b13e4bbec6b55fb79d1eca25f426b37b4b627e81b3958f930c06d726`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:34 GMT
ADD file:475e94b9a8f65c7cd4d4156af31e83190240ff35d8038f3fa86ad124d4d5d299 in / 
# Tue, 21 Nov 2023 06:27:35 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:51:33 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 21 Nov 2023 08:51:40 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Nov 2023 08:51:59 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:78b429e3efdd9f2b163abf0bca6b1462a25b1c5eddc1dd47f5d3445c6413cfa1`  
		Last Modified: Tue, 21 Nov 2023 06:31:45 GMT  
		Size: 26.0 MB (25967796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba61a6960570324786833e88006201960f3b39419902df3c5d72ee859ed1963`  
		Last Modified: Tue, 21 Nov 2023 08:55:27 GMT  
		Size: 2.6 MB (2645887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4dfdc89451aa2b2d34a467dcbb81dea87ba3c921d5535212ff10e6339a11f49`  
		Last Modified: Tue, 21 Nov 2023 08:55:30 GMT  
		Size: 29.6 MB (29575317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; 386

```console
$ docker pull mono@sha256:adebb4a59a77b5ebe589f6a2c04c346021d1d934351d2a4e04d2d64f927c94f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99449439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:763a3fdbea1147f601eab862ca4b54622c848609eff883f70acb6708b075f8da`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:39 GMT
ADD file:f016ddd8ef89ed2b1825b3df9abc595f7e774f9a607e3481272e622153b57aaf in / 
# Wed, 01 Nov 2023 00:39:40 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 09:34:55 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 01 Nov 2023 09:35:06 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Nov 2023 09:35:34 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:36a7e611445c645573e630ead3c9d0a62139e195288b4e02b8a4dba6e0118b73`  
		Last Modified: Wed, 01 Nov 2023 00:45:00 GMT  
		Size: 27.8 MB (27846916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0121fb994873373d1332a70d7aff083930bda8f4874fa6e98379bf39abd5f3b8`  
		Last Modified: Wed, 01 Nov 2023 09:39:00 GMT  
		Size: 2.8 MB (2792538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f19fd2bd2e7c03f8ebdf16da322ba6e84ebc1029bdf08b25a80ca00e46d68c`  
		Last Modified: Wed, 01 Nov 2023 09:39:14 GMT  
		Size: 68.8 MB (68809985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:defa2f8c047d839e590b97fb1b9652e93b82414d17f8dea7279f1bc0f467fcf0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.3 MB (75292278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98e30e35a5de236a142e7288a3c84a86005d1c742b41498b3f75a9f26b3a76ca`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:04 GMT
ADD file:6d33ba25d3625e5f445fc2183b60c64e2cbc780cb541d7f8ac76ce193b311d13 in / 
# Tue, 02 Aug 2022 01:18:06 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 02:08:58 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 03 Aug 2022 02:09:16 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 03 Aug 2022 02:09:49 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:fc8842eebb7ccaf249b2bb2d6a3878fffdae26c9db8f23b393c7f76a6249d2f6`  
		Last Modified: Tue, 02 Aug 2022 01:25:45 GMT  
		Size: 30.6 MB (30560308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0b96bc274eefbc8d34a02735b6f704f29aaf7e6c4095edb588a74c1ffb2825`  
		Last Modified: Wed, 03 Aug 2022 02:15:49 GMT  
		Size: 2.9 MB (2892610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f103eac188d225f1b73fa0b0d6a3f2560c7fc46d7ec0f0e7e7a07330eb1ff0`  
		Last Modified: Wed, 03 Aug 2022 02:16:04 GMT  
		Size: 41.8 MB (41839360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10.0`

```console
$ docker pull mono@sha256:c61c97c26f6f997de3073d1b33bf9cbbaf2c4e8d678806a30c4358d7edf63693
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
$ docker pull mono@sha256:088544cff1ba3e43115fb989479bd9b429f8cec1b783f47ef0544b72e6982db8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.1 MB (225080049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23d6552d29f3abcbc35457990eb489a9c1a6e33a626212398ebacbf7be2f70c9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:33 GMT
ADD file:29d3eb64d192a97184f2aa169407b58e969b06268c6372b49eefb72bcadb6e99 in / 
# Wed, 01 Nov 2023 00:21:34 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 05:01:57 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 01 Nov 2023 05:02:05 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Nov 2023 05:02:30 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 01 Nov 2023 05:09:36 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:113c6ad4754853f4a2ae632cff7d90eba9145cca0bd6fa4d60aa432bd26be6c7`  
		Last Modified: Wed, 01 Nov 2023 00:26:56 GMT  
		Size: 27.2 MB (27187422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce1bd567401672434bad3cc050dbcca8eb38f5c62353edf0be2511a9c392b2c`  
		Last Modified: Wed, 01 Nov 2023 05:10:16 GMT  
		Size: 2.8 MB (2781004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc889d221e45f4a1537b9fd04532bd1fc2b3b0ae20ce2c3f887dfe02ed969df`  
		Last Modified: Wed, 01 Nov 2023 05:10:24 GMT  
		Size: 64.8 MB (64780530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec75df573a6069093bca81532c42e67e5b9f1cd0e0506e48c2ef7d4afa21c00e`  
		Last Modified: Wed, 01 Nov 2023 05:11:28 GMT  
		Size: 130.3 MB (130331093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; arm variant v5

```console
$ docker pull mono@sha256:5fd28ff75f47e10162fa8359e3457ed77e6a13c9eb64585df39efdf63e70a1a1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.9 MB (180861329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efa9d1dae1421f12f6f7eecf8cfaac5d7da3f6b99f6874365ce2f2f5fc9d9662`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:49:37 GMT
ADD file:2ed7ca0d45c68b46a10ae186e8a03f98e72cadfeed17105668f53adf14d31e1f in / 
# Tue, 02 Aug 2022 00:49:38 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 07:18:54 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 01 Mar 2023 07:19:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Mar 2023 07:19:22 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 01 Mar 2023 07:22:13 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:187ecffbd1e0eae5de6567dff32bd58f28623635657779760c9d9539d6b7cc59`  
		Last Modified: Tue, 02 Aug 2022 00:57:06 GMT  
		Size: 24.9 MB (24889750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb25ee9d7e5ee2ba3d5fe6104206a45f2c5c425365a535e0aaac7bb9bd71034e`  
		Last Modified: Wed, 01 Mar 2023 07:23:36 GMT  
		Size: 2.5 MB (2467730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b5b10e99353e19dd9c56deed1fd46d8ffc3c3eb2ad78b8d36ac029a085764e`  
		Last Modified: Wed, 01 Mar 2023 07:23:40 GMT  
		Size: 24.5 MB (24521836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75576104ae9839169a1957af7269a139e0be7d50d8cef2a4fe4011b528926e18`  
		Last Modified: Wed, 01 Mar 2023 07:25:04 GMT  
		Size: 129.0 MB (128982013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; arm variant v7

```console
$ docker pull mono@sha256:fad5d37b9e7772d99c00cd5a30b156b4502dfc9c3a69b2a7290d1fa1180adafb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.8 MB (176808297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fef433b8708da3b8c109fb467e2269cda8731dc543827e9d32cb52f7b6be799`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 03:58:22 GMT
ADD file:407ef80699946b8a8560ae436dfc9ca6148067b3012c02b4cb4e54d6d0aca674 in / 
# Tue, 21 Nov 2023 03:58:22 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:15:28 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 21 Nov 2023 08:15:37 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Nov 2023 08:16:00 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Nov 2023 08:20:09 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d0b016a8027330736e9ca5c23b846a6a9c1eb0a32da6459047c95d22e9544cb7`  
		Last Modified: Tue, 21 Nov 2023 04:03:19 GMT  
		Size: 22.8 MB (22795884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354a94df70d4e7e46b42c1937a573d21ba53d8ee384e3950ba4177ec7b5442c7`  
		Last Modified: Tue, 21 Nov 2023 08:20:53 GMT  
		Size: 2.4 MB (2370779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9330c159bf0d14284d9e46e04b57428e1471f7e5e84343b8dca26138f52d5a5e`  
		Last Modified: Tue, 21 Nov 2023 08:20:59 GMT  
		Size: 23.8 MB (23816041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8cc10095ce3fe4292acef0ffc63f8cdec520e66aeb8fea215f4a4b734a9ba96`  
		Last Modified: Tue, 21 Nov 2023 08:22:09 GMT  
		Size: 127.8 MB (127825593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:d78448d09a4eeb6a3a47bbc370579bc895b933ddd6a8bccba058af7340382321
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.7 MB (203694658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57f4204153e548f97b1f01a568f568e1173830483f0d086894bd8070e9779b69`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:34 GMT
ADD file:475e94b9a8f65c7cd4d4156af31e83190240ff35d8038f3fa86ad124d4d5d299 in / 
# Tue, 21 Nov 2023 06:27:35 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:51:33 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 21 Nov 2023 08:51:40 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Nov 2023 08:51:59 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Nov 2023 08:54:42 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:78b429e3efdd9f2b163abf0bca6b1462a25b1c5eddc1dd47f5d3445c6413cfa1`  
		Last Modified: Tue, 21 Nov 2023 06:31:45 GMT  
		Size: 26.0 MB (25967796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba61a6960570324786833e88006201960f3b39419902df3c5d72ee859ed1963`  
		Last Modified: Tue, 21 Nov 2023 08:55:27 GMT  
		Size: 2.6 MB (2645887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4dfdc89451aa2b2d34a467dcbb81dea87ba3c921d5535212ff10e6339a11f49`  
		Last Modified: Tue, 21 Nov 2023 08:55:30 GMT  
		Size: 29.6 MB (29575317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45897c882cde9d30f02104690f4c3d38fbbe2a61d9efdbed4a8400996f5fc7d7`  
		Last Modified: Tue, 21 Nov 2023 08:56:29 GMT  
		Size: 145.5 MB (145505658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; 386

```console
$ docker pull mono@sha256:b414eb29727dd814a1446707b990c5f2ae04ca33bd48388d2c6b3abab8918a54
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.9 MB (230903961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4153c0670bf89b1b7b982e398d954f5df80c7aaa90641ff7d3f153fed0e8107b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:39 GMT
ADD file:f016ddd8ef89ed2b1825b3df9abc595f7e774f9a607e3481272e622153b57aaf in / 
# Wed, 01 Nov 2023 00:39:40 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 09:34:55 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 01 Nov 2023 09:35:06 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Nov 2023 09:35:34 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 01 Nov 2023 09:38:12 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:36a7e611445c645573e630ead3c9d0a62139e195288b4e02b8a4dba6e0118b73`  
		Last Modified: Wed, 01 Nov 2023 00:45:00 GMT  
		Size: 27.8 MB (27846916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0121fb994873373d1332a70d7aff083930bda8f4874fa6e98379bf39abd5f3b8`  
		Last Modified: Wed, 01 Nov 2023 09:39:00 GMT  
		Size: 2.8 MB (2792538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f19fd2bd2e7c03f8ebdf16da322ba6e84ebc1029bdf08b25a80ca00e46d68c`  
		Last Modified: Wed, 01 Nov 2023 09:39:14 GMT  
		Size: 68.8 MB (68809985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd68142980e47041e12b1331253de545f54139dad1f3044c4ccf7d293a3f62b3`  
		Last Modified: Wed, 01 Nov 2023 09:40:45 GMT  
		Size: 131.5 MB (131454522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; ppc64le

```console
$ docker pull mono@sha256:6126f0b2219e750b391e2e0d63ac7a2df863d9e2356c43fba06fee0708676038
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **209.7 MB (209715776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e4e952c22c47db9a79c5ca425c7de3d576d719e2042713424b88a3dae8e5129`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:04 GMT
ADD file:6d33ba25d3625e5f445fc2183b60c64e2cbc780cb541d7f8ac76ce193b311d13 in / 
# Tue, 02 Aug 2022 01:18:06 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 02:08:58 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 03 Aug 2022 02:09:16 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 03 Aug 2022 02:09:49 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 03 Aug 2022 02:14:18 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:fc8842eebb7ccaf249b2bb2d6a3878fffdae26c9db8f23b393c7f76a6249d2f6`  
		Last Modified: Tue, 02 Aug 2022 01:25:45 GMT  
		Size: 30.6 MB (30560308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0b96bc274eefbc8d34a02735b6f704f29aaf7e6c4095edb588a74c1ffb2825`  
		Last Modified: Wed, 03 Aug 2022 02:15:49 GMT  
		Size: 2.9 MB (2892610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f103eac188d225f1b73fa0b0d6a3f2560c7fc46d7ec0f0e7e7a07330eb1ff0`  
		Last Modified: Wed, 03 Aug 2022 02:16:04 GMT  
		Size: 41.8 MB (41839360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a64f5c66cdaf23afe83539fd8177bddc2e783d6ca6ee6eb3cabd08a6a5c375`  
		Last Modified: Wed, 03 Aug 2022 02:17:54 GMT  
		Size: 134.4 MB (134423498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10.0-slim`

```console
$ docker pull mono@sha256:e0db64c5bcfeb8be85eab1732dca2c1feef667b8e4585057565d8389bf4f0ec5
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
$ docker pull mono@sha256:1abb60d3f90dfb5db58253226fff17b5826a8b0506e63a99e4be9803a088946e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94748956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8367d629ccfdb27d24cb1141138c6ff1c74ba6f524f18e67870a48c962f480d5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:33 GMT
ADD file:29d3eb64d192a97184f2aa169407b58e969b06268c6372b49eefb72bcadb6e99 in / 
# Wed, 01 Nov 2023 00:21:34 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 05:01:57 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 01 Nov 2023 05:02:05 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Nov 2023 05:02:30 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:113c6ad4754853f4a2ae632cff7d90eba9145cca0bd6fa4d60aa432bd26be6c7`  
		Last Modified: Wed, 01 Nov 2023 00:26:56 GMT  
		Size: 27.2 MB (27187422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce1bd567401672434bad3cc050dbcca8eb38f5c62353edf0be2511a9c392b2c`  
		Last Modified: Wed, 01 Nov 2023 05:10:16 GMT  
		Size: 2.8 MB (2781004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc889d221e45f4a1537b9fd04532bd1fc2b3b0ae20ce2c3f887dfe02ed969df`  
		Last Modified: Wed, 01 Nov 2023 05:10:24 GMT  
		Size: 64.8 MB (64780530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:9d52e2f9db76c24f9964eec255de917d7a05b180e6e45f98545846b130400ab6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51879316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccac5ddbcee195ea38a9828f45d157f2ef674624fb9a6a2d5529fc2f8e6b736a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:49:37 GMT
ADD file:2ed7ca0d45c68b46a10ae186e8a03f98e72cadfeed17105668f53adf14d31e1f in / 
# Tue, 02 Aug 2022 00:49:38 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 07:18:54 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 01 Mar 2023 07:19:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Mar 2023 07:19:22 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:187ecffbd1e0eae5de6567dff32bd58f28623635657779760c9d9539d6b7cc59`  
		Last Modified: Tue, 02 Aug 2022 00:57:06 GMT  
		Size: 24.9 MB (24889750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb25ee9d7e5ee2ba3d5fe6104206a45f2c5c425365a535e0aaac7bb9bd71034e`  
		Last Modified: Wed, 01 Mar 2023 07:23:36 GMT  
		Size: 2.5 MB (2467730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b5b10e99353e19dd9c56deed1fd46d8ffc3c3eb2ad78b8d36ac029a085764e`  
		Last Modified: Wed, 01 Mar 2023 07:23:40 GMT  
		Size: 24.5 MB (24521836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:6244f4148355ef7762cdd6fa0a825a4427f77fe830ccf680a3c4b2d169c243a5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48982704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7832d532ed0d3a9a7baa0bd09aebae67770df5cd6714588618f5e38eba5dd36`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 03:58:22 GMT
ADD file:407ef80699946b8a8560ae436dfc9ca6148067b3012c02b4cb4e54d6d0aca674 in / 
# Tue, 21 Nov 2023 03:58:22 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:15:28 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 21 Nov 2023 08:15:37 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Nov 2023 08:16:00 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d0b016a8027330736e9ca5c23b846a6a9c1eb0a32da6459047c95d22e9544cb7`  
		Last Modified: Tue, 21 Nov 2023 04:03:19 GMT  
		Size: 22.8 MB (22795884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354a94df70d4e7e46b42c1937a573d21ba53d8ee384e3950ba4177ec7b5442c7`  
		Last Modified: Tue, 21 Nov 2023 08:20:53 GMT  
		Size: 2.4 MB (2370779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9330c159bf0d14284d9e46e04b57428e1471f7e5e84343b8dca26138f52d5a5e`  
		Last Modified: Tue, 21 Nov 2023 08:20:59 GMT  
		Size: 23.8 MB (23816041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:a47dc78a5b55cc23cb2825635b4e005834682ebcfa5afd2f334e8e0e2bf51077
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.2 MB (58189000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4563ac6b13e4bbec6b55fb79d1eca25f426b37b4b627e81b3958f930c06d726`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:34 GMT
ADD file:475e94b9a8f65c7cd4d4156af31e83190240ff35d8038f3fa86ad124d4d5d299 in / 
# Tue, 21 Nov 2023 06:27:35 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:51:33 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 21 Nov 2023 08:51:40 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Nov 2023 08:51:59 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:78b429e3efdd9f2b163abf0bca6b1462a25b1c5eddc1dd47f5d3445c6413cfa1`  
		Last Modified: Tue, 21 Nov 2023 06:31:45 GMT  
		Size: 26.0 MB (25967796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba61a6960570324786833e88006201960f3b39419902df3c5d72ee859ed1963`  
		Last Modified: Tue, 21 Nov 2023 08:55:27 GMT  
		Size: 2.6 MB (2645887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4dfdc89451aa2b2d34a467dcbb81dea87ba3c921d5535212ff10e6339a11f49`  
		Last Modified: Tue, 21 Nov 2023 08:55:30 GMT  
		Size: 29.6 MB (29575317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; 386

```console
$ docker pull mono@sha256:adebb4a59a77b5ebe589f6a2c04c346021d1d934351d2a4e04d2d64f927c94f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99449439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:763a3fdbea1147f601eab862ca4b54622c848609eff883f70acb6708b075f8da`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:39 GMT
ADD file:f016ddd8ef89ed2b1825b3df9abc595f7e774f9a607e3481272e622153b57aaf in / 
# Wed, 01 Nov 2023 00:39:40 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 09:34:55 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 01 Nov 2023 09:35:06 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Nov 2023 09:35:34 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:36a7e611445c645573e630ead3c9d0a62139e195288b4e02b8a4dba6e0118b73`  
		Last Modified: Wed, 01 Nov 2023 00:45:00 GMT  
		Size: 27.8 MB (27846916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0121fb994873373d1332a70d7aff083930bda8f4874fa6e98379bf39abd5f3b8`  
		Last Modified: Wed, 01 Nov 2023 09:39:00 GMT  
		Size: 2.8 MB (2792538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f19fd2bd2e7c03f8ebdf16da322ba6e84ebc1029bdf08b25a80ca00e46d68c`  
		Last Modified: Wed, 01 Nov 2023 09:39:14 GMT  
		Size: 68.8 MB (68809985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:defa2f8c047d839e590b97fb1b9652e93b82414d17f8dea7279f1bc0f467fcf0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.3 MB (75292278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98e30e35a5de236a142e7288a3c84a86005d1c742b41498b3f75a9f26b3a76ca`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:04 GMT
ADD file:6d33ba25d3625e5f445fc2183b60c64e2cbc780cb541d7f8ac76ce193b311d13 in / 
# Tue, 02 Aug 2022 01:18:06 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 02:08:58 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 03 Aug 2022 02:09:16 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 03 Aug 2022 02:09:49 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:fc8842eebb7ccaf249b2bb2d6a3878fffdae26c9db8f23b393c7f76a6249d2f6`  
		Last Modified: Tue, 02 Aug 2022 01:25:45 GMT  
		Size: 30.6 MB (30560308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0b96bc274eefbc8d34a02735b6f704f29aaf7e6c4095edb588a74c1ffb2825`  
		Last Modified: Wed, 03 Aug 2022 02:15:49 GMT  
		Size: 2.9 MB (2892610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f103eac188d225f1b73fa0b0d6a3f2560c7fc46d7ec0f0e7e7a07330eb1ff0`  
		Last Modified: Wed, 03 Aug 2022 02:16:04 GMT  
		Size: 41.8 MB (41839360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10.0.104`

```console
$ docker pull mono@sha256:c61c97c26f6f997de3073d1b33bf9cbbaf2c4e8d678806a30c4358d7edf63693
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
$ docker pull mono@sha256:088544cff1ba3e43115fb989479bd9b429f8cec1b783f47ef0544b72e6982db8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.1 MB (225080049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23d6552d29f3abcbc35457990eb489a9c1a6e33a626212398ebacbf7be2f70c9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:33 GMT
ADD file:29d3eb64d192a97184f2aa169407b58e969b06268c6372b49eefb72bcadb6e99 in / 
# Wed, 01 Nov 2023 00:21:34 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 05:01:57 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 01 Nov 2023 05:02:05 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Nov 2023 05:02:30 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 01 Nov 2023 05:09:36 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:113c6ad4754853f4a2ae632cff7d90eba9145cca0bd6fa4d60aa432bd26be6c7`  
		Last Modified: Wed, 01 Nov 2023 00:26:56 GMT  
		Size: 27.2 MB (27187422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce1bd567401672434bad3cc050dbcca8eb38f5c62353edf0be2511a9c392b2c`  
		Last Modified: Wed, 01 Nov 2023 05:10:16 GMT  
		Size: 2.8 MB (2781004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc889d221e45f4a1537b9fd04532bd1fc2b3b0ae20ce2c3f887dfe02ed969df`  
		Last Modified: Wed, 01 Nov 2023 05:10:24 GMT  
		Size: 64.8 MB (64780530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec75df573a6069093bca81532c42e67e5b9f1cd0e0506e48c2ef7d4afa21c00e`  
		Last Modified: Wed, 01 Nov 2023 05:11:28 GMT  
		Size: 130.3 MB (130331093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; arm variant v5

```console
$ docker pull mono@sha256:5fd28ff75f47e10162fa8359e3457ed77e6a13c9eb64585df39efdf63e70a1a1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.9 MB (180861329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efa9d1dae1421f12f6f7eecf8cfaac5d7da3f6b99f6874365ce2f2f5fc9d9662`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:49:37 GMT
ADD file:2ed7ca0d45c68b46a10ae186e8a03f98e72cadfeed17105668f53adf14d31e1f in / 
# Tue, 02 Aug 2022 00:49:38 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 07:18:54 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 01 Mar 2023 07:19:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Mar 2023 07:19:22 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 01 Mar 2023 07:22:13 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:187ecffbd1e0eae5de6567dff32bd58f28623635657779760c9d9539d6b7cc59`  
		Last Modified: Tue, 02 Aug 2022 00:57:06 GMT  
		Size: 24.9 MB (24889750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb25ee9d7e5ee2ba3d5fe6104206a45f2c5c425365a535e0aaac7bb9bd71034e`  
		Last Modified: Wed, 01 Mar 2023 07:23:36 GMT  
		Size: 2.5 MB (2467730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b5b10e99353e19dd9c56deed1fd46d8ffc3c3eb2ad78b8d36ac029a085764e`  
		Last Modified: Wed, 01 Mar 2023 07:23:40 GMT  
		Size: 24.5 MB (24521836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75576104ae9839169a1957af7269a139e0be7d50d8cef2a4fe4011b528926e18`  
		Last Modified: Wed, 01 Mar 2023 07:25:04 GMT  
		Size: 129.0 MB (128982013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; arm variant v7

```console
$ docker pull mono@sha256:fad5d37b9e7772d99c00cd5a30b156b4502dfc9c3a69b2a7290d1fa1180adafb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.8 MB (176808297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fef433b8708da3b8c109fb467e2269cda8731dc543827e9d32cb52f7b6be799`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 03:58:22 GMT
ADD file:407ef80699946b8a8560ae436dfc9ca6148067b3012c02b4cb4e54d6d0aca674 in / 
# Tue, 21 Nov 2023 03:58:22 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:15:28 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 21 Nov 2023 08:15:37 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Nov 2023 08:16:00 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Nov 2023 08:20:09 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d0b016a8027330736e9ca5c23b846a6a9c1eb0a32da6459047c95d22e9544cb7`  
		Last Modified: Tue, 21 Nov 2023 04:03:19 GMT  
		Size: 22.8 MB (22795884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354a94df70d4e7e46b42c1937a573d21ba53d8ee384e3950ba4177ec7b5442c7`  
		Last Modified: Tue, 21 Nov 2023 08:20:53 GMT  
		Size: 2.4 MB (2370779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9330c159bf0d14284d9e46e04b57428e1471f7e5e84343b8dca26138f52d5a5e`  
		Last Modified: Tue, 21 Nov 2023 08:20:59 GMT  
		Size: 23.8 MB (23816041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8cc10095ce3fe4292acef0ffc63f8cdec520e66aeb8fea215f4a4b734a9ba96`  
		Last Modified: Tue, 21 Nov 2023 08:22:09 GMT  
		Size: 127.8 MB (127825593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:d78448d09a4eeb6a3a47bbc370579bc895b933ddd6a8bccba058af7340382321
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.7 MB (203694658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57f4204153e548f97b1f01a568f568e1173830483f0d086894bd8070e9779b69`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:34 GMT
ADD file:475e94b9a8f65c7cd4d4156af31e83190240ff35d8038f3fa86ad124d4d5d299 in / 
# Tue, 21 Nov 2023 06:27:35 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:51:33 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 21 Nov 2023 08:51:40 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Nov 2023 08:51:59 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Nov 2023 08:54:42 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:78b429e3efdd9f2b163abf0bca6b1462a25b1c5eddc1dd47f5d3445c6413cfa1`  
		Last Modified: Tue, 21 Nov 2023 06:31:45 GMT  
		Size: 26.0 MB (25967796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba61a6960570324786833e88006201960f3b39419902df3c5d72ee859ed1963`  
		Last Modified: Tue, 21 Nov 2023 08:55:27 GMT  
		Size: 2.6 MB (2645887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4dfdc89451aa2b2d34a467dcbb81dea87ba3c921d5535212ff10e6339a11f49`  
		Last Modified: Tue, 21 Nov 2023 08:55:30 GMT  
		Size: 29.6 MB (29575317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45897c882cde9d30f02104690f4c3d38fbbe2a61d9efdbed4a8400996f5fc7d7`  
		Last Modified: Tue, 21 Nov 2023 08:56:29 GMT  
		Size: 145.5 MB (145505658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; 386

```console
$ docker pull mono@sha256:b414eb29727dd814a1446707b990c5f2ae04ca33bd48388d2c6b3abab8918a54
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.9 MB (230903961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4153c0670bf89b1b7b982e398d954f5df80c7aaa90641ff7d3f153fed0e8107b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:39 GMT
ADD file:f016ddd8ef89ed2b1825b3df9abc595f7e774f9a607e3481272e622153b57aaf in / 
# Wed, 01 Nov 2023 00:39:40 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 09:34:55 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 01 Nov 2023 09:35:06 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Nov 2023 09:35:34 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 01 Nov 2023 09:38:12 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:36a7e611445c645573e630ead3c9d0a62139e195288b4e02b8a4dba6e0118b73`  
		Last Modified: Wed, 01 Nov 2023 00:45:00 GMT  
		Size: 27.8 MB (27846916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0121fb994873373d1332a70d7aff083930bda8f4874fa6e98379bf39abd5f3b8`  
		Last Modified: Wed, 01 Nov 2023 09:39:00 GMT  
		Size: 2.8 MB (2792538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f19fd2bd2e7c03f8ebdf16da322ba6e84ebc1029bdf08b25a80ca00e46d68c`  
		Last Modified: Wed, 01 Nov 2023 09:39:14 GMT  
		Size: 68.8 MB (68809985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd68142980e47041e12b1331253de545f54139dad1f3044c4ccf7d293a3f62b3`  
		Last Modified: Wed, 01 Nov 2023 09:40:45 GMT  
		Size: 131.5 MB (131454522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; ppc64le

```console
$ docker pull mono@sha256:6126f0b2219e750b391e2e0d63ac7a2df863d9e2356c43fba06fee0708676038
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **209.7 MB (209715776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e4e952c22c47db9a79c5ca425c7de3d576d719e2042713424b88a3dae8e5129`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:04 GMT
ADD file:6d33ba25d3625e5f445fc2183b60c64e2cbc780cb541d7f8ac76ce193b311d13 in / 
# Tue, 02 Aug 2022 01:18:06 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 02:08:58 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 03 Aug 2022 02:09:16 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 03 Aug 2022 02:09:49 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 03 Aug 2022 02:14:18 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:fc8842eebb7ccaf249b2bb2d6a3878fffdae26c9db8f23b393c7f76a6249d2f6`  
		Last Modified: Tue, 02 Aug 2022 01:25:45 GMT  
		Size: 30.6 MB (30560308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0b96bc274eefbc8d34a02735b6f704f29aaf7e6c4095edb588a74c1ffb2825`  
		Last Modified: Wed, 03 Aug 2022 02:15:49 GMT  
		Size: 2.9 MB (2892610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f103eac188d225f1b73fa0b0d6a3f2560c7fc46d7ec0f0e7e7a07330eb1ff0`  
		Last Modified: Wed, 03 Aug 2022 02:16:04 GMT  
		Size: 41.8 MB (41839360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a64f5c66cdaf23afe83539fd8177bddc2e783d6ca6ee6eb3cabd08a6a5c375`  
		Last Modified: Wed, 03 Aug 2022 02:17:54 GMT  
		Size: 134.4 MB (134423498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10.0.104-slim`

```console
$ docker pull mono@sha256:e0db64c5bcfeb8be85eab1732dca2c1feef667b8e4585057565d8389bf4f0ec5
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
$ docker pull mono@sha256:1abb60d3f90dfb5db58253226fff17b5826a8b0506e63a99e4be9803a088946e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94748956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8367d629ccfdb27d24cb1141138c6ff1c74ba6f524f18e67870a48c962f480d5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:33 GMT
ADD file:29d3eb64d192a97184f2aa169407b58e969b06268c6372b49eefb72bcadb6e99 in / 
# Wed, 01 Nov 2023 00:21:34 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 05:01:57 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 01 Nov 2023 05:02:05 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Nov 2023 05:02:30 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:113c6ad4754853f4a2ae632cff7d90eba9145cca0bd6fa4d60aa432bd26be6c7`  
		Last Modified: Wed, 01 Nov 2023 00:26:56 GMT  
		Size: 27.2 MB (27187422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce1bd567401672434bad3cc050dbcca8eb38f5c62353edf0be2511a9c392b2c`  
		Last Modified: Wed, 01 Nov 2023 05:10:16 GMT  
		Size: 2.8 MB (2781004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc889d221e45f4a1537b9fd04532bd1fc2b3b0ae20ce2c3f887dfe02ed969df`  
		Last Modified: Wed, 01 Nov 2023 05:10:24 GMT  
		Size: 64.8 MB (64780530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:9d52e2f9db76c24f9964eec255de917d7a05b180e6e45f98545846b130400ab6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51879316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccac5ddbcee195ea38a9828f45d157f2ef674624fb9a6a2d5529fc2f8e6b736a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:49:37 GMT
ADD file:2ed7ca0d45c68b46a10ae186e8a03f98e72cadfeed17105668f53adf14d31e1f in / 
# Tue, 02 Aug 2022 00:49:38 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 07:18:54 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 01 Mar 2023 07:19:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Mar 2023 07:19:22 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:187ecffbd1e0eae5de6567dff32bd58f28623635657779760c9d9539d6b7cc59`  
		Last Modified: Tue, 02 Aug 2022 00:57:06 GMT  
		Size: 24.9 MB (24889750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb25ee9d7e5ee2ba3d5fe6104206a45f2c5c425365a535e0aaac7bb9bd71034e`  
		Last Modified: Wed, 01 Mar 2023 07:23:36 GMT  
		Size: 2.5 MB (2467730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b5b10e99353e19dd9c56deed1fd46d8ffc3c3eb2ad78b8d36ac029a085764e`  
		Last Modified: Wed, 01 Mar 2023 07:23:40 GMT  
		Size: 24.5 MB (24521836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:6244f4148355ef7762cdd6fa0a825a4427f77fe830ccf680a3c4b2d169c243a5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48982704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7832d532ed0d3a9a7baa0bd09aebae67770df5cd6714588618f5e38eba5dd36`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 03:58:22 GMT
ADD file:407ef80699946b8a8560ae436dfc9ca6148067b3012c02b4cb4e54d6d0aca674 in / 
# Tue, 21 Nov 2023 03:58:22 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:15:28 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 21 Nov 2023 08:15:37 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Nov 2023 08:16:00 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d0b016a8027330736e9ca5c23b846a6a9c1eb0a32da6459047c95d22e9544cb7`  
		Last Modified: Tue, 21 Nov 2023 04:03:19 GMT  
		Size: 22.8 MB (22795884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354a94df70d4e7e46b42c1937a573d21ba53d8ee384e3950ba4177ec7b5442c7`  
		Last Modified: Tue, 21 Nov 2023 08:20:53 GMT  
		Size: 2.4 MB (2370779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9330c159bf0d14284d9e46e04b57428e1471f7e5e84343b8dca26138f52d5a5e`  
		Last Modified: Tue, 21 Nov 2023 08:20:59 GMT  
		Size: 23.8 MB (23816041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:a47dc78a5b55cc23cb2825635b4e005834682ebcfa5afd2f334e8e0e2bf51077
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.2 MB (58189000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4563ac6b13e4bbec6b55fb79d1eca25f426b37b4b627e81b3958f930c06d726`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:34 GMT
ADD file:475e94b9a8f65c7cd4d4156af31e83190240ff35d8038f3fa86ad124d4d5d299 in / 
# Tue, 21 Nov 2023 06:27:35 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:51:33 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 21 Nov 2023 08:51:40 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Nov 2023 08:51:59 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:78b429e3efdd9f2b163abf0bca6b1462a25b1c5eddc1dd47f5d3445c6413cfa1`  
		Last Modified: Tue, 21 Nov 2023 06:31:45 GMT  
		Size: 26.0 MB (25967796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba61a6960570324786833e88006201960f3b39419902df3c5d72ee859ed1963`  
		Last Modified: Tue, 21 Nov 2023 08:55:27 GMT  
		Size: 2.6 MB (2645887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4dfdc89451aa2b2d34a467dcbb81dea87ba3c921d5535212ff10e6339a11f49`  
		Last Modified: Tue, 21 Nov 2023 08:55:30 GMT  
		Size: 29.6 MB (29575317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; 386

```console
$ docker pull mono@sha256:adebb4a59a77b5ebe589f6a2c04c346021d1d934351d2a4e04d2d64f927c94f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99449439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:763a3fdbea1147f601eab862ca4b54622c848609eff883f70acb6708b075f8da`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:39 GMT
ADD file:f016ddd8ef89ed2b1825b3df9abc595f7e774f9a607e3481272e622153b57aaf in / 
# Wed, 01 Nov 2023 00:39:40 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 09:34:55 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 01 Nov 2023 09:35:06 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Nov 2023 09:35:34 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:36a7e611445c645573e630ead3c9d0a62139e195288b4e02b8a4dba6e0118b73`  
		Last Modified: Wed, 01 Nov 2023 00:45:00 GMT  
		Size: 27.8 MB (27846916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0121fb994873373d1332a70d7aff083930bda8f4874fa6e98379bf39abd5f3b8`  
		Last Modified: Wed, 01 Nov 2023 09:39:00 GMT  
		Size: 2.8 MB (2792538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f19fd2bd2e7c03f8ebdf16da322ba6e84ebc1029bdf08b25a80ca00e46d68c`  
		Last Modified: Wed, 01 Nov 2023 09:39:14 GMT  
		Size: 68.8 MB (68809985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:defa2f8c047d839e590b97fb1b9652e93b82414d17f8dea7279f1bc0f467fcf0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.3 MB (75292278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98e30e35a5de236a142e7288a3c84a86005d1c742b41498b3f75a9f26b3a76ca`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:04 GMT
ADD file:6d33ba25d3625e5f445fc2183b60c64e2cbc780cb541d7f8ac76ce193b311d13 in / 
# Tue, 02 Aug 2022 01:18:06 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 02:08:58 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 03 Aug 2022 02:09:16 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 03 Aug 2022 02:09:49 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:fc8842eebb7ccaf249b2bb2d6a3878fffdae26c9db8f23b393c7f76a6249d2f6`  
		Last Modified: Tue, 02 Aug 2022 01:25:45 GMT  
		Size: 30.6 MB (30560308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0b96bc274eefbc8d34a02735b6f704f29aaf7e6c4095edb588a74c1ffb2825`  
		Last Modified: Wed, 03 Aug 2022 02:15:49 GMT  
		Size: 2.9 MB (2892610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f103eac188d225f1b73fa0b0d6a3f2560c7fc46d7ec0f0e7e7a07330eb1ff0`  
		Last Modified: Wed, 03 Aug 2022 02:16:04 GMT  
		Size: 41.8 MB (41839360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.12`

```console
$ docker pull mono@sha256:4abe0c2a97bd2cbd2a9ae115a02e685c54f7beab3ecd69532a33ea87f975c579
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
$ docker pull mono@sha256:d4b666878534b77724463e1a48ca0ed272f4ef2e4e57898dfd811089cf5b4c64
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.7 MB (254675607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf33e8f095a74d2e08dbd1cf9dab91f0e023164ed4b29cbcd15e83ea70a08b27`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:33 GMT
ADD file:29d3eb64d192a97184f2aa169407b58e969b06268c6372b49eefb72bcadb6e99 in / 
# Wed, 01 Nov 2023 00:21:34 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 05:01:16 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 01 Nov 2023 05:01:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Nov 2023 05:01:52 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 01 Nov 2023 05:04:26 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:113c6ad4754853f4a2ae632cff7d90eba9145cca0bd6fa4d60aa432bd26be6c7`  
		Last Modified: Wed, 01 Nov 2023 00:26:56 GMT  
		Size: 27.2 MB (27187422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018432e3f09706360a65c7c08b2f2e1997ee3e264599f9ee23b8ae9320814895`  
		Last Modified: Wed, 01 Nov 2023 05:09:53 GMT  
		Size: 2.8 MB (2780992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a7b7f1fcc5fc6bd617d375dabccb96b0eeecd3c1fc72440733884fa4bdc1503`  
		Last Modified: Wed, 01 Nov 2023 05:10:01 GMT  
		Size: 64.8 MB (64774577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6182d0a19d1676c36f4c3b2b64551e3f963466bf61976f0855369b05cc0b5266`  
		Last Modified: Wed, 01 Nov 2023 05:10:57 GMT  
		Size: 159.9 MB (159932616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12` - linux; arm variant v5

```console
$ docker pull mono@sha256:dea4d3a6cf8d83cd0b747ac36b0b7a279de919c38227c259e8f0dd933ad99d3d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.9 MB (192868079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52646a30a3e2966b0a92b143b872a725a0eaa3c003a2b6c3030454d2f5f26220`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:49:37 GMT
ADD file:2ed7ca0d45c68b46a10ae186e8a03f98e72cadfeed17105668f53adf14d31e1f in / 
# Tue, 02 Aug 2022 00:49:38 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 07:17:55 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 01 Mar 2023 07:18:17 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Mar 2023 07:18:42 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 01 Mar 2023 07:20:53 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:187ecffbd1e0eae5de6567dff32bd58f28623635657779760c9d9539d6b7cc59`  
		Last Modified: Tue, 02 Aug 2022 00:57:06 GMT  
		Size: 24.9 MB (24889750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6702eef9c7d9ec6ede2c5f9a15a047b314ccc9140f25694f337c0127478bb25b`  
		Last Modified: Wed, 01 Mar 2023 07:23:12 GMT  
		Size: 2.5 MB (2467715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3781ed66d8db4f1e7c7b6323f62af11c65550a10f339ad7c0fb68f9467f8026d`  
		Last Modified: Wed, 01 Mar 2023 07:23:17 GMT  
		Size: 24.5 MB (24503499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f32f45a77bbef0505ff02ad954c1ce25d1cb8f5b668bbd7c73fa538966d0c0b`  
		Last Modified: Wed, 01 Mar 2023 07:24:21 GMT  
		Size: 141.0 MB (141007115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12` - linux; arm variant v7

```console
$ docker pull mono@sha256:26c6610167b65aa65e842af4393ce1249efd17ef94a7d18e50dac8ec377d49cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.0 MB (189020371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26a526a0911129c09ef96bb6133ec8377df09020139dd8e1a9cfdc10ea46154a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 03:58:22 GMT
ADD file:407ef80699946b8a8560ae436dfc9ca6148067b3012c02b4cb4e54d6d0aca674 in / 
# Tue, 21 Nov 2023 03:58:22 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:14:47 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 21 Nov 2023 08:14:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Nov 2023 08:15:23 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Nov 2023 08:18:03 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d0b016a8027330736e9ca5c23b846a6a9c1eb0a32da6459047c95d22e9544cb7`  
		Last Modified: Tue, 21 Nov 2023 04:03:19 GMT  
		Size: 22.8 MB (22795884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2ab0cc04bbb4f3bd67f5ec694c4008bc3ac663112b267579b7329a492fc8f5`  
		Last Modified: Tue, 21 Nov 2023 08:20:35 GMT  
		Size: 2.4 MB (2370798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d12568a4ad10f5f80b54205380b845267c3ea411300837fe9faa9d56e0d73c4`  
		Last Modified: Tue, 21 Nov 2023 08:20:40 GMT  
		Size: 23.8 MB (23791217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65c029d99d34a3640b09029fcf63907253204fc8737758d0d95e19c924cc1413`  
		Last Modified: Tue, 21 Nov 2023 08:21:33 GMT  
		Size: 140.1 MB (140062472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:dbea7c6015e69ec89dde16e4a20bae61c77f464c82e42e1e21b7970c0344782e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.4 MB (216406658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29846055156fd6a82b9238f73926c1685a42c5d83cd25fa845ef60855b49cd11`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:34 GMT
ADD file:475e94b9a8f65c7cd4d4156af31e83190240ff35d8038f3fa86ad124d4d5d299 in / 
# Tue, 21 Nov 2023 06:27:35 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:50:59 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 21 Nov 2023 08:51:07 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Nov 2023 08:51:26 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Nov 2023 08:52:56 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:78b429e3efdd9f2b163abf0bca6b1462a25b1c5eddc1dd47f5d3445c6413cfa1`  
		Last Modified: Tue, 21 Nov 2023 06:31:45 GMT  
		Size: 26.0 MB (25967796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb5e1161766d0ff99d8c403407e1f624d50aaf500c2caf00c308fa65fd4d1184`  
		Last Modified: Tue, 21 Nov 2023 08:55:09 GMT  
		Size: 2.6 MB (2645901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b10043d7baec43e46ab0e0715597f3d283d2f0a778c399784ae85bd2cadbbe`  
		Last Modified: Tue, 21 Nov 2023 08:55:13 GMT  
		Size: 29.5 MB (29545201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ba77b4c4b8d91f24be23f4fc7919b9d5c36ccca4b44c92f079989544b8095c`  
		Last Modified: Tue, 21 Nov 2023 08:55:58 GMT  
		Size: 158.2 MB (158247760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12` - linux; 386

```console
$ docker pull mono@sha256:d54444ae4601e0badb94b98065160fc1a920d03f21d1c19d739845940929f88f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.6 MB (259559841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:143d59a7ac07f028ecb6dbebc5cfd6927673b6e0441d44b4317abf0bed0d145a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:39 GMT
ADD file:f016ddd8ef89ed2b1825b3df9abc595f7e774f9a607e3481272e622153b57aaf in / 
# Wed, 01 Nov 2023 00:39:40 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 09:34:07 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 01 Nov 2023 09:34:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Nov 2023 09:34:47 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 01 Nov 2023 09:37:01 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:36a7e611445c645573e630ead3c9d0a62139e195288b4e02b8a4dba6e0118b73`  
		Last Modified: Wed, 01 Nov 2023 00:45:00 GMT  
		Size: 27.8 MB (27846916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd0850558d4dd4cda278293930bdaa50e81cd25ab9eb55d766180c0aa1b1f59`  
		Last Modified: Wed, 01 Nov 2023 09:38:31 GMT  
		Size: 2.8 MB (2792539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cd462825126104e75cad134113d9c3120e9b4740eab8bb07a26b82826b51451`  
		Last Modified: Wed, 01 Nov 2023 09:38:45 GMT  
		Size: 68.8 MB (68800612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c56b1989d422bad3403fc2962148dfbcdf1737a8059c285e5883ce1c40872412`  
		Last Modified: Wed, 01 Nov 2023 09:40:00 GMT  
		Size: 160.1 MB (160119774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12` - linux; ppc64le

```console
$ docker pull mono@sha256:fbfb5b60906856f25cc0ffb3ed273fa5da089aed24eab6afb049cc150c221768
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.7 MB (221654331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45a10e5a16545c25df57d5cf1f034acbb78fb5a3c968378416dc576fa88386ef`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:04 GMT
ADD file:6d33ba25d3625e5f445fc2183b60c64e2cbc780cb541d7f8ac76ce193b311d13 in / 
# Tue, 02 Aug 2022 01:18:06 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 02:07:46 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 03 Aug 2022 02:08:06 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 03 Aug 2022 02:08:41 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 03 Aug 2022 02:11:40 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:fc8842eebb7ccaf249b2bb2d6a3878fffdae26c9db8f23b393c7f76a6249d2f6`  
		Last Modified: Tue, 02 Aug 2022 01:25:45 GMT  
		Size: 30.6 MB (30560308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1100971c8a3b3eb42c6e22a4c25f405143f007bda60d16697d49b333925b4d84`  
		Last Modified: Wed, 03 Aug 2022 02:15:13 GMT  
		Size: 2.9 MB (2892658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:390f883f1594b5d2d40b7ba4dc50f375439dd1611f38f0c3d071a38bf2ac62cd`  
		Last Modified: Wed, 03 Aug 2022 02:15:27 GMT  
		Size: 41.9 MB (41897345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae94af697c95b6bf75033b813f19ec72f68da49a681d5ce7078753923129147`  
		Last Modified: Wed, 03 Aug 2022 02:16:58 GMT  
		Size: 146.3 MB (146304020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.12-slim`

```console
$ docker pull mono@sha256:4ee2372e0eab5a1051a61f031a9d6f540ed74cba380afc523c9b31f20eba3b19
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
$ docker pull mono@sha256:3e33848de2b17f18b2ffbfbb6c62dddff99d8150e2a4ccf699bda9fdf2898f7b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94742991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:217398809241e0b3afff0a94ae94d93b7722c12f15c7abd1e6e1f0760d2203f9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:33 GMT
ADD file:29d3eb64d192a97184f2aa169407b58e969b06268c6372b49eefb72bcadb6e99 in / 
# Wed, 01 Nov 2023 00:21:34 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 05:01:16 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 01 Nov 2023 05:01:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Nov 2023 05:01:52 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:113c6ad4754853f4a2ae632cff7d90eba9145cca0bd6fa4d60aa432bd26be6c7`  
		Last Modified: Wed, 01 Nov 2023 00:26:56 GMT  
		Size: 27.2 MB (27187422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018432e3f09706360a65c7c08b2f2e1997ee3e264599f9ee23b8ae9320814895`  
		Last Modified: Wed, 01 Nov 2023 05:09:53 GMT  
		Size: 2.8 MB (2780992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a7b7f1fcc5fc6bd617d375dabccb96b0eeecd3c1fc72440733884fa4bdc1503`  
		Last Modified: Wed, 01 Nov 2023 05:10:01 GMT  
		Size: 64.8 MB (64774577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:f7c133539fa6a4add7484e9c93bc9b62ec32236d4b619f320c20b3248fb4739a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51860964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe52652f149ceedc89ed0c0f70985fcd898b6cd5cc98aa6f99f9ca06fd83046c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:49:37 GMT
ADD file:2ed7ca0d45c68b46a10ae186e8a03f98e72cadfeed17105668f53adf14d31e1f in / 
# Tue, 02 Aug 2022 00:49:38 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 07:17:55 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 01 Mar 2023 07:18:17 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Mar 2023 07:18:42 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:187ecffbd1e0eae5de6567dff32bd58f28623635657779760c9d9539d6b7cc59`  
		Last Modified: Tue, 02 Aug 2022 00:57:06 GMT  
		Size: 24.9 MB (24889750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6702eef9c7d9ec6ede2c5f9a15a047b314ccc9140f25694f337c0127478bb25b`  
		Last Modified: Wed, 01 Mar 2023 07:23:12 GMT  
		Size: 2.5 MB (2467715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3781ed66d8db4f1e7c7b6323f62af11c65550a10f339ad7c0fb68f9467f8026d`  
		Last Modified: Wed, 01 Mar 2023 07:23:17 GMT  
		Size: 24.5 MB (24503499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:5e8757a56832dbc6da018fcfaadf6ff1b6b658b619904346d79bd6dfa424e13d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48957899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec15648cad0f6cf0b22ae385f4806e7f6381f7740b9a0ff446655344513f454f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 03:58:22 GMT
ADD file:407ef80699946b8a8560ae436dfc9ca6148067b3012c02b4cb4e54d6d0aca674 in / 
# Tue, 21 Nov 2023 03:58:22 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:14:47 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 21 Nov 2023 08:14:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Nov 2023 08:15:23 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d0b016a8027330736e9ca5c23b846a6a9c1eb0a32da6459047c95d22e9544cb7`  
		Last Modified: Tue, 21 Nov 2023 04:03:19 GMT  
		Size: 22.8 MB (22795884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2ab0cc04bbb4f3bd67f5ec694c4008bc3ac663112b267579b7329a492fc8f5`  
		Last Modified: Tue, 21 Nov 2023 08:20:35 GMT  
		Size: 2.4 MB (2370798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d12568a4ad10f5f80b54205380b845267c3ea411300837fe9faa9d56e0d73c4`  
		Last Modified: Tue, 21 Nov 2023 08:20:40 GMT  
		Size: 23.8 MB (23791217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:c213688b7ba872a8b663c3a357748701d05bf4a34f8d8577211b43e19bb5a34f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.2 MB (58158898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:394752f8a02fce0133c215e5d4432e3507157d364fb9a64e5d2cb3f666fc8014`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:34 GMT
ADD file:475e94b9a8f65c7cd4d4156af31e83190240ff35d8038f3fa86ad124d4d5d299 in / 
# Tue, 21 Nov 2023 06:27:35 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:50:59 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 21 Nov 2023 08:51:07 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Nov 2023 08:51:26 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:78b429e3efdd9f2b163abf0bca6b1462a25b1c5eddc1dd47f5d3445c6413cfa1`  
		Last Modified: Tue, 21 Nov 2023 06:31:45 GMT  
		Size: 26.0 MB (25967796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb5e1161766d0ff99d8c403407e1f624d50aaf500c2caf00c308fa65fd4d1184`  
		Last Modified: Tue, 21 Nov 2023 08:55:09 GMT  
		Size: 2.6 MB (2645901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b10043d7baec43e46ab0e0715597f3d283d2f0a778c399784ae85bd2cadbbe`  
		Last Modified: Tue, 21 Nov 2023 08:55:13 GMT  
		Size: 29.5 MB (29545201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12-slim` - linux; 386

```console
$ docker pull mono@sha256:599faf3f778e3c5527c6b2884f09cdcbb76e8d4141ff225f16bccaf33eb4262e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99440067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9ea66b266996c0a54d4e901d02fb701aec85b8982405cf787fc22eeb621a04d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:39 GMT
ADD file:f016ddd8ef89ed2b1825b3df9abc595f7e774f9a607e3481272e622153b57aaf in / 
# Wed, 01 Nov 2023 00:39:40 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 09:34:07 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 01 Nov 2023 09:34:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Nov 2023 09:34:47 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:36a7e611445c645573e630ead3c9d0a62139e195288b4e02b8a4dba6e0118b73`  
		Last Modified: Wed, 01 Nov 2023 00:45:00 GMT  
		Size: 27.8 MB (27846916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd0850558d4dd4cda278293930bdaa50e81cd25ab9eb55d766180c0aa1b1f59`  
		Last Modified: Wed, 01 Nov 2023 09:38:31 GMT  
		Size: 2.8 MB (2792539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cd462825126104e75cad134113d9c3120e9b4740eab8bb07a26b82826b51451`  
		Last Modified: Wed, 01 Nov 2023 09:38:45 GMT  
		Size: 68.8 MB (68800612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:b83383e51874bbee097571b303be3299c87d7da8c4c6b0f4e067cfaa552ad925
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75350311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c28d9c810a28445dd3b5767c5be8a3a5c5f459f859498e49f59bb419b735510`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:04 GMT
ADD file:6d33ba25d3625e5f445fc2183b60c64e2cbc780cb541d7f8ac76ce193b311d13 in / 
# Tue, 02 Aug 2022 01:18:06 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 02:07:46 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 03 Aug 2022 02:08:06 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 03 Aug 2022 02:08:41 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:fc8842eebb7ccaf249b2bb2d6a3878fffdae26c9db8f23b393c7f76a6249d2f6`  
		Last Modified: Tue, 02 Aug 2022 01:25:45 GMT  
		Size: 30.6 MB (30560308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1100971c8a3b3eb42c6e22a4c25f405143f007bda60d16697d49b333925b4d84`  
		Last Modified: Wed, 03 Aug 2022 02:15:13 GMT  
		Size: 2.9 MB (2892658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:390f883f1594b5d2d40b7ba4dc50f375439dd1611f38f0c3d071a38bf2ac62cd`  
		Last Modified: Wed, 03 Aug 2022 02:15:27 GMT  
		Size: 41.9 MB (41897345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.12.0`

```console
$ docker pull mono@sha256:4abe0c2a97bd2cbd2a9ae115a02e685c54f7beab3ecd69532a33ea87f975c579
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
$ docker pull mono@sha256:d4b666878534b77724463e1a48ca0ed272f4ef2e4e57898dfd811089cf5b4c64
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.7 MB (254675607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf33e8f095a74d2e08dbd1cf9dab91f0e023164ed4b29cbcd15e83ea70a08b27`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:33 GMT
ADD file:29d3eb64d192a97184f2aa169407b58e969b06268c6372b49eefb72bcadb6e99 in / 
# Wed, 01 Nov 2023 00:21:34 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 05:01:16 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 01 Nov 2023 05:01:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Nov 2023 05:01:52 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 01 Nov 2023 05:04:26 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:113c6ad4754853f4a2ae632cff7d90eba9145cca0bd6fa4d60aa432bd26be6c7`  
		Last Modified: Wed, 01 Nov 2023 00:26:56 GMT  
		Size: 27.2 MB (27187422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018432e3f09706360a65c7c08b2f2e1997ee3e264599f9ee23b8ae9320814895`  
		Last Modified: Wed, 01 Nov 2023 05:09:53 GMT  
		Size: 2.8 MB (2780992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a7b7f1fcc5fc6bd617d375dabccb96b0eeecd3c1fc72440733884fa4bdc1503`  
		Last Modified: Wed, 01 Nov 2023 05:10:01 GMT  
		Size: 64.8 MB (64774577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6182d0a19d1676c36f4c3b2b64551e3f963466bf61976f0855369b05cc0b5266`  
		Last Modified: Wed, 01 Nov 2023 05:10:57 GMT  
		Size: 159.9 MB (159932616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0` - linux; arm variant v5

```console
$ docker pull mono@sha256:dea4d3a6cf8d83cd0b747ac36b0b7a279de919c38227c259e8f0dd933ad99d3d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.9 MB (192868079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52646a30a3e2966b0a92b143b872a725a0eaa3c003a2b6c3030454d2f5f26220`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:49:37 GMT
ADD file:2ed7ca0d45c68b46a10ae186e8a03f98e72cadfeed17105668f53adf14d31e1f in / 
# Tue, 02 Aug 2022 00:49:38 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 07:17:55 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 01 Mar 2023 07:18:17 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Mar 2023 07:18:42 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 01 Mar 2023 07:20:53 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:187ecffbd1e0eae5de6567dff32bd58f28623635657779760c9d9539d6b7cc59`  
		Last Modified: Tue, 02 Aug 2022 00:57:06 GMT  
		Size: 24.9 MB (24889750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6702eef9c7d9ec6ede2c5f9a15a047b314ccc9140f25694f337c0127478bb25b`  
		Last Modified: Wed, 01 Mar 2023 07:23:12 GMT  
		Size: 2.5 MB (2467715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3781ed66d8db4f1e7c7b6323f62af11c65550a10f339ad7c0fb68f9467f8026d`  
		Last Modified: Wed, 01 Mar 2023 07:23:17 GMT  
		Size: 24.5 MB (24503499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f32f45a77bbef0505ff02ad954c1ce25d1cb8f5b668bbd7c73fa538966d0c0b`  
		Last Modified: Wed, 01 Mar 2023 07:24:21 GMT  
		Size: 141.0 MB (141007115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0` - linux; arm variant v7

```console
$ docker pull mono@sha256:26c6610167b65aa65e842af4393ce1249efd17ef94a7d18e50dac8ec377d49cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.0 MB (189020371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26a526a0911129c09ef96bb6133ec8377df09020139dd8e1a9cfdc10ea46154a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 03:58:22 GMT
ADD file:407ef80699946b8a8560ae436dfc9ca6148067b3012c02b4cb4e54d6d0aca674 in / 
# Tue, 21 Nov 2023 03:58:22 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:14:47 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 21 Nov 2023 08:14:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Nov 2023 08:15:23 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Nov 2023 08:18:03 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d0b016a8027330736e9ca5c23b846a6a9c1eb0a32da6459047c95d22e9544cb7`  
		Last Modified: Tue, 21 Nov 2023 04:03:19 GMT  
		Size: 22.8 MB (22795884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2ab0cc04bbb4f3bd67f5ec694c4008bc3ac663112b267579b7329a492fc8f5`  
		Last Modified: Tue, 21 Nov 2023 08:20:35 GMT  
		Size: 2.4 MB (2370798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d12568a4ad10f5f80b54205380b845267c3ea411300837fe9faa9d56e0d73c4`  
		Last Modified: Tue, 21 Nov 2023 08:20:40 GMT  
		Size: 23.8 MB (23791217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65c029d99d34a3640b09029fcf63907253204fc8737758d0d95e19c924cc1413`  
		Last Modified: Tue, 21 Nov 2023 08:21:33 GMT  
		Size: 140.1 MB (140062472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:dbea7c6015e69ec89dde16e4a20bae61c77f464c82e42e1e21b7970c0344782e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.4 MB (216406658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29846055156fd6a82b9238f73926c1685a42c5d83cd25fa845ef60855b49cd11`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:34 GMT
ADD file:475e94b9a8f65c7cd4d4156af31e83190240ff35d8038f3fa86ad124d4d5d299 in / 
# Tue, 21 Nov 2023 06:27:35 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:50:59 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 21 Nov 2023 08:51:07 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Nov 2023 08:51:26 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Nov 2023 08:52:56 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:78b429e3efdd9f2b163abf0bca6b1462a25b1c5eddc1dd47f5d3445c6413cfa1`  
		Last Modified: Tue, 21 Nov 2023 06:31:45 GMT  
		Size: 26.0 MB (25967796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb5e1161766d0ff99d8c403407e1f624d50aaf500c2caf00c308fa65fd4d1184`  
		Last Modified: Tue, 21 Nov 2023 08:55:09 GMT  
		Size: 2.6 MB (2645901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b10043d7baec43e46ab0e0715597f3d283d2f0a778c399784ae85bd2cadbbe`  
		Last Modified: Tue, 21 Nov 2023 08:55:13 GMT  
		Size: 29.5 MB (29545201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ba77b4c4b8d91f24be23f4fc7919b9d5c36ccca4b44c92f079989544b8095c`  
		Last Modified: Tue, 21 Nov 2023 08:55:58 GMT  
		Size: 158.2 MB (158247760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0` - linux; 386

```console
$ docker pull mono@sha256:d54444ae4601e0badb94b98065160fc1a920d03f21d1c19d739845940929f88f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.6 MB (259559841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:143d59a7ac07f028ecb6dbebc5cfd6927673b6e0441d44b4317abf0bed0d145a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:39 GMT
ADD file:f016ddd8ef89ed2b1825b3df9abc595f7e774f9a607e3481272e622153b57aaf in / 
# Wed, 01 Nov 2023 00:39:40 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 09:34:07 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 01 Nov 2023 09:34:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Nov 2023 09:34:47 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 01 Nov 2023 09:37:01 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:36a7e611445c645573e630ead3c9d0a62139e195288b4e02b8a4dba6e0118b73`  
		Last Modified: Wed, 01 Nov 2023 00:45:00 GMT  
		Size: 27.8 MB (27846916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd0850558d4dd4cda278293930bdaa50e81cd25ab9eb55d766180c0aa1b1f59`  
		Last Modified: Wed, 01 Nov 2023 09:38:31 GMT  
		Size: 2.8 MB (2792539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cd462825126104e75cad134113d9c3120e9b4740eab8bb07a26b82826b51451`  
		Last Modified: Wed, 01 Nov 2023 09:38:45 GMT  
		Size: 68.8 MB (68800612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c56b1989d422bad3403fc2962148dfbcdf1737a8059c285e5883ce1c40872412`  
		Last Modified: Wed, 01 Nov 2023 09:40:00 GMT  
		Size: 160.1 MB (160119774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0` - linux; ppc64le

```console
$ docker pull mono@sha256:fbfb5b60906856f25cc0ffb3ed273fa5da089aed24eab6afb049cc150c221768
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.7 MB (221654331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45a10e5a16545c25df57d5cf1f034acbb78fb5a3c968378416dc576fa88386ef`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:04 GMT
ADD file:6d33ba25d3625e5f445fc2183b60c64e2cbc780cb541d7f8ac76ce193b311d13 in / 
# Tue, 02 Aug 2022 01:18:06 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 02:07:46 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 03 Aug 2022 02:08:06 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 03 Aug 2022 02:08:41 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 03 Aug 2022 02:11:40 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:fc8842eebb7ccaf249b2bb2d6a3878fffdae26c9db8f23b393c7f76a6249d2f6`  
		Last Modified: Tue, 02 Aug 2022 01:25:45 GMT  
		Size: 30.6 MB (30560308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1100971c8a3b3eb42c6e22a4c25f405143f007bda60d16697d49b333925b4d84`  
		Last Modified: Wed, 03 Aug 2022 02:15:13 GMT  
		Size: 2.9 MB (2892658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:390f883f1594b5d2d40b7ba4dc50f375439dd1611f38f0c3d071a38bf2ac62cd`  
		Last Modified: Wed, 03 Aug 2022 02:15:27 GMT  
		Size: 41.9 MB (41897345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae94af697c95b6bf75033b813f19ec72f68da49a681d5ce7078753923129147`  
		Last Modified: Wed, 03 Aug 2022 02:16:58 GMT  
		Size: 146.3 MB (146304020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.12.0-slim`

```console
$ docker pull mono@sha256:4ee2372e0eab5a1051a61f031a9d6f540ed74cba380afc523c9b31f20eba3b19
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
$ docker pull mono@sha256:3e33848de2b17f18b2ffbfbb6c62dddff99d8150e2a4ccf699bda9fdf2898f7b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94742991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:217398809241e0b3afff0a94ae94d93b7722c12f15c7abd1e6e1f0760d2203f9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:33 GMT
ADD file:29d3eb64d192a97184f2aa169407b58e969b06268c6372b49eefb72bcadb6e99 in / 
# Wed, 01 Nov 2023 00:21:34 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 05:01:16 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 01 Nov 2023 05:01:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Nov 2023 05:01:52 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:113c6ad4754853f4a2ae632cff7d90eba9145cca0bd6fa4d60aa432bd26be6c7`  
		Last Modified: Wed, 01 Nov 2023 00:26:56 GMT  
		Size: 27.2 MB (27187422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018432e3f09706360a65c7c08b2f2e1997ee3e264599f9ee23b8ae9320814895`  
		Last Modified: Wed, 01 Nov 2023 05:09:53 GMT  
		Size: 2.8 MB (2780992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a7b7f1fcc5fc6bd617d375dabccb96b0eeecd3c1fc72440733884fa4bdc1503`  
		Last Modified: Wed, 01 Nov 2023 05:10:01 GMT  
		Size: 64.8 MB (64774577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:f7c133539fa6a4add7484e9c93bc9b62ec32236d4b619f320c20b3248fb4739a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51860964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe52652f149ceedc89ed0c0f70985fcd898b6cd5cc98aa6f99f9ca06fd83046c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:49:37 GMT
ADD file:2ed7ca0d45c68b46a10ae186e8a03f98e72cadfeed17105668f53adf14d31e1f in / 
# Tue, 02 Aug 2022 00:49:38 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 07:17:55 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 01 Mar 2023 07:18:17 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Mar 2023 07:18:42 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:187ecffbd1e0eae5de6567dff32bd58f28623635657779760c9d9539d6b7cc59`  
		Last Modified: Tue, 02 Aug 2022 00:57:06 GMT  
		Size: 24.9 MB (24889750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6702eef9c7d9ec6ede2c5f9a15a047b314ccc9140f25694f337c0127478bb25b`  
		Last Modified: Wed, 01 Mar 2023 07:23:12 GMT  
		Size: 2.5 MB (2467715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3781ed66d8db4f1e7c7b6323f62af11c65550a10f339ad7c0fb68f9467f8026d`  
		Last Modified: Wed, 01 Mar 2023 07:23:17 GMT  
		Size: 24.5 MB (24503499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:5e8757a56832dbc6da018fcfaadf6ff1b6b658b619904346d79bd6dfa424e13d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48957899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec15648cad0f6cf0b22ae385f4806e7f6381f7740b9a0ff446655344513f454f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 03:58:22 GMT
ADD file:407ef80699946b8a8560ae436dfc9ca6148067b3012c02b4cb4e54d6d0aca674 in / 
# Tue, 21 Nov 2023 03:58:22 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:14:47 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 21 Nov 2023 08:14:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Nov 2023 08:15:23 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d0b016a8027330736e9ca5c23b846a6a9c1eb0a32da6459047c95d22e9544cb7`  
		Last Modified: Tue, 21 Nov 2023 04:03:19 GMT  
		Size: 22.8 MB (22795884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2ab0cc04bbb4f3bd67f5ec694c4008bc3ac663112b267579b7329a492fc8f5`  
		Last Modified: Tue, 21 Nov 2023 08:20:35 GMT  
		Size: 2.4 MB (2370798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d12568a4ad10f5f80b54205380b845267c3ea411300837fe9faa9d56e0d73c4`  
		Last Modified: Tue, 21 Nov 2023 08:20:40 GMT  
		Size: 23.8 MB (23791217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:c213688b7ba872a8b663c3a357748701d05bf4a34f8d8577211b43e19bb5a34f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.2 MB (58158898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:394752f8a02fce0133c215e5d4432e3507157d364fb9a64e5d2cb3f666fc8014`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:34 GMT
ADD file:475e94b9a8f65c7cd4d4156af31e83190240ff35d8038f3fa86ad124d4d5d299 in / 
# Tue, 21 Nov 2023 06:27:35 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:50:59 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 21 Nov 2023 08:51:07 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Nov 2023 08:51:26 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:78b429e3efdd9f2b163abf0bca6b1462a25b1c5eddc1dd47f5d3445c6413cfa1`  
		Last Modified: Tue, 21 Nov 2023 06:31:45 GMT  
		Size: 26.0 MB (25967796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb5e1161766d0ff99d8c403407e1f624d50aaf500c2caf00c308fa65fd4d1184`  
		Last Modified: Tue, 21 Nov 2023 08:55:09 GMT  
		Size: 2.6 MB (2645901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b10043d7baec43e46ab0e0715597f3d283d2f0a778c399784ae85bd2cadbbe`  
		Last Modified: Tue, 21 Nov 2023 08:55:13 GMT  
		Size: 29.5 MB (29545201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0-slim` - linux; 386

```console
$ docker pull mono@sha256:599faf3f778e3c5527c6b2884f09cdcbb76e8d4141ff225f16bccaf33eb4262e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99440067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9ea66b266996c0a54d4e901d02fb701aec85b8982405cf787fc22eeb621a04d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:39 GMT
ADD file:f016ddd8ef89ed2b1825b3df9abc595f7e774f9a607e3481272e622153b57aaf in / 
# Wed, 01 Nov 2023 00:39:40 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 09:34:07 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 01 Nov 2023 09:34:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Nov 2023 09:34:47 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:36a7e611445c645573e630ead3c9d0a62139e195288b4e02b8a4dba6e0118b73`  
		Last Modified: Wed, 01 Nov 2023 00:45:00 GMT  
		Size: 27.8 MB (27846916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd0850558d4dd4cda278293930bdaa50e81cd25ab9eb55d766180c0aa1b1f59`  
		Last Modified: Wed, 01 Nov 2023 09:38:31 GMT  
		Size: 2.8 MB (2792539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cd462825126104e75cad134113d9c3120e9b4740eab8bb07a26b82826b51451`  
		Last Modified: Wed, 01 Nov 2023 09:38:45 GMT  
		Size: 68.8 MB (68800612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:b83383e51874bbee097571b303be3299c87d7da8c4c6b0f4e067cfaa552ad925
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75350311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c28d9c810a28445dd3b5767c5be8a3a5c5f459f859498e49f59bb419b735510`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:04 GMT
ADD file:6d33ba25d3625e5f445fc2183b60c64e2cbc780cb541d7f8ac76ce193b311d13 in / 
# Tue, 02 Aug 2022 01:18:06 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 02:07:46 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 03 Aug 2022 02:08:06 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 03 Aug 2022 02:08:41 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:fc8842eebb7ccaf249b2bb2d6a3878fffdae26c9db8f23b393c7f76a6249d2f6`  
		Last Modified: Tue, 02 Aug 2022 01:25:45 GMT  
		Size: 30.6 MB (30560308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1100971c8a3b3eb42c6e22a4c25f405143f007bda60d16697d49b333925b4d84`  
		Last Modified: Wed, 03 Aug 2022 02:15:13 GMT  
		Size: 2.9 MB (2892658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:390f883f1594b5d2d40b7ba4dc50f375439dd1611f38f0c3d071a38bf2ac62cd`  
		Last Modified: Wed, 03 Aug 2022 02:15:27 GMT  
		Size: 41.9 MB (41897345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.12.0.182`

```console
$ docker pull mono@sha256:4abe0c2a97bd2cbd2a9ae115a02e685c54f7beab3ecd69532a33ea87f975c579
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.12.0.182` - linux; amd64

```console
$ docker pull mono@sha256:d4b666878534b77724463e1a48ca0ed272f4ef2e4e57898dfd811089cf5b4c64
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.7 MB (254675607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf33e8f095a74d2e08dbd1cf9dab91f0e023164ed4b29cbcd15e83ea70a08b27`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:33 GMT
ADD file:29d3eb64d192a97184f2aa169407b58e969b06268c6372b49eefb72bcadb6e99 in / 
# Wed, 01 Nov 2023 00:21:34 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 05:01:16 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 01 Nov 2023 05:01:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Nov 2023 05:01:52 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 01 Nov 2023 05:04:26 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:113c6ad4754853f4a2ae632cff7d90eba9145cca0bd6fa4d60aa432bd26be6c7`  
		Last Modified: Wed, 01 Nov 2023 00:26:56 GMT  
		Size: 27.2 MB (27187422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018432e3f09706360a65c7c08b2f2e1997ee3e264599f9ee23b8ae9320814895`  
		Last Modified: Wed, 01 Nov 2023 05:09:53 GMT  
		Size: 2.8 MB (2780992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a7b7f1fcc5fc6bd617d375dabccb96b0eeecd3c1fc72440733884fa4bdc1503`  
		Last Modified: Wed, 01 Nov 2023 05:10:01 GMT  
		Size: 64.8 MB (64774577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6182d0a19d1676c36f4c3b2b64551e3f963466bf61976f0855369b05cc0b5266`  
		Last Modified: Wed, 01 Nov 2023 05:10:57 GMT  
		Size: 159.9 MB (159932616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.182` - linux; arm variant v5

```console
$ docker pull mono@sha256:dea4d3a6cf8d83cd0b747ac36b0b7a279de919c38227c259e8f0dd933ad99d3d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.9 MB (192868079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52646a30a3e2966b0a92b143b872a725a0eaa3c003a2b6c3030454d2f5f26220`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:49:37 GMT
ADD file:2ed7ca0d45c68b46a10ae186e8a03f98e72cadfeed17105668f53adf14d31e1f in / 
# Tue, 02 Aug 2022 00:49:38 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 07:17:55 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 01 Mar 2023 07:18:17 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Mar 2023 07:18:42 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 01 Mar 2023 07:20:53 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:187ecffbd1e0eae5de6567dff32bd58f28623635657779760c9d9539d6b7cc59`  
		Last Modified: Tue, 02 Aug 2022 00:57:06 GMT  
		Size: 24.9 MB (24889750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6702eef9c7d9ec6ede2c5f9a15a047b314ccc9140f25694f337c0127478bb25b`  
		Last Modified: Wed, 01 Mar 2023 07:23:12 GMT  
		Size: 2.5 MB (2467715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3781ed66d8db4f1e7c7b6323f62af11c65550a10f339ad7c0fb68f9467f8026d`  
		Last Modified: Wed, 01 Mar 2023 07:23:17 GMT  
		Size: 24.5 MB (24503499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f32f45a77bbef0505ff02ad954c1ce25d1cb8f5b668bbd7c73fa538966d0c0b`  
		Last Modified: Wed, 01 Mar 2023 07:24:21 GMT  
		Size: 141.0 MB (141007115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.182` - linux; arm variant v7

```console
$ docker pull mono@sha256:26c6610167b65aa65e842af4393ce1249efd17ef94a7d18e50dac8ec377d49cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.0 MB (189020371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26a526a0911129c09ef96bb6133ec8377df09020139dd8e1a9cfdc10ea46154a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 03:58:22 GMT
ADD file:407ef80699946b8a8560ae436dfc9ca6148067b3012c02b4cb4e54d6d0aca674 in / 
# Tue, 21 Nov 2023 03:58:22 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:14:47 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 21 Nov 2023 08:14:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Nov 2023 08:15:23 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Nov 2023 08:18:03 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d0b016a8027330736e9ca5c23b846a6a9c1eb0a32da6459047c95d22e9544cb7`  
		Last Modified: Tue, 21 Nov 2023 04:03:19 GMT  
		Size: 22.8 MB (22795884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2ab0cc04bbb4f3bd67f5ec694c4008bc3ac663112b267579b7329a492fc8f5`  
		Last Modified: Tue, 21 Nov 2023 08:20:35 GMT  
		Size: 2.4 MB (2370798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d12568a4ad10f5f80b54205380b845267c3ea411300837fe9faa9d56e0d73c4`  
		Last Modified: Tue, 21 Nov 2023 08:20:40 GMT  
		Size: 23.8 MB (23791217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65c029d99d34a3640b09029fcf63907253204fc8737758d0d95e19c924cc1413`  
		Last Modified: Tue, 21 Nov 2023 08:21:33 GMT  
		Size: 140.1 MB (140062472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.182` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:dbea7c6015e69ec89dde16e4a20bae61c77f464c82e42e1e21b7970c0344782e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.4 MB (216406658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29846055156fd6a82b9238f73926c1685a42c5d83cd25fa845ef60855b49cd11`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:34 GMT
ADD file:475e94b9a8f65c7cd4d4156af31e83190240ff35d8038f3fa86ad124d4d5d299 in / 
# Tue, 21 Nov 2023 06:27:35 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:50:59 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 21 Nov 2023 08:51:07 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Nov 2023 08:51:26 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Nov 2023 08:52:56 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:78b429e3efdd9f2b163abf0bca6b1462a25b1c5eddc1dd47f5d3445c6413cfa1`  
		Last Modified: Tue, 21 Nov 2023 06:31:45 GMT  
		Size: 26.0 MB (25967796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb5e1161766d0ff99d8c403407e1f624d50aaf500c2caf00c308fa65fd4d1184`  
		Last Modified: Tue, 21 Nov 2023 08:55:09 GMT  
		Size: 2.6 MB (2645901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b10043d7baec43e46ab0e0715597f3d283d2f0a778c399784ae85bd2cadbbe`  
		Last Modified: Tue, 21 Nov 2023 08:55:13 GMT  
		Size: 29.5 MB (29545201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ba77b4c4b8d91f24be23f4fc7919b9d5c36ccca4b44c92f079989544b8095c`  
		Last Modified: Tue, 21 Nov 2023 08:55:58 GMT  
		Size: 158.2 MB (158247760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.182` - linux; 386

```console
$ docker pull mono@sha256:d54444ae4601e0badb94b98065160fc1a920d03f21d1c19d739845940929f88f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.6 MB (259559841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:143d59a7ac07f028ecb6dbebc5cfd6927673b6e0441d44b4317abf0bed0d145a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:39 GMT
ADD file:f016ddd8ef89ed2b1825b3df9abc595f7e774f9a607e3481272e622153b57aaf in / 
# Wed, 01 Nov 2023 00:39:40 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 09:34:07 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 01 Nov 2023 09:34:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Nov 2023 09:34:47 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 01 Nov 2023 09:37:01 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:36a7e611445c645573e630ead3c9d0a62139e195288b4e02b8a4dba6e0118b73`  
		Last Modified: Wed, 01 Nov 2023 00:45:00 GMT  
		Size: 27.8 MB (27846916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd0850558d4dd4cda278293930bdaa50e81cd25ab9eb55d766180c0aa1b1f59`  
		Last Modified: Wed, 01 Nov 2023 09:38:31 GMT  
		Size: 2.8 MB (2792539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cd462825126104e75cad134113d9c3120e9b4740eab8bb07a26b82826b51451`  
		Last Modified: Wed, 01 Nov 2023 09:38:45 GMT  
		Size: 68.8 MB (68800612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c56b1989d422bad3403fc2962148dfbcdf1737a8059c285e5883ce1c40872412`  
		Last Modified: Wed, 01 Nov 2023 09:40:00 GMT  
		Size: 160.1 MB (160119774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.182` - linux; ppc64le

```console
$ docker pull mono@sha256:fbfb5b60906856f25cc0ffb3ed273fa5da089aed24eab6afb049cc150c221768
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.7 MB (221654331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45a10e5a16545c25df57d5cf1f034acbb78fb5a3c968378416dc576fa88386ef`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:04 GMT
ADD file:6d33ba25d3625e5f445fc2183b60c64e2cbc780cb541d7f8ac76ce193b311d13 in / 
# Tue, 02 Aug 2022 01:18:06 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 02:07:46 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 03 Aug 2022 02:08:06 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 03 Aug 2022 02:08:41 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 03 Aug 2022 02:11:40 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:fc8842eebb7ccaf249b2bb2d6a3878fffdae26c9db8f23b393c7f76a6249d2f6`  
		Last Modified: Tue, 02 Aug 2022 01:25:45 GMT  
		Size: 30.6 MB (30560308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1100971c8a3b3eb42c6e22a4c25f405143f007bda60d16697d49b333925b4d84`  
		Last Modified: Wed, 03 Aug 2022 02:15:13 GMT  
		Size: 2.9 MB (2892658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:390f883f1594b5d2d40b7ba4dc50f375439dd1611f38f0c3d071a38bf2ac62cd`  
		Last Modified: Wed, 03 Aug 2022 02:15:27 GMT  
		Size: 41.9 MB (41897345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae94af697c95b6bf75033b813f19ec72f68da49a681d5ce7078753923129147`  
		Last Modified: Wed, 03 Aug 2022 02:16:58 GMT  
		Size: 146.3 MB (146304020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.12.0.182-slim`

```console
$ docker pull mono@sha256:4ee2372e0eab5a1051a61f031a9d6f540ed74cba380afc523c9b31f20eba3b19
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.12.0.182-slim` - linux; amd64

```console
$ docker pull mono@sha256:3e33848de2b17f18b2ffbfbb6c62dddff99d8150e2a4ccf699bda9fdf2898f7b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94742991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:217398809241e0b3afff0a94ae94d93b7722c12f15c7abd1e6e1f0760d2203f9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:33 GMT
ADD file:29d3eb64d192a97184f2aa169407b58e969b06268c6372b49eefb72bcadb6e99 in / 
# Wed, 01 Nov 2023 00:21:34 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 05:01:16 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 01 Nov 2023 05:01:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Nov 2023 05:01:52 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:113c6ad4754853f4a2ae632cff7d90eba9145cca0bd6fa4d60aa432bd26be6c7`  
		Last Modified: Wed, 01 Nov 2023 00:26:56 GMT  
		Size: 27.2 MB (27187422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018432e3f09706360a65c7c08b2f2e1997ee3e264599f9ee23b8ae9320814895`  
		Last Modified: Wed, 01 Nov 2023 05:09:53 GMT  
		Size: 2.8 MB (2780992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a7b7f1fcc5fc6bd617d375dabccb96b0eeecd3c1fc72440733884fa4bdc1503`  
		Last Modified: Wed, 01 Nov 2023 05:10:01 GMT  
		Size: 64.8 MB (64774577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.182-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:f7c133539fa6a4add7484e9c93bc9b62ec32236d4b619f320c20b3248fb4739a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51860964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe52652f149ceedc89ed0c0f70985fcd898b6cd5cc98aa6f99f9ca06fd83046c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:49:37 GMT
ADD file:2ed7ca0d45c68b46a10ae186e8a03f98e72cadfeed17105668f53adf14d31e1f in / 
# Tue, 02 Aug 2022 00:49:38 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 07:17:55 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 01 Mar 2023 07:18:17 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Mar 2023 07:18:42 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:187ecffbd1e0eae5de6567dff32bd58f28623635657779760c9d9539d6b7cc59`  
		Last Modified: Tue, 02 Aug 2022 00:57:06 GMT  
		Size: 24.9 MB (24889750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6702eef9c7d9ec6ede2c5f9a15a047b314ccc9140f25694f337c0127478bb25b`  
		Last Modified: Wed, 01 Mar 2023 07:23:12 GMT  
		Size: 2.5 MB (2467715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3781ed66d8db4f1e7c7b6323f62af11c65550a10f339ad7c0fb68f9467f8026d`  
		Last Modified: Wed, 01 Mar 2023 07:23:17 GMT  
		Size: 24.5 MB (24503499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.182-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:5e8757a56832dbc6da018fcfaadf6ff1b6b658b619904346d79bd6dfa424e13d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48957899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec15648cad0f6cf0b22ae385f4806e7f6381f7740b9a0ff446655344513f454f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 03:58:22 GMT
ADD file:407ef80699946b8a8560ae436dfc9ca6148067b3012c02b4cb4e54d6d0aca674 in / 
# Tue, 21 Nov 2023 03:58:22 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:14:47 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 21 Nov 2023 08:14:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Nov 2023 08:15:23 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d0b016a8027330736e9ca5c23b846a6a9c1eb0a32da6459047c95d22e9544cb7`  
		Last Modified: Tue, 21 Nov 2023 04:03:19 GMT  
		Size: 22.8 MB (22795884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2ab0cc04bbb4f3bd67f5ec694c4008bc3ac663112b267579b7329a492fc8f5`  
		Last Modified: Tue, 21 Nov 2023 08:20:35 GMT  
		Size: 2.4 MB (2370798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d12568a4ad10f5f80b54205380b845267c3ea411300837fe9faa9d56e0d73c4`  
		Last Modified: Tue, 21 Nov 2023 08:20:40 GMT  
		Size: 23.8 MB (23791217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.182-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:c213688b7ba872a8b663c3a357748701d05bf4a34f8d8577211b43e19bb5a34f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.2 MB (58158898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:394752f8a02fce0133c215e5d4432e3507157d364fb9a64e5d2cb3f666fc8014`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:34 GMT
ADD file:475e94b9a8f65c7cd4d4156af31e83190240ff35d8038f3fa86ad124d4d5d299 in / 
# Tue, 21 Nov 2023 06:27:35 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:50:59 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 21 Nov 2023 08:51:07 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Nov 2023 08:51:26 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:78b429e3efdd9f2b163abf0bca6b1462a25b1c5eddc1dd47f5d3445c6413cfa1`  
		Last Modified: Tue, 21 Nov 2023 06:31:45 GMT  
		Size: 26.0 MB (25967796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb5e1161766d0ff99d8c403407e1f624d50aaf500c2caf00c308fa65fd4d1184`  
		Last Modified: Tue, 21 Nov 2023 08:55:09 GMT  
		Size: 2.6 MB (2645901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b10043d7baec43e46ab0e0715597f3d283d2f0a778c399784ae85bd2cadbbe`  
		Last Modified: Tue, 21 Nov 2023 08:55:13 GMT  
		Size: 29.5 MB (29545201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.182-slim` - linux; 386

```console
$ docker pull mono@sha256:599faf3f778e3c5527c6b2884f09cdcbb76e8d4141ff225f16bccaf33eb4262e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99440067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9ea66b266996c0a54d4e901d02fb701aec85b8982405cf787fc22eeb621a04d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:39 GMT
ADD file:f016ddd8ef89ed2b1825b3df9abc595f7e774f9a607e3481272e622153b57aaf in / 
# Wed, 01 Nov 2023 00:39:40 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 09:34:07 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 01 Nov 2023 09:34:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Nov 2023 09:34:47 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:36a7e611445c645573e630ead3c9d0a62139e195288b4e02b8a4dba6e0118b73`  
		Last Modified: Wed, 01 Nov 2023 00:45:00 GMT  
		Size: 27.8 MB (27846916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd0850558d4dd4cda278293930bdaa50e81cd25ab9eb55d766180c0aa1b1f59`  
		Last Modified: Wed, 01 Nov 2023 09:38:31 GMT  
		Size: 2.8 MB (2792539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cd462825126104e75cad134113d9c3120e9b4740eab8bb07a26b82826b51451`  
		Last Modified: Wed, 01 Nov 2023 09:38:45 GMT  
		Size: 68.8 MB (68800612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.182-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:b83383e51874bbee097571b303be3299c87d7da8c4c6b0f4e067cfaa552ad925
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75350311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c28d9c810a28445dd3b5767c5be8a3a5c5f459f859498e49f59bb419b735510`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:04 GMT
ADD file:6d33ba25d3625e5f445fc2183b60c64e2cbc780cb541d7f8ac76ce193b311d13 in / 
# Tue, 02 Aug 2022 01:18:06 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 02:07:46 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 03 Aug 2022 02:08:06 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 03 Aug 2022 02:08:41 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:fc8842eebb7ccaf249b2bb2d6a3878fffdae26c9db8f23b393c7f76a6249d2f6`  
		Last Modified: Tue, 02 Aug 2022 01:25:45 GMT  
		Size: 30.6 MB (30560308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1100971c8a3b3eb42c6e22a4c25f405143f007bda60d16697d49b333925b4d84`  
		Last Modified: Wed, 03 Aug 2022 02:15:13 GMT  
		Size: 2.9 MB (2892658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:390f883f1594b5d2d40b7ba4dc50f375439dd1611f38f0c3d071a38bf2ac62cd`  
		Last Modified: Wed, 03 Aug 2022 02:15:27 GMT  
		Size: 41.9 MB (41897345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:latest`

```console
$ docker pull mono@sha256:4abe0c2a97bd2cbd2a9ae115a02e685c54f7beab3ecd69532a33ea87f975c579
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
$ docker pull mono@sha256:d4b666878534b77724463e1a48ca0ed272f4ef2e4e57898dfd811089cf5b4c64
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.7 MB (254675607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf33e8f095a74d2e08dbd1cf9dab91f0e023164ed4b29cbcd15e83ea70a08b27`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:33 GMT
ADD file:29d3eb64d192a97184f2aa169407b58e969b06268c6372b49eefb72bcadb6e99 in / 
# Wed, 01 Nov 2023 00:21:34 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 05:01:16 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 01 Nov 2023 05:01:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Nov 2023 05:01:52 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 01 Nov 2023 05:04:26 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:113c6ad4754853f4a2ae632cff7d90eba9145cca0bd6fa4d60aa432bd26be6c7`  
		Last Modified: Wed, 01 Nov 2023 00:26:56 GMT  
		Size: 27.2 MB (27187422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018432e3f09706360a65c7c08b2f2e1997ee3e264599f9ee23b8ae9320814895`  
		Last Modified: Wed, 01 Nov 2023 05:09:53 GMT  
		Size: 2.8 MB (2780992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a7b7f1fcc5fc6bd617d375dabccb96b0eeecd3c1fc72440733884fa4bdc1503`  
		Last Modified: Wed, 01 Nov 2023 05:10:01 GMT  
		Size: 64.8 MB (64774577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6182d0a19d1676c36f4c3b2b64551e3f963466bf61976f0855369b05cc0b5266`  
		Last Modified: Wed, 01 Nov 2023 05:10:57 GMT  
		Size: 159.9 MB (159932616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm variant v5

```console
$ docker pull mono@sha256:dea4d3a6cf8d83cd0b747ac36b0b7a279de919c38227c259e8f0dd933ad99d3d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.9 MB (192868079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52646a30a3e2966b0a92b143b872a725a0eaa3c003a2b6c3030454d2f5f26220`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:49:37 GMT
ADD file:2ed7ca0d45c68b46a10ae186e8a03f98e72cadfeed17105668f53adf14d31e1f in / 
# Tue, 02 Aug 2022 00:49:38 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 07:17:55 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 01 Mar 2023 07:18:17 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Mar 2023 07:18:42 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 01 Mar 2023 07:20:53 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:187ecffbd1e0eae5de6567dff32bd58f28623635657779760c9d9539d6b7cc59`  
		Last Modified: Tue, 02 Aug 2022 00:57:06 GMT  
		Size: 24.9 MB (24889750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6702eef9c7d9ec6ede2c5f9a15a047b314ccc9140f25694f337c0127478bb25b`  
		Last Modified: Wed, 01 Mar 2023 07:23:12 GMT  
		Size: 2.5 MB (2467715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3781ed66d8db4f1e7c7b6323f62af11c65550a10f339ad7c0fb68f9467f8026d`  
		Last Modified: Wed, 01 Mar 2023 07:23:17 GMT  
		Size: 24.5 MB (24503499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f32f45a77bbef0505ff02ad954c1ce25d1cb8f5b668bbd7c73fa538966d0c0b`  
		Last Modified: Wed, 01 Mar 2023 07:24:21 GMT  
		Size: 141.0 MB (141007115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm variant v7

```console
$ docker pull mono@sha256:26c6610167b65aa65e842af4393ce1249efd17ef94a7d18e50dac8ec377d49cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.0 MB (189020371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26a526a0911129c09ef96bb6133ec8377df09020139dd8e1a9cfdc10ea46154a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 03:58:22 GMT
ADD file:407ef80699946b8a8560ae436dfc9ca6148067b3012c02b4cb4e54d6d0aca674 in / 
# Tue, 21 Nov 2023 03:58:22 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:14:47 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 21 Nov 2023 08:14:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Nov 2023 08:15:23 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Nov 2023 08:18:03 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d0b016a8027330736e9ca5c23b846a6a9c1eb0a32da6459047c95d22e9544cb7`  
		Last Modified: Tue, 21 Nov 2023 04:03:19 GMT  
		Size: 22.8 MB (22795884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2ab0cc04bbb4f3bd67f5ec694c4008bc3ac663112b267579b7329a492fc8f5`  
		Last Modified: Tue, 21 Nov 2023 08:20:35 GMT  
		Size: 2.4 MB (2370798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d12568a4ad10f5f80b54205380b845267c3ea411300837fe9faa9d56e0d73c4`  
		Last Modified: Tue, 21 Nov 2023 08:20:40 GMT  
		Size: 23.8 MB (23791217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65c029d99d34a3640b09029fcf63907253204fc8737758d0d95e19c924cc1413`  
		Last Modified: Tue, 21 Nov 2023 08:21:33 GMT  
		Size: 140.1 MB (140062472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:dbea7c6015e69ec89dde16e4a20bae61c77f464c82e42e1e21b7970c0344782e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.4 MB (216406658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29846055156fd6a82b9238f73926c1685a42c5d83cd25fa845ef60855b49cd11`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:34 GMT
ADD file:475e94b9a8f65c7cd4d4156af31e83190240ff35d8038f3fa86ad124d4d5d299 in / 
# Tue, 21 Nov 2023 06:27:35 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:50:59 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 21 Nov 2023 08:51:07 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Nov 2023 08:51:26 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 21 Nov 2023 08:52:56 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:78b429e3efdd9f2b163abf0bca6b1462a25b1c5eddc1dd47f5d3445c6413cfa1`  
		Last Modified: Tue, 21 Nov 2023 06:31:45 GMT  
		Size: 26.0 MB (25967796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb5e1161766d0ff99d8c403407e1f624d50aaf500c2caf00c308fa65fd4d1184`  
		Last Modified: Tue, 21 Nov 2023 08:55:09 GMT  
		Size: 2.6 MB (2645901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b10043d7baec43e46ab0e0715597f3d283d2f0a778c399784ae85bd2cadbbe`  
		Last Modified: Tue, 21 Nov 2023 08:55:13 GMT  
		Size: 29.5 MB (29545201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ba77b4c4b8d91f24be23f4fc7919b9d5c36ccca4b44c92f079989544b8095c`  
		Last Modified: Tue, 21 Nov 2023 08:55:58 GMT  
		Size: 158.2 MB (158247760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; 386

```console
$ docker pull mono@sha256:d54444ae4601e0badb94b98065160fc1a920d03f21d1c19d739845940929f88f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.6 MB (259559841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:143d59a7ac07f028ecb6dbebc5cfd6927673b6e0441d44b4317abf0bed0d145a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:39 GMT
ADD file:f016ddd8ef89ed2b1825b3df9abc595f7e774f9a607e3481272e622153b57aaf in / 
# Wed, 01 Nov 2023 00:39:40 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 09:34:07 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 01 Nov 2023 09:34:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Nov 2023 09:34:47 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 01 Nov 2023 09:37:01 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:36a7e611445c645573e630ead3c9d0a62139e195288b4e02b8a4dba6e0118b73`  
		Last Modified: Wed, 01 Nov 2023 00:45:00 GMT  
		Size: 27.8 MB (27846916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd0850558d4dd4cda278293930bdaa50e81cd25ab9eb55d766180c0aa1b1f59`  
		Last Modified: Wed, 01 Nov 2023 09:38:31 GMT  
		Size: 2.8 MB (2792539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cd462825126104e75cad134113d9c3120e9b4740eab8bb07a26b82826b51451`  
		Last Modified: Wed, 01 Nov 2023 09:38:45 GMT  
		Size: 68.8 MB (68800612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c56b1989d422bad3403fc2962148dfbcdf1737a8059c285e5883ce1c40872412`  
		Last Modified: Wed, 01 Nov 2023 09:40:00 GMT  
		Size: 160.1 MB (160119774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; ppc64le

```console
$ docker pull mono@sha256:fbfb5b60906856f25cc0ffb3ed273fa5da089aed24eab6afb049cc150c221768
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.7 MB (221654331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45a10e5a16545c25df57d5cf1f034acbb78fb5a3c968378416dc576fa88386ef`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:04 GMT
ADD file:6d33ba25d3625e5f445fc2183b60c64e2cbc780cb541d7f8ac76ce193b311d13 in / 
# Tue, 02 Aug 2022 01:18:06 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 02:07:46 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 03 Aug 2022 02:08:06 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 03 Aug 2022 02:08:41 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 03 Aug 2022 02:11:40 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:fc8842eebb7ccaf249b2bb2d6a3878fffdae26c9db8f23b393c7f76a6249d2f6`  
		Last Modified: Tue, 02 Aug 2022 01:25:45 GMT  
		Size: 30.6 MB (30560308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1100971c8a3b3eb42c6e22a4c25f405143f007bda60d16697d49b333925b4d84`  
		Last Modified: Wed, 03 Aug 2022 02:15:13 GMT  
		Size: 2.9 MB (2892658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:390f883f1594b5d2d40b7ba4dc50f375439dd1611f38f0c3d071a38bf2ac62cd`  
		Last Modified: Wed, 03 Aug 2022 02:15:27 GMT  
		Size: 41.9 MB (41897345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae94af697c95b6bf75033b813f19ec72f68da49a681d5ce7078753923129147`  
		Last Modified: Wed, 03 Aug 2022 02:16:58 GMT  
		Size: 146.3 MB (146304020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:slim`

```console
$ docker pull mono@sha256:4ee2372e0eab5a1051a61f031a9d6f540ed74cba380afc523c9b31f20eba3b19
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
$ docker pull mono@sha256:3e33848de2b17f18b2ffbfbb6c62dddff99d8150e2a4ccf699bda9fdf2898f7b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94742991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:217398809241e0b3afff0a94ae94d93b7722c12f15c7abd1e6e1f0760d2203f9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:33 GMT
ADD file:29d3eb64d192a97184f2aa169407b58e969b06268c6372b49eefb72bcadb6e99 in / 
# Wed, 01 Nov 2023 00:21:34 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 05:01:16 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 01 Nov 2023 05:01:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Nov 2023 05:01:52 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:113c6ad4754853f4a2ae632cff7d90eba9145cca0bd6fa4d60aa432bd26be6c7`  
		Last Modified: Wed, 01 Nov 2023 00:26:56 GMT  
		Size: 27.2 MB (27187422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018432e3f09706360a65c7c08b2f2e1997ee3e264599f9ee23b8ae9320814895`  
		Last Modified: Wed, 01 Nov 2023 05:09:53 GMT  
		Size: 2.8 MB (2780992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a7b7f1fcc5fc6bd617d375dabccb96b0eeecd3c1fc72440733884fa4bdc1503`  
		Last Modified: Wed, 01 Nov 2023 05:10:01 GMT  
		Size: 64.8 MB (64774577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:f7c133539fa6a4add7484e9c93bc9b62ec32236d4b619f320c20b3248fb4739a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51860964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe52652f149ceedc89ed0c0f70985fcd898b6cd5cc98aa6f99f9ca06fd83046c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:49:37 GMT
ADD file:2ed7ca0d45c68b46a10ae186e8a03f98e72cadfeed17105668f53adf14d31e1f in / 
# Tue, 02 Aug 2022 00:49:38 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 07:17:55 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 01 Mar 2023 07:18:17 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Mar 2023 07:18:42 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:187ecffbd1e0eae5de6567dff32bd58f28623635657779760c9d9539d6b7cc59`  
		Last Modified: Tue, 02 Aug 2022 00:57:06 GMT  
		Size: 24.9 MB (24889750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6702eef9c7d9ec6ede2c5f9a15a047b314ccc9140f25694f337c0127478bb25b`  
		Last Modified: Wed, 01 Mar 2023 07:23:12 GMT  
		Size: 2.5 MB (2467715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3781ed66d8db4f1e7c7b6323f62af11c65550a10f339ad7c0fb68f9467f8026d`  
		Last Modified: Wed, 01 Mar 2023 07:23:17 GMT  
		Size: 24.5 MB (24503499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:5e8757a56832dbc6da018fcfaadf6ff1b6b658b619904346d79bd6dfa424e13d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48957899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec15648cad0f6cf0b22ae385f4806e7f6381f7740b9a0ff446655344513f454f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 03:58:22 GMT
ADD file:407ef80699946b8a8560ae436dfc9ca6148067b3012c02b4cb4e54d6d0aca674 in / 
# Tue, 21 Nov 2023 03:58:22 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:14:47 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 21 Nov 2023 08:14:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Nov 2023 08:15:23 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d0b016a8027330736e9ca5c23b846a6a9c1eb0a32da6459047c95d22e9544cb7`  
		Last Modified: Tue, 21 Nov 2023 04:03:19 GMT  
		Size: 22.8 MB (22795884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2ab0cc04bbb4f3bd67f5ec694c4008bc3ac663112b267579b7329a492fc8f5`  
		Last Modified: Tue, 21 Nov 2023 08:20:35 GMT  
		Size: 2.4 MB (2370798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d12568a4ad10f5f80b54205380b845267c3ea411300837fe9faa9d56e0d73c4`  
		Last Modified: Tue, 21 Nov 2023 08:20:40 GMT  
		Size: 23.8 MB (23791217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:c213688b7ba872a8b663c3a357748701d05bf4a34f8d8577211b43e19bb5a34f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.2 MB (58158898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:394752f8a02fce0133c215e5d4432e3507157d364fb9a64e5d2cb3f666fc8014`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:34 GMT
ADD file:475e94b9a8f65c7cd4d4156af31e83190240ff35d8038f3fa86ad124d4d5d299 in / 
# Tue, 21 Nov 2023 06:27:35 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:50:59 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 21 Nov 2023 08:51:07 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 21 Nov 2023 08:51:26 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:78b429e3efdd9f2b163abf0bca6b1462a25b1c5eddc1dd47f5d3445c6413cfa1`  
		Last Modified: Tue, 21 Nov 2023 06:31:45 GMT  
		Size: 26.0 MB (25967796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb5e1161766d0ff99d8c403407e1f624d50aaf500c2caf00c308fa65fd4d1184`  
		Last Modified: Tue, 21 Nov 2023 08:55:09 GMT  
		Size: 2.6 MB (2645901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b10043d7baec43e46ab0e0715597f3d283d2f0a778c399784ae85bd2cadbbe`  
		Last Modified: Tue, 21 Nov 2023 08:55:13 GMT  
		Size: 29.5 MB (29545201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; 386

```console
$ docker pull mono@sha256:599faf3f778e3c5527c6b2884f09cdcbb76e8d4141ff225f16bccaf33eb4262e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99440067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9ea66b266996c0a54d4e901d02fb701aec85b8982405cf787fc22eeb621a04d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:39 GMT
ADD file:f016ddd8ef89ed2b1825b3df9abc595f7e774f9a607e3481272e622153b57aaf in / 
# Wed, 01 Nov 2023 00:39:40 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 09:34:07 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 01 Nov 2023 09:34:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 01 Nov 2023 09:34:47 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:36a7e611445c645573e630ead3c9d0a62139e195288b4e02b8a4dba6e0118b73`  
		Last Modified: Wed, 01 Nov 2023 00:45:00 GMT  
		Size: 27.8 MB (27846916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd0850558d4dd4cda278293930bdaa50e81cd25ab9eb55d766180c0aa1b1f59`  
		Last Modified: Wed, 01 Nov 2023 09:38:31 GMT  
		Size: 2.8 MB (2792539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cd462825126104e75cad134113d9c3120e9b4740eab8bb07a26b82826b51451`  
		Last Modified: Wed, 01 Nov 2023 09:38:45 GMT  
		Size: 68.8 MB (68800612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; ppc64le

```console
$ docker pull mono@sha256:b83383e51874bbee097571b303be3299c87d7da8c4c6b0f4e067cfaa552ad925
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75350311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c28d9c810a28445dd3b5767c5be8a3a5c5f459f859498e49f59bb419b735510`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:04 GMT
ADD file:6d33ba25d3625e5f445fc2183b60c64e2cbc780cb541d7f8ac76ce193b311d13 in / 
# Tue, 02 Aug 2022 01:18:06 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 02:07:46 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 03 Aug 2022 02:08:06 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 03 Aug 2022 02:08:41 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:fc8842eebb7ccaf249b2bb2d6a3878fffdae26c9db8f23b393c7f76a6249d2f6`  
		Last Modified: Tue, 02 Aug 2022 01:25:45 GMT  
		Size: 30.6 MB (30560308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1100971c8a3b3eb42c6e22a4c25f405143f007bda60d16697d49b333925b4d84`  
		Last Modified: Wed, 03 Aug 2022 02:15:13 GMT  
		Size: 2.9 MB (2892658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:390f883f1594b5d2d40b7ba4dc50f375439dd1611f38f0c3d071a38bf2ac62cd`  
		Last Modified: Wed, 03 Aug 2022 02:15:27 GMT  
		Size: 41.9 MB (41897345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
