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
$ docker pull mono@sha256:c12127bb8f71a7c6e0b13776c9d4221178e12e66dd30eabd5576a2477951754d
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
$ docker pull mono@sha256:18d3fdaf18efe584c791dc668f67459b087287c2f3f44b1aa912d53cff9d0af5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.3 MB (218271546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e067982592a2865379ccfeb3b0082e70e15de3452e86a7683bd19279cb10ef05`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:08 GMT
ADD file:e077f4d014ea0869fc4b3d5a3e6b3c8b792a97a8b4a328f33a994369225ff222 in / 
# Tue, 31 Mar 2020 01:24:08 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 20:55:51 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 31 Mar 2020 20:56:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 31 Mar 2020 20:56:28 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 31 Mar 2020 21:27:00 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:48839397421a64189661c2b86a34eb515d09a28204587a2b06b59df9f6e2d786`  
		Last Modified: Tue, 31 Mar 2020 01:29:28 GMT  
		Size: 22.5 MB (22513374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b5755347d44e006a3743488432c6a77d081bcc3b67cee3609370ca29e83804`  
		Last Modified: Tue, 31 Mar 2020 21:27:55 GMT  
		Size: 244.5 KB (244461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652e7215b25a09c4468906d2f9dd0e353a17465cc5be4ce2a3d2c093ea079f75`  
		Last Modified: Tue, 31 Mar 2020 21:28:08 GMT  
		Size: 55.5 MB (55519226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4f8b06dfd3bb1ae8411acd5538c4c0380f2aad99867fec747bfbbc2f479ccb`  
		Last Modified: Tue, 31 Mar 2020 21:30:48 GMT  
		Size: 140.0 MB (139994485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5` - linux; arm variant v5

```console
$ docker pull mono@sha256:728b3a09731eabb589d971feaf17a5833942c6843ab9cd8358b32ff1b6383cd9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.9 MB (170941920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ee915002d6e2050563346a5fc0731204436dda9794421c36437fc915a77105d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:54:51 GMT
ADD file:ba6c5e03457e69f59231e8e7c6465c1ec985812f0d8f7a65d9842f2be3e947fb in / 
# Thu, 16 Apr 2020 00:54:54 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 03:25:11 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 16 Apr 2020 03:25:36 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 03:26:21 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 03:35:41 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b7d527e4baf13a6c926fb354fe1b38cb42b96f249ae65fdc0f52c853b654e06e`  
		Last Modified: Thu, 16 Apr 2020 01:02:32 GMT  
		Size: 21.2 MB (21190797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8340381d358ecc9e44596343db49a1d8fe9fc408313742adb549d7acbfa010d9`  
		Last Modified: Thu, 16 Apr 2020 03:36:49 GMT  
		Size: 244.5 KB (244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c829c702c9ea78e5f1e834e27d5270a1aeb340e0c387fd2bcca835a6508a18`  
		Last Modified: Thu, 16 Apr 2020 03:36:59 GMT  
		Size: 24.3 MB (24265251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26391aed7c1279d19a1ba1f92bea83bd9306ccb069b953d6af33c408532dccc7`  
		Last Modified: Thu, 16 Apr 2020 03:39:37 GMT  
		Size: 125.2 MB (125241339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5` - linux; arm variant v7

```console
$ docker pull mono@sha256:259a95f5c94430a70d4bfbb3aff1c86b1c46f66e932e58986f5eb0d57da28d35
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.0 MB (166993370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25818813ac0ce16ba21dc50510c7e882df7888a2fde8c2e99ecdcfd9d9bc02f9`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:05:08 GMT
ADD file:e37c4728c0c89ac126542ac35e7e493425c021bfac751079c9b266821a1b4e99 in / 
# Thu, 16 Apr 2020 01:05:10 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:43:14 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 16 Apr 2020 04:43:33 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 04:44:18 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 04:53:30 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f78d9963dfddc4747d6200353b50f6093a6e37ca82e1612fa397d64ff13e7299`  
		Last Modified: Thu, 16 Apr 2020 01:12:33 GMT  
		Size: 19.3 MB (19298546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf684cdea8a2272c82e09cbbb5024552c6e67b7dcf59ea62af547f9c730474e`  
		Last Modified: Thu, 16 Apr 2020 04:54:37 GMT  
		Size: 244.6 KB (244560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249d36139d8bc596df209162b7386211edf003733b4286aa7405033282389c33`  
		Last Modified: Thu, 16 Apr 2020 04:54:47 GMT  
		Size: 23.6 MB (23562096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90019bfc9c5e3ea379d7a72fbc13f136f207f2c152f545a4225d506472e4cec`  
		Last Modified: Thu, 16 Apr 2020 04:57:32 GMT  
		Size: 123.9 MB (123888168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:110949e51fd64f0a4861ad92137d717f431d06f6d24f8e519a5cf346185fde38
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.8 MB (187800067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d6f3e069a025df695d5e7cdae84f0ad9c50ec134a1ef7ed87c306daf10c4955`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 02:45:19 GMT
ADD file:1588320d1c43714ec0353b7471f2ffd649045ca0f5f70dcb1eb064875fff9578 in / 
# Thu, 16 Apr 2020 02:45:21 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:49:41 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 16 Apr 2020 06:50:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:50:40 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 06:58:49 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8978c87ff45d64d1663a585dcf1ed66d9e711c2e4048d83ef561da9514ef46e6`  
		Last Modified: Thu, 16 Apr 2020 02:51:32 GMT  
		Size: 20.4 MB (20370106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554199a06aed010aa14e2e6ed810ac12e3f7ea1f01b4b484029b46c769a914b5`  
		Last Modified: Thu, 16 Apr 2020 07:00:00 GMT  
		Size: 244.4 KB (244384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f9c219c23779432f95dca105f2822e4e5cce0035ec90439890cb4ba1c4b3e0`  
		Last Modified: Thu, 16 Apr 2020 07:00:06 GMT  
		Size: 28.2 MB (28156920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706e37f95124ae6304e93e036c626bc45828f29f97c939ca3dc7b4d8d51e31f6`  
		Last Modified: Thu, 16 Apr 2020 07:02:52 GMT  
		Size: 139.0 MB (139028657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5` - linux; 386

```console
$ docker pull mono@sha256:8ddc25e668dd9f7369fc232cb2b192e58406adb44e30ce9554fa03667fb3ccb2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.8 MB (227783415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e2f7e8e74fa090030747657f6f35d85803a5713cd0745c0b40174549145ce02`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:24 GMT
ADD file:0e72ab6d3f5ce06d7170bd6b0ceeda8687d1a5e2dab40308a8b8960d67fceffe in / 
# Thu, 16 Apr 2020 01:43:24 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:20:38 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 16 Apr 2020 06:20:48 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:21:29 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 06:29:49 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:706a1cdc903b54148ad6d5b672b2bafacadd79daffc0487b4949dd5d193f96f8`  
		Last Modified: Thu, 16 Apr 2020 01:49:33 GMT  
		Size: 23.1 MB (23141457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940906367b61b1c8c02650fa596d87e143b9b9e32639b66e59d0bbd65115133a`  
		Last Modified: Thu, 16 Apr 2020 06:31:23 GMT  
		Size: 244.5 KB (244472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f8edae7689fc4d1bd35e9614dfe86e03e42588bece0cf4d18c3b6c18e651c41`  
		Last Modified: Thu, 16 Apr 2020 06:31:48 GMT  
		Size: 58.6 MB (58557430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e09172c98cd791ef5c541987e57ef03eb73f70dd5c831af61d628cc60a85268c`  
		Last Modified: Thu, 16 Apr 2020 06:35:22 GMT  
		Size: 145.8 MB (145840056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5` - linux; ppc64le

```console
$ docker pull mono@sha256:10f28b145295a978f9628fb30440d346accccf597d45f8b66e8d390fb00f5d12
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.3 MB (173292013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69236ccfa3a77e72c4d43a2c28acf141d1bebac5e126f5c9e4a764fa4b508c23`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:57 GMT
ADD file:1c7f60f778e4b93490d570487d56275925e5eb477632e71cb9f035ce6edf2460 in / 
# Thu, 16 Apr 2020 01:44:03 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:44:48 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 16 Apr 2020 06:46:25 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:47:57 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 07:18:06 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:15e508b90ba1d327da83b72fc494ca263c1566ef6f70b91001cf2093395ffa3d`  
		Last Modified: Thu, 16 Apr 2020 02:04:33 GMT  
		Size: 22.8 MB (22785425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f669c3fbfce943d77701b69e7857eb6d1b88bbf7f9167a449d80be23eb3243`  
		Last Modified: Thu, 16 Apr 2020 07:19:18 GMT  
		Size: 244.6 KB (244638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c16782e8edab25bcd823ec760e3d334f1009343a5a1ef80520730ea6acd56e3`  
		Last Modified: Thu, 16 Apr 2020 07:19:25 GMT  
		Size: 24.6 MB (24639647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8407cfcba2823e2d7d5cf4a042cc54da9defa5fb96119e64542272d1eb1ff98e`  
		Last Modified: Thu, 16 Apr 2020 07:21:36 GMT  
		Size: 125.6 MB (125622303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.20`

```console
$ docker pull mono@sha256:c12127bb8f71a7c6e0b13776c9d4221178e12e66dd30eabd5576a2477951754d
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
$ docker pull mono@sha256:18d3fdaf18efe584c791dc668f67459b087287c2f3f44b1aa912d53cff9d0af5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.3 MB (218271546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e067982592a2865379ccfeb3b0082e70e15de3452e86a7683bd19279cb10ef05`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:08 GMT
ADD file:e077f4d014ea0869fc4b3d5a3e6b3c8b792a97a8b4a328f33a994369225ff222 in / 
# Tue, 31 Mar 2020 01:24:08 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 20:55:51 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 31 Mar 2020 20:56:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 31 Mar 2020 20:56:28 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 31 Mar 2020 21:27:00 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:48839397421a64189661c2b86a34eb515d09a28204587a2b06b59df9f6e2d786`  
		Last Modified: Tue, 31 Mar 2020 01:29:28 GMT  
		Size: 22.5 MB (22513374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b5755347d44e006a3743488432c6a77d081bcc3b67cee3609370ca29e83804`  
		Last Modified: Tue, 31 Mar 2020 21:27:55 GMT  
		Size: 244.5 KB (244461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652e7215b25a09c4468906d2f9dd0e353a17465cc5be4ce2a3d2c093ea079f75`  
		Last Modified: Tue, 31 Mar 2020 21:28:08 GMT  
		Size: 55.5 MB (55519226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4f8b06dfd3bb1ae8411acd5538c4c0380f2aad99867fec747bfbbc2f479ccb`  
		Last Modified: Tue, 31 Mar 2020 21:30:48 GMT  
		Size: 140.0 MB (139994485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20` - linux; arm variant v5

```console
$ docker pull mono@sha256:728b3a09731eabb589d971feaf17a5833942c6843ab9cd8358b32ff1b6383cd9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.9 MB (170941920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ee915002d6e2050563346a5fc0731204436dda9794421c36437fc915a77105d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:54:51 GMT
ADD file:ba6c5e03457e69f59231e8e7c6465c1ec985812f0d8f7a65d9842f2be3e947fb in / 
# Thu, 16 Apr 2020 00:54:54 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 03:25:11 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 16 Apr 2020 03:25:36 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 03:26:21 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 03:35:41 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b7d527e4baf13a6c926fb354fe1b38cb42b96f249ae65fdc0f52c853b654e06e`  
		Last Modified: Thu, 16 Apr 2020 01:02:32 GMT  
		Size: 21.2 MB (21190797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8340381d358ecc9e44596343db49a1d8fe9fc408313742adb549d7acbfa010d9`  
		Last Modified: Thu, 16 Apr 2020 03:36:49 GMT  
		Size: 244.5 KB (244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c829c702c9ea78e5f1e834e27d5270a1aeb340e0c387fd2bcca835a6508a18`  
		Last Modified: Thu, 16 Apr 2020 03:36:59 GMT  
		Size: 24.3 MB (24265251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26391aed7c1279d19a1ba1f92bea83bd9306ccb069b953d6af33c408532dccc7`  
		Last Modified: Thu, 16 Apr 2020 03:39:37 GMT  
		Size: 125.2 MB (125241339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20` - linux; arm variant v7

```console
$ docker pull mono@sha256:259a95f5c94430a70d4bfbb3aff1c86b1c46f66e932e58986f5eb0d57da28d35
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.0 MB (166993370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25818813ac0ce16ba21dc50510c7e882df7888a2fde8c2e99ecdcfd9d9bc02f9`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:05:08 GMT
ADD file:e37c4728c0c89ac126542ac35e7e493425c021bfac751079c9b266821a1b4e99 in / 
# Thu, 16 Apr 2020 01:05:10 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:43:14 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 16 Apr 2020 04:43:33 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 04:44:18 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 04:53:30 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f78d9963dfddc4747d6200353b50f6093a6e37ca82e1612fa397d64ff13e7299`  
		Last Modified: Thu, 16 Apr 2020 01:12:33 GMT  
		Size: 19.3 MB (19298546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf684cdea8a2272c82e09cbbb5024552c6e67b7dcf59ea62af547f9c730474e`  
		Last Modified: Thu, 16 Apr 2020 04:54:37 GMT  
		Size: 244.6 KB (244560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249d36139d8bc596df209162b7386211edf003733b4286aa7405033282389c33`  
		Last Modified: Thu, 16 Apr 2020 04:54:47 GMT  
		Size: 23.6 MB (23562096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90019bfc9c5e3ea379d7a72fbc13f136f207f2c152f545a4225d506472e4cec`  
		Last Modified: Thu, 16 Apr 2020 04:57:32 GMT  
		Size: 123.9 MB (123888168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:110949e51fd64f0a4861ad92137d717f431d06f6d24f8e519a5cf346185fde38
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.8 MB (187800067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d6f3e069a025df695d5e7cdae84f0ad9c50ec134a1ef7ed87c306daf10c4955`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 02:45:19 GMT
ADD file:1588320d1c43714ec0353b7471f2ffd649045ca0f5f70dcb1eb064875fff9578 in / 
# Thu, 16 Apr 2020 02:45:21 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:49:41 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 16 Apr 2020 06:50:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:50:40 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 06:58:49 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8978c87ff45d64d1663a585dcf1ed66d9e711c2e4048d83ef561da9514ef46e6`  
		Last Modified: Thu, 16 Apr 2020 02:51:32 GMT  
		Size: 20.4 MB (20370106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554199a06aed010aa14e2e6ed810ac12e3f7ea1f01b4b484029b46c769a914b5`  
		Last Modified: Thu, 16 Apr 2020 07:00:00 GMT  
		Size: 244.4 KB (244384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f9c219c23779432f95dca105f2822e4e5cce0035ec90439890cb4ba1c4b3e0`  
		Last Modified: Thu, 16 Apr 2020 07:00:06 GMT  
		Size: 28.2 MB (28156920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706e37f95124ae6304e93e036c626bc45828f29f97c939ca3dc7b4d8d51e31f6`  
		Last Modified: Thu, 16 Apr 2020 07:02:52 GMT  
		Size: 139.0 MB (139028657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20` - linux; 386

```console
$ docker pull mono@sha256:8ddc25e668dd9f7369fc232cb2b192e58406adb44e30ce9554fa03667fb3ccb2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.8 MB (227783415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e2f7e8e74fa090030747657f6f35d85803a5713cd0745c0b40174549145ce02`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:24 GMT
ADD file:0e72ab6d3f5ce06d7170bd6b0ceeda8687d1a5e2dab40308a8b8960d67fceffe in / 
# Thu, 16 Apr 2020 01:43:24 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:20:38 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 16 Apr 2020 06:20:48 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:21:29 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 06:29:49 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:706a1cdc903b54148ad6d5b672b2bafacadd79daffc0487b4949dd5d193f96f8`  
		Last Modified: Thu, 16 Apr 2020 01:49:33 GMT  
		Size: 23.1 MB (23141457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940906367b61b1c8c02650fa596d87e143b9b9e32639b66e59d0bbd65115133a`  
		Last Modified: Thu, 16 Apr 2020 06:31:23 GMT  
		Size: 244.5 KB (244472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f8edae7689fc4d1bd35e9614dfe86e03e42588bece0cf4d18c3b6c18e651c41`  
		Last Modified: Thu, 16 Apr 2020 06:31:48 GMT  
		Size: 58.6 MB (58557430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e09172c98cd791ef5c541987e57ef03eb73f70dd5c831af61d628cc60a85268c`  
		Last Modified: Thu, 16 Apr 2020 06:35:22 GMT  
		Size: 145.8 MB (145840056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20` - linux; ppc64le

```console
$ docker pull mono@sha256:10f28b145295a978f9628fb30440d346accccf597d45f8b66e8d390fb00f5d12
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.3 MB (173292013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69236ccfa3a77e72c4d43a2c28acf141d1bebac5e126f5c9e4a764fa4b508c23`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:57 GMT
ADD file:1c7f60f778e4b93490d570487d56275925e5eb477632e71cb9f035ce6edf2460 in / 
# Thu, 16 Apr 2020 01:44:03 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:44:48 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 16 Apr 2020 06:46:25 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:47:57 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 07:18:06 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:15e508b90ba1d327da83b72fc494ca263c1566ef6f70b91001cf2093395ffa3d`  
		Last Modified: Thu, 16 Apr 2020 02:04:33 GMT  
		Size: 22.8 MB (22785425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f669c3fbfce943d77701b69e7857eb6d1b88bbf7f9167a449d80be23eb3243`  
		Last Modified: Thu, 16 Apr 2020 07:19:18 GMT  
		Size: 244.6 KB (244638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c16782e8edab25bcd823ec760e3d334f1009343a5a1ef80520730ea6acd56e3`  
		Last Modified: Thu, 16 Apr 2020 07:19:25 GMT  
		Size: 24.6 MB (24639647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8407cfcba2823e2d7d5cf4a042cc54da9defa5fb96119e64542272d1eb1ff98e`  
		Last Modified: Thu, 16 Apr 2020 07:21:36 GMT  
		Size: 125.6 MB (125622303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.20.1`

```console
$ docker pull mono@sha256:c12127bb8f71a7c6e0b13776c9d4221178e12e66dd30eabd5576a2477951754d
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
$ docker pull mono@sha256:18d3fdaf18efe584c791dc668f67459b087287c2f3f44b1aa912d53cff9d0af5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.3 MB (218271546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e067982592a2865379ccfeb3b0082e70e15de3452e86a7683bd19279cb10ef05`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:08 GMT
ADD file:e077f4d014ea0869fc4b3d5a3e6b3c8b792a97a8b4a328f33a994369225ff222 in / 
# Tue, 31 Mar 2020 01:24:08 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 20:55:51 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 31 Mar 2020 20:56:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 31 Mar 2020 20:56:28 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 31 Mar 2020 21:27:00 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:48839397421a64189661c2b86a34eb515d09a28204587a2b06b59df9f6e2d786`  
		Last Modified: Tue, 31 Mar 2020 01:29:28 GMT  
		Size: 22.5 MB (22513374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b5755347d44e006a3743488432c6a77d081bcc3b67cee3609370ca29e83804`  
		Last Modified: Tue, 31 Mar 2020 21:27:55 GMT  
		Size: 244.5 KB (244461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652e7215b25a09c4468906d2f9dd0e353a17465cc5be4ce2a3d2c093ea079f75`  
		Last Modified: Tue, 31 Mar 2020 21:28:08 GMT  
		Size: 55.5 MB (55519226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4f8b06dfd3bb1ae8411acd5538c4c0380f2aad99867fec747bfbbc2f479ccb`  
		Last Modified: Tue, 31 Mar 2020 21:30:48 GMT  
		Size: 140.0 MB (139994485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1` - linux; arm variant v5

```console
$ docker pull mono@sha256:728b3a09731eabb589d971feaf17a5833942c6843ab9cd8358b32ff1b6383cd9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.9 MB (170941920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ee915002d6e2050563346a5fc0731204436dda9794421c36437fc915a77105d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:54:51 GMT
ADD file:ba6c5e03457e69f59231e8e7c6465c1ec985812f0d8f7a65d9842f2be3e947fb in / 
# Thu, 16 Apr 2020 00:54:54 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 03:25:11 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 16 Apr 2020 03:25:36 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 03:26:21 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 03:35:41 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b7d527e4baf13a6c926fb354fe1b38cb42b96f249ae65fdc0f52c853b654e06e`  
		Last Modified: Thu, 16 Apr 2020 01:02:32 GMT  
		Size: 21.2 MB (21190797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8340381d358ecc9e44596343db49a1d8fe9fc408313742adb549d7acbfa010d9`  
		Last Modified: Thu, 16 Apr 2020 03:36:49 GMT  
		Size: 244.5 KB (244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c829c702c9ea78e5f1e834e27d5270a1aeb340e0c387fd2bcca835a6508a18`  
		Last Modified: Thu, 16 Apr 2020 03:36:59 GMT  
		Size: 24.3 MB (24265251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26391aed7c1279d19a1ba1f92bea83bd9306ccb069b953d6af33c408532dccc7`  
		Last Modified: Thu, 16 Apr 2020 03:39:37 GMT  
		Size: 125.2 MB (125241339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1` - linux; arm variant v7

```console
$ docker pull mono@sha256:259a95f5c94430a70d4bfbb3aff1c86b1c46f66e932e58986f5eb0d57da28d35
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.0 MB (166993370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25818813ac0ce16ba21dc50510c7e882df7888a2fde8c2e99ecdcfd9d9bc02f9`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:05:08 GMT
ADD file:e37c4728c0c89ac126542ac35e7e493425c021bfac751079c9b266821a1b4e99 in / 
# Thu, 16 Apr 2020 01:05:10 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:43:14 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 16 Apr 2020 04:43:33 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 04:44:18 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 04:53:30 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f78d9963dfddc4747d6200353b50f6093a6e37ca82e1612fa397d64ff13e7299`  
		Last Modified: Thu, 16 Apr 2020 01:12:33 GMT  
		Size: 19.3 MB (19298546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf684cdea8a2272c82e09cbbb5024552c6e67b7dcf59ea62af547f9c730474e`  
		Last Modified: Thu, 16 Apr 2020 04:54:37 GMT  
		Size: 244.6 KB (244560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249d36139d8bc596df209162b7386211edf003733b4286aa7405033282389c33`  
		Last Modified: Thu, 16 Apr 2020 04:54:47 GMT  
		Size: 23.6 MB (23562096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90019bfc9c5e3ea379d7a72fbc13f136f207f2c152f545a4225d506472e4cec`  
		Last Modified: Thu, 16 Apr 2020 04:57:32 GMT  
		Size: 123.9 MB (123888168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:110949e51fd64f0a4861ad92137d717f431d06f6d24f8e519a5cf346185fde38
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.8 MB (187800067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d6f3e069a025df695d5e7cdae84f0ad9c50ec134a1ef7ed87c306daf10c4955`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 02:45:19 GMT
ADD file:1588320d1c43714ec0353b7471f2ffd649045ca0f5f70dcb1eb064875fff9578 in / 
# Thu, 16 Apr 2020 02:45:21 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:49:41 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 16 Apr 2020 06:50:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:50:40 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 06:58:49 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8978c87ff45d64d1663a585dcf1ed66d9e711c2e4048d83ef561da9514ef46e6`  
		Last Modified: Thu, 16 Apr 2020 02:51:32 GMT  
		Size: 20.4 MB (20370106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554199a06aed010aa14e2e6ed810ac12e3f7ea1f01b4b484029b46c769a914b5`  
		Last Modified: Thu, 16 Apr 2020 07:00:00 GMT  
		Size: 244.4 KB (244384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f9c219c23779432f95dca105f2822e4e5cce0035ec90439890cb4ba1c4b3e0`  
		Last Modified: Thu, 16 Apr 2020 07:00:06 GMT  
		Size: 28.2 MB (28156920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706e37f95124ae6304e93e036c626bc45828f29f97c939ca3dc7b4d8d51e31f6`  
		Last Modified: Thu, 16 Apr 2020 07:02:52 GMT  
		Size: 139.0 MB (139028657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1` - linux; 386

```console
$ docker pull mono@sha256:8ddc25e668dd9f7369fc232cb2b192e58406adb44e30ce9554fa03667fb3ccb2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.8 MB (227783415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e2f7e8e74fa090030747657f6f35d85803a5713cd0745c0b40174549145ce02`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:24 GMT
ADD file:0e72ab6d3f5ce06d7170bd6b0ceeda8687d1a5e2dab40308a8b8960d67fceffe in / 
# Thu, 16 Apr 2020 01:43:24 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:20:38 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 16 Apr 2020 06:20:48 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:21:29 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 06:29:49 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:706a1cdc903b54148ad6d5b672b2bafacadd79daffc0487b4949dd5d193f96f8`  
		Last Modified: Thu, 16 Apr 2020 01:49:33 GMT  
		Size: 23.1 MB (23141457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940906367b61b1c8c02650fa596d87e143b9b9e32639b66e59d0bbd65115133a`  
		Last Modified: Thu, 16 Apr 2020 06:31:23 GMT  
		Size: 244.5 KB (244472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f8edae7689fc4d1bd35e9614dfe86e03e42588bece0cf4d18c3b6c18e651c41`  
		Last Modified: Thu, 16 Apr 2020 06:31:48 GMT  
		Size: 58.6 MB (58557430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e09172c98cd791ef5c541987e57ef03eb73f70dd5c831af61d628cc60a85268c`  
		Last Modified: Thu, 16 Apr 2020 06:35:22 GMT  
		Size: 145.8 MB (145840056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1` - linux; ppc64le

```console
$ docker pull mono@sha256:10f28b145295a978f9628fb30440d346accccf597d45f8b66e8d390fb00f5d12
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.3 MB (173292013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69236ccfa3a77e72c4d43a2c28acf141d1bebac5e126f5c9e4a764fa4b508c23`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:57 GMT
ADD file:1c7f60f778e4b93490d570487d56275925e5eb477632e71cb9f035ce6edf2460 in / 
# Thu, 16 Apr 2020 01:44:03 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:44:48 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 16 Apr 2020 06:46:25 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:47:57 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 07:18:06 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:15e508b90ba1d327da83b72fc494ca263c1566ef6f70b91001cf2093395ffa3d`  
		Last Modified: Thu, 16 Apr 2020 02:04:33 GMT  
		Size: 22.8 MB (22785425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f669c3fbfce943d77701b69e7857eb6d1b88bbf7f9167a449d80be23eb3243`  
		Last Modified: Thu, 16 Apr 2020 07:19:18 GMT  
		Size: 244.6 KB (244638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c16782e8edab25bcd823ec760e3d334f1009343a5a1ef80520730ea6acd56e3`  
		Last Modified: Thu, 16 Apr 2020 07:19:25 GMT  
		Size: 24.6 MB (24639647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8407cfcba2823e2d7d5cf4a042cc54da9defa5fb96119e64542272d1eb1ff98e`  
		Last Modified: Thu, 16 Apr 2020 07:21:36 GMT  
		Size: 125.6 MB (125622303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.20.1.34`

```console
$ docker pull mono@sha256:c12127bb8f71a7c6e0b13776c9d4221178e12e66dd30eabd5576a2477951754d
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
$ docker pull mono@sha256:18d3fdaf18efe584c791dc668f67459b087287c2f3f44b1aa912d53cff9d0af5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.3 MB (218271546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e067982592a2865379ccfeb3b0082e70e15de3452e86a7683bd19279cb10ef05`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:08 GMT
ADD file:e077f4d014ea0869fc4b3d5a3e6b3c8b792a97a8b4a328f33a994369225ff222 in / 
# Tue, 31 Mar 2020 01:24:08 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 20:55:51 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 31 Mar 2020 20:56:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 31 Mar 2020 20:56:28 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 31 Mar 2020 21:27:00 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:48839397421a64189661c2b86a34eb515d09a28204587a2b06b59df9f6e2d786`  
		Last Modified: Tue, 31 Mar 2020 01:29:28 GMT  
		Size: 22.5 MB (22513374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b5755347d44e006a3743488432c6a77d081bcc3b67cee3609370ca29e83804`  
		Last Modified: Tue, 31 Mar 2020 21:27:55 GMT  
		Size: 244.5 KB (244461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652e7215b25a09c4468906d2f9dd0e353a17465cc5be4ce2a3d2c093ea079f75`  
		Last Modified: Tue, 31 Mar 2020 21:28:08 GMT  
		Size: 55.5 MB (55519226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4f8b06dfd3bb1ae8411acd5538c4c0380f2aad99867fec747bfbbc2f479ccb`  
		Last Modified: Tue, 31 Mar 2020 21:30:48 GMT  
		Size: 140.0 MB (139994485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1.34` - linux; arm variant v5

```console
$ docker pull mono@sha256:728b3a09731eabb589d971feaf17a5833942c6843ab9cd8358b32ff1b6383cd9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.9 MB (170941920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ee915002d6e2050563346a5fc0731204436dda9794421c36437fc915a77105d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:54:51 GMT
ADD file:ba6c5e03457e69f59231e8e7c6465c1ec985812f0d8f7a65d9842f2be3e947fb in / 
# Thu, 16 Apr 2020 00:54:54 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 03:25:11 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 16 Apr 2020 03:25:36 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 03:26:21 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 03:35:41 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b7d527e4baf13a6c926fb354fe1b38cb42b96f249ae65fdc0f52c853b654e06e`  
		Last Modified: Thu, 16 Apr 2020 01:02:32 GMT  
		Size: 21.2 MB (21190797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8340381d358ecc9e44596343db49a1d8fe9fc408313742adb549d7acbfa010d9`  
		Last Modified: Thu, 16 Apr 2020 03:36:49 GMT  
		Size: 244.5 KB (244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c829c702c9ea78e5f1e834e27d5270a1aeb340e0c387fd2bcca835a6508a18`  
		Last Modified: Thu, 16 Apr 2020 03:36:59 GMT  
		Size: 24.3 MB (24265251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26391aed7c1279d19a1ba1f92bea83bd9306ccb069b953d6af33c408532dccc7`  
		Last Modified: Thu, 16 Apr 2020 03:39:37 GMT  
		Size: 125.2 MB (125241339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1.34` - linux; arm variant v7

```console
$ docker pull mono@sha256:259a95f5c94430a70d4bfbb3aff1c86b1c46f66e932e58986f5eb0d57da28d35
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.0 MB (166993370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25818813ac0ce16ba21dc50510c7e882df7888a2fde8c2e99ecdcfd9d9bc02f9`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:05:08 GMT
ADD file:e37c4728c0c89ac126542ac35e7e493425c021bfac751079c9b266821a1b4e99 in / 
# Thu, 16 Apr 2020 01:05:10 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:43:14 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 16 Apr 2020 04:43:33 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 04:44:18 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 04:53:30 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f78d9963dfddc4747d6200353b50f6093a6e37ca82e1612fa397d64ff13e7299`  
		Last Modified: Thu, 16 Apr 2020 01:12:33 GMT  
		Size: 19.3 MB (19298546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf684cdea8a2272c82e09cbbb5024552c6e67b7dcf59ea62af547f9c730474e`  
		Last Modified: Thu, 16 Apr 2020 04:54:37 GMT  
		Size: 244.6 KB (244560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249d36139d8bc596df209162b7386211edf003733b4286aa7405033282389c33`  
		Last Modified: Thu, 16 Apr 2020 04:54:47 GMT  
		Size: 23.6 MB (23562096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90019bfc9c5e3ea379d7a72fbc13f136f207f2c152f545a4225d506472e4cec`  
		Last Modified: Thu, 16 Apr 2020 04:57:32 GMT  
		Size: 123.9 MB (123888168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1.34` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:110949e51fd64f0a4861ad92137d717f431d06f6d24f8e519a5cf346185fde38
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.8 MB (187800067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d6f3e069a025df695d5e7cdae84f0ad9c50ec134a1ef7ed87c306daf10c4955`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 02:45:19 GMT
ADD file:1588320d1c43714ec0353b7471f2ffd649045ca0f5f70dcb1eb064875fff9578 in / 
# Thu, 16 Apr 2020 02:45:21 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:49:41 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 16 Apr 2020 06:50:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:50:40 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 06:58:49 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8978c87ff45d64d1663a585dcf1ed66d9e711c2e4048d83ef561da9514ef46e6`  
		Last Modified: Thu, 16 Apr 2020 02:51:32 GMT  
		Size: 20.4 MB (20370106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554199a06aed010aa14e2e6ed810ac12e3f7ea1f01b4b484029b46c769a914b5`  
		Last Modified: Thu, 16 Apr 2020 07:00:00 GMT  
		Size: 244.4 KB (244384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f9c219c23779432f95dca105f2822e4e5cce0035ec90439890cb4ba1c4b3e0`  
		Last Modified: Thu, 16 Apr 2020 07:00:06 GMT  
		Size: 28.2 MB (28156920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706e37f95124ae6304e93e036c626bc45828f29f97c939ca3dc7b4d8d51e31f6`  
		Last Modified: Thu, 16 Apr 2020 07:02:52 GMT  
		Size: 139.0 MB (139028657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1.34` - linux; 386

```console
$ docker pull mono@sha256:8ddc25e668dd9f7369fc232cb2b192e58406adb44e30ce9554fa03667fb3ccb2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.8 MB (227783415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e2f7e8e74fa090030747657f6f35d85803a5713cd0745c0b40174549145ce02`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:24 GMT
ADD file:0e72ab6d3f5ce06d7170bd6b0ceeda8687d1a5e2dab40308a8b8960d67fceffe in / 
# Thu, 16 Apr 2020 01:43:24 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:20:38 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 16 Apr 2020 06:20:48 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:21:29 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 06:29:49 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:706a1cdc903b54148ad6d5b672b2bafacadd79daffc0487b4949dd5d193f96f8`  
		Last Modified: Thu, 16 Apr 2020 01:49:33 GMT  
		Size: 23.1 MB (23141457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940906367b61b1c8c02650fa596d87e143b9b9e32639b66e59d0bbd65115133a`  
		Last Modified: Thu, 16 Apr 2020 06:31:23 GMT  
		Size: 244.5 KB (244472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f8edae7689fc4d1bd35e9614dfe86e03e42588bece0cf4d18c3b6c18e651c41`  
		Last Modified: Thu, 16 Apr 2020 06:31:48 GMT  
		Size: 58.6 MB (58557430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e09172c98cd791ef5c541987e57ef03eb73f70dd5c831af61d628cc60a85268c`  
		Last Modified: Thu, 16 Apr 2020 06:35:22 GMT  
		Size: 145.8 MB (145840056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1.34` - linux; ppc64le

```console
$ docker pull mono@sha256:10f28b145295a978f9628fb30440d346accccf597d45f8b66e8d390fb00f5d12
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.3 MB (173292013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69236ccfa3a77e72c4d43a2c28acf141d1bebac5e126f5c9e4a764fa4b508c23`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:57 GMT
ADD file:1c7f60f778e4b93490d570487d56275925e5eb477632e71cb9f035ce6edf2460 in / 
# Thu, 16 Apr 2020 01:44:03 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:44:48 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 16 Apr 2020 06:46:25 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:47:57 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 07:18:06 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:15e508b90ba1d327da83b72fc494ca263c1566ef6f70b91001cf2093395ffa3d`  
		Last Modified: Thu, 16 Apr 2020 02:04:33 GMT  
		Size: 22.8 MB (22785425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f669c3fbfce943d77701b69e7857eb6d1b88bbf7f9167a449d80be23eb3243`  
		Last Modified: Thu, 16 Apr 2020 07:19:18 GMT  
		Size: 244.6 KB (244638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c16782e8edab25bcd823ec760e3d334f1009343a5a1ef80520730ea6acd56e3`  
		Last Modified: Thu, 16 Apr 2020 07:19:25 GMT  
		Size: 24.6 MB (24639647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8407cfcba2823e2d7d5cf4a042cc54da9defa5fb96119e64542272d1eb1ff98e`  
		Last Modified: Thu, 16 Apr 2020 07:21:36 GMT  
		Size: 125.6 MB (125622303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.20.1.34-slim`

```console
$ docker pull mono@sha256:bdb33a29bcd7335c6f30827a2ca6aa41003005bfbfd095050e7c8d38ace10fd2
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
$ docker pull mono@sha256:f76de3e15ebf2e6b8857bc3ba426abb656fd3237dece954f0e1cc2f8415de2b5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78277061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf91b469701e2d4be79fff2b3ee2f9d2ac9ecf1c8088873c5a76091656ac8965`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:08 GMT
ADD file:e077f4d014ea0869fc4b3d5a3e6b3c8b792a97a8b4a328f33a994369225ff222 in / 
# Tue, 31 Mar 2020 01:24:08 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 20:55:51 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 31 Mar 2020 20:56:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 31 Mar 2020 20:56:28 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:48839397421a64189661c2b86a34eb515d09a28204587a2b06b59df9f6e2d786`  
		Last Modified: Tue, 31 Mar 2020 01:29:28 GMT  
		Size: 22.5 MB (22513374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b5755347d44e006a3743488432c6a77d081bcc3b67cee3609370ca29e83804`  
		Last Modified: Tue, 31 Mar 2020 21:27:55 GMT  
		Size: 244.5 KB (244461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652e7215b25a09c4468906d2f9dd0e353a17465cc5be4ce2a3d2c093ea079f75`  
		Last Modified: Tue, 31 Mar 2020 21:28:08 GMT  
		Size: 55.5 MB (55519226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1.34-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:24277a451c25923284bd552e52a477c6d5f0550d5bc4bf36c6f011cdab833f5a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.7 MB (45700581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ded18f1bc26bdd165c560e353704c774e72c61edf6306f0a301734b1cd592d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:54:51 GMT
ADD file:ba6c5e03457e69f59231e8e7c6465c1ec985812f0d8f7a65d9842f2be3e947fb in / 
# Thu, 16 Apr 2020 00:54:54 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 03:25:11 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 16 Apr 2020 03:25:36 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 03:26:21 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b7d527e4baf13a6c926fb354fe1b38cb42b96f249ae65fdc0f52c853b654e06e`  
		Last Modified: Thu, 16 Apr 2020 01:02:32 GMT  
		Size: 21.2 MB (21190797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8340381d358ecc9e44596343db49a1d8fe9fc408313742adb549d7acbfa010d9`  
		Last Modified: Thu, 16 Apr 2020 03:36:49 GMT  
		Size: 244.5 KB (244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c829c702c9ea78e5f1e834e27d5270a1aeb340e0c387fd2bcca835a6508a18`  
		Last Modified: Thu, 16 Apr 2020 03:36:59 GMT  
		Size: 24.3 MB (24265251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1.34-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:82879b2317895d2b306e14bd38f26be346070655d8441662bd05aa9f85797783
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43105202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab6576fb1edf563a52cf0994636f3e1619b6508c783b4906ed59494f06d03533`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:05:08 GMT
ADD file:e37c4728c0c89ac126542ac35e7e493425c021bfac751079c9b266821a1b4e99 in / 
# Thu, 16 Apr 2020 01:05:10 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:43:14 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 16 Apr 2020 04:43:33 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 04:44:18 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f78d9963dfddc4747d6200353b50f6093a6e37ca82e1612fa397d64ff13e7299`  
		Last Modified: Thu, 16 Apr 2020 01:12:33 GMT  
		Size: 19.3 MB (19298546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf684cdea8a2272c82e09cbbb5024552c6e67b7dcf59ea62af547f9c730474e`  
		Last Modified: Thu, 16 Apr 2020 04:54:37 GMT  
		Size: 244.6 KB (244560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249d36139d8bc596df209162b7386211edf003733b4286aa7405033282389c33`  
		Last Modified: Thu, 16 Apr 2020 04:54:47 GMT  
		Size: 23.6 MB (23562096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1.34-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:373e3d9ccf313cac211d9ede8eec8a2ccb1d1c0303fc5312fddfccc026277c41
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48771410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43f116c952bab72566e217b3d9571b9572c6e2ac731995c266825ca5ff059e14`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 02:45:19 GMT
ADD file:1588320d1c43714ec0353b7471f2ffd649045ca0f5f70dcb1eb064875fff9578 in / 
# Thu, 16 Apr 2020 02:45:21 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:49:41 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 16 Apr 2020 06:50:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:50:40 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8978c87ff45d64d1663a585dcf1ed66d9e711c2e4048d83ef561da9514ef46e6`  
		Last Modified: Thu, 16 Apr 2020 02:51:32 GMT  
		Size: 20.4 MB (20370106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554199a06aed010aa14e2e6ed810ac12e3f7ea1f01b4b484029b46c769a914b5`  
		Last Modified: Thu, 16 Apr 2020 07:00:00 GMT  
		Size: 244.4 KB (244384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f9c219c23779432f95dca105f2822e4e5cce0035ec90439890cb4ba1c4b3e0`  
		Last Modified: Thu, 16 Apr 2020 07:00:06 GMT  
		Size: 28.2 MB (28156920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1.34-slim` - linux; 386

```console
$ docker pull mono@sha256:22ba0007f042aa7ea555aef6e713a085984cf41290c3631975530fbc0e9b3648
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81943359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc471f7432a6acd1af4c999f8e978b7262817bd9a4d73655712d304817917e00`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:24 GMT
ADD file:0e72ab6d3f5ce06d7170bd6b0ceeda8687d1a5e2dab40308a8b8960d67fceffe in / 
# Thu, 16 Apr 2020 01:43:24 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:20:38 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 16 Apr 2020 06:20:48 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:21:29 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:706a1cdc903b54148ad6d5b672b2bafacadd79daffc0487b4949dd5d193f96f8`  
		Last Modified: Thu, 16 Apr 2020 01:49:33 GMT  
		Size: 23.1 MB (23141457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940906367b61b1c8c02650fa596d87e143b9b9e32639b66e59d0bbd65115133a`  
		Last Modified: Thu, 16 Apr 2020 06:31:23 GMT  
		Size: 244.5 KB (244472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f8edae7689fc4d1bd35e9614dfe86e03e42588bece0cf4d18c3b6c18e651c41`  
		Last Modified: Thu, 16 Apr 2020 06:31:48 GMT  
		Size: 58.6 MB (58557430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1.34-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:8075f272b67d3b0230b83dec1f4ea321e0f9e68390fb4208b5cbfbde3e339a6c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.7 MB (47669710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b4f4a283b7df8fb74adb07675407330610860bf778c831f068775f705090dfd`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:57 GMT
ADD file:1c7f60f778e4b93490d570487d56275925e5eb477632e71cb9f035ce6edf2460 in / 
# Thu, 16 Apr 2020 01:44:03 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:44:48 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 16 Apr 2020 06:46:25 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:47:57 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:15e508b90ba1d327da83b72fc494ca263c1566ef6f70b91001cf2093395ffa3d`  
		Last Modified: Thu, 16 Apr 2020 02:04:33 GMT  
		Size: 22.8 MB (22785425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f669c3fbfce943d77701b69e7857eb6d1b88bbf7f9167a449d80be23eb3243`  
		Last Modified: Thu, 16 Apr 2020 07:19:18 GMT  
		Size: 244.6 KB (244638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c16782e8edab25bcd823ec760e3d334f1009343a5a1ef80520730ea6acd56e3`  
		Last Modified: Thu, 16 Apr 2020 07:19:25 GMT  
		Size: 24.6 MB (24639647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.20.1-slim`

```console
$ docker pull mono@sha256:bdb33a29bcd7335c6f30827a2ca6aa41003005bfbfd095050e7c8d38ace10fd2
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
$ docker pull mono@sha256:f76de3e15ebf2e6b8857bc3ba426abb656fd3237dece954f0e1cc2f8415de2b5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78277061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf91b469701e2d4be79fff2b3ee2f9d2ac9ecf1c8088873c5a76091656ac8965`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:08 GMT
ADD file:e077f4d014ea0869fc4b3d5a3e6b3c8b792a97a8b4a328f33a994369225ff222 in / 
# Tue, 31 Mar 2020 01:24:08 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 20:55:51 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 31 Mar 2020 20:56:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 31 Mar 2020 20:56:28 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:48839397421a64189661c2b86a34eb515d09a28204587a2b06b59df9f6e2d786`  
		Last Modified: Tue, 31 Mar 2020 01:29:28 GMT  
		Size: 22.5 MB (22513374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b5755347d44e006a3743488432c6a77d081bcc3b67cee3609370ca29e83804`  
		Last Modified: Tue, 31 Mar 2020 21:27:55 GMT  
		Size: 244.5 KB (244461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652e7215b25a09c4468906d2f9dd0e353a17465cc5be4ce2a3d2c093ea079f75`  
		Last Modified: Tue, 31 Mar 2020 21:28:08 GMT  
		Size: 55.5 MB (55519226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:24277a451c25923284bd552e52a477c6d5f0550d5bc4bf36c6f011cdab833f5a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.7 MB (45700581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ded18f1bc26bdd165c560e353704c774e72c61edf6306f0a301734b1cd592d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:54:51 GMT
ADD file:ba6c5e03457e69f59231e8e7c6465c1ec985812f0d8f7a65d9842f2be3e947fb in / 
# Thu, 16 Apr 2020 00:54:54 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 03:25:11 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 16 Apr 2020 03:25:36 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 03:26:21 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b7d527e4baf13a6c926fb354fe1b38cb42b96f249ae65fdc0f52c853b654e06e`  
		Last Modified: Thu, 16 Apr 2020 01:02:32 GMT  
		Size: 21.2 MB (21190797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8340381d358ecc9e44596343db49a1d8fe9fc408313742adb549d7acbfa010d9`  
		Last Modified: Thu, 16 Apr 2020 03:36:49 GMT  
		Size: 244.5 KB (244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c829c702c9ea78e5f1e834e27d5270a1aeb340e0c387fd2bcca835a6508a18`  
		Last Modified: Thu, 16 Apr 2020 03:36:59 GMT  
		Size: 24.3 MB (24265251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:82879b2317895d2b306e14bd38f26be346070655d8441662bd05aa9f85797783
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43105202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab6576fb1edf563a52cf0994636f3e1619b6508c783b4906ed59494f06d03533`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:05:08 GMT
ADD file:e37c4728c0c89ac126542ac35e7e493425c021bfac751079c9b266821a1b4e99 in / 
# Thu, 16 Apr 2020 01:05:10 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:43:14 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 16 Apr 2020 04:43:33 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 04:44:18 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f78d9963dfddc4747d6200353b50f6093a6e37ca82e1612fa397d64ff13e7299`  
		Last Modified: Thu, 16 Apr 2020 01:12:33 GMT  
		Size: 19.3 MB (19298546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf684cdea8a2272c82e09cbbb5024552c6e67b7dcf59ea62af547f9c730474e`  
		Last Modified: Thu, 16 Apr 2020 04:54:37 GMT  
		Size: 244.6 KB (244560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249d36139d8bc596df209162b7386211edf003733b4286aa7405033282389c33`  
		Last Modified: Thu, 16 Apr 2020 04:54:47 GMT  
		Size: 23.6 MB (23562096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:373e3d9ccf313cac211d9ede8eec8a2ccb1d1c0303fc5312fddfccc026277c41
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48771410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43f116c952bab72566e217b3d9571b9572c6e2ac731995c266825ca5ff059e14`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 02:45:19 GMT
ADD file:1588320d1c43714ec0353b7471f2ffd649045ca0f5f70dcb1eb064875fff9578 in / 
# Thu, 16 Apr 2020 02:45:21 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:49:41 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 16 Apr 2020 06:50:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:50:40 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8978c87ff45d64d1663a585dcf1ed66d9e711c2e4048d83ef561da9514ef46e6`  
		Last Modified: Thu, 16 Apr 2020 02:51:32 GMT  
		Size: 20.4 MB (20370106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554199a06aed010aa14e2e6ed810ac12e3f7ea1f01b4b484029b46c769a914b5`  
		Last Modified: Thu, 16 Apr 2020 07:00:00 GMT  
		Size: 244.4 KB (244384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f9c219c23779432f95dca105f2822e4e5cce0035ec90439890cb4ba1c4b3e0`  
		Last Modified: Thu, 16 Apr 2020 07:00:06 GMT  
		Size: 28.2 MB (28156920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1-slim` - linux; 386

```console
$ docker pull mono@sha256:22ba0007f042aa7ea555aef6e713a085984cf41290c3631975530fbc0e9b3648
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81943359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc471f7432a6acd1af4c999f8e978b7262817bd9a4d73655712d304817917e00`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:24 GMT
ADD file:0e72ab6d3f5ce06d7170bd6b0ceeda8687d1a5e2dab40308a8b8960d67fceffe in / 
# Thu, 16 Apr 2020 01:43:24 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:20:38 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 16 Apr 2020 06:20:48 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:21:29 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:706a1cdc903b54148ad6d5b672b2bafacadd79daffc0487b4949dd5d193f96f8`  
		Last Modified: Thu, 16 Apr 2020 01:49:33 GMT  
		Size: 23.1 MB (23141457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940906367b61b1c8c02650fa596d87e143b9b9e32639b66e59d0bbd65115133a`  
		Last Modified: Thu, 16 Apr 2020 06:31:23 GMT  
		Size: 244.5 KB (244472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f8edae7689fc4d1bd35e9614dfe86e03e42588bece0cf4d18c3b6c18e651c41`  
		Last Modified: Thu, 16 Apr 2020 06:31:48 GMT  
		Size: 58.6 MB (58557430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:8075f272b67d3b0230b83dec1f4ea321e0f9e68390fb4208b5cbfbde3e339a6c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.7 MB (47669710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b4f4a283b7df8fb74adb07675407330610860bf778c831f068775f705090dfd`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:57 GMT
ADD file:1c7f60f778e4b93490d570487d56275925e5eb477632e71cb9f035ce6edf2460 in / 
# Thu, 16 Apr 2020 01:44:03 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:44:48 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 16 Apr 2020 06:46:25 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:47:57 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:15e508b90ba1d327da83b72fc494ca263c1566ef6f70b91001cf2093395ffa3d`  
		Last Modified: Thu, 16 Apr 2020 02:04:33 GMT  
		Size: 22.8 MB (22785425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f669c3fbfce943d77701b69e7857eb6d1b88bbf7f9167a449d80be23eb3243`  
		Last Modified: Thu, 16 Apr 2020 07:19:18 GMT  
		Size: 244.6 KB (244638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c16782e8edab25bcd823ec760e3d334f1009343a5a1ef80520730ea6acd56e3`  
		Last Modified: Thu, 16 Apr 2020 07:19:25 GMT  
		Size: 24.6 MB (24639647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.20-slim`

```console
$ docker pull mono@sha256:bdb33a29bcd7335c6f30827a2ca6aa41003005bfbfd095050e7c8d38ace10fd2
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
$ docker pull mono@sha256:f76de3e15ebf2e6b8857bc3ba426abb656fd3237dece954f0e1cc2f8415de2b5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78277061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf91b469701e2d4be79fff2b3ee2f9d2ac9ecf1c8088873c5a76091656ac8965`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:08 GMT
ADD file:e077f4d014ea0869fc4b3d5a3e6b3c8b792a97a8b4a328f33a994369225ff222 in / 
# Tue, 31 Mar 2020 01:24:08 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 20:55:51 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 31 Mar 2020 20:56:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 31 Mar 2020 20:56:28 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:48839397421a64189661c2b86a34eb515d09a28204587a2b06b59df9f6e2d786`  
		Last Modified: Tue, 31 Mar 2020 01:29:28 GMT  
		Size: 22.5 MB (22513374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b5755347d44e006a3743488432c6a77d081bcc3b67cee3609370ca29e83804`  
		Last Modified: Tue, 31 Mar 2020 21:27:55 GMT  
		Size: 244.5 KB (244461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652e7215b25a09c4468906d2f9dd0e353a17465cc5be4ce2a3d2c093ea079f75`  
		Last Modified: Tue, 31 Mar 2020 21:28:08 GMT  
		Size: 55.5 MB (55519226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:24277a451c25923284bd552e52a477c6d5f0550d5bc4bf36c6f011cdab833f5a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.7 MB (45700581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ded18f1bc26bdd165c560e353704c774e72c61edf6306f0a301734b1cd592d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:54:51 GMT
ADD file:ba6c5e03457e69f59231e8e7c6465c1ec985812f0d8f7a65d9842f2be3e947fb in / 
# Thu, 16 Apr 2020 00:54:54 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 03:25:11 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 16 Apr 2020 03:25:36 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 03:26:21 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b7d527e4baf13a6c926fb354fe1b38cb42b96f249ae65fdc0f52c853b654e06e`  
		Last Modified: Thu, 16 Apr 2020 01:02:32 GMT  
		Size: 21.2 MB (21190797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8340381d358ecc9e44596343db49a1d8fe9fc408313742adb549d7acbfa010d9`  
		Last Modified: Thu, 16 Apr 2020 03:36:49 GMT  
		Size: 244.5 KB (244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c829c702c9ea78e5f1e834e27d5270a1aeb340e0c387fd2bcca835a6508a18`  
		Last Modified: Thu, 16 Apr 2020 03:36:59 GMT  
		Size: 24.3 MB (24265251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:82879b2317895d2b306e14bd38f26be346070655d8441662bd05aa9f85797783
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43105202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab6576fb1edf563a52cf0994636f3e1619b6508c783b4906ed59494f06d03533`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:05:08 GMT
ADD file:e37c4728c0c89ac126542ac35e7e493425c021bfac751079c9b266821a1b4e99 in / 
# Thu, 16 Apr 2020 01:05:10 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:43:14 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 16 Apr 2020 04:43:33 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 04:44:18 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f78d9963dfddc4747d6200353b50f6093a6e37ca82e1612fa397d64ff13e7299`  
		Last Modified: Thu, 16 Apr 2020 01:12:33 GMT  
		Size: 19.3 MB (19298546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf684cdea8a2272c82e09cbbb5024552c6e67b7dcf59ea62af547f9c730474e`  
		Last Modified: Thu, 16 Apr 2020 04:54:37 GMT  
		Size: 244.6 KB (244560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249d36139d8bc596df209162b7386211edf003733b4286aa7405033282389c33`  
		Last Modified: Thu, 16 Apr 2020 04:54:47 GMT  
		Size: 23.6 MB (23562096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:373e3d9ccf313cac211d9ede8eec8a2ccb1d1c0303fc5312fddfccc026277c41
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48771410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43f116c952bab72566e217b3d9571b9572c6e2ac731995c266825ca5ff059e14`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 02:45:19 GMT
ADD file:1588320d1c43714ec0353b7471f2ffd649045ca0f5f70dcb1eb064875fff9578 in / 
# Thu, 16 Apr 2020 02:45:21 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:49:41 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 16 Apr 2020 06:50:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:50:40 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8978c87ff45d64d1663a585dcf1ed66d9e711c2e4048d83ef561da9514ef46e6`  
		Last Modified: Thu, 16 Apr 2020 02:51:32 GMT  
		Size: 20.4 MB (20370106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554199a06aed010aa14e2e6ed810ac12e3f7ea1f01b4b484029b46c769a914b5`  
		Last Modified: Thu, 16 Apr 2020 07:00:00 GMT  
		Size: 244.4 KB (244384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f9c219c23779432f95dca105f2822e4e5cce0035ec90439890cb4ba1c4b3e0`  
		Last Modified: Thu, 16 Apr 2020 07:00:06 GMT  
		Size: 28.2 MB (28156920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20-slim` - linux; 386

```console
$ docker pull mono@sha256:22ba0007f042aa7ea555aef6e713a085984cf41290c3631975530fbc0e9b3648
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81943359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc471f7432a6acd1af4c999f8e978b7262817bd9a4d73655712d304817917e00`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:24 GMT
ADD file:0e72ab6d3f5ce06d7170bd6b0ceeda8687d1a5e2dab40308a8b8960d67fceffe in / 
# Thu, 16 Apr 2020 01:43:24 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:20:38 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 16 Apr 2020 06:20:48 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:21:29 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:706a1cdc903b54148ad6d5b672b2bafacadd79daffc0487b4949dd5d193f96f8`  
		Last Modified: Thu, 16 Apr 2020 01:49:33 GMT  
		Size: 23.1 MB (23141457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940906367b61b1c8c02650fa596d87e143b9b9e32639b66e59d0bbd65115133a`  
		Last Modified: Thu, 16 Apr 2020 06:31:23 GMT  
		Size: 244.5 KB (244472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f8edae7689fc4d1bd35e9614dfe86e03e42588bece0cf4d18c3b6c18e651c41`  
		Last Modified: Thu, 16 Apr 2020 06:31:48 GMT  
		Size: 58.6 MB (58557430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:8075f272b67d3b0230b83dec1f4ea321e0f9e68390fb4208b5cbfbde3e339a6c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.7 MB (47669710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b4f4a283b7df8fb74adb07675407330610860bf778c831f068775f705090dfd`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:57 GMT
ADD file:1c7f60f778e4b93490d570487d56275925e5eb477632e71cb9f035ce6edf2460 in / 
# Thu, 16 Apr 2020 01:44:03 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:44:48 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 16 Apr 2020 06:46:25 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:47:57 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:15e508b90ba1d327da83b72fc494ca263c1566ef6f70b91001cf2093395ffa3d`  
		Last Modified: Thu, 16 Apr 2020 02:04:33 GMT  
		Size: 22.8 MB (22785425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f669c3fbfce943d77701b69e7857eb6d1b88bbf7f9167a449d80be23eb3243`  
		Last Modified: Thu, 16 Apr 2020 07:19:18 GMT  
		Size: 244.6 KB (244638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c16782e8edab25bcd823ec760e3d334f1009343a5a1ef80520730ea6acd56e3`  
		Last Modified: Thu, 16 Apr 2020 07:19:25 GMT  
		Size: 24.6 MB (24639647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5-slim`

```console
$ docker pull mono@sha256:bdb33a29bcd7335c6f30827a2ca6aa41003005bfbfd095050e7c8d38ace10fd2
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
$ docker pull mono@sha256:f76de3e15ebf2e6b8857bc3ba426abb656fd3237dece954f0e1cc2f8415de2b5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78277061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf91b469701e2d4be79fff2b3ee2f9d2ac9ecf1c8088873c5a76091656ac8965`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:08 GMT
ADD file:e077f4d014ea0869fc4b3d5a3e6b3c8b792a97a8b4a328f33a994369225ff222 in / 
# Tue, 31 Mar 2020 01:24:08 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 20:55:51 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 31 Mar 2020 20:56:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 31 Mar 2020 20:56:28 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:48839397421a64189661c2b86a34eb515d09a28204587a2b06b59df9f6e2d786`  
		Last Modified: Tue, 31 Mar 2020 01:29:28 GMT  
		Size: 22.5 MB (22513374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b5755347d44e006a3743488432c6a77d081bcc3b67cee3609370ca29e83804`  
		Last Modified: Tue, 31 Mar 2020 21:27:55 GMT  
		Size: 244.5 KB (244461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652e7215b25a09c4468906d2f9dd0e353a17465cc5be4ce2a3d2c093ea079f75`  
		Last Modified: Tue, 31 Mar 2020 21:28:08 GMT  
		Size: 55.5 MB (55519226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:24277a451c25923284bd552e52a477c6d5f0550d5bc4bf36c6f011cdab833f5a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.7 MB (45700581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ded18f1bc26bdd165c560e353704c774e72c61edf6306f0a301734b1cd592d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:54:51 GMT
ADD file:ba6c5e03457e69f59231e8e7c6465c1ec985812f0d8f7a65d9842f2be3e947fb in / 
# Thu, 16 Apr 2020 00:54:54 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 03:25:11 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 16 Apr 2020 03:25:36 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 03:26:21 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b7d527e4baf13a6c926fb354fe1b38cb42b96f249ae65fdc0f52c853b654e06e`  
		Last Modified: Thu, 16 Apr 2020 01:02:32 GMT  
		Size: 21.2 MB (21190797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8340381d358ecc9e44596343db49a1d8fe9fc408313742adb549d7acbfa010d9`  
		Last Modified: Thu, 16 Apr 2020 03:36:49 GMT  
		Size: 244.5 KB (244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c829c702c9ea78e5f1e834e27d5270a1aeb340e0c387fd2bcca835a6508a18`  
		Last Modified: Thu, 16 Apr 2020 03:36:59 GMT  
		Size: 24.3 MB (24265251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:82879b2317895d2b306e14bd38f26be346070655d8441662bd05aa9f85797783
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43105202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab6576fb1edf563a52cf0994636f3e1619b6508c783b4906ed59494f06d03533`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:05:08 GMT
ADD file:e37c4728c0c89ac126542ac35e7e493425c021bfac751079c9b266821a1b4e99 in / 
# Thu, 16 Apr 2020 01:05:10 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:43:14 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 16 Apr 2020 04:43:33 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 04:44:18 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f78d9963dfddc4747d6200353b50f6093a6e37ca82e1612fa397d64ff13e7299`  
		Last Modified: Thu, 16 Apr 2020 01:12:33 GMT  
		Size: 19.3 MB (19298546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf684cdea8a2272c82e09cbbb5024552c6e67b7dcf59ea62af547f9c730474e`  
		Last Modified: Thu, 16 Apr 2020 04:54:37 GMT  
		Size: 244.6 KB (244560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249d36139d8bc596df209162b7386211edf003733b4286aa7405033282389c33`  
		Last Modified: Thu, 16 Apr 2020 04:54:47 GMT  
		Size: 23.6 MB (23562096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:373e3d9ccf313cac211d9ede8eec8a2ccb1d1c0303fc5312fddfccc026277c41
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48771410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43f116c952bab72566e217b3d9571b9572c6e2ac731995c266825ca5ff059e14`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 02:45:19 GMT
ADD file:1588320d1c43714ec0353b7471f2ffd649045ca0f5f70dcb1eb064875fff9578 in / 
# Thu, 16 Apr 2020 02:45:21 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:49:41 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 16 Apr 2020 06:50:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:50:40 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8978c87ff45d64d1663a585dcf1ed66d9e711c2e4048d83ef561da9514ef46e6`  
		Last Modified: Thu, 16 Apr 2020 02:51:32 GMT  
		Size: 20.4 MB (20370106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554199a06aed010aa14e2e6ed810ac12e3f7ea1f01b4b484029b46c769a914b5`  
		Last Modified: Thu, 16 Apr 2020 07:00:00 GMT  
		Size: 244.4 KB (244384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f9c219c23779432f95dca105f2822e4e5cce0035ec90439890cb4ba1c4b3e0`  
		Last Modified: Thu, 16 Apr 2020 07:00:06 GMT  
		Size: 28.2 MB (28156920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5-slim` - linux; 386

```console
$ docker pull mono@sha256:22ba0007f042aa7ea555aef6e713a085984cf41290c3631975530fbc0e9b3648
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81943359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc471f7432a6acd1af4c999f8e978b7262817bd9a4d73655712d304817917e00`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:24 GMT
ADD file:0e72ab6d3f5ce06d7170bd6b0ceeda8687d1a5e2dab40308a8b8960d67fceffe in / 
# Thu, 16 Apr 2020 01:43:24 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:20:38 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 16 Apr 2020 06:20:48 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:21:29 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:706a1cdc903b54148ad6d5b672b2bafacadd79daffc0487b4949dd5d193f96f8`  
		Last Modified: Thu, 16 Apr 2020 01:49:33 GMT  
		Size: 23.1 MB (23141457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940906367b61b1c8c02650fa596d87e143b9b9e32639b66e59d0bbd65115133a`  
		Last Modified: Thu, 16 Apr 2020 06:31:23 GMT  
		Size: 244.5 KB (244472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f8edae7689fc4d1bd35e9614dfe86e03e42588bece0cf4d18c3b6c18e651c41`  
		Last Modified: Thu, 16 Apr 2020 06:31:48 GMT  
		Size: 58.6 MB (58557430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:8075f272b67d3b0230b83dec1f4ea321e0f9e68390fb4208b5cbfbde3e339a6c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.7 MB (47669710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b4f4a283b7df8fb74adb07675407330610860bf778c831f068775f705090dfd`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:57 GMT
ADD file:1c7f60f778e4b93490d570487d56275925e5eb477632e71cb9f035ce6edf2460 in / 
# Thu, 16 Apr 2020 01:44:03 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:44:48 GMT
ENV MONO_VERSION=5.20.1.34
# Thu, 16 Apr 2020 06:46:25 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:47:57 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:15e508b90ba1d327da83b72fc494ca263c1566ef6f70b91001cf2093395ffa3d`  
		Last Modified: Thu, 16 Apr 2020 02:04:33 GMT  
		Size: 22.8 MB (22785425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f669c3fbfce943d77701b69e7857eb6d1b88bbf7f9167a449d80be23eb3243`  
		Last Modified: Thu, 16 Apr 2020 07:19:18 GMT  
		Size: 244.6 KB (244638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c16782e8edab25bcd823ec760e3d334f1009343a5a1ef80520730ea6acd56e3`  
		Last Modified: Thu, 16 Apr 2020 07:19:25 GMT  
		Size: 24.6 MB (24639647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6`

```console
$ docker pull mono@sha256:b976fe5178f784ec89e63e12804e24408dde1be2a42b8715369350614b60f420
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
$ docker pull mono@sha256:81582109869f82484faaff740559cf18e92c7dbb6776d949ffd1584ed2052d07
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.1 MB (235136288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6258db5099bae58f82a4b00866b799387bf6f845a18647cbc4eff62573a03750`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:08 GMT
ADD file:e077f4d014ea0869fc4b3d5a3e6b3c8b792a97a8b4a328f33a994369225ff222 in / 
# Tue, 31 Mar 2020 01:24:08 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 20:53:54 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 31 Mar 2020 20:54:07 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 31 Mar 2020 20:54:46 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 31 Mar 2020 21:07:25 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:48839397421a64189661c2b86a34eb515d09a28204587a2b06b59df9f6e2d786`  
		Last Modified: Tue, 31 Mar 2020 01:29:28 GMT  
		Size: 22.5 MB (22513374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978d1e7775eef6eeed6c7cc7e4c060677dd6202aac3fa0913cd117b94e0b0729`  
		Last Modified: Tue, 31 Mar 2020 21:27:17 GMT  
		Size: 244.5 KB (244470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c82f16ec565f137b31bfb7a2102b30c050898aab6b0cb3a72cff11a75ee98d`  
		Last Modified: Tue, 31 Mar 2020 21:27:30 GMT  
		Size: 64.6 MB (64584224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b58815a2352a01b3b0ed3200dca917e29fd58f3690ff55bbf5b7456d7cdd10`  
		Last Modified: Tue, 31 Mar 2020 21:28:57 GMT  
		Size: 147.8 MB (147794220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; arm variant v5

```console
$ docker pull mono@sha256:039a6be7bba94963928fb63f0cd7624bdcc24ff437d3511659983bf8a15da61c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.7 MB (176695282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbb0da5905f2877688de5793cf7d5f0c6b5cdbb737868e678439fec995215cfa`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:54:51 GMT
ADD file:ba6c5e03457e69f59231e8e7c6465c1ec985812f0d8f7a65d9842f2be3e947fb in / 
# Thu, 16 Apr 2020 00:54:54 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 03:22:05 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 03:22:36 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 03:23:29 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 03:29:10 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b7d527e4baf13a6c926fb354fe1b38cb42b96f249ae65fdc0f52c853b654e06e`  
		Last Modified: Thu, 16 Apr 2020 01:02:32 GMT  
		Size: 21.2 MB (21190797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5251e801555d8cd1370a8d39ca953a0fb8f39729ff494b4a60bd03b4255c45be`  
		Last Modified: Thu, 16 Apr 2020 03:36:12 GMT  
		Size: 244.6 KB (244555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c9b96b75ebb7a3cac23cf75e27179b71b5aa2cee0c40c33aca6399e29516f2`  
		Last Modified: Thu, 16 Apr 2020 03:36:22 GMT  
		Size: 25.4 MB (25367763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33b43ad8da6addb8c852a68a9848cba5f48be98873fc8db208731eb55f31b9b`  
		Last Modified: Thu, 16 Apr 2020 03:37:53 GMT  
		Size: 129.9 MB (129892167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; arm variant v7

```console
$ docker pull mono@sha256:09076495aacfba71beb6f4e5812d597a2d059b58d0d1a053068e4fa0fdec8443
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.7 MB (172708239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6e489c47305d9f8c107b00d2a1e335c874014e8fa4a3fc5ecb9082df7c5be0f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:05:08 GMT
ADD file:e37c4728c0c89ac126542ac35e7e493425c021bfac751079c9b266821a1b4e99 in / 
# Thu, 16 Apr 2020 01:05:10 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:40:35 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 04:40:56 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 04:41:45 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 04:47:13 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f78d9963dfddc4747d6200353b50f6093a6e37ca82e1612fa397d64ff13e7299`  
		Last Modified: Thu, 16 Apr 2020 01:12:33 GMT  
		Size: 19.3 MB (19298546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70114347da279136ebd21697ef769dc5764f716c6f7331568bbf7306c17da63c`  
		Last Modified: Thu, 16 Apr 2020 04:54:02 GMT  
		Size: 244.6 KB (244551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802f26edffea7b59f9cc74e47561799e0c847d999b0db0dd2d99497c42af3511`  
		Last Modified: Thu, 16 Apr 2020 04:54:10 GMT  
		Size: 24.6 MB (24608740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a9fd3d7648204f077b0034260c1887fe3c12c26ffadbb4223d8dc7ff65c1eb`  
		Last Modified: Thu, 16 Apr 2020 04:55:42 GMT  
		Size: 128.6 MB (128556402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:abe9ae9da3ff9d1c710471ec6a5c1b39b18e33e11b0abba7d4245a3e75b11dc0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.7 MB (194747450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5a96031ff7018d8a3f1e18642728c41f24ad314d26c4fc40907ef19fce71fcd`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 02:45:19 GMT
ADD file:1588320d1c43714ec0353b7471f2ffd649045ca0f5f70dcb1eb064875fff9578 in / 
# Thu, 16 Apr 2020 02:45:21 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:47:03 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 06:47:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:48:05 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 06:53:15 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8978c87ff45d64d1663a585dcf1ed66d9e711c2e4048d83ef561da9514ef46e6`  
		Last Modified: Thu, 16 Apr 2020 02:51:32 GMT  
		Size: 20.4 MB (20370106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:090b996e11040b9a724d4b94b5f6fea43f5cee5558fdcdcb2e4627d1c596f82c`  
		Last Modified: Thu, 16 Apr 2020 06:59:20 GMT  
		Size: 244.4 KB (244369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be77ae0e8a98b883233d159b79364894a76d49f1b02badb9f57b227a26a8e1a`  
		Last Modified: Thu, 16 Apr 2020 06:59:30 GMT  
		Size: 29.4 MB (29420188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1774c3e17e0d83d02e086998900775da6efe1356459c585e7d5800434b5aaf21`  
		Last Modified: Thu, 16 Apr 2020 07:01:03 GMT  
		Size: 144.7 MB (144712787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; 386

```console
$ docker pull mono@sha256:1ebc75a12b856eab7355f64cd759c76ed529107995cb75f9e829cf2849cc0080
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.5 MB (243510596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04327a60fe104894839dc0076d6d5fb91bfada9228944cc9208c5855a57cea38`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:24 GMT
ADD file:0e72ab6d3f5ce06d7170bd6b0ceeda8687d1a5e2dab40308a8b8960d67fceffe in / 
# Thu, 16 Apr 2020 01:43:24 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:18:27 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 06:18:41 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:19:30 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 06:24:27 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:706a1cdc903b54148ad6d5b672b2bafacadd79daffc0487b4949dd5d193f96f8`  
		Last Modified: Thu, 16 Apr 2020 01:49:33 GMT  
		Size: 23.1 MB (23141457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667a9abd427eb4a5747168a8400ed0e9a6f9721abdc28627ceba31ffd4a687b2`  
		Last Modified: Thu, 16 Apr 2020 06:30:13 GMT  
		Size: 244.5 KB (244471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d7350249a79bb472729379d572433d2228dd8059cab2e58477277a9e66bb36`  
		Last Modified: Thu, 16 Apr 2020 06:30:40 GMT  
		Size: 68.6 MB (68631183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cf9820146ece539d30304f98e198b7bd9e334cae43f76008522272d551c88e`  
		Last Modified: Thu, 16 Apr 2020 06:32:59 GMT  
		Size: 151.5 MB (151493485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; ppc64le

```console
$ docker pull mono@sha256:0434d01a8617e75170a4dd8a638d786d1e67ac13c9fc880e023ccd0950428e36
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.0 MB (178997743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b5e14702ff1aff3bacfb8485b742086b08ff9d01cadd82d9f8327e6ac887fcc`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:57 GMT
ADD file:1c7f60f778e4b93490d570487d56275925e5eb477632e71cb9f035ce6edf2460 in / 
# Thu, 16 Apr 2020 01:44:03 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:37:42 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 06:39:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:41:27 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 06:58:08 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:15e508b90ba1d327da83b72fc494ca263c1566ef6f70b91001cf2093395ffa3d`  
		Last Modified: Thu, 16 Apr 2020 02:04:33 GMT  
		Size: 22.8 MB (22785425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1629fdf02d54d31ae3023cd8b4a515c3c17a085c6135c7a10e412896d06a1f62`  
		Last Modified: Thu, 16 Apr 2020 07:18:38 GMT  
		Size: 244.7 KB (244669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc63fa4246f2b9b66f762d8c33434e375c088c1ca73c3a389a8fb2525f93c7c`  
		Last Modified: Thu, 16 Apr 2020 07:18:43 GMT  
		Size: 25.8 MB (25775805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ed038a48cf0007c67072a64fc2d4d1d4efd20b275bff6a15884fcfe67b0afa`  
		Last Modified: Thu, 16 Apr 2020 07:20:07 GMT  
		Size: 130.2 MB (130191844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.6`

```console
$ docker pull mono@sha256:1940594089c52bedc2e9d08b8b46fb7b1875c70f55523603b337f6fc5a91870d
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
$ docker pull mono@sha256:c113ba90a42252d25544d7d0d27a99a8d8e553685cbf5c192895a31c1b0a45d2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.0 MB (233036642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e7c27d127f6836d2d4972e6b82e9046152464239ad8ac3aaad6696864c64e16`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:08 GMT
ADD file:e077f4d014ea0869fc4b3d5a3e6b3c8b792a97a8b4a328f33a994369225ff222 in / 
# Tue, 31 Mar 2020 01:24:08 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 20:54:58 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 31 Mar 2020 20:55:11 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 31 Mar 2020 20:55:43 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 31 Mar 2020 21:17:58 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:48839397421a64189661c2b86a34eb515d09a28204587a2b06b59df9f6e2d786`  
		Last Modified: Tue, 31 Mar 2020 01:29:28 GMT  
		Size: 22.5 MB (22513374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cef279d6fccf8f7a2abb49adc21335effaffbb8d81f78f8d30427551259df0a5`  
		Last Modified: Tue, 31 Mar 2020 21:27:36 GMT  
		Size: 244.5 KB (244469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32b6f35cb053886f016caeac50e475439029a048326710a2734fd3753f889de4`  
		Last Modified: Tue, 31 Mar 2020 21:27:50 GMT  
		Size: 63.0 MB (62971415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5fbda8a405c2b89e3d11bcafc37999c82f579869fa6abd74e9997263d00c626`  
		Last Modified: Tue, 31 Mar 2020 21:30:03 GMT  
		Size: 147.3 MB (147307384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6` - linux; arm variant v5

```console
$ docker pull mono@sha256:953b98f308c725c908039c6b0119c4308afde0a43bee73a9212123c246e3ba14
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.5 MB (176499196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30ab99fcbe0706e2c5cbf3b3f402c4f222fa6a4deec87d1658ac0883e0de7c94`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:54:51 GMT
ADD file:ba6c5e03457e69f59231e8e7c6465c1ec985812f0d8f7a65d9842f2be3e947fb in / 
# Thu, 16 Apr 2020 00:54:54 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 03:23:39 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 16 Apr 2020 03:24:08 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 03:25:01 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 03:32:10 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b7d527e4baf13a6c926fb354fe1b38cb42b96f249ae65fdc0f52c853b654e06e`  
		Last Modified: Thu, 16 Apr 2020 01:02:32 GMT  
		Size: 21.2 MB (21190797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2182e7eff26a84a3839979b8dc30f86f313c10d5a9c5cb556911ea13a0a09b7`  
		Last Modified: Thu, 16 Apr 2020 03:36:31 GMT  
		Size: 244.6 KB (244558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ecd30f76c6d61fc0338f94136d06ae87f496afd7cccaea0a67ef39cc037534`  
		Last Modified: Thu, 16 Apr 2020 03:36:42 GMT  
		Size: 25.4 MB (25414654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71bbeb6d8b71001853c4ac6381a1e2da4bed657325144da5a05f53de8571155b`  
		Last Modified: Thu, 16 Apr 2020 03:38:48 GMT  
		Size: 129.6 MB (129649187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6` - linux; arm variant v7

```console
$ docker pull mono@sha256:dfff052f102fe7d4378e5d2b0245680892904cbd70cb13786faf09e0ac56dfb3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.5 MB (172506927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b22ad409e9a2275f54ce587900650610baa7b303fd2f52317ef1049368fce42`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:05:08 GMT
ADD file:e37c4728c0c89ac126542ac35e7e493425c021bfac751079c9b266821a1b4e99 in / 
# Thu, 16 Apr 2020 01:05:10 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:41:55 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 16 Apr 2020 04:42:15 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 04:43:04 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 04:50:27 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f78d9963dfddc4747d6200353b50f6093a6e37ca82e1612fa397d64ff13e7299`  
		Last Modified: Thu, 16 Apr 2020 01:12:33 GMT  
		Size: 19.3 MB (19298546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c709444af1581614022f19533f2bd4e0a3468d7051453df34e50bf99df9321`  
		Last Modified: Thu, 16 Apr 2020 04:54:19 GMT  
		Size: 244.5 KB (244546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96b6dd89ea6225de279fd91629a436f6398c0547a59d1d7935d302802dec507`  
		Last Modified: Thu, 16 Apr 2020 04:54:29 GMT  
		Size: 24.6 MB (24648627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ff75ba1385b277ecc3e4c7e6201fd3706aa69b722a429fefcc75f0c5beb09b7`  
		Last Modified: Thu, 16 Apr 2020 04:56:40 GMT  
		Size: 128.3 MB (128315208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:d50f772e76b54a7da4d565208fcabf191b1246e0ad0853a269e282f7824d2623
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.4 MB (194394691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daed0db4cc3b4df6b71cd4424bfe0f98d8c6bffb99925929d809841240cd7d31`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 02:45:19 GMT
ADD file:1588320d1c43714ec0353b7471f2ffd649045ca0f5f70dcb1eb064875fff9578 in / 
# Thu, 16 Apr 2020 02:45:21 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:48:23 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 16 Apr 2020 06:48:40 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:49:27 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 06:56:13 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8978c87ff45d64d1663a585dcf1ed66d9e711c2e4048d83ef561da9514ef46e6`  
		Last Modified: Thu, 16 Apr 2020 02:51:32 GMT  
		Size: 20.4 MB (20370106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4cefd4f77cad9e57aea080af9eb57c1991ab847ef1ab0a04c72c47d4d11332`  
		Last Modified: Thu, 16 Apr 2020 06:59:39 GMT  
		Size: 244.4 KB (244371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a24563d28e05e4d85e2e968cf5a1be1fd764682e892a24a0323b2c2daee23a`  
		Last Modified: Thu, 16 Apr 2020 06:59:49 GMT  
		Size: 29.4 MB (29438693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5fd0d429b209d5930a2be3ed4225f606136251ea4a38b4a31f015eb3c3b25a`  
		Last Modified: Thu, 16 Apr 2020 07:02:02 GMT  
		Size: 144.3 MB (144341521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6` - linux; 386

```console
$ docker pull mono@sha256:29af9b6efa5143f1d81764b86b78d7db2504c7d04c5aa2386fe0bcf0476280f1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.3 MB (241294484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:890cca65def3382a543580173ca495ed0aba1a555f1e9a9d813b8d5f95714305`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:24 GMT
ADD file:0e72ab6d3f5ce06d7170bd6b0ceeda8687d1a5e2dab40308a8b8960d67fceffe in / 
# Thu, 16 Apr 2020 01:43:24 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:19:43 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 16 Apr 2020 06:19:53 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:20:30 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 06:27:14 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:706a1cdc903b54148ad6d5b672b2bafacadd79daffc0487b4949dd5d193f96f8`  
		Last Modified: Thu, 16 Apr 2020 01:49:33 GMT  
		Size: 23.1 MB (23141457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1abe5d8ecb0169b5a6a5ebb5bf709648f1815f3702100f598996f8d853daf674`  
		Last Modified: Thu, 16 Apr 2020 06:30:48 GMT  
		Size: 244.5 KB (244474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e284eb35520ad5064e9d622a563b63a88039f514d5267a8b326b02f796f17bff`  
		Last Modified: Thu, 16 Apr 2020 06:31:16 GMT  
		Size: 66.7 MB (66747525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8260d313d0b255843fe0fbb95f6ca70bccf372bd3bf7d269a7f5c81444dd0641`  
		Last Modified: Thu, 16 Apr 2020 06:34:12 GMT  
		Size: 151.2 MB (151161028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6` - linux; ppc64le

```console
$ docker pull mono@sha256:4235fd48012578b4b57f350c979ce60090348f15633d786dc80f4411f4c99add
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.8 MB (178801331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0e1d4c00d6874adca289180ab7f6005e5ac7d7624540b0086d8e64f470f7981`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:57 GMT
ADD file:1c7f60f778e4b93490d570487d56275925e5eb477632e71cb9f035ce6edf2460 in / 
# Thu, 16 Apr 2020 01:44:03 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:41:39 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 16 Apr 2020 06:42:53 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:44:39 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 07:10:39 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:15e508b90ba1d327da83b72fc494ca263c1566ef6f70b91001cf2093395ffa3d`  
		Last Modified: Thu, 16 Apr 2020 02:04:33 GMT  
		Size: 22.8 MB (22785425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800a5760720ebbe560ce8ace6be98139c4a1b70fe59bfc7d95e64b47f5b3d969`  
		Last Modified: Thu, 16 Apr 2020 07:19:01 GMT  
		Size: 244.6 KB (244581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f899767b86a83eb94a1fb10e4abe4060361f3991cd7998c06677ee9f1875d4`  
		Last Modified: Thu, 16 Apr 2020 07:19:06 GMT  
		Size: 25.8 MB (25828268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e9c715d026067720e1b2fda245dc97d172d2aeb0bd6be2d86bd4cc8807af4c`  
		Last Modified: Thu, 16 Apr 2020 07:20:54 GMT  
		Size: 129.9 MB (129943057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.6.0`

```console
$ docker pull mono@sha256:1940594089c52bedc2e9d08b8b46fb7b1875c70f55523603b337f6fc5a91870d
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
$ docker pull mono@sha256:c113ba90a42252d25544d7d0d27a99a8d8e553685cbf5c192895a31c1b0a45d2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.0 MB (233036642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e7c27d127f6836d2d4972e6b82e9046152464239ad8ac3aaad6696864c64e16`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:08 GMT
ADD file:e077f4d014ea0869fc4b3d5a3e6b3c8b792a97a8b4a328f33a994369225ff222 in / 
# Tue, 31 Mar 2020 01:24:08 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 20:54:58 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 31 Mar 2020 20:55:11 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 31 Mar 2020 20:55:43 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 31 Mar 2020 21:17:58 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:48839397421a64189661c2b86a34eb515d09a28204587a2b06b59df9f6e2d786`  
		Last Modified: Tue, 31 Mar 2020 01:29:28 GMT  
		Size: 22.5 MB (22513374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cef279d6fccf8f7a2abb49adc21335effaffbb8d81f78f8d30427551259df0a5`  
		Last Modified: Tue, 31 Mar 2020 21:27:36 GMT  
		Size: 244.5 KB (244469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32b6f35cb053886f016caeac50e475439029a048326710a2734fd3753f889de4`  
		Last Modified: Tue, 31 Mar 2020 21:27:50 GMT  
		Size: 63.0 MB (62971415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5fbda8a405c2b89e3d11bcafc37999c82f579869fa6abd74e9997263d00c626`  
		Last Modified: Tue, 31 Mar 2020 21:30:03 GMT  
		Size: 147.3 MB (147307384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0` - linux; arm variant v5

```console
$ docker pull mono@sha256:953b98f308c725c908039c6b0119c4308afde0a43bee73a9212123c246e3ba14
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.5 MB (176499196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30ab99fcbe0706e2c5cbf3b3f402c4f222fa6a4deec87d1658ac0883e0de7c94`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:54:51 GMT
ADD file:ba6c5e03457e69f59231e8e7c6465c1ec985812f0d8f7a65d9842f2be3e947fb in / 
# Thu, 16 Apr 2020 00:54:54 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 03:23:39 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 16 Apr 2020 03:24:08 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 03:25:01 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 03:32:10 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b7d527e4baf13a6c926fb354fe1b38cb42b96f249ae65fdc0f52c853b654e06e`  
		Last Modified: Thu, 16 Apr 2020 01:02:32 GMT  
		Size: 21.2 MB (21190797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2182e7eff26a84a3839979b8dc30f86f313c10d5a9c5cb556911ea13a0a09b7`  
		Last Modified: Thu, 16 Apr 2020 03:36:31 GMT  
		Size: 244.6 KB (244558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ecd30f76c6d61fc0338f94136d06ae87f496afd7cccaea0a67ef39cc037534`  
		Last Modified: Thu, 16 Apr 2020 03:36:42 GMT  
		Size: 25.4 MB (25414654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71bbeb6d8b71001853c4ac6381a1e2da4bed657325144da5a05f53de8571155b`  
		Last Modified: Thu, 16 Apr 2020 03:38:48 GMT  
		Size: 129.6 MB (129649187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0` - linux; arm variant v7

```console
$ docker pull mono@sha256:dfff052f102fe7d4378e5d2b0245680892904cbd70cb13786faf09e0ac56dfb3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.5 MB (172506927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b22ad409e9a2275f54ce587900650610baa7b303fd2f52317ef1049368fce42`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:05:08 GMT
ADD file:e37c4728c0c89ac126542ac35e7e493425c021bfac751079c9b266821a1b4e99 in / 
# Thu, 16 Apr 2020 01:05:10 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:41:55 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 16 Apr 2020 04:42:15 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 04:43:04 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 04:50:27 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f78d9963dfddc4747d6200353b50f6093a6e37ca82e1612fa397d64ff13e7299`  
		Last Modified: Thu, 16 Apr 2020 01:12:33 GMT  
		Size: 19.3 MB (19298546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c709444af1581614022f19533f2bd4e0a3468d7051453df34e50bf99df9321`  
		Last Modified: Thu, 16 Apr 2020 04:54:19 GMT  
		Size: 244.5 KB (244546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96b6dd89ea6225de279fd91629a436f6398c0547a59d1d7935d302802dec507`  
		Last Modified: Thu, 16 Apr 2020 04:54:29 GMT  
		Size: 24.6 MB (24648627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ff75ba1385b277ecc3e4c7e6201fd3706aa69b722a429fefcc75f0c5beb09b7`  
		Last Modified: Thu, 16 Apr 2020 04:56:40 GMT  
		Size: 128.3 MB (128315208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:d50f772e76b54a7da4d565208fcabf191b1246e0ad0853a269e282f7824d2623
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.4 MB (194394691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daed0db4cc3b4df6b71cd4424bfe0f98d8c6bffb99925929d809841240cd7d31`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 02:45:19 GMT
ADD file:1588320d1c43714ec0353b7471f2ffd649045ca0f5f70dcb1eb064875fff9578 in / 
# Thu, 16 Apr 2020 02:45:21 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:48:23 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 16 Apr 2020 06:48:40 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:49:27 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 06:56:13 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8978c87ff45d64d1663a585dcf1ed66d9e711c2e4048d83ef561da9514ef46e6`  
		Last Modified: Thu, 16 Apr 2020 02:51:32 GMT  
		Size: 20.4 MB (20370106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4cefd4f77cad9e57aea080af9eb57c1991ab847ef1ab0a04c72c47d4d11332`  
		Last Modified: Thu, 16 Apr 2020 06:59:39 GMT  
		Size: 244.4 KB (244371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a24563d28e05e4d85e2e968cf5a1be1fd764682e892a24a0323b2c2daee23a`  
		Last Modified: Thu, 16 Apr 2020 06:59:49 GMT  
		Size: 29.4 MB (29438693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5fd0d429b209d5930a2be3ed4225f606136251ea4a38b4a31f015eb3c3b25a`  
		Last Modified: Thu, 16 Apr 2020 07:02:02 GMT  
		Size: 144.3 MB (144341521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0` - linux; 386

```console
$ docker pull mono@sha256:29af9b6efa5143f1d81764b86b78d7db2504c7d04c5aa2386fe0bcf0476280f1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.3 MB (241294484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:890cca65def3382a543580173ca495ed0aba1a555f1e9a9d813b8d5f95714305`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:24 GMT
ADD file:0e72ab6d3f5ce06d7170bd6b0ceeda8687d1a5e2dab40308a8b8960d67fceffe in / 
# Thu, 16 Apr 2020 01:43:24 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:19:43 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 16 Apr 2020 06:19:53 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:20:30 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 06:27:14 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:706a1cdc903b54148ad6d5b672b2bafacadd79daffc0487b4949dd5d193f96f8`  
		Last Modified: Thu, 16 Apr 2020 01:49:33 GMT  
		Size: 23.1 MB (23141457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1abe5d8ecb0169b5a6a5ebb5bf709648f1815f3702100f598996f8d853daf674`  
		Last Modified: Thu, 16 Apr 2020 06:30:48 GMT  
		Size: 244.5 KB (244474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e284eb35520ad5064e9d622a563b63a88039f514d5267a8b326b02f796f17bff`  
		Last Modified: Thu, 16 Apr 2020 06:31:16 GMT  
		Size: 66.7 MB (66747525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8260d313d0b255843fe0fbb95f6ca70bccf372bd3bf7d269a7f5c81444dd0641`  
		Last Modified: Thu, 16 Apr 2020 06:34:12 GMT  
		Size: 151.2 MB (151161028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0` - linux; ppc64le

```console
$ docker pull mono@sha256:4235fd48012578b4b57f350c979ce60090348f15633d786dc80f4411f4c99add
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.8 MB (178801331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0e1d4c00d6874adca289180ab7f6005e5ac7d7624540b0086d8e64f470f7981`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:57 GMT
ADD file:1c7f60f778e4b93490d570487d56275925e5eb477632e71cb9f035ce6edf2460 in / 
# Thu, 16 Apr 2020 01:44:03 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:41:39 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 16 Apr 2020 06:42:53 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:44:39 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 07:10:39 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:15e508b90ba1d327da83b72fc494ca263c1566ef6f70b91001cf2093395ffa3d`  
		Last Modified: Thu, 16 Apr 2020 02:04:33 GMT  
		Size: 22.8 MB (22785425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800a5760720ebbe560ce8ace6be98139c4a1b70fe59bfc7d95e64b47f5b3d969`  
		Last Modified: Thu, 16 Apr 2020 07:19:01 GMT  
		Size: 244.6 KB (244581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f899767b86a83eb94a1fb10e4abe4060361f3991cd7998c06677ee9f1875d4`  
		Last Modified: Thu, 16 Apr 2020 07:19:06 GMT  
		Size: 25.8 MB (25828268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e9c715d026067720e1b2fda245dc97d172d2aeb0bd6be2d86bd4cc8807af4c`  
		Last Modified: Thu, 16 Apr 2020 07:20:54 GMT  
		Size: 129.9 MB (129943057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.6.0.161`

```console
$ docker pull mono@sha256:1940594089c52bedc2e9d08b8b46fb7b1875c70f55523603b337f6fc5a91870d
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
$ docker pull mono@sha256:c113ba90a42252d25544d7d0d27a99a8d8e553685cbf5c192895a31c1b0a45d2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.0 MB (233036642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e7c27d127f6836d2d4972e6b82e9046152464239ad8ac3aaad6696864c64e16`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:08 GMT
ADD file:e077f4d014ea0869fc4b3d5a3e6b3c8b792a97a8b4a328f33a994369225ff222 in / 
# Tue, 31 Mar 2020 01:24:08 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 20:54:58 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 31 Mar 2020 20:55:11 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 31 Mar 2020 20:55:43 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 31 Mar 2020 21:17:58 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:48839397421a64189661c2b86a34eb515d09a28204587a2b06b59df9f6e2d786`  
		Last Modified: Tue, 31 Mar 2020 01:29:28 GMT  
		Size: 22.5 MB (22513374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cef279d6fccf8f7a2abb49adc21335effaffbb8d81f78f8d30427551259df0a5`  
		Last Modified: Tue, 31 Mar 2020 21:27:36 GMT  
		Size: 244.5 KB (244469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32b6f35cb053886f016caeac50e475439029a048326710a2734fd3753f889de4`  
		Last Modified: Tue, 31 Mar 2020 21:27:50 GMT  
		Size: 63.0 MB (62971415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5fbda8a405c2b89e3d11bcafc37999c82f579869fa6abd74e9997263d00c626`  
		Last Modified: Tue, 31 Mar 2020 21:30:03 GMT  
		Size: 147.3 MB (147307384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0.161` - linux; arm variant v5

```console
$ docker pull mono@sha256:953b98f308c725c908039c6b0119c4308afde0a43bee73a9212123c246e3ba14
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.5 MB (176499196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30ab99fcbe0706e2c5cbf3b3f402c4f222fa6a4deec87d1658ac0883e0de7c94`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:54:51 GMT
ADD file:ba6c5e03457e69f59231e8e7c6465c1ec985812f0d8f7a65d9842f2be3e947fb in / 
# Thu, 16 Apr 2020 00:54:54 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 03:23:39 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 16 Apr 2020 03:24:08 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 03:25:01 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 03:32:10 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b7d527e4baf13a6c926fb354fe1b38cb42b96f249ae65fdc0f52c853b654e06e`  
		Last Modified: Thu, 16 Apr 2020 01:02:32 GMT  
		Size: 21.2 MB (21190797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2182e7eff26a84a3839979b8dc30f86f313c10d5a9c5cb556911ea13a0a09b7`  
		Last Modified: Thu, 16 Apr 2020 03:36:31 GMT  
		Size: 244.6 KB (244558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ecd30f76c6d61fc0338f94136d06ae87f496afd7cccaea0a67ef39cc037534`  
		Last Modified: Thu, 16 Apr 2020 03:36:42 GMT  
		Size: 25.4 MB (25414654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71bbeb6d8b71001853c4ac6381a1e2da4bed657325144da5a05f53de8571155b`  
		Last Modified: Thu, 16 Apr 2020 03:38:48 GMT  
		Size: 129.6 MB (129649187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0.161` - linux; arm variant v7

```console
$ docker pull mono@sha256:dfff052f102fe7d4378e5d2b0245680892904cbd70cb13786faf09e0ac56dfb3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.5 MB (172506927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b22ad409e9a2275f54ce587900650610baa7b303fd2f52317ef1049368fce42`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:05:08 GMT
ADD file:e37c4728c0c89ac126542ac35e7e493425c021bfac751079c9b266821a1b4e99 in / 
# Thu, 16 Apr 2020 01:05:10 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:41:55 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 16 Apr 2020 04:42:15 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 04:43:04 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 04:50:27 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f78d9963dfddc4747d6200353b50f6093a6e37ca82e1612fa397d64ff13e7299`  
		Last Modified: Thu, 16 Apr 2020 01:12:33 GMT  
		Size: 19.3 MB (19298546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c709444af1581614022f19533f2bd4e0a3468d7051453df34e50bf99df9321`  
		Last Modified: Thu, 16 Apr 2020 04:54:19 GMT  
		Size: 244.5 KB (244546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96b6dd89ea6225de279fd91629a436f6398c0547a59d1d7935d302802dec507`  
		Last Modified: Thu, 16 Apr 2020 04:54:29 GMT  
		Size: 24.6 MB (24648627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ff75ba1385b277ecc3e4c7e6201fd3706aa69b722a429fefcc75f0c5beb09b7`  
		Last Modified: Thu, 16 Apr 2020 04:56:40 GMT  
		Size: 128.3 MB (128315208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0.161` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:d50f772e76b54a7da4d565208fcabf191b1246e0ad0853a269e282f7824d2623
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.4 MB (194394691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daed0db4cc3b4df6b71cd4424bfe0f98d8c6bffb99925929d809841240cd7d31`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 02:45:19 GMT
ADD file:1588320d1c43714ec0353b7471f2ffd649045ca0f5f70dcb1eb064875fff9578 in / 
# Thu, 16 Apr 2020 02:45:21 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:48:23 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 16 Apr 2020 06:48:40 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:49:27 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 06:56:13 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8978c87ff45d64d1663a585dcf1ed66d9e711c2e4048d83ef561da9514ef46e6`  
		Last Modified: Thu, 16 Apr 2020 02:51:32 GMT  
		Size: 20.4 MB (20370106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4cefd4f77cad9e57aea080af9eb57c1991ab847ef1ab0a04c72c47d4d11332`  
		Last Modified: Thu, 16 Apr 2020 06:59:39 GMT  
		Size: 244.4 KB (244371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a24563d28e05e4d85e2e968cf5a1be1fd764682e892a24a0323b2c2daee23a`  
		Last Modified: Thu, 16 Apr 2020 06:59:49 GMT  
		Size: 29.4 MB (29438693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5fd0d429b209d5930a2be3ed4225f606136251ea4a38b4a31f015eb3c3b25a`  
		Last Modified: Thu, 16 Apr 2020 07:02:02 GMT  
		Size: 144.3 MB (144341521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0.161` - linux; 386

```console
$ docker pull mono@sha256:29af9b6efa5143f1d81764b86b78d7db2504c7d04c5aa2386fe0bcf0476280f1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.3 MB (241294484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:890cca65def3382a543580173ca495ed0aba1a555f1e9a9d813b8d5f95714305`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:24 GMT
ADD file:0e72ab6d3f5ce06d7170bd6b0ceeda8687d1a5e2dab40308a8b8960d67fceffe in / 
# Thu, 16 Apr 2020 01:43:24 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:19:43 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 16 Apr 2020 06:19:53 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:20:30 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 06:27:14 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:706a1cdc903b54148ad6d5b672b2bafacadd79daffc0487b4949dd5d193f96f8`  
		Last Modified: Thu, 16 Apr 2020 01:49:33 GMT  
		Size: 23.1 MB (23141457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1abe5d8ecb0169b5a6a5ebb5bf709648f1815f3702100f598996f8d853daf674`  
		Last Modified: Thu, 16 Apr 2020 06:30:48 GMT  
		Size: 244.5 KB (244474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e284eb35520ad5064e9d622a563b63a88039f514d5267a8b326b02f796f17bff`  
		Last Modified: Thu, 16 Apr 2020 06:31:16 GMT  
		Size: 66.7 MB (66747525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8260d313d0b255843fe0fbb95f6ca70bccf372bd3bf7d269a7f5c81444dd0641`  
		Last Modified: Thu, 16 Apr 2020 06:34:12 GMT  
		Size: 151.2 MB (151161028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0.161` - linux; ppc64le

```console
$ docker pull mono@sha256:4235fd48012578b4b57f350c979ce60090348f15633d786dc80f4411f4c99add
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.8 MB (178801331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0e1d4c00d6874adca289180ab7f6005e5ac7d7624540b0086d8e64f470f7981`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:57 GMT
ADD file:1c7f60f778e4b93490d570487d56275925e5eb477632e71cb9f035ce6edf2460 in / 
# Thu, 16 Apr 2020 01:44:03 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:41:39 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 16 Apr 2020 06:42:53 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:44:39 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 07:10:39 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:15e508b90ba1d327da83b72fc494ca263c1566ef6f70b91001cf2093395ffa3d`  
		Last Modified: Thu, 16 Apr 2020 02:04:33 GMT  
		Size: 22.8 MB (22785425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800a5760720ebbe560ce8ace6be98139c4a1b70fe59bfc7d95e64b47f5b3d969`  
		Last Modified: Thu, 16 Apr 2020 07:19:01 GMT  
		Size: 244.6 KB (244581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f899767b86a83eb94a1fb10e4abe4060361f3991cd7998c06677ee9f1875d4`  
		Last Modified: Thu, 16 Apr 2020 07:19:06 GMT  
		Size: 25.8 MB (25828268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e9c715d026067720e1b2fda245dc97d172d2aeb0bd6be2d86bd4cc8807af4c`  
		Last Modified: Thu, 16 Apr 2020 07:20:54 GMT  
		Size: 129.9 MB (129943057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.6.0.161-slim`

```console
$ docker pull mono@sha256:1e8791f254d91c23de48379f1773a820e50b9eba10e00d348ebd2727e24e661e
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
$ docker pull mono@sha256:08b421cc2fdffe7ad104feade9edbed46116944a9d608c06879c9b59207ae638
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.7 MB (85729258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b036ac2bee95a47d5f64e67c4bff1f8d6064ea6d2ce26e92fa6164d0b4d9197`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:08 GMT
ADD file:e077f4d014ea0869fc4b3d5a3e6b3c8b792a97a8b4a328f33a994369225ff222 in / 
# Tue, 31 Mar 2020 01:24:08 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 20:54:58 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 31 Mar 2020 20:55:11 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 31 Mar 2020 20:55:43 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:48839397421a64189661c2b86a34eb515d09a28204587a2b06b59df9f6e2d786`  
		Last Modified: Tue, 31 Mar 2020 01:29:28 GMT  
		Size: 22.5 MB (22513374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cef279d6fccf8f7a2abb49adc21335effaffbb8d81f78f8d30427551259df0a5`  
		Last Modified: Tue, 31 Mar 2020 21:27:36 GMT  
		Size: 244.5 KB (244469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32b6f35cb053886f016caeac50e475439029a048326710a2734fd3753f889de4`  
		Last Modified: Tue, 31 Mar 2020 21:27:50 GMT  
		Size: 63.0 MB (62971415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0.161-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:ff7be92bffd22f5c5c9ee40c5ca9dc8bfc0a339f7b2d1258d8fcd80f473fe8d9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46850009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cb507c773d86606ba4283207fa5d7c414c8a0e2600d98a83fab25e2a0000af4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:54:51 GMT
ADD file:ba6c5e03457e69f59231e8e7c6465c1ec985812f0d8f7a65d9842f2be3e947fb in / 
# Thu, 16 Apr 2020 00:54:54 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 03:23:39 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 16 Apr 2020 03:24:08 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 03:25:01 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b7d527e4baf13a6c926fb354fe1b38cb42b96f249ae65fdc0f52c853b654e06e`  
		Last Modified: Thu, 16 Apr 2020 01:02:32 GMT  
		Size: 21.2 MB (21190797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2182e7eff26a84a3839979b8dc30f86f313c10d5a9c5cb556911ea13a0a09b7`  
		Last Modified: Thu, 16 Apr 2020 03:36:31 GMT  
		Size: 244.6 KB (244558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ecd30f76c6d61fc0338f94136d06ae87f496afd7cccaea0a67ef39cc037534`  
		Last Modified: Thu, 16 Apr 2020 03:36:42 GMT  
		Size: 25.4 MB (25414654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0.161-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:178e41cc93222a41c9213913be27ccaef31e8bdae25c236b9bc7f15c586556fa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44191719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b603e30bde8ac1284185618c04169108253926d664211535358329cdba084966`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:05:08 GMT
ADD file:e37c4728c0c89ac126542ac35e7e493425c021bfac751079c9b266821a1b4e99 in / 
# Thu, 16 Apr 2020 01:05:10 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:41:55 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 16 Apr 2020 04:42:15 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 04:43:04 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f78d9963dfddc4747d6200353b50f6093a6e37ca82e1612fa397d64ff13e7299`  
		Last Modified: Thu, 16 Apr 2020 01:12:33 GMT  
		Size: 19.3 MB (19298546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c709444af1581614022f19533f2bd4e0a3468d7051453df34e50bf99df9321`  
		Last Modified: Thu, 16 Apr 2020 04:54:19 GMT  
		Size: 244.5 KB (244546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96b6dd89ea6225de279fd91629a436f6398c0547a59d1d7935d302802dec507`  
		Last Modified: Thu, 16 Apr 2020 04:54:29 GMT  
		Size: 24.6 MB (24648627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0.161-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:1073439807b38491b1361fa823ed651e7d2fe8946f4daa186cdb534c5806a53e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50053170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f03b552f7a35880b1429c8cd04ab1e514af560cdec6a4b938eec85fb4171df4a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 02:45:19 GMT
ADD file:1588320d1c43714ec0353b7471f2ffd649045ca0f5f70dcb1eb064875fff9578 in / 
# Thu, 16 Apr 2020 02:45:21 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:48:23 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 16 Apr 2020 06:48:40 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:49:27 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8978c87ff45d64d1663a585dcf1ed66d9e711c2e4048d83ef561da9514ef46e6`  
		Last Modified: Thu, 16 Apr 2020 02:51:32 GMT  
		Size: 20.4 MB (20370106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4cefd4f77cad9e57aea080af9eb57c1991ab847ef1ab0a04c72c47d4d11332`  
		Last Modified: Thu, 16 Apr 2020 06:59:39 GMT  
		Size: 244.4 KB (244371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a24563d28e05e4d85e2e968cf5a1be1fd764682e892a24a0323b2c2daee23a`  
		Last Modified: Thu, 16 Apr 2020 06:59:49 GMT  
		Size: 29.4 MB (29438693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0.161-slim` - linux; 386

```console
$ docker pull mono@sha256:3cc313cbfca08ea78bd3c962e3efd5f9ee92bb2c0d99f7bc5108c4dea2a4231b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.1 MB (90133456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3231fc9c710ac1ff331fb131df67fac40d08cdc7c62f3459f651486d469a6dfa`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:24 GMT
ADD file:0e72ab6d3f5ce06d7170bd6b0ceeda8687d1a5e2dab40308a8b8960d67fceffe in / 
# Thu, 16 Apr 2020 01:43:24 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:19:43 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 16 Apr 2020 06:19:53 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:20:30 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:706a1cdc903b54148ad6d5b672b2bafacadd79daffc0487b4949dd5d193f96f8`  
		Last Modified: Thu, 16 Apr 2020 01:49:33 GMT  
		Size: 23.1 MB (23141457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1abe5d8ecb0169b5a6a5ebb5bf709648f1815f3702100f598996f8d853daf674`  
		Last Modified: Thu, 16 Apr 2020 06:30:48 GMT  
		Size: 244.5 KB (244474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e284eb35520ad5064e9d622a563b63a88039f514d5267a8b326b02f796f17bff`  
		Last Modified: Thu, 16 Apr 2020 06:31:16 GMT  
		Size: 66.7 MB (66747525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0.161-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:fe2739cc6a3e74a354559a9adf6a4ef35e99e02919f63f61a638212d94db1cf3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48858274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a7b23b2940938c882d83d74c0abfcb54a61b2ffe4ee58f84c629f4339ea2007`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:57 GMT
ADD file:1c7f60f778e4b93490d570487d56275925e5eb477632e71cb9f035ce6edf2460 in / 
# Thu, 16 Apr 2020 01:44:03 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:41:39 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 16 Apr 2020 06:42:53 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:44:39 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:15e508b90ba1d327da83b72fc494ca263c1566ef6f70b91001cf2093395ffa3d`  
		Last Modified: Thu, 16 Apr 2020 02:04:33 GMT  
		Size: 22.8 MB (22785425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800a5760720ebbe560ce8ace6be98139c4a1b70fe59bfc7d95e64b47f5b3d969`  
		Last Modified: Thu, 16 Apr 2020 07:19:01 GMT  
		Size: 244.6 KB (244581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f899767b86a83eb94a1fb10e4abe4060361f3991cd7998c06677ee9f1875d4`  
		Last Modified: Thu, 16 Apr 2020 07:19:06 GMT  
		Size: 25.8 MB (25828268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.6.0-slim`

```console
$ docker pull mono@sha256:1e8791f254d91c23de48379f1773a820e50b9eba10e00d348ebd2727e24e661e
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
$ docker pull mono@sha256:08b421cc2fdffe7ad104feade9edbed46116944a9d608c06879c9b59207ae638
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.7 MB (85729258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b036ac2bee95a47d5f64e67c4bff1f8d6064ea6d2ce26e92fa6164d0b4d9197`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:08 GMT
ADD file:e077f4d014ea0869fc4b3d5a3e6b3c8b792a97a8b4a328f33a994369225ff222 in / 
# Tue, 31 Mar 2020 01:24:08 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 20:54:58 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 31 Mar 2020 20:55:11 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 31 Mar 2020 20:55:43 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:48839397421a64189661c2b86a34eb515d09a28204587a2b06b59df9f6e2d786`  
		Last Modified: Tue, 31 Mar 2020 01:29:28 GMT  
		Size: 22.5 MB (22513374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cef279d6fccf8f7a2abb49adc21335effaffbb8d81f78f8d30427551259df0a5`  
		Last Modified: Tue, 31 Mar 2020 21:27:36 GMT  
		Size: 244.5 KB (244469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32b6f35cb053886f016caeac50e475439029a048326710a2734fd3753f889de4`  
		Last Modified: Tue, 31 Mar 2020 21:27:50 GMT  
		Size: 63.0 MB (62971415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:ff7be92bffd22f5c5c9ee40c5ca9dc8bfc0a339f7b2d1258d8fcd80f473fe8d9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46850009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cb507c773d86606ba4283207fa5d7c414c8a0e2600d98a83fab25e2a0000af4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:54:51 GMT
ADD file:ba6c5e03457e69f59231e8e7c6465c1ec985812f0d8f7a65d9842f2be3e947fb in / 
# Thu, 16 Apr 2020 00:54:54 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 03:23:39 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 16 Apr 2020 03:24:08 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 03:25:01 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b7d527e4baf13a6c926fb354fe1b38cb42b96f249ae65fdc0f52c853b654e06e`  
		Last Modified: Thu, 16 Apr 2020 01:02:32 GMT  
		Size: 21.2 MB (21190797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2182e7eff26a84a3839979b8dc30f86f313c10d5a9c5cb556911ea13a0a09b7`  
		Last Modified: Thu, 16 Apr 2020 03:36:31 GMT  
		Size: 244.6 KB (244558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ecd30f76c6d61fc0338f94136d06ae87f496afd7cccaea0a67ef39cc037534`  
		Last Modified: Thu, 16 Apr 2020 03:36:42 GMT  
		Size: 25.4 MB (25414654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:178e41cc93222a41c9213913be27ccaef31e8bdae25c236b9bc7f15c586556fa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44191719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b603e30bde8ac1284185618c04169108253926d664211535358329cdba084966`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:05:08 GMT
ADD file:e37c4728c0c89ac126542ac35e7e493425c021bfac751079c9b266821a1b4e99 in / 
# Thu, 16 Apr 2020 01:05:10 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:41:55 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 16 Apr 2020 04:42:15 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 04:43:04 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f78d9963dfddc4747d6200353b50f6093a6e37ca82e1612fa397d64ff13e7299`  
		Last Modified: Thu, 16 Apr 2020 01:12:33 GMT  
		Size: 19.3 MB (19298546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c709444af1581614022f19533f2bd4e0a3468d7051453df34e50bf99df9321`  
		Last Modified: Thu, 16 Apr 2020 04:54:19 GMT  
		Size: 244.5 KB (244546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96b6dd89ea6225de279fd91629a436f6398c0547a59d1d7935d302802dec507`  
		Last Modified: Thu, 16 Apr 2020 04:54:29 GMT  
		Size: 24.6 MB (24648627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:1073439807b38491b1361fa823ed651e7d2fe8946f4daa186cdb534c5806a53e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50053170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f03b552f7a35880b1429c8cd04ab1e514af560cdec6a4b938eec85fb4171df4a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 02:45:19 GMT
ADD file:1588320d1c43714ec0353b7471f2ffd649045ca0f5f70dcb1eb064875fff9578 in / 
# Thu, 16 Apr 2020 02:45:21 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:48:23 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 16 Apr 2020 06:48:40 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:49:27 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8978c87ff45d64d1663a585dcf1ed66d9e711c2e4048d83ef561da9514ef46e6`  
		Last Modified: Thu, 16 Apr 2020 02:51:32 GMT  
		Size: 20.4 MB (20370106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4cefd4f77cad9e57aea080af9eb57c1991ab847ef1ab0a04c72c47d4d11332`  
		Last Modified: Thu, 16 Apr 2020 06:59:39 GMT  
		Size: 244.4 KB (244371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a24563d28e05e4d85e2e968cf5a1be1fd764682e892a24a0323b2c2daee23a`  
		Last Modified: Thu, 16 Apr 2020 06:59:49 GMT  
		Size: 29.4 MB (29438693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0-slim` - linux; 386

```console
$ docker pull mono@sha256:3cc313cbfca08ea78bd3c962e3efd5f9ee92bb2c0d99f7bc5108c4dea2a4231b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.1 MB (90133456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3231fc9c710ac1ff331fb131df67fac40d08cdc7c62f3459f651486d469a6dfa`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:24 GMT
ADD file:0e72ab6d3f5ce06d7170bd6b0ceeda8687d1a5e2dab40308a8b8960d67fceffe in / 
# Thu, 16 Apr 2020 01:43:24 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:19:43 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 16 Apr 2020 06:19:53 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:20:30 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:706a1cdc903b54148ad6d5b672b2bafacadd79daffc0487b4949dd5d193f96f8`  
		Last Modified: Thu, 16 Apr 2020 01:49:33 GMT  
		Size: 23.1 MB (23141457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1abe5d8ecb0169b5a6a5ebb5bf709648f1815f3702100f598996f8d853daf674`  
		Last Modified: Thu, 16 Apr 2020 06:30:48 GMT  
		Size: 244.5 KB (244474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e284eb35520ad5064e9d622a563b63a88039f514d5267a8b326b02f796f17bff`  
		Last Modified: Thu, 16 Apr 2020 06:31:16 GMT  
		Size: 66.7 MB (66747525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:fe2739cc6a3e74a354559a9adf6a4ef35e99e02919f63f61a638212d94db1cf3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48858274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a7b23b2940938c882d83d74c0abfcb54a61b2ffe4ee58f84c629f4339ea2007`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:57 GMT
ADD file:1c7f60f778e4b93490d570487d56275925e5eb477632e71cb9f035ce6edf2460 in / 
# Thu, 16 Apr 2020 01:44:03 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:41:39 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 16 Apr 2020 06:42:53 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:44:39 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:15e508b90ba1d327da83b72fc494ca263c1566ef6f70b91001cf2093395ffa3d`  
		Last Modified: Thu, 16 Apr 2020 02:04:33 GMT  
		Size: 22.8 MB (22785425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800a5760720ebbe560ce8ace6be98139c4a1b70fe59bfc7d95e64b47f5b3d969`  
		Last Modified: Thu, 16 Apr 2020 07:19:01 GMT  
		Size: 244.6 KB (244581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f899767b86a83eb94a1fb10e4abe4060361f3991cd7998c06677ee9f1875d4`  
		Last Modified: Thu, 16 Apr 2020 07:19:06 GMT  
		Size: 25.8 MB (25828268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.6-slim`

```console
$ docker pull mono@sha256:1e8791f254d91c23de48379f1773a820e50b9eba10e00d348ebd2727e24e661e
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
$ docker pull mono@sha256:08b421cc2fdffe7ad104feade9edbed46116944a9d608c06879c9b59207ae638
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.7 MB (85729258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b036ac2bee95a47d5f64e67c4bff1f8d6064ea6d2ce26e92fa6164d0b4d9197`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:08 GMT
ADD file:e077f4d014ea0869fc4b3d5a3e6b3c8b792a97a8b4a328f33a994369225ff222 in / 
# Tue, 31 Mar 2020 01:24:08 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 20:54:58 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 31 Mar 2020 20:55:11 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 31 Mar 2020 20:55:43 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:48839397421a64189661c2b86a34eb515d09a28204587a2b06b59df9f6e2d786`  
		Last Modified: Tue, 31 Mar 2020 01:29:28 GMT  
		Size: 22.5 MB (22513374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cef279d6fccf8f7a2abb49adc21335effaffbb8d81f78f8d30427551259df0a5`  
		Last Modified: Tue, 31 Mar 2020 21:27:36 GMT  
		Size: 244.5 KB (244469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32b6f35cb053886f016caeac50e475439029a048326710a2734fd3753f889de4`  
		Last Modified: Tue, 31 Mar 2020 21:27:50 GMT  
		Size: 63.0 MB (62971415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:ff7be92bffd22f5c5c9ee40c5ca9dc8bfc0a339f7b2d1258d8fcd80f473fe8d9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46850009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cb507c773d86606ba4283207fa5d7c414c8a0e2600d98a83fab25e2a0000af4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:54:51 GMT
ADD file:ba6c5e03457e69f59231e8e7c6465c1ec985812f0d8f7a65d9842f2be3e947fb in / 
# Thu, 16 Apr 2020 00:54:54 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 03:23:39 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 16 Apr 2020 03:24:08 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 03:25:01 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b7d527e4baf13a6c926fb354fe1b38cb42b96f249ae65fdc0f52c853b654e06e`  
		Last Modified: Thu, 16 Apr 2020 01:02:32 GMT  
		Size: 21.2 MB (21190797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2182e7eff26a84a3839979b8dc30f86f313c10d5a9c5cb556911ea13a0a09b7`  
		Last Modified: Thu, 16 Apr 2020 03:36:31 GMT  
		Size: 244.6 KB (244558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ecd30f76c6d61fc0338f94136d06ae87f496afd7cccaea0a67ef39cc037534`  
		Last Modified: Thu, 16 Apr 2020 03:36:42 GMT  
		Size: 25.4 MB (25414654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:178e41cc93222a41c9213913be27ccaef31e8bdae25c236b9bc7f15c586556fa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44191719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b603e30bde8ac1284185618c04169108253926d664211535358329cdba084966`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:05:08 GMT
ADD file:e37c4728c0c89ac126542ac35e7e493425c021bfac751079c9b266821a1b4e99 in / 
# Thu, 16 Apr 2020 01:05:10 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:41:55 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 16 Apr 2020 04:42:15 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 04:43:04 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f78d9963dfddc4747d6200353b50f6093a6e37ca82e1612fa397d64ff13e7299`  
		Last Modified: Thu, 16 Apr 2020 01:12:33 GMT  
		Size: 19.3 MB (19298546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c709444af1581614022f19533f2bd4e0a3468d7051453df34e50bf99df9321`  
		Last Modified: Thu, 16 Apr 2020 04:54:19 GMT  
		Size: 244.5 KB (244546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96b6dd89ea6225de279fd91629a436f6398c0547a59d1d7935d302802dec507`  
		Last Modified: Thu, 16 Apr 2020 04:54:29 GMT  
		Size: 24.6 MB (24648627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:1073439807b38491b1361fa823ed651e7d2fe8946f4daa186cdb534c5806a53e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50053170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f03b552f7a35880b1429c8cd04ab1e514af560cdec6a4b938eec85fb4171df4a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 02:45:19 GMT
ADD file:1588320d1c43714ec0353b7471f2ffd649045ca0f5f70dcb1eb064875fff9578 in / 
# Thu, 16 Apr 2020 02:45:21 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:48:23 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 16 Apr 2020 06:48:40 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:49:27 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8978c87ff45d64d1663a585dcf1ed66d9e711c2e4048d83ef561da9514ef46e6`  
		Last Modified: Thu, 16 Apr 2020 02:51:32 GMT  
		Size: 20.4 MB (20370106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4cefd4f77cad9e57aea080af9eb57c1991ab847ef1ab0a04c72c47d4d11332`  
		Last Modified: Thu, 16 Apr 2020 06:59:39 GMT  
		Size: 244.4 KB (244371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a24563d28e05e4d85e2e968cf5a1be1fd764682e892a24a0323b2c2daee23a`  
		Last Modified: Thu, 16 Apr 2020 06:59:49 GMT  
		Size: 29.4 MB (29438693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6-slim` - linux; 386

```console
$ docker pull mono@sha256:3cc313cbfca08ea78bd3c962e3efd5f9ee92bb2c0d99f7bc5108c4dea2a4231b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.1 MB (90133456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3231fc9c710ac1ff331fb131df67fac40d08cdc7c62f3459f651486d469a6dfa`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:24 GMT
ADD file:0e72ab6d3f5ce06d7170bd6b0ceeda8687d1a5e2dab40308a8b8960d67fceffe in / 
# Thu, 16 Apr 2020 01:43:24 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:19:43 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 16 Apr 2020 06:19:53 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:20:30 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:706a1cdc903b54148ad6d5b672b2bafacadd79daffc0487b4949dd5d193f96f8`  
		Last Modified: Thu, 16 Apr 2020 01:49:33 GMT  
		Size: 23.1 MB (23141457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1abe5d8ecb0169b5a6a5ebb5bf709648f1815f3702100f598996f8d853daf674`  
		Last Modified: Thu, 16 Apr 2020 06:30:48 GMT  
		Size: 244.5 KB (244474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e284eb35520ad5064e9d622a563b63a88039f514d5267a8b326b02f796f17bff`  
		Last Modified: Thu, 16 Apr 2020 06:31:16 GMT  
		Size: 66.7 MB (66747525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:fe2739cc6a3e74a354559a9adf6a4ef35e99e02919f63f61a638212d94db1cf3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48858274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a7b23b2940938c882d83d74c0abfcb54a61b2ffe4ee58f84c629f4339ea2007`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:57 GMT
ADD file:1c7f60f778e4b93490d570487d56275925e5eb477632e71cb9f035ce6edf2460 in / 
# Thu, 16 Apr 2020 01:44:03 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:41:39 GMT
ENV MONO_VERSION=6.6.0.161
# Thu, 16 Apr 2020 06:42:53 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:44:39 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:15e508b90ba1d327da83b72fc494ca263c1566ef6f70b91001cf2093395ffa3d`  
		Last Modified: Thu, 16 Apr 2020 02:04:33 GMT  
		Size: 22.8 MB (22785425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800a5760720ebbe560ce8ace6be98139c4a1b70fe59bfc7d95e64b47f5b3d969`  
		Last Modified: Thu, 16 Apr 2020 07:19:01 GMT  
		Size: 244.6 KB (244581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f899767b86a83eb94a1fb10e4abe4060361f3991cd7998c06677ee9f1875d4`  
		Last Modified: Thu, 16 Apr 2020 07:19:06 GMT  
		Size: 25.8 MB (25828268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.8`

```console
$ docker pull mono@sha256:b976fe5178f784ec89e63e12804e24408dde1be2a42b8715369350614b60f420
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
$ docker pull mono@sha256:81582109869f82484faaff740559cf18e92c7dbb6776d949ffd1584ed2052d07
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.1 MB (235136288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6258db5099bae58f82a4b00866b799387bf6f845a18647cbc4eff62573a03750`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:08 GMT
ADD file:e077f4d014ea0869fc4b3d5a3e6b3c8b792a97a8b4a328f33a994369225ff222 in / 
# Tue, 31 Mar 2020 01:24:08 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 20:53:54 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 31 Mar 2020 20:54:07 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 31 Mar 2020 20:54:46 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 31 Mar 2020 21:07:25 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:48839397421a64189661c2b86a34eb515d09a28204587a2b06b59df9f6e2d786`  
		Last Modified: Tue, 31 Mar 2020 01:29:28 GMT  
		Size: 22.5 MB (22513374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978d1e7775eef6eeed6c7cc7e4c060677dd6202aac3fa0913cd117b94e0b0729`  
		Last Modified: Tue, 31 Mar 2020 21:27:17 GMT  
		Size: 244.5 KB (244470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c82f16ec565f137b31bfb7a2102b30c050898aab6b0cb3a72cff11a75ee98d`  
		Last Modified: Tue, 31 Mar 2020 21:27:30 GMT  
		Size: 64.6 MB (64584224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b58815a2352a01b3b0ed3200dca917e29fd58f3690ff55bbf5b7456d7cdd10`  
		Last Modified: Tue, 31 Mar 2020 21:28:57 GMT  
		Size: 147.8 MB (147794220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8` - linux; arm variant v5

```console
$ docker pull mono@sha256:039a6be7bba94963928fb63f0cd7624bdcc24ff437d3511659983bf8a15da61c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.7 MB (176695282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbb0da5905f2877688de5793cf7d5f0c6b5cdbb737868e678439fec995215cfa`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:54:51 GMT
ADD file:ba6c5e03457e69f59231e8e7c6465c1ec985812f0d8f7a65d9842f2be3e947fb in / 
# Thu, 16 Apr 2020 00:54:54 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 03:22:05 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 03:22:36 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 03:23:29 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 03:29:10 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b7d527e4baf13a6c926fb354fe1b38cb42b96f249ae65fdc0f52c853b654e06e`  
		Last Modified: Thu, 16 Apr 2020 01:02:32 GMT  
		Size: 21.2 MB (21190797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5251e801555d8cd1370a8d39ca953a0fb8f39729ff494b4a60bd03b4255c45be`  
		Last Modified: Thu, 16 Apr 2020 03:36:12 GMT  
		Size: 244.6 KB (244555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c9b96b75ebb7a3cac23cf75e27179b71b5aa2cee0c40c33aca6399e29516f2`  
		Last Modified: Thu, 16 Apr 2020 03:36:22 GMT  
		Size: 25.4 MB (25367763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33b43ad8da6addb8c852a68a9848cba5f48be98873fc8db208731eb55f31b9b`  
		Last Modified: Thu, 16 Apr 2020 03:37:53 GMT  
		Size: 129.9 MB (129892167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8` - linux; arm variant v7

```console
$ docker pull mono@sha256:09076495aacfba71beb6f4e5812d597a2d059b58d0d1a053068e4fa0fdec8443
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.7 MB (172708239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6e489c47305d9f8c107b00d2a1e335c874014e8fa4a3fc5ecb9082df7c5be0f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:05:08 GMT
ADD file:e37c4728c0c89ac126542ac35e7e493425c021bfac751079c9b266821a1b4e99 in / 
# Thu, 16 Apr 2020 01:05:10 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:40:35 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 04:40:56 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 04:41:45 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 04:47:13 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f78d9963dfddc4747d6200353b50f6093a6e37ca82e1612fa397d64ff13e7299`  
		Last Modified: Thu, 16 Apr 2020 01:12:33 GMT  
		Size: 19.3 MB (19298546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70114347da279136ebd21697ef769dc5764f716c6f7331568bbf7306c17da63c`  
		Last Modified: Thu, 16 Apr 2020 04:54:02 GMT  
		Size: 244.6 KB (244551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802f26edffea7b59f9cc74e47561799e0c847d999b0db0dd2d99497c42af3511`  
		Last Modified: Thu, 16 Apr 2020 04:54:10 GMT  
		Size: 24.6 MB (24608740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a9fd3d7648204f077b0034260c1887fe3c12c26ffadbb4223d8dc7ff65c1eb`  
		Last Modified: Thu, 16 Apr 2020 04:55:42 GMT  
		Size: 128.6 MB (128556402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:abe9ae9da3ff9d1c710471ec6a5c1b39b18e33e11b0abba7d4245a3e75b11dc0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.7 MB (194747450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5a96031ff7018d8a3f1e18642728c41f24ad314d26c4fc40907ef19fce71fcd`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 02:45:19 GMT
ADD file:1588320d1c43714ec0353b7471f2ffd649045ca0f5f70dcb1eb064875fff9578 in / 
# Thu, 16 Apr 2020 02:45:21 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:47:03 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 06:47:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:48:05 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 06:53:15 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8978c87ff45d64d1663a585dcf1ed66d9e711c2e4048d83ef561da9514ef46e6`  
		Last Modified: Thu, 16 Apr 2020 02:51:32 GMT  
		Size: 20.4 MB (20370106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:090b996e11040b9a724d4b94b5f6fea43f5cee5558fdcdcb2e4627d1c596f82c`  
		Last Modified: Thu, 16 Apr 2020 06:59:20 GMT  
		Size: 244.4 KB (244369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be77ae0e8a98b883233d159b79364894a76d49f1b02badb9f57b227a26a8e1a`  
		Last Modified: Thu, 16 Apr 2020 06:59:30 GMT  
		Size: 29.4 MB (29420188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1774c3e17e0d83d02e086998900775da6efe1356459c585e7d5800434b5aaf21`  
		Last Modified: Thu, 16 Apr 2020 07:01:03 GMT  
		Size: 144.7 MB (144712787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8` - linux; 386

```console
$ docker pull mono@sha256:1ebc75a12b856eab7355f64cd759c76ed529107995cb75f9e829cf2849cc0080
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.5 MB (243510596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04327a60fe104894839dc0076d6d5fb91bfada9228944cc9208c5855a57cea38`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:24 GMT
ADD file:0e72ab6d3f5ce06d7170bd6b0ceeda8687d1a5e2dab40308a8b8960d67fceffe in / 
# Thu, 16 Apr 2020 01:43:24 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:18:27 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 06:18:41 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:19:30 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 06:24:27 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:706a1cdc903b54148ad6d5b672b2bafacadd79daffc0487b4949dd5d193f96f8`  
		Last Modified: Thu, 16 Apr 2020 01:49:33 GMT  
		Size: 23.1 MB (23141457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667a9abd427eb4a5747168a8400ed0e9a6f9721abdc28627ceba31ffd4a687b2`  
		Last Modified: Thu, 16 Apr 2020 06:30:13 GMT  
		Size: 244.5 KB (244471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d7350249a79bb472729379d572433d2228dd8059cab2e58477277a9e66bb36`  
		Last Modified: Thu, 16 Apr 2020 06:30:40 GMT  
		Size: 68.6 MB (68631183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cf9820146ece539d30304f98e198b7bd9e334cae43f76008522272d551c88e`  
		Last Modified: Thu, 16 Apr 2020 06:32:59 GMT  
		Size: 151.5 MB (151493485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8` - linux; ppc64le

```console
$ docker pull mono@sha256:0434d01a8617e75170a4dd8a638d786d1e67ac13c9fc880e023ccd0950428e36
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.0 MB (178997743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b5e14702ff1aff3bacfb8485b742086b08ff9d01cadd82d9f8327e6ac887fcc`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:57 GMT
ADD file:1c7f60f778e4b93490d570487d56275925e5eb477632e71cb9f035ce6edf2460 in / 
# Thu, 16 Apr 2020 01:44:03 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:37:42 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 06:39:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:41:27 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 06:58:08 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:15e508b90ba1d327da83b72fc494ca263c1566ef6f70b91001cf2093395ffa3d`  
		Last Modified: Thu, 16 Apr 2020 02:04:33 GMT  
		Size: 22.8 MB (22785425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1629fdf02d54d31ae3023cd8b4a515c3c17a085c6135c7a10e412896d06a1f62`  
		Last Modified: Thu, 16 Apr 2020 07:18:38 GMT  
		Size: 244.7 KB (244669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc63fa4246f2b9b66f762d8c33434e375c088c1ca73c3a389a8fb2525f93c7c`  
		Last Modified: Thu, 16 Apr 2020 07:18:43 GMT  
		Size: 25.8 MB (25775805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ed038a48cf0007c67072a64fc2d4d1d4efd20b275bff6a15884fcfe67b0afa`  
		Last Modified: Thu, 16 Apr 2020 07:20:07 GMT  
		Size: 130.2 MB (130191844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.8.0`

```console
$ docker pull mono@sha256:b976fe5178f784ec89e63e12804e24408dde1be2a42b8715369350614b60f420
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
$ docker pull mono@sha256:81582109869f82484faaff740559cf18e92c7dbb6776d949ffd1584ed2052d07
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.1 MB (235136288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6258db5099bae58f82a4b00866b799387bf6f845a18647cbc4eff62573a03750`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:08 GMT
ADD file:e077f4d014ea0869fc4b3d5a3e6b3c8b792a97a8b4a328f33a994369225ff222 in / 
# Tue, 31 Mar 2020 01:24:08 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 20:53:54 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 31 Mar 2020 20:54:07 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 31 Mar 2020 20:54:46 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 31 Mar 2020 21:07:25 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:48839397421a64189661c2b86a34eb515d09a28204587a2b06b59df9f6e2d786`  
		Last Modified: Tue, 31 Mar 2020 01:29:28 GMT  
		Size: 22.5 MB (22513374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978d1e7775eef6eeed6c7cc7e4c060677dd6202aac3fa0913cd117b94e0b0729`  
		Last Modified: Tue, 31 Mar 2020 21:27:17 GMT  
		Size: 244.5 KB (244470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c82f16ec565f137b31bfb7a2102b30c050898aab6b0cb3a72cff11a75ee98d`  
		Last Modified: Tue, 31 Mar 2020 21:27:30 GMT  
		Size: 64.6 MB (64584224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b58815a2352a01b3b0ed3200dca917e29fd58f3690ff55bbf5b7456d7cdd10`  
		Last Modified: Tue, 31 Mar 2020 21:28:57 GMT  
		Size: 147.8 MB (147794220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0` - linux; arm variant v5

```console
$ docker pull mono@sha256:039a6be7bba94963928fb63f0cd7624bdcc24ff437d3511659983bf8a15da61c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.7 MB (176695282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbb0da5905f2877688de5793cf7d5f0c6b5cdbb737868e678439fec995215cfa`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:54:51 GMT
ADD file:ba6c5e03457e69f59231e8e7c6465c1ec985812f0d8f7a65d9842f2be3e947fb in / 
# Thu, 16 Apr 2020 00:54:54 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 03:22:05 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 03:22:36 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 03:23:29 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 03:29:10 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b7d527e4baf13a6c926fb354fe1b38cb42b96f249ae65fdc0f52c853b654e06e`  
		Last Modified: Thu, 16 Apr 2020 01:02:32 GMT  
		Size: 21.2 MB (21190797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5251e801555d8cd1370a8d39ca953a0fb8f39729ff494b4a60bd03b4255c45be`  
		Last Modified: Thu, 16 Apr 2020 03:36:12 GMT  
		Size: 244.6 KB (244555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c9b96b75ebb7a3cac23cf75e27179b71b5aa2cee0c40c33aca6399e29516f2`  
		Last Modified: Thu, 16 Apr 2020 03:36:22 GMT  
		Size: 25.4 MB (25367763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33b43ad8da6addb8c852a68a9848cba5f48be98873fc8db208731eb55f31b9b`  
		Last Modified: Thu, 16 Apr 2020 03:37:53 GMT  
		Size: 129.9 MB (129892167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0` - linux; arm variant v7

```console
$ docker pull mono@sha256:09076495aacfba71beb6f4e5812d597a2d059b58d0d1a053068e4fa0fdec8443
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.7 MB (172708239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6e489c47305d9f8c107b00d2a1e335c874014e8fa4a3fc5ecb9082df7c5be0f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:05:08 GMT
ADD file:e37c4728c0c89ac126542ac35e7e493425c021bfac751079c9b266821a1b4e99 in / 
# Thu, 16 Apr 2020 01:05:10 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:40:35 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 04:40:56 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 04:41:45 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 04:47:13 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f78d9963dfddc4747d6200353b50f6093a6e37ca82e1612fa397d64ff13e7299`  
		Last Modified: Thu, 16 Apr 2020 01:12:33 GMT  
		Size: 19.3 MB (19298546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70114347da279136ebd21697ef769dc5764f716c6f7331568bbf7306c17da63c`  
		Last Modified: Thu, 16 Apr 2020 04:54:02 GMT  
		Size: 244.6 KB (244551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802f26edffea7b59f9cc74e47561799e0c847d999b0db0dd2d99497c42af3511`  
		Last Modified: Thu, 16 Apr 2020 04:54:10 GMT  
		Size: 24.6 MB (24608740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a9fd3d7648204f077b0034260c1887fe3c12c26ffadbb4223d8dc7ff65c1eb`  
		Last Modified: Thu, 16 Apr 2020 04:55:42 GMT  
		Size: 128.6 MB (128556402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:abe9ae9da3ff9d1c710471ec6a5c1b39b18e33e11b0abba7d4245a3e75b11dc0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.7 MB (194747450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5a96031ff7018d8a3f1e18642728c41f24ad314d26c4fc40907ef19fce71fcd`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 02:45:19 GMT
ADD file:1588320d1c43714ec0353b7471f2ffd649045ca0f5f70dcb1eb064875fff9578 in / 
# Thu, 16 Apr 2020 02:45:21 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:47:03 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 06:47:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:48:05 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 06:53:15 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8978c87ff45d64d1663a585dcf1ed66d9e711c2e4048d83ef561da9514ef46e6`  
		Last Modified: Thu, 16 Apr 2020 02:51:32 GMT  
		Size: 20.4 MB (20370106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:090b996e11040b9a724d4b94b5f6fea43f5cee5558fdcdcb2e4627d1c596f82c`  
		Last Modified: Thu, 16 Apr 2020 06:59:20 GMT  
		Size: 244.4 KB (244369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be77ae0e8a98b883233d159b79364894a76d49f1b02badb9f57b227a26a8e1a`  
		Last Modified: Thu, 16 Apr 2020 06:59:30 GMT  
		Size: 29.4 MB (29420188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1774c3e17e0d83d02e086998900775da6efe1356459c585e7d5800434b5aaf21`  
		Last Modified: Thu, 16 Apr 2020 07:01:03 GMT  
		Size: 144.7 MB (144712787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0` - linux; 386

```console
$ docker pull mono@sha256:1ebc75a12b856eab7355f64cd759c76ed529107995cb75f9e829cf2849cc0080
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.5 MB (243510596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04327a60fe104894839dc0076d6d5fb91bfada9228944cc9208c5855a57cea38`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:24 GMT
ADD file:0e72ab6d3f5ce06d7170bd6b0ceeda8687d1a5e2dab40308a8b8960d67fceffe in / 
# Thu, 16 Apr 2020 01:43:24 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:18:27 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 06:18:41 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:19:30 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 06:24:27 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:706a1cdc903b54148ad6d5b672b2bafacadd79daffc0487b4949dd5d193f96f8`  
		Last Modified: Thu, 16 Apr 2020 01:49:33 GMT  
		Size: 23.1 MB (23141457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667a9abd427eb4a5747168a8400ed0e9a6f9721abdc28627ceba31ffd4a687b2`  
		Last Modified: Thu, 16 Apr 2020 06:30:13 GMT  
		Size: 244.5 KB (244471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d7350249a79bb472729379d572433d2228dd8059cab2e58477277a9e66bb36`  
		Last Modified: Thu, 16 Apr 2020 06:30:40 GMT  
		Size: 68.6 MB (68631183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cf9820146ece539d30304f98e198b7bd9e334cae43f76008522272d551c88e`  
		Last Modified: Thu, 16 Apr 2020 06:32:59 GMT  
		Size: 151.5 MB (151493485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0` - linux; ppc64le

```console
$ docker pull mono@sha256:0434d01a8617e75170a4dd8a638d786d1e67ac13c9fc880e023ccd0950428e36
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.0 MB (178997743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b5e14702ff1aff3bacfb8485b742086b08ff9d01cadd82d9f8327e6ac887fcc`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:57 GMT
ADD file:1c7f60f778e4b93490d570487d56275925e5eb477632e71cb9f035ce6edf2460 in / 
# Thu, 16 Apr 2020 01:44:03 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:37:42 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 06:39:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:41:27 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 06:58:08 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:15e508b90ba1d327da83b72fc494ca263c1566ef6f70b91001cf2093395ffa3d`  
		Last Modified: Thu, 16 Apr 2020 02:04:33 GMT  
		Size: 22.8 MB (22785425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1629fdf02d54d31ae3023cd8b4a515c3c17a085c6135c7a10e412896d06a1f62`  
		Last Modified: Thu, 16 Apr 2020 07:18:38 GMT  
		Size: 244.7 KB (244669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc63fa4246f2b9b66f762d8c33434e375c088c1ca73c3a389a8fb2525f93c7c`  
		Last Modified: Thu, 16 Apr 2020 07:18:43 GMT  
		Size: 25.8 MB (25775805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ed038a48cf0007c67072a64fc2d4d1d4efd20b275bff6a15884fcfe67b0afa`  
		Last Modified: Thu, 16 Apr 2020 07:20:07 GMT  
		Size: 130.2 MB (130191844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.8.0.96`

```console
$ docker pull mono@sha256:b976fe5178f784ec89e63e12804e24408dde1be2a42b8715369350614b60f420
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
$ docker pull mono@sha256:81582109869f82484faaff740559cf18e92c7dbb6776d949ffd1584ed2052d07
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.1 MB (235136288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6258db5099bae58f82a4b00866b799387bf6f845a18647cbc4eff62573a03750`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:08 GMT
ADD file:e077f4d014ea0869fc4b3d5a3e6b3c8b792a97a8b4a328f33a994369225ff222 in / 
# Tue, 31 Mar 2020 01:24:08 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 20:53:54 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 31 Mar 2020 20:54:07 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 31 Mar 2020 20:54:46 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 31 Mar 2020 21:07:25 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:48839397421a64189661c2b86a34eb515d09a28204587a2b06b59df9f6e2d786`  
		Last Modified: Tue, 31 Mar 2020 01:29:28 GMT  
		Size: 22.5 MB (22513374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978d1e7775eef6eeed6c7cc7e4c060677dd6202aac3fa0913cd117b94e0b0729`  
		Last Modified: Tue, 31 Mar 2020 21:27:17 GMT  
		Size: 244.5 KB (244470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c82f16ec565f137b31bfb7a2102b30c050898aab6b0cb3a72cff11a75ee98d`  
		Last Modified: Tue, 31 Mar 2020 21:27:30 GMT  
		Size: 64.6 MB (64584224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b58815a2352a01b3b0ed3200dca917e29fd58f3690ff55bbf5b7456d7cdd10`  
		Last Modified: Tue, 31 Mar 2020 21:28:57 GMT  
		Size: 147.8 MB (147794220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.96` - linux; arm variant v5

```console
$ docker pull mono@sha256:039a6be7bba94963928fb63f0cd7624bdcc24ff437d3511659983bf8a15da61c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.7 MB (176695282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbb0da5905f2877688de5793cf7d5f0c6b5cdbb737868e678439fec995215cfa`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:54:51 GMT
ADD file:ba6c5e03457e69f59231e8e7c6465c1ec985812f0d8f7a65d9842f2be3e947fb in / 
# Thu, 16 Apr 2020 00:54:54 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 03:22:05 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 03:22:36 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 03:23:29 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 03:29:10 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b7d527e4baf13a6c926fb354fe1b38cb42b96f249ae65fdc0f52c853b654e06e`  
		Last Modified: Thu, 16 Apr 2020 01:02:32 GMT  
		Size: 21.2 MB (21190797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5251e801555d8cd1370a8d39ca953a0fb8f39729ff494b4a60bd03b4255c45be`  
		Last Modified: Thu, 16 Apr 2020 03:36:12 GMT  
		Size: 244.6 KB (244555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c9b96b75ebb7a3cac23cf75e27179b71b5aa2cee0c40c33aca6399e29516f2`  
		Last Modified: Thu, 16 Apr 2020 03:36:22 GMT  
		Size: 25.4 MB (25367763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33b43ad8da6addb8c852a68a9848cba5f48be98873fc8db208731eb55f31b9b`  
		Last Modified: Thu, 16 Apr 2020 03:37:53 GMT  
		Size: 129.9 MB (129892167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.96` - linux; arm variant v7

```console
$ docker pull mono@sha256:09076495aacfba71beb6f4e5812d597a2d059b58d0d1a053068e4fa0fdec8443
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.7 MB (172708239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6e489c47305d9f8c107b00d2a1e335c874014e8fa4a3fc5ecb9082df7c5be0f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:05:08 GMT
ADD file:e37c4728c0c89ac126542ac35e7e493425c021bfac751079c9b266821a1b4e99 in / 
# Thu, 16 Apr 2020 01:05:10 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:40:35 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 04:40:56 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 04:41:45 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 04:47:13 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f78d9963dfddc4747d6200353b50f6093a6e37ca82e1612fa397d64ff13e7299`  
		Last Modified: Thu, 16 Apr 2020 01:12:33 GMT  
		Size: 19.3 MB (19298546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70114347da279136ebd21697ef769dc5764f716c6f7331568bbf7306c17da63c`  
		Last Modified: Thu, 16 Apr 2020 04:54:02 GMT  
		Size: 244.6 KB (244551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802f26edffea7b59f9cc74e47561799e0c847d999b0db0dd2d99497c42af3511`  
		Last Modified: Thu, 16 Apr 2020 04:54:10 GMT  
		Size: 24.6 MB (24608740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a9fd3d7648204f077b0034260c1887fe3c12c26ffadbb4223d8dc7ff65c1eb`  
		Last Modified: Thu, 16 Apr 2020 04:55:42 GMT  
		Size: 128.6 MB (128556402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.96` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:abe9ae9da3ff9d1c710471ec6a5c1b39b18e33e11b0abba7d4245a3e75b11dc0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.7 MB (194747450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5a96031ff7018d8a3f1e18642728c41f24ad314d26c4fc40907ef19fce71fcd`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 02:45:19 GMT
ADD file:1588320d1c43714ec0353b7471f2ffd649045ca0f5f70dcb1eb064875fff9578 in / 
# Thu, 16 Apr 2020 02:45:21 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:47:03 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 06:47:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:48:05 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 06:53:15 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8978c87ff45d64d1663a585dcf1ed66d9e711c2e4048d83ef561da9514ef46e6`  
		Last Modified: Thu, 16 Apr 2020 02:51:32 GMT  
		Size: 20.4 MB (20370106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:090b996e11040b9a724d4b94b5f6fea43f5cee5558fdcdcb2e4627d1c596f82c`  
		Last Modified: Thu, 16 Apr 2020 06:59:20 GMT  
		Size: 244.4 KB (244369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be77ae0e8a98b883233d159b79364894a76d49f1b02badb9f57b227a26a8e1a`  
		Last Modified: Thu, 16 Apr 2020 06:59:30 GMT  
		Size: 29.4 MB (29420188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1774c3e17e0d83d02e086998900775da6efe1356459c585e7d5800434b5aaf21`  
		Last Modified: Thu, 16 Apr 2020 07:01:03 GMT  
		Size: 144.7 MB (144712787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.96` - linux; 386

```console
$ docker pull mono@sha256:1ebc75a12b856eab7355f64cd759c76ed529107995cb75f9e829cf2849cc0080
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.5 MB (243510596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04327a60fe104894839dc0076d6d5fb91bfada9228944cc9208c5855a57cea38`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:24 GMT
ADD file:0e72ab6d3f5ce06d7170bd6b0ceeda8687d1a5e2dab40308a8b8960d67fceffe in / 
# Thu, 16 Apr 2020 01:43:24 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:18:27 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 06:18:41 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:19:30 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 06:24:27 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:706a1cdc903b54148ad6d5b672b2bafacadd79daffc0487b4949dd5d193f96f8`  
		Last Modified: Thu, 16 Apr 2020 01:49:33 GMT  
		Size: 23.1 MB (23141457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667a9abd427eb4a5747168a8400ed0e9a6f9721abdc28627ceba31ffd4a687b2`  
		Last Modified: Thu, 16 Apr 2020 06:30:13 GMT  
		Size: 244.5 KB (244471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d7350249a79bb472729379d572433d2228dd8059cab2e58477277a9e66bb36`  
		Last Modified: Thu, 16 Apr 2020 06:30:40 GMT  
		Size: 68.6 MB (68631183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cf9820146ece539d30304f98e198b7bd9e334cae43f76008522272d551c88e`  
		Last Modified: Thu, 16 Apr 2020 06:32:59 GMT  
		Size: 151.5 MB (151493485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.96` - linux; ppc64le

```console
$ docker pull mono@sha256:0434d01a8617e75170a4dd8a638d786d1e67ac13c9fc880e023ccd0950428e36
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.0 MB (178997743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b5e14702ff1aff3bacfb8485b742086b08ff9d01cadd82d9f8327e6ac887fcc`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:57 GMT
ADD file:1c7f60f778e4b93490d570487d56275925e5eb477632e71cb9f035ce6edf2460 in / 
# Thu, 16 Apr 2020 01:44:03 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:37:42 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 06:39:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:41:27 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 06:58:08 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:15e508b90ba1d327da83b72fc494ca263c1566ef6f70b91001cf2093395ffa3d`  
		Last Modified: Thu, 16 Apr 2020 02:04:33 GMT  
		Size: 22.8 MB (22785425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1629fdf02d54d31ae3023cd8b4a515c3c17a085c6135c7a10e412896d06a1f62`  
		Last Modified: Thu, 16 Apr 2020 07:18:38 GMT  
		Size: 244.7 KB (244669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc63fa4246f2b9b66f762d8c33434e375c088c1ca73c3a389a8fb2525f93c7c`  
		Last Modified: Thu, 16 Apr 2020 07:18:43 GMT  
		Size: 25.8 MB (25775805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ed038a48cf0007c67072a64fc2d4d1d4efd20b275bff6a15884fcfe67b0afa`  
		Last Modified: Thu, 16 Apr 2020 07:20:07 GMT  
		Size: 130.2 MB (130191844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.8.0.96-slim`

```console
$ docker pull mono@sha256:e283cd94cb3d139f1dfad8ff78c39cde4ef3f418b53745ce1194ea44adc7c694
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
$ docker pull mono@sha256:16ad829001a98d74a3d32f80f5865bdc3f6ec6bc0bbdb514069e3ff2956b8664
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.3 MB (87342068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:755f960b5885e01b06366f22620568cc1ca381b5d88f46e3904bee4016fed03e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:08 GMT
ADD file:e077f4d014ea0869fc4b3d5a3e6b3c8b792a97a8b4a328f33a994369225ff222 in / 
# Tue, 31 Mar 2020 01:24:08 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 20:53:54 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 31 Mar 2020 20:54:07 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 31 Mar 2020 20:54:46 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:48839397421a64189661c2b86a34eb515d09a28204587a2b06b59df9f6e2d786`  
		Last Modified: Tue, 31 Mar 2020 01:29:28 GMT  
		Size: 22.5 MB (22513374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978d1e7775eef6eeed6c7cc7e4c060677dd6202aac3fa0913cd117b94e0b0729`  
		Last Modified: Tue, 31 Mar 2020 21:27:17 GMT  
		Size: 244.5 KB (244470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c82f16ec565f137b31bfb7a2102b30c050898aab6b0cb3a72cff11a75ee98d`  
		Last Modified: Tue, 31 Mar 2020 21:27:30 GMT  
		Size: 64.6 MB (64584224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.96-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:988781ce7fd3739dba6c395332912434cb391801f362378ff13316fdc0c50a3b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.8 MB (46803115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8e01bfb2e90fa41fdda2d35621f00b8a0d51e600f008dd4e4518771218af14c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:54:51 GMT
ADD file:ba6c5e03457e69f59231e8e7c6465c1ec985812f0d8f7a65d9842f2be3e947fb in / 
# Thu, 16 Apr 2020 00:54:54 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 03:22:05 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 03:22:36 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 03:23:29 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b7d527e4baf13a6c926fb354fe1b38cb42b96f249ae65fdc0f52c853b654e06e`  
		Last Modified: Thu, 16 Apr 2020 01:02:32 GMT  
		Size: 21.2 MB (21190797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5251e801555d8cd1370a8d39ca953a0fb8f39729ff494b4a60bd03b4255c45be`  
		Last Modified: Thu, 16 Apr 2020 03:36:12 GMT  
		Size: 244.6 KB (244555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c9b96b75ebb7a3cac23cf75e27179b71b5aa2cee0c40c33aca6399e29516f2`  
		Last Modified: Thu, 16 Apr 2020 03:36:22 GMT  
		Size: 25.4 MB (25367763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.96-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:fec0e4861eab05dd7c3eb364beefae8f8d5fc2ef225162e038b210af4cb3d508
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44151837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b78272cf77806b892fb8ce1da5a728ff7eaee3e059bb9ed6a77bd80478f1be7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:05:08 GMT
ADD file:e37c4728c0c89ac126542ac35e7e493425c021bfac751079c9b266821a1b4e99 in / 
# Thu, 16 Apr 2020 01:05:10 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:40:35 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 04:40:56 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 04:41:45 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f78d9963dfddc4747d6200353b50f6093a6e37ca82e1612fa397d64ff13e7299`  
		Last Modified: Thu, 16 Apr 2020 01:12:33 GMT  
		Size: 19.3 MB (19298546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70114347da279136ebd21697ef769dc5764f716c6f7331568bbf7306c17da63c`  
		Last Modified: Thu, 16 Apr 2020 04:54:02 GMT  
		Size: 244.6 KB (244551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802f26edffea7b59f9cc74e47561799e0c847d999b0db0dd2d99497c42af3511`  
		Last Modified: Thu, 16 Apr 2020 04:54:10 GMT  
		Size: 24.6 MB (24608740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.96-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:d08953373b3ef1fc7db79f7f13d8698af415ccec4a187b24ccd2e20c729b8c7d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.0 MB (50034663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4c3ba9afd0517a25a4e83d0efc8b8d5d84880dbcc969fd912d6ce0463995374`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 02:45:19 GMT
ADD file:1588320d1c43714ec0353b7471f2ffd649045ca0f5f70dcb1eb064875fff9578 in / 
# Thu, 16 Apr 2020 02:45:21 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:47:03 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 06:47:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:48:05 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8978c87ff45d64d1663a585dcf1ed66d9e711c2e4048d83ef561da9514ef46e6`  
		Last Modified: Thu, 16 Apr 2020 02:51:32 GMT  
		Size: 20.4 MB (20370106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:090b996e11040b9a724d4b94b5f6fea43f5cee5558fdcdcb2e4627d1c596f82c`  
		Last Modified: Thu, 16 Apr 2020 06:59:20 GMT  
		Size: 244.4 KB (244369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be77ae0e8a98b883233d159b79364894a76d49f1b02badb9f57b227a26a8e1a`  
		Last Modified: Thu, 16 Apr 2020 06:59:30 GMT  
		Size: 29.4 MB (29420188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.96-slim` - linux; 386

```console
$ docker pull mono@sha256:1bd521f164e72bfedaa4b84ff032becb6cd48254d229233d338e39d68c234afb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.0 MB (92017111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae15c2b3c37ced7865f4ee9b7312cae7e74e77a42ea630787456d7efe775ed93`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:24 GMT
ADD file:0e72ab6d3f5ce06d7170bd6b0ceeda8687d1a5e2dab40308a8b8960d67fceffe in / 
# Thu, 16 Apr 2020 01:43:24 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:18:27 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 06:18:41 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:19:30 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:706a1cdc903b54148ad6d5b672b2bafacadd79daffc0487b4949dd5d193f96f8`  
		Last Modified: Thu, 16 Apr 2020 01:49:33 GMT  
		Size: 23.1 MB (23141457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667a9abd427eb4a5747168a8400ed0e9a6f9721abdc28627ceba31ffd4a687b2`  
		Last Modified: Thu, 16 Apr 2020 06:30:13 GMT  
		Size: 244.5 KB (244471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d7350249a79bb472729379d572433d2228dd8059cab2e58477277a9e66bb36`  
		Last Modified: Thu, 16 Apr 2020 06:30:40 GMT  
		Size: 68.6 MB (68631183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.96-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:fa72fc4c116a54fd72fa979ab6db10a3798c1a0719a1b40884ceabbb476291c2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48805899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccafa8bda50e8b6b041a02bca8290435a0dac26f6b7f52a0f59d6d21222413f1`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:57 GMT
ADD file:1c7f60f778e4b93490d570487d56275925e5eb477632e71cb9f035ce6edf2460 in / 
# Thu, 16 Apr 2020 01:44:03 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:37:42 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 06:39:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:41:27 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:15e508b90ba1d327da83b72fc494ca263c1566ef6f70b91001cf2093395ffa3d`  
		Last Modified: Thu, 16 Apr 2020 02:04:33 GMT  
		Size: 22.8 MB (22785425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1629fdf02d54d31ae3023cd8b4a515c3c17a085c6135c7a10e412896d06a1f62`  
		Last Modified: Thu, 16 Apr 2020 07:18:38 GMT  
		Size: 244.7 KB (244669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc63fa4246f2b9b66f762d8c33434e375c088c1ca73c3a389a8fb2525f93c7c`  
		Last Modified: Thu, 16 Apr 2020 07:18:43 GMT  
		Size: 25.8 MB (25775805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.8.0-slim`

```console
$ docker pull mono@sha256:e283cd94cb3d139f1dfad8ff78c39cde4ef3f418b53745ce1194ea44adc7c694
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
$ docker pull mono@sha256:16ad829001a98d74a3d32f80f5865bdc3f6ec6bc0bbdb514069e3ff2956b8664
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.3 MB (87342068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:755f960b5885e01b06366f22620568cc1ca381b5d88f46e3904bee4016fed03e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:08 GMT
ADD file:e077f4d014ea0869fc4b3d5a3e6b3c8b792a97a8b4a328f33a994369225ff222 in / 
# Tue, 31 Mar 2020 01:24:08 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 20:53:54 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 31 Mar 2020 20:54:07 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 31 Mar 2020 20:54:46 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:48839397421a64189661c2b86a34eb515d09a28204587a2b06b59df9f6e2d786`  
		Last Modified: Tue, 31 Mar 2020 01:29:28 GMT  
		Size: 22.5 MB (22513374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978d1e7775eef6eeed6c7cc7e4c060677dd6202aac3fa0913cd117b94e0b0729`  
		Last Modified: Tue, 31 Mar 2020 21:27:17 GMT  
		Size: 244.5 KB (244470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c82f16ec565f137b31bfb7a2102b30c050898aab6b0cb3a72cff11a75ee98d`  
		Last Modified: Tue, 31 Mar 2020 21:27:30 GMT  
		Size: 64.6 MB (64584224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:988781ce7fd3739dba6c395332912434cb391801f362378ff13316fdc0c50a3b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.8 MB (46803115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8e01bfb2e90fa41fdda2d35621f00b8a0d51e600f008dd4e4518771218af14c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:54:51 GMT
ADD file:ba6c5e03457e69f59231e8e7c6465c1ec985812f0d8f7a65d9842f2be3e947fb in / 
# Thu, 16 Apr 2020 00:54:54 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 03:22:05 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 03:22:36 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 03:23:29 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b7d527e4baf13a6c926fb354fe1b38cb42b96f249ae65fdc0f52c853b654e06e`  
		Last Modified: Thu, 16 Apr 2020 01:02:32 GMT  
		Size: 21.2 MB (21190797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5251e801555d8cd1370a8d39ca953a0fb8f39729ff494b4a60bd03b4255c45be`  
		Last Modified: Thu, 16 Apr 2020 03:36:12 GMT  
		Size: 244.6 KB (244555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c9b96b75ebb7a3cac23cf75e27179b71b5aa2cee0c40c33aca6399e29516f2`  
		Last Modified: Thu, 16 Apr 2020 03:36:22 GMT  
		Size: 25.4 MB (25367763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:fec0e4861eab05dd7c3eb364beefae8f8d5fc2ef225162e038b210af4cb3d508
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44151837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b78272cf77806b892fb8ce1da5a728ff7eaee3e059bb9ed6a77bd80478f1be7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:05:08 GMT
ADD file:e37c4728c0c89ac126542ac35e7e493425c021bfac751079c9b266821a1b4e99 in / 
# Thu, 16 Apr 2020 01:05:10 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:40:35 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 04:40:56 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 04:41:45 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f78d9963dfddc4747d6200353b50f6093a6e37ca82e1612fa397d64ff13e7299`  
		Last Modified: Thu, 16 Apr 2020 01:12:33 GMT  
		Size: 19.3 MB (19298546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70114347da279136ebd21697ef769dc5764f716c6f7331568bbf7306c17da63c`  
		Last Modified: Thu, 16 Apr 2020 04:54:02 GMT  
		Size: 244.6 KB (244551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802f26edffea7b59f9cc74e47561799e0c847d999b0db0dd2d99497c42af3511`  
		Last Modified: Thu, 16 Apr 2020 04:54:10 GMT  
		Size: 24.6 MB (24608740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:d08953373b3ef1fc7db79f7f13d8698af415ccec4a187b24ccd2e20c729b8c7d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.0 MB (50034663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4c3ba9afd0517a25a4e83d0efc8b8d5d84880dbcc969fd912d6ce0463995374`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 02:45:19 GMT
ADD file:1588320d1c43714ec0353b7471f2ffd649045ca0f5f70dcb1eb064875fff9578 in / 
# Thu, 16 Apr 2020 02:45:21 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:47:03 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 06:47:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:48:05 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8978c87ff45d64d1663a585dcf1ed66d9e711c2e4048d83ef561da9514ef46e6`  
		Last Modified: Thu, 16 Apr 2020 02:51:32 GMT  
		Size: 20.4 MB (20370106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:090b996e11040b9a724d4b94b5f6fea43f5cee5558fdcdcb2e4627d1c596f82c`  
		Last Modified: Thu, 16 Apr 2020 06:59:20 GMT  
		Size: 244.4 KB (244369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be77ae0e8a98b883233d159b79364894a76d49f1b02badb9f57b227a26a8e1a`  
		Last Modified: Thu, 16 Apr 2020 06:59:30 GMT  
		Size: 29.4 MB (29420188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0-slim` - linux; 386

```console
$ docker pull mono@sha256:1bd521f164e72bfedaa4b84ff032becb6cd48254d229233d338e39d68c234afb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.0 MB (92017111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae15c2b3c37ced7865f4ee9b7312cae7e74e77a42ea630787456d7efe775ed93`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:24 GMT
ADD file:0e72ab6d3f5ce06d7170bd6b0ceeda8687d1a5e2dab40308a8b8960d67fceffe in / 
# Thu, 16 Apr 2020 01:43:24 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:18:27 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 06:18:41 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:19:30 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:706a1cdc903b54148ad6d5b672b2bafacadd79daffc0487b4949dd5d193f96f8`  
		Last Modified: Thu, 16 Apr 2020 01:49:33 GMT  
		Size: 23.1 MB (23141457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667a9abd427eb4a5747168a8400ed0e9a6f9721abdc28627ceba31ffd4a687b2`  
		Last Modified: Thu, 16 Apr 2020 06:30:13 GMT  
		Size: 244.5 KB (244471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d7350249a79bb472729379d572433d2228dd8059cab2e58477277a9e66bb36`  
		Last Modified: Thu, 16 Apr 2020 06:30:40 GMT  
		Size: 68.6 MB (68631183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:fa72fc4c116a54fd72fa979ab6db10a3798c1a0719a1b40884ceabbb476291c2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48805899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccafa8bda50e8b6b041a02bca8290435a0dac26f6b7f52a0f59d6d21222413f1`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:57 GMT
ADD file:1c7f60f778e4b93490d570487d56275925e5eb477632e71cb9f035ce6edf2460 in / 
# Thu, 16 Apr 2020 01:44:03 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:37:42 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 06:39:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:41:27 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:15e508b90ba1d327da83b72fc494ca263c1566ef6f70b91001cf2093395ffa3d`  
		Last Modified: Thu, 16 Apr 2020 02:04:33 GMT  
		Size: 22.8 MB (22785425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1629fdf02d54d31ae3023cd8b4a515c3c17a085c6135c7a10e412896d06a1f62`  
		Last Modified: Thu, 16 Apr 2020 07:18:38 GMT  
		Size: 244.7 KB (244669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc63fa4246f2b9b66f762d8c33434e375c088c1ca73c3a389a8fb2525f93c7c`  
		Last Modified: Thu, 16 Apr 2020 07:18:43 GMT  
		Size: 25.8 MB (25775805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.8-slim`

```console
$ docker pull mono@sha256:e283cd94cb3d139f1dfad8ff78c39cde4ef3f418b53745ce1194ea44adc7c694
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
$ docker pull mono@sha256:16ad829001a98d74a3d32f80f5865bdc3f6ec6bc0bbdb514069e3ff2956b8664
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.3 MB (87342068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:755f960b5885e01b06366f22620568cc1ca381b5d88f46e3904bee4016fed03e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:08 GMT
ADD file:e077f4d014ea0869fc4b3d5a3e6b3c8b792a97a8b4a328f33a994369225ff222 in / 
# Tue, 31 Mar 2020 01:24:08 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 20:53:54 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 31 Mar 2020 20:54:07 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 31 Mar 2020 20:54:46 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:48839397421a64189661c2b86a34eb515d09a28204587a2b06b59df9f6e2d786`  
		Last Modified: Tue, 31 Mar 2020 01:29:28 GMT  
		Size: 22.5 MB (22513374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978d1e7775eef6eeed6c7cc7e4c060677dd6202aac3fa0913cd117b94e0b0729`  
		Last Modified: Tue, 31 Mar 2020 21:27:17 GMT  
		Size: 244.5 KB (244470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c82f16ec565f137b31bfb7a2102b30c050898aab6b0cb3a72cff11a75ee98d`  
		Last Modified: Tue, 31 Mar 2020 21:27:30 GMT  
		Size: 64.6 MB (64584224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:988781ce7fd3739dba6c395332912434cb391801f362378ff13316fdc0c50a3b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.8 MB (46803115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8e01bfb2e90fa41fdda2d35621f00b8a0d51e600f008dd4e4518771218af14c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:54:51 GMT
ADD file:ba6c5e03457e69f59231e8e7c6465c1ec985812f0d8f7a65d9842f2be3e947fb in / 
# Thu, 16 Apr 2020 00:54:54 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 03:22:05 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 03:22:36 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 03:23:29 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b7d527e4baf13a6c926fb354fe1b38cb42b96f249ae65fdc0f52c853b654e06e`  
		Last Modified: Thu, 16 Apr 2020 01:02:32 GMT  
		Size: 21.2 MB (21190797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5251e801555d8cd1370a8d39ca953a0fb8f39729ff494b4a60bd03b4255c45be`  
		Last Modified: Thu, 16 Apr 2020 03:36:12 GMT  
		Size: 244.6 KB (244555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c9b96b75ebb7a3cac23cf75e27179b71b5aa2cee0c40c33aca6399e29516f2`  
		Last Modified: Thu, 16 Apr 2020 03:36:22 GMT  
		Size: 25.4 MB (25367763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:fec0e4861eab05dd7c3eb364beefae8f8d5fc2ef225162e038b210af4cb3d508
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44151837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b78272cf77806b892fb8ce1da5a728ff7eaee3e059bb9ed6a77bd80478f1be7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:05:08 GMT
ADD file:e37c4728c0c89ac126542ac35e7e493425c021bfac751079c9b266821a1b4e99 in / 
# Thu, 16 Apr 2020 01:05:10 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:40:35 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 04:40:56 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 04:41:45 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f78d9963dfddc4747d6200353b50f6093a6e37ca82e1612fa397d64ff13e7299`  
		Last Modified: Thu, 16 Apr 2020 01:12:33 GMT  
		Size: 19.3 MB (19298546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70114347da279136ebd21697ef769dc5764f716c6f7331568bbf7306c17da63c`  
		Last Modified: Thu, 16 Apr 2020 04:54:02 GMT  
		Size: 244.6 KB (244551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802f26edffea7b59f9cc74e47561799e0c847d999b0db0dd2d99497c42af3511`  
		Last Modified: Thu, 16 Apr 2020 04:54:10 GMT  
		Size: 24.6 MB (24608740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:d08953373b3ef1fc7db79f7f13d8698af415ccec4a187b24ccd2e20c729b8c7d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.0 MB (50034663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4c3ba9afd0517a25a4e83d0efc8b8d5d84880dbcc969fd912d6ce0463995374`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 02:45:19 GMT
ADD file:1588320d1c43714ec0353b7471f2ffd649045ca0f5f70dcb1eb064875fff9578 in / 
# Thu, 16 Apr 2020 02:45:21 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:47:03 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 06:47:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:48:05 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8978c87ff45d64d1663a585dcf1ed66d9e711c2e4048d83ef561da9514ef46e6`  
		Last Modified: Thu, 16 Apr 2020 02:51:32 GMT  
		Size: 20.4 MB (20370106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:090b996e11040b9a724d4b94b5f6fea43f5cee5558fdcdcb2e4627d1c596f82c`  
		Last Modified: Thu, 16 Apr 2020 06:59:20 GMT  
		Size: 244.4 KB (244369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be77ae0e8a98b883233d159b79364894a76d49f1b02badb9f57b227a26a8e1a`  
		Last Modified: Thu, 16 Apr 2020 06:59:30 GMT  
		Size: 29.4 MB (29420188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8-slim` - linux; 386

```console
$ docker pull mono@sha256:1bd521f164e72bfedaa4b84ff032becb6cd48254d229233d338e39d68c234afb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.0 MB (92017111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae15c2b3c37ced7865f4ee9b7312cae7e74e77a42ea630787456d7efe775ed93`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:24 GMT
ADD file:0e72ab6d3f5ce06d7170bd6b0ceeda8687d1a5e2dab40308a8b8960d67fceffe in / 
# Thu, 16 Apr 2020 01:43:24 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:18:27 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 06:18:41 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:19:30 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:706a1cdc903b54148ad6d5b672b2bafacadd79daffc0487b4949dd5d193f96f8`  
		Last Modified: Thu, 16 Apr 2020 01:49:33 GMT  
		Size: 23.1 MB (23141457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667a9abd427eb4a5747168a8400ed0e9a6f9721abdc28627ceba31ffd4a687b2`  
		Last Modified: Thu, 16 Apr 2020 06:30:13 GMT  
		Size: 244.5 KB (244471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d7350249a79bb472729379d572433d2228dd8059cab2e58477277a9e66bb36`  
		Last Modified: Thu, 16 Apr 2020 06:30:40 GMT  
		Size: 68.6 MB (68631183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:fa72fc4c116a54fd72fa979ab6db10a3798c1a0719a1b40884ceabbb476291c2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48805899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccafa8bda50e8b6b041a02bca8290435a0dac26f6b7f52a0f59d6d21222413f1`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:57 GMT
ADD file:1c7f60f778e4b93490d570487d56275925e5eb477632e71cb9f035ce6edf2460 in / 
# Thu, 16 Apr 2020 01:44:03 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:37:42 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 06:39:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:41:27 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:15e508b90ba1d327da83b72fc494ca263c1566ef6f70b91001cf2093395ffa3d`  
		Last Modified: Thu, 16 Apr 2020 02:04:33 GMT  
		Size: 22.8 MB (22785425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1629fdf02d54d31ae3023cd8b4a515c3c17a085c6135c7a10e412896d06a1f62`  
		Last Modified: Thu, 16 Apr 2020 07:18:38 GMT  
		Size: 244.7 KB (244669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc63fa4246f2b9b66f762d8c33434e375c088c1ca73c3a389a8fb2525f93c7c`  
		Last Modified: Thu, 16 Apr 2020 07:18:43 GMT  
		Size: 25.8 MB (25775805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6-slim`

```console
$ docker pull mono@sha256:e283cd94cb3d139f1dfad8ff78c39cde4ef3f418b53745ce1194ea44adc7c694
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
$ docker pull mono@sha256:16ad829001a98d74a3d32f80f5865bdc3f6ec6bc0bbdb514069e3ff2956b8664
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.3 MB (87342068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:755f960b5885e01b06366f22620568cc1ca381b5d88f46e3904bee4016fed03e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:08 GMT
ADD file:e077f4d014ea0869fc4b3d5a3e6b3c8b792a97a8b4a328f33a994369225ff222 in / 
# Tue, 31 Mar 2020 01:24:08 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 20:53:54 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 31 Mar 2020 20:54:07 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 31 Mar 2020 20:54:46 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:48839397421a64189661c2b86a34eb515d09a28204587a2b06b59df9f6e2d786`  
		Last Modified: Tue, 31 Mar 2020 01:29:28 GMT  
		Size: 22.5 MB (22513374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978d1e7775eef6eeed6c7cc7e4c060677dd6202aac3fa0913cd117b94e0b0729`  
		Last Modified: Tue, 31 Mar 2020 21:27:17 GMT  
		Size: 244.5 KB (244470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c82f16ec565f137b31bfb7a2102b30c050898aab6b0cb3a72cff11a75ee98d`  
		Last Modified: Tue, 31 Mar 2020 21:27:30 GMT  
		Size: 64.6 MB (64584224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:988781ce7fd3739dba6c395332912434cb391801f362378ff13316fdc0c50a3b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.8 MB (46803115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8e01bfb2e90fa41fdda2d35621f00b8a0d51e600f008dd4e4518771218af14c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:54:51 GMT
ADD file:ba6c5e03457e69f59231e8e7c6465c1ec985812f0d8f7a65d9842f2be3e947fb in / 
# Thu, 16 Apr 2020 00:54:54 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 03:22:05 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 03:22:36 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 03:23:29 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b7d527e4baf13a6c926fb354fe1b38cb42b96f249ae65fdc0f52c853b654e06e`  
		Last Modified: Thu, 16 Apr 2020 01:02:32 GMT  
		Size: 21.2 MB (21190797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5251e801555d8cd1370a8d39ca953a0fb8f39729ff494b4a60bd03b4255c45be`  
		Last Modified: Thu, 16 Apr 2020 03:36:12 GMT  
		Size: 244.6 KB (244555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c9b96b75ebb7a3cac23cf75e27179b71b5aa2cee0c40c33aca6399e29516f2`  
		Last Modified: Thu, 16 Apr 2020 03:36:22 GMT  
		Size: 25.4 MB (25367763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:fec0e4861eab05dd7c3eb364beefae8f8d5fc2ef225162e038b210af4cb3d508
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44151837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b78272cf77806b892fb8ce1da5a728ff7eaee3e059bb9ed6a77bd80478f1be7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:05:08 GMT
ADD file:e37c4728c0c89ac126542ac35e7e493425c021bfac751079c9b266821a1b4e99 in / 
# Thu, 16 Apr 2020 01:05:10 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:40:35 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 04:40:56 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 04:41:45 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f78d9963dfddc4747d6200353b50f6093a6e37ca82e1612fa397d64ff13e7299`  
		Last Modified: Thu, 16 Apr 2020 01:12:33 GMT  
		Size: 19.3 MB (19298546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70114347da279136ebd21697ef769dc5764f716c6f7331568bbf7306c17da63c`  
		Last Modified: Thu, 16 Apr 2020 04:54:02 GMT  
		Size: 244.6 KB (244551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802f26edffea7b59f9cc74e47561799e0c847d999b0db0dd2d99497c42af3511`  
		Last Modified: Thu, 16 Apr 2020 04:54:10 GMT  
		Size: 24.6 MB (24608740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:d08953373b3ef1fc7db79f7f13d8698af415ccec4a187b24ccd2e20c729b8c7d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.0 MB (50034663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4c3ba9afd0517a25a4e83d0efc8b8d5d84880dbcc969fd912d6ce0463995374`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 02:45:19 GMT
ADD file:1588320d1c43714ec0353b7471f2ffd649045ca0f5f70dcb1eb064875fff9578 in / 
# Thu, 16 Apr 2020 02:45:21 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:47:03 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 06:47:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:48:05 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8978c87ff45d64d1663a585dcf1ed66d9e711c2e4048d83ef561da9514ef46e6`  
		Last Modified: Thu, 16 Apr 2020 02:51:32 GMT  
		Size: 20.4 MB (20370106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:090b996e11040b9a724d4b94b5f6fea43f5cee5558fdcdcb2e4627d1c596f82c`  
		Last Modified: Thu, 16 Apr 2020 06:59:20 GMT  
		Size: 244.4 KB (244369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be77ae0e8a98b883233d159b79364894a76d49f1b02badb9f57b227a26a8e1a`  
		Last Modified: Thu, 16 Apr 2020 06:59:30 GMT  
		Size: 29.4 MB (29420188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; 386

```console
$ docker pull mono@sha256:1bd521f164e72bfedaa4b84ff032becb6cd48254d229233d338e39d68c234afb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.0 MB (92017111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae15c2b3c37ced7865f4ee9b7312cae7e74e77a42ea630787456d7efe775ed93`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:24 GMT
ADD file:0e72ab6d3f5ce06d7170bd6b0ceeda8687d1a5e2dab40308a8b8960d67fceffe in / 
# Thu, 16 Apr 2020 01:43:24 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:18:27 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 06:18:41 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:19:30 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:706a1cdc903b54148ad6d5b672b2bafacadd79daffc0487b4949dd5d193f96f8`  
		Last Modified: Thu, 16 Apr 2020 01:49:33 GMT  
		Size: 23.1 MB (23141457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667a9abd427eb4a5747168a8400ed0e9a6f9721abdc28627ceba31ffd4a687b2`  
		Last Modified: Thu, 16 Apr 2020 06:30:13 GMT  
		Size: 244.5 KB (244471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d7350249a79bb472729379d572433d2228dd8059cab2e58477277a9e66bb36`  
		Last Modified: Thu, 16 Apr 2020 06:30:40 GMT  
		Size: 68.6 MB (68631183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:fa72fc4c116a54fd72fa979ab6db10a3798c1a0719a1b40884ceabbb476291c2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48805899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccafa8bda50e8b6b041a02bca8290435a0dac26f6b7f52a0f59d6d21222413f1`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:57 GMT
ADD file:1c7f60f778e4b93490d570487d56275925e5eb477632e71cb9f035ce6edf2460 in / 
# Thu, 16 Apr 2020 01:44:03 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:37:42 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 06:39:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:41:27 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:15e508b90ba1d327da83b72fc494ca263c1566ef6f70b91001cf2093395ffa3d`  
		Last Modified: Thu, 16 Apr 2020 02:04:33 GMT  
		Size: 22.8 MB (22785425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1629fdf02d54d31ae3023cd8b4a515c3c17a085c6135c7a10e412896d06a1f62`  
		Last Modified: Thu, 16 Apr 2020 07:18:38 GMT  
		Size: 244.7 KB (244669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc63fa4246f2b9b66f762d8c33434e375c088c1ca73c3a389a8fb2525f93c7c`  
		Last Modified: Thu, 16 Apr 2020 07:18:43 GMT  
		Size: 25.8 MB (25775805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:latest`

```console
$ docker pull mono@sha256:b976fe5178f784ec89e63e12804e24408dde1be2a42b8715369350614b60f420
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
$ docker pull mono@sha256:81582109869f82484faaff740559cf18e92c7dbb6776d949ffd1584ed2052d07
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.1 MB (235136288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6258db5099bae58f82a4b00866b799387bf6f845a18647cbc4eff62573a03750`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:08 GMT
ADD file:e077f4d014ea0869fc4b3d5a3e6b3c8b792a97a8b4a328f33a994369225ff222 in / 
# Tue, 31 Mar 2020 01:24:08 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 20:53:54 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 31 Mar 2020 20:54:07 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 31 Mar 2020 20:54:46 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 31 Mar 2020 21:07:25 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:48839397421a64189661c2b86a34eb515d09a28204587a2b06b59df9f6e2d786`  
		Last Modified: Tue, 31 Mar 2020 01:29:28 GMT  
		Size: 22.5 MB (22513374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978d1e7775eef6eeed6c7cc7e4c060677dd6202aac3fa0913cd117b94e0b0729`  
		Last Modified: Tue, 31 Mar 2020 21:27:17 GMT  
		Size: 244.5 KB (244470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c82f16ec565f137b31bfb7a2102b30c050898aab6b0cb3a72cff11a75ee98d`  
		Last Modified: Tue, 31 Mar 2020 21:27:30 GMT  
		Size: 64.6 MB (64584224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b58815a2352a01b3b0ed3200dca917e29fd58f3690ff55bbf5b7456d7cdd10`  
		Last Modified: Tue, 31 Mar 2020 21:28:57 GMT  
		Size: 147.8 MB (147794220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm variant v5

```console
$ docker pull mono@sha256:039a6be7bba94963928fb63f0cd7624bdcc24ff437d3511659983bf8a15da61c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.7 MB (176695282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbb0da5905f2877688de5793cf7d5f0c6b5cdbb737868e678439fec995215cfa`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:54:51 GMT
ADD file:ba6c5e03457e69f59231e8e7c6465c1ec985812f0d8f7a65d9842f2be3e947fb in / 
# Thu, 16 Apr 2020 00:54:54 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 03:22:05 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 03:22:36 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 03:23:29 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 03:29:10 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b7d527e4baf13a6c926fb354fe1b38cb42b96f249ae65fdc0f52c853b654e06e`  
		Last Modified: Thu, 16 Apr 2020 01:02:32 GMT  
		Size: 21.2 MB (21190797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5251e801555d8cd1370a8d39ca953a0fb8f39729ff494b4a60bd03b4255c45be`  
		Last Modified: Thu, 16 Apr 2020 03:36:12 GMT  
		Size: 244.6 KB (244555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c9b96b75ebb7a3cac23cf75e27179b71b5aa2cee0c40c33aca6399e29516f2`  
		Last Modified: Thu, 16 Apr 2020 03:36:22 GMT  
		Size: 25.4 MB (25367763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33b43ad8da6addb8c852a68a9848cba5f48be98873fc8db208731eb55f31b9b`  
		Last Modified: Thu, 16 Apr 2020 03:37:53 GMT  
		Size: 129.9 MB (129892167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm variant v7

```console
$ docker pull mono@sha256:09076495aacfba71beb6f4e5812d597a2d059b58d0d1a053068e4fa0fdec8443
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.7 MB (172708239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6e489c47305d9f8c107b00d2a1e335c874014e8fa4a3fc5ecb9082df7c5be0f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:05:08 GMT
ADD file:e37c4728c0c89ac126542ac35e7e493425c021bfac751079c9b266821a1b4e99 in / 
# Thu, 16 Apr 2020 01:05:10 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:40:35 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 04:40:56 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 04:41:45 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 04:47:13 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f78d9963dfddc4747d6200353b50f6093a6e37ca82e1612fa397d64ff13e7299`  
		Last Modified: Thu, 16 Apr 2020 01:12:33 GMT  
		Size: 19.3 MB (19298546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70114347da279136ebd21697ef769dc5764f716c6f7331568bbf7306c17da63c`  
		Last Modified: Thu, 16 Apr 2020 04:54:02 GMT  
		Size: 244.6 KB (244551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802f26edffea7b59f9cc74e47561799e0c847d999b0db0dd2d99497c42af3511`  
		Last Modified: Thu, 16 Apr 2020 04:54:10 GMT  
		Size: 24.6 MB (24608740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a9fd3d7648204f077b0034260c1887fe3c12c26ffadbb4223d8dc7ff65c1eb`  
		Last Modified: Thu, 16 Apr 2020 04:55:42 GMT  
		Size: 128.6 MB (128556402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:abe9ae9da3ff9d1c710471ec6a5c1b39b18e33e11b0abba7d4245a3e75b11dc0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.7 MB (194747450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5a96031ff7018d8a3f1e18642728c41f24ad314d26c4fc40907ef19fce71fcd`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 02:45:19 GMT
ADD file:1588320d1c43714ec0353b7471f2ffd649045ca0f5f70dcb1eb064875fff9578 in / 
# Thu, 16 Apr 2020 02:45:21 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:47:03 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 06:47:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:48:05 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 06:53:15 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8978c87ff45d64d1663a585dcf1ed66d9e711c2e4048d83ef561da9514ef46e6`  
		Last Modified: Thu, 16 Apr 2020 02:51:32 GMT  
		Size: 20.4 MB (20370106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:090b996e11040b9a724d4b94b5f6fea43f5cee5558fdcdcb2e4627d1c596f82c`  
		Last Modified: Thu, 16 Apr 2020 06:59:20 GMT  
		Size: 244.4 KB (244369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be77ae0e8a98b883233d159b79364894a76d49f1b02badb9f57b227a26a8e1a`  
		Last Modified: Thu, 16 Apr 2020 06:59:30 GMT  
		Size: 29.4 MB (29420188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1774c3e17e0d83d02e086998900775da6efe1356459c585e7d5800434b5aaf21`  
		Last Modified: Thu, 16 Apr 2020 07:01:03 GMT  
		Size: 144.7 MB (144712787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; 386

```console
$ docker pull mono@sha256:1ebc75a12b856eab7355f64cd759c76ed529107995cb75f9e829cf2849cc0080
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.5 MB (243510596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04327a60fe104894839dc0076d6d5fb91bfada9228944cc9208c5855a57cea38`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:24 GMT
ADD file:0e72ab6d3f5ce06d7170bd6b0ceeda8687d1a5e2dab40308a8b8960d67fceffe in / 
# Thu, 16 Apr 2020 01:43:24 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:18:27 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 06:18:41 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:19:30 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 06:24:27 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:706a1cdc903b54148ad6d5b672b2bafacadd79daffc0487b4949dd5d193f96f8`  
		Last Modified: Thu, 16 Apr 2020 01:49:33 GMT  
		Size: 23.1 MB (23141457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667a9abd427eb4a5747168a8400ed0e9a6f9721abdc28627ceba31ffd4a687b2`  
		Last Modified: Thu, 16 Apr 2020 06:30:13 GMT  
		Size: 244.5 KB (244471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d7350249a79bb472729379d572433d2228dd8059cab2e58477277a9e66bb36`  
		Last Modified: Thu, 16 Apr 2020 06:30:40 GMT  
		Size: 68.6 MB (68631183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cf9820146ece539d30304f98e198b7bd9e334cae43f76008522272d551c88e`  
		Last Modified: Thu, 16 Apr 2020 06:32:59 GMT  
		Size: 151.5 MB (151493485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; ppc64le

```console
$ docker pull mono@sha256:0434d01a8617e75170a4dd8a638d786d1e67ac13c9fc880e023ccd0950428e36
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.0 MB (178997743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b5e14702ff1aff3bacfb8485b742086b08ff9d01cadd82d9f8327e6ac887fcc`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:57 GMT
ADD file:1c7f60f778e4b93490d570487d56275925e5eb477632e71cb9f035ce6edf2460 in / 
# Thu, 16 Apr 2020 01:44:03 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:37:42 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 06:39:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:41:27 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 16 Apr 2020 06:58:08 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:15e508b90ba1d327da83b72fc494ca263c1566ef6f70b91001cf2093395ffa3d`  
		Last Modified: Thu, 16 Apr 2020 02:04:33 GMT  
		Size: 22.8 MB (22785425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1629fdf02d54d31ae3023cd8b4a515c3c17a085c6135c7a10e412896d06a1f62`  
		Last Modified: Thu, 16 Apr 2020 07:18:38 GMT  
		Size: 244.7 KB (244669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc63fa4246f2b9b66f762d8c33434e375c088c1ca73c3a389a8fb2525f93c7c`  
		Last Modified: Thu, 16 Apr 2020 07:18:43 GMT  
		Size: 25.8 MB (25775805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ed038a48cf0007c67072a64fc2d4d1d4efd20b275bff6a15884fcfe67b0afa`  
		Last Modified: Thu, 16 Apr 2020 07:20:07 GMT  
		Size: 130.2 MB (130191844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:slim`

```console
$ docker pull mono@sha256:e283cd94cb3d139f1dfad8ff78c39cde4ef3f418b53745ce1194ea44adc7c694
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
$ docker pull mono@sha256:16ad829001a98d74a3d32f80f5865bdc3f6ec6bc0bbdb514069e3ff2956b8664
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.3 MB (87342068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:755f960b5885e01b06366f22620568cc1ca381b5d88f46e3904bee4016fed03e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:08 GMT
ADD file:e077f4d014ea0869fc4b3d5a3e6b3c8b792a97a8b4a328f33a994369225ff222 in / 
# Tue, 31 Mar 2020 01:24:08 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 20:53:54 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 31 Mar 2020 20:54:07 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 31 Mar 2020 20:54:46 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:48839397421a64189661c2b86a34eb515d09a28204587a2b06b59df9f6e2d786`  
		Last Modified: Tue, 31 Mar 2020 01:29:28 GMT  
		Size: 22.5 MB (22513374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978d1e7775eef6eeed6c7cc7e4c060677dd6202aac3fa0913cd117b94e0b0729`  
		Last Modified: Tue, 31 Mar 2020 21:27:17 GMT  
		Size: 244.5 KB (244470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c82f16ec565f137b31bfb7a2102b30c050898aab6b0cb3a72cff11a75ee98d`  
		Last Modified: Tue, 31 Mar 2020 21:27:30 GMT  
		Size: 64.6 MB (64584224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:988781ce7fd3739dba6c395332912434cb391801f362378ff13316fdc0c50a3b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.8 MB (46803115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8e01bfb2e90fa41fdda2d35621f00b8a0d51e600f008dd4e4518771218af14c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:54:51 GMT
ADD file:ba6c5e03457e69f59231e8e7c6465c1ec985812f0d8f7a65d9842f2be3e947fb in / 
# Thu, 16 Apr 2020 00:54:54 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 03:22:05 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 03:22:36 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 03:23:29 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b7d527e4baf13a6c926fb354fe1b38cb42b96f249ae65fdc0f52c853b654e06e`  
		Last Modified: Thu, 16 Apr 2020 01:02:32 GMT  
		Size: 21.2 MB (21190797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5251e801555d8cd1370a8d39ca953a0fb8f39729ff494b4a60bd03b4255c45be`  
		Last Modified: Thu, 16 Apr 2020 03:36:12 GMT  
		Size: 244.6 KB (244555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c9b96b75ebb7a3cac23cf75e27179b71b5aa2cee0c40c33aca6399e29516f2`  
		Last Modified: Thu, 16 Apr 2020 03:36:22 GMT  
		Size: 25.4 MB (25367763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:fec0e4861eab05dd7c3eb364beefae8f8d5fc2ef225162e038b210af4cb3d508
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44151837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b78272cf77806b892fb8ce1da5a728ff7eaee3e059bb9ed6a77bd80478f1be7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:05:08 GMT
ADD file:e37c4728c0c89ac126542ac35e7e493425c021bfac751079c9b266821a1b4e99 in / 
# Thu, 16 Apr 2020 01:05:10 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:40:35 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 04:40:56 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 04:41:45 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f78d9963dfddc4747d6200353b50f6093a6e37ca82e1612fa397d64ff13e7299`  
		Last Modified: Thu, 16 Apr 2020 01:12:33 GMT  
		Size: 19.3 MB (19298546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70114347da279136ebd21697ef769dc5764f716c6f7331568bbf7306c17da63c`  
		Last Modified: Thu, 16 Apr 2020 04:54:02 GMT  
		Size: 244.6 KB (244551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802f26edffea7b59f9cc74e47561799e0c847d999b0db0dd2d99497c42af3511`  
		Last Modified: Thu, 16 Apr 2020 04:54:10 GMT  
		Size: 24.6 MB (24608740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:d08953373b3ef1fc7db79f7f13d8698af415ccec4a187b24ccd2e20c729b8c7d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.0 MB (50034663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4c3ba9afd0517a25a4e83d0efc8b8d5d84880dbcc969fd912d6ce0463995374`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 02:45:19 GMT
ADD file:1588320d1c43714ec0353b7471f2ffd649045ca0f5f70dcb1eb064875fff9578 in / 
# Thu, 16 Apr 2020 02:45:21 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:47:03 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 06:47:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:48:05 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8978c87ff45d64d1663a585dcf1ed66d9e711c2e4048d83ef561da9514ef46e6`  
		Last Modified: Thu, 16 Apr 2020 02:51:32 GMT  
		Size: 20.4 MB (20370106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:090b996e11040b9a724d4b94b5f6fea43f5cee5558fdcdcb2e4627d1c596f82c`  
		Last Modified: Thu, 16 Apr 2020 06:59:20 GMT  
		Size: 244.4 KB (244369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be77ae0e8a98b883233d159b79364894a76d49f1b02badb9f57b227a26a8e1a`  
		Last Modified: Thu, 16 Apr 2020 06:59:30 GMT  
		Size: 29.4 MB (29420188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; 386

```console
$ docker pull mono@sha256:1bd521f164e72bfedaa4b84ff032becb6cd48254d229233d338e39d68c234afb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.0 MB (92017111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae15c2b3c37ced7865f4ee9b7312cae7e74e77a42ea630787456d7efe775ed93`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:24 GMT
ADD file:0e72ab6d3f5ce06d7170bd6b0ceeda8687d1a5e2dab40308a8b8960d67fceffe in / 
# Thu, 16 Apr 2020 01:43:24 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:18:27 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 06:18:41 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:19:30 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:706a1cdc903b54148ad6d5b672b2bafacadd79daffc0487b4949dd5d193f96f8`  
		Last Modified: Thu, 16 Apr 2020 01:49:33 GMT  
		Size: 23.1 MB (23141457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667a9abd427eb4a5747168a8400ed0e9a6f9721abdc28627ceba31ffd4a687b2`  
		Last Modified: Thu, 16 Apr 2020 06:30:13 GMT  
		Size: 244.5 KB (244471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d7350249a79bb472729379d572433d2228dd8059cab2e58477277a9e66bb36`  
		Last Modified: Thu, 16 Apr 2020 06:30:40 GMT  
		Size: 68.6 MB (68631183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; ppc64le

```console
$ docker pull mono@sha256:fa72fc4c116a54fd72fa979ab6db10a3798c1a0719a1b40884ceabbb476291c2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48805899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccafa8bda50e8b6b041a02bca8290435a0dac26f6b7f52a0f59d6d21222413f1`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:57 GMT
ADD file:1c7f60f778e4b93490d570487d56275925e5eb477632e71cb9f035ce6edf2460 in / 
# Thu, 16 Apr 2020 01:44:03 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:37:42 GMT
ENV MONO_VERSION=6.8.0.96
# Thu, 16 Apr 2020 06:39:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 16 Apr 2020 06:41:27 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:15e508b90ba1d327da83b72fc494ca263c1566ef6f70b91001cf2093395ffa3d`  
		Last Modified: Thu, 16 Apr 2020 02:04:33 GMT  
		Size: 22.8 MB (22785425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1629fdf02d54d31ae3023cd8b4a515c3c17a085c6135c7a10e412896d06a1f62`  
		Last Modified: Thu, 16 Apr 2020 07:18:38 GMT  
		Size: 244.7 KB (244669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc63fa4246f2b9b66f762d8c33434e375c088c1ca73c3a389a8fb2525f93c7c`  
		Last Modified: Thu, 16 Apr 2020 07:18:43 GMT  
		Size: 25.8 MB (25775805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
