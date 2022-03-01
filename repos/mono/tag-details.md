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
$ docker pull mono@sha256:0fb67a9a37f9399572c9446f92acf97f8e242b665f60f51805498cab2b17fc84
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
$ docker pull mono@sha256:6b7a7e5a048189d49dcb401794583cc3d7994ddbace52c916b229f9e68545f2e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.1 MB (236118449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:088d59542ba84be22020630040214ac5714f5455ed7dfa5f99cf2c05a964590b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:42:22 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 26 Jan 2022 08:42:47 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 08:43:11 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 26 Jan 2022 08:49:07 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd7c8aa8024e5da067c560f0319ca71064f55299dcc8b8d0cdf0c26dc826d09`  
		Last Modified: Wed, 26 Jan 2022 08:55:23 GMT  
		Size: 2.8 MB (2767042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d82173799248cedffd37d5bdd1f07b1c51a1b625b2e7a880a43d222f116d07`  
		Last Modified: Wed, 26 Jan 2022 08:55:34 GMT  
		Size: 64.8 MB (64759888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7823e38b4160826b37443754a040cea87df23809a9681e8be62028744db322ed`  
		Last Modified: Wed, 26 Jan 2022 08:56:37 GMT  
		Size: 141.4 MB (141437788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; arm variant v5

```console
$ docker pull mono@sha256:cff835ec8c22098c42940eeb3618fed0b00c836fe1157eda320f0d000bf4a0e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.9 MB (191929783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c8d899777bbcafd23a69b4effe3d6c1ce8c82f871ff44333774ad8e1360e804`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:03:56 GMT
ADD file:f5674cd595d2eb9d698a67c0669348b7dca3158b3c949498321a875d56d1db0e in / 
# Tue, 01 Mar 2022 02:03:57 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:55:41 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 01 Mar 2022 03:56:20 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 01 Mar 2022 03:57:06 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 01 Mar 2022 04:02:10 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d93143e6711bdadb9413c811c28fed68303bd0eafd6640f6552d2147730818af`  
		Last Modified: Tue, 01 Mar 2022 02:20:01 GMT  
		Size: 24.9 MB (24886227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0217ce2cacf32a6058fe38fb20cfe9a6d980cf80cca400013545f361b1b3fd`  
		Last Modified: Tue, 01 Mar 2022 04:07:02 GMT  
		Size: 2.5 MB (2462533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68de90092907e27be985b209e7586a431f836320c0bb1b413435a590965fc290`  
		Last Modified: Tue, 01 Mar 2022 04:07:19 GMT  
		Size: 24.5 MB (24493246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b35ea8d607897d4a5fc65b78859a5f93a1d200489340e252ec304024542a0da`  
		Last Modified: Tue, 01 Mar 2022 04:09:54 GMT  
		Size: 140.1 MB (140087777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; arm variant v7

```console
$ docker pull mono@sha256:a0f15b2324df9644625fd899bc9491ba399197f1554bea1fa931b12eb1dd1e74
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.8 MB (187845702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dcbf347de76bd0a6f0723618d9de9548b3d0e9b6af63961becd5a5d1ff74837`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:43:12 GMT
ADD file:ca8132e20773f7037458cc53fe20a7116f93c21c7479be5a2a1d739495dbe44e in / 
# Wed, 26 Jan 2022 01:43:13 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 03:02:36 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 26 Jan 2022 03:03:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 03:04:03 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 26 Jan 2022 03:09:10 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:20cc49690d9072283406c1c11e9b1dc1a247782cc8daa526b375d4a7f1cb6a94`  
		Last Modified: Wed, 26 Jan 2022 01:59:27 GMT  
		Size: 22.8 MB (22754397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242f21c9f2ea2b8610338b20aa4a933d07978910d00d961eb9395cf5ad6a14ba`  
		Last Modified: Wed, 26 Jan 2022 03:14:04 GMT  
		Size: 2.4 MB (2361950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf05b1bf44b0bc6e31c02c1f89b71c97d2120bd5088a235a9a2a58ccdc973e4`  
		Last Modified: Wed, 26 Jan 2022 03:14:20 GMT  
		Size: 23.8 MB (23782786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd4b90a8da9c282d5bd778e5a73064eeef59ebcf39aeacd8d471e25e4ee8e9b`  
		Last Modified: Wed, 26 Jan 2022 03:16:54 GMT  
		Size: 138.9 MB (138946569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:6099f20ed14b5d90f2c433f1b5be4fdb75ecb73e555e27d832226aa745ab9a99
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.5 MB (214451499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34db74ee86a7e6e6ce7640619a498ddf102f6457b05048d89e5cacb3d02e8f57`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:56 GMT
ADD file:796bc43a948899ba53bddebf7f613769fe96e8ea3a27eb7143d079c7a166ab01 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 04:54:45 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 26 Jan 2022 04:55:28 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 04:55:43 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 26 Jan 2022 04:57:25 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4c7c9f6f1115fd4f35807a2f6c1375759365a991748aee0111873e55255f150b`  
		Last Modified: Wed, 26 Jan 2022 01:49:55 GMT  
		Size: 25.9 MB (25923216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145db9a792c54fdb1a14e3673d8bf7e6bfbdcfcd16e9f20670088dc797a755f9`  
		Last Modified: Wed, 26 Jan 2022 04:59:19 GMT  
		Size: 2.6 MB (2634624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba55b80938abbcaf307229652d0245d64085b55a6aa9db6572f5ac715e9d3959`  
		Last Modified: Wed, 26 Jan 2022 04:59:26 GMT  
		Size: 29.3 MB (29318190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4d2da081a628a5666b5ec038b6bdadd12c4a83da6c999e6b2c9cf213c84874`  
		Last Modified: Wed, 26 Jan 2022 05:00:30 GMT  
		Size: 156.6 MB (156575469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; 386

```console
$ docker pull mono@sha256:82a3f21fd720a3de8dd1e2ac27a9ba549947ca8fc1fefb8cae9a4680183cf19e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.9 MB (241920861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:629648c952e20ac82023401475080241331753ddc53cd6ec14a439a426731e84`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:08:04 GMT
ADD file:d9d384f0402bc696e46e7529f52d64859a66aa7a60bca9c7beee7433a5f7af6e in / 
# Tue, 01 Mar 2022 02:08:04 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:13:49 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 01 Mar 2022 10:14:37 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 01 Mar 2022 10:15:09 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 01 Mar 2022 10:18:40 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c761ce6f2bf0aed07e1198c6f827444969d6e76dda0e55dbb45900920e551d27`  
		Last Modified: Tue, 01 Mar 2022 02:16:51 GMT  
		Size: 27.8 MB (27804590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011b9d654300beab54b280fd3e0b1f7170919be5028f5e31a210af8a83500cfc`  
		Last Modified: Tue, 01 Mar 2022 10:22:39 GMT  
		Size: 2.8 MB (2781491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4b91a20a9ead3771e864dc94eb15af13cf873e35ca6bbc27fe1fdd66f0422f`  
		Last Modified: Tue, 01 Mar 2022 10:23:02 GMT  
		Size: 68.8 MB (68778600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500a4fcb909ee1b095dc7db9d0546dcd766236538aa5715dc6dc627ab73b5df6`  
		Last Modified: Tue, 01 Mar 2022 10:25:00 GMT  
		Size: 142.6 MB (142556180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; ppc64le

```console
$ docker pull mono@sha256:56250e313f76e60e694eec7ba9ff5ca5179b9ca48a2c2e412195364e66aa79b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.6 MB (203588810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05b37ef992318378fe939868450034dde3384ac8ea697fb3550081a98836d2f1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:47:48 GMT
ADD file:d87bdffbd9392364fecbbd4148c710bc4948073e773a47c7b9ac1440ebb81c1e in / 
# Wed, 26 Jan 2022 01:47:52 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 05:16:29 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 26 Jan 2022 05:17:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 05:19:13 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 26 Jan 2022 05:28:25 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:249357001395b3de58d51723447880f3205d37ea7b902930b5c19f475d4ac8f9`  
		Last Modified: Wed, 26 Jan 2022 01:58:50 GMT  
		Size: 30.6 MB (30562293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b424ab5d806f162b76c369311f6e539940178ab8b306c053879a77ff4a77d4`  
		Last Modified: Wed, 26 Jan 2022 05:36:07 GMT  
		Size: 2.9 MB (2884629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7982f75341da8b4f46a0677a86d66dfaa5a4b464e669fc85629e0bf531fa21`  
		Last Modified: Wed, 26 Jan 2022 05:36:13 GMT  
		Size: 26.9 MB (26874043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210fd04001c965c8d905729a394f394aa15b2fa6eba24a1d6f8b31ee1a5457f0`  
		Last Modified: Wed, 26 Jan 2022 05:37:22 GMT  
		Size: 143.3 MB (143267845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6-slim`

```console
$ docker pull mono@sha256:64905a436cf3e3de5b6f7f987510b79c99887049d9017f6fe39c8b7dbe3a2952
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
$ docker pull mono@sha256:ed5b708feef72f630c6308b60ceed7cb68bb7b7c387578bfbde1053beaabce61
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94680661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a18e38b2a9d6d4f318e22f13aefc58314f800630814e3f42179f97f985e865e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:42:22 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 26 Jan 2022 08:42:47 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 08:43:11 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd7c8aa8024e5da067c560f0319ca71064f55299dcc8b8d0cdf0c26dc826d09`  
		Last Modified: Wed, 26 Jan 2022 08:55:23 GMT  
		Size: 2.8 MB (2767042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d82173799248cedffd37d5bdd1f07b1c51a1b625b2e7a880a43d222f116d07`  
		Last Modified: Wed, 26 Jan 2022 08:55:34 GMT  
		Size: 64.8 MB (64759888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:9ebb92f30258b4a717d77f185bc834d5f02ec3aab3634d67488b930d268acf7b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51842006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bd52c60156350534c857630fa5165139d0297938596bd00c52e61afaf7b7779`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:03:56 GMT
ADD file:f5674cd595d2eb9d698a67c0669348b7dca3158b3c949498321a875d56d1db0e in / 
# Tue, 01 Mar 2022 02:03:57 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:55:41 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 01 Mar 2022 03:56:20 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 01 Mar 2022 03:57:06 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d93143e6711bdadb9413c811c28fed68303bd0eafd6640f6552d2147730818af`  
		Last Modified: Tue, 01 Mar 2022 02:20:01 GMT  
		Size: 24.9 MB (24886227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0217ce2cacf32a6058fe38fb20cfe9a6d980cf80cca400013545f361b1b3fd`  
		Last Modified: Tue, 01 Mar 2022 04:07:02 GMT  
		Size: 2.5 MB (2462533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68de90092907e27be985b209e7586a431f836320c0bb1b413435a590965fc290`  
		Last Modified: Tue, 01 Mar 2022 04:07:19 GMT  
		Size: 24.5 MB (24493246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:deeb347482762f58ad102823f33d7538fa92175c60c0b63faaeee9a648fb10c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48899133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72cf0e6b2305941d40d03f813edfbd2a1b015b02e86552bc90cfe2a050b14bd7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:43:12 GMT
ADD file:ca8132e20773f7037458cc53fe20a7116f93c21c7479be5a2a1d739495dbe44e in / 
# Wed, 26 Jan 2022 01:43:13 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 03:02:36 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 26 Jan 2022 03:03:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 03:04:03 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:20cc49690d9072283406c1c11e9b1dc1a247782cc8daa526b375d4a7f1cb6a94`  
		Last Modified: Wed, 26 Jan 2022 01:59:27 GMT  
		Size: 22.8 MB (22754397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242f21c9f2ea2b8610338b20aa4a933d07978910d00d961eb9395cf5ad6a14ba`  
		Last Modified: Wed, 26 Jan 2022 03:14:04 GMT  
		Size: 2.4 MB (2361950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf05b1bf44b0bc6e31c02c1f89b71c97d2120bd5088a235a9a2a58ccdc973e4`  
		Last Modified: Wed, 26 Jan 2022 03:14:20 GMT  
		Size: 23.8 MB (23782786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:2d8b961112b0f7f9c0cb6a334ffd574c95162bc7fa8d5b2aa366004f11c42d1e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57876030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:670158c5d1ee00bcf609d8daf07279a4093cc98203ef3362fc17510761426523`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:56 GMT
ADD file:796bc43a948899ba53bddebf7f613769fe96e8ea3a27eb7143d079c7a166ab01 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 04:54:45 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 26 Jan 2022 04:55:28 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 04:55:43 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4c7c9f6f1115fd4f35807a2f6c1375759365a991748aee0111873e55255f150b`  
		Last Modified: Wed, 26 Jan 2022 01:49:55 GMT  
		Size: 25.9 MB (25923216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145db9a792c54fdb1a14e3673d8bf7e6bfbdcfcd16e9f20670088dc797a755f9`  
		Last Modified: Wed, 26 Jan 2022 04:59:19 GMT  
		Size: 2.6 MB (2634624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba55b80938abbcaf307229652d0245d64085b55a6aa9db6572f5ac715e9d3959`  
		Last Modified: Wed, 26 Jan 2022 04:59:26 GMT  
		Size: 29.3 MB (29318190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; 386

```console
$ docker pull mono@sha256:d9c23198eec7e2c304b84f004811aa4baba762614a35374bd820ff5d24e3c378
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99364681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18db94f8442093daf5003e5853ae0b168af2ec80a3ed2a7babfbbd1dc3627d99`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:08:04 GMT
ADD file:d9d384f0402bc696e46e7529f52d64859a66aa7a60bca9c7beee7433a5f7af6e in / 
# Tue, 01 Mar 2022 02:08:04 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:13:49 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 01 Mar 2022 10:14:37 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 01 Mar 2022 10:15:09 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c761ce6f2bf0aed07e1198c6f827444969d6e76dda0e55dbb45900920e551d27`  
		Last Modified: Tue, 01 Mar 2022 02:16:51 GMT  
		Size: 27.8 MB (27804590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011b9d654300beab54b280fd3e0b1f7170919be5028f5e31a210af8a83500cfc`  
		Last Modified: Tue, 01 Mar 2022 10:22:39 GMT  
		Size: 2.8 MB (2781491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4b91a20a9ead3771e864dc94eb15af13cf873e35ca6bbc27fe1fdd66f0422f`  
		Last Modified: Tue, 01 Mar 2022 10:23:02 GMT  
		Size: 68.8 MB (68778600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:d575747ba8940111c62f95739e8a754b9b87078977fba75f2e18524deb22a8a2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.3 MB (60320965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e081680305b9949003bab588e040386a8353300452f2a819aae1a529471cea28`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:47:48 GMT
ADD file:d87bdffbd9392364fecbbd4148c710bc4948073e773a47c7b9ac1440ebb81c1e in / 
# Wed, 26 Jan 2022 01:47:52 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 05:16:29 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 26 Jan 2022 05:17:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 05:19:13 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:249357001395b3de58d51723447880f3205d37ea7b902930b5c19f475d4ac8f9`  
		Last Modified: Wed, 26 Jan 2022 01:58:50 GMT  
		Size: 30.6 MB (30562293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b424ab5d806f162b76c369311f6e539940178ab8b306c053879a77ff4a77d4`  
		Last Modified: Wed, 26 Jan 2022 05:36:07 GMT  
		Size: 2.9 MB (2884629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7982f75341da8b4f46a0677a86d66dfaa5a4b464e669fc85629e0bf531fa21`  
		Last Modified: Wed, 26 Jan 2022 05:36:13 GMT  
		Size: 26.9 MB (26874043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10`

```console
$ docker pull mono@sha256:8db42556dc1e3afbdeb3b61de12c33922aa4b21bf4ed2f3c6afb639d8b5dde14
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
$ docker pull mono@sha256:74160f03572bdd44429a9b6eb44b8b53652c69d117c2a86563630a30d5cbaa9b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.0 MB (224998076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c344d77aaa5d5562d4220fe82d15cde77656b3a799ba079d41c22baf0eb9a2c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:43:20 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 26 Jan 2022 08:43:53 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 08:44:24 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 26 Jan 2022 08:54:47 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abebfb740ccc1862e47af90e80198192a8d3bdde5c0ed19b0f7cca498ca47651`  
		Last Modified: Wed, 26 Jan 2022 08:55:51 GMT  
		Size: 2.8 MB (2767028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2795ec88f83979b15e3c6db1c2ec3f0821d8d29e95c8e0300b1ba78d59018181`  
		Last Modified: Wed, 26 Jan 2022 08:56:01 GMT  
		Size: 64.8 MB (64778834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2766927b7358cb50e33a4326859b2b1ad063b157770ad6a0819e943d7def00d`  
		Last Modified: Wed, 26 Jan 2022 08:57:16 GMT  
		Size: 130.3 MB (130298483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; arm variant v5

```console
$ docker pull mono@sha256:2de02077ffd026f0975f56ff875d3e01107d6a3ccf8eaad0d9ccba3f9f133f6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.8 MB (180837635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7602ff61f125b4efcbd840b507c1c34d54e082649ecb9720a71df1ca425d07bd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:03:56 GMT
ADD file:f5674cd595d2eb9d698a67c0669348b7dca3158b3c949498321a875d56d1db0e in / 
# Tue, 01 Mar 2022 02:03:57 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:57:21 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 01 Mar 2022 03:58:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 01 Mar 2022 03:58:49 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 01 Mar 2022 04:05:36 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d93143e6711bdadb9413c811c28fed68303bd0eafd6640f6552d2147730818af`  
		Last Modified: Tue, 01 Mar 2022 02:20:01 GMT  
		Size: 24.9 MB (24886227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7183825792d2a4117dfd934e7bfa98096c0e0f7009bb2128ec1d0aee3687d91e`  
		Last Modified: Tue, 01 Mar 2022 04:07:42 GMT  
		Size: 2.5 MB (2462551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc482a880ade229d848039a9be2d482fec2b1322b972199cb414e1707e677641`  
		Last Modified: Tue, 01 Mar 2022 04:08:00 GMT  
		Size: 24.5 MB (24521787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241a55f8d12b4610dd0125cb5c3b0bf0a064c857337d54cfa8570c221585989e`  
		Last Modified: Tue, 01 Mar 2022 04:11:49 GMT  
		Size: 129.0 MB (128967070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; arm variant v7

```console
$ docker pull mono@sha256:6708588cf68ce4a7fccbbfce38ab30a657941e51f544730c2ffcea61ed5319fd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.7 MB (176747173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ea98640a9f50a3cd63b299c56d4e2e04af60cd16d20d893a06d5bafa619d0c9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:43:12 GMT
ADD file:ca8132e20773f7037458cc53fe20a7116f93c21c7479be5a2a1d739495dbe44e in / 
# Wed, 26 Jan 2022 01:43:13 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 03:04:26 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 26 Jan 2022 03:05:05 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 03:05:50 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 26 Jan 2022 03:12:29 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:20cc49690d9072283406c1c11e9b1dc1a247782cc8daa526b375d4a7f1cb6a94`  
		Last Modified: Wed, 26 Jan 2022 01:59:27 GMT  
		Size: 22.8 MB (22754397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a4467ce4f128a192b52b0b9f32a8d72323526aa13d035c32fe63f2d58df1289`  
		Last Modified: Wed, 26 Jan 2022 03:14:45 GMT  
		Size: 2.4 MB (2361945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914cd7581388c33133fdc5c0a7e0c93ec50175e1cb1331f950b31c7051370614`  
		Last Modified: Wed, 26 Jan 2022 03:15:00 GMT  
		Size: 23.8 MB (23814845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593ff100dd783ec2f01efe4b3dc5b03046f044b0a790839f94f167b991bb947f`  
		Last Modified: Wed, 26 Jan 2022 03:18:53 GMT  
		Size: 127.8 MB (127815986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:acd82d00ed67b121a1cc150a1d58789979051f1557cc80bf3bdc0b1816781a68
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.4 MB (203356562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1329aa306eb5aa2d88e3e014426c4883f34d13de4ea0e6cef07bb0faabae637b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:56 GMT
ADD file:796bc43a948899ba53bddebf7f613769fe96e8ea3a27eb7143d079c7a166ab01 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 04:55:58 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 26 Jan 2022 04:56:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 04:56:25 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 26 Jan 2022 04:58:31 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4c7c9f6f1115fd4f35807a2f6c1375759365a991748aee0111873e55255f150b`  
		Last Modified: Wed, 26 Jan 2022 01:49:55 GMT  
		Size: 25.9 MB (25923216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ae41c0f21a5178f528f317b54a12441d63a269bcac400d6d11308d3bdc345e`  
		Last Modified: Wed, 26 Jan 2022 04:59:46 GMT  
		Size: 2.6 MB (2634620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507fb7df7db2f4f93eba551713aafe01015a508c9e8a35ea0924671a6fbe4371`  
		Last Modified: Wed, 26 Jan 2022 04:59:51 GMT  
		Size: 29.4 MB (29361684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c88441c5b9c6960f220774c22bedfc47be13f42970a9c99de4471ee3968c2a8`  
		Last Modified: Wed, 26 Jan 2022 05:01:14 GMT  
		Size: 145.4 MB (145437042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; 386

```console
$ docker pull mono@sha256:fa39480455c25cb424336140fbaecb99658fdf5136cbc75a6c8bd864a7c9aed1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.8 MB (230817178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3efe880f33d8ecc6cfd9e0b6a8d078e70d7633f74730c9740f0194da19849ce0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:08:04 GMT
ADD file:d9d384f0402bc696e46e7529f52d64859a66aa7a60bca9c7beee7433a5f7af6e in / 
# Tue, 01 Mar 2022 02:08:04 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:15:20 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 01 Mar 2022 10:15:56 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 01 Mar 2022 10:16:42 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 01 Mar 2022 10:21:25 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c761ce6f2bf0aed07e1198c6f827444969d6e76dda0e55dbb45900920e551d27`  
		Last Modified: Tue, 01 Mar 2022 02:16:51 GMT  
		Size: 27.8 MB (27804590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffcb35ffd7b72ebed83212ac6044002e43ef026f4264a71f2968d42bde5b6d0c`  
		Last Modified: Tue, 01 Mar 2022 10:23:27 GMT  
		Size: 2.8 MB (2781505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:464559ee70703f0a5b09cdf8f320e12ccc8e8d8f5e465d178e72d4d1abc38f0f`  
		Last Modified: Tue, 01 Mar 2022 10:23:51 GMT  
		Size: 68.8 MB (68807982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28d6eb2c577bdff525ed34cb4d66e53492e36cbf7865103d344a84da6779e61b`  
		Last Modified: Tue, 01 Mar 2022 10:26:12 GMT  
		Size: 131.4 MB (131423101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; ppc64le

```console
$ docker pull mono@sha256:ac5c7487a16669c4cadeb0f80d26c37ca5d70cf6ecb443aba8978ae66d4e7b68
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.4 MB (192366459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e3e53ffd30bb030cc702a90f80528673dc449f07e331af50870b290e62c2cf6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:47:48 GMT
ADD file:d87bdffbd9392364fecbbd4148c710bc4948073e773a47c7b9ac1440ebb81c1e in / 
# Wed, 26 Jan 2022 01:47:52 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 05:19:28 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 26 Jan 2022 05:20:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 05:21:42 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 26 Jan 2022 05:35:14 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:249357001395b3de58d51723447880f3205d37ea7b902930b5c19f475d4ac8f9`  
		Last Modified: Wed, 26 Jan 2022 01:58:50 GMT  
		Size: 30.6 MB (30562293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca324940cbb49c6123545694d6238b2f9867f777b30db019afb8be32b821690d`  
		Last Modified: Wed, 26 Jan 2022 05:36:34 GMT  
		Size: 2.9 MB (2884587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8bbc208746983c602a3c5b3ed057beef5a9179e883614d0e67d4fa2b0480a0`  
		Last Modified: Wed, 26 Jan 2022 05:36:40 GMT  
		Size: 26.9 MB (26917771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22a606bee1870aa5fc638f38c2a60bc791119ef59136cb94a8dd8e9bb1a191b`  
		Last Modified: Wed, 26 Jan 2022 05:38:09 GMT  
		Size: 132.0 MB (132001808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10-slim`

```console
$ docker pull mono@sha256:47d5e1e94fa69b60e942d2911b3fbd10e26c42a194a7be9c14cda425ba6ac1ce
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
$ docker pull mono@sha256:50e0722f8e2967051c8eccd7c397b2abcbf7d55e07a581df5d5536a7fcc08f90
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94699593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4795a449eb03d2f677d6257d278263ad60660738af09cb361ecc9e48bf605b45`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:43:20 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 26 Jan 2022 08:43:53 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 08:44:24 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abebfb740ccc1862e47af90e80198192a8d3bdde5c0ed19b0f7cca498ca47651`  
		Last Modified: Wed, 26 Jan 2022 08:55:51 GMT  
		Size: 2.8 MB (2767028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2795ec88f83979b15e3c6db1c2ec3f0821d8d29e95c8e0300b1ba78d59018181`  
		Last Modified: Wed, 26 Jan 2022 08:56:01 GMT  
		Size: 64.8 MB (64778834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:31e36af681ea89764d353b09a3eb23169afc0de090c9f84ad9f61fdd4319b668
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51870565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ec2cc7350e7bd363783c078ee1b1887a529d3869df5e3b617f70ad376a8799f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:03:56 GMT
ADD file:f5674cd595d2eb9d698a67c0669348b7dca3158b3c949498321a875d56d1db0e in / 
# Tue, 01 Mar 2022 02:03:57 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:57:21 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 01 Mar 2022 03:58:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 01 Mar 2022 03:58:49 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d93143e6711bdadb9413c811c28fed68303bd0eafd6640f6552d2147730818af`  
		Last Modified: Tue, 01 Mar 2022 02:20:01 GMT  
		Size: 24.9 MB (24886227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7183825792d2a4117dfd934e7bfa98096c0e0f7009bb2128ec1d0aee3687d91e`  
		Last Modified: Tue, 01 Mar 2022 04:07:42 GMT  
		Size: 2.5 MB (2462551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc482a880ade229d848039a9be2d482fec2b1322b972199cb414e1707e677641`  
		Last Modified: Tue, 01 Mar 2022 04:08:00 GMT  
		Size: 24.5 MB (24521787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:f96167e344ddaa6095f07eabcc82fe8f3eca0b68e50832a3dce5d6710e13f1b6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48931187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb57121fb2edfad6c6cf3878875dfa4d89a277a6542473eb43c3abda83a12282`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:43:12 GMT
ADD file:ca8132e20773f7037458cc53fe20a7116f93c21c7479be5a2a1d739495dbe44e in / 
# Wed, 26 Jan 2022 01:43:13 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 03:04:26 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 26 Jan 2022 03:05:05 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 03:05:50 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:20cc49690d9072283406c1c11e9b1dc1a247782cc8daa526b375d4a7f1cb6a94`  
		Last Modified: Wed, 26 Jan 2022 01:59:27 GMT  
		Size: 22.8 MB (22754397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a4467ce4f128a192b52b0b9f32a8d72323526aa13d035c32fe63f2d58df1289`  
		Last Modified: Wed, 26 Jan 2022 03:14:45 GMT  
		Size: 2.4 MB (2361945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914cd7581388c33133fdc5c0a7e0c93ec50175e1cb1331f950b31c7051370614`  
		Last Modified: Wed, 26 Jan 2022 03:15:00 GMT  
		Size: 23.8 MB (23814845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:465edab3ad56e7c838daccd74dc2a98dcc141eb1582a7dbf5751bc4035efbb55
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57919520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72b6a3a2de34b9943fb43a4576eadad9747736546f6068f7b35aa7141e3821f3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:56 GMT
ADD file:796bc43a948899ba53bddebf7f613769fe96e8ea3a27eb7143d079c7a166ab01 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 04:55:58 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 26 Jan 2022 04:56:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 04:56:25 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4c7c9f6f1115fd4f35807a2f6c1375759365a991748aee0111873e55255f150b`  
		Last Modified: Wed, 26 Jan 2022 01:49:55 GMT  
		Size: 25.9 MB (25923216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ae41c0f21a5178f528f317b54a12441d63a269bcac400d6d11308d3bdc345e`  
		Last Modified: Wed, 26 Jan 2022 04:59:46 GMT  
		Size: 2.6 MB (2634620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507fb7df7db2f4f93eba551713aafe01015a508c9e8a35ea0924671a6fbe4371`  
		Last Modified: Wed, 26 Jan 2022 04:59:51 GMT  
		Size: 29.4 MB (29361684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; 386

```console
$ docker pull mono@sha256:ffc700d55d2531ca1a7ef781b6a35bc38f91cc563256a0a0d53cb63c536dd0f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99394077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92045d634716a8201968be5d5bba7b01b90b811f3a9aa00837d6c26ec20b463e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:08:04 GMT
ADD file:d9d384f0402bc696e46e7529f52d64859a66aa7a60bca9c7beee7433a5f7af6e in / 
# Tue, 01 Mar 2022 02:08:04 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:15:20 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 01 Mar 2022 10:15:56 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 01 Mar 2022 10:16:42 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c761ce6f2bf0aed07e1198c6f827444969d6e76dda0e55dbb45900920e551d27`  
		Last Modified: Tue, 01 Mar 2022 02:16:51 GMT  
		Size: 27.8 MB (27804590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffcb35ffd7b72ebed83212ac6044002e43ef026f4264a71f2968d42bde5b6d0c`  
		Last Modified: Tue, 01 Mar 2022 10:23:27 GMT  
		Size: 2.8 MB (2781505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:464559ee70703f0a5b09cdf8f320e12ccc8e8d8f5e465d178e72d4d1abc38f0f`  
		Last Modified: Tue, 01 Mar 2022 10:23:51 GMT  
		Size: 68.8 MB (68807982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:7278ad04855aa006705d06d8116073aaf8a4f650572b9059f49755cd64828d60
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.4 MB (60364651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6121787f7e75a0a14eca2f81b9decb58a0d48053fa53f032a995dd645d887da7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:47:48 GMT
ADD file:d87bdffbd9392364fecbbd4148c710bc4948073e773a47c7b9ac1440ebb81c1e in / 
# Wed, 26 Jan 2022 01:47:52 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 05:19:28 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 26 Jan 2022 05:20:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 05:21:42 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:249357001395b3de58d51723447880f3205d37ea7b902930b5c19f475d4ac8f9`  
		Last Modified: Wed, 26 Jan 2022 01:58:50 GMT  
		Size: 30.6 MB (30562293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca324940cbb49c6123545694d6238b2f9867f777b30db019afb8be32b821690d`  
		Last Modified: Wed, 26 Jan 2022 05:36:34 GMT  
		Size: 2.9 MB (2884587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8bbc208746983c602a3c5b3ed057beef5a9179e883614d0e67d4fa2b0480a0`  
		Last Modified: Wed, 26 Jan 2022 05:36:40 GMT  
		Size: 26.9 MB (26917771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10.0`

```console
$ docker pull mono@sha256:8db42556dc1e3afbdeb3b61de12c33922aa4b21bf4ed2f3c6afb639d8b5dde14
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
$ docker pull mono@sha256:74160f03572bdd44429a9b6eb44b8b53652c69d117c2a86563630a30d5cbaa9b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.0 MB (224998076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c344d77aaa5d5562d4220fe82d15cde77656b3a799ba079d41c22baf0eb9a2c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:43:20 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 26 Jan 2022 08:43:53 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 08:44:24 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 26 Jan 2022 08:54:47 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abebfb740ccc1862e47af90e80198192a8d3bdde5c0ed19b0f7cca498ca47651`  
		Last Modified: Wed, 26 Jan 2022 08:55:51 GMT  
		Size: 2.8 MB (2767028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2795ec88f83979b15e3c6db1c2ec3f0821d8d29e95c8e0300b1ba78d59018181`  
		Last Modified: Wed, 26 Jan 2022 08:56:01 GMT  
		Size: 64.8 MB (64778834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2766927b7358cb50e33a4326859b2b1ad063b157770ad6a0819e943d7def00d`  
		Last Modified: Wed, 26 Jan 2022 08:57:16 GMT  
		Size: 130.3 MB (130298483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; arm variant v5

```console
$ docker pull mono@sha256:2de02077ffd026f0975f56ff875d3e01107d6a3ccf8eaad0d9ccba3f9f133f6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.8 MB (180837635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7602ff61f125b4efcbd840b507c1c34d54e082649ecb9720a71df1ca425d07bd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:03:56 GMT
ADD file:f5674cd595d2eb9d698a67c0669348b7dca3158b3c949498321a875d56d1db0e in / 
# Tue, 01 Mar 2022 02:03:57 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:57:21 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 01 Mar 2022 03:58:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 01 Mar 2022 03:58:49 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 01 Mar 2022 04:05:36 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d93143e6711bdadb9413c811c28fed68303bd0eafd6640f6552d2147730818af`  
		Last Modified: Tue, 01 Mar 2022 02:20:01 GMT  
		Size: 24.9 MB (24886227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7183825792d2a4117dfd934e7bfa98096c0e0f7009bb2128ec1d0aee3687d91e`  
		Last Modified: Tue, 01 Mar 2022 04:07:42 GMT  
		Size: 2.5 MB (2462551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc482a880ade229d848039a9be2d482fec2b1322b972199cb414e1707e677641`  
		Last Modified: Tue, 01 Mar 2022 04:08:00 GMT  
		Size: 24.5 MB (24521787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241a55f8d12b4610dd0125cb5c3b0bf0a064c857337d54cfa8570c221585989e`  
		Last Modified: Tue, 01 Mar 2022 04:11:49 GMT  
		Size: 129.0 MB (128967070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; arm variant v7

```console
$ docker pull mono@sha256:6708588cf68ce4a7fccbbfce38ab30a657941e51f544730c2ffcea61ed5319fd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.7 MB (176747173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ea98640a9f50a3cd63b299c56d4e2e04af60cd16d20d893a06d5bafa619d0c9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:43:12 GMT
ADD file:ca8132e20773f7037458cc53fe20a7116f93c21c7479be5a2a1d739495dbe44e in / 
# Wed, 26 Jan 2022 01:43:13 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 03:04:26 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 26 Jan 2022 03:05:05 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 03:05:50 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 26 Jan 2022 03:12:29 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:20cc49690d9072283406c1c11e9b1dc1a247782cc8daa526b375d4a7f1cb6a94`  
		Last Modified: Wed, 26 Jan 2022 01:59:27 GMT  
		Size: 22.8 MB (22754397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a4467ce4f128a192b52b0b9f32a8d72323526aa13d035c32fe63f2d58df1289`  
		Last Modified: Wed, 26 Jan 2022 03:14:45 GMT  
		Size: 2.4 MB (2361945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914cd7581388c33133fdc5c0a7e0c93ec50175e1cb1331f950b31c7051370614`  
		Last Modified: Wed, 26 Jan 2022 03:15:00 GMT  
		Size: 23.8 MB (23814845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593ff100dd783ec2f01efe4b3dc5b03046f044b0a790839f94f167b991bb947f`  
		Last Modified: Wed, 26 Jan 2022 03:18:53 GMT  
		Size: 127.8 MB (127815986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:acd82d00ed67b121a1cc150a1d58789979051f1557cc80bf3bdc0b1816781a68
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.4 MB (203356562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1329aa306eb5aa2d88e3e014426c4883f34d13de4ea0e6cef07bb0faabae637b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:56 GMT
ADD file:796bc43a948899ba53bddebf7f613769fe96e8ea3a27eb7143d079c7a166ab01 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 04:55:58 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 26 Jan 2022 04:56:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 04:56:25 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 26 Jan 2022 04:58:31 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4c7c9f6f1115fd4f35807a2f6c1375759365a991748aee0111873e55255f150b`  
		Last Modified: Wed, 26 Jan 2022 01:49:55 GMT  
		Size: 25.9 MB (25923216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ae41c0f21a5178f528f317b54a12441d63a269bcac400d6d11308d3bdc345e`  
		Last Modified: Wed, 26 Jan 2022 04:59:46 GMT  
		Size: 2.6 MB (2634620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507fb7df7db2f4f93eba551713aafe01015a508c9e8a35ea0924671a6fbe4371`  
		Last Modified: Wed, 26 Jan 2022 04:59:51 GMT  
		Size: 29.4 MB (29361684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c88441c5b9c6960f220774c22bedfc47be13f42970a9c99de4471ee3968c2a8`  
		Last Modified: Wed, 26 Jan 2022 05:01:14 GMT  
		Size: 145.4 MB (145437042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; 386

```console
$ docker pull mono@sha256:fa39480455c25cb424336140fbaecb99658fdf5136cbc75a6c8bd864a7c9aed1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.8 MB (230817178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3efe880f33d8ecc6cfd9e0b6a8d078e70d7633f74730c9740f0194da19849ce0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:08:04 GMT
ADD file:d9d384f0402bc696e46e7529f52d64859a66aa7a60bca9c7beee7433a5f7af6e in / 
# Tue, 01 Mar 2022 02:08:04 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:15:20 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 01 Mar 2022 10:15:56 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 01 Mar 2022 10:16:42 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 01 Mar 2022 10:21:25 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c761ce6f2bf0aed07e1198c6f827444969d6e76dda0e55dbb45900920e551d27`  
		Last Modified: Tue, 01 Mar 2022 02:16:51 GMT  
		Size: 27.8 MB (27804590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffcb35ffd7b72ebed83212ac6044002e43ef026f4264a71f2968d42bde5b6d0c`  
		Last Modified: Tue, 01 Mar 2022 10:23:27 GMT  
		Size: 2.8 MB (2781505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:464559ee70703f0a5b09cdf8f320e12ccc8e8d8f5e465d178e72d4d1abc38f0f`  
		Last Modified: Tue, 01 Mar 2022 10:23:51 GMT  
		Size: 68.8 MB (68807982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28d6eb2c577bdff525ed34cb4d66e53492e36cbf7865103d344a84da6779e61b`  
		Last Modified: Tue, 01 Mar 2022 10:26:12 GMT  
		Size: 131.4 MB (131423101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; ppc64le

```console
$ docker pull mono@sha256:ac5c7487a16669c4cadeb0f80d26c37ca5d70cf6ecb443aba8978ae66d4e7b68
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.4 MB (192366459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e3e53ffd30bb030cc702a90f80528673dc449f07e331af50870b290e62c2cf6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:47:48 GMT
ADD file:d87bdffbd9392364fecbbd4148c710bc4948073e773a47c7b9ac1440ebb81c1e in / 
# Wed, 26 Jan 2022 01:47:52 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 05:19:28 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 26 Jan 2022 05:20:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 05:21:42 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 26 Jan 2022 05:35:14 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:249357001395b3de58d51723447880f3205d37ea7b902930b5c19f475d4ac8f9`  
		Last Modified: Wed, 26 Jan 2022 01:58:50 GMT  
		Size: 30.6 MB (30562293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca324940cbb49c6123545694d6238b2f9867f777b30db019afb8be32b821690d`  
		Last Modified: Wed, 26 Jan 2022 05:36:34 GMT  
		Size: 2.9 MB (2884587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8bbc208746983c602a3c5b3ed057beef5a9179e883614d0e67d4fa2b0480a0`  
		Last Modified: Wed, 26 Jan 2022 05:36:40 GMT  
		Size: 26.9 MB (26917771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22a606bee1870aa5fc638f38c2a60bc791119ef59136cb94a8dd8e9bb1a191b`  
		Last Modified: Wed, 26 Jan 2022 05:38:09 GMT  
		Size: 132.0 MB (132001808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10.0-slim`

```console
$ docker pull mono@sha256:47d5e1e94fa69b60e942d2911b3fbd10e26c42a194a7be9c14cda425ba6ac1ce
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
$ docker pull mono@sha256:50e0722f8e2967051c8eccd7c397b2abcbf7d55e07a581df5d5536a7fcc08f90
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94699593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4795a449eb03d2f677d6257d278263ad60660738af09cb361ecc9e48bf605b45`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:43:20 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 26 Jan 2022 08:43:53 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 08:44:24 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abebfb740ccc1862e47af90e80198192a8d3bdde5c0ed19b0f7cca498ca47651`  
		Last Modified: Wed, 26 Jan 2022 08:55:51 GMT  
		Size: 2.8 MB (2767028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2795ec88f83979b15e3c6db1c2ec3f0821d8d29e95c8e0300b1ba78d59018181`  
		Last Modified: Wed, 26 Jan 2022 08:56:01 GMT  
		Size: 64.8 MB (64778834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:31e36af681ea89764d353b09a3eb23169afc0de090c9f84ad9f61fdd4319b668
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51870565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ec2cc7350e7bd363783c078ee1b1887a529d3869df5e3b617f70ad376a8799f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:03:56 GMT
ADD file:f5674cd595d2eb9d698a67c0669348b7dca3158b3c949498321a875d56d1db0e in / 
# Tue, 01 Mar 2022 02:03:57 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:57:21 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 01 Mar 2022 03:58:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 01 Mar 2022 03:58:49 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d93143e6711bdadb9413c811c28fed68303bd0eafd6640f6552d2147730818af`  
		Last Modified: Tue, 01 Mar 2022 02:20:01 GMT  
		Size: 24.9 MB (24886227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7183825792d2a4117dfd934e7bfa98096c0e0f7009bb2128ec1d0aee3687d91e`  
		Last Modified: Tue, 01 Mar 2022 04:07:42 GMT  
		Size: 2.5 MB (2462551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc482a880ade229d848039a9be2d482fec2b1322b972199cb414e1707e677641`  
		Last Modified: Tue, 01 Mar 2022 04:08:00 GMT  
		Size: 24.5 MB (24521787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:f96167e344ddaa6095f07eabcc82fe8f3eca0b68e50832a3dce5d6710e13f1b6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48931187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb57121fb2edfad6c6cf3878875dfa4d89a277a6542473eb43c3abda83a12282`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:43:12 GMT
ADD file:ca8132e20773f7037458cc53fe20a7116f93c21c7479be5a2a1d739495dbe44e in / 
# Wed, 26 Jan 2022 01:43:13 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 03:04:26 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 26 Jan 2022 03:05:05 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 03:05:50 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:20cc49690d9072283406c1c11e9b1dc1a247782cc8daa526b375d4a7f1cb6a94`  
		Last Modified: Wed, 26 Jan 2022 01:59:27 GMT  
		Size: 22.8 MB (22754397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a4467ce4f128a192b52b0b9f32a8d72323526aa13d035c32fe63f2d58df1289`  
		Last Modified: Wed, 26 Jan 2022 03:14:45 GMT  
		Size: 2.4 MB (2361945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914cd7581388c33133fdc5c0a7e0c93ec50175e1cb1331f950b31c7051370614`  
		Last Modified: Wed, 26 Jan 2022 03:15:00 GMT  
		Size: 23.8 MB (23814845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:465edab3ad56e7c838daccd74dc2a98dcc141eb1582a7dbf5751bc4035efbb55
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57919520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72b6a3a2de34b9943fb43a4576eadad9747736546f6068f7b35aa7141e3821f3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:56 GMT
ADD file:796bc43a948899ba53bddebf7f613769fe96e8ea3a27eb7143d079c7a166ab01 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 04:55:58 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 26 Jan 2022 04:56:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 04:56:25 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4c7c9f6f1115fd4f35807a2f6c1375759365a991748aee0111873e55255f150b`  
		Last Modified: Wed, 26 Jan 2022 01:49:55 GMT  
		Size: 25.9 MB (25923216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ae41c0f21a5178f528f317b54a12441d63a269bcac400d6d11308d3bdc345e`  
		Last Modified: Wed, 26 Jan 2022 04:59:46 GMT  
		Size: 2.6 MB (2634620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507fb7df7db2f4f93eba551713aafe01015a508c9e8a35ea0924671a6fbe4371`  
		Last Modified: Wed, 26 Jan 2022 04:59:51 GMT  
		Size: 29.4 MB (29361684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; 386

```console
$ docker pull mono@sha256:ffc700d55d2531ca1a7ef781b6a35bc38f91cc563256a0a0d53cb63c536dd0f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99394077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92045d634716a8201968be5d5bba7b01b90b811f3a9aa00837d6c26ec20b463e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:08:04 GMT
ADD file:d9d384f0402bc696e46e7529f52d64859a66aa7a60bca9c7beee7433a5f7af6e in / 
# Tue, 01 Mar 2022 02:08:04 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:15:20 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 01 Mar 2022 10:15:56 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 01 Mar 2022 10:16:42 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c761ce6f2bf0aed07e1198c6f827444969d6e76dda0e55dbb45900920e551d27`  
		Last Modified: Tue, 01 Mar 2022 02:16:51 GMT  
		Size: 27.8 MB (27804590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffcb35ffd7b72ebed83212ac6044002e43ef026f4264a71f2968d42bde5b6d0c`  
		Last Modified: Tue, 01 Mar 2022 10:23:27 GMT  
		Size: 2.8 MB (2781505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:464559ee70703f0a5b09cdf8f320e12ccc8e8d8f5e465d178e72d4d1abc38f0f`  
		Last Modified: Tue, 01 Mar 2022 10:23:51 GMT  
		Size: 68.8 MB (68807982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:7278ad04855aa006705d06d8116073aaf8a4f650572b9059f49755cd64828d60
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.4 MB (60364651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6121787f7e75a0a14eca2f81b9decb58a0d48053fa53f032a995dd645d887da7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:47:48 GMT
ADD file:d87bdffbd9392364fecbbd4148c710bc4948073e773a47c7b9ac1440ebb81c1e in / 
# Wed, 26 Jan 2022 01:47:52 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 05:19:28 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 26 Jan 2022 05:20:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 05:21:42 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:249357001395b3de58d51723447880f3205d37ea7b902930b5c19f475d4ac8f9`  
		Last Modified: Wed, 26 Jan 2022 01:58:50 GMT  
		Size: 30.6 MB (30562293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca324940cbb49c6123545694d6238b2f9867f777b30db019afb8be32b821690d`  
		Last Modified: Wed, 26 Jan 2022 05:36:34 GMT  
		Size: 2.9 MB (2884587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8bbc208746983c602a3c5b3ed057beef5a9179e883614d0e67d4fa2b0480a0`  
		Last Modified: Wed, 26 Jan 2022 05:36:40 GMT  
		Size: 26.9 MB (26917771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10.0.104`

```console
$ docker pull mono@sha256:8db42556dc1e3afbdeb3b61de12c33922aa4b21bf4ed2f3c6afb639d8b5dde14
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
$ docker pull mono@sha256:74160f03572bdd44429a9b6eb44b8b53652c69d117c2a86563630a30d5cbaa9b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.0 MB (224998076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c344d77aaa5d5562d4220fe82d15cde77656b3a799ba079d41c22baf0eb9a2c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:43:20 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 26 Jan 2022 08:43:53 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 08:44:24 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 26 Jan 2022 08:54:47 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abebfb740ccc1862e47af90e80198192a8d3bdde5c0ed19b0f7cca498ca47651`  
		Last Modified: Wed, 26 Jan 2022 08:55:51 GMT  
		Size: 2.8 MB (2767028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2795ec88f83979b15e3c6db1c2ec3f0821d8d29e95c8e0300b1ba78d59018181`  
		Last Modified: Wed, 26 Jan 2022 08:56:01 GMT  
		Size: 64.8 MB (64778834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2766927b7358cb50e33a4326859b2b1ad063b157770ad6a0819e943d7def00d`  
		Last Modified: Wed, 26 Jan 2022 08:57:16 GMT  
		Size: 130.3 MB (130298483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; arm variant v5

```console
$ docker pull mono@sha256:2de02077ffd026f0975f56ff875d3e01107d6a3ccf8eaad0d9ccba3f9f133f6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.8 MB (180837635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7602ff61f125b4efcbd840b507c1c34d54e082649ecb9720a71df1ca425d07bd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:03:56 GMT
ADD file:f5674cd595d2eb9d698a67c0669348b7dca3158b3c949498321a875d56d1db0e in / 
# Tue, 01 Mar 2022 02:03:57 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:57:21 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 01 Mar 2022 03:58:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 01 Mar 2022 03:58:49 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 01 Mar 2022 04:05:36 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d93143e6711bdadb9413c811c28fed68303bd0eafd6640f6552d2147730818af`  
		Last Modified: Tue, 01 Mar 2022 02:20:01 GMT  
		Size: 24.9 MB (24886227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7183825792d2a4117dfd934e7bfa98096c0e0f7009bb2128ec1d0aee3687d91e`  
		Last Modified: Tue, 01 Mar 2022 04:07:42 GMT  
		Size: 2.5 MB (2462551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc482a880ade229d848039a9be2d482fec2b1322b972199cb414e1707e677641`  
		Last Modified: Tue, 01 Mar 2022 04:08:00 GMT  
		Size: 24.5 MB (24521787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241a55f8d12b4610dd0125cb5c3b0bf0a064c857337d54cfa8570c221585989e`  
		Last Modified: Tue, 01 Mar 2022 04:11:49 GMT  
		Size: 129.0 MB (128967070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; arm variant v7

```console
$ docker pull mono@sha256:6708588cf68ce4a7fccbbfce38ab30a657941e51f544730c2ffcea61ed5319fd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.7 MB (176747173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ea98640a9f50a3cd63b299c56d4e2e04af60cd16d20d893a06d5bafa619d0c9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:43:12 GMT
ADD file:ca8132e20773f7037458cc53fe20a7116f93c21c7479be5a2a1d739495dbe44e in / 
# Wed, 26 Jan 2022 01:43:13 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 03:04:26 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 26 Jan 2022 03:05:05 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 03:05:50 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 26 Jan 2022 03:12:29 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:20cc49690d9072283406c1c11e9b1dc1a247782cc8daa526b375d4a7f1cb6a94`  
		Last Modified: Wed, 26 Jan 2022 01:59:27 GMT  
		Size: 22.8 MB (22754397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a4467ce4f128a192b52b0b9f32a8d72323526aa13d035c32fe63f2d58df1289`  
		Last Modified: Wed, 26 Jan 2022 03:14:45 GMT  
		Size: 2.4 MB (2361945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914cd7581388c33133fdc5c0a7e0c93ec50175e1cb1331f950b31c7051370614`  
		Last Modified: Wed, 26 Jan 2022 03:15:00 GMT  
		Size: 23.8 MB (23814845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593ff100dd783ec2f01efe4b3dc5b03046f044b0a790839f94f167b991bb947f`  
		Last Modified: Wed, 26 Jan 2022 03:18:53 GMT  
		Size: 127.8 MB (127815986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:acd82d00ed67b121a1cc150a1d58789979051f1557cc80bf3bdc0b1816781a68
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.4 MB (203356562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1329aa306eb5aa2d88e3e014426c4883f34d13de4ea0e6cef07bb0faabae637b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:56 GMT
ADD file:796bc43a948899ba53bddebf7f613769fe96e8ea3a27eb7143d079c7a166ab01 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 04:55:58 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 26 Jan 2022 04:56:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 04:56:25 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 26 Jan 2022 04:58:31 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4c7c9f6f1115fd4f35807a2f6c1375759365a991748aee0111873e55255f150b`  
		Last Modified: Wed, 26 Jan 2022 01:49:55 GMT  
		Size: 25.9 MB (25923216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ae41c0f21a5178f528f317b54a12441d63a269bcac400d6d11308d3bdc345e`  
		Last Modified: Wed, 26 Jan 2022 04:59:46 GMT  
		Size: 2.6 MB (2634620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507fb7df7db2f4f93eba551713aafe01015a508c9e8a35ea0924671a6fbe4371`  
		Last Modified: Wed, 26 Jan 2022 04:59:51 GMT  
		Size: 29.4 MB (29361684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c88441c5b9c6960f220774c22bedfc47be13f42970a9c99de4471ee3968c2a8`  
		Last Modified: Wed, 26 Jan 2022 05:01:14 GMT  
		Size: 145.4 MB (145437042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; 386

```console
$ docker pull mono@sha256:fa39480455c25cb424336140fbaecb99658fdf5136cbc75a6c8bd864a7c9aed1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.8 MB (230817178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3efe880f33d8ecc6cfd9e0b6a8d078e70d7633f74730c9740f0194da19849ce0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:08:04 GMT
ADD file:d9d384f0402bc696e46e7529f52d64859a66aa7a60bca9c7beee7433a5f7af6e in / 
# Tue, 01 Mar 2022 02:08:04 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:15:20 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 01 Mar 2022 10:15:56 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 01 Mar 2022 10:16:42 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 01 Mar 2022 10:21:25 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c761ce6f2bf0aed07e1198c6f827444969d6e76dda0e55dbb45900920e551d27`  
		Last Modified: Tue, 01 Mar 2022 02:16:51 GMT  
		Size: 27.8 MB (27804590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffcb35ffd7b72ebed83212ac6044002e43ef026f4264a71f2968d42bde5b6d0c`  
		Last Modified: Tue, 01 Mar 2022 10:23:27 GMT  
		Size: 2.8 MB (2781505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:464559ee70703f0a5b09cdf8f320e12ccc8e8d8f5e465d178e72d4d1abc38f0f`  
		Last Modified: Tue, 01 Mar 2022 10:23:51 GMT  
		Size: 68.8 MB (68807982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28d6eb2c577bdff525ed34cb4d66e53492e36cbf7865103d344a84da6779e61b`  
		Last Modified: Tue, 01 Mar 2022 10:26:12 GMT  
		Size: 131.4 MB (131423101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; ppc64le

```console
$ docker pull mono@sha256:ac5c7487a16669c4cadeb0f80d26c37ca5d70cf6ecb443aba8978ae66d4e7b68
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.4 MB (192366459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e3e53ffd30bb030cc702a90f80528673dc449f07e331af50870b290e62c2cf6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:47:48 GMT
ADD file:d87bdffbd9392364fecbbd4148c710bc4948073e773a47c7b9ac1440ebb81c1e in / 
# Wed, 26 Jan 2022 01:47:52 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 05:19:28 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 26 Jan 2022 05:20:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 05:21:42 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 26 Jan 2022 05:35:14 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:249357001395b3de58d51723447880f3205d37ea7b902930b5c19f475d4ac8f9`  
		Last Modified: Wed, 26 Jan 2022 01:58:50 GMT  
		Size: 30.6 MB (30562293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca324940cbb49c6123545694d6238b2f9867f777b30db019afb8be32b821690d`  
		Last Modified: Wed, 26 Jan 2022 05:36:34 GMT  
		Size: 2.9 MB (2884587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8bbc208746983c602a3c5b3ed057beef5a9179e883614d0e67d4fa2b0480a0`  
		Last Modified: Wed, 26 Jan 2022 05:36:40 GMT  
		Size: 26.9 MB (26917771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22a606bee1870aa5fc638f38c2a60bc791119ef59136cb94a8dd8e9bb1a191b`  
		Last Modified: Wed, 26 Jan 2022 05:38:09 GMT  
		Size: 132.0 MB (132001808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10.0.104-slim`

```console
$ docker pull mono@sha256:47d5e1e94fa69b60e942d2911b3fbd10e26c42a194a7be9c14cda425ba6ac1ce
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
$ docker pull mono@sha256:50e0722f8e2967051c8eccd7c397b2abcbf7d55e07a581df5d5536a7fcc08f90
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94699593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4795a449eb03d2f677d6257d278263ad60660738af09cb361ecc9e48bf605b45`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:43:20 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 26 Jan 2022 08:43:53 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 08:44:24 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abebfb740ccc1862e47af90e80198192a8d3bdde5c0ed19b0f7cca498ca47651`  
		Last Modified: Wed, 26 Jan 2022 08:55:51 GMT  
		Size: 2.8 MB (2767028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2795ec88f83979b15e3c6db1c2ec3f0821d8d29e95c8e0300b1ba78d59018181`  
		Last Modified: Wed, 26 Jan 2022 08:56:01 GMT  
		Size: 64.8 MB (64778834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:31e36af681ea89764d353b09a3eb23169afc0de090c9f84ad9f61fdd4319b668
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51870565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ec2cc7350e7bd363783c078ee1b1887a529d3869df5e3b617f70ad376a8799f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:03:56 GMT
ADD file:f5674cd595d2eb9d698a67c0669348b7dca3158b3c949498321a875d56d1db0e in / 
# Tue, 01 Mar 2022 02:03:57 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:57:21 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 01 Mar 2022 03:58:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 01 Mar 2022 03:58:49 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d93143e6711bdadb9413c811c28fed68303bd0eafd6640f6552d2147730818af`  
		Last Modified: Tue, 01 Mar 2022 02:20:01 GMT  
		Size: 24.9 MB (24886227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7183825792d2a4117dfd934e7bfa98096c0e0f7009bb2128ec1d0aee3687d91e`  
		Last Modified: Tue, 01 Mar 2022 04:07:42 GMT  
		Size: 2.5 MB (2462551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc482a880ade229d848039a9be2d482fec2b1322b972199cb414e1707e677641`  
		Last Modified: Tue, 01 Mar 2022 04:08:00 GMT  
		Size: 24.5 MB (24521787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:f96167e344ddaa6095f07eabcc82fe8f3eca0b68e50832a3dce5d6710e13f1b6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48931187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb57121fb2edfad6c6cf3878875dfa4d89a277a6542473eb43c3abda83a12282`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:43:12 GMT
ADD file:ca8132e20773f7037458cc53fe20a7116f93c21c7479be5a2a1d739495dbe44e in / 
# Wed, 26 Jan 2022 01:43:13 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 03:04:26 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 26 Jan 2022 03:05:05 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 03:05:50 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:20cc49690d9072283406c1c11e9b1dc1a247782cc8daa526b375d4a7f1cb6a94`  
		Last Modified: Wed, 26 Jan 2022 01:59:27 GMT  
		Size: 22.8 MB (22754397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a4467ce4f128a192b52b0b9f32a8d72323526aa13d035c32fe63f2d58df1289`  
		Last Modified: Wed, 26 Jan 2022 03:14:45 GMT  
		Size: 2.4 MB (2361945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914cd7581388c33133fdc5c0a7e0c93ec50175e1cb1331f950b31c7051370614`  
		Last Modified: Wed, 26 Jan 2022 03:15:00 GMT  
		Size: 23.8 MB (23814845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:465edab3ad56e7c838daccd74dc2a98dcc141eb1582a7dbf5751bc4035efbb55
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57919520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72b6a3a2de34b9943fb43a4576eadad9747736546f6068f7b35aa7141e3821f3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:56 GMT
ADD file:796bc43a948899ba53bddebf7f613769fe96e8ea3a27eb7143d079c7a166ab01 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 04:55:58 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 26 Jan 2022 04:56:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 04:56:25 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4c7c9f6f1115fd4f35807a2f6c1375759365a991748aee0111873e55255f150b`  
		Last Modified: Wed, 26 Jan 2022 01:49:55 GMT  
		Size: 25.9 MB (25923216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ae41c0f21a5178f528f317b54a12441d63a269bcac400d6d11308d3bdc345e`  
		Last Modified: Wed, 26 Jan 2022 04:59:46 GMT  
		Size: 2.6 MB (2634620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507fb7df7db2f4f93eba551713aafe01015a508c9e8a35ea0924671a6fbe4371`  
		Last Modified: Wed, 26 Jan 2022 04:59:51 GMT  
		Size: 29.4 MB (29361684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; 386

```console
$ docker pull mono@sha256:ffc700d55d2531ca1a7ef781b6a35bc38f91cc563256a0a0d53cb63c536dd0f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99394077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92045d634716a8201968be5d5bba7b01b90b811f3a9aa00837d6c26ec20b463e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:08:04 GMT
ADD file:d9d384f0402bc696e46e7529f52d64859a66aa7a60bca9c7beee7433a5f7af6e in / 
# Tue, 01 Mar 2022 02:08:04 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:15:20 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 01 Mar 2022 10:15:56 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 01 Mar 2022 10:16:42 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c761ce6f2bf0aed07e1198c6f827444969d6e76dda0e55dbb45900920e551d27`  
		Last Modified: Tue, 01 Mar 2022 02:16:51 GMT  
		Size: 27.8 MB (27804590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffcb35ffd7b72ebed83212ac6044002e43ef026f4264a71f2968d42bde5b6d0c`  
		Last Modified: Tue, 01 Mar 2022 10:23:27 GMT  
		Size: 2.8 MB (2781505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:464559ee70703f0a5b09cdf8f320e12ccc8e8d8f5e465d178e72d4d1abc38f0f`  
		Last Modified: Tue, 01 Mar 2022 10:23:51 GMT  
		Size: 68.8 MB (68807982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:7278ad04855aa006705d06d8116073aaf8a4f650572b9059f49755cd64828d60
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.4 MB (60364651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6121787f7e75a0a14eca2f81b9decb58a0d48053fa53f032a995dd645d887da7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:47:48 GMT
ADD file:d87bdffbd9392364fecbbd4148c710bc4948073e773a47c7b9ac1440ebb81c1e in / 
# Wed, 26 Jan 2022 01:47:52 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 05:19:28 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 26 Jan 2022 05:20:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 05:21:42 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:249357001395b3de58d51723447880f3205d37ea7b902930b5c19f475d4ac8f9`  
		Last Modified: Wed, 26 Jan 2022 01:58:50 GMT  
		Size: 30.6 MB (30562293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca324940cbb49c6123545694d6238b2f9867f777b30db019afb8be32b821690d`  
		Last Modified: Wed, 26 Jan 2022 05:36:34 GMT  
		Size: 2.9 MB (2884587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8bbc208746983c602a3c5b3ed057beef5a9179e883614d0e67d4fa2b0480a0`  
		Last Modified: Wed, 26 Jan 2022 05:36:40 GMT  
		Size: 26.9 MB (26917771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.12`

```console
$ docker pull mono@sha256:0fb67a9a37f9399572c9446f92acf97f8e242b665f60f51805498cab2b17fc84
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
$ docker pull mono@sha256:6b7a7e5a048189d49dcb401794583cc3d7994ddbace52c916b229f9e68545f2e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.1 MB (236118449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:088d59542ba84be22020630040214ac5714f5455ed7dfa5f99cf2c05a964590b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:42:22 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 26 Jan 2022 08:42:47 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 08:43:11 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 26 Jan 2022 08:49:07 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd7c8aa8024e5da067c560f0319ca71064f55299dcc8b8d0cdf0c26dc826d09`  
		Last Modified: Wed, 26 Jan 2022 08:55:23 GMT  
		Size: 2.8 MB (2767042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d82173799248cedffd37d5bdd1f07b1c51a1b625b2e7a880a43d222f116d07`  
		Last Modified: Wed, 26 Jan 2022 08:55:34 GMT  
		Size: 64.8 MB (64759888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7823e38b4160826b37443754a040cea87df23809a9681e8be62028744db322ed`  
		Last Modified: Wed, 26 Jan 2022 08:56:37 GMT  
		Size: 141.4 MB (141437788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12` - linux; arm variant v5

```console
$ docker pull mono@sha256:cff835ec8c22098c42940eeb3618fed0b00c836fe1157eda320f0d000bf4a0e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.9 MB (191929783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c8d899777bbcafd23a69b4effe3d6c1ce8c82f871ff44333774ad8e1360e804`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:03:56 GMT
ADD file:f5674cd595d2eb9d698a67c0669348b7dca3158b3c949498321a875d56d1db0e in / 
# Tue, 01 Mar 2022 02:03:57 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:55:41 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 01 Mar 2022 03:56:20 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 01 Mar 2022 03:57:06 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 01 Mar 2022 04:02:10 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d93143e6711bdadb9413c811c28fed68303bd0eafd6640f6552d2147730818af`  
		Last Modified: Tue, 01 Mar 2022 02:20:01 GMT  
		Size: 24.9 MB (24886227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0217ce2cacf32a6058fe38fb20cfe9a6d980cf80cca400013545f361b1b3fd`  
		Last Modified: Tue, 01 Mar 2022 04:07:02 GMT  
		Size: 2.5 MB (2462533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68de90092907e27be985b209e7586a431f836320c0bb1b413435a590965fc290`  
		Last Modified: Tue, 01 Mar 2022 04:07:19 GMT  
		Size: 24.5 MB (24493246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b35ea8d607897d4a5fc65b78859a5f93a1d200489340e252ec304024542a0da`  
		Last Modified: Tue, 01 Mar 2022 04:09:54 GMT  
		Size: 140.1 MB (140087777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12` - linux; arm variant v7

```console
$ docker pull mono@sha256:a0f15b2324df9644625fd899bc9491ba399197f1554bea1fa931b12eb1dd1e74
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.8 MB (187845702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dcbf347de76bd0a6f0723618d9de9548b3d0e9b6af63961becd5a5d1ff74837`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:43:12 GMT
ADD file:ca8132e20773f7037458cc53fe20a7116f93c21c7479be5a2a1d739495dbe44e in / 
# Wed, 26 Jan 2022 01:43:13 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 03:02:36 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 26 Jan 2022 03:03:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 03:04:03 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 26 Jan 2022 03:09:10 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:20cc49690d9072283406c1c11e9b1dc1a247782cc8daa526b375d4a7f1cb6a94`  
		Last Modified: Wed, 26 Jan 2022 01:59:27 GMT  
		Size: 22.8 MB (22754397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242f21c9f2ea2b8610338b20aa4a933d07978910d00d961eb9395cf5ad6a14ba`  
		Last Modified: Wed, 26 Jan 2022 03:14:04 GMT  
		Size: 2.4 MB (2361950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf05b1bf44b0bc6e31c02c1f89b71c97d2120bd5088a235a9a2a58ccdc973e4`  
		Last Modified: Wed, 26 Jan 2022 03:14:20 GMT  
		Size: 23.8 MB (23782786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd4b90a8da9c282d5bd778e5a73064eeef59ebcf39aeacd8d471e25e4ee8e9b`  
		Last Modified: Wed, 26 Jan 2022 03:16:54 GMT  
		Size: 138.9 MB (138946569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:6099f20ed14b5d90f2c433f1b5be4fdb75ecb73e555e27d832226aa745ab9a99
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.5 MB (214451499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34db74ee86a7e6e6ce7640619a498ddf102f6457b05048d89e5cacb3d02e8f57`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:56 GMT
ADD file:796bc43a948899ba53bddebf7f613769fe96e8ea3a27eb7143d079c7a166ab01 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 04:54:45 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 26 Jan 2022 04:55:28 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 04:55:43 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 26 Jan 2022 04:57:25 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4c7c9f6f1115fd4f35807a2f6c1375759365a991748aee0111873e55255f150b`  
		Last Modified: Wed, 26 Jan 2022 01:49:55 GMT  
		Size: 25.9 MB (25923216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145db9a792c54fdb1a14e3673d8bf7e6bfbdcfcd16e9f20670088dc797a755f9`  
		Last Modified: Wed, 26 Jan 2022 04:59:19 GMT  
		Size: 2.6 MB (2634624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba55b80938abbcaf307229652d0245d64085b55a6aa9db6572f5ac715e9d3959`  
		Last Modified: Wed, 26 Jan 2022 04:59:26 GMT  
		Size: 29.3 MB (29318190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4d2da081a628a5666b5ec038b6bdadd12c4a83da6c999e6b2c9cf213c84874`  
		Last Modified: Wed, 26 Jan 2022 05:00:30 GMT  
		Size: 156.6 MB (156575469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12` - linux; 386

```console
$ docker pull mono@sha256:82a3f21fd720a3de8dd1e2ac27a9ba549947ca8fc1fefb8cae9a4680183cf19e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.9 MB (241920861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:629648c952e20ac82023401475080241331753ddc53cd6ec14a439a426731e84`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:08:04 GMT
ADD file:d9d384f0402bc696e46e7529f52d64859a66aa7a60bca9c7beee7433a5f7af6e in / 
# Tue, 01 Mar 2022 02:08:04 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:13:49 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 01 Mar 2022 10:14:37 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 01 Mar 2022 10:15:09 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 01 Mar 2022 10:18:40 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c761ce6f2bf0aed07e1198c6f827444969d6e76dda0e55dbb45900920e551d27`  
		Last Modified: Tue, 01 Mar 2022 02:16:51 GMT  
		Size: 27.8 MB (27804590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011b9d654300beab54b280fd3e0b1f7170919be5028f5e31a210af8a83500cfc`  
		Last Modified: Tue, 01 Mar 2022 10:22:39 GMT  
		Size: 2.8 MB (2781491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4b91a20a9ead3771e864dc94eb15af13cf873e35ca6bbc27fe1fdd66f0422f`  
		Last Modified: Tue, 01 Mar 2022 10:23:02 GMT  
		Size: 68.8 MB (68778600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500a4fcb909ee1b095dc7db9d0546dcd766236538aa5715dc6dc627ab73b5df6`  
		Last Modified: Tue, 01 Mar 2022 10:25:00 GMT  
		Size: 142.6 MB (142556180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12` - linux; ppc64le

```console
$ docker pull mono@sha256:56250e313f76e60e694eec7ba9ff5ca5179b9ca48a2c2e412195364e66aa79b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.6 MB (203588810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05b37ef992318378fe939868450034dde3384ac8ea697fb3550081a98836d2f1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:47:48 GMT
ADD file:d87bdffbd9392364fecbbd4148c710bc4948073e773a47c7b9ac1440ebb81c1e in / 
# Wed, 26 Jan 2022 01:47:52 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 05:16:29 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 26 Jan 2022 05:17:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 05:19:13 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 26 Jan 2022 05:28:25 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:249357001395b3de58d51723447880f3205d37ea7b902930b5c19f475d4ac8f9`  
		Last Modified: Wed, 26 Jan 2022 01:58:50 GMT  
		Size: 30.6 MB (30562293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b424ab5d806f162b76c369311f6e539940178ab8b306c053879a77ff4a77d4`  
		Last Modified: Wed, 26 Jan 2022 05:36:07 GMT  
		Size: 2.9 MB (2884629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7982f75341da8b4f46a0677a86d66dfaa5a4b464e669fc85629e0bf531fa21`  
		Last Modified: Wed, 26 Jan 2022 05:36:13 GMT  
		Size: 26.9 MB (26874043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210fd04001c965c8d905729a394f394aa15b2fa6eba24a1d6f8b31ee1a5457f0`  
		Last Modified: Wed, 26 Jan 2022 05:37:22 GMT  
		Size: 143.3 MB (143267845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.12-slim`

```console
$ docker pull mono@sha256:64905a436cf3e3de5b6f7f987510b79c99887049d9017f6fe39c8b7dbe3a2952
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
$ docker pull mono@sha256:ed5b708feef72f630c6308b60ceed7cb68bb7b7c387578bfbde1053beaabce61
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94680661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a18e38b2a9d6d4f318e22f13aefc58314f800630814e3f42179f97f985e865e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:42:22 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 26 Jan 2022 08:42:47 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 08:43:11 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd7c8aa8024e5da067c560f0319ca71064f55299dcc8b8d0cdf0c26dc826d09`  
		Last Modified: Wed, 26 Jan 2022 08:55:23 GMT  
		Size: 2.8 MB (2767042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d82173799248cedffd37d5bdd1f07b1c51a1b625b2e7a880a43d222f116d07`  
		Last Modified: Wed, 26 Jan 2022 08:55:34 GMT  
		Size: 64.8 MB (64759888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:9ebb92f30258b4a717d77f185bc834d5f02ec3aab3634d67488b930d268acf7b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51842006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bd52c60156350534c857630fa5165139d0297938596bd00c52e61afaf7b7779`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:03:56 GMT
ADD file:f5674cd595d2eb9d698a67c0669348b7dca3158b3c949498321a875d56d1db0e in / 
# Tue, 01 Mar 2022 02:03:57 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:55:41 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 01 Mar 2022 03:56:20 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 01 Mar 2022 03:57:06 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d93143e6711bdadb9413c811c28fed68303bd0eafd6640f6552d2147730818af`  
		Last Modified: Tue, 01 Mar 2022 02:20:01 GMT  
		Size: 24.9 MB (24886227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0217ce2cacf32a6058fe38fb20cfe9a6d980cf80cca400013545f361b1b3fd`  
		Last Modified: Tue, 01 Mar 2022 04:07:02 GMT  
		Size: 2.5 MB (2462533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68de90092907e27be985b209e7586a431f836320c0bb1b413435a590965fc290`  
		Last Modified: Tue, 01 Mar 2022 04:07:19 GMT  
		Size: 24.5 MB (24493246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:deeb347482762f58ad102823f33d7538fa92175c60c0b63faaeee9a648fb10c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48899133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72cf0e6b2305941d40d03f813edfbd2a1b015b02e86552bc90cfe2a050b14bd7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:43:12 GMT
ADD file:ca8132e20773f7037458cc53fe20a7116f93c21c7479be5a2a1d739495dbe44e in / 
# Wed, 26 Jan 2022 01:43:13 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 03:02:36 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 26 Jan 2022 03:03:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 03:04:03 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:20cc49690d9072283406c1c11e9b1dc1a247782cc8daa526b375d4a7f1cb6a94`  
		Last Modified: Wed, 26 Jan 2022 01:59:27 GMT  
		Size: 22.8 MB (22754397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242f21c9f2ea2b8610338b20aa4a933d07978910d00d961eb9395cf5ad6a14ba`  
		Last Modified: Wed, 26 Jan 2022 03:14:04 GMT  
		Size: 2.4 MB (2361950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf05b1bf44b0bc6e31c02c1f89b71c97d2120bd5088a235a9a2a58ccdc973e4`  
		Last Modified: Wed, 26 Jan 2022 03:14:20 GMT  
		Size: 23.8 MB (23782786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:2d8b961112b0f7f9c0cb6a334ffd574c95162bc7fa8d5b2aa366004f11c42d1e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57876030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:670158c5d1ee00bcf609d8daf07279a4093cc98203ef3362fc17510761426523`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:56 GMT
ADD file:796bc43a948899ba53bddebf7f613769fe96e8ea3a27eb7143d079c7a166ab01 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 04:54:45 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 26 Jan 2022 04:55:28 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 04:55:43 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4c7c9f6f1115fd4f35807a2f6c1375759365a991748aee0111873e55255f150b`  
		Last Modified: Wed, 26 Jan 2022 01:49:55 GMT  
		Size: 25.9 MB (25923216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145db9a792c54fdb1a14e3673d8bf7e6bfbdcfcd16e9f20670088dc797a755f9`  
		Last Modified: Wed, 26 Jan 2022 04:59:19 GMT  
		Size: 2.6 MB (2634624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba55b80938abbcaf307229652d0245d64085b55a6aa9db6572f5ac715e9d3959`  
		Last Modified: Wed, 26 Jan 2022 04:59:26 GMT  
		Size: 29.3 MB (29318190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12-slim` - linux; 386

```console
$ docker pull mono@sha256:d9c23198eec7e2c304b84f004811aa4baba762614a35374bd820ff5d24e3c378
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99364681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18db94f8442093daf5003e5853ae0b168af2ec80a3ed2a7babfbbd1dc3627d99`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:08:04 GMT
ADD file:d9d384f0402bc696e46e7529f52d64859a66aa7a60bca9c7beee7433a5f7af6e in / 
# Tue, 01 Mar 2022 02:08:04 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:13:49 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 01 Mar 2022 10:14:37 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 01 Mar 2022 10:15:09 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c761ce6f2bf0aed07e1198c6f827444969d6e76dda0e55dbb45900920e551d27`  
		Last Modified: Tue, 01 Mar 2022 02:16:51 GMT  
		Size: 27.8 MB (27804590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011b9d654300beab54b280fd3e0b1f7170919be5028f5e31a210af8a83500cfc`  
		Last Modified: Tue, 01 Mar 2022 10:22:39 GMT  
		Size: 2.8 MB (2781491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4b91a20a9ead3771e864dc94eb15af13cf873e35ca6bbc27fe1fdd66f0422f`  
		Last Modified: Tue, 01 Mar 2022 10:23:02 GMT  
		Size: 68.8 MB (68778600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:d575747ba8940111c62f95739e8a754b9b87078977fba75f2e18524deb22a8a2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.3 MB (60320965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e081680305b9949003bab588e040386a8353300452f2a819aae1a529471cea28`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:47:48 GMT
ADD file:d87bdffbd9392364fecbbd4148c710bc4948073e773a47c7b9ac1440ebb81c1e in / 
# Wed, 26 Jan 2022 01:47:52 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 05:16:29 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 26 Jan 2022 05:17:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 05:19:13 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:249357001395b3de58d51723447880f3205d37ea7b902930b5c19f475d4ac8f9`  
		Last Modified: Wed, 26 Jan 2022 01:58:50 GMT  
		Size: 30.6 MB (30562293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b424ab5d806f162b76c369311f6e539940178ab8b306c053879a77ff4a77d4`  
		Last Modified: Wed, 26 Jan 2022 05:36:07 GMT  
		Size: 2.9 MB (2884629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7982f75341da8b4f46a0677a86d66dfaa5a4b464e669fc85629e0bf531fa21`  
		Last Modified: Wed, 26 Jan 2022 05:36:13 GMT  
		Size: 26.9 MB (26874043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.12.0`

```console
$ docker pull mono@sha256:0fb67a9a37f9399572c9446f92acf97f8e242b665f60f51805498cab2b17fc84
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
$ docker pull mono@sha256:6b7a7e5a048189d49dcb401794583cc3d7994ddbace52c916b229f9e68545f2e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.1 MB (236118449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:088d59542ba84be22020630040214ac5714f5455ed7dfa5f99cf2c05a964590b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:42:22 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 26 Jan 2022 08:42:47 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 08:43:11 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 26 Jan 2022 08:49:07 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd7c8aa8024e5da067c560f0319ca71064f55299dcc8b8d0cdf0c26dc826d09`  
		Last Modified: Wed, 26 Jan 2022 08:55:23 GMT  
		Size: 2.8 MB (2767042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d82173799248cedffd37d5bdd1f07b1c51a1b625b2e7a880a43d222f116d07`  
		Last Modified: Wed, 26 Jan 2022 08:55:34 GMT  
		Size: 64.8 MB (64759888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7823e38b4160826b37443754a040cea87df23809a9681e8be62028744db322ed`  
		Last Modified: Wed, 26 Jan 2022 08:56:37 GMT  
		Size: 141.4 MB (141437788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0` - linux; arm variant v5

```console
$ docker pull mono@sha256:cff835ec8c22098c42940eeb3618fed0b00c836fe1157eda320f0d000bf4a0e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.9 MB (191929783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c8d899777bbcafd23a69b4effe3d6c1ce8c82f871ff44333774ad8e1360e804`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:03:56 GMT
ADD file:f5674cd595d2eb9d698a67c0669348b7dca3158b3c949498321a875d56d1db0e in / 
# Tue, 01 Mar 2022 02:03:57 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:55:41 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 01 Mar 2022 03:56:20 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 01 Mar 2022 03:57:06 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 01 Mar 2022 04:02:10 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d93143e6711bdadb9413c811c28fed68303bd0eafd6640f6552d2147730818af`  
		Last Modified: Tue, 01 Mar 2022 02:20:01 GMT  
		Size: 24.9 MB (24886227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0217ce2cacf32a6058fe38fb20cfe9a6d980cf80cca400013545f361b1b3fd`  
		Last Modified: Tue, 01 Mar 2022 04:07:02 GMT  
		Size: 2.5 MB (2462533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68de90092907e27be985b209e7586a431f836320c0bb1b413435a590965fc290`  
		Last Modified: Tue, 01 Mar 2022 04:07:19 GMT  
		Size: 24.5 MB (24493246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b35ea8d607897d4a5fc65b78859a5f93a1d200489340e252ec304024542a0da`  
		Last Modified: Tue, 01 Mar 2022 04:09:54 GMT  
		Size: 140.1 MB (140087777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0` - linux; arm variant v7

```console
$ docker pull mono@sha256:a0f15b2324df9644625fd899bc9491ba399197f1554bea1fa931b12eb1dd1e74
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.8 MB (187845702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dcbf347de76bd0a6f0723618d9de9548b3d0e9b6af63961becd5a5d1ff74837`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:43:12 GMT
ADD file:ca8132e20773f7037458cc53fe20a7116f93c21c7479be5a2a1d739495dbe44e in / 
# Wed, 26 Jan 2022 01:43:13 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 03:02:36 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 26 Jan 2022 03:03:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 03:04:03 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 26 Jan 2022 03:09:10 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:20cc49690d9072283406c1c11e9b1dc1a247782cc8daa526b375d4a7f1cb6a94`  
		Last Modified: Wed, 26 Jan 2022 01:59:27 GMT  
		Size: 22.8 MB (22754397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242f21c9f2ea2b8610338b20aa4a933d07978910d00d961eb9395cf5ad6a14ba`  
		Last Modified: Wed, 26 Jan 2022 03:14:04 GMT  
		Size: 2.4 MB (2361950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf05b1bf44b0bc6e31c02c1f89b71c97d2120bd5088a235a9a2a58ccdc973e4`  
		Last Modified: Wed, 26 Jan 2022 03:14:20 GMT  
		Size: 23.8 MB (23782786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd4b90a8da9c282d5bd778e5a73064eeef59ebcf39aeacd8d471e25e4ee8e9b`  
		Last Modified: Wed, 26 Jan 2022 03:16:54 GMT  
		Size: 138.9 MB (138946569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:6099f20ed14b5d90f2c433f1b5be4fdb75ecb73e555e27d832226aa745ab9a99
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.5 MB (214451499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34db74ee86a7e6e6ce7640619a498ddf102f6457b05048d89e5cacb3d02e8f57`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:56 GMT
ADD file:796bc43a948899ba53bddebf7f613769fe96e8ea3a27eb7143d079c7a166ab01 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 04:54:45 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 26 Jan 2022 04:55:28 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 04:55:43 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 26 Jan 2022 04:57:25 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4c7c9f6f1115fd4f35807a2f6c1375759365a991748aee0111873e55255f150b`  
		Last Modified: Wed, 26 Jan 2022 01:49:55 GMT  
		Size: 25.9 MB (25923216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145db9a792c54fdb1a14e3673d8bf7e6bfbdcfcd16e9f20670088dc797a755f9`  
		Last Modified: Wed, 26 Jan 2022 04:59:19 GMT  
		Size: 2.6 MB (2634624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba55b80938abbcaf307229652d0245d64085b55a6aa9db6572f5ac715e9d3959`  
		Last Modified: Wed, 26 Jan 2022 04:59:26 GMT  
		Size: 29.3 MB (29318190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4d2da081a628a5666b5ec038b6bdadd12c4a83da6c999e6b2c9cf213c84874`  
		Last Modified: Wed, 26 Jan 2022 05:00:30 GMT  
		Size: 156.6 MB (156575469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0` - linux; 386

```console
$ docker pull mono@sha256:82a3f21fd720a3de8dd1e2ac27a9ba549947ca8fc1fefb8cae9a4680183cf19e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.9 MB (241920861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:629648c952e20ac82023401475080241331753ddc53cd6ec14a439a426731e84`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:08:04 GMT
ADD file:d9d384f0402bc696e46e7529f52d64859a66aa7a60bca9c7beee7433a5f7af6e in / 
# Tue, 01 Mar 2022 02:08:04 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:13:49 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 01 Mar 2022 10:14:37 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 01 Mar 2022 10:15:09 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 01 Mar 2022 10:18:40 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c761ce6f2bf0aed07e1198c6f827444969d6e76dda0e55dbb45900920e551d27`  
		Last Modified: Tue, 01 Mar 2022 02:16:51 GMT  
		Size: 27.8 MB (27804590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011b9d654300beab54b280fd3e0b1f7170919be5028f5e31a210af8a83500cfc`  
		Last Modified: Tue, 01 Mar 2022 10:22:39 GMT  
		Size: 2.8 MB (2781491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4b91a20a9ead3771e864dc94eb15af13cf873e35ca6bbc27fe1fdd66f0422f`  
		Last Modified: Tue, 01 Mar 2022 10:23:02 GMT  
		Size: 68.8 MB (68778600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500a4fcb909ee1b095dc7db9d0546dcd766236538aa5715dc6dc627ab73b5df6`  
		Last Modified: Tue, 01 Mar 2022 10:25:00 GMT  
		Size: 142.6 MB (142556180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0` - linux; ppc64le

```console
$ docker pull mono@sha256:56250e313f76e60e694eec7ba9ff5ca5179b9ca48a2c2e412195364e66aa79b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.6 MB (203588810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05b37ef992318378fe939868450034dde3384ac8ea697fb3550081a98836d2f1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:47:48 GMT
ADD file:d87bdffbd9392364fecbbd4148c710bc4948073e773a47c7b9ac1440ebb81c1e in / 
# Wed, 26 Jan 2022 01:47:52 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 05:16:29 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 26 Jan 2022 05:17:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 05:19:13 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 26 Jan 2022 05:28:25 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:249357001395b3de58d51723447880f3205d37ea7b902930b5c19f475d4ac8f9`  
		Last Modified: Wed, 26 Jan 2022 01:58:50 GMT  
		Size: 30.6 MB (30562293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b424ab5d806f162b76c369311f6e539940178ab8b306c053879a77ff4a77d4`  
		Last Modified: Wed, 26 Jan 2022 05:36:07 GMT  
		Size: 2.9 MB (2884629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7982f75341da8b4f46a0677a86d66dfaa5a4b464e669fc85629e0bf531fa21`  
		Last Modified: Wed, 26 Jan 2022 05:36:13 GMT  
		Size: 26.9 MB (26874043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210fd04001c965c8d905729a394f394aa15b2fa6eba24a1d6f8b31ee1a5457f0`  
		Last Modified: Wed, 26 Jan 2022 05:37:22 GMT  
		Size: 143.3 MB (143267845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.12.0-slim`

```console
$ docker pull mono@sha256:64905a436cf3e3de5b6f7f987510b79c99887049d9017f6fe39c8b7dbe3a2952
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
$ docker pull mono@sha256:ed5b708feef72f630c6308b60ceed7cb68bb7b7c387578bfbde1053beaabce61
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94680661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a18e38b2a9d6d4f318e22f13aefc58314f800630814e3f42179f97f985e865e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:42:22 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 26 Jan 2022 08:42:47 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 08:43:11 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd7c8aa8024e5da067c560f0319ca71064f55299dcc8b8d0cdf0c26dc826d09`  
		Last Modified: Wed, 26 Jan 2022 08:55:23 GMT  
		Size: 2.8 MB (2767042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d82173799248cedffd37d5bdd1f07b1c51a1b625b2e7a880a43d222f116d07`  
		Last Modified: Wed, 26 Jan 2022 08:55:34 GMT  
		Size: 64.8 MB (64759888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:9ebb92f30258b4a717d77f185bc834d5f02ec3aab3634d67488b930d268acf7b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51842006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bd52c60156350534c857630fa5165139d0297938596bd00c52e61afaf7b7779`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:03:56 GMT
ADD file:f5674cd595d2eb9d698a67c0669348b7dca3158b3c949498321a875d56d1db0e in / 
# Tue, 01 Mar 2022 02:03:57 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:55:41 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 01 Mar 2022 03:56:20 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 01 Mar 2022 03:57:06 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d93143e6711bdadb9413c811c28fed68303bd0eafd6640f6552d2147730818af`  
		Last Modified: Tue, 01 Mar 2022 02:20:01 GMT  
		Size: 24.9 MB (24886227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0217ce2cacf32a6058fe38fb20cfe9a6d980cf80cca400013545f361b1b3fd`  
		Last Modified: Tue, 01 Mar 2022 04:07:02 GMT  
		Size: 2.5 MB (2462533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68de90092907e27be985b209e7586a431f836320c0bb1b413435a590965fc290`  
		Last Modified: Tue, 01 Mar 2022 04:07:19 GMT  
		Size: 24.5 MB (24493246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:deeb347482762f58ad102823f33d7538fa92175c60c0b63faaeee9a648fb10c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48899133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72cf0e6b2305941d40d03f813edfbd2a1b015b02e86552bc90cfe2a050b14bd7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:43:12 GMT
ADD file:ca8132e20773f7037458cc53fe20a7116f93c21c7479be5a2a1d739495dbe44e in / 
# Wed, 26 Jan 2022 01:43:13 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 03:02:36 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 26 Jan 2022 03:03:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 03:04:03 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:20cc49690d9072283406c1c11e9b1dc1a247782cc8daa526b375d4a7f1cb6a94`  
		Last Modified: Wed, 26 Jan 2022 01:59:27 GMT  
		Size: 22.8 MB (22754397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242f21c9f2ea2b8610338b20aa4a933d07978910d00d961eb9395cf5ad6a14ba`  
		Last Modified: Wed, 26 Jan 2022 03:14:04 GMT  
		Size: 2.4 MB (2361950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf05b1bf44b0bc6e31c02c1f89b71c97d2120bd5088a235a9a2a58ccdc973e4`  
		Last Modified: Wed, 26 Jan 2022 03:14:20 GMT  
		Size: 23.8 MB (23782786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:2d8b961112b0f7f9c0cb6a334ffd574c95162bc7fa8d5b2aa366004f11c42d1e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57876030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:670158c5d1ee00bcf609d8daf07279a4093cc98203ef3362fc17510761426523`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:56 GMT
ADD file:796bc43a948899ba53bddebf7f613769fe96e8ea3a27eb7143d079c7a166ab01 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 04:54:45 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 26 Jan 2022 04:55:28 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 04:55:43 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4c7c9f6f1115fd4f35807a2f6c1375759365a991748aee0111873e55255f150b`  
		Last Modified: Wed, 26 Jan 2022 01:49:55 GMT  
		Size: 25.9 MB (25923216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145db9a792c54fdb1a14e3673d8bf7e6bfbdcfcd16e9f20670088dc797a755f9`  
		Last Modified: Wed, 26 Jan 2022 04:59:19 GMT  
		Size: 2.6 MB (2634624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba55b80938abbcaf307229652d0245d64085b55a6aa9db6572f5ac715e9d3959`  
		Last Modified: Wed, 26 Jan 2022 04:59:26 GMT  
		Size: 29.3 MB (29318190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0-slim` - linux; 386

```console
$ docker pull mono@sha256:d9c23198eec7e2c304b84f004811aa4baba762614a35374bd820ff5d24e3c378
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99364681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18db94f8442093daf5003e5853ae0b168af2ec80a3ed2a7babfbbd1dc3627d99`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:08:04 GMT
ADD file:d9d384f0402bc696e46e7529f52d64859a66aa7a60bca9c7beee7433a5f7af6e in / 
# Tue, 01 Mar 2022 02:08:04 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:13:49 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 01 Mar 2022 10:14:37 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 01 Mar 2022 10:15:09 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c761ce6f2bf0aed07e1198c6f827444969d6e76dda0e55dbb45900920e551d27`  
		Last Modified: Tue, 01 Mar 2022 02:16:51 GMT  
		Size: 27.8 MB (27804590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011b9d654300beab54b280fd3e0b1f7170919be5028f5e31a210af8a83500cfc`  
		Last Modified: Tue, 01 Mar 2022 10:22:39 GMT  
		Size: 2.8 MB (2781491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4b91a20a9ead3771e864dc94eb15af13cf873e35ca6bbc27fe1fdd66f0422f`  
		Last Modified: Tue, 01 Mar 2022 10:23:02 GMT  
		Size: 68.8 MB (68778600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:d575747ba8940111c62f95739e8a754b9b87078977fba75f2e18524deb22a8a2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.3 MB (60320965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e081680305b9949003bab588e040386a8353300452f2a819aae1a529471cea28`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:47:48 GMT
ADD file:d87bdffbd9392364fecbbd4148c710bc4948073e773a47c7b9ac1440ebb81c1e in / 
# Wed, 26 Jan 2022 01:47:52 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 05:16:29 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 26 Jan 2022 05:17:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 05:19:13 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:249357001395b3de58d51723447880f3205d37ea7b902930b5c19f475d4ac8f9`  
		Last Modified: Wed, 26 Jan 2022 01:58:50 GMT  
		Size: 30.6 MB (30562293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b424ab5d806f162b76c369311f6e539940178ab8b306c053879a77ff4a77d4`  
		Last Modified: Wed, 26 Jan 2022 05:36:07 GMT  
		Size: 2.9 MB (2884629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7982f75341da8b4f46a0677a86d66dfaa5a4b464e669fc85629e0bf531fa21`  
		Last Modified: Wed, 26 Jan 2022 05:36:13 GMT  
		Size: 26.9 MB (26874043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.12.0.122`

```console
$ docker pull mono@sha256:0fb67a9a37f9399572c9446f92acf97f8e242b665f60f51805498cab2b17fc84
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
$ docker pull mono@sha256:6b7a7e5a048189d49dcb401794583cc3d7994ddbace52c916b229f9e68545f2e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.1 MB (236118449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:088d59542ba84be22020630040214ac5714f5455ed7dfa5f99cf2c05a964590b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:42:22 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 26 Jan 2022 08:42:47 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 08:43:11 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 26 Jan 2022 08:49:07 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd7c8aa8024e5da067c560f0319ca71064f55299dcc8b8d0cdf0c26dc826d09`  
		Last Modified: Wed, 26 Jan 2022 08:55:23 GMT  
		Size: 2.8 MB (2767042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d82173799248cedffd37d5bdd1f07b1c51a1b625b2e7a880a43d222f116d07`  
		Last Modified: Wed, 26 Jan 2022 08:55:34 GMT  
		Size: 64.8 MB (64759888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7823e38b4160826b37443754a040cea87df23809a9681e8be62028744db322ed`  
		Last Modified: Wed, 26 Jan 2022 08:56:37 GMT  
		Size: 141.4 MB (141437788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.122` - linux; arm variant v5

```console
$ docker pull mono@sha256:cff835ec8c22098c42940eeb3618fed0b00c836fe1157eda320f0d000bf4a0e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.9 MB (191929783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c8d899777bbcafd23a69b4effe3d6c1ce8c82f871ff44333774ad8e1360e804`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:03:56 GMT
ADD file:f5674cd595d2eb9d698a67c0669348b7dca3158b3c949498321a875d56d1db0e in / 
# Tue, 01 Mar 2022 02:03:57 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:55:41 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 01 Mar 2022 03:56:20 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 01 Mar 2022 03:57:06 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 01 Mar 2022 04:02:10 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d93143e6711bdadb9413c811c28fed68303bd0eafd6640f6552d2147730818af`  
		Last Modified: Tue, 01 Mar 2022 02:20:01 GMT  
		Size: 24.9 MB (24886227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0217ce2cacf32a6058fe38fb20cfe9a6d980cf80cca400013545f361b1b3fd`  
		Last Modified: Tue, 01 Mar 2022 04:07:02 GMT  
		Size: 2.5 MB (2462533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68de90092907e27be985b209e7586a431f836320c0bb1b413435a590965fc290`  
		Last Modified: Tue, 01 Mar 2022 04:07:19 GMT  
		Size: 24.5 MB (24493246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b35ea8d607897d4a5fc65b78859a5f93a1d200489340e252ec304024542a0da`  
		Last Modified: Tue, 01 Mar 2022 04:09:54 GMT  
		Size: 140.1 MB (140087777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.122` - linux; arm variant v7

```console
$ docker pull mono@sha256:a0f15b2324df9644625fd899bc9491ba399197f1554bea1fa931b12eb1dd1e74
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.8 MB (187845702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dcbf347de76bd0a6f0723618d9de9548b3d0e9b6af63961becd5a5d1ff74837`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:43:12 GMT
ADD file:ca8132e20773f7037458cc53fe20a7116f93c21c7479be5a2a1d739495dbe44e in / 
# Wed, 26 Jan 2022 01:43:13 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 03:02:36 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 26 Jan 2022 03:03:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 03:04:03 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 26 Jan 2022 03:09:10 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:20cc49690d9072283406c1c11e9b1dc1a247782cc8daa526b375d4a7f1cb6a94`  
		Last Modified: Wed, 26 Jan 2022 01:59:27 GMT  
		Size: 22.8 MB (22754397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242f21c9f2ea2b8610338b20aa4a933d07978910d00d961eb9395cf5ad6a14ba`  
		Last Modified: Wed, 26 Jan 2022 03:14:04 GMT  
		Size: 2.4 MB (2361950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf05b1bf44b0bc6e31c02c1f89b71c97d2120bd5088a235a9a2a58ccdc973e4`  
		Last Modified: Wed, 26 Jan 2022 03:14:20 GMT  
		Size: 23.8 MB (23782786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd4b90a8da9c282d5bd778e5a73064eeef59ebcf39aeacd8d471e25e4ee8e9b`  
		Last Modified: Wed, 26 Jan 2022 03:16:54 GMT  
		Size: 138.9 MB (138946569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.122` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:6099f20ed14b5d90f2c433f1b5be4fdb75ecb73e555e27d832226aa745ab9a99
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.5 MB (214451499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34db74ee86a7e6e6ce7640619a498ddf102f6457b05048d89e5cacb3d02e8f57`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:56 GMT
ADD file:796bc43a948899ba53bddebf7f613769fe96e8ea3a27eb7143d079c7a166ab01 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 04:54:45 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 26 Jan 2022 04:55:28 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 04:55:43 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 26 Jan 2022 04:57:25 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4c7c9f6f1115fd4f35807a2f6c1375759365a991748aee0111873e55255f150b`  
		Last Modified: Wed, 26 Jan 2022 01:49:55 GMT  
		Size: 25.9 MB (25923216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145db9a792c54fdb1a14e3673d8bf7e6bfbdcfcd16e9f20670088dc797a755f9`  
		Last Modified: Wed, 26 Jan 2022 04:59:19 GMT  
		Size: 2.6 MB (2634624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba55b80938abbcaf307229652d0245d64085b55a6aa9db6572f5ac715e9d3959`  
		Last Modified: Wed, 26 Jan 2022 04:59:26 GMT  
		Size: 29.3 MB (29318190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4d2da081a628a5666b5ec038b6bdadd12c4a83da6c999e6b2c9cf213c84874`  
		Last Modified: Wed, 26 Jan 2022 05:00:30 GMT  
		Size: 156.6 MB (156575469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.122` - linux; 386

```console
$ docker pull mono@sha256:82a3f21fd720a3de8dd1e2ac27a9ba549947ca8fc1fefb8cae9a4680183cf19e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.9 MB (241920861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:629648c952e20ac82023401475080241331753ddc53cd6ec14a439a426731e84`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:08:04 GMT
ADD file:d9d384f0402bc696e46e7529f52d64859a66aa7a60bca9c7beee7433a5f7af6e in / 
# Tue, 01 Mar 2022 02:08:04 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:13:49 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 01 Mar 2022 10:14:37 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 01 Mar 2022 10:15:09 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 01 Mar 2022 10:18:40 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c761ce6f2bf0aed07e1198c6f827444969d6e76dda0e55dbb45900920e551d27`  
		Last Modified: Tue, 01 Mar 2022 02:16:51 GMT  
		Size: 27.8 MB (27804590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011b9d654300beab54b280fd3e0b1f7170919be5028f5e31a210af8a83500cfc`  
		Last Modified: Tue, 01 Mar 2022 10:22:39 GMT  
		Size: 2.8 MB (2781491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4b91a20a9ead3771e864dc94eb15af13cf873e35ca6bbc27fe1fdd66f0422f`  
		Last Modified: Tue, 01 Mar 2022 10:23:02 GMT  
		Size: 68.8 MB (68778600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500a4fcb909ee1b095dc7db9d0546dcd766236538aa5715dc6dc627ab73b5df6`  
		Last Modified: Tue, 01 Mar 2022 10:25:00 GMT  
		Size: 142.6 MB (142556180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.122` - linux; ppc64le

```console
$ docker pull mono@sha256:56250e313f76e60e694eec7ba9ff5ca5179b9ca48a2c2e412195364e66aa79b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.6 MB (203588810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05b37ef992318378fe939868450034dde3384ac8ea697fb3550081a98836d2f1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:47:48 GMT
ADD file:d87bdffbd9392364fecbbd4148c710bc4948073e773a47c7b9ac1440ebb81c1e in / 
# Wed, 26 Jan 2022 01:47:52 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 05:16:29 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 26 Jan 2022 05:17:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 05:19:13 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 26 Jan 2022 05:28:25 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:249357001395b3de58d51723447880f3205d37ea7b902930b5c19f475d4ac8f9`  
		Last Modified: Wed, 26 Jan 2022 01:58:50 GMT  
		Size: 30.6 MB (30562293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b424ab5d806f162b76c369311f6e539940178ab8b306c053879a77ff4a77d4`  
		Last Modified: Wed, 26 Jan 2022 05:36:07 GMT  
		Size: 2.9 MB (2884629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7982f75341da8b4f46a0677a86d66dfaa5a4b464e669fc85629e0bf531fa21`  
		Last Modified: Wed, 26 Jan 2022 05:36:13 GMT  
		Size: 26.9 MB (26874043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210fd04001c965c8d905729a394f394aa15b2fa6eba24a1d6f8b31ee1a5457f0`  
		Last Modified: Wed, 26 Jan 2022 05:37:22 GMT  
		Size: 143.3 MB (143267845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.12.0.122-slim`

```console
$ docker pull mono@sha256:64905a436cf3e3de5b6f7f987510b79c99887049d9017f6fe39c8b7dbe3a2952
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
$ docker pull mono@sha256:ed5b708feef72f630c6308b60ceed7cb68bb7b7c387578bfbde1053beaabce61
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94680661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a18e38b2a9d6d4f318e22f13aefc58314f800630814e3f42179f97f985e865e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:42:22 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 26 Jan 2022 08:42:47 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 08:43:11 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd7c8aa8024e5da067c560f0319ca71064f55299dcc8b8d0cdf0c26dc826d09`  
		Last Modified: Wed, 26 Jan 2022 08:55:23 GMT  
		Size: 2.8 MB (2767042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d82173799248cedffd37d5bdd1f07b1c51a1b625b2e7a880a43d222f116d07`  
		Last Modified: Wed, 26 Jan 2022 08:55:34 GMT  
		Size: 64.8 MB (64759888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.122-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:9ebb92f30258b4a717d77f185bc834d5f02ec3aab3634d67488b930d268acf7b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51842006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bd52c60156350534c857630fa5165139d0297938596bd00c52e61afaf7b7779`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:03:56 GMT
ADD file:f5674cd595d2eb9d698a67c0669348b7dca3158b3c949498321a875d56d1db0e in / 
# Tue, 01 Mar 2022 02:03:57 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:55:41 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 01 Mar 2022 03:56:20 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 01 Mar 2022 03:57:06 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d93143e6711bdadb9413c811c28fed68303bd0eafd6640f6552d2147730818af`  
		Last Modified: Tue, 01 Mar 2022 02:20:01 GMT  
		Size: 24.9 MB (24886227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0217ce2cacf32a6058fe38fb20cfe9a6d980cf80cca400013545f361b1b3fd`  
		Last Modified: Tue, 01 Mar 2022 04:07:02 GMT  
		Size: 2.5 MB (2462533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68de90092907e27be985b209e7586a431f836320c0bb1b413435a590965fc290`  
		Last Modified: Tue, 01 Mar 2022 04:07:19 GMT  
		Size: 24.5 MB (24493246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.122-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:deeb347482762f58ad102823f33d7538fa92175c60c0b63faaeee9a648fb10c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48899133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72cf0e6b2305941d40d03f813edfbd2a1b015b02e86552bc90cfe2a050b14bd7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:43:12 GMT
ADD file:ca8132e20773f7037458cc53fe20a7116f93c21c7479be5a2a1d739495dbe44e in / 
# Wed, 26 Jan 2022 01:43:13 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 03:02:36 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 26 Jan 2022 03:03:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 03:04:03 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:20cc49690d9072283406c1c11e9b1dc1a247782cc8daa526b375d4a7f1cb6a94`  
		Last Modified: Wed, 26 Jan 2022 01:59:27 GMT  
		Size: 22.8 MB (22754397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242f21c9f2ea2b8610338b20aa4a933d07978910d00d961eb9395cf5ad6a14ba`  
		Last Modified: Wed, 26 Jan 2022 03:14:04 GMT  
		Size: 2.4 MB (2361950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf05b1bf44b0bc6e31c02c1f89b71c97d2120bd5088a235a9a2a58ccdc973e4`  
		Last Modified: Wed, 26 Jan 2022 03:14:20 GMT  
		Size: 23.8 MB (23782786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.122-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:2d8b961112b0f7f9c0cb6a334ffd574c95162bc7fa8d5b2aa366004f11c42d1e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57876030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:670158c5d1ee00bcf609d8daf07279a4093cc98203ef3362fc17510761426523`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:56 GMT
ADD file:796bc43a948899ba53bddebf7f613769fe96e8ea3a27eb7143d079c7a166ab01 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 04:54:45 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 26 Jan 2022 04:55:28 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 04:55:43 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4c7c9f6f1115fd4f35807a2f6c1375759365a991748aee0111873e55255f150b`  
		Last Modified: Wed, 26 Jan 2022 01:49:55 GMT  
		Size: 25.9 MB (25923216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145db9a792c54fdb1a14e3673d8bf7e6bfbdcfcd16e9f20670088dc797a755f9`  
		Last Modified: Wed, 26 Jan 2022 04:59:19 GMT  
		Size: 2.6 MB (2634624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba55b80938abbcaf307229652d0245d64085b55a6aa9db6572f5ac715e9d3959`  
		Last Modified: Wed, 26 Jan 2022 04:59:26 GMT  
		Size: 29.3 MB (29318190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.122-slim` - linux; 386

```console
$ docker pull mono@sha256:d9c23198eec7e2c304b84f004811aa4baba762614a35374bd820ff5d24e3c378
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99364681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18db94f8442093daf5003e5853ae0b168af2ec80a3ed2a7babfbbd1dc3627d99`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:08:04 GMT
ADD file:d9d384f0402bc696e46e7529f52d64859a66aa7a60bca9c7beee7433a5f7af6e in / 
# Tue, 01 Mar 2022 02:08:04 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:13:49 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 01 Mar 2022 10:14:37 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 01 Mar 2022 10:15:09 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c761ce6f2bf0aed07e1198c6f827444969d6e76dda0e55dbb45900920e551d27`  
		Last Modified: Tue, 01 Mar 2022 02:16:51 GMT  
		Size: 27.8 MB (27804590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011b9d654300beab54b280fd3e0b1f7170919be5028f5e31a210af8a83500cfc`  
		Last Modified: Tue, 01 Mar 2022 10:22:39 GMT  
		Size: 2.8 MB (2781491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4b91a20a9ead3771e864dc94eb15af13cf873e35ca6bbc27fe1fdd66f0422f`  
		Last Modified: Tue, 01 Mar 2022 10:23:02 GMT  
		Size: 68.8 MB (68778600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.122-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:d575747ba8940111c62f95739e8a754b9b87078977fba75f2e18524deb22a8a2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.3 MB (60320965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e081680305b9949003bab588e040386a8353300452f2a819aae1a529471cea28`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:47:48 GMT
ADD file:d87bdffbd9392364fecbbd4148c710bc4948073e773a47c7b9ac1440ebb81c1e in / 
# Wed, 26 Jan 2022 01:47:52 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 05:16:29 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 26 Jan 2022 05:17:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 05:19:13 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:249357001395b3de58d51723447880f3205d37ea7b902930b5c19f475d4ac8f9`  
		Last Modified: Wed, 26 Jan 2022 01:58:50 GMT  
		Size: 30.6 MB (30562293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b424ab5d806f162b76c369311f6e539940178ab8b306c053879a77ff4a77d4`  
		Last Modified: Wed, 26 Jan 2022 05:36:07 GMT  
		Size: 2.9 MB (2884629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7982f75341da8b4f46a0677a86d66dfaa5a4b464e669fc85629e0bf531fa21`  
		Last Modified: Wed, 26 Jan 2022 05:36:13 GMT  
		Size: 26.9 MB (26874043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:latest`

```console
$ docker pull mono@sha256:0fb67a9a37f9399572c9446f92acf97f8e242b665f60f51805498cab2b17fc84
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
$ docker pull mono@sha256:6b7a7e5a048189d49dcb401794583cc3d7994ddbace52c916b229f9e68545f2e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.1 MB (236118449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:088d59542ba84be22020630040214ac5714f5455ed7dfa5f99cf2c05a964590b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:42:22 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 26 Jan 2022 08:42:47 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 08:43:11 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 26 Jan 2022 08:49:07 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd7c8aa8024e5da067c560f0319ca71064f55299dcc8b8d0cdf0c26dc826d09`  
		Last Modified: Wed, 26 Jan 2022 08:55:23 GMT  
		Size: 2.8 MB (2767042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d82173799248cedffd37d5bdd1f07b1c51a1b625b2e7a880a43d222f116d07`  
		Last Modified: Wed, 26 Jan 2022 08:55:34 GMT  
		Size: 64.8 MB (64759888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7823e38b4160826b37443754a040cea87df23809a9681e8be62028744db322ed`  
		Last Modified: Wed, 26 Jan 2022 08:56:37 GMT  
		Size: 141.4 MB (141437788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm variant v5

```console
$ docker pull mono@sha256:cff835ec8c22098c42940eeb3618fed0b00c836fe1157eda320f0d000bf4a0e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.9 MB (191929783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c8d899777bbcafd23a69b4effe3d6c1ce8c82f871ff44333774ad8e1360e804`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:03:56 GMT
ADD file:f5674cd595d2eb9d698a67c0669348b7dca3158b3c949498321a875d56d1db0e in / 
# Tue, 01 Mar 2022 02:03:57 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:55:41 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 01 Mar 2022 03:56:20 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 01 Mar 2022 03:57:06 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 01 Mar 2022 04:02:10 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d93143e6711bdadb9413c811c28fed68303bd0eafd6640f6552d2147730818af`  
		Last Modified: Tue, 01 Mar 2022 02:20:01 GMT  
		Size: 24.9 MB (24886227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0217ce2cacf32a6058fe38fb20cfe9a6d980cf80cca400013545f361b1b3fd`  
		Last Modified: Tue, 01 Mar 2022 04:07:02 GMT  
		Size: 2.5 MB (2462533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68de90092907e27be985b209e7586a431f836320c0bb1b413435a590965fc290`  
		Last Modified: Tue, 01 Mar 2022 04:07:19 GMT  
		Size: 24.5 MB (24493246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b35ea8d607897d4a5fc65b78859a5f93a1d200489340e252ec304024542a0da`  
		Last Modified: Tue, 01 Mar 2022 04:09:54 GMT  
		Size: 140.1 MB (140087777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm variant v7

```console
$ docker pull mono@sha256:a0f15b2324df9644625fd899bc9491ba399197f1554bea1fa931b12eb1dd1e74
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.8 MB (187845702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dcbf347de76bd0a6f0723618d9de9548b3d0e9b6af63961becd5a5d1ff74837`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:43:12 GMT
ADD file:ca8132e20773f7037458cc53fe20a7116f93c21c7479be5a2a1d739495dbe44e in / 
# Wed, 26 Jan 2022 01:43:13 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 03:02:36 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 26 Jan 2022 03:03:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 03:04:03 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 26 Jan 2022 03:09:10 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:20cc49690d9072283406c1c11e9b1dc1a247782cc8daa526b375d4a7f1cb6a94`  
		Last Modified: Wed, 26 Jan 2022 01:59:27 GMT  
		Size: 22.8 MB (22754397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242f21c9f2ea2b8610338b20aa4a933d07978910d00d961eb9395cf5ad6a14ba`  
		Last Modified: Wed, 26 Jan 2022 03:14:04 GMT  
		Size: 2.4 MB (2361950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf05b1bf44b0bc6e31c02c1f89b71c97d2120bd5088a235a9a2a58ccdc973e4`  
		Last Modified: Wed, 26 Jan 2022 03:14:20 GMT  
		Size: 23.8 MB (23782786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd4b90a8da9c282d5bd778e5a73064eeef59ebcf39aeacd8d471e25e4ee8e9b`  
		Last Modified: Wed, 26 Jan 2022 03:16:54 GMT  
		Size: 138.9 MB (138946569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:6099f20ed14b5d90f2c433f1b5be4fdb75ecb73e555e27d832226aa745ab9a99
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.5 MB (214451499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34db74ee86a7e6e6ce7640619a498ddf102f6457b05048d89e5cacb3d02e8f57`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:56 GMT
ADD file:796bc43a948899ba53bddebf7f613769fe96e8ea3a27eb7143d079c7a166ab01 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 04:54:45 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 26 Jan 2022 04:55:28 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 04:55:43 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 26 Jan 2022 04:57:25 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4c7c9f6f1115fd4f35807a2f6c1375759365a991748aee0111873e55255f150b`  
		Last Modified: Wed, 26 Jan 2022 01:49:55 GMT  
		Size: 25.9 MB (25923216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145db9a792c54fdb1a14e3673d8bf7e6bfbdcfcd16e9f20670088dc797a755f9`  
		Last Modified: Wed, 26 Jan 2022 04:59:19 GMT  
		Size: 2.6 MB (2634624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba55b80938abbcaf307229652d0245d64085b55a6aa9db6572f5ac715e9d3959`  
		Last Modified: Wed, 26 Jan 2022 04:59:26 GMT  
		Size: 29.3 MB (29318190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4d2da081a628a5666b5ec038b6bdadd12c4a83da6c999e6b2c9cf213c84874`  
		Last Modified: Wed, 26 Jan 2022 05:00:30 GMT  
		Size: 156.6 MB (156575469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; 386

```console
$ docker pull mono@sha256:82a3f21fd720a3de8dd1e2ac27a9ba549947ca8fc1fefb8cae9a4680183cf19e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.9 MB (241920861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:629648c952e20ac82023401475080241331753ddc53cd6ec14a439a426731e84`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:08:04 GMT
ADD file:d9d384f0402bc696e46e7529f52d64859a66aa7a60bca9c7beee7433a5f7af6e in / 
# Tue, 01 Mar 2022 02:08:04 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:13:49 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 01 Mar 2022 10:14:37 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 01 Mar 2022 10:15:09 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 01 Mar 2022 10:18:40 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c761ce6f2bf0aed07e1198c6f827444969d6e76dda0e55dbb45900920e551d27`  
		Last Modified: Tue, 01 Mar 2022 02:16:51 GMT  
		Size: 27.8 MB (27804590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011b9d654300beab54b280fd3e0b1f7170919be5028f5e31a210af8a83500cfc`  
		Last Modified: Tue, 01 Mar 2022 10:22:39 GMT  
		Size: 2.8 MB (2781491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4b91a20a9ead3771e864dc94eb15af13cf873e35ca6bbc27fe1fdd66f0422f`  
		Last Modified: Tue, 01 Mar 2022 10:23:02 GMT  
		Size: 68.8 MB (68778600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500a4fcb909ee1b095dc7db9d0546dcd766236538aa5715dc6dc627ab73b5df6`  
		Last Modified: Tue, 01 Mar 2022 10:25:00 GMT  
		Size: 142.6 MB (142556180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; ppc64le

```console
$ docker pull mono@sha256:56250e313f76e60e694eec7ba9ff5ca5179b9ca48a2c2e412195364e66aa79b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.6 MB (203588810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05b37ef992318378fe939868450034dde3384ac8ea697fb3550081a98836d2f1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:47:48 GMT
ADD file:d87bdffbd9392364fecbbd4148c710bc4948073e773a47c7b9ac1440ebb81c1e in / 
# Wed, 26 Jan 2022 01:47:52 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 05:16:29 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 26 Jan 2022 05:17:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 05:19:13 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 26 Jan 2022 05:28:25 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:249357001395b3de58d51723447880f3205d37ea7b902930b5c19f475d4ac8f9`  
		Last Modified: Wed, 26 Jan 2022 01:58:50 GMT  
		Size: 30.6 MB (30562293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b424ab5d806f162b76c369311f6e539940178ab8b306c053879a77ff4a77d4`  
		Last Modified: Wed, 26 Jan 2022 05:36:07 GMT  
		Size: 2.9 MB (2884629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7982f75341da8b4f46a0677a86d66dfaa5a4b464e669fc85629e0bf531fa21`  
		Last Modified: Wed, 26 Jan 2022 05:36:13 GMT  
		Size: 26.9 MB (26874043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210fd04001c965c8d905729a394f394aa15b2fa6eba24a1d6f8b31ee1a5457f0`  
		Last Modified: Wed, 26 Jan 2022 05:37:22 GMT  
		Size: 143.3 MB (143267845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:slim`

```console
$ docker pull mono@sha256:64905a436cf3e3de5b6f7f987510b79c99887049d9017f6fe39c8b7dbe3a2952
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
$ docker pull mono@sha256:ed5b708feef72f630c6308b60ceed7cb68bb7b7c387578bfbde1053beaabce61
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94680661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a18e38b2a9d6d4f318e22f13aefc58314f800630814e3f42179f97f985e865e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:42:22 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 26 Jan 2022 08:42:47 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 08:43:11 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd7c8aa8024e5da067c560f0319ca71064f55299dcc8b8d0cdf0c26dc826d09`  
		Last Modified: Wed, 26 Jan 2022 08:55:23 GMT  
		Size: 2.8 MB (2767042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d82173799248cedffd37d5bdd1f07b1c51a1b625b2e7a880a43d222f116d07`  
		Last Modified: Wed, 26 Jan 2022 08:55:34 GMT  
		Size: 64.8 MB (64759888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:9ebb92f30258b4a717d77f185bc834d5f02ec3aab3634d67488b930d268acf7b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51842006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bd52c60156350534c857630fa5165139d0297938596bd00c52e61afaf7b7779`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:03:56 GMT
ADD file:f5674cd595d2eb9d698a67c0669348b7dca3158b3c949498321a875d56d1db0e in / 
# Tue, 01 Mar 2022 02:03:57 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:55:41 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 01 Mar 2022 03:56:20 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 01 Mar 2022 03:57:06 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d93143e6711bdadb9413c811c28fed68303bd0eafd6640f6552d2147730818af`  
		Last Modified: Tue, 01 Mar 2022 02:20:01 GMT  
		Size: 24.9 MB (24886227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0217ce2cacf32a6058fe38fb20cfe9a6d980cf80cca400013545f361b1b3fd`  
		Last Modified: Tue, 01 Mar 2022 04:07:02 GMT  
		Size: 2.5 MB (2462533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68de90092907e27be985b209e7586a431f836320c0bb1b413435a590965fc290`  
		Last Modified: Tue, 01 Mar 2022 04:07:19 GMT  
		Size: 24.5 MB (24493246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:deeb347482762f58ad102823f33d7538fa92175c60c0b63faaeee9a648fb10c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48899133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72cf0e6b2305941d40d03f813edfbd2a1b015b02e86552bc90cfe2a050b14bd7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:43:12 GMT
ADD file:ca8132e20773f7037458cc53fe20a7116f93c21c7479be5a2a1d739495dbe44e in / 
# Wed, 26 Jan 2022 01:43:13 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 03:02:36 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 26 Jan 2022 03:03:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 03:04:03 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:20cc49690d9072283406c1c11e9b1dc1a247782cc8daa526b375d4a7f1cb6a94`  
		Last Modified: Wed, 26 Jan 2022 01:59:27 GMT  
		Size: 22.8 MB (22754397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242f21c9f2ea2b8610338b20aa4a933d07978910d00d961eb9395cf5ad6a14ba`  
		Last Modified: Wed, 26 Jan 2022 03:14:04 GMT  
		Size: 2.4 MB (2361950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf05b1bf44b0bc6e31c02c1f89b71c97d2120bd5088a235a9a2a58ccdc973e4`  
		Last Modified: Wed, 26 Jan 2022 03:14:20 GMT  
		Size: 23.8 MB (23782786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:2d8b961112b0f7f9c0cb6a334ffd574c95162bc7fa8d5b2aa366004f11c42d1e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57876030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:670158c5d1ee00bcf609d8daf07279a4093cc98203ef3362fc17510761426523`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:56 GMT
ADD file:796bc43a948899ba53bddebf7f613769fe96e8ea3a27eb7143d079c7a166ab01 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 04:54:45 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 26 Jan 2022 04:55:28 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 04:55:43 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4c7c9f6f1115fd4f35807a2f6c1375759365a991748aee0111873e55255f150b`  
		Last Modified: Wed, 26 Jan 2022 01:49:55 GMT  
		Size: 25.9 MB (25923216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145db9a792c54fdb1a14e3673d8bf7e6bfbdcfcd16e9f20670088dc797a755f9`  
		Last Modified: Wed, 26 Jan 2022 04:59:19 GMT  
		Size: 2.6 MB (2634624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba55b80938abbcaf307229652d0245d64085b55a6aa9db6572f5ac715e9d3959`  
		Last Modified: Wed, 26 Jan 2022 04:59:26 GMT  
		Size: 29.3 MB (29318190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; 386

```console
$ docker pull mono@sha256:d9c23198eec7e2c304b84f004811aa4baba762614a35374bd820ff5d24e3c378
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99364681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18db94f8442093daf5003e5853ae0b168af2ec80a3ed2a7babfbbd1dc3627d99`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:08:04 GMT
ADD file:d9d384f0402bc696e46e7529f52d64859a66aa7a60bca9c7beee7433a5f7af6e in / 
# Tue, 01 Mar 2022 02:08:04 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:13:49 GMT
ENV MONO_VERSION=6.12.0.122
# Tue, 01 Mar 2022 10:14:37 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 01 Mar 2022 10:15:09 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c761ce6f2bf0aed07e1198c6f827444969d6e76dda0e55dbb45900920e551d27`  
		Last Modified: Tue, 01 Mar 2022 02:16:51 GMT  
		Size: 27.8 MB (27804590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011b9d654300beab54b280fd3e0b1f7170919be5028f5e31a210af8a83500cfc`  
		Last Modified: Tue, 01 Mar 2022 10:22:39 GMT  
		Size: 2.8 MB (2781491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4b91a20a9ead3771e864dc94eb15af13cf873e35ca6bbc27fe1fdd66f0422f`  
		Last Modified: Tue, 01 Mar 2022 10:23:02 GMT  
		Size: 68.8 MB (68778600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; ppc64le

```console
$ docker pull mono@sha256:d575747ba8940111c62f95739e8a754b9b87078977fba75f2e18524deb22a8a2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.3 MB (60320965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e081680305b9949003bab588e040386a8353300452f2a819aae1a529471cea28`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:47:48 GMT
ADD file:d87bdffbd9392364fecbbd4148c710bc4948073e773a47c7b9ac1440ebb81c1e in / 
# Wed, 26 Jan 2022 01:47:52 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 05:16:29 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 26 Jan 2022 05:17:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 26 Jan 2022 05:19:13 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:249357001395b3de58d51723447880f3205d37ea7b902930b5c19f475d4ac8f9`  
		Last Modified: Wed, 26 Jan 2022 01:58:50 GMT  
		Size: 30.6 MB (30562293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b424ab5d806f162b76c369311f6e539940178ab8b306c053879a77ff4a77d4`  
		Last Modified: Wed, 26 Jan 2022 05:36:07 GMT  
		Size: 2.9 MB (2884629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7982f75341da8b4f46a0677a86d66dfaa5a4b464e669fc85629e0bf531fa21`  
		Last Modified: Wed, 26 Jan 2022 05:36:13 GMT  
		Size: 26.9 MB (26874043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
