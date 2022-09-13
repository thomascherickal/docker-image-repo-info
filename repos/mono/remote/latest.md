## `mono:latest`

```console
$ docker pull mono@sha256:875d2da12c3466e916da349436d387b3155cd27d94a07d40c1251aeb029dc592
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
$ docker pull mono@sha256:0f87583446c377101f4a836bb80863262cfed0a76977f2828e8b2f71d80a73b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.4 MB (254410613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe28f835cd5014d333b328e9f5ef251645023b646c0c706ffd031948dfd5f399`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:48 GMT
ADD file:782d864aa72c2d5fb599311ebae56db4067d2e91ff532c1aaf1a291c3dbce5bb in / 
# Tue, 13 Sep 2022 00:56:49 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 13:17:37 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 13 Sep 2022 13:17:46 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Sep 2022 13:18:05 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Sep 2022 13:19:54 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4b7b4a8876e2f677668e51b8473f97a237d3d4df201b9df4031bcaa8068370b1`  
		Last Modified: Tue, 13 Sep 2022 01:01:16 GMT  
		Size: 27.1 MB (27130552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f8ea394174077f9198e4dc4dbd025a81c5c8c6ba17b1678efbecee1bdf20de`  
		Last Modified: Tue, 13 Sep 2022 13:25:44 GMT  
		Size: 2.8 MB (2777620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c1f2a8daaa8fc01b6f5ad67922ae8b7d5d4d0346a803a49370432678f225be`  
		Last Modified: Tue, 13 Sep 2022 13:25:54 GMT  
		Size: 64.8 MB (64772924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b06a8737a816cd557e6e42f1da537e5cef0b36255c5de504e6004ad611ce0e5`  
		Last Modified: Tue, 13 Sep 2022 13:27:14 GMT  
		Size: 159.7 MB (159729517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm variant v5

```console
$ docker pull mono@sha256:153723f54a88cb623b7c91adb146c12c5b467ac223a63507b497da89866148a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.9 MB (192878879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8a34fd2ee9f007475dd6af42f2772c497ab5e6859dc48c5c2ea264aee22337a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:49:37 GMT
ADD file:2ed7ca0d45c68b46a10ae186e8a03f98e72cadfeed17105668f53adf14d31e1f in / 
# Tue, 02 Aug 2022 00:49:38 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:05:39 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 02 Aug 2022 02:05:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 02 Aug 2022 02:06:12 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 02 Aug 2022 02:08:16 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:187ecffbd1e0eae5de6567dff32bd58f28623635657779760c9d9539d6b7cc59`  
		Last Modified: Tue, 02 Aug 2022 00:57:06 GMT  
		Size: 24.9 MB (24889750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5adcc503826343dbf406a02e57a44c42d684547b38770857bc2c7cab47ebabd9`  
		Last Modified: Tue, 02 Aug 2022 02:11:17 GMT  
		Size: 2.5 MB (2467686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2f60b5de6d7eebe25217cf4c9fbb14330dcb34be9f59c368e74c7aad0ff38f`  
		Last Modified: Tue, 02 Aug 2022 02:11:23 GMT  
		Size: 24.5 MB (24503302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0736c53353aeb7848dc15b8ae67124016edcdfa15088576a6afbd2cb59af3659`  
		Last Modified: Tue, 02 Aug 2022 02:12:36 GMT  
		Size: 141.0 MB (141018141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm variant v7

```console
$ docker pull mono@sha256:5b799daeb01a4dcdb27fffd995a2fb6370f3a13157fe6e0ae051706b94049c24
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **188.8 MB (188779736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecbc4d370c702bc821de6f1e6072c8cab170611a76eed90f0ba234d71d101439`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:43:37 GMT
ADD file:8d67c07b9926dee5d0124e48bd4b5039e6a84fdfe07a9e1077392f0e5772aa52 in / 
# Tue, 23 Aug 2022 01:43:37 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 21:11:21 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 23 Aug 2022 21:11:34 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 23 Aug 2022 21:11:56 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 23 Aug 2022 21:14:16 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:838efeda083c4fc3f1262c9c56947c82c6fdb90b64993afdb1375ce01ce1724b`  
		Last Modified: Tue, 23 Aug 2022 01:51:00 GMT  
		Size: 22.7 MB (22746698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38edabceecaf7d7ce8716dc9367d65645472c7d9d55595ea7e793549a2fb1dfd`  
		Last Modified: Tue, 23 Aug 2022 21:17:24 GMT  
		Size: 2.4 MB (2366962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df030e708ab2810b1b403656abed07b3acad91db4a1ab9a324ce8f867d90ad5`  
		Last Modified: Tue, 23 Aug 2022 21:17:29 GMT  
		Size: 23.8 MB (23789509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07cdc8dd267dd44a0df33576d020f2aef80c61a821f263e66fb530babd196810`  
		Last Modified: Tue, 23 Aug 2022 21:18:47 GMT  
		Size: 139.9 MB (139876567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:4d8ae333eada8643b1e3b720a593484960e24d7a97081d2b1ebcc3a2827726f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.9 MB (215904271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:992e23be3ddc609fb49c16fe55df76adad14346ca8f9321eeb3605b73a887329`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:58 GMT
ADD file:4c5bca2d158b11314fb47a6d4b34239575621c2f00f92e77870f23aa02913fac in / 
# Tue, 23 Aug 2022 01:52:59 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 13:16:26 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 23 Aug 2022 13:16:35 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 23 Aug 2022 13:16:50 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 23 Aug 2022 13:18:26 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a84b81edbdb892b3702892bbb01c240695b0b9d619fda43a9b951c9d2df1443c`  
		Last Modified: Tue, 23 Aug 2022 01:58:50 GMT  
		Size: 25.9 MB (25912515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7bd1a3749b3f6e3f2650136370ac7cf4432a69c3ea6089be520887feb8e7ee0`  
		Last Modified: Tue, 23 Aug 2022 13:20:25 GMT  
		Size: 2.6 MB (2641377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2516d51c34bbfe5d10f7aa17931b7bedcc269cd983cfeb7da2cb5307d17d19a1`  
		Last Modified: Tue, 23 Aug 2022 13:20:29 GMT  
		Size: 29.3 MB (29333413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e468bc8a5fafb868d5e649527d94f42d75e22b90c0cbf61aa51637e42c49b93`  
		Last Modified: Tue, 23 Aug 2022 13:21:32 GMT  
		Size: 158.0 MB (158016966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; 386

```console
$ docker pull mono@sha256:cf165c9510755cec665c833f99ca97c2b46f05ca60049d7dc6d5e1fe51289c6f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.1 MB (259070643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05d6d185cc237700b6538edfcc97ec5cfade585baa10f189cc28ad8bdc598feb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 01:40:12 GMT
ADD file:da95249e10828562612e8b0a3595f3cbf6a5cb5dbfb47302a4d42a4a8c5025b1 in / 
# Tue, 13 Sep 2022 01:40:12 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:48:43 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 13 Sep 2022 06:48:52 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Sep 2022 06:49:14 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Sep 2022 06:51:08 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7db2238a0cb6ea85529a33cb395b0243796e76066f31656ba5e08232e2fb0308`  
		Last Modified: Tue, 13 Sep 2022 01:46:12 GMT  
		Size: 27.8 MB (27790952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091742160360f141d6c1912368e67f0efb260e76cbf1c811424d15a2e198fb46`  
		Last Modified: Tue, 13 Sep 2022 06:53:32 GMT  
		Size: 2.8 MB (2789378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec07acb1c3a9f7a6015eaf4414ea88b8c41fc479f6c52a059e93dd2e8f1ee534`  
		Last Modified: Tue, 13 Sep 2022 06:53:41 GMT  
		Size: 68.6 MB (68586176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5219709757eb9519ffe0dcaf296c42ac50f5f1e6c21a4971083af5f6ed0ff1`  
		Last Modified: Tue, 13 Sep 2022 06:54:47 GMT  
		Size: 159.9 MB (159904137 bytes)  
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
