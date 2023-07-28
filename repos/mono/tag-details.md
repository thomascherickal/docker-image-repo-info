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
$ docker pull mono@sha256:f6aa5061fb9bc2b02181d353b20f053f5ca5f4a146754221c2e1eabaa4b723b1
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
$ docker pull mono@sha256:312c08a95ef6d46ef6e4c8fafdd00a3db2217a08a723b2522b34202587c4d022
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.7 MB (254674669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bdd38b14cfa4b2efc29dbdd11524b52dbce269382bba20486585d925feb75b4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:29 GMT
ADD file:20e7ad6bec617357895302b08431eb3430cce3113bdf0a8ff9827115f858d313 in / 
# Thu, 27 Jul 2023 23:25:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 02:09:38 GMT
ENV MONO_VERSION=6.12.0.182
# Fri, 28 Jul 2023 02:09:47 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 28 Jul 2023 02:10:14 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 28 Jul 2023 02:13:35 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3240fe174df9a5a4923c4b52f1d887dd1ad1a9ee69245c1fb867f399167584dd`  
		Last Modified: Thu, 27 Jul 2023 23:30:49 GMT  
		Size: 27.2 MB (27187431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe764ada48e9c07b599b90c63ebf3a1516f625cfe72cdf4ba823f1dfcd9e713`  
		Last Modified: Fri, 28 Jul 2023 02:20:05 GMT  
		Size: 2.8 MB (2780934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8209140f449ce8c93dde23e84011feda1a897dd0d7876f5cc4a254360ace6840`  
		Last Modified: Fri, 28 Jul 2023 02:20:14 GMT  
		Size: 64.8 MB (64774344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271c2c4f0ae1503f76d16d77b0a241d5be0f7d669404ae4df1b6ae7ee4deb3ce`  
		Last Modified: Fri, 28 Jul 2023 02:21:14 GMT  
		Size: 159.9 MB (159931960 bytes)  
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
$ docker pull mono@sha256:228365b9003bdbe155f3d1f786fc0e8d5a2b98e83c495b12a270f5337c8fb46a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.0 MB (188972314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37b28609e2e91c56b2be84cb3697f9ba18acf52db99ce37b3503f38b49378e05`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:42 GMT
ADD file:d2008875df919cb9817e6af97438428c2632113c1ef2b67b96607e184a7af941 in / 
# Tue, 04 Jul 2023 00:58:42 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:31:12 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 04 Jul 2023 06:31:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 04 Jul 2023 06:31:53 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 04 Jul 2023 06:33:51 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:966944a300a7cf6431aa9fc3454d07eb7764f6b99d43a67de45ba53c30d69010`  
		Last Modified: Tue, 04 Jul 2023 01:04:17 GMT  
		Size: 22.7 MB (22747297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be94cc696a98d0e36d1f47670d4612782edee527ba65bb72a8b5128330db74d8`  
		Last Modified: Tue, 04 Jul 2023 06:35:30 GMT  
		Size: 2.4 MB (2370509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa72191f7045ac1a8fcb97997b3af65dab038d93dd285c50c65ca49534aa37ff`  
		Last Modified: Tue, 04 Jul 2023 06:35:34 GMT  
		Size: 23.8 MB (23790933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4043418131df76e0b09bfaf3cb531466c9cfb585e2d3ededccb5cd061ac5f61`  
		Last Modified: Tue, 04 Jul 2023 06:36:33 GMT  
		Size: 140.1 MB (140063575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:40f7ed4f999fe484219df8a1e9b9fcc2fe65aa67500d21c88ce8d59284a4389a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.4 MB (216357868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4bf7d3fee3485c84588b0570a26e13c1a0f2f6e096cce8293a7f514a1a7330a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:58:08 GMT
ADD file:1368964550b1f674dd0365f72bb1d55cfebf5e3c651d49b5e168f9be97a6df76 in / 
# Tue, 04 Jul 2023 01:58:09 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:56:32 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 04 Jul 2023 03:56:40 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 04 Jul 2023 03:56:52 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 04 Jul 2023 03:58:21 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:30bfbe1cefebb80f6f9d5d90c39fcdf9d6367bbc76fa68e33ea3b4391c0f9a77`  
		Last Modified: Tue, 04 Jul 2023 02:02:39 GMT  
		Size: 25.9 MB (25921455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99107951ff3754b1aeac3435c4535489d259e102359c031ccb790837666a0254`  
		Last Modified: Tue, 04 Jul 2023 04:00:27 GMT  
		Size: 2.6 MB (2645523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a3a83b2512643cf8777bd8cba8b9fc610132d25a87896c421fd37587d19c16`  
		Last Modified: Tue, 04 Jul 2023 04:00:30 GMT  
		Size: 29.5 MB (29545091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56580de2946a5e2abae6377300a7c78a96f6203adc35b626f6ce779173618a4a`  
		Last Modified: Tue, 04 Jul 2023 04:01:18 GMT  
		Size: 158.2 MB (158245799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; 386

```console
$ docker pull mono@sha256:1c5f4caca4cce6f99b6c360bca43499da6471f93cb3382548133c45c3301ff5b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.6 MB (259559303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afc318cff1d908e73180f1168f11a2d7e1327709c80436c93543d7e80222d7e6`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:39:38 GMT
ADD file:a97f1ea317cafcf2810dfbe8ff5dfde5c43414d9cd1480b4e5f49d3ada8633f7 in / 
# Thu, 27 Jul 2023 23:39:38 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:17:04 GMT
ENV MONO_VERSION=6.12.0.182
# Fri, 28 Jul 2023 00:17:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 28 Jul 2023 00:17:51 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 28 Jul 2023 00:20:55 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7eefe1e1e0f6af56fb4d37f33d6efcd121b57a2c33f6ce8272858d586e51f9d0`  
		Last Modified: Thu, 27 Jul 2023 23:44:57 GMT  
		Size: 27.8 MB (27846808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4faf5b429a2c65753fbcbf71ad8350c16724286c522a53fdeca6f8c9de6a894`  
		Last Modified: Fri, 28 Jul 2023 00:23:35 GMT  
		Size: 2.8 MB (2792567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3bc6db4d28a564350a4e9900fdf992bb455b93448bc0f64c5fbad0bea76da8`  
		Last Modified: Fri, 28 Jul 2023 00:23:48 GMT  
		Size: 68.8 MB (68800619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584274866dcb05649b337a249dc340029a4a5b359ef05fd57c4ade73be901175`  
		Last Modified: Fri, 28 Jul 2023 00:25:02 GMT  
		Size: 160.1 MB (160119309 bytes)  
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
$ docker pull mono@sha256:3b9876153cf5c1d1d6851372b14f02a4fc89bd4a9b1cb728f30766b88485dc24
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
$ docker pull mono@sha256:244c2a452e789e780cfc8afeb08ffc7e82222f183e7d1801155ae3ebd2d4fe31
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94742709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63b4ec69d3f5477554d095f405458f17f96471b81e653da1bf2301b579f96dd4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:29 GMT
ADD file:20e7ad6bec617357895302b08431eb3430cce3113bdf0a8ff9827115f858d313 in / 
# Thu, 27 Jul 2023 23:25:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 02:09:38 GMT
ENV MONO_VERSION=6.12.0.182
# Fri, 28 Jul 2023 02:09:47 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 28 Jul 2023 02:10:14 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3240fe174df9a5a4923c4b52f1d887dd1ad1a9ee69245c1fb867f399167584dd`  
		Last Modified: Thu, 27 Jul 2023 23:30:49 GMT  
		Size: 27.2 MB (27187431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe764ada48e9c07b599b90c63ebf3a1516f625cfe72cdf4ba823f1dfcd9e713`  
		Last Modified: Fri, 28 Jul 2023 02:20:05 GMT  
		Size: 2.8 MB (2780934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8209140f449ce8c93dde23e84011feda1a897dd0d7876f5cc4a254360ace6840`  
		Last Modified: Fri, 28 Jul 2023 02:20:14 GMT  
		Size: 64.8 MB (64774344 bytes)  
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
$ docker pull mono@sha256:e2a0784d2210c17aea82ca670401c851aab819882d06758dfb442a714345710d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48908739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ceea04ca6ea018102d4ffa23c11390bceca7108660a0db90e4c2c476b0463ae`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:42 GMT
ADD file:d2008875df919cb9817e6af97438428c2632113c1ef2b67b96607e184a7af941 in / 
# Tue, 04 Jul 2023 00:58:42 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:31:12 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 04 Jul 2023 06:31:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 04 Jul 2023 06:31:53 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:966944a300a7cf6431aa9fc3454d07eb7764f6b99d43a67de45ba53c30d69010`  
		Last Modified: Tue, 04 Jul 2023 01:04:17 GMT  
		Size: 22.7 MB (22747297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be94cc696a98d0e36d1f47670d4612782edee527ba65bb72a8b5128330db74d8`  
		Last Modified: Tue, 04 Jul 2023 06:35:30 GMT  
		Size: 2.4 MB (2370509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa72191f7045ac1a8fcb97997b3af65dab038d93dd285c50c65ca49534aa37ff`  
		Last Modified: Tue, 04 Jul 2023 06:35:34 GMT  
		Size: 23.8 MB (23790933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:658ec51415f0f6cd3ba15b340b3a4f86bda1c9410628b628282d876fa27ae5f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.1 MB (58112069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3803682e19eaccfbba33a5e261f5edf4db80b54cdc5a641c65a4c91aef3c2b88`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:58:08 GMT
ADD file:1368964550b1f674dd0365f72bb1d55cfebf5e3c651d49b5e168f9be97a6df76 in / 
# Tue, 04 Jul 2023 01:58:09 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:56:32 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 04 Jul 2023 03:56:40 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 04 Jul 2023 03:56:52 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:30bfbe1cefebb80f6f9d5d90c39fcdf9d6367bbc76fa68e33ea3b4391c0f9a77`  
		Last Modified: Tue, 04 Jul 2023 02:02:39 GMT  
		Size: 25.9 MB (25921455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99107951ff3754b1aeac3435c4535489d259e102359c031ccb790837666a0254`  
		Last Modified: Tue, 04 Jul 2023 04:00:27 GMT  
		Size: 2.6 MB (2645523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a3a83b2512643cf8777bd8cba8b9fc610132d25a87896c421fd37587d19c16`  
		Last Modified: Tue, 04 Jul 2023 04:00:30 GMT  
		Size: 29.5 MB (29545091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; 386

```console
$ docker pull mono@sha256:0436c43d2f9e492d4631868efa906eb9cdd910922385c0462185520ffaa12863
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99439994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c3f4516d8f9d9ea6bd9ec818e6b1d189c281e9937425b38353efa04dcfa0922`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:39:38 GMT
ADD file:a97f1ea317cafcf2810dfbe8ff5dfde5c43414d9cd1480b4e5f49d3ada8633f7 in / 
# Thu, 27 Jul 2023 23:39:38 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:17:04 GMT
ENV MONO_VERSION=6.12.0.182
# Fri, 28 Jul 2023 00:17:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 28 Jul 2023 00:17:51 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7eefe1e1e0f6af56fb4d37f33d6efcd121b57a2c33f6ce8272858d586e51f9d0`  
		Last Modified: Thu, 27 Jul 2023 23:44:57 GMT  
		Size: 27.8 MB (27846808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4faf5b429a2c65753fbcbf71ad8350c16724286c522a53fdeca6f8c9de6a894`  
		Last Modified: Fri, 28 Jul 2023 00:23:35 GMT  
		Size: 2.8 MB (2792567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3bc6db4d28a564350a4e9900fdf992bb455b93448bc0f64c5fbad0bea76da8`  
		Last Modified: Fri, 28 Jul 2023 00:23:48 GMT  
		Size: 68.8 MB (68800619 bytes)  
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
$ docker pull mono@sha256:59b4edfb90e7cd06ade869d569e1914380a51dcb5887caac1d2d7fd2ad5c73b7
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
$ docker pull mono@sha256:0be87cc428dda77766f4f40330c6e0dd6cdf433ba2b6c71c2123d347c055d31c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.1 MB (225070968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b748adca6f2ad10aa75252ac5286f272867815f858621d5f58eaf0ef62d2959`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:29 GMT
ADD file:20e7ad6bec617357895302b08431eb3430cce3113bdf0a8ff9827115f858d313 in / 
# Thu, 27 Jul 2023 23:25:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 02:10:18 GMT
ENV MONO_VERSION=6.10.0.104
# Fri, 28 Jul 2023 02:10:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 28 Jul 2023 02:10:53 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 28 Jul 2023 02:19:34 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3240fe174df9a5a4923c4b52f1d887dd1ad1a9ee69245c1fb867f399167584dd`  
		Last Modified: Thu, 27 Jul 2023 23:30:49 GMT  
		Size: 27.2 MB (27187431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1844110300ea6e99d4c8a76acd8a683a2444d0b0baede2ecf5a7f4063c7183`  
		Last Modified: Fri, 28 Jul 2023 02:20:32 GMT  
		Size: 2.8 MB (2780924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6e5fb93922666dd6459d63d863bb5bf9a6b7a1070f889d2fd716ac0c23397f`  
		Last Modified: Fri, 28 Jul 2023 02:20:41 GMT  
		Size: 64.8 MB (64780295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da34c79e6b9d22874be585b9cdc50e773fa9f42576b5e42bd5134472e6065e7`  
		Last Modified: Fri, 28 Jul 2023 02:21:46 GMT  
		Size: 130.3 MB (130322318 bytes)  
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
$ docker pull mono@sha256:25dd113c172b145b766b05b452084e3e313621aaaec34ea9062a70f337b868ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.8 MB (176770923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2545c9d6c5aa21d789e453d7ad35a30b4a178e15ca3850cde48814b80b2822aa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:42 GMT
ADD file:d2008875df919cb9817e6af97438428c2632113c1ef2b67b96607e184a7af941 in / 
# Tue, 04 Jul 2023 00:58:42 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:32:00 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 04 Jul 2023 06:32:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 04 Jul 2023 06:32:26 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 04 Jul 2023 06:35:02 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:966944a300a7cf6431aa9fc3454d07eb7764f6b99d43a67de45ba53c30d69010`  
		Last Modified: Tue, 04 Jul 2023 01:04:17 GMT  
		Size: 22.7 MB (22747297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4fd9b730e1ab19f995d5d691e05bccdf9b337e2a15d6d9f1781de5c6579e7cc`  
		Last Modified: Tue, 04 Jul 2023 06:35:50 GMT  
		Size: 2.4 MB (2370517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51fe2c3df3b18da4f962019eff7638498a2db6624cf89245b6f00643173e2cca`  
		Last Modified: Tue, 04 Jul 2023 06:35:54 GMT  
		Size: 23.8 MB (23815900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aacb225790a400fa97adb8175865c817447aed5ff5523eae5a8ad51500ed824`  
		Last Modified: Tue, 04 Jul 2023 06:37:13 GMT  
		Size: 127.8 MB (127837209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:0adb85f49109889b9ae292eb137f3edce6191e8ca291aa90fa692f360d17cf9f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.6 MB (203632163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e77af2ad462e8c6aeb9ccde0e1de1eaea6b8c3f252f8e6dd5656d2a38b0fe0f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:58:08 GMT
ADD file:1368964550b1f674dd0365f72bb1d55cfebf5e3c651d49b5e168f9be97a6df76 in / 
# Tue, 04 Jul 2023 01:58:09 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:56:55 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 04 Jul 2023 03:57:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 04 Jul 2023 03:57:20 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 04 Jul 2023 03:59:53 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:30bfbe1cefebb80f6f9d5d90c39fcdf9d6367bbc76fa68e33ea3b4391c0f9a77`  
		Last Modified: Tue, 04 Jul 2023 02:02:39 GMT  
		Size: 25.9 MB (25921455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9d56499228dc544904c4f856e05eabbbc50a057f1f5c2c635fd9819918678a`  
		Last Modified: Tue, 04 Jul 2023 04:00:45 GMT  
		Size: 2.6 MB (2645506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf4543b7545b83567c58ed1a44a835ffbaec3ca198633571906c741a4dff715`  
		Last Modified: Tue, 04 Jul 2023 04:00:49 GMT  
		Size: 29.6 MB (29575025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430d7034a447934d872db6e100a7aa718d623d89b83de7f985a2aa49fcd80d18`  
		Last Modified: Tue, 04 Jul 2023 04:01:49 GMT  
		Size: 145.5 MB (145490177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; 386

```console
$ docker pull mono@sha256:69b0f37952dfec261e8c16ae861b9b7c014df9857b61e95850b6ed290e38b6bc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.9 MB (230911957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04b838af64bab97ad8516a3feafea2b25ed2375b55faeccbcdd7c1802bc3df32`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:39:38 GMT
ADD file:a97f1ea317cafcf2810dfbe8ff5dfde5c43414d9cd1480b4e5f49d3ada8633f7 in / 
# Thu, 27 Jul 2023 23:39:38 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:18:02 GMT
ENV MONO_VERSION=6.10.0.104
# Fri, 28 Jul 2023 00:18:11 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 28 Jul 2023 00:18:42 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 28 Jul 2023 00:23:07 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7eefe1e1e0f6af56fb4d37f33d6efcd121b57a2c33f6ce8272858d586e51f9d0`  
		Last Modified: Thu, 27 Jul 2023 23:44:57 GMT  
		Size: 27.8 MB (27846808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb81f87ac0902af9cd72dd1a5d8f01551f16c706bea82dfd669de2f57cb751b8`  
		Last Modified: Fri, 28 Jul 2023 00:24:03 GMT  
		Size: 2.8 MB (2792583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47bcb454af9ee892f7e2583cb648812806b28177403c8f009873d5aa0efc66e3`  
		Last Modified: Fri, 28 Jul 2023 00:24:17 GMT  
		Size: 68.8 MB (68810219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda2f933d4bef882598229a8603092208e007fc59737f262213209cf95204793`  
		Last Modified: Fri, 28 Jul 2023 00:25:45 GMT  
		Size: 131.5 MB (131462347 bytes)  
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
$ docker pull mono@sha256:05ff7a757f8860e19f76fe22b86eab0b4ea6bca961eed8a8c7a3b014bdb3eefb
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
$ docker pull mono@sha256:8d297cfcbc2a1e56515df7327cf4ce2cb9ca26ff280669428a30c3e68dcf5047
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94748650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4a804387646babe1a7dbcd754d6e57853d95eef5a8311f2b62e55a0b1e191c4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:29 GMT
ADD file:20e7ad6bec617357895302b08431eb3430cce3113bdf0a8ff9827115f858d313 in / 
# Thu, 27 Jul 2023 23:25:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 02:10:18 GMT
ENV MONO_VERSION=6.10.0.104
# Fri, 28 Jul 2023 02:10:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 28 Jul 2023 02:10:53 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3240fe174df9a5a4923c4b52f1d887dd1ad1a9ee69245c1fb867f399167584dd`  
		Last Modified: Thu, 27 Jul 2023 23:30:49 GMT  
		Size: 27.2 MB (27187431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1844110300ea6e99d4c8a76acd8a683a2444d0b0baede2ecf5a7f4063c7183`  
		Last Modified: Fri, 28 Jul 2023 02:20:32 GMT  
		Size: 2.8 MB (2780924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6e5fb93922666dd6459d63d863bb5bf9a6b7a1070f889d2fd716ac0c23397f`  
		Last Modified: Fri, 28 Jul 2023 02:20:41 GMT  
		Size: 64.8 MB (64780295 bytes)  
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
$ docker pull mono@sha256:b24a3e81a35e7f7ea3c0b5cbfa0b5bd79bf6ce8bcdad103ea7d9ac800c40fc17
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48933714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc5e4e91a8e59eb53786e087ebe42be632689c3c5b5e4cc534aed3552898a2ea`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:42 GMT
ADD file:d2008875df919cb9817e6af97438428c2632113c1ef2b67b96607e184a7af941 in / 
# Tue, 04 Jul 2023 00:58:42 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:32:00 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 04 Jul 2023 06:32:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 04 Jul 2023 06:32:26 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:966944a300a7cf6431aa9fc3454d07eb7764f6b99d43a67de45ba53c30d69010`  
		Last Modified: Tue, 04 Jul 2023 01:04:17 GMT  
		Size: 22.7 MB (22747297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4fd9b730e1ab19f995d5d691e05bccdf9b337e2a15d6d9f1781de5c6579e7cc`  
		Last Modified: Tue, 04 Jul 2023 06:35:50 GMT  
		Size: 2.4 MB (2370517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51fe2c3df3b18da4f962019eff7638498a2db6624cf89245b6f00643173e2cca`  
		Last Modified: Tue, 04 Jul 2023 06:35:54 GMT  
		Size: 23.8 MB (23815900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:5d7a2bc8b55d06994602682bff2dd141fab2f0e8cebb837e768a99f1a34339c6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.1 MB (58141986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b020da906a0162533c72484f0c414bbdd4fce371306ec5102f05fd1dc697128`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:58:08 GMT
ADD file:1368964550b1f674dd0365f72bb1d55cfebf5e3c651d49b5e168f9be97a6df76 in / 
# Tue, 04 Jul 2023 01:58:09 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:56:55 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 04 Jul 2023 03:57:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 04 Jul 2023 03:57:20 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:30bfbe1cefebb80f6f9d5d90c39fcdf9d6367bbc76fa68e33ea3b4391c0f9a77`  
		Last Modified: Tue, 04 Jul 2023 02:02:39 GMT  
		Size: 25.9 MB (25921455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9d56499228dc544904c4f856e05eabbbc50a057f1f5c2c635fd9819918678a`  
		Last Modified: Tue, 04 Jul 2023 04:00:45 GMT  
		Size: 2.6 MB (2645506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf4543b7545b83567c58ed1a44a835ffbaec3ca198633571906c741a4dff715`  
		Last Modified: Tue, 04 Jul 2023 04:00:49 GMT  
		Size: 29.6 MB (29575025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; 386

```console
$ docker pull mono@sha256:178c16cffc8c9a4a8cd20de9b2b6a986e07f2ff2296342c262a4d2b8f960bb5d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99449610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b274d656f895f0925fd50eadb0b84b7cfff70a99a4439b9a82ce34de90e3805`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:39:38 GMT
ADD file:a97f1ea317cafcf2810dfbe8ff5dfde5c43414d9cd1480b4e5f49d3ada8633f7 in / 
# Thu, 27 Jul 2023 23:39:38 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:18:02 GMT
ENV MONO_VERSION=6.10.0.104
# Fri, 28 Jul 2023 00:18:11 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 28 Jul 2023 00:18:42 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7eefe1e1e0f6af56fb4d37f33d6efcd121b57a2c33f6ce8272858d586e51f9d0`  
		Last Modified: Thu, 27 Jul 2023 23:44:57 GMT  
		Size: 27.8 MB (27846808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb81f87ac0902af9cd72dd1a5d8f01551f16c706bea82dfd669de2f57cb751b8`  
		Last Modified: Fri, 28 Jul 2023 00:24:03 GMT  
		Size: 2.8 MB (2792583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47bcb454af9ee892f7e2583cb648812806b28177403c8f009873d5aa0efc66e3`  
		Last Modified: Fri, 28 Jul 2023 00:24:17 GMT  
		Size: 68.8 MB (68810219 bytes)  
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
$ docker pull mono@sha256:59b4edfb90e7cd06ade869d569e1914380a51dcb5887caac1d2d7fd2ad5c73b7
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
$ docker pull mono@sha256:0be87cc428dda77766f4f40330c6e0dd6cdf433ba2b6c71c2123d347c055d31c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.1 MB (225070968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b748adca6f2ad10aa75252ac5286f272867815f858621d5f58eaf0ef62d2959`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:29 GMT
ADD file:20e7ad6bec617357895302b08431eb3430cce3113bdf0a8ff9827115f858d313 in / 
# Thu, 27 Jul 2023 23:25:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 02:10:18 GMT
ENV MONO_VERSION=6.10.0.104
# Fri, 28 Jul 2023 02:10:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 28 Jul 2023 02:10:53 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 28 Jul 2023 02:19:34 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3240fe174df9a5a4923c4b52f1d887dd1ad1a9ee69245c1fb867f399167584dd`  
		Last Modified: Thu, 27 Jul 2023 23:30:49 GMT  
		Size: 27.2 MB (27187431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1844110300ea6e99d4c8a76acd8a683a2444d0b0baede2ecf5a7f4063c7183`  
		Last Modified: Fri, 28 Jul 2023 02:20:32 GMT  
		Size: 2.8 MB (2780924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6e5fb93922666dd6459d63d863bb5bf9a6b7a1070f889d2fd716ac0c23397f`  
		Last Modified: Fri, 28 Jul 2023 02:20:41 GMT  
		Size: 64.8 MB (64780295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da34c79e6b9d22874be585b9cdc50e773fa9f42576b5e42bd5134472e6065e7`  
		Last Modified: Fri, 28 Jul 2023 02:21:46 GMT  
		Size: 130.3 MB (130322318 bytes)  
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
$ docker pull mono@sha256:25dd113c172b145b766b05b452084e3e313621aaaec34ea9062a70f337b868ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.8 MB (176770923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2545c9d6c5aa21d789e453d7ad35a30b4a178e15ca3850cde48814b80b2822aa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:42 GMT
ADD file:d2008875df919cb9817e6af97438428c2632113c1ef2b67b96607e184a7af941 in / 
# Tue, 04 Jul 2023 00:58:42 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:32:00 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 04 Jul 2023 06:32:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 04 Jul 2023 06:32:26 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 04 Jul 2023 06:35:02 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:966944a300a7cf6431aa9fc3454d07eb7764f6b99d43a67de45ba53c30d69010`  
		Last Modified: Tue, 04 Jul 2023 01:04:17 GMT  
		Size: 22.7 MB (22747297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4fd9b730e1ab19f995d5d691e05bccdf9b337e2a15d6d9f1781de5c6579e7cc`  
		Last Modified: Tue, 04 Jul 2023 06:35:50 GMT  
		Size: 2.4 MB (2370517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51fe2c3df3b18da4f962019eff7638498a2db6624cf89245b6f00643173e2cca`  
		Last Modified: Tue, 04 Jul 2023 06:35:54 GMT  
		Size: 23.8 MB (23815900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aacb225790a400fa97adb8175865c817447aed5ff5523eae5a8ad51500ed824`  
		Last Modified: Tue, 04 Jul 2023 06:37:13 GMT  
		Size: 127.8 MB (127837209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:0adb85f49109889b9ae292eb137f3edce6191e8ca291aa90fa692f360d17cf9f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.6 MB (203632163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e77af2ad462e8c6aeb9ccde0e1de1eaea6b8c3f252f8e6dd5656d2a38b0fe0f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:58:08 GMT
ADD file:1368964550b1f674dd0365f72bb1d55cfebf5e3c651d49b5e168f9be97a6df76 in / 
# Tue, 04 Jul 2023 01:58:09 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:56:55 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 04 Jul 2023 03:57:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 04 Jul 2023 03:57:20 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 04 Jul 2023 03:59:53 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:30bfbe1cefebb80f6f9d5d90c39fcdf9d6367bbc76fa68e33ea3b4391c0f9a77`  
		Last Modified: Tue, 04 Jul 2023 02:02:39 GMT  
		Size: 25.9 MB (25921455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9d56499228dc544904c4f856e05eabbbc50a057f1f5c2c635fd9819918678a`  
		Last Modified: Tue, 04 Jul 2023 04:00:45 GMT  
		Size: 2.6 MB (2645506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf4543b7545b83567c58ed1a44a835ffbaec3ca198633571906c741a4dff715`  
		Last Modified: Tue, 04 Jul 2023 04:00:49 GMT  
		Size: 29.6 MB (29575025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430d7034a447934d872db6e100a7aa718d623d89b83de7f985a2aa49fcd80d18`  
		Last Modified: Tue, 04 Jul 2023 04:01:49 GMT  
		Size: 145.5 MB (145490177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; 386

```console
$ docker pull mono@sha256:69b0f37952dfec261e8c16ae861b9b7c014df9857b61e95850b6ed290e38b6bc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.9 MB (230911957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04b838af64bab97ad8516a3feafea2b25ed2375b55faeccbcdd7c1802bc3df32`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:39:38 GMT
ADD file:a97f1ea317cafcf2810dfbe8ff5dfde5c43414d9cd1480b4e5f49d3ada8633f7 in / 
# Thu, 27 Jul 2023 23:39:38 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:18:02 GMT
ENV MONO_VERSION=6.10.0.104
# Fri, 28 Jul 2023 00:18:11 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 28 Jul 2023 00:18:42 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 28 Jul 2023 00:23:07 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7eefe1e1e0f6af56fb4d37f33d6efcd121b57a2c33f6ce8272858d586e51f9d0`  
		Last Modified: Thu, 27 Jul 2023 23:44:57 GMT  
		Size: 27.8 MB (27846808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb81f87ac0902af9cd72dd1a5d8f01551f16c706bea82dfd669de2f57cb751b8`  
		Last Modified: Fri, 28 Jul 2023 00:24:03 GMT  
		Size: 2.8 MB (2792583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47bcb454af9ee892f7e2583cb648812806b28177403c8f009873d5aa0efc66e3`  
		Last Modified: Fri, 28 Jul 2023 00:24:17 GMT  
		Size: 68.8 MB (68810219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda2f933d4bef882598229a8603092208e007fc59737f262213209cf95204793`  
		Last Modified: Fri, 28 Jul 2023 00:25:45 GMT  
		Size: 131.5 MB (131462347 bytes)  
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
$ docker pull mono@sha256:05ff7a757f8860e19f76fe22b86eab0b4ea6bca961eed8a8c7a3b014bdb3eefb
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
$ docker pull mono@sha256:8d297cfcbc2a1e56515df7327cf4ce2cb9ca26ff280669428a30c3e68dcf5047
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94748650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4a804387646babe1a7dbcd754d6e57853d95eef5a8311f2b62e55a0b1e191c4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:29 GMT
ADD file:20e7ad6bec617357895302b08431eb3430cce3113bdf0a8ff9827115f858d313 in / 
# Thu, 27 Jul 2023 23:25:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 02:10:18 GMT
ENV MONO_VERSION=6.10.0.104
# Fri, 28 Jul 2023 02:10:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 28 Jul 2023 02:10:53 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3240fe174df9a5a4923c4b52f1d887dd1ad1a9ee69245c1fb867f399167584dd`  
		Last Modified: Thu, 27 Jul 2023 23:30:49 GMT  
		Size: 27.2 MB (27187431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1844110300ea6e99d4c8a76acd8a683a2444d0b0baede2ecf5a7f4063c7183`  
		Last Modified: Fri, 28 Jul 2023 02:20:32 GMT  
		Size: 2.8 MB (2780924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6e5fb93922666dd6459d63d863bb5bf9a6b7a1070f889d2fd716ac0c23397f`  
		Last Modified: Fri, 28 Jul 2023 02:20:41 GMT  
		Size: 64.8 MB (64780295 bytes)  
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
$ docker pull mono@sha256:b24a3e81a35e7f7ea3c0b5cbfa0b5bd79bf6ce8bcdad103ea7d9ac800c40fc17
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48933714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc5e4e91a8e59eb53786e087ebe42be632689c3c5b5e4cc534aed3552898a2ea`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:42 GMT
ADD file:d2008875df919cb9817e6af97438428c2632113c1ef2b67b96607e184a7af941 in / 
# Tue, 04 Jul 2023 00:58:42 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:32:00 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 04 Jul 2023 06:32:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 04 Jul 2023 06:32:26 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:966944a300a7cf6431aa9fc3454d07eb7764f6b99d43a67de45ba53c30d69010`  
		Last Modified: Tue, 04 Jul 2023 01:04:17 GMT  
		Size: 22.7 MB (22747297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4fd9b730e1ab19f995d5d691e05bccdf9b337e2a15d6d9f1781de5c6579e7cc`  
		Last Modified: Tue, 04 Jul 2023 06:35:50 GMT  
		Size: 2.4 MB (2370517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51fe2c3df3b18da4f962019eff7638498a2db6624cf89245b6f00643173e2cca`  
		Last Modified: Tue, 04 Jul 2023 06:35:54 GMT  
		Size: 23.8 MB (23815900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:5d7a2bc8b55d06994602682bff2dd141fab2f0e8cebb837e768a99f1a34339c6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.1 MB (58141986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b020da906a0162533c72484f0c414bbdd4fce371306ec5102f05fd1dc697128`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:58:08 GMT
ADD file:1368964550b1f674dd0365f72bb1d55cfebf5e3c651d49b5e168f9be97a6df76 in / 
# Tue, 04 Jul 2023 01:58:09 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:56:55 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 04 Jul 2023 03:57:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 04 Jul 2023 03:57:20 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:30bfbe1cefebb80f6f9d5d90c39fcdf9d6367bbc76fa68e33ea3b4391c0f9a77`  
		Last Modified: Tue, 04 Jul 2023 02:02:39 GMT  
		Size: 25.9 MB (25921455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9d56499228dc544904c4f856e05eabbbc50a057f1f5c2c635fd9819918678a`  
		Last Modified: Tue, 04 Jul 2023 04:00:45 GMT  
		Size: 2.6 MB (2645506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf4543b7545b83567c58ed1a44a835ffbaec3ca198633571906c741a4dff715`  
		Last Modified: Tue, 04 Jul 2023 04:00:49 GMT  
		Size: 29.6 MB (29575025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; 386

```console
$ docker pull mono@sha256:178c16cffc8c9a4a8cd20de9b2b6a986e07f2ff2296342c262a4d2b8f960bb5d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99449610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b274d656f895f0925fd50eadb0b84b7cfff70a99a4439b9a82ce34de90e3805`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:39:38 GMT
ADD file:a97f1ea317cafcf2810dfbe8ff5dfde5c43414d9cd1480b4e5f49d3ada8633f7 in / 
# Thu, 27 Jul 2023 23:39:38 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:18:02 GMT
ENV MONO_VERSION=6.10.0.104
# Fri, 28 Jul 2023 00:18:11 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 28 Jul 2023 00:18:42 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7eefe1e1e0f6af56fb4d37f33d6efcd121b57a2c33f6ce8272858d586e51f9d0`  
		Last Modified: Thu, 27 Jul 2023 23:44:57 GMT  
		Size: 27.8 MB (27846808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb81f87ac0902af9cd72dd1a5d8f01551f16c706bea82dfd669de2f57cb751b8`  
		Last Modified: Fri, 28 Jul 2023 00:24:03 GMT  
		Size: 2.8 MB (2792583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47bcb454af9ee892f7e2583cb648812806b28177403c8f009873d5aa0efc66e3`  
		Last Modified: Fri, 28 Jul 2023 00:24:17 GMT  
		Size: 68.8 MB (68810219 bytes)  
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
$ docker pull mono@sha256:59b4edfb90e7cd06ade869d569e1914380a51dcb5887caac1d2d7fd2ad5c73b7
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
$ docker pull mono@sha256:0be87cc428dda77766f4f40330c6e0dd6cdf433ba2b6c71c2123d347c055d31c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.1 MB (225070968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b748adca6f2ad10aa75252ac5286f272867815f858621d5f58eaf0ef62d2959`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:29 GMT
ADD file:20e7ad6bec617357895302b08431eb3430cce3113bdf0a8ff9827115f858d313 in / 
# Thu, 27 Jul 2023 23:25:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 02:10:18 GMT
ENV MONO_VERSION=6.10.0.104
# Fri, 28 Jul 2023 02:10:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 28 Jul 2023 02:10:53 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 28 Jul 2023 02:19:34 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3240fe174df9a5a4923c4b52f1d887dd1ad1a9ee69245c1fb867f399167584dd`  
		Last Modified: Thu, 27 Jul 2023 23:30:49 GMT  
		Size: 27.2 MB (27187431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1844110300ea6e99d4c8a76acd8a683a2444d0b0baede2ecf5a7f4063c7183`  
		Last Modified: Fri, 28 Jul 2023 02:20:32 GMT  
		Size: 2.8 MB (2780924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6e5fb93922666dd6459d63d863bb5bf9a6b7a1070f889d2fd716ac0c23397f`  
		Last Modified: Fri, 28 Jul 2023 02:20:41 GMT  
		Size: 64.8 MB (64780295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da34c79e6b9d22874be585b9cdc50e773fa9f42576b5e42bd5134472e6065e7`  
		Last Modified: Fri, 28 Jul 2023 02:21:46 GMT  
		Size: 130.3 MB (130322318 bytes)  
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
$ docker pull mono@sha256:25dd113c172b145b766b05b452084e3e313621aaaec34ea9062a70f337b868ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.8 MB (176770923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2545c9d6c5aa21d789e453d7ad35a30b4a178e15ca3850cde48814b80b2822aa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:42 GMT
ADD file:d2008875df919cb9817e6af97438428c2632113c1ef2b67b96607e184a7af941 in / 
# Tue, 04 Jul 2023 00:58:42 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:32:00 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 04 Jul 2023 06:32:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 04 Jul 2023 06:32:26 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 04 Jul 2023 06:35:02 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:966944a300a7cf6431aa9fc3454d07eb7764f6b99d43a67de45ba53c30d69010`  
		Last Modified: Tue, 04 Jul 2023 01:04:17 GMT  
		Size: 22.7 MB (22747297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4fd9b730e1ab19f995d5d691e05bccdf9b337e2a15d6d9f1781de5c6579e7cc`  
		Last Modified: Tue, 04 Jul 2023 06:35:50 GMT  
		Size: 2.4 MB (2370517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51fe2c3df3b18da4f962019eff7638498a2db6624cf89245b6f00643173e2cca`  
		Last Modified: Tue, 04 Jul 2023 06:35:54 GMT  
		Size: 23.8 MB (23815900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aacb225790a400fa97adb8175865c817447aed5ff5523eae5a8ad51500ed824`  
		Last Modified: Tue, 04 Jul 2023 06:37:13 GMT  
		Size: 127.8 MB (127837209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:0adb85f49109889b9ae292eb137f3edce6191e8ca291aa90fa692f360d17cf9f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.6 MB (203632163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e77af2ad462e8c6aeb9ccde0e1de1eaea6b8c3f252f8e6dd5656d2a38b0fe0f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:58:08 GMT
ADD file:1368964550b1f674dd0365f72bb1d55cfebf5e3c651d49b5e168f9be97a6df76 in / 
# Tue, 04 Jul 2023 01:58:09 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:56:55 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 04 Jul 2023 03:57:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 04 Jul 2023 03:57:20 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 04 Jul 2023 03:59:53 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:30bfbe1cefebb80f6f9d5d90c39fcdf9d6367bbc76fa68e33ea3b4391c0f9a77`  
		Last Modified: Tue, 04 Jul 2023 02:02:39 GMT  
		Size: 25.9 MB (25921455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9d56499228dc544904c4f856e05eabbbc50a057f1f5c2c635fd9819918678a`  
		Last Modified: Tue, 04 Jul 2023 04:00:45 GMT  
		Size: 2.6 MB (2645506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf4543b7545b83567c58ed1a44a835ffbaec3ca198633571906c741a4dff715`  
		Last Modified: Tue, 04 Jul 2023 04:00:49 GMT  
		Size: 29.6 MB (29575025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430d7034a447934d872db6e100a7aa718d623d89b83de7f985a2aa49fcd80d18`  
		Last Modified: Tue, 04 Jul 2023 04:01:49 GMT  
		Size: 145.5 MB (145490177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; 386

```console
$ docker pull mono@sha256:69b0f37952dfec261e8c16ae861b9b7c014df9857b61e95850b6ed290e38b6bc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.9 MB (230911957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04b838af64bab97ad8516a3feafea2b25ed2375b55faeccbcdd7c1802bc3df32`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:39:38 GMT
ADD file:a97f1ea317cafcf2810dfbe8ff5dfde5c43414d9cd1480b4e5f49d3ada8633f7 in / 
# Thu, 27 Jul 2023 23:39:38 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:18:02 GMT
ENV MONO_VERSION=6.10.0.104
# Fri, 28 Jul 2023 00:18:11 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 28 Jul 2023 00:18:42 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 28 Jul 2023 00:23:07 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7eefe1e1e0f6af56fb4d37f33d6efcd121b57a2c33f6ce8272858d586e51f9d0`  
		Last Modified: Thu, 27 Jul 2023 23:44:57 GMT  
		Size: 27.8 MB (27846808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb81f87ac0902af9cd72dd1a5d8f01551f16c706bea82dfd669de2f57cb751b8`  
		Last Modified: Fri, 28 Jul 2023 00:24:03 GMT  
		Size: 2.8 MB (2792583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47bcb454af9ee892f7e2583cb648812806b28177403c8f009873d5aa0efc66e3`  
		Last Modified: Fri, 28 Jul 2023 00:24:17 GMT  
		Size: 68.8 MB (68810219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda2f933d4bef882598229a8603092208e007fc59737f262213209cf95204793`  
		Last Modified: Fri, 28 Jul 2023 00:25:45 GMT  
		Size: 131.5 MB (131462347 bytes)  
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
$ docker pull mono@sha256:05ff7a757f8860e19f76fe22b86eab0b4ea6bca961eed8a8c7a3b014bdb3eefb
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
$ docker pull mono@sha256:8d297cfcbc2a1e56515df7327cf4ce2cb9ca26ff280669428a30c3e68dcf5047
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94748650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4a804387646babe1a7dbcd754d6e57853d95eef5a8311f2b62e55a0b1e191c4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:29 GMT
ADD file:20e7ad6bec617357895302b08431eb3430cce3113bdf0a8ff9827115f858d313 in / 
# Thu, 27 Jul 2023 23:25:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 02:10:18 GMT
ENV MONO_VERSION=6.10.0.104
# Fri, 28 Jul 2023 02:10:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 28 Jul 2023 02:10:53 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3240fe174df9a5a4923c4b52f1d887dd1ad1a9ee69245c1fb867f399167584dd`  
		Last Modified: Thu, 27 Jul 2023 23:30:49 GMT  
		Size: 27.2 MB (27187431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1844110300ea6e99d4c8a76acd8a683a2444d0b0baede2ecf5a7f4063c7183`  
		Last Modified: Fri, 28 Jul 2023 02:20:32 GMT  
		Size: 2.8 MB (2780924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6e5fb93922666dd6459d63d863bb5bf9a6b7a1070f889d2fd716ac0c23397f`  
		Last Modified: Fri, 28 Jul 2023 02:20:41 GMT  
		Size: 64.8 MB (64780295 bytes)  
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
$ docker pull mono@sha256:b24a3e81a35e7f7ea3c0b5cbfa0b5bd79bf6ce8bcdad103ea7d9ac800c40fc17
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48933714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc5e4e91a8e59eb53786e087ebe42be632689c3c5b5e4cc534aed3552898a2ea`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:42 GMT
ADD file:d2008875df919cb9817e6af97438428c2632113c1ef2b67b96607e184a7af941 in / 
# Tue, 04 Jul 2023 00:58:42 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:32:00 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 04 Jul 2023 06:32:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 04 Jul 2023 06:32:26 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:966944a300a7cf6431aa9fc3454d07eb7764f6b99d43a67de45ba53c30d69010`  
		Last Modified: Tue, 04 Jul 2023 01:04:17 GMT  
		Size: 22.7 MB (22747297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4fd9b730e1ab19f995d5d691e05bccdf9b337e2a15d6d9f1781de5c6579e7cc`  
		Last Modified: Tue, 04 Jul 2023 06:35:50 GMT  
		Size: 2.4 MB (2370517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51fe2c3df3b18da4f962019eff7638498a2db6624cf89245b6f00643173e2cca`  
		Last Modified: Tue, 04 Jul 2023 06:35:54 GMT  
		Size: 23.8 MB (23815900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:5d7a2bc8b55d06994602682bff2dd141fab2f0e8cebb837e768a99f1a34339c6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.1 MB (58141986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b020da906a0162533c72484f0c414bbdd4fce371306ec5102f05fd1dc697128`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:58:08 GMT
ADD file:1368964550b1f674dd0365f72bb1d55cfebf5e3c651d49b5e168f9be97a6df76 in / 
# Tue, 04 Jul 2023 01:58:09 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:56:55 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 04 Jul 2023 03:57:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 04 Jul 2023 03:57:20 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:30bfbe1cefebb80f6f9d5d90c39fcdf9d6367bbc76fa68e33ea3b4391c0f9a77`  
		Last Modified: Tue, 04 Jul 2023 02:02:39 GMT  
		Size: 25.9 MB (25921455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9d56499228dc544904c4f856e05eabbbc50a057f1f5c2c635fd9819918678a`  
		Last Modified: Tue, 04 Jul 2023 04:00:45 GMT  
		Size: 2.6 MB (2645506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf4543b7545b83567c58ed1a44a835ffbaec3ca198633571906c741a4dff715`  
		Last Modified: Tue, 04 Jul 2023 04:00:49 GMT  
		Size: 29.6 MB (29575025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; 386

```console
$ docker pull mono@sha256:178c16cffc8c9a4a8cd20de9b2b6a986e07f2ff2296342c262a4d2b8f960bb5d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99449610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b274d656f895f0925fd50eadb0b84b7cfff70a99a4439b9a82ce34de90e3805`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:39:38 GMT
ADD file:a97f1ea317cafcf2810dfbe8ff5dfde5c43414d9cd1480b4e5f49d3ada8633f7 in / 
# Thu, 27 Jul 2023 23:39:38 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:18:02 GMT
ENV MONO_VERSION=6.10.0.104
# Fri, 28 Jul 2023 00:18:11 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 28 Jul 2023 00:18:42 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7eefe1e1e0f6af56fb4d37f33d6efcd121b57a2c33f6ce8272858d586e51f9d0`  
		Last Modified: Thu, 27 Jul 2023 23:44:57 GMT  
		Size: 27.8 MB (27846808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb81f87ac0902af9cd72dd1a5d8f01551f16c706bea82dfd669de2f57cb751b8`  
		Last Modified: Fri, 28 Jul 2023 00:24:03 GMT  
		Size: 2.8 MB (2792583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47bcb454af9ee892f7e2583cb648812806b28177403c8f009873d5aa0efc66e3`  
		Last Modified: Fri, 28 Jul 2023 00:24:17 GMT  
		Size: 68.8 MB (68810219 bytes)  
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
$ docker pull mono@sha256:f6aa5061fb9bc2b02181d353b20f053f5ca5f4a146754221c2e1eabaa4b723b1
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
$ docker pull mono@sha256:312c08a95ef6d46ef6e4c8fafdd00a3db2217a08a723b2522b34202587c4d022
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.7 MB (254674669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bdd38b14cfa4b2efc29dbdd11524b52dbce269382bba20486585d925feb75b4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:29 GMT
ADD file:20e7ad6bec617357895302b08431eb3430cce3113bdf0a8ff9827115f858d313 in / 
# Thu, 27 Jul 2023 23:25:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 02:09:38 GMT
ENV MONO_VERSION=6.12.0.182
# Fri, 28 Jul 2023 02:09:47 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 28 Jul 2023 02:10:14 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 28 Jul 2023 02:13:35 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3240fe174df9a5a4923c4b52f1d887dd1ad1a9ee69245c1fb867f399167584dd`  
		Last Modified: Thu, 27 Jul 2023 23:30:49 GMT  
		Size: 27.2 MB (27187431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe764ada48e9c07b599b90c63ebf3a1516f625cfe72cdf4ba823f1dfcd9e713`  
		Last Modified: Fri, 28 Jul 2023 02:20:05 GMT  
		Size: 2.8 MB (2780934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8209140f449ce8c93dde23e84011feda1a897dd0d7876f5cc4a254360ace6840`  
		Last Modified: Fri, 28 Jul 2023 02:20:14 GMT  
		Size: 64.8 MB (64774344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271c2c4f0ae1503f76d16d77b0a241d5be0f7d669404ae4df1b6ae7ee4deb3ce`  
		Last Modified: Fri, 28 Jul 2023 02:21:14 GMT  
		Size: 159.9 MB (159931960 bytes)  
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
$ docker pull mono@sha256:228365b9003bdbe155f3d1f786fc0e8d5a2b98e83c495b12a270f5337c8fb46a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.0 MB (188972314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37b28609e2e91c56b2be84cb3697f9ba18acf52db99ce37b3503f38b49378e05`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:42 GMT
ADD file:d2008875df919cb9817e6af97438428c2632113c1ef2b67b96607e184a7af941 in / 
# Tue, 04 Jul 2023 00:58:42 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:31:12 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 04 Jul 2023 06:31:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 04 Jul 2023 06:31:53 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 04 Jul 2023 06:33:51 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:966944a300a7cf6431aa9fc3454d07eb7764f6b99d43a67de45ba53c30d69010`  
		Last Modified: Tue, 04 Jul 2023 01:04:17 GMT  
		Size: 22.7 MB (22747297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be94cc696a98d0e36d1f47670d4612782edee527ba65bb72a8b5128330db74d8`  
		Last Modified: Tue, 04 Jul 2023 06:35:30 GMT  
		Size: 2.4 MB (2370509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa72191f7045ac1a8fcb97997b3af65dab038d93dd285c50c65ca49534aa37ff`  
		Last Modified: Tue, 04 Jul 2023 06:35:34 GMT  
		Size: 23.8 MB (23790933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4043418131df76e0b09bfaf3cb531466c9cfb585e2d3ededccb5cd061ac5f61`  
		Last Modified: Tue, 04 Jul 2023 06:36:33 GMT  
		Size: 140.1 MB (140063575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:40f7ed4f999fe484219df8a1e9b9fcc2fe65aa67500d21c88ce8d59284a4389a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.4 MB (216357868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4bf7d3fee3485c84588b0570a26e13c1a0f2f6e096cce8293a7f514a1a7330a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:58:08 GMT
ADD file:1368964550b1f674dd0365f72bb1d55cfebf5e3c651d49b5e168f9be97a6df76 in / 
# Tue, 04 Jul 2023 01:58:09 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:56:32 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 04 Jul 2023 03:56:40 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 04 Jul 2023 03:56:52 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 04 Jul 2023 03:58:21 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:30bfbe1cefebb80f6f9d5d90c39fcdf9d6367bbc76fa68e33ea3b4391c0f9a77`  
		Last Modified: Tue, 04 Jul 2023 02:02:39 GMT  
		Size: 25.9 MB (25921455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99107951ff3754b1aeac3435c4535489d259e102359c031ccb790837666a0254`  
		Last Modified: Tue, 04 Jul 2023 04:00:27 GMT  
		Size: 2.6 MB (2645523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a3a83b2512643cf8777bd8cba8b9fc610132d25a87896c421fd37587d19c16`  
		Last Modified: Tue, 04 Jul 2023 04:00:30 GMT  
		Size: 29.5 MB (29545091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56580de2946a5e2abae6377300a7c78a96f6203adc35b626f6ce779173618a4a`  
		Last Modified: Tue, 04 Jul 2023 04:01:18 GMT  
		Size: 158.2 MB (158245799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12` - linux; 386

```console
$ docker pull mono@sha256:1c5f4caca4cce6f99b6c360bca43499da6471f93cb3382548133c45c3301ff5b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.6 MB (259559303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afc318cff1d908e73180f1168f11a2d7e1327709c80436c93543d7e80222d7e6`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:39:38 GMT
ADD file:a97f1ea317cafcf2810dfbe8ff5dfde5c43414d9cd1480b4e5f49d3ada8633f7 in / 
# Thu, 27 Jul 2023 23:39:38 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:17:04 GMT
ENV MONO_VERSION=6.12.0.182
# Fri, 28 Jul 2023 00:17:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 28 Jul 2023 00:17:51 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 28 Jul 2023 00:20:55 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7eefe1e1e0f6af56fb4d37f33d6efcd121b57a2c33f6ce8272858d586e51f9d0`  
		Last Modified: Thu, 27 Jul 2023 23:44:57 GMT  
		Size: 27.8 MB (27846808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4faf5b429a2c65753fbcbf71ad8350c16724286c522a53fdeca6f8c9de6a894`  
		Last Modified: Fri, 28 Jul 2023 00:23:35 GMT  
		Size: 2.8 MB (2792567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3bc6db4d28a564350a4e9900fdf992bb455b93448bc0f64c5fbad0bea76da8`  
		Last Modified: Fri, 28 Jul 2023 00:23:48 GMT  
		Size: 68.8 MB (68800619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584274866dcb05649b337a249dc340029a4a5b359ef05fd57c4ade73be901175`  
		Last Modified: Fri, 28 Jul 2023 00:25:02 GMT  
		Size: 160.1 MB (160119309 bytes)  
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
$ docker pull mono@sha256:3b9876153cf5c1d1d6851372b14f02a4fc89bd4a9b1cb728f30766b88485dc24
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
$ docker pull mono@sha256:244c2a452e789e780cfc8afeb08ffc7e82222f183e7d1801155ae3ebd2d4fe31
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94742709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63b4ec69d3f5477554d095f405458f17f96471b81e653da1bf2301b579f96dd4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:29 GMT
ADD file:20e7ad6bec617357895302b08431eb3430cce3113bdf0a8ff9827115f858d313 in / 
# Thu, 27 Jul 2023 23:25:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 02:09:38 GMT
ENV MONO_VERSION=6.12.0.182
# Fri, 28 Jul 2023 02:09:47 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 28 Jul 2023 02:10:14 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3240fe174df9a5a4923c4b52f1d887dd1ad1a9ee69245c1fb867f399167584dd`  
		Last Modified: Thu, 27 Jul 2023 23:30:49 GMT  
		Size: 27.2 MB (27187431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe764ada48e9c07b599b90c63ebf3a1516f625cfe72cdf4ba823f1dfcd9e713`  
		Last Modified: Fri, 28 Jul 2023 02:20:05 GMT  
		Size: 2.8 MB (2780934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8209140f449ce8c93dde23e84011feda1a897dd0d7876f5cc4a254360ace6840`  
		Last Modified: Fri, 28 Jul 2023 02:20:14 GMT  
		Size: 64.8 MB (64774344 bytes)  
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
$ docker pull mono@sha256:e2a0784d2210c17aea82ca670401c851aab819882d06758dfb442a714345710d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48908739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ceea04ca6ea018102d4ffa23c11390bceca7108660a0db90e4c2c476b0463ae`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:42 GMT
ADD file:d2008875df919cb9817e6af97438428c2632113c1ef2b67b96607e184a7af941 in / 
# Tue, 04 Jul 2023 00:58:42 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:31:12 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 04 Jul 2023 06:31:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 04 Jul 2023 06:31:53 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:966944a300a7cf6431aa9fc3454d07eb7764f6b99d43a67de45ba53c30d69010`  
		Last Modified: Tue, 04 Jul 2023 01:04:17 GMT  
		Size: 22.7 MB (22747297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be94cc696a98d0e36d1f47670d4612782edee527ba65bb72a8b5128330db74d8`  
		Last Modified: Tue, 04 Jul 2023 06:35:30 GMT  
		Size: 2.4 MB (2370509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa72191f7045ac1a8fcb97997b3af65dab038d93dd285c50c65ca49534aa37ff`  
		Last Modified: Tue, 04 Jul 2023 06:35:34 GMT  
		Size: 23.8 MB (23790933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:658ec51415f0f6cd3ba15b340b3a4f86bda1c9410628b628282d876fa27ae5f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.1 MB (58112069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3803682e19eaccfbba33a5e261f5edf4db80b54cdc5a641c65a4c91aef3c2b88`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:58:08 GMT
ADD file:1368964550b1f674dd0365f72bb1d55cfebf5e3c651d49b5e168f9be97a6df76 in / 
# Tue, 04 Jul 2023 01:58:09 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:56:32 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 04 Jul 2023 03:56:40 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 04 Jul 2023 03:56:52 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:30bfbe1cefebb80f6f9d5d90c39fcdf9d6367bbc76fa68e33ea3b4391c0f9a77`  
		Last Modified: Tue, 04 Jul 2023 02:02:39 GMT  
		Size: 25.9 MB (25921455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99107951ff3754b1aeac3435c4535489d259e102359c031ccb790837666a0254`  
		Last Modified: Tue, 04 Jul 2023 04:00:27 GMT  
		Size: 2.6 MB (2645523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a3a83b2512643cf8777bd8cba8b9fc610132d25a87896c421fd37587d19c16`  
		Last Modified: Tue, 04 Jul 2023 04:00:30 GMT  
		Size: 29.5 MB (29545091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12-slim` - linux; 386

```console
$ docker pull mono@sha256:0436c43d2f9e492d4631868efa906eb9cdd910922385c0462185520ffaa12863
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99439994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c3f4516d8f9d9ea6bd9ec818e6b1d189c281e9937425b38353efa04dcfa0922`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:39:38 GMT
ADD file:a97f1ea317cafcf2810dfbe8ff5dfde5c43414d9cd1480b4e5f49d3ada8633f7 in / 
# Thu, 27 Jul 2023 23:39:38 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:17:04 GMT
ENV MONO_VERSION=6.12.0.182
# Fri, 28 Jul 2023 00:17:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 28 Jul 2023 00:17:51 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7eefe1e1e0f6af56fb4d37f33d6efcd121b57a2c33f6ce8272858d586e51f9d0`  
		Last Modified: Thu, 27 Jul 2023 23:44:57 GMT  
		Size: 27.8 MB (27846808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4faf5b429a2c65753fbcbf71ad8350c16724286c522a53fdeca6f8c9de6a894`  
		Last Modified: Fri, 28 Jul 2023 00:23:35 GMT  
		Size: 2.8 MB (2792567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3bc6db4d28a564350a4e9900fdf992bb455b93448bc0f64c5fbad0bea76da8`  
		Last Modified: Fri, 28 Jul 2023 00:23:48 GMT  
		Size: 68.8 MB (68800619 bytes)  
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
$ docker pull mono@sha256:f6aa5061fb9bc2b02181d353b20f053f5ca5f4a146754221c2e1eabaa4b723b1
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
$ docker pull mono@sha256:312c08a95ef6d46ef6e4c8fafdd00a3db2217a08a723b2522b34202587c4d022
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.7 MB (254674669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bdd38b14cfa4b2efc29dbdd11524b52dbce269382bba20486585d925feb75b4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:29 GMT
ADD file:20e7ad6bec617357895302b08431eb3430cce3113bdf0a8ff9827115f858d313 in / 
# Thu, 27 Jul 2023 23:25:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 02:09:38 GMT
ENV MONO_VERSION=6.12.0.182
# Fri, 28 Jul 2023 02:09:47 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 28 Jul 2023 02:10:14 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 28 Jul 2023 02:13:35 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3240fe174df9a5a4923c4b52f1d887dd1ad1a9ee69245c1fb867f399167584dd`  
		Last Modified: Thu, 27 Jul 2023 23:30:49 GMT  
		Size: 27.2 MB (27187431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe764ada48e9c07b599b90c63ebf3a1516f625cfe72cdf4ba823f1dfcd9e713`  
		Last Modified: Fri, 28 Jul 2023 02:20:05 GMT  
		Size: 2.8 MB (2780934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8209140f449ce8c93dde23e84011feda1a897dd0d7876f5cc4a254360ace6840`  
		Last Modified: Fri, 28 Jul 2023 02:20:14 GMT  
		Size: 64.8 MB (64774344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271c2c4f0ae1503f76d16d77b0a241d5be0f7d669404ae4df1b6ae7ee4deb3ce`  
		Last Modified: Fri, 28 Jul 2023 02:21:14 GMT  
		Size: 159.9 MB (159931960 bytes)  
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
$ docker pull mono@sha256:228365b9003bdbe155f3d1f786fc0e8d5a2b98e83c495b12a270f5337c8fb46a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.0 MB (188972314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37b28609e2e91c56b2be84cb3697f9ba18acf52db99ce37b3503f38b49378e05`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:42 GMT
ADD file:d2008875df919cb9817e6af97438428c2632113c1ef2b67b96607e184a7af941 in / 
# Tue, 04 Jul 2023 00:58:42 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:31:12 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 04 Jul 2023 06:31:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 04 Jul 2023 06:31:53 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 04 Jul 2023 06:33:51 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:966944a300a7cf6431aa9fc3454d07eb7764f6b99d43a67de45ba53c30d69010`  
		Last Modified: Tue, 04 Jul 2023 01:04:17 GMT  
		Size: 22.7 MB (22747297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be94cc696a98d0e36d1f47670d4612782edee527ba65bb72a8b5128330db74d8`  
		Last Modified: Tue, 04 Jul 2023 06:35:30 GMT  
		Size: 2.4 MB (2370509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa72191f7045ac1a8fcb97997b3af65dab038d93dd285c50c65ca49534aa37ff`  
		Last Modified: Tue, 04 Jul 2023 06:35:34 GMT  
		Size: 23.8 MB (23790933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4043418131df76e0b09bfaf3cb531466c9cfb585e2d3ededccb5cd061ac5f61`  
		Last Modified: Tue, 04 Jul 2023 06:36:33 GMT  
		Size: 140.1 MB (140063575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:40f7ed4f999fe484219df8a1e9b9fcc2fe65aa67500d21c88ce8d59284a4389a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.4 MB (216357868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4bf7d3fee3485c84588b0570a26e13c1a0f2f6e096cce8293a7f514a1a7330a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:58:08 GMT
ADD file:1368964550b1f674dd0365f72bb1d55cfebf5e3c651d49b5e168f9be97a6df76 in / 
# Tue, 04 Jul 2023 01:58:09 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:56:32 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 04 Jul 2023 03:56:40 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 04 Jul 2023 03:56:52 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 04 Jul 2023 03:58:21 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:30bfbe1cefebb80f6f9d5d90c39fcdf9d6367bbc76fa68e33ea3b4391c0f9a77`  
		Last Modified: Tue, 04 Jul 2023 02:02:39 GMT  
		Size: 25.9 MB (25921455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99107951ff3754b1aeac3435c4535489d259e102359c031ccb790837666a0254`  
		Last Modified: Tue, 04 Jul 2023 04:00:27 GMT  
		Size: 2.6 MB (2645523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a3a83b2512643cf8777bd8cba8b9fc610132d25a87896c421fd37587d19c16`  
		Last Modified: Tue, 04 Jul 2023 04:00:30 GMT  
		Size: 29.5 MB (29545091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56580de2946a5e2abae6377300a7c78a96f6203adc35b626f6ce779173618a4a`  
		Last Modified: Tue, 04 Jul 2023 04:01:18 GMT  
		Size: 158.2 MB (158245799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0` - linux; 386

```console
$ docker pull mono@sha256:1c5f4caca4cce6f99b6c360bca43499da6471f93cb3382548133c45c3301ff5b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.6 MB (259559303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afc318cff1d908e73180f1168f11a2d7e1327709c80436c93543d7e80222d7e6`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:39:38 GMT
ADD file:a97f1ea317cafcf2810dfbe8ff5dfde5c43414d9cd1480b4e5f49d3ada8633f7 in / 
# Thu, 27 Jul 2023 23:39:38 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:17:04 GMT
ENV MONO_VERSION=6.12.0.182
# Fri, 28 Jul 2023 00:17:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 28 Jul 2023 00:17:51 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 28 Jul 2023 00:20:55 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7eefe1e1e0f6af56fb4d37f33d6efcd121b57a2c33f6ce8272858d586e51f9d0`  
		Last Modified: Thu, 27 Jul 2023 23:44:57 GMT  
		Size: 27.8 MB (27846808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4faf5b429a2c65753fbcbf71ad8350c16724286c522a53fdeca6f8c9de6a894`  
		Last Modified: Fri, 28 Jul 2023 00:23:35 GMT  
		Size: 2.8 MB (2792567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3bc6db4d28a564350a4e9900fdf992bb455b93448bc0f64c5fbad0bea76da8`  
		Last Modified: Fri, 28 Jul 2023 00:23:48 GMT  
		Size: 68.8 MB (68800619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584274866dcb05649b337a249dc340029a4a5b359ef05fd57c4ade73be901175`  
		Last Modified: Fri, 28 Jul 2023 00:25:02 GMT  
		Size: 160.1 MB (160119309 bytes)  
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
$ docker pull mono@sha256:3b9876153cf5c1d1d6851372b14f02a4fc89bd4a9b1cb728f30766b88485dc24
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
$ docker pull mono@sha256:244c2a452e789e780cfc8afeb08ffc7e82222f183e7d1801155ae3ebd2d4fe31
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94742709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63b4ec69d3f5477554d095f405458f17f96471b81e653da1bf2301b579f96dd4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:29 GMT
ADD file:20e7ad6bec617357895302b08431eb3430cce3113bdf0a8ff9827115f858d313 in / 
# Thu, 27 Jul 2023 23:25:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 02:09:38 GMT
ENV MONO_VERSION=6.12.0.182
# Fri, 28 Jul 2023 02:09:47 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 28 Jul 2023 02:10:14 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3240fe174df9a5a4923c4b52f1d887dd1ad1a9ee69245c1fb867f399167584dd`  
		Last Modified: Thu, 27 Jul 2023 23:30:49 GMT  
		Size: 27.2 MB (27187431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe764ada48e9c07b599b90c63ebf3a1516f625cfe72cdf4ba823f1dfcd9e713`  
		Last Modified: Fri, 28 Jul 2023 02:20:05 GMT  
		Size: 2.8 MB (2780934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8209140f449ce8c93dde23e84011feda1a897dd0d7876f5cc4a254360ace6840`  
		Last Modified: Fri, 28 Jul 2023 02:20:14 GMT  
		Size: 64.8 MB (64774344 bytes)  
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
$ docker pull mono@sha256:e2a0784d2210c17aea82ca670401c851aab819882d06758dfb442a714345710d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48908739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ceea04ca6ea018102d4ffa23c11390bceca7108660a0db90e4c2c476b0463ae`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:42 GMT
ADD file:d2008875df919cb9817e6af97438428c2632113c1ef2b67b96607e184a7af941 in / 
# Tue, 04 Jul 2023 00:58:42 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:31:12 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 04 Jul 2023 06:31:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 04 Jul 2023 06:31:53 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:966944a300a7cf6431aa9fc3454d07eb7764f6b99d43a67de45ba53c30d69010`  
		Last Modified: Tue, 04 Jul 2023 01:04:17 GMT  
		Size: 22.7 MB (22747297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be94cc696a98d0e36d1f47670d4612782edee527ba65bb72a8b5128330db74d8`  
		Last Modified: Tue, 04 Jul 2023 06:35:30 GMT  
		Size: 2.4 MB (2370509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa72191f7045ac1a8fcb97997b3af65dab038d93dd285c50c65ca49534aa37ff`  
		Last Modified: Tue, 04 Jul 2023 06:35:34 GMT  
		Size: 23.8 MB (23790933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:658ec51415f0f6cd3ba15b340b3a4f86bda1c9410628b628282d876fa27ae5f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.1 MB (58112069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3803682e19eaccfbba33a5e261f5edf4db80b54cdc5a641c65a4c91aef3c2b88`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:58:08 GMT
ADD file:1368964550b1f674dd0365f72bb1d55cfebf5e3c651d49b5e168f9be97a6df76 in / 
# Tue, 04 Jul 2023 01:58:09 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:56:32 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 04 Jul 2023 03:56:40 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 04 Jul 2023 03:56:52 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:30bfbe1cefebb80f6f9d5d90c39fcdf9d6367bbc76fa68e33ea3b4391c0f9a77`  
		Last Modified: Tue, 04 Jul 2023 02:02:39 GMT  
		Size: 25.9 MB (25921455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99107951ff3754b1aeac3435c4535489d259e102359c031ccb790837666a0254`  
		Last Modified: Tue, 04 Jul 2023 04:00:27 GMT  
		Size: 2.6 MB (2645523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a3a83b2512643cf8777bd8cba8b9fc610132d25a87896c421fd37587d19c16`  
		Last Modified: Tue, 04 Jul 2023 04:00:30 GMT  
		Size: 29.5 MB (29545091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0-slim` - linux; 386

```console
$ docker pull mono@sha256:0436c43d2f9e492d4631868efa906eb9cdd910922385c0462185520ffaa12863
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99439994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c3f4516d8f9d9ea6bd9ec818e6b1d189c281e9937425b38353efa04dcfa0922`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:39:38 GMT
ADD file:a97f1ea317cafcf2810dfbe8ff5dfde5c43414d9cd1480b4e5f49d3ada8633f7 in / 
# Thu, 27 Jul 2023 23:39:38 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:17:04 GMT
ENV MONO_VERSION=6.12.0.182
# Fri, 28 Jul 2023 00:17:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 28 Jul 2023 00:17:51 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7eefe1e1e0f6af56fb4d37f33d6efcd121b57a2c33f6ce8272858d586e51f9d0`  
		Last Modified: Thu, 27 Jul 2023 23:44:57 GMT  
		Size: 27.8 MB (27846808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4faf5b429a2c65753fbcbf71ad8350c16724286c522a53fdeca6f8c9de6a894`  
		Last Modified: Fri, 28 Jul 2023 00:23:35 GMT  
		Size: 2.8 MB (2792567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3bc6db4d28a564350a4e9900fdf992bb455b93448bc0f64c5fbad0bea76da8`  
		Last Modified: Fri, 28 Jul 2023 00:23:48 GMT  
		Size: 68.8 MB (68800619 bytes)  
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
$ docker pull mono@sha256:f6aa5061fb9bc2b02181d353b20f053f5ca5f4a146754221c2e1eabaa4b723b1
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
$ docker pull mono@sha256:312c08a95ef6d46ef6e4c8fafdd00a3db2217a08a723b2522b34202587c4d022
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.7 MB (254674669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bdd38b14cfa4b2efc29dbdd11524b52dbce269382bba20486585d925feb75b4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:29 GMT
ADD file:20e7ad6bec617357895302b08431eb3430cce3113bdf0a8ff9827115f858d313 in / 
# Thu, 27 Jul 2023 23:25:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 02:09:38 GMT
ENV MONO_VERSION=6.12.0.182
# Fri, 28 Jul 2023 02:09:47 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 28 Jul 2023 02:10:14 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 28 Jul 2023 02:13:35 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3240fe174df9a5a4923c4b52f1d887dd1ad1a9ee69245c1fb867f399167584dd`  
		Last Modified: Thu, 27 Jul 2023 23:30:49 GMT  
		Size: 27.2 MB (27187431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe764ada48e9c07b599b90c63ebf3a1516f625cfe72cdf4ba823f1dfcd9e713`  
		Last Modified: Fri, 28 Jul 2023 02:20:05 GMT  
		Size: 2.8 MB (2780934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8209140f449ce8c93dde23e84011feda1a897dd0d7876f5cc4a254360ace6840`  
		Last Modified: Fri, 28 Jul 2023 02:20:14 GMT  
		Size: 64.8 MB (64774344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271c2c4f0ae1503f76d16d77b0a241d5be0f7d669404ae4df1b6ae7ee4deb3ce`  
		Last Modified: Fri, 28 Jul 2023 02:21:14 GMT  
		Size: 159.9 MB (159931960 bytes)  
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
$ docker pull mono@sha256:228365b9003bdbe155f3d1f786fc0e8d5a2b98e83c495b12a270f5337c8fb46a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.0 MB (188972314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37b28609e2e91c56b2be84cb3697f9ba18acf52db99ce37b3503f38b49378e05`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:42 GMT
ADD file:d2008875df919cb9817e6af97438428c2632113c1ef2b67b96607e184a7af941 in / 
# Tue, 04 Jul 2023 00:58:42 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:31:12 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 04 Jul 2023 06:31:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 04 Jul 2023 06:31:53 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 04 Jul 2023 06:33:51 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:966944a300a7cf6431aa9fc3454d07eb7764f6b99d43a67de45ba53c30d69010`  
		Last Modified: Tue, 04 Jul 2023 01:04:17 GMT  
		Size: 22.7 MB (22747297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be94cc696a98d0e36d1f47670d4612782edee527ba65bb72a8b5128330db74d8`  
		Last Modified: Tue, 04 Jul 2023 06:35:30 GMT  
		Size: 2.4 MB (2370509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa72191f7045ac1a8fcb97997b3af65dab038d93dd285c50c65ca49534aa37ff`  
		Last Modified: Tue, 04 Jul 2023 06:35:34 GMT  
		Size: 23.8 MB (23790933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4043418131df76e0b09bfaf3cb531466c9cfb585e2d3ededccb5cd061ac5f61`  
		Last Modified: Tue, 04 Jul 2023 06:36:33 GMT  
		Size: 140.1 MB (140063575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.182` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:40f7ed4f999fe484219df8a1e9b9fcc2fe65aa67500d21c88ce8d59284a4389a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.4 MB (216357868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4bf7d3fee3485c84588b0570a26e13c1a0f2f6e096cce8293a7f514a1a7330a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:58:08 GMT
ADD file:1368964550b1f674dd0365f72bb1d55cfebf5e3c651d49b5e168f9be97a6df76 in / 
# Tue, 04 Jul 2023 01:58:09 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:56:32 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 04 Jul 2023 03:56:40 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 04 Jul 2023 03:56:52 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 04 Jul 2023 03:58:21 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:30bfbe1cefebb80f6f9d5d90c39fcdf9d6367bbc76fa68e33ea3b4391c0f9a77`  
		Last Modified: Tue, 04 Jul 2023 02:02:39 GMT  
		Size: 25.9 MB (25921455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99107951ff3754b1aeac3435c4535489d259e102359c031ccb790837666a0254`  
		Last Modified: Tue, 04 Jul 2023 04:00:27 GMT  
		Size: 2.6 MB (2645523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a3a83b2512643cf8777bd8cba8b9fc610132d25a87896c421fd37587d19c16`  
		Last Modified: Tue, 04 Jul 2023 04:00:30 GMT  
		Size: 29.5 MB (29545091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56580de2946a5e2abae6377300a7c78a96f6203adc35b626f6ce779173618a4a`  
		Last Modified: Tue, 04 Jul 2023 04:01:18 GMT  
		Size: 158.2 MB (158245799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.182` - linux; 386

```console
$ docker pull mono@sha256:1c5f4caca4cce6f99b6c360bca43499da6471f93cb3382548133c45c3301ff5b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.6 MB (259559303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afc318cff1d908e73180f1168f11a2d7e1327709c80436c93543d7e80222d7e6`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:39:38 GMT
ADD file:a97f1ea317cafcf2810dfbe8ff5dfde5c43414d9cd1480b4e5f49d3ada8633f7 in / 
# Thu, 27 Jul 2023 23:39:38 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:17:04 GMT
ENV MONO_VERSION=6.12.0.182
# Fri, 28 Jul 2023 00:17:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 28 Jul 2023 00:17:51 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 28 Jul 2023 00:20:55 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7eefe1e1e0f6af56fb4d37f33d6efcd121b57a2c33f6ce8272858d586e51f9d0`  
		Last Modified: Thu, 27 Jul 2023 23:44:57 GMT  
		Size: 27.8 MB (27846808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4faf5b429a2c65753fbcbf71ad8350c16724286c522a53fdeca6f8c9de6a894`  
		Last Modified: Fri, 28 Jul 2023 00:23:35 GMT  
		Size: 2.8 MB (2792567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3bc6db4d28a564350a4e9900fdf992bb455b93448bc0f64c5fbad0bea76da8`  
		Last Modified: Fri, 28 Jul 2023 00:23:48 GMT  
		Size: 68.8 MB (68800619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584274866dcb05649b337a249dc340029a4a5b359ef05fd57c4ade73be901175`  
		Last Modified: Fri, 28 Jul 2023 00:25:02 GMT  
		Size: 160.1 MB (160119309 bytes)  
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
$ docker pull mono@sha256:3b9876153cf5c1d1d6851372b14f02a4fc89bd4a9b1cb728f30766b88485dc24
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
$ docker pull mono@sha256:244c2a452e789e780cfc8afeb08ffc7e82222f183e7d1801155ae3ebd2d4fe31
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94742709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63b4ec69d3f5477554d095f405458f17f96471b81e653da1bf2301b579f96dd4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:29 GMT
ADD file:20e7ad6bec617357895302b08431eb3430cce3113bdf0a8ff9827115f858d313 in / 
# Thu, 27 Jul 2023 23:25:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 02:09:38 GMT
ENV MONO_VERSION=6.12.0.182
# Fri, 28 Jul 2023 02:09:47 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 28 Jul 2023 02:10:14 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3240fe174df9a5a4923c4b52f1d887dd1ad1a9ee69245c1fb867f399167584dd`  
		Last Modified: Thu, 27 Jul 2023 23:30:49 GMT  
		Size: 27.2 MB (27187431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe764ada48e9c07b599b90c63ebf3a1516f625cfe72cdf4ba823f1dfcd9e713`  
		Last Modified: Fri, 28 Jul 2023 02:20:05 GMT  
		Size: 2.8 MB (2780934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8209140f449ce8c93dde23e84011feda1a897dd0d7876f5cc4a254360ace6840`  
		Last Modified: Fri, 28 Jul 2023 02:20:14 GMT  
		Size: 64.8 MB (64774344 bytes)  
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
$ docker pull mono@sha256:e2a0784d2210c17aea82ca670401c851aab819882d06758dfb442a714345710d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48908739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ceea04ca6ea018102d4ffa23c11390bceca7108660a0db90e4c2c476b0463ae`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:42 GMT
ADD file:d2008875df919cb9817e6af97438428c2632113c1ef2b67b96607e184a7af941 in / 
# Tue, 04 Jul 2023 00:58:42 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:31:12 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 04 Jul 2023 06:31:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 04 Jul 2023 06:31:53 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:966944a300a7cf6431aa9fc3454d07eb7764f6b99d43a67de45ba53c30d69010`  
		Last Modified: Tue, 04 Jul 2023 01:04:17 GMT  
		Size: 22.7 MB (22747297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be94cc696a98d0e36d1f47670d4612782edee527ba65bb72a8b5128330db74d8`  
		Last Modified: Tue, 04 Jul 2023 06:35:30 GMT  
		Size: 2.4 MB (2370509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa72191f7045ac1a8fcb97997b3af65dab038d93dd285c50c65ca49534aa37ff`  
		Last Modified: Tue, 04 Jul 2023 06:35:34 GMT  
		Size: 23.8 MB (23790933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.182-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:658ec51415f0f6cd3ba15b340b3a4f86bda1c9410628b628282d876fa27ae5f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.1 MB (58112069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3803682e19eaccfbba33a5e261f5edf4db80b54cdc5a641c65a4c91aef3c2b88`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:58:08 GMT
ADD file:1368964550b1f674dd0365f72bb1d55cfebf5e3c651d49b5e168f9be97a6df76 in / 
# Tue, 04 Jul 2023 01:58:09 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:56:32 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 04 Jul 2023 03:56:40 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 04 Jul 2023 03:56:52 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:30bfbe1cefebb80f6f9d5d90c39fcdf9d6367bbc76fa68e33ea3b4391c0f9a77`  
		Last Modified: Tue, 04 Jul 2023 02:02:39 GMT  
		Size: 25.9 MB (25921455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99107951ff3754b1aeac3435c4535489d259e102359c031ccb790837666a0254`  
		Last Modified: Tue, 04 Jul 2023 04:00:27 GMT  
		Size: 2.6 MB (2645523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a3a83b2512643cf8777bd8cba8b9fc610132d25a87896c421fd37587d19c16`  
		Last Modified: Tue, 04 Jul 2023 04:00:30 GMT  
		Size: 29.5 MB (29545091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.182-slim` - linux; 386

```console
$ docker pull mono@sha256:0436c43d2f9e492d4631868efa906eb9cdd910922385c0462185520ffaa12863
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99439994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c3f4516d8f9d9ea6bd9ec818e6b1d189c281e9937425b38353efa04dcfa0922`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:39:38 GMT
ADD file:a97f1ea317cafcf2810dfbe8ff5dfde5c43414d9cd1480b4e5f49d3ada8633f7 in / 
# Thu, 27 Jul 2023 23:39:38 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:17:04 GMT
ENV MONO_VERSION=6.12.0.182
# Fri, 28 Jul 2023 00:17:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 28 Jul 2023 00:17:51 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7eefe1e1e0f6af56fb4d37f33d6efcd121b57a2c33f6ce8272858d586e51f9d0`  
		Last Modified: Thu, 27 Jul 2023 23:44:57 GMT  
		Size: 27.8 MB (27846808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4faf5b429a2c65753fbcbf71ad8350c16724286c522a53fdeca6f8c9de6a894`  
		Last Modified: Fri, 28 Jul 2023 00:23:35 GMT  
		Size: 2.8 MB (2792567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3bc6db4d28a564350a4e9900fdf992bb455b93448bc0f64c5fbad0bea76da8`  
		Last Modified: Fri, 28 Jul 2023 00:23:48 GMT  
		Size: 68.8 MB (68800619 bytes)  
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
$ docker pull mono@sha256:f6aa5061fb9bc2b02181d353b20f053f5ca5f4a146754221c2e1eabaa4b723b1
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
$ docker pull mono@sha256:312c08a95ef6d46ef6e4c8fafdd00a3db2217a08a723b2522b34202587c4d022
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.7 MB (254674669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bdd38b14cfa4b2efc29dbdd11524b52dbce269382bba20486585d925feb75b4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:29 GMT
ADD file:20e7ad6bec617357895302b08431eb3430cce3113bdf0a8ff9827115f858d313 in / 
# Thu, 27 Jul 2023 23:25:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 02:09:38 GMT
ENV MONO_VERSION=6.12.0.182
# Fri, 28 Jul 2023 02:09:47 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 28 Jul 2023 02:10:14 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 28 Jul 2023 02:13:35 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3240fe174df9a5a4923c4b52f1d887dd1ad1a9ee69245c1fb867f399167584dd`  
		Last Modified: Thu, 27 Jul 2023 23:30:49 GMT  
		Size: 27.2 MB (27187431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe764ada48e9c07b599b90c63ebf3a1516f625cfe72cdf4ba823f1dfcd9e713`  
		Last Modified: Fri, 28 Jul 2023 02:20:05 GMT  
		Size: 2.8 MB (2780934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8209140f449ce8c93dde23e84011feda1a897dd0d7876f5cc4a254360ace6840`  
		Last Modified: Fri, 28 Jul 2023 02:20:14 GMT  
		Size: 64.8 MB (64774344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271c2c4f0ae1503f76d16d77b0a241d5be0f7d669404ae4df1b6ae7ee4deb3ce`  
		Last Modified: Fri, 28 Jul 2023 02:21:14 GMT  
		Size: 159.9 MB (159931960 bytes)  
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
$ docker pull mono@sha256:228365b9003bdbe155f3d1f786fc0e8d5a2b98e83c495b12a270f5337c8fb46a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.0 MB (188972314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37b28609e2e91c56b2be84cb3697f9ba18acf52db99ce37b3503f38b49378e05`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:42 GMT
ADD file:d2008875df919cb9817e6af97438428c2632113c1ef2b67b96607e184a7af941 in / 
# Tue, 04 Jul 2023 00:58:42 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:31:12 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 04 Jul 2023 06:31:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 04 Jul 2023 06:31:53 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 04 Jul 2023 06:33:51 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:966944a300a7cf6431aa9fc3454d07eb7764f6b99d43a67de45ba53c30d69010`  
		Last Modified: Tue, 04 Jul 2023 01:04:17 GMT  
		Size: 22.7 MB (22747297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be94cc696a98d0e36d1f47670d4612782edee527ba65bb72a8b5128330db74d8`  
		Last Modified: Tue, 04 Jul 2023 06:35:30 GMT  
		Size: 2.4 MB (2370509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa72191f7045ac1a8fcb97997b3af65dab038d93dd285c50c65ca49534aa37ff`  
		Last Modified: Tue, 04 Jul 2023 06:35:34 GMT  
		Size: 23.8 MB (23790933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4043418131df76e0b09bfaf3cb531466c9cfb585e2d3ededccb5cd061ac5f61`  
		Last Modified: Tue, 04 Jul 2023 06:36:33 GMT  
		Size: 140.1 MB (140063575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:40f7ed4f999fe484219df8a1e9b9fcc2fe65aa67500d21c88ce8d59284a4389a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.4 MB (216357868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4bf7d3fee3485c84588b0570a26e13c1a0f2f6e096cce8293a7f514a1a7330a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:58:08 GMT
ADD file:1368964550b1f674dd0365f72bb1d55cfebf5e3c651d49b5e168f9be97a6df76 in / 
# Tue, 04 Jul 2023 01:58:09 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:56:32 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 04 Jul 2023 03:56:40 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 04 Jul 2023 03:56:52 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 04 Jul 2023 03:58:21 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:30bfbe1cefebb80f6f9d5d90c39fcdf9d6367bbc76fa68e33ea3b4391c0f9a77`  
		Last Modified: Tue, 04 Jul 2023 02:02:39 GMT  
		Size: 25.9 MB (25921455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99107951ff3754b1aeac3435c4535489d259e102359c031ccb790837666a0254`  
		Last Modified: Tue, 04 Jul 2023 04:00:27 GMT  
		Size: 2.6 MB (2645523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a3a83b2512643cf8777bd8cba8b9fc610132d25a87896c421fd37587d19c16`  
		Last Modified: Tue, 04 Jul 2023 04:00:30 GMT  
		Size: 29.5 MB (29545091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56580de2946a5e2abae6377300a7c78a96f6203adc35b626f6ce779173618a4a`  
		Last Modified: Tue, 04 Jul 2023 04:01:18 GMT  
		Size: 158.2 MB (158245799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; 386

```console
$ docker pull mono@sha256:1c5f4caca4cce6f99b6c360bca43499da6471f93cb3382548133c45c3301ff5b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.6 MB (259559303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afc318cff1d908e73180f1168f11a2d7e1327709c80436c93543d7e80222d7e6`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:39:38 GMT
ADD file:a97f1ea317cafcf2810dfbe8ff5dfde5c43414d9cd1480b4e5f49d3ada8633f7 in / 
# Thu, 27 Jul 2023 23:39:38 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:17:04 GMT
ENV MONO_VERSION=6.12.0.182
# Fri, 28 Jul 2023 00:17:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 28 Jul 2023 00:17:51 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 28 Jul 2023 00:20:55 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7eefe1e1e0f6af56fb4d37f33d6efcd121b57a2c33f6ce8272858d586e51f9d0`  
		Last Modified: Thu, 27 Jul 2023 23:44:57 GMT  
		Size: 27.8 MB (27846808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4faf5b429a2c65753fbcbf71ad8350c16724286c522a53fdeca6f8c9de6a894`  
		Last Modified: Fri, 28 Jul 2023 00:23:35 GMT  
		Size: 2.8 MB (2792567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3bc6db4d28a564350a4e9900fdf992bb455b93448bc0f64c5fbad0bea76da8`  
		Last Modified: Fri, 28 Jul 2023 00:23:48 GMT  
		Size: 68.8 MB (68800619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584274866dcb05649b337a249dc340029a4a5b359ef05fd57c4ade73be901175`  
		Last Modified: Fri, 28 Jul 2023 00:25:02 GMT  
		Size: 160.1 MB (160119309 bytes)  
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
$ docker pull mono@sha256:3b9876153cf5c1d1d6851372b14f02a4fc89bd4a9b1cb728f30766b88485dc24
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
$ docker pull mono@sha256:244c2a452e789e780cfc8afeb08ffc7e82222f183e7d1801155ae3ebd2d4fe31
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94742709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63b4ec69d3f5477554d095f405458f17f96471b81e653da1bf2301b579f96dd4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:29 GMT
ADD file:20e7ad6bec617357895302b08431eb3430cce3113bdf0a8ff9827115f858d313 in / 
# Thu, 27 Jul 2023 23:25:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 02:09:38 GMT
ENV MONO_VERSION=6.12.0.182
# Fri, 28 Jul 2023 02:09:47 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 28 Jul 2023 02:10:14 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3240fe174df9a5a4923c4b52f1d887dd1ad1a9ee69245c1fb867f399167584dd`  
		Last Modified: Thu, 27 Jul 2023 23:30:49 GMT  
		Size: 27.2 MB (27187431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe764ada48e9c07b599b90c63ebf3a1516f625cfe72cdf4ba823f1dfcd9e713`  
		Last Modified: Fri, 28 Jul 2023 02:20:05 GMT  
		Size: 2.8 MB (2780934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8209140f449ce8c93dde23e84011feda1a897dd0d7876f5cc4a254360ace6840`  
		Last Modified: Fri, 28 Jul 2023 02:20:14 GMT  
		Size: 64.8 MB (64774344 bytes)  
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
$ docker pull mono@sha256:e2a0784d2210c17aea82ca670401c851aab819882d06758dfb442a714345710d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48908739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ceea04ca6ea018102d4ffa23c11390bceca7108660a0db90e4c2c476b0463ae`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:42 GMT
ADD file:d2008875df919cb9817e6af97438428c2632113c1ef2b67b96607e184a7af941 in / 
# Tue, 04 Jul 2023 00:58:42 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:31:12 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 04 Jul 2023 06:31:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 04 Jul 2023 06:31:53 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:966944a300a7cf6431aa9fc3454d07eb7764f6b99d43a67de45ba53c30d69010`  
		Last Modified: Tue, 04 Jul 2023 01:04:17 GMT  
		Size: 22.7 MB (22747297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be94cc696a98d0e36d1f47670d4612782edee527ba65bb72a8b5128330db74d8`  
		Last Modified: Tue, 04 Jul 2023 06:35:30 GMT  
		Size: 2.4 MB (2370509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa72191f7045ac1a8fcb97997b3af65dab038d93dd285c50c65ca49534aa37ff`  
		Last Modified: Tue, 04 Jul 2023 06:35:34 GMT  
		Size: 23.8 MB (23790933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:658ec51415f0f6cd3ba15b340b3a4f86bda1c9410628b628282d876fa27ae5f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.1 MB (58112069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3803682e19eaccfbba33a5e261f5edf4db80b54cdc5a641c65a4c91aef3c2b88`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:58:08 GMT
ADD file:1368964550b1f674dd0365f72bb1d55cfebf5e3c651d49b5e168f9be97a6df76 in / 
# Tue, 04 Jul 2023 01:58:09 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:56:32 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 04 Jul 2023 03:56:40 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 04 Jul 2023 03:56:52 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:30bfbe1cefebb80f6f9d5d90c39fcdf9d6367bbc76fa68e33ea3b4391c0f9a77`  
		Last Modified: Tue, 04 Jul 2023 02:02:39 GMT  
		Size: 25.9 MB (25921455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99107951ff3754b1aeac3435c4535489d259e102359c031ccb790837666a0254`  
		Last Modified: Tue, 04 Jul 2023 04:00:27 GMT  
		Size: 2.6 MB (2645523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a3a83b2512643cf8777bd8cba8b9fc610132d25a87896c421fd37587d19c16`  
		Last Modified: Tue, 04 Jul 2023 04:00:30 GMT  
		Size: 29.5 MB (29545091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; 386

```console
$ docker pull mono@sha256:0436c43d2f9e492d4631868efa906eb9cdd910922385c0462185520ffaa12863
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99439994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c3f4516d8f9d9ea6bd9ec818e6b1d189c281e9937425b38353efa04dcfa0922`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:39:38 GMT
ADD file:a97f1ea317cafcf2810dfbe8ff5dfde5c43414d9cd1480b4e5f49d3ada8633f7 in / 
# Thu, 27 Jul 2023 23:39:38 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:17:04 GMT
ENV MONO_VERSION=6.12.0.182
# Fri, 28 Jul 2023 00:17:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 28 Jul 2023 00:17:51 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7eefe1e1e0f6af56fb4d37f33d6efcd121b57a2c33f6ce8272858d586e51f9d0`  
		Last Modified: Thu, 27 Jul 2023 23:44:57 GMT  
		Size: 27.8 MB (27846808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4faf5b429a2c65753fbcbf71ad8350c16724286c522a53fdeca6f8c9de6a894`  
		Last Modified: Fri, 28 Jul 2023 00:23:35 GMT  
		Size: 2.8 MB (2792567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3bc6db4d28a564350a4e9900fdf992bb455b93448bc0f64c5fbad0bea76da8`  
		Last Modified: Fri, 28 Jul 2023 00:23:48 GMT  
		Size: 68.8 MB (68800619 bytes)  
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
