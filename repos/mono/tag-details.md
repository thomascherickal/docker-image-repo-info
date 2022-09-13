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
$ docker pull mono@sha256:b34a1b1b205c78b01e44fcf6b5155308e83c6c357977fd5e7026eff7407de026
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

### `mono:6` - linux; arm variant v5

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

### `mono:6` - linux; arm variant v7

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

### `mono:6` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:fd4938ac21581458b75a7f3513bae5635920c5e027861498324557d8f88cdee9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.9 MB (215898442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f85bcf336e06b49a2ce77e7f49b7d8f28c4983260055e62d8dd47624f239b723`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 02:11:20 GMT
ADD file:18fa3591fcbf0c3e065dbe581a069fc2af6fab9e4446047348404881af960725 in / 
# Tue, 13 Sep 2022 02:11:21 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 14:25:23 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 13 Sep 2022 14:25:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Sep 2022 14:25:47 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Sep 2022 14:27:23 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4c3f5cce277263c7aeaf67f83255af76927e03363e775f39d7587bc5036fcf1e`  
		Last Modified: Tue, 13 Sep 2022 02:17:10 GMT  
		Size: 25.9 MB (25904152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf1bcd765746fb733fe53109f7f09254547fc14af9cd08cfebb1fe80289a004`  
		Last Modified: Tue, 13 Sep 2022 14:29:03 GMT  
		Size: 2.6 MB (2641320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eedb38f3cdc2b7d72d243d8f80d986fc8c5722148df30f2b6ac2b9019f7e3b9`  
		Last Modified: Tue, 13 Sep 2022 14:29:08 GMT  
		Size: 29.3 MB (29333406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b50613517341b9dd3da923e0cec24f35044bf3377544ce59b470cf0ab35e993`  
		Last Modified: Tue, 13 Sep 2022 14:30:10 GMT  
		Size: 158.0 MB (158019564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; 386

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
$ docker pull mono@sha256:406d40ad3587b24cbf640473398da229a4577dbfff5f5ab8dd88e9b2b27d8a8a
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
$ docker pull mono@sha256:43e21877587c21a125ba97d474435087e87de3e0d19a5fb59226814a2ed4a556
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94681096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36f89a89c017304e116d9818f24b08de656e3841a6a7f587c8c5bc2b0228d6b8`
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

### `mono:6-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:3d36decf8882609bab164b6571c9e1975e4cd53e07ac0a376f9a774febc45c74
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51860738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5251c1b1cc35b1d2cb554f30f5b2f12a90a53f3472b1fc7839dfa91530021631`
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

### `mono:6-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:fb09f2f2c204a4635c74bd5a95114ed9d5dc7fd180c0050b0c25f32b8c989e49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48903169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e602747f8e64b4af84f3c87450b816d181ac4abd009c3255a96a56b0c58bde14`
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

### `mono:6-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:2aa229cb03c6549b44b14e24b115dccd2106ef10afc95f66529a8f90f9da5fb3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57878878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91be6728a6a5d81c6dfb3c13b2340ad35f6611dad08c35bf6640d49bbb9db356`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 02:11:20 GMT
ADD file:18fa3591fcbf0c3e065dbe581a069fc2af6fab9e4446047348404881af960725 in / 
# Tue, 13 Sep 2022 02:11:21 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 14:25:23 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 13 Sep 2022 14:25:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Sep 2022 14:25:47 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4c3f5cce277263c7aeaf67f83255af76927e03363e775f39d7587bc5036fcf1e`  
		Last Modified: Tue, 13 Sep 2022 02:17:10 GMT  
		Size: 25.9 MB (25904152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf1bcd765746fb733fe53109f7f09254547fc14af9cd08cfebb1fe80289a004`  
		Last Modified: Tue, 13 Sep 2022 14:29:03 GMT  
		Size: 2.6 MB (2641320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eedb38f3cdc2b7d72d243d8f80d986fc8c5722148df30f2b6ac2b9019f7e3b9`  
		Last Modified: Tue, 13 Sep 2022 14:29:08 GMT  
		Size: 29.3 MB (29333406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; 386

```console
$ docker pull mono@sha256:8ef911eede2000787ec9614d4147d27fd3cc3cff7299098645d2c331ff5000ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99166506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a06eb501431fb5c4a879cdedfba520528fb72e991ce30c46d974238e2103341`
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
$ docker pull mono@sha256:54c927dc76c98d6940d95191939e959bdb1c0b09d688a6eefa525b0b23e02143
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
$ docker pull mono@sha256:da05a83bdf8e682a1384d08f93d96c19241e438d65115bb64a93542368b49033
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.0 MB (225002881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86657b2acd31350e074591d40fed046d95443d90c5d22a4e30889b198d31c655`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:48 GMT
ADD file:782d864aa72c2d5fb599311ebae56db4067d2e91ff532c1aaf1a291c3dbce5bb in / 
# Tue, 13 Sep 2022 00:56:49 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 13:18:11 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Sep 2022 13:18:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Sep 2022 13:18:46 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Sep 2022 13:25:20 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4b7b4a8876e2f677668e51b8473f97a237d3d4df201b9df4031bcaa8068370b1`  
		Last Modified: Tue, 13 Sep 2022 01:01:16 GMT  
		Size: 27.1 MB (27130552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f30d1a79e581bc63843e16797ef34c77d71e42f8dab5b92e7bad411deabcac`  
		Last Modified: Tue, 13 Sep 2022 13:26:22 GMT  
		Size: 2.8 MB (2777658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4b42d23b8e39b264cc02008c057e7def09645acf552e125b3a136fa2ca017a`  
		Last Modified: Tue, 13 Sep 2022 13:26:31 GMT  
		Size: 64.8 MB (64779327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283bc86196f31f839c30c146b3c7128054d25d0e6821c034928eedc5e1e1f46b`  
		Last Modified: Tue, 13 Sep 2022 13:27:56 GMT  
		Size: 130.3 MB (130315344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; arm variant v5

```console
$ docker pull mono@sha256:0222156facf0460ee81820ef7977de4063cd983148f665910c5a49e24e3a7402
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.9 MB (180857422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2104524aaaa5c48fd39ac37bfe94bbeda0086a1ea289e1be14e280f94b1c0c8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:49:37 GMT
ADD file:2ed7ca0d45c68b46a10ae186e8a03f98e72cadfeed17105668f53adf14d31e1f in / 
# Tue, 02 Aug 2022 00:49:38 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:06:21 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 02 Aug 2022 02:06:31 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 02 Aug 2022 02:06:57 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 02 Aug 2022 02:10:28 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:187ecffbd1e0eae5de6567dff32bd58f28623635657779760c9d9539d6b7cc59`  
		Last Modified: Tue, 02 Aug 2022 00:57:06 GMT  
		Size: 24.9 MB (24889750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d1f7c779aa2742311c359ef531049f9a015701cf53969ec3c0b86bb6ed4d7d`  
		Last Modified: Tue, 02 Aug 2022 02:11:45 GMT  
		Size: 2.5 MB (2467689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e0854b1d2110cdccf321fe15cae0adbd1e734b32a4557490c2c49abd2d66f97`  
		Last Modified: Tue, 02 Aug 2022 02:11:50 GMT  
		Size: 24.5 MB (24521669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8006236a82fb24514f586974ded95bdd60e0959951dde202b6113bc760326e`  
		Last Modified: Tue, 02 Aug 2022 02:13:30 GMT  
		Size: 129.0 MB (128978314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; arm variant v7

```console
$ docker pull mono@sha256:37de3b0c33584ae9731b35fe2a5e38402f85f92eac9f77008303773a8f6d9920
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.8 MB (176757012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:227e330c7acb2efbfb2773f807f3860a49e1a3d515fa2984e14681244c767683`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:43:37 GMT
ADD file:8d67c07b9926dee5d0124e48bd4b5039e6a84fdfe07a9e1077392f0e5772aa52 in / 
# Tue, 23 Aug 2022 01:43:37 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 21:12:04 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 23 Aug 2022 21:12:16 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 23 Aug 2022 21:12:44 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 23 Aug 2022 21:16:33 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:838efeda083c4fc3f1262c9c56947c82c6fdb90b64993afdb1375ce01ce1724b`  
		Last Modified: Tue, 23 Aug 2022 01:51:00 GMT  
		Size: 22.7 MB (22746698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75d8ba3b02424e687c31e5dd2e4a8e74b8c51b4d0175a81b69735aeebb0e7a52`  
		Last Modified: Tue, 23 Aug 2022 21:17:53 GMT  
		Size: 2.4 MB (2366966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6094a07154b3e0a1af790f2b4281bedb8eda5373688ddf4d7758c78f16865911`  
		Last Modified: Tue, 23 Aug 2022 21:17:58 GMT  
		Size: 23.8 MB (23814792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9179f457685aedac47e660f0319e528f3aee0892c9cf3ddc4664fd15380d4c7c`  
		Last Modified: Tue, 23 Aug 2022 21:19:38 GMT  
		Size: 127.8 MB (127828556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:212c83e316ac1b28ef0e7b7b7a0072e061383b9bac36dfa231b54dda2b9a0f56
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.4 MB (203357374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c4c0d5dcca91ba6de1291aeb772e7035c4bf4cbf85b03c7b5c1cf1aa4b94b1b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 02:11:20 GMT
ADD file:18fa3591fcbf0c3e065dbe581a069fc2af6fab9e4446047348404881af960725 in / 
# Tue, 13 Sep 2022 02:11:21 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 14:25:55 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Sep 2022 14:26:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Sep 2022 14:26:19 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Sep 2022 14:28:26 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4c3f5cce277263c7aeaf67f83255af76927e03363e775f39d7587bc5036fcf1e`  
		Last Modified: Tue, 13 Sep 2022 02:17:10 GMT  
		Size: 25.9 MB (25904152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715d7d34ba910bd2b5bd88a1b9746572cd399b1b321eadfb5e9bf89f35f5cf01`  
		Last Modified: Tue, 13 Sep 2022 14:29:27 GMT  
		Size: 2.6 MB (2641345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4865d20ade904a532cc524f8362ec7e259ab3ef39d670cb72e47ce063c303523`  
		Last Modified: Tue, 13 Sep 2022 14:29:32 GMT  
		Size: 29.4 MB (29361197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b677a59228f837aadd289b9fdeef07443f81706ae644d4c62532ce8656cfcbd4`  
		Last Modified: Tue, 13 Sep 2022 14:30:52 GMT  
		Size: 145.5 MB (145450680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; 386

```console
$ docker pull mono@sha256:667dfaee00f413dea2417bb04680f0a5de4328515ab45ee2e4dc0c41269b278f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.6 MB (230595906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a8e479ba8c4dc385ee6f4c11f741d9587bd697e143f659af9c0ad81c27ef9a0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 01:40:12 GMT
ADD file:da95249e10828562612e8b0a3595f3cbf6a5cb5dbfb47302a4d42a4a8c5025b1 in / 
# Tue, 13 Sep 2022 01:40:12 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:49:20 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Sep 2022 06:49:29 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Sep 2022 06:49:55 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Sep 2022 06:52:39 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7db2238a0cb6ea85529a33cb395b0243796e76066f31656ba5e08232e2fb0308`  
		Last Modified: Tue, 13 Sep 2022 01:46:12 GMT  
		Size: 27.8 MB (27790952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2f07907e6e47b8f80c60ae70573642fdda80eaa70791e8977fadf5d56a73b6`  
		Last Modified: Tue, 13 Sep 2022 06:54:02 GMT  
		Size: 2.8 MB (2789402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ae77ac5737c4b823e9852bffe8c8ee90553eb251aa3b041c126afd7fc70dec`  
		Last Modified: Tue, 13 Sep 2022 06:54:11 GMT  
		Size: 68.6 MB (68594239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74689d9182ad76725ecab8ec2fec0741718d4acf1087aaec4e464598dee7529`  
		Last Modified: Tue, 13 Sep 2022 06:55:25 GMT  
		Size: 131.4 MB (131421313 bytes)  
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
$ docker pull mono@sha256:53c4698cf99fa5a401ac9a1788f9a00c4186bb94ca25639e68ba2344958f34ae
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
$ docker pull mono@sha256:2e27adc57339c044a89fb2342fda8870a173a6a6c8e8131a1e89ec3a7ac232e8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94687537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da3a916440f7b6003ed959fff5e81f5d938202484f7a341992557a5fe0f4173e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:48 GMT
ADD file:782d864aa72c2d5fb599311ebae56db4067d2e91ff532c1aaf1a291c3dbce5bb in / 
# Tue, 13 Sep 2022 00:56:49 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 13:18:11 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Sep 2022 13:18:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Sep 2022 13:18:46 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4b7b4a8876e2f677668e51b8473f97a237d3d4df201b9df4031bcaa8068370b1`  
		Last Modified: Tue, 13 Sep 2022 01:01:16 GMT  
		Size: 27.1 MB (27130552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f30d1a79e581bc63843e16797ef34c77d71e42f8dab5b92e7bad411deabcac`  
		Last Modified: Tue, 13 Sep 2022 13:26:22 GMT  
		Size: 2.8 MB (2777658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4b42d23b8e39b264cc02008c057e7def09645acf552e125b3a136fa2ca017a`  
		Last Modified: Tue, 13 Sep 2022 13:26:31 GMT  
		Size: 64.8 MB (64779327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:a8069b8877f03f3a84f1fde543373ea5fa5dd16258ebea604db4d4c0bd927356
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51879108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e2c7afdb95fb0f18db354afb36b56e1fd21cb176fdeafc0f12cc623a1607b20`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:49:37 GMT
ADD file:2ed7ca0d45c68b46a10ae186e8a03f98e72cadfeed17105668f53adf14d31e1f in / 
# Tue, 02 Aug 2022 00:49:38 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:06:21 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 02 Aug 2022 02:06:31 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 02 Aug 2022 02:06:57 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:187ecffbd1e0eae5de6567dff32bd58f28623635657779760c9d9539d6b7cc59`  
		Last Modified: Tue, 02 Aug 2022 00:57:06 GMT  
		Size: 24.9 MB (24889750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d1f7c779aa2742311c359ef531049f9a015701cf53969ec3c0b86bb6ed4d7d`  
		Last Modified: Tue, 02 Aug 2022 02:11:45 GMT  
		Size: 2.5 MB (2467689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e0854b1d2110cdccf321fe15cae0adbd1e734b32a4557490c2c49abd2d66f97`  
		Last Modified: Tue, 02 Aug 2022 02:11:50 GMT  
		Size: 24.5 MB (24521669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:3863383c39eff5563c9b1c3467d7ac2bfc816acd5e8b0ea8864da1facd148c9b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48928456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55e72d8fdbee41778d9f35eddcdede7be88e58087ea39509912186c093c6a9ff`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:43:37 GMT
ADD file:8d67c07b9926dee5d0124e48bd4b5039e6a84fdfe07a9e1077392f0e5772aa52 in / 
# Tue, 23 Aug 2022 01:43:37 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 21:12:04 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 23 Aug 2022 21:12:16 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 23 Aug 2022 21:12:44 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:838efeda083c4fc3f1262c9c56947c82c6fdb90b64993afdb1375ce01ce1724b`  
		Last Modified: Tue, 23 Aug 2022 01:51:00 GMT  
		Size: 22.7 MB (22746698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75d8ba3b02424e687c31e5dd2e4a8e74b8c51b4d0175a81b69735aeebb0e7a52`  
		Last Modified: Tue, 23 Aug 2022 21:17:53 GMT  
		Size: 2.4 MB (2366966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6094a07154b3e0a1af790f2b4281bedb8eda5373688ddf4d7758c78f16865911`  
		Last Modified: Tue, 23 Aug 2022 21:17:58 GMT  
		Size: 23.8 MB (23814792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:20fda12151f0a25e5cc59797c6f085a4dbae2bc9d6d94ed5a76f540babbc0488
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57906694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d598b3fa1997e8f2c1231c6a8851d4cd7fc44e075515af8a5f36f036c868216`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 02:11:20 GMT
ADD file:18fa3591fcbf0c3e065dbe581a069fc2af6fab9e4446047348404881af960725 in / 
# Tue, 13 Sep 2022 02:11:21 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 14:25:55 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Sep 2022 14:26:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Sep 2022 14:26:19 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4c3f5cce277263c7aeaf67f83255af76927e03363e775f39d7587bc5036fcf1e`  
		Last Modified: Tue, 13 Sep 2022 02:17:10 GMT  
		Size: 25.9 MB (25904152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715d7d34ba910bd2b5bd88a1b9746572cd399b1b321eadfb5e9bf89f35f5cf01`  
		Last Modified: Tue, 13 Sep 2022 14:29:27 GMT  
		Size: 2.6 MB (2641345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4865d20ade904a532cc524f8362ec7e259ab3ef39d670cb72e47ce063c303523`  
		Last Modified: Tue, 13 Sep 2022 14:29:32 GMT  
		Size: 29.4 MB (29361197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; 386

```console
$ docker pull mono@sha256:52003ec451d3bb83ca2d41b0ac7dcad9aeb2ba407e0523e2f806c037d0b63e61
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99174593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7e420ca0bef5096adeb782603c753d355ac014c7640c78432be93fe5894d7f8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 01:40:12 GMT
ADD file:da95249e10828562612e8b0a3595f3cbf6a5cb5dbfb47302a4d42a4a8c5025b1 in / 
# Tue, 13 Sep 2022 01:40:12 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:49:20 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Sep 2022 06:49:29 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Sep 2022 06:49:55 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7db2238a0cb6ea85529a33cb395b0243796e76066f31656ba5e08232e2fb0308`  
		Last Modified: Tue, 13 Sep 2022 01:46:12 GMT  
		Size: 27.8 MB (27790952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2f07907e6e47b8f80c60ae70573642fdda80eaa70791e8977fadf5d56a73b6`  
		Last Modified: Tue, 13 Sep 2022 06:54:02 GMT  
		Size: 2.8 MB (2789402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ae77ac5737c4b823e9852bffe8c8ee90553eb251aa3b041c126afd7fc70dec`  
		Last Modified: Tue, 13 Sep 2022 06:54:11 GMT  
		Size: 68.6 MB (68594239 bytes)  
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
$ docker pull mono@sha256:54c927dc76c98d6940d95191939e959bdb1c0b09d688a6eefa525b0b23e02143
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
$ docker pull mono@sha256:da05a83bdf8e682a1384d08f93d96c19241e438d65115bb64a93542368b49033
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.0 MB (225002881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86657b2acd31350e074591d40fed046d95443d90c5d22a4e30889b198d31c655`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:48 GMT
ADD file:782d864aa72c2d5fb599311ebae56db4067d2e91ff532c1aaf1a291c3dbce5bb in / 
# Tue, 13 Sep 2022 00:56:49 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 13:18:11 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Sep 2022 13:18:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Sep 2022 13:18:46 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Sep 2022 13:25:20 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4b7b4a8876e2f677668e51b8473f97a237d3d4df201b9df4031bcaa8068370b1`  
		Last Modified: Tue, 13 Sep 2022 01:01:16 GMT  
		Size: 27.1 MB (27130552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f30d1a79e581bc63843e16797ef34c77d71e42f8dab5b92e7bad411deabcac`  
		Last Modified: Tue, 13 Sep 2022 13:26:22 GMT  
		Size: 2.8 MB (2777658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4b42d23b8e39b264cc02008c057e7def09645acf552e125b3a136fa2ca017a`  
		Last Modified: Tue, 13 Sep 2022 13:26:31 GMT  
		Size: 64.8 MB (64779327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283bc86196f31f839c30c146b3c7128054d25d0e6821c034928eedc5e1e1f46b`  
		Last Modified: Tue, 13 Sep 2022 13:27:56 GMT  
		Size: 130.3 MB (130315344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; arm variant v5

```console
$ docker pull mono@sha256:0222156facf0460ee81820ef7977de4063cd983148f665910c5a49e24e3a7402
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.9 MB (180857422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2104524aaaa5c48fd39ac37bfe94bbeda0086a1ea289e1be14e280f94b1c0c8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:49:37 GMT
ADD file:2ed7ca0d45c68b46a10ae186e8a03f98e72cadfeed17105668f53adf14d31e1f in / 
# Tue, 02 Aug 2022 00:49:38 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:06:21 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 02 Aug 2022 02:06:31 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 02 Aug 2022 02:06:57 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 02 Aug 2022 02:10:28 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:187ecffbd1e0eae5de6567dff32bd58f28623635657779760c9d9539d6b7cc59`  
		Last Modified: Tue, 02 Aug 2022 00:57:06 GMT  
		Size: 24.9 MB (24889750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d1f7c779aa2742311c359ef531049f9a015701cf53969ec3c0b86bb6ed4d7d`  
		Last Modified: Tue, 02 Aug 2022 02:11:45 GMT  
		Size: 2.5 MB (2467689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e0854b1d2110cdccf321fe15cae0adbd1e734b32a4557490c2c49abd2d66f97`  
		Last Modified: Tue, 02 Aug 2022 02:11:50 GMT  
		Size: 24.5 MB (24521669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8006236a82fb24514f586974ded95bdd60e0959951dde202b6113bc760326e`  
		Last Modified: Tue, 02 Aug 2022 02:13:30 GMT  
		Size: 129.0 MB (128978314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; arm variant v7

```console
$ docker pull mono@sha256:37de3b0c33584ae9731b35fe2a5e38402f85f92eac9f77008303773a8f6d9920
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.8 MB (176757012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:227e330c7acb2efbfb2773f807f3860a49e1a3d515fa2984e14681244c767683`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:43:37 GMT
ADD file:8d67c07b9926dee5d0124e48bd4b5039e6a84fdfe07a9e1077392f0e5772aa52 in / 
# Tue, 23 Aug 2022 01:43:37 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 21:12:04 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 23 Aug 2022 21:12:16 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 23 Aug 2022 21:12:44 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 23 Aug 2022 21:16:33 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:838efeda083c4fc3f1262c9c56947c82c6fdb90b64993afdb1375ce01ce1724b`  
		Last Modified: Tue, 23 Aug 2022 01:51:00 GMT  
		Size: 22.7 MB (22746698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75d8ba3b02424e687c31e5dd2e4a8e74b8c51b4d0175a81b69735aeebb0e7a52`  
		Last Modified: Tue, 23 Aug 2022 21:17:53 GMT  
		Size: 2.4 MB (2366966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6094a07154b3e0a1af790f2b4281bedb8eda5373688ddf4d7758c78f16865911`  
		Last Modified: Tue, 23 Aug 2022 21:17:58 GMT  
		Size: 23.8 MB (23814792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9179f457685aedac47e660f0319e528f3aee0892c9cf3ddc4664fd15380d4c7c`  
		Last Modified: Tue, 23 Aug 2022 21:19:38 GMT  
		Size: 127.8 MB (127828556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:212c83e316ac1b28ef0e7b7b7a0072e061383b9bac36dfa231b54dda2b9a0f56
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.4 MB (203357374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c4c0d5dcca91ba6de1291aeb772e7035c4bf4cbf85b03c7b5c1cf1aa4b94b1b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 02:11:20 GMT
ADD file:18fa3591fcbf0c3e065dbe581a069fc2af6fab9e4446047348404881af960725 in / 
# Tue, 13 Sep 2022 02:11:21 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 14:25:55 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Sep 2022 14:26:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Sep 2022 14:26:19 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Sep 2022 14:28:26 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4c3f5cce277263c7aeaf67f83255af76927e03363e775f39d7587bc5036fcf1e`  
		Last Modified: Tue, 13 Sep 2022 02:17:10 GMT  
		Size: 25.9 MB (25904152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715d7d34ba910bd2b5bd88a1b9746572cd399b1b321eadfb5e9bf89f35f5cf01`  
		Last Modified: Tue, 13 Sep 2022 14:29:27 GMT  
		Size: 2.6 MB (2641345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4865d20ade904a532cc524f8362ec7e259ab3ef39d670cb72e47ce063c303523`  
		Last Modified: Tue, 13 Sep 2022 14:29:32 GMT  
		Size: 29.4 MB (29361197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b677a59228f837aadd289b9fdeef07443f81706ae644d4c62532ce8656cfcbd4`  
		Last Modified: Tue, 13 Sep 2022 14:30:52 GMT  
		Size: 145.5 MB (145450680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; 386

```console
$ docker pull mono@sha256:667dfaee00f413dea2417bb04680f0a5de4328515ab45ee2e4dc0c41269b278f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.6 MB (230595906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a8e479ba8c4dc385ee6f4c11f741d9587bd697e143f659af9c0ad81c27ef9a0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 01:40:12 GMT
ADD file:da95249e10828562612e8b0a3595f3cbf6a5cb5dbfb47302a4d42a4a8c5025b1 in / 
# Tue, 13 Sep 2022 01:40:12 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:49:20 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Sep 2022 06:49:29 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Sep 2022 06:49:55 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Sep 2022 06:52:39 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7db2238a0cb6ea85529a33cb395b0243796e76066f31656ba5e08232e2fb0308`  
		Last Modified: Tue, 13 Sep 2022 01:46:12 GMT  
		Size: 27.8 MB (27790952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2f07907e6e47b8f80c60ae70573642fdda80eaa70791e8977fadf5d56a73b6`  
		Last Modified: Tue, 13 Sep 2022 06:54:02 GMT  
		Size: 2.8 MB (2789402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ae77ac5737c4b823e9852bffe8c8ee90553eb251aa3b041c126afd7fc70dec`  
		Last Modified: Tue, 13 Sep 2022 06:54:11 GMT  
		Size: 68.6 MB (68594239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74689d9182ad76725ecab8ec2fec0741718d4acf1087aaec4e464598dee7529`  
		Last Modified: Tue, 13 Sep 2022 06:55:25 GMT  
		Size: 131.4 MB (131421313 bytes)  
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
$ docker pull mono@sha256:53c4698cf99fa5a401ac9a1788f9a00c4186bb94ca25639e68ba2344958f34ae
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
$ docker pull mono@sha256:2e27adc57339c044a89fb2342fda8870a173a6a6c8e8131a1e89ec3a7ac232e8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94687537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da3a916440f7b6003ed959fff5e81f5d938202484f7a341992557a5fe0f4173e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:48 GMT
ADD file:782d864aa72c2d5fb599311ebae56db4067d2e91ff532c1aaf1a291c3dbce5bb in / 
# Tue, 13 Sep 2022 00:56:49 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 13:18:11 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Sep 2022 13:18:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Sep 2022 13:18:46 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4b7b4a8876e2f677668e51b8473f97a237d3d4df201b9df4031bcaa8068370b1`  
		Last Modified: Tue, 13 Sep 2022 01:01:16 GMT  
		Size: 27.1 MB (27130552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f30d1a79e581bc63843e16797ef34c77d71e42f8dab5b92e7bad411deabcac`  
		Last Modified: Tue, 13 Sep 2022 13:26:22 GMT  
		Size: 2.8 MB (2777658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4b42d23b8e39b264cc02008c057e7def09645acf552e125b3a136fa2ca017a`  
		Last Modified: Tue, 13 Sep 2022 13:26:31 GMT  
		Size: 64.8 MB (64779327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:a8069b8877f03f3a84f1fde543373ea5fa5dd16258ebea604db4d4c0bd927356
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51879108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e2c7afdb95fb0f18db354afb36b56e1fd21cb176fdeafc0f12cc623a1607b20`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:49:37 GMT
ADD file:2ed7ca0d45c68b46a10ae186e8a03f98e72cadfeed17105668f53adf14d31e1f in / 
# Tue, 02 Aug 2022 00:49:38 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:06:21 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 02 Aug 2022 02:06:31 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 02 Aug 2022 02:06:57 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:187ecffbd1e0eae5de6567dff32bd58f28623635657779760c9d9539d6b7cc59`  
		Last Modified: Tue, 02 Aug 2022 00:57:06 GMT  
		Size: 24.9 MB (24889750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d1f7c779aa2742311c359ef531049f9a015701cf53969ec3c0b86bb6ed4d7d`  
		Last Modified: Tue, 02 Aug 2022 02:11:45 GMT  
		Size: 2.5 MB (2467689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e0854b1d2110cdccf321fe15cae0adbd1e734b32a4557490c2c49abd2d66f97`  
		Last Modified: Tue, 02 Aug 2022 02:11:50 GMT  
		Size: 24.5 MB (24521669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:3863383c39eff5563c9b1c3467d7ac2bfc816acd5e8b0ea8864da1facd148c9b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48928456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55e72d8fdbee41778d9f35eddcdede7be88e58087ea39509912186c093c6a9ff`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:43:37 GMT
ADD file:8d67c07b9926dee5d0124e48bd4b5039e6a84fdfe07a9e1077392f0e5772aa52 in / 
# Tue, 23 Aug 2022 01:43:37 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 21:12:04 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 23 Aug 2022 21:12:16 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 23 Aug 2022 21:12:44 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:838efeda083c4fc3f1262c9c56947c82c6fdb90b64993afdb1375ce01ce1724b`  
		Last Modified: Tue, 23 Aug 2022 01:51:00 GMT  
		Size: 22.7 MB (22746698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75d8ba3b02424e687c31e5dd2e4a8e74b8c51b4d0175a81b69735aeebb0e7a52`  
		Last Modified: Tue, 23 Aug 2022 21:17:53 GMT  
		Size: 2.4 MB (2366966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6094a07154b3e0a1af790f2b4281bedb8eda5373688ddf4d7758c78f16865911`  
		Last Modified: Tue, 23 Aug 2022 21:17:58 GMT  
		Size: 23.8 MB (23814792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:20fda12151f0a25e5cc59797c6f085a4dbae2bc9d6d94ed5a76f540babbc0488
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57906694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d598b3fa1997e8f2c1231c6a8851d4cd7fc44e075515af8a5f36f036c868216`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 02:11:20 GMT
ADD file:18fa3591fcbf0c3e065dbe581a069fc2af6fab9e4446047348404881af960725 in / 
# Tue, 13 Sep 2022 02:11:21 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 14:25:55 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Sep 2022 14:26:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Sep 2022 14:26:19 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4c3f5cce277263c7aeaf67f83255af76927e03363e775f39d7587bc5036fcf1e`  
		Last Modified: Tue, 13 Sep 2022 02:17:10 GMT  
		Size: 25.9 MB (25904152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715d7d34ba910bd2b5bd88a1b9746572cd399b1b321eadfb5e9bf89f35f5cf01`  
		Last Modified: Tue, 13 Sep 2022 14:29:27 GMT  
		Size: 2.6 MB (2641345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4865d20ade904a532cc524f8362ec7e259ab3ef39d670cb72e47ce063c303523`  
		Last Modified: Tue, 13 Sep 2022 14:29:32 GMT  
		Size: 29.4 MB (29361197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; 386

```console
$ docker pull mono@sha256:52003ec451d3bb83ca2d41b0ac7dcad9aeb2ba407e0523e2f806c037d0b63e61
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99174593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7e420ca0bef5096adeb782603c753d355ac014c7640c78432be93fe5894d7f8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 01:40:12 GMT
ADD file:da95249e10828562612e8b0a3595f3cbf6a5cb5dbfb47302a4d42a4a8c5025b1 in / 
# Tue, 13 Sep 2022 01:40:12 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:49:20 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Sep 2022 06:49:29 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Sep 2022 06:49:55 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7db2238a0cb6ea85529a33cb395b0243796e76066f31656ba5e08232e2fb0308`  
		Last Modified: Tue, 13 Sep 2022 01:46:12 GMT  
		Size: 27.8 MB (27790952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2f07907e6e47b8f80c60ae70573642fdda80eaa70791e8977fadf5d56a73b6`  
		Last Modified: Tue, 13 Sep 2022 06:54:02 GMT  
		Size: 2.8 MB (2789402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ae77ac5737c4b823e9852bffe8c8ee90553eb251aa3b041c126afd7fc70dec`  
		Last Modified: Tue, 13 Sep 2022 06:54:11 GMT  
		Size: 68.6 MB (68594239 bytes)  
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
$ docker pull mono@sha256:54c927dc76c98d6940d95191939e959bdb1c0b09d688a6eefa525b0b23e02143
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
$ docker pull mono@sha256:da05a83bdf8e682a1384d08f93d96c19241e438d65115bb64a93542368b49033
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.0 MB (225002881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86657b2acd31350e074591d40fed046d95443d90c5d22a4e30889b198d31c655`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:48 GMT
ADD file:782d864aa72c2d5fb599311ebae56db4067d2e91ff532c1aaf1a291c3dbce5bb in / 
# Tue, 13 Sep 2022 00:56:49 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 13:18:11 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Sep 2022 13:18:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Sep 2022 13:18:46 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Sep 2022 13:25:20 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4b7b4a8876e2f677668e51b8473f97a237d3d4df201b9df4031bcaa8068370b1`  
		Last Modified: Tue, 13 Sep 2022 01:01:16 GMT  
		Size: 27.1 MB (27130552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f30d1a79e581bc63843e16797ef34c77d71e42f8dab5b92e7bad411deabcac`  
		Last Modified: Tue, 13 Sep 2022 13:26:22 GMT  
		Size: 2.8 MB (2777658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4b42d23b8e39b264cc02008c057e7def09645acf552e125b3a136fa2ca017a`  
		Last Modified: Tue, 13 Sep 2022 13:26:31 GMT  
		Size: 64.8 MB (64779327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283bc86196f31f839c30c146b3c7128054d25d0e6821c034928eedc5e1e1f46b`  
		Last Modified: Tue, 13 Sep 2022 13:27:56 GMT  
		Size: 130.3 MB (130315344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; arm variant v5

```console
$ docker pull mono@sha256:0222156facf0460ee81820ef7977de4063cd983148f665910c5a49e24e3a7402
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.9 MB (180857422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2104524aaaa5c48fd39ac37bfe94bbeda0086a1ea289e1be14e280f94b1c0c8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:49:37 GMT
ADD file:2ed7ca0d45c68b46a10ae186e8a03f98e72cadfeed17105668f53adf14d31e1f in / 
# Tue, 02 Aug 2022 00:49:38 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:06:21 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 02 Aug 2022 02:06:31 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 02 Aug 2022 02:06:57 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 02 Aug 2022 02:10:28 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:187ecffbd1e0eae5de6567dff32bd58f28623635657779760c9d9539d6b7cc59`  
		Last Modified: Tue, 02 Aug 2022 00:57:06 GMT  
		Size: 24.9 MB (24889750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d1f7c779aa2742311c359ef531049f9a015701cf53969ec3c0b86bb6ed4d7d`  
		Last Modified: Tue, 02 Aug 2022 02:11:45 GMT  
		Size: 2.5 MB (2467689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e0854b1d2110cdccf321fe15cae0adbd1e734b32a4557490c2c49abd2d66f97`  
		Last Modified: Tue, 02 Aug 2022 02:11:50 GMT  
		Size: 24.5 MB (24521669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8006236a82fb24514f586974ded95bdd60e0959951dde202b6113bc760326e`  
		Last Modified: Tue, 02 Aug 2022 02:13:30 GMT  
		Size: 129.0 MB (128978314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; arm variant v7

```console
$ docker pull mono@sha256:37de3b0c33584ae9731b35fe2a5e38402f85f92eac9f77008303773a8f6d9920
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.8 MB (176757012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:227e330c7acb2efbfb2773f807f3860a49e1a3d515fa2984e14681244c767683`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:43:37 GMT
ADD file:8d67c07b9926dee5d0124e48bd4b5039e6a84fdfe07a9e1077392f0e5772aa52 in / 
# Tue, 23 Aug 2022 01:43:37 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 21:12:04 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 23 Aug 2022 21:12:16 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 23 Aug 2022 21:12:44 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 23 Aug 2022 21:16:33 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:838efeda083c4fc3f1262c9c56947c82c6fdb90b64993afdb1375ce01ce1724b`  
		Last Modified: Tue, 23 Aug 2022 01:51:00 GMT  
		Size: 22.7 MB (22746698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75d8ba3b02424e687c31e5dd2e4a8e74b8c51b4d0175a81b69735aeebb0e7a52`  
		Last Modified: Tue, 23 Aug 2022 21:17:53 GMT  
		Size: 2.4 MB (2366966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6094a07154b3e0a1af790f2b4281bedb8eda5373688ddf4d7758c78f16865911`  
		Last Modified: Tue, 23 Aug 2022 21:17:58 GMT  
		Size: 23.8 MB (23814792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9179f457685aedac47e660f0319e528f3aee0892c9cf3ddc4664fd15380d4c7c`  
		Last Modified: Tue, 23 Aug 2022 21:19:38 GMT  
		Size: 127.8 MB (127828556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:212c83e316ac1b28ef0e7b7b7a0072e061383b9bac36dfa231b54dda2b9a0f56
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.4 MB (203357374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c4c0d5dcca91ba6de1291aeb772e7035c4bf4cbf85b03c7b5c1cf1aa4b94b1b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 02:11:20 GMT
ADD file:18fa3591fcbf0c3e065dbe581a069fc2af6fab9e4446047348404881af960725 in / 
# Tue, 13 Sep 2022 02:11:21 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 14:25:55 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Sep 2022 14:26:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Sep 2022 14:26:19 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Sep 2022 14:28:26 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4c3f5cce277263c7aeaf67f83255af76927e03363e775f39d7587bc5036fcf1e`  
		Last Modified: Tue, 13 Sep 2022 02:17:10 GMT  
		Size: 25.9 MB (25904152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715d7d34ba910bd2b5bd88a1b9746572cd399b1b321eadfb5e9bf89f35f5cf01`  
		Last Modified: Tue, 13 Sep 2022 14:29:27 GMT  
		Size: 2.6 MB (2641345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4865d20ade904a532cc524f8362ec7e259ab3ef39d670cb72e47ce063c303523`  
		Last Modified: Tue, 13 Sep 2022 14:29:32 GMT  
		Size: 29.4 MB (29361197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b677a59228f837aadd289b9fdeef07443f81706ae644d4c62532ce8656cfcbd4`  
		Last Modified: Tue, 13 Sep 2022 14:30:52 GMT  
		Size: 145.5 MB (145450680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; 386

```console
$ docker pull mono@sha256:667dfaee00f413dea2417bb04680f0a5de4328515ab45ee2e4dc0c41269b278f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.6 MB (230595906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a8e479ba8c4dc385ee6f4c11f741d9587bd697e143f659af9c0ad81c27ef9a0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 01:40:12 GMT
ADD file:da95249e10828562612e8b0a3595f3cbf6a5cb5dbfb47302a4d42a4a8c5025b1 in / 
# Tue, 13 Sep 2022 01:40:12 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:49:20 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Sep 2022 06:49:29 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Sep 2022 06:49:55 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Sep 2022 06:52:39 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7db2238a0cb6ea85529a33cb395b0243796e76066f31656ba5e08232e2fb0308`  
		Last Modified: Tue, 13 Sep 2022 01:46:12 GMT  
		Size: 27.8 MB (27790952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2f07907e6e47b8f80c60ae70573642fdda80eaa70791e8977fadf5d56a73b6`  
		Last Modified: Tue, 13 Sep 2022 06:54:02 GMT  
		Size: 2.8 MB (2789402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ae77ac5737c4b823e9852bffe8c8ee90553eb251aa3b041c126afd7fc70dec`  
		Last Modified: Tue, 13 Sep 2022 06:54:11 GMT  
		Size: 68.6 MB (68594239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74689d9182ad76725ecab8ec2fec0741718d4acf1087aaec4e464598dee7529`  
		Last Modified: Tue, 13 Sep 2022 06:55:25 GMT  
		Size: 131.4 MB (131421313 bytes)  
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
$ docker pull mono@sha256:53c4698cf99fa5a401ac9a1788f9a00c4186bb94ca25639e68ba2344958f34ae
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
$ docker pull mono@sha256:2e27adc57339c044a89fb2342fda8870a173a6a6c8e8131a1e89ec3a7ac232e8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94687537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da3a916440f7b6003ed959fff5e81f5d938202484f7a341992557a5fe0f4173e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:48 GMT
ADD file:782d864aa72c2d5fb599311ebae56db4067d2e91ff532c1aaf1a291c3dbce5bb in / 
# Tue, 13 Sep 2022 00:56:49 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 13:18:11 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Sep 2022 13:18:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Sep 2022 13:18:46 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4b7b4a8876e2f677668e51b8473f97a237d3d4df201b9df4031bcaa8068370b1`  
		Last Modified: Tue, 13 Sep 2022 01:01:16 GMT  
		Size: 27.1 MB (27130552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f30d1a79e581bc63843e16797ef34c77d71e42f8dab5b92e7bad411deabcac`  
		Last Modified: Tue, 13 Sep 2022 13:26:22 GMT  
		Size: 2.8 MB (2777658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4b42d23b8e39b264cc02008c057e7def09645acf552e125b3a136fa2ca017a`  
		Last Modified: Tue, 13 Sep 2022 13:26:31 GMT  
		Size: 64.8 MB (64779327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:a8069b8877f03f3a84f1fde543373ea5fa5dd16258ebea604db4d4c0bd927356
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51879108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e2c7afdb95fb0f18db354afb36b56e1fd21cb176fdeafc0f12cc623a1607b20`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:49:37 GMT
ADD file:2ed7ca0d45c68b46a10ae186e8a03f98e72cadfeed17105668f53adf14d31e1f in / 
# Tue, 02 Aug 2022 00:49:38 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:06:21 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 02 Aug 2022 02:06:31 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 02 Aug 2022 02:06:57 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:187ecffbd1e0eae5de6567dff32bd58f28623635657779760c9d9539d6b7cc59`  
		Last Modified: Tue, 02 Aug 2022 00:57:06 GMT  
		Size: 24.9 MB (24889750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d1f7c779aa2742311c359ef531049f9a015701cf53969ec3c0b86bb6ed4d7d`  
		Last Modified: Tue, 02 Aug 2022 02:11:45 GMT  
		Size: 2.5 MB (2467689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e0854b1d2110cdccf321fe15cae0adbd1e734b32a4557490c2c49abd2d66f97`  
		Last Modified: Tue, 02 Aug 2022 02:11:50 GMT  
		Size: 24.5 MB (24521669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:3863383c39eff5563c9b1c3467d7ac2bfc816acd5e8b0ea8864da1facd148c9b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48928456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55e72d8fdbee41778d9f35eddcdede7be88e58087ea39509912186c093c6a9ff`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:43:37 GMT
ADD file:8d67c07b9926dee5d0124e48bd4b5039e6a84fdfe07a9e1077392f0e5772aa52 in / 
# Tue, 23 Aug 2022 01:43:37 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 21:12:04 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 23 Aug 2022 21:12:16 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 23 Aug 2022 21:12:44 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:838efeda083c4fc3f1262c9c56947c82c6fdb90b64993afdb1375ce01ce1724b`  
		Last Modified: Tue, 23 Aug 2022 01:51:00 GMT  
		Size: 22.7 MB (22746698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75d8ba3b02424e687c31e5dd2e4a8e74b8c51b4d0175a81b69735aeebb0e7a52`  
		Last Modified: Tue, 23 Aug 2022 21:17:53 GMT  
		Size: 2.4 MB (2366966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6094a07154b3e0a1af790f2b4281bedb8eda5373688ddf4d7758c78f16865911`  
		Last Modified: Tue, 23 Aug 2022 21:17:58 GMT  
		Size: 23.8 MB (23814792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:20fda12151f0a25e5cc59797c6f085a4dbae2bc9d6d94ed5a76f540babbc0488
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57906694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d598b3fa1997e8f2c1231c6a8851d4cd7fc44e075515af8a5f36f036c868216`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 02:11:20 GMT
ADD file:18fa3591fcbf0c3e065dbe581a069fc2af6fab9e4446047348404881af960725 in / 
# Tue, 13 Sep 2022 02:11:21 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 14:25:55 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Sep 2022 14:26:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Sep 2022 14:26:19 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4c3f5cce277263c7aeaf67f83255af76927e03363e775f39d7587bc5036fcf1e`  
		Last Modified: Tue, 13 Sep 2022 02:17:10 GMT  
		Size: 25.9 MB (25904152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715d7d34ba910bd2b5bd88a1b9746572cd399b1b321eadfb5e9bf89f35f5cf01`  
		Last Modified: Tue, 13 Sep 2022 14:29:27 GMT  
		Size: 2.6 MB (2641345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4865d20ade904a532cc524f8362ec7e259ab3ef39d670cb72e47ce063c303523`  
		Last Modified: Tue, 13 Sep 2022 14:29:32 GMT  
		Size: 29.4 MB (29361197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; 386

```console
$ docker pull mono@sha256:52003ec451d3bb83ca2d41b0ac7dcad9aeb2ba407e0523e2f806c037d0b63e61
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99174593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7e420ca0bef5096adeb782603c753d355ac014c7640c78432be93fe5894d7f8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 01:40:12 GMT
ADD file:da95249e10828562612e8b0a3595f3cbf6a5cb5dbfb47302a4d42a4a8c5025b1 in / 
# Tue, 13 Sep 2022 01:40:12 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:49:20 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Sep 2022 06:49:29 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Sep 2022 06:49:55 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7db2238a0cb6ea85529a33cb395b0243796e76066f31656ba5e08232e2fb0308`  
		Last Modified: Tue, 13 Sep 2022 01:46:12 GMT  
		Size: 27.8 MB (27790952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2f07907e6e47b8f80c60ae70573642fdda80eaa70791e8977fadf5d56a73b6`  
		Last Modified: Tue, 13 Sep 2022 06:54:02 GMT  
		Size: 2.8 MB (2789402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ae77ac5737c4b823e9852bffe8c8ee90553eb251aa3b041c126afd7fc70dec`  
		Last Modified: Tue, 13 Sep 2022 06:54:11 GMT  
		Size: 68.6 MB (68594239 bytes)  
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
$ docker pull mono@sha256:b34a1b1b205c78b01e44fcf6b5155308e83c6c357977fd5e7026eff7407de026
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

### `mono:6.12` - linux; arm variant v5

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

### `mono:6.12` - linux; arm variant v7

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

### `mono:6.12` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:fd4938ac21581458b75a7f3513bae5635920c5e027861498324557d8f88cdee9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.9 MB (215898442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f85bcf336e06b49a2ce77e7f49b7d8f28c4983260055e62d8dd47624f239b723`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 02:11:20 GMT
ADD file:18fa3591fcbf0c3e065dbe581a069fc2af6fab9e4446047348404881af960725 in / 
# Tue, 13 Sep 2022 02:11:21 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 14:25:23 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 13 Sep 2022 14:25:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Sep 2022 14:25:47 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Sep 2022 14:27:23 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4c3f5cce277263c7aeaf67f83255af76927e03363e775f39d7587bc5036fcf1e`  
		Last Modified: Tue, 13 Sep 2022 02:17:10 GMT  
		Size: 25.9 MB (25904152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf1bcd765746fb733fe53109f7f09254547fc14af9cd08cfebb1fe80289a004`  
		Last Modified: Tue, 13 Sep 2022 14:29:03 GMT  
		Size: 2.6 MB (2641320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eedb38f3cdc2b7d72d243d8f80d986fc8c5722148df30f2b6ac2b9019f7e3b9`  
		Last Modified: Tue, 13 Sep 2022 14:29:08 GMT  
		Size: 29.3 MB (29333406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b50613517341b9dd3da923e0cec24f35044bf3377544ce59b470cf0ab35e993`  
		Last Modified: Tue, 13 Sep 2022 14:30:10 GMT  
		Size: 158.0 MB (158019564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12` - linux; 386

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
$ docker pull mono@sha256:406d40ad3587b24cbf640473398da229a4577dbfff5f5ab8dd88e9b2b27d8a8a
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
$ docker pull mono@sha256:43e21877587c21a125ba97d474435087e87de3e0d19a5fb59226814a2ed4a556
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94681096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36f89a89c017304e116d9818f24b08de656e3841a6a7f587c8c5bc2b0228d6b8`
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

### `mono:6.12-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:3d36decf8882609bab164b6571c9e1975e4cd53e07ac0a376f9a774febc45c74
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51860738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5251c1b1cc35b1d2cb554f30f5b2f12a90a53f3472b1fc7839dfa91530021631`
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

### `mono:6.12-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:fb09f2f2c204a4635c74bd5a95114ed9d5dc7fd180c0050b0c25f32b8c989e49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48903169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e602747f8e64b4af84f3c87450b816d181ac4abd009c3255a96a56b0c58bde14`
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

### `mono:6.12-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:2aa229cb03c6549b44b14e24b115dccd2106ef10afc95f66529a8f90f9da5fb3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57878878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91be6728a6a5d81c6dfb3c13b2340ad35f6611dad08c35bf6640d49bbb9db356`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 02:11:20 GMT
ADD file:18fa3591fcbf0c3e065dbe581a069fc2af6fab9e4446047348404881af960725 in / 
# Tue, 13 Sep 2022 02:11:21 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 14:25:23 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 13 Sep 2022 14:25:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Sep 2022 14:25:47 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4c3f5cce277263c7aeaf67f83255af76927e03363e775f39d7587bc5036fcf1e`  
		Last Modified: Tue, 13 Sep 2022 02:17:10 GMT  
		Size: 25.9 MB (25904152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf1bcd765746fb733fe53109f7f09254547fc14af9cd08cfebb1fe80289a004`  
		Last Modified: Tue, 13 Sep 2022 14:29:03 GMT  
		Size: 2.6 MB (2641320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eedb38f3cdc2b7d72d243d8f80d986fc8c5722148df30f2b6ac2b9019f7e3b9`  
		Last Modified: Tue, 13 Sep 2022 14:29:08 GMT  
		Size: 29.3 MB (29333406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12-slim` - linux; 386

```console
$ docker pull mono@sha256:8ef911eede2000787ec9614d4147d27fd3cc3cff7299098645d2c331ff5000ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99166506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a06eb501431fb5c4a879cdedfba520528fb72e991ce30c46d974238e2103341`
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
$ docker pull mono@sha256:b34a1b1b205c78b01e44fcf6b5155308e83c6c357977fd5e7026eff7407de026
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

### `mono:6.12.0` - linux; arm variant v5

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

### `mono:6.12.0` - linux; arm variant v7

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

### `mono:6.12.0` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:fd4938ac21581458b75a7f3513bae5635920c5e027861498324557d8f88cdee9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.9 MB (215898442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f85bcf336e06b49a2ce77e7f49b7d8f28c4983260055e62d8dd47624f239b723`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 02:11:20 GMT
ADD file:18fa3591fcbf0c3e065dbe581a069fc2af6fab9e4446047348404881af960725 in / 
# Tue, 13 Sep 2022 02:11:21 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 14:25:23 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 13 Sep 2022 14:25:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Sep 2022 14:25:47 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Sep 2022 14:27:23 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4c3f5cce277263c7aeaf67f83255af76927e03363e775f39d7587bc5036fcf1e`  
		Last Modified: Tue, 13 Sep 2022 02:17:10 GMT  
		Size: 25.9 MB (25904152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf1bcd765746fb733fe53109f7f09254547fc14af9cd08cfebb1fe80289a004`  
		Last Modified: Tue, 13 Sep 2022 14:29:03 GMT  
		Size: 2.6 MB (2641320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eedb38f3cdc2b7d72d243d8f80d986fc8c5722148df30f2b6ac2b9019f7e3b9`  
		Last Modified: Tue, 13 Sep 2022 14:29:08 GMT  
		Size: 29.3 MB (29333406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b50613517341b9dd3da923e0cec24f35044bf3377544ce59b470cf0ab35e993`  
		Last Modified: Tue, 13 Sep 2022 14:30:10 GMT  
		Size: 158.0 MB (158019564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0` - linux; 386

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
$ docker pull mono@sha256:406d40ad3587b24cbf640473398da229a4577dbfff5f5ab8dd88e9b2b27d8a8a
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
$ docker pull mono@sha256:43e21877587c21a125ba97d474435087e87de3e0d19a5fb59226814a2ed4a556
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94681096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36f89a89c017304e116d9818f24b08de656e3841a6a7f587c8c5bc2b0228d6b8`
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

### `mono:6.12.0-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:3d36decf8882609bab164b6571c9e1975e4cd53e07ac0a376f9a774febc45c74
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51860738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5251c1b1cc35b1d2cb554f30f5b2f12a90a53f3472b1fc7839dfa91530021631`
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

### `mono:6.12.0-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:fb09f2f2c204a4635c74bd5a95114ed9d5dc7fd180c0050b0c25f32b8c989e49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48903169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e602747f8e64b4af84f3c87450b816d181ac4abd009c3255a96a56b0c58bde14`
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

### `mono:6.12.0-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:2aa229cb03c6549b44b14e24b115dccd2106ef10afc95f66529a8f90f9da5fb3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57878878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91be6728a6a5d81c6dfb3c13b2340ad35f6611dad08c35bf6640d49bbb9db356`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 02:11:20 GMT
ADD file:18fa3591fcbf0c3e065dbe581a069fc2af6fab9e4446047348404881af960725 in / 
# Tue, 13 Sep 2022 02:11:21 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 14:25:23 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 13 Sep 2022 14:25:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Sep 2022 14:25:47 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4c3f5cce277263c7aeaf67f83255af76927e03363e775f39d7587bc5036fcf1e`  
		Last Modified: Tue, 13 Sep 2022 02:17:10 GMT  
		Size: 25.9 MB (25904152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf1bcd765746fb733fe53109f7f09254547fc14af9cd08cfebb1fe80289a004`  
		Last Modified: Tue, 13 Sep 2022 14:29:03 GMT  
		Size: 2.6 MB (2641320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eedb38f3cdc2b7d72d243d8f80d986fc8c5722148df30f2b6ac2b9019f7e3b9`  
		Last Modified: Tue, 13 Sep 2022 14:29:08 GMT  
		Size: 29.3 MB (29333406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0-slim` - linux; 386

```console
$ docker pull mono@sha256:8ef911eede2000787ec9614d4147d27fd3cc3cff7299098645d2c331ff5000ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99166506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a06eb501431fb5c4a879cdedfba520528fb72e991ce30c46d974238e2103341`
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
$ docker pull mono@sha256:b34a1b1b205c78b01e44fcf6b5155308e83c6c357977fd5e7026eff7407de026
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

### `mono:6.12.0.182` - linux; arm variant v5

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

### `mono:6.12.0.182` - linux; arm variant v7

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

### `mono:6.12.0.182` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:fd4938ac21581458b75a7f3513bae5635920c5e027861498324557d8f88cdee9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.9 MB (215898442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f85bcf336e06b49a2ce77e7f49b7d8f28c4983260055e62d8dd47624f239b723`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 02:11:20 GMT
ADD file:18fa3591fcbf0c3e065dbe581a069fc2af6fab9e4446047348404881af960725 in / 
# Tue, 13 Sep 2022 02:11:21 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 14:25:23 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 13 Sep 2022 14:25:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Sep 2022 14:25:47 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Sep 2022 14:27:23 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4c3f5cce277263c7aeaf67f83255af76927e03363e775f39d7587bc5036fcf1e`  
		Last Modified: Tue, 13 Sep 2022 02:17:10 GMT  
		Size: 25.9 MB (25904152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf1bcd765746fb733fe53109f7f09254547fc14af9cd08cfebb1fe80289a004`  
		Last Modified: Tue, 13 Sep 2022 14:29:03 GMT  
		Size: 2.6 MB (2641320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eedb38f3cdc2b7d72d243d8f80d986fc8c5722148df30f2b6ac2b9019f7e3b9`  
		Last Modified: Tue, 13 Sep 2022 14:29:08 GMT  
		Size: 29.3 MB (29333406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b50613517341b9dd3da923e0cec24f35044bf3377544ce59b470cf0ab35e993`  
		Last Modified: Tue, 13 Sep 2022 14:30:10 GMT  
		Size: 158.0 MB (158019564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.182` - linux; 386

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
$ docker pull mono@sha256:406d40ad3587b24cbf640473398da229a4577dbfff5f5ab8dd88e9b2b27d8a8a
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
$ docker pull mono@sha256:43e21877587c21a125ba97d474435087e87de3e0d19a5fb59226814a2ed4a556
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94681096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36f89a89c017304e116d9818f24b08de656e3841a6a7f587c8c5bc2b0228d6b8`
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

### `mono:6.12.0.182-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:3d36decf8882609bab164b6571c9e1975e4cd53e07ac0a376f9a774febc45c74
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51860738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5251c1b1cc35b1d2cb554f30f5b2f12a90a53f3472b1fc7839dfa91530021631`
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

### `mono:6.12.0.182-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:fb09f2f2c204a4635c74bd5a95114ed9d5dc7fd180c0050b0c25f32b8c989e49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48903169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e602747f8e64b4af84f3c87450b816d181ac4abd009c3255a96a56b0c58bde14`
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

### `mono:6.12.0.182-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:2aa229cb03c6549b44b14e24b115dccd2106ef10afc95f66529a8f90f9da5fb3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57878878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91be6728a6a5d81c6dfb3c13b2340ad35f6611dad08c35bf6640d49bbb9db356`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 02:11:20 GMT
ADD file:18fa3591fcbf0c3e065dbe581a069fc2af6fab9e4446047348404881af960725 in / 
# Tue, 13 Sep 2022 02:11:21 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 14:25:23 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 13 Sep 2022 14:25:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Sep 2022 14:25:47 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4c3f5cce277263c7aeaf67f83255af76927e03363e775f39d7587bc5036fcf1e`  
		Last Modified: Tue, 13 Sep 2022 02:17:10 GMT  
		Size: 25.9 MB (25904152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf1bcd765746fb733fe53109f7f09254547fc14af9cd08cfebb1fe80289a004`  
		Last Modified: Tue, 13 Sep 2022 14:29:03 GMT  
		Size: 2.6 MB (2641320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eedb38f3cdc2b7d72d243d8f80d986fc8c5722148df30f2b6ac2b9019f7e3b9`  
		Last Modified: Tue, 13 Sep 2022 14:29:08 GMT  
		Size: 29.3 MB (29333406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.182-slim` - linux; 386

```console
$ docker pull mono@sha256:8ef911eede2000787ec9614d4147d27fd3cc3cff7299098645d2c331ff5000ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99166506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a06eb501431fb5c4a879cdedfba520528fb72e991ce30c46d974238e2103341`
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
$ docker pull mono@sha256:b34a1b1b205c78b01e44fcf6b5155308e83c6c357977fd5e7026eff7407de026
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
$ docker pull mono@sha256:fd4938ac21581458b75a7f3513bae5635920c5e027861498324557d8f88cdee9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.9 MB (215898442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f85bcf336e06b49a2ce77e7f49b7d8f28c4983260055e62d8dd47624f239b723`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 02:11:20 GMT
ADD file:18fa3591fcbf0c3e065dbe581a069fc2af6fab9e4446047348404881af960725 in / 
# Tue, 13 Sep 2022 02:11:21 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 14:25:23 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 13 Sep 2022 14:25:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Sep 2022 14:25:47 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Sep 2022 14:27:23 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4c3f5cce277263c7aeaf67f83255af76927e03363e775f39d7587bc5036fcf1e`  
		Last Modified: Tue, 13 Sep 2022 02:17:10 GMT  
		Size: 25.9 MB (25904152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf1bcd765746fb733fe53109f7f09254547fc14af9cd08cfebb1fe80289a004`  
		Last Modified: Tue, 13 Sep 2022 14:29:03 GMT  
		Size: 2.6 MB (2641320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eedb38f3cdc2b7d72d243d8f80d986fc8c5722148df30f2b6ac2b9019f7e3b9`  
		Last Modified: Tue, 13 Sep 2022 14:29:08 GMT  
		Size: 29.3 MB (29333406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b50613517341b9dd3da923e0cec24f35044bf3377544ce59b470cf0ab35e993`  
		Last Modified: Tue, 13 Sep 2022 14:30:10 GMT  
		Size: 158.0 MB (158019564 bytes)  
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

## `mono:slim`

```console
$ docker pull mono@sha256:406d40ad3587b24cbf640473398da229a4577dbfff5f5ab8dd88e9b2b27d8a8a
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
$ docker pull mono@sha256:43e21877587c21a125ba97d474435087e87de3e0d19a5fb59226814a2ed4a556
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94681096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36f89a89c017304e116d9818f24b08de656e3841a6a7f587c8c5bc2b0228d6b8`
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

### `mono:slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:3d36decf8882609bab164b6571c9e1975e4cd53e07ac0a376f9a774febc45c74
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51860738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5251c1b1cc35b1d2cb554f30f5b2f12a90a53f3472b1fc7839dfa91530021631`
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

### `mono:slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:fb09f2f2c204a4635c74bd5a95114ed9d5dc7fd180c0050b0c25f32b8c989e49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48903169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e602747f8e64b4af84f3c87450b816d181ac4abd009c3255a96a56b0c58bde14`
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

### `mono:slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:2aa229cb03c6549b44b14e24b115dccd2106ef10afc95f66529a8f90f9da5fb3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57878878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91be6728a6a5d81c6dfb3c13b2340ad35f6611dad08c35bf6640d49bbb9db356`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 02:11:20 GMT
ADD file:18fa3591fcbf0c3e065dbe581a069fc2af6fab9e4446047348404881af960725 in / 
# Tue, 13 Sep 2022 02:11:21 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 14:25:23 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 13 Sep 2022 14:25:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Sep 2022 14:25:47 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4c3f5cce277263c7aeaf67f83255af76927e03363e775f39d7587bc5036fcf1e`  
		Last Modified: Tue, 13 Sep 2022 02:17:10 GMT  
		Size: 25.9 MB (25904152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf1bcd765746fb733fe53109f7f09254547fc14af9cd08cfebb1fe80289a004`  
		Last Modified: Tue, 13 Sep 2022 14:29:03 GMT  
		Size: 2.6 MB (2641320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eedb38f3cdc2b7d72d243d8f80d986fc8c5722148df30f2b6ac2b9019f7e3b9`  
		Last Modified: Tue, 13 Sep 2022 14:29:08 GMT  
		Size: 29.3 MB (29333406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; 386

```console
$ docker pull mono@sha256:8ef911eede2000787ec9614d4147d27fd3cc3cff7299098645d2c331ff5000ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99166506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a06eb501431fb5c4a879cdedfba520528fb72e991ce30c46d974238e2103341`
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
