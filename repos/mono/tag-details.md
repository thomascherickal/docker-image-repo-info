<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mono`

-	[`mono:6`](#mono6)
-	[`mono:6.10`](#mono610)
-	[`mono:6.10.0`](#mono6100)
-	[`mono:6.10.0.104`](#mono6100104)
-	[`mono:6.10.0.104-slim`](#mono6100104-slim)
-	[`mono:6.10.0-slim`](#mono6100-slim)
-	[`mono:6.10-slim`](#mono610-slim)
-	[`mono:6.8`](#mono68)
-	[`mono:6.8.0`](#mono680)
-	[`mono:6.8.0.123`](#mono680123)
-	[`mono:6.8.0.123-slim`](#mono680123-slim)
-	[`mono:6.8.0-slim`](#mono680-slim)
-	[`mono:6.8-slim`](#mono68-slim)
-	[`mono:6-slim`](#mono6-slim)
-	[`mono:latest`](#monolatest)
-	[`mono:slim`](#monoslim)

## `mono:6`

```console
$ docker pull mono@sha256:21a4e78b865656f518c7b14ed1b839c7cb188a133a3375ab9a27ac7efa8b6239
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
$ docker pull mono@sha256:c4118ed710f19848f2f29877a06271e11cfc3577e23c0018360a4cb347da404e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.0 MB (235018613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13d1331c323d17d5bd48ce6ff2e86f956687ec264d9d39f96bd0b6714de6272e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:07:07 GMT
ADD file:c11db0b135382f4c5b0f55b50740639bd8c1a22153b931b409cb9e41136734f2 in / 
# Wed, 22 Jul 2020 02:07:07 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 19:26:50 GMT
ENV MONO_VERSION=6.8.0.96
# Wed, 22 Jul 2020 19:26:59 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 22 Jul 2020 19:27:42 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 22 Jul 2020 19:40:41 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:cbd31ae332794bb723708526045b062b2fe6a08ccc0f143ea7dc18e0ebe46dea`  
		Last Modified: Wed, 22 Jul 2020 02:12:25 GMT  
		Size: 22.5 MB (22515635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fa40bfbf0082f2bae5777ccd52f3ca2add17d21a2375de40cb7b6a738aee92a`  
		Last Modified: Wed, 22 Jul 2020 20:02:10 GMT  
		Size: 244.5 KB (244495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989dabcb56d661ce7dac9d54d0c22d40088fb13ced11ca7807786cd9cd61431d`  
		Last Modified: Wed, 22 Jul 2020 20:02:28 GMT  
		Size: 64.5 MB (64467293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e08265401bb5017665068ac267affc91b2e11ffe852bd9b9d73572f1ebdede`  
		Last Modified: Wed, 22 Jul 2020 20:03:51 GMT  
		Size: 147.8 MB (147791190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; arm variant v5

```console
$ docker pull mono@sha256:d216197c3136cf659053d08e0eb5d8f3961128d38d9893e9f8b19e7bddf3c51c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180580599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e9781e28afc6ae2bd019f175f92455997398b3d6b80688994a75f6b4acbb27f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:51:01 GMT
ADD file:4ea2d111c970d510f4eccf0fa08caafde1d227fc4c249d67c1b9d99998b0b906 in / 
# Wed, 22 Jul 2020 00:51:04 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 21:12:42 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 22 Jul 2020 21:13:14 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 22 Jul 2020 21:14:39 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 22 Jul 2020 21:20:33 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7ae4223cfc253e8d54407ec654ed8fb606352daea8da124f33dacd17626259ad`  
		Last Modified: Wed, 22 Jul 2020 00:58:53 GMT  
		Size: 24.8 MB (24837461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b201b7c93f2f75a8f765155e3fd569dbc95a79c57c644b4595e1eff9afe8e9`  
		Last Modified: Wed, 22 Jul 2020 21:21:16 GMT  
		Size: 256.0 KB (255977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47783e7ea018044b2c75ce172154e65072809be55a95a291093f770a8c261e75`  
		Last Modified: Wed, 22 Jul 2020 21:21:27 GMT  
		Size: 26.5 MB (26529324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9bba9be5aff5dfd8562a172dd933fd2bddcdbfc9c5cf46797c28e7f1d276576`  
		Last Modified: Wed, 22 Jul 2020 21:23:21 GMT  
		Size: 129.0 MB (128957837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; arm variant v7

```console
$ docker pull mono@sha256:0e79b73ff74791117dd0a42084eee5040160bdfa1d76e7e4cf2ffdd2b18b3cb9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.6 MB (172599115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a12c1996dc94982e4e9871cb355f1304e8c978c416bef75350d2fc25fb5fcad2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 01:33:30 GMT
ADD file:49b1a1b4f5c2201b0e23e29dca24c4f6ffc14620196c4bd77770952500c4bee1 in / 
# Wed, 22 Jul 2020 01:33:38 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 02:15:12 GMT
ENV MONO_VERSION=6.8.0.96
# Wed, 22 Jul 2020 02:15:59 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 22 Jul 2020 02:17:08 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 22 Jul 2020 02:24:59 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:cd38ad753522d120e27c5343b08f661ee3aebfe531d60102d7c624c16dba4d09`  
		Last Modified: Wed, 22 Jul 2020 01:44:24 GMT  
		Size: 19.3 MB (19298267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678b77b1123ed730afaccee19cb50f8fdf077e6011636b04af9cd365e6ebdf13`  
		Last Modified: Wed, 22 Jul 2020 02:32:32 GMT  
		Size: 244.6 KB (244569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ee2966b2ed591a8caba8af3012b33613fdcd2925dffc5f9eaa9328292c5af9`  
		Last Modified: Wed, 22 Jul 2020 02:32:40 GMT  
		Size: 24.5 MB (24495473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156d85b212d8926604522d94038ef09d4862f7a5aebd52d8f0c5e9546ef12c06`  
		Last Modified: Wed, 22 Jul 2020 02:34:24 GMT  
		Size: 128.6 MB (128560806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:5b229ee910d41136f26b4fb24e774ce778751f846e023acfd13481f13aaf480b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.3 MB (203299242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38c4746a1607b1fea5aedd8e27f9cd4cf4b52d846b634e1593a5deccdac7600f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:41:09 GMT
ADD file:1efd5b51a56f36bcf79a1bcea1df36ef28299a42bc11e758f9e49066f2a1f085 in / 
# Wed, 22 Jul 2020 00:41:10 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 05:21:19 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 23 Jul 2020 05:21:40 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 05:22:18 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 23 Jul 2020 05:27:01 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3999339def4d7591a8064bfc698302ae0e29bc5e0557ae392c122e1b3efa9305`  
		Last Modified: Wed, 22 Jul 2020 00:47:42 GMT  
		Size: 25.9 MB (25857826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072a4eb4e02ed79a5f02c37ff3909423a2376488a8c9f16c1d2a94ac58359078`  
		Last Modified: Thu, 23 Jul 2020 05:27:50 GMT  
		Size: 255.9 KB (255908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfeb41b8c951ba90f625eda71258c0aa6098d6281c21319a2db7cdf691d34fc`  
		Last Modified: Thu, 23 Jul 2020 05:28:00 GMT  
		Size: 31.7 MB (31748118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34df94ccaa6daaeb0c5cce32d31458a2550823303e09ca160f143178cd78a3ec`  
		Last Modified: Thu, 23 Jul 2020 05:29:48 GMT  
		Size: 145.4 MB (145437390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; 386

```console
$ docker pull mono@sha256:104b3ad8a26e6ce2f6829d32b6a39ae39bb6c586c0ae5fc2b6dee6cf6b40a3d8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.5 MB (230542185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f7e6a79136b95af481af9503fdaaa4cb19dc983225e59b060f2effacbf3878b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:09:15 GMT
ADD file:ee51bd8fcf2e02243de32c0f0e7899acebfa23bdceb783f13feb33c484ee98b8 in / 
# Wed, 22 Jul 2020 02:09:15 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 00:17:56 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 23 Jul 2020 00:18:08 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 00:18:59 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 23 Jul 2020 00:24:07 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:75157e9ef5a857d6b02d235e08a164737ad009bae299277f86131063e6204e0b`  
		Last Modified: Wed, 22 Jul 2020 02:15:45 GMT  
		Size: 27.8 MB (27754899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf3d2401f59eb0e901a248e7de7b81f6d0ce70dc8958450d9406575c5ae402a`  
		Last Modified: Thu, 23 Jul 2020 00:24:53 GMT  
		Size: 255.9 KB (255866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49c7cc3cfa683a1a7f140766f83ef1205f003c8f18a9e7dc6192211af762bdd`  
		Last Modified: Thu, 23 Jul 2020 00:25:12 GMT  
		Size: 71.1 MB (71134676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4814f34046c756d82b2e0956d1226d8adf44644864681f318e6d3cc6c3276b1a`  
		Last Modified: Thu, 23 Jul 2020 00:26:45 GMT  
		Size: 131.4 MB (131396744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; ppc64le

```console
$ docker pull mono@sha256:d869978f01d503070bd620fdbd1e1f69c88d9749580f61d4b81cf818f4c6958d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.1 MB (192091144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d9744232b7d0bd9e597e8dfaaf5e81c9ee17bc9a6fff9cf4b633939d80230fc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:16:05 GMT
ADD file:037dec996d9b742fc49f675272aa42ebd31f04226ba3d28836a6556cb61c29e7 in / 
# Wed, 22 Jul 2020 02:16:14 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 06:10:34 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 23 Jul 2020 06:12:20 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 06:14:21 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 23 Jul 2020 06:58:00 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d022338f917106731b8902d4c3d7009435a41381c11c8d210bbd6af007569f69`  
		Last Modified: Wed, 22 Jul 2020 02:26:01 GMT  
		Size: 30.5 MB (30524562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a35a0ce279229326ca6a3a4114458fe3e7a42a86875ae4b3f3e6a8a914127f`  
		Last Modified: Thu, 23 Jul 2020 06:59:10 GMT  
		Size: 256.2 KB (256204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c409da6637fbd5bae065a688f5b8fa5bca60053859e7f816079c977f9193411c`  
		Last Modified: Thu, 23 Jul 2020 06:59:18 GMT  
		Size: 29.3 MB (29349424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857181e3045e28d43363265a023c6a51347e982d06b1ce96ce27aae83e425231`  
		Last Modified: Thu, 23 Jul 2020 07:00:47 GMT  
		Size: 132.0 MB (131960954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10`

```console
$ docker pull mono@sha256:88d400dde06a820dc847629438ce7eb7d99515384796650419ae38973a10285c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v5
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.10` - linux; arm variant v5

```console
$ docker pull mono@sha256:d216197c3136cf659053d08e0eb5d8f3961128d38d9893e9f8b19e7bddf3c51c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180580599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e9781e28afc6ae2bd019f175f92455997398b3d6b80688994a75f6b4acbb27f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:51:01 GMT
ADD file:4ea2d111c970d510f4eccf0fa08caafde1d227fc4c249d67c1b9d99998b0b906 in / 
# Wed, 22 Jul 2020 00:51:04 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 21:12:42 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 22 Jul 2020 21:13:14 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 22 Jul 2020 21:14:39 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 22 Jul 2020 21:20:33 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7ae4223cfc253e8d54407ec654ed8fb606352daea8da124f33dacd17626259ad`  
		Last Modified: Wed, 22 Jul 2020 00:58:53 GMT  
		Size: 24.8 MB (24837461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b201b7c93f2f75a8f765155e3fd569dbc95a79c57c644b4595e1eff9afe8e9`  
		Last Modified: Wed, 22 Jul 2020 21:21:16 GMT  
		Size: 256.0 KB (255977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47783e7ea018044b2c75ce172154e65072809be55a95a291093f770a8c261e75`  
		Last Modified: Wed, 22 Jul 2020 21:21:27 GMT  
		Size: 26.5 MB (26529324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9bba9be5aff5dfd8562a172dd933fd2bddcdbfc9c5cf46797c28e7f1d276576`  
		Last Modified: Wed, 22 Jul 2020 21:23:21 GMT  
		Size: 129.0 MB (128957837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:5b229ee910d41136f26b4fb24e774ce778751f846e023acfd13481f13aaf480b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.3 MB (203299242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38c4746a1607b1fea5aedd8e27f9cd4cf4b52d846b634e1593a5deccdac7600f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:41:09 GMT
ADD file:1efd5b51a56f36bcf79a1bcea1df36ef28299a42bc11e758f9e49066f2a1f085 in / 
# Wed, 22 Jul 2020 00:41:10 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 05:21:19 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 23 Jul 2020 05:21:40 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 05:22:18 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 23 Jul 2020 05:27:01 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3999339def4d7591a8064bfc698302ae0e29bc5e0557ae392c122e1b3efa9305`  
		Last Modified: Wed, 22 Jul 2020 00:47:42 GMT  
		Size: 25.9 MB (25857826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072a4eb4e02ed79a5f02c37ff3909423a2376488a8c9f16c1d2a94ac58359078`  
		Last Modified: Thu, 23 Jul 2020 05:27:50 GMT  
		Size: 255.9 KB (255908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfeb41b8c951ba90f625eda71258c0aa6098d6281c21319a2db7cdf691d34fc`  
		Last Modified: Thu, 23 Jul 2020 05:28:00 GMT  
		Size: 31.7 MB (31748118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34df94ccaa6daaeb0c5cce32d31458a2550823303e09ca160f143178cd78a3ec`  
		Last Modified: Thu, 23 Jul 2020 05:29:48 GMT  
		Size: 145.4 MB (145437390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; 386

```console
$ docker pull mono@sha256:104b3ad8a26e6ce2f6829d32b6a39ae39bb6c586c0ae5fc2b6dee6cf6b40a3d8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.5 MB (230542185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f7e6a79136b95af481af9503fdaaa4cb19dc983225e59b060f2effacbf3878b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:09:15 GMT
ADD file:ee51bd8fcf2e02243de32c0f0e7899acebfa23bdceb783f13feb33c484ee98b8 in / 
# Wed, 22 Jul 2020 02:09:15 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 00:17:56 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 23 Jul 2020 00:18:08 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 00:18:59 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 23 Jul 2020 00:24:07 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:75157e9ef5a857d6b02d235e08a164737ad009bae299277f86131063e6204e0b`  
		Last Modified: Wed, 22 Jul 2020 02:15:45 GMT  
		Size: 27.8 MB (27754899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf3d2401f59eb0e901a248e7de7b81f6d0ce70dc8958450d9406575c5ae402a`  
		Last Modified: Thu, 23 Jul 2020 00:24:53 GMT  
		Size: 255.9 KB (255866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49c7cc3cfa683a1a7f140766f83ef1205f003c8f18a9e7dc6192211af762bdd`  
		Last Modified: Thu, 23 Jul 2020 00:25:12 GMT  
		Size: 71.1 MB (71134676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4814f34046c756d82b2e0956d1226d8adf44644864681f318e6d3cc6c3276b1a`  
		Last Modified: Thu, 23 Jul 2020 00:26:45 GMT  
		Size: 131.4 MB (131396744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; ppc64le

```console
$ docker pull mono@sha256:d869978f01d503070bd620fdbd1e1f69c88d9749580f61d4b81cf818f4c6958d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.1 MB (192091144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d9744232b7d0bd9e597e8dfaaf5e81c9ee17bc9a6fff9cf4b633939d80230fc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:16:05 GMT
ADD file:037dec996d9b742fc49f675272aa42ebd31f04226ba3d28836a6556cb61c29e7 in / 
# Wed, 22 Jul 2020 02:16:14 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 06:10:34 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 23 Jul 2020 06:12:20 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 06:14:21 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 23 Jul 2020 06:58:00 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d022338f917106731b8902d4c3d7009435a41381c11c8d210bbd6af007569f69`  
		Last Modified: Wed, 22 Jul 2020 02:26:01 GMT  
		Size: 30.5 MB (30524562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a35a0ce279229326ca6a3a4114458fe3e7a42a86875ae4b3f3e6a8a914127f`  
		Last Modified: Thu, 23 Jul 2020 06:59:10 GMT  
		Size: 256.2 KB (256204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c409da6637fbd5bae065a688f5b8fa5bca60053859e7f816079c977f9193411c`  
		Last Modified: Thu, 23 Jul 2020 06:59:18 GMT  
		Size: 29.3 MB (29349424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857181e3045e28d43363265a023c6a51347e982d06b1ce96ce27aae83e425231`  
		Last Modified: Thu, 23 Jul 2020 07:00:47 GMT  
		Size: 132.0 MB (131960954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10.0`

```console
$ docker pull mono@sha256:88d400dde06a820dc847629438ce7eb7d99515384796650419ae38973a10285c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v5
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.10.0` - linux; arm variant v5

```console
$ docker pull mono@sha256:d216197c3136cf659053d08e0eb5d8f3961128d38d9893e9f8b19e7bddf3c51c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180580599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e9781e28afc6ae2bd019f175f92455997398b3d6b80688994a75f6b4acbb27f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:51:01 GMT
ADD file:4ea2d111c970d510f4eccf0fa08caafde1d227fc4c249d67c1b9d99998b0b906 in / 
# Wed, 22 Jul 2020 00:51:04 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 21:12:42 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 22 Jul 2020 21:13:14 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 22 Jul 2020 21:14:39 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 22 Jul 2020 21:20:33 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7ae4223cfc253e8d54407ec654ed8fb606352daea8da124f33dacd17626259ad`  
		Last Modified: Wed, 22 Jul 2020 00:58:53 GMT  
		Size: 24.8 MB (24837461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b201b7c93f2f75a8f765155e3fd569dbc95a79c57c644b4595e1eff9afe8e9`  
		Last Modified: Wed, 22 Jul 2020 21:21:16 GMT  
		Size: 256.0 KB (255977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47783e7ea018044b2c75ce172154e65072809be55a95a291093f770a8c261e75`  
		Last Modified: Wed, 22 Jul 2020 21:21:27 GMT  
		Size: 26.5 MB (26529324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9bba9be5aff5dfd8562a172dd933fd2bddcdbfc9c5cf46797c28e7f1d276576`  
		Last Modified: Wed, 22 Jul 2020 21:23:21 GMT  
		Size: 129.0 MB (128957837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:5b229ee910d41136f26b4fb24e774ce778751f846e023acfd13481f13aaf480b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.3 MB (203299242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38c4746a1607b1fea5aedd8e27f9cd4cf4b52d846b634e1593a5deccdac7600f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:41:09 GMT
ADD file:1efd5b51a56f36bcf79a1bcea1df36ef28299a42bc11e758f9e49066f2a1f085 in / 
# Wed, 22 Jul 2020 00:41:10 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 05:21:19 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 23 Jul 2020 05:21:40 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 05:22:18 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 23 Jul 2020 05:27:01 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3999339def4d7591a8064bfc698302ae0e29bc5e0557ae392c122e1b3efa9305`  
		Last Modified: Wed, 22 Jul 2020 00:47:42 GMT  
		Size: 25.9 MB (25857826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072a4eb4e02ed79a5f02c37ff3909423a2376488a8c9f16c1d2a94ac58359078`  
		Last Modified: Thu, 23 Jul 2020 05:27:50 GMT  
		Size: 255.9 KB (255908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfeb41b8c951ba90f625eda71258c0aa6098d6281c21319a2db7cdf691d34fc`  
		Last Modified: Thu, 23 Jul 2020 05:28:00 GMT  
		Size: 31.7 MB (31748118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34df94ccaa6daaeb0c5cce32d31458a2550823303e09ca160f143178cd78a3ec`  
		Last Modified: Thu, 23 Jul 2020 05:29:48 GMT  
		Size: 145.4 MB (145437390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; 386

```console
$ docker pull mono@sha256:104b3ad8a26e6ce2f6829d32b6a39ae39bb6c586c0ae5fc2b6dee6cf6b40a3d8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.5 MB (230542185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f7e6a79136b95af481af9503fdaaa4cb19dc983225e59b060f2effacbf3878b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:09:15 GMT
ADD file:ee51bd8fcf2e02243de32c0f0e7899acebfa23bdceb783f13feb33c484ee98b8 in / 
# Wed, 22 Jul 2020 02:09:15 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 00:17:56 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 23 Jul 2020 00:18:08 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 00:18:59 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 23 Jul 2020 00:24:07 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:75157e9ef5a857d6b02d235e08a164737ad009bae299277f86131063e6204e0b`  
		Last Modified: Wed, 22 Jul 2020 02:15:45 GMT  
		Size: 27.8 MB (27754899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf3d2401f59eb0e901a248e7de7b81f6d0ce70dc8958450d9406575c5ae402a`  
		Last Modified: Thu, 23 Jul 2020 00:24:53 GMT  
		Size: 255.9 KB (255866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49c7cc3cfa683a1a7f140766f83ef1205f003c8f18a9e7dc6192211af762bdd`  
		Last Modified: Thu, 23 Jul 2020 00:25:12 GMT  
		Size: 71.1 MB (71134676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4814f34046c756d82b2e0956d1226d8adf44644864681f318e6d3cc6c3276b1a`  
		Last Modified: Thu, 23 Jul 2020 00:26:45 GMT  
		Size: 131.4 MB (131396744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; ppc64le

```console
$ docker pull mono@sha256:d869978f01d503070bd620fdbd1e1f69c88d9749580f61d4b81cf818f4c6958d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.1 MB (192091144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d9744232b7d0bd9e597e8dfaaf5e81c9ee17bc9a6fff9cf4b633939d80230fc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:16:05 GMT
ADD file:037dec996d9b742fc49f675272aa42ebd31f04226ba3d28836a6556cb61c29e7 in / 
# Wed, 22 Jul 2020 02:16:14 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 06:10:34 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 23 Jul 2020 06:12:20 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 06:14:21 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 23 Jul 2020 06:58:00 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d022338f917106731b8902d4c3d7009435a41381c11c8d210bbd6af007569f69`  
		Last Modified: Wed, 22 Jul 2020 02:26:01 GMT  
		Size: 30.5 MB (30524562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a35a0ce279229326ca6a3a4114458fe3e7a42a86875ae4b3f3e6a8a914127f`  
		Last Modified: Thu, 23 Jul 2020 06:59:10 GMT  
		Size: 256.2 KB (256204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c409da6637fbd5bae065a688f5b8fa5bca60053859e7f816079c977f9193411c`  
		Last Modified: Thu, 23 Jul 2020 06:59:18 GMT  
		Size: 29.3 MB (29349424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857181e3045e28d43363265a023c6a51347e982d06b1ce96ce27aae83e425231`  
		Last Modified: Thu, 23 Jul 2020 07:00:47 GMT  
		Size: 132.0 MB (131960954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10.0.104`

```console
$ docker pull mono@sha256:88d400dde06a820dc847629438ce7eb7d99515384796650419ae38973a10285c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v5
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.10.0.104` - linux; arm variant v5

```console
$ docker pull mono@sha256:d216197c3136cf659053d08e0eb5d8f3961128d38d9893e9f8b19e7bddf3c51c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180580599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e9781e28afc6ae2bd019f175f92455997398b3d6b80688994a75f6b4acbb27f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:51:01 GMT
ADD file:4ea2d111c970d510f4eccf0fa08caafde1d227fc4c249d67c1b9d99998b0b906 in / 
# Wed, 22 Jul 2020 00:51:04 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 21:12:42 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 22 Jul 2020 21:13:14 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 22 Jul 2020 21:14:39 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 22 Jul 2020 21:20:33 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7ae4223cfc253e8d54407ec654ed8fb606352daea8da124f33dacd17626259ad`  
		Last Modified: Wed, 22 Jul 2020 00:58:53 GMT  
		Size: 24.8 MB (24837461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b201b7c93f2f75a8f765155e3fd569dbc95a79c57c644b4595e1eff9afe8e9`  
		Last Modified: Wed, 22 Jul 2020 21:21:16 GMT  
		Size: 256.0 KB (255977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47783e7ea018044b2c75ce172154e65072809be55a95a291093f770a8c261e75`  
		Last Modified: Wed, 22 Jul 2020 21:21:27 GMT  
		Size: 26.5 MB (26529324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9bba9be5aff5dfd8562a172dd933fd2bddcdbfc9c5cf46797c28e7f1d276576`  
		Last Modified: Wed, 22 Jul 2020 21:23:21 GMT  
		Size: 129.0 MB (128957837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:5b229ee910d41136f26b4fb24e774ce778751f846e023acfd13481f13aaf480b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.3 MB (203299242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38c4746a1607b1fea5aedd8e27f9cd4cf4b52d846b634e1593a5deccdac7600f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:41:09 GMT
ADD file:1efd5b51a56f36bcf79a1bcea1df36ef28299a42bc11e758f9e49066f2a1f085 in / 
# Wed, 22 Jul 2020 00:41:10 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 05:21:19 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 23 Jul 2020 05:21:40 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 05:22:18 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 23 Jul 2020 05:27:01 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3999339def4d7591a8064bfc698302ae0e29bc5e0557ae392c122e1b3efa9305`  
		Last Modified: Wed, 22 Jul 2020 00:47:42 GMT  
		Size: 25.9 MB (25857826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072a4eb4e02ed79a5f02c37ff3909423a2376488a8c9f16c1d2a94ac58359078`  
		Last Modified: Thu, 23 Jul 2020 05:27:50 GMT  
		Size: 255.9 KB (255908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfeb41b8c951ba90f625eda71258c0aa6098d6281c21319a2db7cdf691d34fc`  
		Last Modified: Thu, 23 Jul 2020 05:28:00 GMT  
		Size: 31.7 MB (31748118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34df94ccaa6daaeb0c5cce32d31458a2550823303e09ca160f143178cd78a3ec`  
		Last Modified: Thu, 23 Jul 2020 05:29:48 GMT  
		Size: 145.4 MB (145437390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; 386

```console
$ docker pull mono@sha256:104b3ad8a26e6ce2f6829d32b6a39ae39bb6c586c0ae5fc2b6dee6cf6b40a3d8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.5 MB (230542185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f7e6a79136b95af481af9503fdaaa4cb19dc983225e59b060f2effacbf3878b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:09:15 GMT
ADD file:ee51bd8fcf2e02243de32c0f0e7899acebfa23bdceb783f13feb33c484ee98b8 in / 
# Wed, 22 Jul 2020 02:09:15 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 00:17:56 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 23 Jul 2020 00:18:08 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 00:18:59 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 23 Jul 2020 00:24:07 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:75157e9ef5a857d6b02d235e08a164737ad009bae299277f86131063e6204e0b`  
		Last Modified: Wed, 22 Jul 2020 02:15:45 GMT  
		Size: 27.8 MB (27754899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf3d2401f59eb0e901a248e7de7b81f6d0ce70dc8958450d9406575c5ae402a`  
		Last Modified: Thu, 23 Jul 2020 00:24:53 GMT  
		Size: 255.9 KB (255866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49c7cc3cfa683a1a7f140766f83ef1205f003c8f18a9e7dc6192211af762bdd`  
		Last Modified: Thu, 23 Jul 2020 00:25:12 GMT  
		Size: 71.1 MB (71134676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4814f34046c756d82b2e0956d1226d8adf44644864681f318e6d3cc6c3276b1a`  
		Last Modified: Thu, 23 Jul 2020 00:26:45 GMT  
		Size: 131.4 MB (131396744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; ppc64le

```console
$ docker pull mono@sha256:d869978f01d503070bd620fdbd1e1f69c88d9749580f61d4b81cf818f4c6958d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.1 MB (192091144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d9744232b7d0bd9e597e8dfaaf5e81c9ee17bc9a6fff9cf4b633939d80230fc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:16:05 GMT
ADD file:037dec996d9b742fc49f675272aa42ebd31f04226ba3d28836a6556cb61c29e7 in / 
# Wed, 22 Jul 2020 02:16:14 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 06:10:34 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 23 Jul 2020 06:12:20 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 06:14:21 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 23 Jul 2020 06:58:00 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d022338f917106731b8902d4c3d7009435a41381c11c8d210bbd6af007569f69`  
		Last Modified: Wed, 22 Jul 2020 02:26:01 GMT  
		Size: 30.5 MB (30524562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a35a0ce279229326ca6a3a4114458fe3e7a42a86875ae4b3f3e6a8a914127f`  
		Last Modified: Thu, 23 Jul 2020 06:59:10 GMT  
		Size: 256.2 KB (256204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c409da6637fbd5bae065a688f5b8fa5bca60053859e7f816079c977f9193411c`  
		Last Modified: Thu, 23 Jul 2020 06:59:18 GMT  
		Size: 29.3 MB (29349424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857181e3045e28d43363265a023c6a51347e982d06b1ce96ce27aae83e425231`  
		Last Modified: Thu, 23 Jul 2020 07:00:47 GMT  
		Size: 132.0 MB (131960954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10.0.104-slim`

```console
$ docker pull mono@sha256:1329f019558cff676a9d8531f5cc4a7f558b8cda33b11f1809f6ccd2c14618f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v5
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.10.0.104-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:bfbf7d0dd6ec900bd4fb046e1171472d0cc6b4bc32c10095bcc1718d0d2fb4f3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51622762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0887bb40baf7e1ebaa4491740009839e418df248c2f18e393048574e7a3283aa`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:51:01 GMT
ADD file:4ea2d111c970d510f4eccf0fa08caafde1d227fc4c249d67c1b9d99998b0b906 in / 
# Wed, 22 Jul 2020 00:51:04 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 21:12:42 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 22 Jul 2020 21:13:14 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 22 Jul 2020 21:14:39 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7ae4223cfc253e8d54407ec654ed8fb606352daea8da124f33dacd17626259ad`  
		Last Modified: Wed, 22 Jul 2020 00:58:53 GMT  
		Size: 24.8 MB (24837461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b201b7c93f2f75a8f765155e3fd569dbc95a79c57c644b4595e1eff9afe8e9`  
		Last Modified: Wed, 22 Jul 2020 21:21:16 GMT  
		Size: 256.0 KB (255977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47783e7ea018044b2c75ce172154e65072809be55a95a291093f770a8c261e75`  
		Last Modified: Wed, 22 Jul 2020 21:21:27 GMT  
		Size: 26.5 MB (26529324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:90c6e2ff8ea8544e22e0263aff48c2e93d9b0d5744988b3450b239c9a01bce98
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57861852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9eaeca8f8945189ca2b07c8c7261bb0dcfea6c27e322fe4f79f9e4bbb082dbb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:41:09 GMT
ADD file:1efd5b51a56f36bcf79a1bcea1df36ef28299a42bc11e758f9e49066f2a1f085 in / 
# Wed, 22 Jul 2020 00:41:10 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 05:21:19 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 23 Jul 2020 05:21:40 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 05:22:18 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3999339def4d7591a8064bfc698302ae0e29bc5e0557ae392c122e1b3efa9305`  
		Last Modified: Wed, 22 Jul 2020 00:47:42 GMT  
		Size: 25.9 MB (25857826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072a4eb4e02ed79a5f02c37ff3909423a2376488a8c9f16c1d2a94ac58359078`  
		Last Modified: Thu, 23 Jul 2020 05:27:50 GMT  
		Size: 255.9 KB (255908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfeb41b8c951ba90f625eda71258c0aa6098d6281c21319a2db7cdf691d34fc`  
		Last Modified: Thu, 23 Jul 2020 05:28:00 GMT  
		Size: 31.7 MB (31748118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; 386

```console
$ docker pull mono@sha256:832edc5e755243979388a770f2a26b002ff53970f4d5980d4646408b83977600
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99145441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0acbbfdbc517756895fa8f98bd81276148a67102797ffbda89f1c47569e381a4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:09:15 GMT
ADD file:ee51bd8fcf2e02243de32c0f0e7899acebfa23bdceb783f13feb33c484ee98b8 in / 
# Wed, 22 Jul 2020 02:09:15 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 00:17:56 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 23 Jul 2020 00:18:08 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 00:18:59 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:75157e9ef5a857d6b02d235e08a164737ad009bae299277f86131063e6204e0b`  
		Last Modified: Wed, 22 Jul 2020 02:15:45 GMT  
		Size: 27.8 MB (27754899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf3d2401f59eb0e901a248e7de7b81f6d0ce70dc8958450d9406575c5ae402a`  
		Last Modified: Thu, 23 Jul 2020 00:24:53 GMT  
		Size: 255.9 KB (255866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49c7cc3cfa683a1a7f140766f83ef1205f003c8f18a9e7dc6192211af762bdd`  
		Last Modified: Thu, 23 Jul 2020 00:25:12 GMT  
		Size: 71.1 MB (71134676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:305c285592ef4afd7c1e21fc7f28ec09f07868e0d8f8fad13e56251960215f56
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60130190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe7500199f77ce97cf00689537fd03120b78b47c57f1894538baaf0659deafc3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:16:05 GMT
ADD file:037dec996d9b742fc49f675272aa42ebd31f04226ba3d28836a6556cb61c29e7 in / 
# Wed, 22 Jul 2020 02:16:14 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 06:10:34 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 23 Jul 2020 06:12:20 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 06:14:21 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d022338f917106731b8902d4c3d7009435a41381c11c8d210bbd6af007569f69`  
		Last Modified: Wed, 22 Jul 2020 02:26:01 GMT  
		Size: 30.5 MB (30524562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a35a0ce279229326ca6a3a4114458fe3e7a42a86875ae4b3f3e6a8a914127f`  
		Last Modified: Thu, 23 Jul 2020 06:59:10 GMT  
		Size: 256.2 KB (256204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c409da6637fbd5bae065a688f5b8fa5bca60053859e7f816079c977f9193411c`  
		Last Modified: Thu, 23 Jul 2020 06:59:18 GMT  
		Size: 29.3 MB (29349424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10.0-slim`

```console
$ docker pull mono@sha256:1329f019558cff676a9d8531f5cc4a7f558b8cda33b11f1809f6ccd2c14618f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v5
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.10.0-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:bfbf7d0dd6ec900bd4fb046e1171472d0cc6b4bc32c10095bcc1718d0d2fb4f3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51622762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0887bb40baf7e1ebaa4491740009839e418df248c2f18e393048574e7a3283aa`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:51:01 GMT
ADD file:4ea2d111c970d510f4eccf0fa08caafde1d227fc4c249d67c1b9d99998b0b906 in / 
# Wed, 22 Jul 2020 00:51:04 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 21:12:42 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 22 Jul 2020 21:13:14 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 22 Jul 2020 21:14:39 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7ae4223cfc253e8d54407ec654ed8fb606352daea8da124f33dacd17626259ad`  
		Last Modified: Wed, 22 Jul 2020 00:58:53 GMT  
		Size: 24.8 MB (24837461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b201b7c93f2f75a8f765155e3fd569dbc95a79c57c644b4595e1eff9afe8e9`  
		Last Modified: Wed, 22 Jul 2020 21:21:16 GMT  
		Size: 256.0 KB (255977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47783e7ea018044b2c75ce172154e65072809be55a95a291093f770a8c261e75`  
		Last Modified: Wed, 22 Jul 2020 21:21:27 GMT  
		Size: 26.5 MB (26529324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:90c6e2ff8ea8544e22e0263aff48c2e93d9b0d5744988b3450b239c9a01bce98
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57861852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9eaeca8f8945189ca2b07c8c7261bb0dcfea6c27e322fe4f79f9e4bbb082dbb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:41:09 GMT
ADD file:1efd5b51a56f36bcf79a1bcea1df36ef28299a42bc11e758f9e49066f2a1f085 in / 
# Wed, 22 Jul 2020 00:41:10 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 05:21:19 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 23 Jul 2020 05:21:40 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 05:22:18 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3999339def4d7591a8064bfc698302ae0e29bc5e0557ae392c122e1b3efa9305`  
		Last Modified: Wed, 22 Jul 2020 00:47:42 GMT  
		Size: 25.9 MB (25857826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072a4eb4e02ed79a5f02c37ff3909423a2376488a8c9f16c1d2a94ac58359078`  
		Last Modified: Thu, 23 Jul 2020 05:27:50 GMT  
		Size: 255.9 KB (255908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfeb41b8c951ba90f625eda71258c0aa6098d6281c21319a2db7cdf691d34fc`  
		Last Modified: Thu, 23 Jul 2020 05:28:00 GMT  
		Size: 31.7 MB (31748118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; 386

```console
$ docker pull mono@sha256:832edc5e755243979388a770f2a26b002ff53970f4d5980d4646408b83977600
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99145441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0acbbfdbc517756895fa8f98bd81276148a67102797ffbda89f1c47569e381a4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:09:15 GMT
ADD file:ee51bd8fcf2e02243de32c0f0e7899acebfa23bdceb783f13feb33c484ee98b8 in / 
# Wed, 22 Jul 2020 02:09:15 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 00:17:56 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 23 Jul 2020 00:18:08 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 00:18:59 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:75157e9ef5a857d6b02d235e08a164737ad009bae299277f86131063e6204e0b`  
		Last Modified: Wed, 22 Jul 2020 02:15:45 GMT  
		Size: 27.8 MB (27754899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf3d2401f59eb0e901a248e7de7b81f6d0ce70dc8958450d9406575c5ae402a`  
		Last Modified: Thu, 23 Jul 2020 00:24:53 GMT  
		Size: 255.9 KB (255866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49c7cc3cfa683a1a7f140766f83ef1205f003c8f18a9e7dc6192211af762bdd`  
		Last Modified: Thu, 23 Jul 2020 00:25:12 GMT  
		Size: 71.1 MB (71134676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:305c285592ef4afd7c1e21fc7f28ec09f07868e0d8f8fad13e56251960215f56
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60130190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe7500199f77ce97cf00689537fd03120b78b47c57f1894538baaf0659deafc3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:16:05 GMT
ADD file:037dec996d9b742fc49f675272aa42ebd31f04226ba3d28836a6556cb61c29e7 in / 
# Wed, 22 Jul 2020 02:16:14 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 06:10:34 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 23 Jul 2020 06:12:20 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 06:14:21 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d022338f917106731b8902d4c3d7009435a41381c11c8d210bbd6af007569f69`  
		Last Modified: Wed, 22 Jul 2020 02:26:01 GMT  
		Size: 30.5 MB (30524562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a35a0ce279229326ca6a3a4114458fe3e7a42a86875ae4b3f3e6a8a914127f`  
		Last Modified: Thu, 23 Jul 2020 06:59:10 GMT  
		Size: 256.2 KB (256204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c409da6637fbd5bae065a688f5b8fa5bca60053859e7f816079c977f9193411c`  
		Last Modified: Thu, 23 Jul 2020 06:59:18 GMT  
		Size: 29.3 MB (29349424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10-slim`

```console
$ docker pull mono@sha256:1329f019558cff676a9d8531f5cc4a7f558b8cda33b11f1809f6ccd2c14618f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v5
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.10-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:bfbf7d0dd6ec900bd4fb046e1171472d0cc6b4bc32c10095bcc1718d0d2fb4f3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51622762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0887bb40baf7e1ebaa4491740009839e418df248c2f18e393048574e7a3283aa`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:51:01 GMT
ADD file:4ea2d111c970d510f4eccf0fa08caafde1d227fc4c249d67c1b9d99998b0b906 in / 
# Wed, 22 Jul 2020 00:51:04 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 21:12:42 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 22 Jul 2020 21:13:14 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 22 Jul 2020 21:14:39 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7ae4223cfc253e8d54407ec654ed8fb606352daea8da124f33dacd17626259ad`  
		Last Modified: Wed, 22 Jul 2020 00:58:53 GMT  
		Size: 24.8 MB (24837461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b201b7c93f2f75a8f765155e3fd569dbc95a79c57c644b4595e1eff9afe8e9`  
		Last Modified: Wed, 22 Jul 2020 21:21:16 GMT  
		Size: 256.0 KB (255977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47783e7ea018044b2c75ce172154e65072809be55a95a291093f770a8c261e75`  
		Last Modified: Wed, 22 Jul 2020 21:21:27 GMT  
		Size: 26.5 MB (26529324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:90c6e2ff8ea8544e22e0263aff48c2e93d9b0d5744988b3450b239c9a01bce98
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57861852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9eaeca8f8945189ca2b07c8c7261bb0dcfea6c27e322fe4f79f9e4bbb082dbb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:41:09 GMT
ADD file:1efd5b51a56f36bcf79a1bcea1df36ef28299a42bc11e758f9e49066f2a1f085 in / 
# Wed, 22 Jul 2020 00:41:10 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 05:21:19 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 23 Jul 2020 05:21:40 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 05:22:18 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3999339def4d7591a8064bfc698302ae0e29bc5e0557ae392c122e1b3efa9305`  
		Last Modified: Wed, 22 Jul 2020 00:47:42 GMT  
		Size: 25.9 MB (25857826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072a4eb4e02ed79a5f02c37ff3909423a2376488a8c9f16c1d2a94ac58359078`  
		Last Modified: Thu, 23 Jul 2020 05:27:50 GMT  
		Size: 255.9 KB (255908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfeb41b8c951ba90f625eda71258c0aa6098d6281c21319a2db7cdf691d34fc`  
		Last Modified: Thu, 23 Jul 2020 05:28:00 GMT  
		Size: 31.7 MB (31748118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; 386

```console
$ docker pull mono@sha256:832edc5e755243979388a770f2a26b002ff53970f4d5980d4646408b83977600
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99145441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0acbbfdbc517756895fa8f98bd81276148a67102797ffbda89f1c47569e381a4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:09:15 GMT
ADD file:ee51bd8fcf2e02243de32c0f0e7899acebfa23bdceb783f13feb33c484ee98b8 in / 
# Wed, 22 Jul 2020 02:09:15 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 00:17:56 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 23 Jul 2020 00:18:08 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 00:18:59 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:75157e9ef5a857d6b02d235e08a164737ad009bae299277f86131063e6204e0b`  
		Last Modified: Wed, 22 Jul 2020 02:15:45 GMT  
		Size: 27.8 MB (27754899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf3d2401f59eb0e901a248e7de7b81f6d0ce70dc8958450d9406575c5ae402a`  
		Last Modified: Thu, 23 Jul 2020 00:24:53 GMT  
		Size: 255.9 KB (255866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49c7cc3cfa683a1a7f140766f83ef1205f003c8f18a9e7dc6192211af762bdd`  
		Last Modified: Thu, 23 Jul 2020 00:25:12 GMT  
		Size: 71.1 MB (71134676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:305c285592ef4afd7c1e21fc7f28ec09f07868e0d8f8fad13e56251960215f56
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60130190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe7500199f77ce97cf00689537fd03120b78b47c57f1894538baaf0659deafc3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:16:05 GMT
ADD file:037dec996d9b742fc49f675272aa42ebd31f04226ba3d28836a6556cb61c29e7 in / 
# Wed, 22 Jul 2020 02:16:14 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 06:10:34 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 23 Jul 2020 06:12:20 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 06:14:21 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d022338f917106731b8902d4c3d7009435a41381c11c8d210bbd6af007569f69`  
		Last Modified: Wed, 22 Jul 2020 02:26:01 GMT  
		Size: 30.5 MB (30524562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a35a0ce279229326ca6a3a4114458fe3e7a42a86875ae4b3f3e6a8a914127f`  
		Last Modified: Thu, 23 Jul 2020 06:59:10 GMT  
		Size: 256.2 KB (256204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c409da6637fbd5bae065a688f5b8fa5bca60053859e7f816079c977f9193411c`  
		Last Modified: Thu, 23 Jul 2020 06:59:18 GMT  
		Size: 29.3 MB (29349424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.8`

```console
$ docker pull mono@sha256:c3737329d0532da6281fedb7e4e5084a825319efa97e23e1c469692de59ca824
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
$ docker pull mono@sha256:c4118ed710f19848f2f29877a06271e11cfc3577e23c0018360a4cb347da404e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.0 MB (235018613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13d1331c323d17d5bd48ce6ff2e86f956687ec264d9d39f96bd0b6714de6272e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:07:07 GMT
ADD file:c11db0b135382f4c5b0f55b50740639bd8c1a22153b931b409cb9e41136734f2 in / 
# Wed, 22 Jul 2020 02:07:07 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 19:26:50 GMT
ENV MONO_VERSION=6.8.0.96
# Wed, 22 Jul 2020 19:26:59 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 22 Jul 2020 19:27:42 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 22 Jul 2020 19:40:41 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:cbd31ae332794bb723708526045b062b2fe6a08ccc0f143ea7dc18e0ebe46dea`  
		Last Modified: Wed, 22 Jul 2020 02:12:25 GMT  
		Size: 22.5 MB (22515635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fa40bfbf0082f2bae5777ccd52f3ca2add17d21a2375de40cb7b6a738aee92a`  
		Last Modified: Wed, 22 Jul 2020 20:02:10 GMT  
		Size: 244.5 KB (244495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989dabcb56d661ce7dac9d54d0c22d40088fb13ced11ca7807786cd9cd61431d`  
		Last Modified: Wed, 22 Jul 2020 20:02:28 GMT  
		Size: 64.5 MB (64467293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e08265401bb5017665068ac267affc91b2e11ffe852bd9b9d73572f1ebdede`  
		Last Modified: Wed, 22 Jul 2020 20:03:51 GMT  
		Size: 147.8 MB (147791190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8` - linux; arm variant v5

```console
$ docker pull mono@sha256:222855f1d87c83fc2078370052f5fd4895631780e62d693aade0aeff3c769bf2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.9 MB (179916751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91f1f1ff386350118a8ce9a2c7f17dd5696cc6b55c330292451eb4d9ee1465fb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:51:01 GMT
ADD file:4ea2d111c970d510f4eccf0fa08caafde1d227fc4c249d67c1b9d99998b0b906 in / 
# Wed, 22 Jul 2020 00:51:04 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 21:11:24 GMT
ENV MONO_VERSION=6.8.0.123
# Wed, 22 Jul 2020 21:11:44 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 22 Jul 2020 21:12:30 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 22 Jul 2020 21:17:46 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7ae4223cfc253e8d54407ec654ed8fb606352daea8da124f33dacd17626259ad`  
		Last Modified: Wed, 22 Jul 2020 00:58:53 GMT  
		Size: 24.8 MB (24837461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d8c961c83915aef58530df48e050cb089a654dc4fb1a86eb474065650ef16f`  
		Last Modified: Wed, 22 Jul 2020 21:20:59 GMT  
		Size: 255.9 KB (255928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d001b5f08f93019fc37285f1115dde2c26f6bf3c49763f303bb4f1b33ec04a`  
		Last Modified: Wed, 22 Jul 2020 21:21:08 GMT  
		Size: 26.5 MB (26538537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77ff39a638b9bd63864c5bb7680d2b7abb8e400600f65e1b3316c3c26d9ff8a`  
		Last Modified: Wed, 22 Jul 2020 21:22:24 GMT  
		Size: 128.3 MB (128284825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8` - linux; arm variant v7

```console
$ docker pull mono@sha256:0e79b73ff74791117dd0a42084eee5040160bdfa1d76e7e4cf2ffdd2b18b3cb9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.6 MB (172599115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a12c1996dc94982e4e9871cb355f1304e8c978c416bef75350d2fc25fb5fcad2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 01:33:30 GMT
ADD file:49b1a1b4f5c2201b0e23e29dca24c4f6ffc14620196c4bd77770952500c4bee1 in / 
# Wed, 22 Jul 2020 01:33:38 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 02:15:12 GMT
ENV MONO_VERSION=6.8.0.96
# Wed, 22 Jul 2020 02:15:59 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 22 Jul 2020 02:17:08 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 22 Jul 2020 02:24:59 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:cd38ad753522d120e27c5343b08f661ee3aebfe531d60102d7c624c16dba4d09`  
		Last Modified: Wed, 22 Jul 2020 01:44:24 GMT  
		Size: 19.3 MB (19298267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678b77b1123ed730afaccee19cb50f8fdf077e6011636b04af9cd365e6ebdf13`  
		Last Modified: Wed, 22 Jul 2020 02:32:32 GMT  
		Size: 244.6 KB (244569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ee2966b2ed591a8caba8af3012b33613fdcd2925dffc5f9eaa9328292c5af9`  
		Last Modified: Wed, 22 Jul 2020 02:32:40 GMT  
		Size: 24.5 MB (24495473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156d85b212d8926604522d94038ef09d4862f7a5aebd52d8f0c5e9546ef12c06`  
		Last Modified: Wed, 22 Jul 2020 02:34:24 GMT  
		Size: 128.6 MB (128560806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:e0289aed2a01d7d760e8abc0d9b67bc4a487781d5bb761baad0ccde9d6f6dfa5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.4 MB (202439135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb7737b586ecb6ce2555ee6b4c07ae7e79b41f2d35ce5bb5d085b33212307aa8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:41:09 GMT
ADD file:1efd5b51a56f36bcf79a1bcea1df36ef28299a42bc11e758f9e49066f2a1f085 in / 
# Wed, 22 Jul 2020 00:41:10 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 05:20:01 GMT
ENV MONO_VERSION=6.8.0.123
# Thu, 23 Jul 2020 05:20:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 05:21:02 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 23 Jul 2020 05:24:34 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3999339def4d7591a8064bfc698302ae0e29bc5e0557ae392c122e1b3efa9305`  
		Last Modified: Wed, 22 Jul 2020 00:47:42 GMT  
		Size: 25.9 MB (25857826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91dee914802069198081b9830f230791b963b151ca88cf067757c3d8cd371a13`  
		Last Modified: Thu, 23 Jul 2020 05:27:33 GMT  
		Size: 255.8 KB (255847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d3eb1d03b9d89fcf5c7a08a8311e1b85fbd48df7e35070b3089ad0ac45b2c4`  
		Last Modified: Thu, 23 Jul 2020 05:27:43 GMT  
		Size: 31.7 MB (31690772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c97190a7db7997a52b12b89e585e6e829a8092deae456c9f002be8ee81053483`  
		Last Modified: Thu, 23 Jul 2020 05:28:54 GMT  
		Size: 144.6 MB (144634690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8` - linux; 386

```console
$ docker pull mono@sha256:fcd250e16db30c0c698265db47269fc0673afcb47538f6a95e7c8f5a9280f098
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.2 MB (249237307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ffafcb346069c6cc6a0e111f6790ad53e3bc9c2b89db6c4b2dd0796cb78e635`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:09:15 GMT
ADD file:ee51bd8fcf2e02243de32c0f0e7899acebfa23bdceb783f13feb33c484ee98b8 in / 
# Wed, 22 Jul 2020 02:09:15 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 00:17:00 GMT
ENV MONO_VERSION=6.8.0.123
# Thu, 23 Jul 2020 00:17:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 00:17:45 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 23 Jul 2020 00:21:59 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:75157e9ef5a857d6b02d235e08a164737ad009bae299277f86131063e6204e0b`  
		Last Modified: Wed, 22 Jul 2020 02:15:45 GMT  
		Size: 27.8 MB (27754899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ba29ddb73580b652aba3f042666e92696e05ee037a5ff9508008da2a929068`  
		Last Modified: Thu, 23 Jul 2020 00:24:27 GMT  
		Size: 255.9 KB (255872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fd9fcc335c689030b50ca22351c854252fa068c37e3efd73653553affdaf01`  
		Last Modified: Thu, 23 Jul 2020 00:24:47 GMT  
		Size: 71.1 MB (71108412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0e7d36ac8ff15acf0581697122b917e8cadf082f9c614225d016ecbbccdd5ab`  
		Last Modified: Thu, 23 Jul 2020 00:26:02 GMT  
		Size: 150.1 MB (150118124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8` - linux; ppc64le

```console
$ docker pull mono@sha256:b4d92f0ff78fd67cbd5ea63e347333778c8b3b5974f70c5ae234e3f53fb7bf20
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.4 MB (191358103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7680d6fd68edf4baa7ddfb7fa92d5d945ff9bde41626f704d3fc3699fce8d77`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:16:05 GMT
ADD file:037dec996d9b742fc49f675272aa42ebd31f04226ba3d28836a6556cb61c29e7 in / 
# Wed, 22 Jul 2020 02:16:14 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 06:04:37 GMT
ENV MONO_VERSION=6.8.0.123
# Thu, 23 Jul 2020 06:07:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 06:10:16 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 23 Jul 2020 06:35:40 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d022338f917106731b8902d4c3d7009435a41381c11c8d210bbd6af007569f69`  
		Last Modified: Wed, 22 Jul 2020 02:26:01 GMT  
		Size: 30.5 MB (30524562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ca191b55b915f6b7ad3d902885fa98a129469b14899a01d0bd7c52010d99cc`  
		Last Modified: Thu, 23 Jul 2020 06:58:47 GMT  
		Size: 256.3 KB (256306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a84194e1de14f8fca94d699787f71ab71d1442427d80cd74146e3f00960eb4`  
		Last Modified: Thu, 23 Jul 2020 06:58:56 GMT  
		Size: 29.3 MB (29334189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10f92efe9a856d77d38bb83e21c093f2718942bb21ac2776f2788936a1d96ac`  
		Last Modified: Thu, 23 Jul 2020 07:00:04 GMT  
		Size: 131.2 MB (131243046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.8.0`

```console
$ docker pull mono@sha256:c3737329d0532da6281fedb7e4e5084a825319efa97e23e1c469692de59ca824
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
$ docker pull mono@sha256:c4118ed710f19848f2f29877a06271e11cfc3577e23c0018360a4cb347da404e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.0 MB (235018613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13d1331c323d17d5bd48ce6ff2e86f956687ec264d9d39f96bd0b6714de6272e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:07:07 GMT
ADD file:c11db0b135382f4c5b0f55b50740639bd8c1a22153b931b409cb9e41136734f2 in / 
# Wed, 22 Jul 2020 02:07:07 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 19:26:50 GMT
ENV MONO_VERSION=6.8.0.96
# Wed, 22 Jul 2020 19:26:59 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 22 Jul 2020 19:27:42 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 22 Jul 2020 19:40:41 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:cbd31ae332794bb723708526045b062b2fe6a08ccc0f143ea7dc18e0ebe46dea`  
		Last Modified: Wed, 22 Jul 2020 02:12:25 GMT  
		Size: 22.5 MB (22515635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fa40bfbf0082f2bae5777ccd52f3ca2add17d21a2375de40cb7b6a738aee92a`  
		Last Modified: Wed, 22 Jul 2020 20:02:10 GMT  
		Size: 244.5 KB (244495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989dabcb56d661ce7dac9d54d0c22d40088fb13ced11ca7807786cd9cd61431d`  
		Last Modified: Wed, 22 Jul 2020 20:02:28 GMT  
		Size: 64.5 MB (64467293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e08265401bb5017665068ac267affc91b2e11ffe852bd9b9d73572f1ebdede`  
		Last Modified: Wed, 22 Jul 2020 20:03:51 GMT  
		Size: 147.8 MB (147791190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0` - linux; arm variant v5

```console
$ docker pull mono@sha256:222855f1d87c83fc2078370052f5fd4895631780e62d693aade0aeff3c769bf2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.9 MB (179916751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91f1f1ff386350118a8ce9a2c7f17dd5696cc6b55c330292451eb4d9ee1465fb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:51:01 GMT
ADD file:4ea2d111c970d510f4eccf0fa08caafde1d227fc4c249d67c1b9d99998b0b906 in / 
# Wed, 22 Jul 2020 00:51:04 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 21:11:24 GMT
ENV MONO_VERSION=6.8.0.123
# Wed, 22 Jul 2020 21:11:44 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 22 Jul 2020 21:12:30 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 22 Jul 2020 21:17:46 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7ae4223cfc253e8d54407ec654ed8fb606352daea8da124f33dacd17626259ad`  
		Last Modified: Wed, 22 Jul 2020 00:58:53 GMT  
		Size: 24.8 MB (24837461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d8c961c83915aef58530df48e050cb089a654dc4fb1a86eb474065650ef16f`  
		Last Modified: Wed, 22 Jul 2020 21:20:59 GMT  
		Size: 255.9 KB (255928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d001b5f08f93019fc37285f1115dde2c26f6bf3c49763f303bb4f1b33ec04a`  
		Last Modified: Wed, 22 Jul 2020 21:21:08 GMT  
		Size: 26.5 MB (26538537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77ff39a638b9bd63864c5bb7680d2b7abb8e400600f65e1b3316c3c26d9ff8a`  
		Last Modified: Wed, 22 Jul 2020 21:22:24 GMT  
		Size: 128.3 MB (128284825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0` - linux; arm variant v7

```console
$ docker pull mono@sha256:0e79b73ff74791117dd0a42084eee5040160bdfa1d76e7e4cf2ffdd2b18b3cb9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.6 MB (172599115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a12c1996dc94982e4e9871cb355f1304e8c978c416bef75350d2fc25fb5fcad2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 01:33:30 GMT
ADD file:49b1a1b4f5c2201b0e23e29dca24c4f6ffc14620196c4bd77770952500c4bee1 in / 
# Wed, 22 Jul 2020 01:33:38 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 02:15:12 GMT
ENV MONO_VERSION=6.8.0.96
# Wed, 22 Jul 2020 02:15:59 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 22 Jul 2020 02:17:08 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 22 Jul 2020 02:24:59 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:cd38ad753522d120e27c5343b08f661ee3aebfe531d60102d7c624c16dba4d09`  
		Last Modified: Wed, 22 Jul 2020 01:44:24 GMT  
		Size: 19.3 MB (19298267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678b77b1123ed730afaccee19cb50f8fdf077e6011636b04af9cd365e6ebdf13`  
		Last Modified: Wed, 22 Jul 2020 02:32:32 GMT  
		Size: 244.6 KB (244569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ee2966b2ed591a8caba8af3012b33613fdcd2925dffc5f9eaa9328292c5af9`  
		Last Modified: Wed, 22 Jul 2020 02:32:40 GMT  
		Size: 24.5 MB (24495473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156d85b212d8926604522d94038ef09d4862f7a5aebd52d8f0c5e9546ef12c06`  
		Last Modified: Wed, 22 Jul 2020 02:34:24 GMT  
		Size: 128.6 MB (128560806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:e0289aed2a01d7d760e8abc0d9b67bc4a487781d5bb761baad0ccde9d6f6dfa5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.4 MB (202439135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb7737b586ecb6ce2555ee6b4c07ae7e79b41f2d35ce5bb5d085b33212307aa8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:41:09 GMT
ADD file:1efd5b51a56f36bcf79a1bcea1df36ef28299a42bc11e758f9e49066f2a1f085 in / 
# Wed, 22 Jul 2020 00:41:10 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 05:20:01 GMT
ENV MONO_VERSION=6.8.0.123
# Thu, 23 Jul 2020 05:20:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 05:21:02 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 23 Jul 2020 05:24:34 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3999339def4d7591a8064bfc698302ae0e29bc5e0557ae392c122e1b3efa9305`  
		Last Modified: Wed, 22 Jul 2020 00:47:42 GMT  
		Size: 25.9 MB (25857826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91dee914802069198081b9830f230791b963b151ca88cf067757c3d8cd371a13`  
		Last Modified: Thu, 23 Jul 2020 05:27:33 GMT  
		Size: 255.8 KB (255847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d3eb1d03b9d89fcf5c7a08a8311e1b85fbd48df7e35070b3089ad0ac45b2c4`  
		Last Modified: Thu, 23 Jul 2020 05:27:43 GMT  
		Size: 31.7 MB (31690772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c97190a7db7997a52b12b89e585e6e829a8092deae456c9f002be8ee81053483`  
		Last Modified: Thu, 23 Jul 2020 05:28:54 GMT  
		Size: 144.6 MB (144634690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0` - linux; 386

```console
$ docker pull mono@sha256:fcd250e16db30c0c698265db47269fc0673afcb47538f6a95e7c8f5a9280f098
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.2 MB (249237307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ffafcb346069c6cc6a0e111f6790ad53e3bc9c2b89db6c4b2dd0796cb78e635`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:09:15 GMT
ADD file:ee51bd8fcf2e02243de32c0f0e7899acebfa23bdceb783f13feb33c484ee98b8 in / 
# Wed, 22 Jul 2020 02:09:15 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 00:17:00 GMT
ENV MONO_VERSION=6.8.0.123
# Thu, 23 Jul 2020 00:17:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 00:17:45 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 23 Jul 2020 00:21:59 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:75157e9ef5a857d6b02d235e08a164737ad009bae299277f86131063e6204e0b`  
		Last Modified: Wed, 22 Jul 2020 02:15:45 GMT  
		Size: 27.8 MB (27754899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ba29ddb73580b652aba3f042666e92696e05ee037a5ff9508008da2a929068`  
		Last Modified: Thu, 23 Jul 2020 00:24:27 GMT  
		Size: 255.9 KB (255872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fd9fcc335c689030b50ca22351c854252fa068c37e3efd73653553affdaf01`  
		Last Modified: Thu, 23 Jul 2020 00:24:47 GMT  
		Size: 71.1 MB (71108412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0e7d36ac8ff15acf0581697122b917e8cadf082f9c614225d016ecbbccdd5ab`  
		Last Modified: Thu, 23 Jul 2020 00:26:02 GMT  
		Size: 150.1 MB (150118124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0` - linux; ppc64le

```console
$ docker pull mono@sha256:b4d92f0ff78fd67cbd5ea63e347333778c8b3b5974f70c5ae234e3f53fb7bf20
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.4 MB (191358103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7680d6fd68edf4baa7ddfb7fa92d5d945ff9bde41626f704d3fc3699fce8d77`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:16:05 GMT
ADD file:037dec996d9b742fc49f675272aa42ebd31f04226ba3d28836a6556cb61c29e7 in / 
# Wed, 22 Jul 2020 02:16:14 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 06:04:37 GMT
ENV MONO_VERSION=6.8.0.123
# Thu, 23 Jul 2020 06:07:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 06:10:16 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 23 Jul 2020 06:35:40 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d022338f917106731b8902d4c3d7009435a41381c11c8d210bbd6af007569f69`  
		Last Modified: Wed, 22 Jul 2020 02:26:01 GMT  
		Size: 30.5 MB (30524562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ca191b55b915f6b7ad3d902885fa98a129469b14899a01d0bd7c52010d99cc`  
		Last Modified: Thu, 23 Jul 2020 06:58:47 GMT  
		Size: 256.3 KB (256306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a84194e1de14f8fca94d699787f71ab71d1442427d80cd74146e3f00960eb4`  
		Last Modified: Thu, 23 Jul 2020 06:58:56 GMT  
		Size: 29.3 MB (29334189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10f92efe9a856d77d38bb83e21c093f2718942bb21ac2776f2788936a1d96ac`  
		Last Modified: Thu, 23 Jul 2020 07:00:04 GMT  
		Size: 131.2 MB (131243046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.8.0.123`

```console
$ docker pull mono@sha256:826b3c108520037cb28583f4ac32e7fa205780469df3b73b133a0b0e44270b93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v5
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.8.0.123` - linux; arm variant v5

```console
$ docker pull mono@sha256:222855f1d87c83fc2078370052f5fd4895631780e62d693aade0aeff3c769bf2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.9 MB (179916751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91f1f1ff386350118a8ce9a2c7f17dd5696cc6b55c330292451eb4d9ee1465fb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:51:01 GMT
ADD file:4ea2d111c970d510f4eccf0fa08caafde1d227fc4c249d67c1b9d99998b0b906 in / 
# Wed, 22 Jul 2020 00:51:04 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 21:11:24 GMT
ENV MONO_VERSION=6.8.0.123
# Wed, 22 Jul 2020 21:11:44 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 22 Jul 2020 21:12:30 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 22 Jul 2020 21:17:46 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7ae4223cfc253e8d54407ec654ed8fb606352daea8da124f33dacd17626259ad`  
		Last Modified: Wed, 22 Jul 2020 00:58:53 GMT  
		Size: 24.8 MB (24837461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d8c961c83915aef58530df48e050cb089a654dc4fb1a86eb474065650ef16f`  
		Last Modified: Wed, 22 Jul 2020 21:20:59 GMT  
		Size: 255.9 KB (255928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d001b5f08f93019fc37285f1115dde2c26f6bf3c49763f303bb4f1b33ec04a`  
		Last Modified: Wed, 22 Jul 2020 21:21:08 GMT  
		Size: 26.5 MB (26538537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77ff39a638b9bd63864c5bb7680d2b7abb8e400600f65e1b3316c3c26d9ff8a`  
		Last Modified: Wed, 22 Jul 2020 21:22:24 GMT  
		Size: 128.3 MB (128284825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.123` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:e0289aed2a01d7d760e8abc0d9b67bc4a487781d5bb761baad0ccde9d6f6dfa5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.4 MB (202439135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb7737b586ecb6ce2555ee6b4c07ae7e79b41f2d35ce5bb5d085b33212307aa8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:41:09 GMT
ADD file:1efd5b51a56f36bcf79a1bcea1df36ef28299a42bc11e758f9e49066f2a1f085 in / 
# Wed, 22 Jul 2020 00:41:10 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 05:20:01 GMT
ENV MONO_VERSION=6.8.0.123
# Thu, 23 Jul 2020 05:20:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 05:21:02 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 23 Jul 2020 05:24:34 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3999339def4d7591a8064bfc698302ae0e29bc5e0557ae392c122e1b3efa9305`  
		Last Modified: Wed, 22 Jul 2020 00:47:42 GMT  
		Size: 25.9 MB (25857826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91dee914802069198081b9830f230791b963b151ca88cf067757c3d8cd371a13`  
		Last Modified: Thu, 23 Jul 2020 05:27:33 GMT  
		Size: 255.8 KB (255847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d3eb1d03b9d89fcf5c7a08a8311e1b85fbd48df7e35070b3089ad0ac45b2c4`  
		Last Modified: Thu, 23 Jul 2020 05:27:43 GMT  
		Size: 31.7 MB (31690772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c97190a7db7997a52b12b89e585e6e829a8092deae456c9f002be8ee81053483`  
		Last Modified: Thu, 23 Jul 2020 05:28:54 GMT  
		Size: 144.6 MB (144634690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.123` - linux; 386

```console
$ docker pull mono@sha256:fcd250e16db30c0c698265db47269fc0673afcb47538f6a95e7c8f5a9280f098
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.2 MB (249237307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ffafcb346069c6cc6a0e111f6790ad53e3bc9c2b89db6c4b2dd0796cb78e635`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:09:15 GMT
ADD file:ee51bd8fcf2e02243de32c0f0e7899acebfa23bdceb783f13feb33c484ee98b8 in / 
# Wed, 22 Jul 2020 02:09:15 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 00:17:00 GMT
ENV MONO_VERSION=6.8.0.123
# Thu, 23 Jul 2020 00:17:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 00:17:45 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 23 Jul 2020 00:21:59 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:75157e9ef5a857d6b02d235e08a164737ad009bae299277f86131063e6204e0b`  
		Last Modified: Wed, 22 Jul 2020 02:15:45 GMT  
		Size: 27.8 MB (27754899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ba29ddb73580b652aba3f042666e92696e05ee037a5ff9508008da2a929068`  
		Last Modified: Thu, 23 Jul 2020 00:24:27 GMT  
		Size: 255.9 KB (255872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fd9fcc335c689030b50ca22351c854252fa068c37e3efd73653553affdaf01`  
		Last Modified: Thu, 23 Jul 2020 00:24:47 GMT  
		Size: 71.1 MB (71108412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0e7d36ac8ff15acf0581697122b917e8cadf082f9c614225d016ecbbccdd5ab`  
		Last Modified: Thu, 23 Jul 2020 00:26:02 GMT  
		Size: 150.1 MB (150118124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.123` - linux; ppc64le

```console
$ docker pull mono@sha256:b4d92f0ff78fd67cbd5ea63e347333778c8b3b5974f70c5ae234e3f53fb7bf20
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.4 MB (191358103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7680d6fd68edf4baa7ddfb7fa92d5d945ff9bde41626f704d3fc3699fce8d77`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:16:05 GMT
ADD file:037dec996d9b742fc49f675272aa42ebd31f04226ba3d28836a6556cb61c29e7 in / 
# Wed, 22 Jul 2020 02:16:14 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 06:04:37 GMT
ENV MONO_VERSION=6.8.0.123
# Thu, 23 Jul 2020 06:07:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 06:10:16 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 23 Jul 2020 06:35:40 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d022338f917106731b8902d4c3d7009435a41381c11c8d210bbd6af007569f69`  
		Last Modified: Wed, 22 Jul 2020 02:26:01 GMT  
		Size: 30.5 MB (30524562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ca191b55b915f6b7ad3d902885fa98a129469b14899a01d0bd7c52010d99cc`  
		Last Modified: Thu, 23 Jul 2020 06:58:47 GMT  
		Size: 256.3 KB (256306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a84194e1de14f8fca94d699787f71ab71d1442427d80cd74146e3f00960eb4`  
		Last Modified: Thu, 23 Jul 2020 06:58:56 GMT  
		Size: 29.3 MB (29334189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10f92efe9a856d77d38bb83e21c093f2718942bb21ac2776f2788936a1d96ac`  
		Last Modified: Thu, 23 Jul 2020 07:00:04 GMT  
		Size: 131.2 MB (131243046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.8.0.123-slim`

```console
$ docker pull mono@sha256:802ca93fc1d9a27f82cba6b6a64519632e928a313dee173099b1daef25462566
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v5
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.8.0.123-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:d72c898eb547cda9a6e5857284580215f3602b27ba2234b8764a6ae1b650f86e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51631926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bc12135113cfe2a5c3ed5bdaf06aeb9429d60e66859df0814d3b5247740995e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:51:01 GMT
ADD file:4ea2d111c970d510f4eccf0fa08caafde1d227fc4c249d67c1b9d99998b0b906 in / 
# Wed, 22 Jul 2020 00:51:04 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 21:11:24 GMT
ENV MONO_VERSION=6.8.0.123
# Wed, 22 Jul 2020 21:11:44 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 22 Jul 2020 21:12:30 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7ae4223cfc253e8d54407ec654ed8fb606352daea8da124f33dacd17626259ad`  
		Last Modified: Wed, 22 Jul 2020 00:58:53 GMT  
		Size: 24.8 MB (24837461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d8c961c83915aef58530df48e050cb089a654dc4fb1a86eb474065650ef16f`  
		Last Modified: Wed, 22 Jul 2020 21:20:59 GMT  
		Size: 255.9 KB (255928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d001b5f08f93019fc37285f1115dde2c26f6bf3c49763f303bb4f1b33ec04a`  
		Last Modified: Wed, 22 Jul 2020 21:21:08 GMT  
		Size: 26.5 MB (26538537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.123-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:c76b6b01456424bbd8ba00d4a5491e79c1b95b0d392108c1dc565aa6cc48ddda
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.8 MB (57804445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5d56502b1cb7a06a62abf1cfd6532606baedd8b063ed2570b80f9055c8d3695`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:41:09 GMT
ADD file:1efd5b51a56f36bcf79a1bcea1df36ef28299a42bc11e758f9e49066f2a1f085 in / 
# Wed, 22 Jul 2020 00:41:10 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 05:20:01 GMT
ENV MONO_VERSION=6.8.0.123
# Thu, 23 Jul 2020 05:20:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 05:21:02 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3999339def4d7591a8064bfc698302ae0e29bc5e0557ae392c122e1b3efa9305`  
		Last Modified: Wed, 22 Jul 2020 00:47:42 GMT  
		Size: 25.9 MB (25857826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91dee914802069198081b9830f230791b963b151ca88cf067757c3d8cd371a13`  
		Last Modified: Thu, 23 Jul 2020 05:27:33 GMT  
		Size: 255.8 KB (255847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d3eb1d03b9d89fcf5c7a08a8311e1b85fbd48df7e35070b3089ad0ac45b2c4`  
		Last Modified: Thu, 23 Jul 2020 05:27:43 GMT  
		Size: 31.7 MB (31690772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.123-slim` - linux; 386

```console
$ docker pull mono@sha256:199ec55527e4b2020319721e151a287fb4ce6ed93c0737310622df898f41ab0f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99119183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ade7dd182faa328aabc014e5550b15fc780caff82ed554e9f69e61caaf606152`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:09:15 GMT
ADD file:ee51bd8fcf2e02243de32c0f0e7899acebfa23bdceb783f13feb33c484ee98b8 in / 
# Wed, 22 Jul 2020 02:09:15 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 00:17:00 GMT
ENV MONO_VERSION=6.8.0.123
# Thu, 23 Jul 2020 00:17:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 00:17:45 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:75157e9ef5a857d6b02d235e08a164737ad009bae299277f86131063e6204e0b`  
		Last Modified: Wed, 22 Jul 2020 02:15:45 GMT  
		Size: 27.8 MB (27754899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ba29ddb73580b652aba3f042666e92696e05ee037a5ff9508008da2a929068`  
		Last Modified: Thu, 23 Jul 2020 00:24:27 GMT  
		Size: 255.9 KB (255872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fd9fcc335c689030b50ca22351c854252fa068c37e3efd73653553affdaf01`  
		Last Modified: Thu, 23 Jul 2020 00:24:47 GMT  
		Size: 71.1 MB (71108412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.123-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:f2f499da5dbca01406880d92c693f6ed9b6abe15117a095e12cbe87bffcb0fdf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60115057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be9d3c0f68e3c61dbc6c0e1472f4b3c8f6c5114ad076514baf04536f76851c70`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:16:05 GMT
ADD file:037dec996d9b742fc49f675272aa42ebd31f04226ba3d28836a6556cb61c29e7 in / 
# Wed, 22 Jul 2020 02:16:14 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 06:04:37 GMT
ENV MONO_VERSION=6.8.0.123
# Thu, 23 Jul 2020 06:07:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 06:10:16 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d022338f917106731b8902d4c3d7009435a41381c11c8d210bbd6af007569f69`  
		Last Modified: Wed, 22 Jul 2020 02:26:01 GMT  
		Size: 30.5 MB (30524562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ca191b55b915f6b7ad3d902885fa98a129469b14899a01d0bd7c52010d99cc`  
		Last Modified: Thu, 23 Jul 2020 06:58:47 GMT  
		Size: 256.3 KB (256306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a84194e1de14f8fca94d699787f71ab71d1442427d80cd74146e3f00960eb4`  
		Last Modified: Thu, 23 Jul 2020 06:58:56 GMT  
		Size: 29.3 MB (29334189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.8.0-slim`

```console
$ docker pull mono@sha256:7c5e8518f53e61f76b2890372a3e5689b52b71233c531232ca1af83a5669641e
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
$ docker pull mono@sha256:8662fe5f43ce6662afc770942a78620711529e22bfb3a6915d08de61f0391b0c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.2 MB (87227423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c8044236c95b15c23c907be455632697f74ca4ba4e6a5836dd26b5d9b5cbcd4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:07:07 GMT
ADD file:c11db0b135382f4c5b0f55b50740639bd8c1a22153b931b409cb9e41136734f2 in / 
# Wed, 22 Jul 2020 02:07:07 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 19:26:50 GMT
ENV MONO_VERSION=6.8.0.96
# Wed, 22 Jul 2020 19:26:59 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 22 Jul 2020 19:27:42 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:cbd31ae332794bb723708526045b062b2fe6a08ccc0f143ea7dc18e0ebe46dea`  
		Last Modified: Wed, 22 Jul 2020 02:12:25 GMT  
		Size: 22.5 MB (22515635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fa40bfbf0082f2bae5777ccd52f3ca2add17d21a2375de40cb7b6a738aee92a`  
		Last Modified: Wed, 22 Jul 2020 20:02:10 GMT  
		Size: 244.5 KB (244495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989dabcb56d661ce7dac9d54d0c22d40088fb13ced11ca7807786cd9cd61431d`  
		Last Modified: Wed, 22 Jul 2020 20:02:28 GMT  
		Size: 64.5 MB (64467293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:d72c898eb547cda9a6e5857284580215f3602b27ba2234b8764a6ae1b650f86e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51631926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bc12135113cfe2a5c3ed5bdaf06aeb9429d60e66859df0814d3b5247740995e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:51:01 GMT
ADD file:4ea2d111c970d510f4eccf0fa08caafde1d227fc4c249d67c1b9d99998b0b906 in / 
# Wed, 22 Jul 2020 00:51:04 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 21:11:24 GMT
ENV MONO_VERSION=6.8.0.123
# Wed, 22 Jul 2020 21:11:44 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 22 Jul 2020 21:12:30 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7ae4223cfc253e8d54407ec654ed8fb606352daea8da124f33dacd17626259ad`  
		Last Modified: Wed, 22 Jul 2020 00:58:53 GMT  
		Size: 24.8 MB (24837461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d8c961c83915aef58530df48e050cb089a654dc4fb1a86eb474065650ef16f`  
		Last Modified: Wed, 22 Jul 2020 21:20:59 GMT  
		Size: 255.9 KB (255928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d001b5f08f93019fc37285f1115dde2c26f6bf3c49763f303bb4f1b33ec04a`  
		Last Modified: Wed, 22 Jul 2020 21:21:08 GMT  
		Size: 26.5 MB (26538537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:43efe3765087680c99e00ef8f63dd9f8d1ba2a569c9a8af61dc54a18d82f9cc6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (44038309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:777fd2ade7d45508d862b53c0c85624224196846719397190648e897a2222b24`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 01:33:30 GMT
ADD file:49b1a1b4f5c2201b0e23e29dca24c4f6ffc14620196c4bd77770952500c4bee1 in / 
# Wed, 22 Jul 2020 01:33:38 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 02:15:12 GMT
ENV MONO_VERSION=6.8.0.96
# Wed, 22 Jul 2020 02:15:59 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 22 Jul 2020 02:17:08 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:cd38ad753522d120e27c5343b08f661ee3aebfe531d60102d7c624c16dba4d09`  
		Last Modified: Wed, 22 Jul 2020 01:44:24 GMT  
		Size: 19.3 MB (19298267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678b77b1123ed730afaccee19cb50f8fdf077e6011636b04af9cd365e6ebdf13`  
		Last Modified: Wed, 22 Jul 2020 02:32:32 GMT  
		Size: 244.6 KB (244569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ee2966b2ed591a8caba8af3012b33613fdcd2925dffc5f9eaa9328292c5af9`  
		Last Modified: Wed, 22 Jul 2020 02:32:40 GMT  
		Size: 24.5 MB (24495473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:c76b6b01456424bbd8ba00d4a5491e79c1b95b0d392108c1dc565aa6cc48ddda
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.8 MB (57804445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5d56502b1cb7a06a62abf1cfd6532606baedd8b063ed2570b80f9055c8d3695`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:41:09 GMT
ADD file:1efd5b51a56f36bcf79a1bcea1df36ef28299a42bc11e758f9e49066f2a1f085 in / 
# Wed, 22 Jul 2020 00:41:10 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 05:20:01 GMT
ENV MONO_VERSION=6.8.0.123
# Thu, 23 Jul 2020 05:20:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 05:21:02 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3999339def4d7591a8064bfc698302ae0e29bc5e0557ae392c122e1b3efa9305`  
		Last Modified: Wed, 22 Jul 2020 00:47:42 GMT  
		Size: 25.9 MB (25857826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91dee914802069198081b9830f230791b963b151ca88cf067757c3d8cd371a13`  
		Last Modified: Thu, 23 Jul 2020 05:27:33 GMT  
		Size: 255.8 KB (255847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d3eb1d03b9d89fcf5c7a08a8311e1b85fbd48df7e35070b3089ad0ac45b2c4`  
		Last Modified: Thu, 23 Jul 2020 05:27:43 GMT  
		Size: 31.7 MB (31690772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0-slim` - linux; 386

```console
$ docker pull mono@sha256:199ec55527e4b2020319721e151a287fb4ce6ed93c0737310622df898f41ab0f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99119183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ade7dd182faa328aabc014e5550b15fc780caff82ed554e9f69e61caaf606152`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:09:15 GMT
ADD file:ee51bd8fcf2e02243de32c0f0e7899acebfa23bdceb783f13feb33c484ee98b8 in / 
# Wed, 22 Jul 2020 02:09:15 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 00:17:00 GMT
ENV MONO_VERSION=6.8.0.123
# Thu, 23 Jul 2020 00:17:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 00:17:45 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:75157e9ef5a857d6b02d235e08a164737ad009bae299277f86131063e6204e0b`  
		Last Modified: Wed, 22 Jul 2020 02:15:45 GMT  
		Size: 27.8 MB (27754899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ba29ddb73580b652aba3f042666e92696e05ee037a5ff9508008da2a929068`  
		Last Modified: Thu, 23 Jul 2020 00:24:27 GMT  
		Size: 255.9 KB (255872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fd9fcc335c689030b50ca22351c854252fa068c37e3efd73653553affdaf01`  
		Last Modified: Thu, 23 Jul 2020 00:24:47 GMT  
		Size: 71.1 MB (71108412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:f2f499da5dbca01406880d92c693f6ed9b6abe15117a095e12cbe87bffcb0fdf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60115057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be9d3c0f68e3c61dbc6c0e1472f4b3c8f6c5114ad076514baf04536f76851c70`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:16:05 GMT
ADD file:037dec996d9b742fc49f675272aa42ebd31f04226ba3d28836a6556cb61c29e7 in / 
# Wed, 22 Jul 2020 02:16:14 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 06:04:37 GMT
ENV MONO_VERSION=6.8.0.123
# Thu, 23 Jul 2020 06:07:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 06:10:16 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d022338f917106731b8902d4c3d7009435a41381c11c8d210bbd6af007569f69`  
		Last Modified: Wed, 22 Jul 2020 02:26:01 GMT  
		Size: 30.5 MB (30524562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ca191b55b915f6b7ad3d902885fa98a129469b14899a01d0bd7c52010d99cc`  
		Last Modified: Thu, 23 Jul 2020 06:58:47 GMT  
		Size: 256.3 KB (256306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a84194e1de14f8fca94d699787f71ab71d1442427d80cd74146e3f00960eb4`  
		Last Modified: Thu, 23 Jul 2020 06:58:56 GMT  
		Size: 29.3 MB (29334189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.8-slim`

```console
$ docker pull mono@sha256:7c5e8518f53e61f76b2890372a3e5689b52b71233c531232ca1af83a5669641e
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
$ docker pull mono@sha256:8662fe5f43ce6662afc770942a78620711529e22bfb3a6915d08de61f0391b0c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.2 MB (87227423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c8044236c95b15c23c907be455632697f74ca4ba4e6a5836dd26b5d9b5cbcd4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:07:07 GMT
ADD file:c11db0b135382f4c5b0f55b50740639bd8c1a22153b931b409cb9e41136734f2 in / 
# Wed, 22 Jul 2020 02:07:07 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 19:26:50 GMT
ENV MONO_VERSION=6.8.0.96
# Wed, 22 Jul 2020 19:26:59 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 22 Jul 2020 19:27:42 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:cbd31ae332794bb723708526045b062b2fe6a08ccc0f143ea7dc18e0ebe46dea`  
		Last Modified: Wed, 22 Jul 2020 02:12:25 GMT  
		Size: 22.5 MB (22515635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fa40bfbf0082f2bae5777ccd52f3ca2add17d21a2375de40cb7b6a738aee92a`  
		Last Modified: Wed, 22 Jul 2020 20:02:10 GMT  
		Size: 244.5 KB (244495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989dabcb56d661ce7dac9d54d0c22d40088fb13ced11ca7807786cd9cd61431d`  
		Last Modified: Wed, 22 Jul 2020 20:02:28 GMT  
		Size: 64.5 MB (64467293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:d72c898eb547cda9a6e5857284580215f3602b27ba2234b8764a6ae1b650f86e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51631926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bc12135113cfe2a5c3ed5bdaf06aeb9429d60e66859df0814d3b5247740995e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:51:01 GMT
ADD file:4ea2d111c970d510f4eccf0fa08caafde1d227fc4c249d67c1b9d99998b0b906 in / 
# Wed, 22 Jul 2020 00:51:04 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 21:11:24 GMT
ENV MONO_VERSION=6.8.0.123
# Wed, 22 Jul 2020 21:11:44 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 22 Jul 2020 21:12:30 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7ae4223cfc253e8d54407ec654ed8fb606352daea8da124f33dacd17626259ad`  
		Last Modified: Wed, 22 Jul 2020 00:58:53 GMT  
		Size: 24.8 MB (24837461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d8c961c83915aef58530df48e050cb089a654dc4fb1a86eb474065650ef16f`  
		Last Modified: Wed, 22 Jul 2020 21:20:59 GMT  
		Size: 255.9 KB (255928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d001b5f08f93019fc37285f1115dde2c26f6bf3c49763f303bb4f1b33ec04a`  
		Last Modified: Wed, 22 Jul 2020 21:21:08 GMT  
		Size: 26.5 MB (26538537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:43efe3765087680c99e00ef8f63dd9f8d1ba2a569c9a8af61dc54a18d82f9cc6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (44038309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:777fd2ade7d45508d862b53c0c85624224196846719397190648e897a2222b24`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 01:33:30 GMT
ADD file:49b1a1b4f5c2201b0e23e29dca24c4f6ffc14620196c4bd77770952500c4bee1 in / 
# Wed, 22 Jul 2020 01:33:38 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 02:15:12 GMT
ENV MONO_VERSION=6.8.0.96
# Wed, 22 Jul 2020 02:15:59 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 22 Jul 2020 02:17:08 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:cd38ad753522d120e27c5343b08f661ee3aebfe531d60102d7c624c16dba4d09`  
		Last Modified: Wed, 22 Jul 2020 01:44:24 GMT  
		Size: 19.3 MB (19298267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678b77b1123ed730afaccee19cb50f8fdf077e6011636b04af9cd365e6ebdf13`  
		Last Modified: Wed, 22 Jul 2020 02:32:32 GMT  
		Size: 244.6 KB (244569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ee2966b2ed591a8caba8af3012b33613fdcd2925dffc5f9eaa9328292c5af9`  
		Last Modified: Wed, 22 Jul 2020 02:32:40 GMT  
		Size: 24.5 MB (24495473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:c76b6b01456424bbd8ba00d4a5491e79c1b95b0d392108c1dc565aa6cc48ddda
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.8 MB (57804445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5d56502b1cb7a06a62abf1cfd6532606baedd8b063ed2570b80f9055c8d3695`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:41:09 GMT
ADD file:1efd5b51a56f36bcf79a1bcea1df36ef28299a42bc11e758f9e49066f2a1f085 in / 
# Wed, 22 Jul 2020 00:41:10 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 05:20:01 GMT
ENV MONO_VERSION=6.8.0.123
# Thu, 23 Jul 2020 05:20:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 05:21:02 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3999339def4d7591a8064bfc698302ae0e29bc5e0557ae392c122e1b3efa9305`  
		Last Modified: Wed, 22 Jul 2020 00:47:42 GMT  
		Size: 25.9 MB (25857826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91dee914802069198081b9830f230791b963b151ca88cf067757c3d8cd371a13`  
		Last Modified: Thu, 23 Jul 2020 05:27:33 GMT  
		Size: 255.8 KB (255847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d3eb1d03b9d89fcf5c7a08a8311e1b85fbd48df7e35070b3089ad0ac45b2c4`  
		Last Modified: Thu, 23 Jul 2020 05:27:43 GMT  
		Size: 31.7 MB (31690772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8-slim` - linux; 386

```console
$ docker pull mono@sha256:199ec55527e4b2020319721e151a287fb4ce6ed93c0737310622df898f41ab0f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99119183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ade7dd182faa328aabc014e5550b15fc780caff82ed554e9f69e61caaf606152`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:09:15 GMT
ADD file:ee51bd8fcf2e02243de32c0f0e7899acebfa23bdceb783f13feb33c484ee98b8 in / 
# Wed, 22 Jul 2020 02:09:15 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 00:17:00 GMT
ENV MONO_VERSION=6.8.0.123
# Thu, 23 Jul 2020 00:17:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 00:17:45 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:75157e9ef5a857d6b02d235e08a164737ad009bae299277f86131063e6204e0b`  
		Last Modified: Wed, 22 Jul 2020 02:15:45 GMT  
		Size: 27.8 MB (27754899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ba29ddb73580b652aba3f042666e92696e05ee037a5ff9508008da2a929068`  
		Last Modified: Thu, 23 Jul 2020 00:24:27 GMT  
		Size: 255.9 KB (255872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fd9fcc335c689030b50ca22351c854252fa068c37e3efd73653553affdaf01`  
		Last Modified: Thu, 23 Jul 2020 00:24:47 GMT  
		Size: 71.1 MB (71108412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:f2f499da5dbca01406880d92c693f6ed9b6abe15117a095e12cbe87bffcb0fdf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60115057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be9d3c0f68e3c61dbc6c0e1472f4b3c8f6c5114ad076514baf04536f76851c70`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:16:05 GMT
ADD file:037dec996d9b742fc49f675272aa42ebd31f04226ba3d28836a6556cb61c29e7 in / 
# Wed, 22 Jul 2020 02:16:14 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 06:04:37 GMT
ENV MONO_VERSION=6.8.0.123
# Thu, 23 Jul 2020 06:07:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 06:10:16 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d022338f917106731b8902d4c3d7009435a41381c11c8d210bbd6af007569f69`  
		Last Modified: Wed, 22 Jul 2020 02:26:01 GMT  
		Size: 30.5 MB (30524562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ca191b55b915f6b7ad3d902885fa98a129469b14899a01d0bd7c52010d99cc`  
		Last Modified: Thu, 23 Jul 2020 06:58:47 GMT  
		Size: 256.3 KB (256306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a84194e1de14f8fca94d699787f71ab71d1442427d80cd74146e3f00960eb4`  
		Last Modified: Thu, 23 Jul 2020 06:58:56 GMT  
		Size: 29.3 MB (29334189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6-slim`

```console
$ docker pull mono@sha256:4c09ae1b53e6cb0f9c15da768c7d29a26b5c4cc1deead2fcad57bda4b6ee5ed3
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
$ docker pull mono@sha256:8662fe5f43ce6662afc770942a78620711529e22bfb3a6915d08de61f0391b0c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.2 MB (87227423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c8044236c95b15c23c907be455632697f74ca4ba4e6a5836dd26b5d9b5cbcd4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:07:07 GMT
ADD file:c11db0b135382f4c5b0f55b50740639bd8c1a22153b931b409cb9e41136734f2 in / 
# Wed, 22 Jul 2020 02:07:07 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 19:26:50 GMT
ENV MONO_VERSION=6.8.0.96
# Wed, 22 Jul 2020 19:26:59 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 22 Jul 2020 19:27:42 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:cbd31ae332794bb723708526045b062b2fe6a08ccc0f143ea7dc18e0ebe46dea`  
		Last Modified: Wed, 22 Jul 2020 02:12:25 GMT  
		Size: 22.5 MB (22515635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fa40bfbf0082f2bae5777ccd52f3ca2add17d21a2375de40cb7b6a738aee92a`  
		Last Modified: Wed, 22 Jul 2020 20:02:10 GMT  
		Size: 244.5 KB (244495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989dabcb56d661ce7dac9d54d0c22d40088fb13ced11ca7807786cd9cd61431d`  
		Last Modified: Wed, 22 Jul 2020 20:02:28 GMT  
		Size: 64.5 MB (64467293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:bfbf7d0dd6ec900bd4fb046e1171472d0cc6b4bc32c10095bcc1718d0d2fb4f3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51622762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0887bb40baf7e1ebaa4491740009839e418df248c2f18e393048574e7a3283aa`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:51:01 GMT
ADD file:4ea2d111c970d510f4eccf0fa08caafde1d227fc4c249d67c1b9d99998b0b906 in / 
# Wed, 22 Jul 2020 00:51:04 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 21:12:42 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 22 Jul 2020 21:13:14 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 22 Jul 2020 21:14:39 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7ae4223cfc253e8d54407ec654ed8fb606352daea8da124f33dacd17626259ad`  
		Last Modified: Wed, 22 Jul 2020 00:58:53 GMT  
		Size: 24.8 MB (24837461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b201b7c93f2f75a8f765155e3fd569dbc95a79c57c644b4595e1eff9afe8e9`  
		Last Modified: Wed, 22 Jul 2020 21:21:16 GMT  
		Size: 256.0 KB (255977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47783e7ea018044b2c75ce172154e65072809be55a95a291093f770a8c261e75`  
		Last Modified: Wed, 22 Jul 2020 21:21:27 GMT  
		Size: 26.5 MB (26529324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:43efe3765087680c99e00ef8f63dd9f8d1ba2a569c9a8af61dc54a18d82f9cc6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (44038309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:777fd2ade7d45508d862b53c0c85624224196846719397190648e897a2222b24`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 01:33:30 GMT
ADD file:49b1a1b4f5c2201b0e23e29dca24c4f6ffc14620196c4bd77770952500c4bee1 in / 
# Wed, 22 Jul 2020 01:33:38 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 02:15:12 GMT
ENV MONO_VERSION=6.8.0.96
# Wed, 22 Jul 2020 02:15:59 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 22 Jul 2020 02:17:08 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:cd38ad753522d120e27c5343b08f661ee3aebfe531d60102d7c624c16dba4d09`  
		Last Modified: Wed, 22 Jul 2020 01:44:24 GMT  
		Size: 19.3 MB (19298267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678b77b1123ed730afaccee19cb50f8fdf077e6011636b04af9cd365e6ebdf13`  
		Last Modified: Wed, 22 Jul 2020 02:32:32 GMT  
		Size: 244.6 KB (244569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ee2966b2ed591a8caba8af3012b33613fdcd2925dffc5f9eaa9328292c5af9`  
		Last Modified: Wed, 22 Jul 2020 02:32:40 GMT  
		Size: 24.5 MB (24495473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:90c6e2ff8ea8544e22e0263aff48c2e93d9b0d5744988b3450b239c9a01bce98
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57861852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9eaeca8f8945189ca2b07c8c7261bb0dcfea6c27e322fe4f79f9e4bbb082dbb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:41:09 GMT
ADD file:1efd5b51a56f36bcf79a1bcea1df36ef28299a42bc11e758f9e49066f2a1f085 in / 
# Wed, 22 Jul 2020 00:41:10 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 05:21:19 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 23 Jul 2020 05:21:40 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 05:22:18 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3999339def4d7591a8064bfc698302ae0e29bc5e0557ae392c122e1b3efa9305`  
		Last Modified: Wed, 22 Jul 2020 00:47:42 GMT  
		Size: 25.9 MB (25857826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072a4eb4e02ed79a5f02c37ff3909423a2376488a8c9f16c1d2a94ac58359078`  
		Last Modified: Thu, 23 Jul 2020 05:27:50 GMT  
		Size: 255.9 KB (255908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfeb41b8c951ba90f625eda71258c0aa6098d6281c21319a2db7cdf691d34fc`  
		Last Modified: Thu, 23 Jul 2020 05:28:00 GMT  
		Size: 31.7 MB (31748118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; 386

```console
$ docker pull mono@sha256:832edc5e755243979388a770f2a26b002ff53970f4d5980d4646408b83977600
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99145441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0acbbfdbc517756895fa8f98bd81276148a67102797ffbda89f1c47569e381a4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:09:15 GMT
ADD file:ee51bd8fcf2e02243de32c0f0e7899acebfa23bdceb783f13feb33c484ee98b8 in / 
# Wed, 22 Jul 2020 02:09:15 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 00:17:56 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 23 Jul 2020 00:18:08 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 00:18:59 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:75157e9ef5a857d6b02d235e08a164737ad009bae299277f86131063e6204e0b`  
		Last Modified: Wed, 22 Jul 2020 02:15:45 GMT  
		Size: 27.8 MB (27754899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf3d2401f59eb0e901a248e7de7b81f6d0ce70dc8958450d9406575c5ae402a`  
		Last Modified: Thu, 23 Jul 2020 00:24:53 GMT  
		Size: 255.9 KB (255866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49c7cc3cfa683a1a7f140766f83ef1205f003c8f18a9e7dc6192211af762bdd`  
		Last Modified: Thu, 23 Jul 2020 00:25:12 GMT  
		Size: 71.1 MB (71134676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:305c285592ef4afd7c1e21fc7f28ec09f07868e0d8f8fad13e56251960215f56
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60130190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe7500199f77ce97cf00689537fd03120b78b47c57f1894538baaf0659deafc3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:16:05 GMT
ADD file:037dec996d9b742fc49f675272aa42ebd31f04226ba3d28836a6556cb61c29e7 in / 
# Wed, 22 Jul 2020 02:16:14 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 06:10:34 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 23 Jul 2020 06:12:20 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 06:14:21 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d022338f917106731b8902d4c3d7009435a41381c11c8d210bbd6af007569f69`  
		Last Modified: Wed, 22 Jul 2020 02:26:01 GMT  
		Size: 30.5 MB (30524562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a35a0ce279229326ca6a3a4114458fe3e7a42a86875ae4b3f3e6a8a914127f`  
		Last Modified: Thu, 23 Jul 2020 06:59:10 GMT  
		Size: 256.2 KB (256204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c409da6637fbd5bae065a688f5b8fa5bca60053859e7f816079c977f9193411c`  
		Last Modified: Thu, 23 Jul 2020 06:59:18 GMT  
		Size: 29.3 MB (29349424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:latest`

```console
$ docker pull mono@sha256:21a4e78b865656f518c7b14ed1b839c7cb188a133a3375ab9a27ac7efa8b6239
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
$ docker pull mono@sha256:c4118ed710f19848f2f29877a06271e11cfc3577e23c0018360a4cb347da404e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.0 MB (235018613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13d1331c323d17d5bd48ce6ff2e86f956687ec264d9d39f96bd0b6714de6272e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:07:07 GMT
ADD file:c11db0b135382f4c5b0f55b50740639bd8c1a22153b931b409cb9e41136734f2 in / 
# Wed, 22 Jul 2020 02:07:07 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 19:26:50 GMT
ENV MONO_VERSION=6.8.0.96
# Wed, 22 Jul 2020 19:26:59 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 22 Jul 2020 19:27:42 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 22 Jul 2020 19:40:41 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:cbd31ae332794bb723708526045b062b2fe6a08ccc0f143ea7dc18e0ebe46dea`  
		Last Modified: Wed, 22 Jul 2020 02:12:25 GMT  
		Size: 22.5 MB (22515635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fa40bfbf0082f2bae5777ccd52f3ca2add17d21a2375de40cb7b6a738aee92a`  
		Last Modified: Wed, 22 Jul 2020 20:02:10 GMT  
		Size: 244.5 KB (244495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989dabcb56d661ce7dac9d54d0c22d40088fb13ced11ca7807786cd9cd61431d`  
		Last Modified: Wed, 22 Jul 2020 20:02:28 GMT  
		Size: 64.5 MB (64467293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e08265401bb5017665068ac267affc91b2e11ffe852bd9b9d73572f1ebdede`  
		Last Modified: Wed, 22 Jul 2020 20:03:51 GMT  
		Size: 147.8 MB (147791190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm variant v5

```console
$ docker pull mono@sha256:d216197c3136cf659053d08e0eb5d8f3961128d38d9893e9f8b19e7bddf3c51c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180580599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e9781e28afc6ae2bd019f175f92455997398b3d6b80688994a75f6b4acbb27f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:51:01 GMT
ADD file:4ea2d111c970d510f4eccf0fa08caafde1d227fc4c249d67c1b9d99998b0b906 in / 
# Wed, 22 Jul 2020 00:51:04 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 21:12:42 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 22 Jul 2020 21:13:14 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 22 Jul 2020 21:14:39 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 22 Jul 2020 21:20:33 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7ae4223cfc253e8d54407ec654ed8fb606352daea8da124f33dacd17626259ad`  
		Last Modified: Wed, 22 Jul 2020 00:58:53 GMT  
		Size: 24.8 MB (24837461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b201b7c93f2f75a8f765155e3fd569dbc95a79c57c644b4595e1eff9afe8e9`  
		Last Modified: Wed, 22 Jul 2020 21:21:16 GMT  
		Size: 256.0 KB (255977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47783e7ea018044b2c75ce172154e65072809be55a95a291093f770a8c261e75`  
		Last Modified: Wed, 22 Jul 2020 21:21:27 GMT  
		Size: 26.5 MB (26529324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9bba9be5aff5dfd8562a172dd933fd2bddcdbfc9c5cf46797c28e7f1d276576`  
		Last Modified: Wed, 22 Jul 2020 21:23:21 GMT  
		Size: 129.0 MB (128957837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm variant v7

```console
$ docker pull mono@sha256:0e79b73ff74791117dd0a42084eee5040160bdfa1d76e7e4cf2ffdd2b18b3cb9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.6 MB (172599115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a12c1996dc94982e4e9871cb355f1304e8c978c416bef75350d2fc25fb5fcad2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 01:33:30 GMT
ADD file:49b1a1b4f5c2201b0e23e29dca24c4f6ffc14620196c4bd77770952500c4bee1 in / 
# Wed, 22 Jul 2020 01:33:38 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 02:15:12 GMT
ENV MONO_VERSION=6.8.0.96
# Wed, 22 Jul 2020 02:15:59 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 22 Jul 2020 02:17:08 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 22 Jul 2020 02:24:59 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:cd38ad753522d120e27c5343b08f661ee3aebfe531d60102d7c624c16dba4d09`  
		Last Modified: Wed, 22 Jul 2020 01:44:24 GMT  
		Size: 19.3 MB (19298267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678b77b1123ed730afaccee19cb50f8fdf077e6011636b04af9cd365e6ebdf13`  
		Last Modified: Wed, 22 Jul 2020 02:32:32 GMT  
		Size: 244.6 KB (244569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ee2966b2ed591a8caba8af3012b33613fdcd2925dffc5f9eaa9328292c5af9`  
		Last Modified: Wed, 22 Jul 2020 02:32:40 GMT  
		Size: 24.5 MB (24495473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156d85b212d8926604522d94038ef09d4862f7a5aebd52d8f0c5e9546ef12c06`  
		Last Modified: Wed, 22 Jul 2020 02:34:24 GMT  
		Size: 128.6 MB (128560806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:5b229ee910d41136f26b4fb24e774ce778751f846e023acfd13481f13aaf480b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.3 MB (203299242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38c4746a1607b1fea5aedd8e27f9cd4cf4b52d846b634e1593a5deccdac7600f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:41:09 GMT
ADD file:1efd5b51a56f36bcf79a1bcea1df36ef28299a42bc11e758f9e49066f2a1f085 in / 
# Wed, 22 Jul 2020 00:41:10 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 05:21:19 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 23 Jul 2020 05:21:40 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 05:22:18 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 23 Jul 2020 05:27:01 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3999339def4d7591a8064bfc698302ae0e29bc5e0557ae392c122e1b3efa9305`  
		Last Modified: Wed, 22 Jul 2020 00:47:42 GMT  
		Size: 25.9 MB (25857826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072a4eb4e02ed79a5f02c37ff3909423a2376488a8c9f16c1d2a94ac58359078`  
		Last Modified: Thu, 23 Jul 2020 05:27:50 GMT  
		Size: 255.9 KB (255908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfeb41b8c951ba90f625eda71258c0aa6098d6281c21319a2db7cdf691d34fc`  
		Last Modified: Thu, 23 Jul 2020 05:28:00 GMT  
		Size: 31.7 MB (31748118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34df94ccaa6daaeb0c5cce32d31458a2550823303e09ca160f143178cd78a3ec`  
		Last Modified: Thu, 23 Jul 2020 05:29:48 GMT  
		Size: 145.4 MB (145437390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; 386

```console
$ docker pull mono@sha256:104b3ad8a26e6ce2f6829d32b6a39ae39bb6c586c0ae5fc2b6dee6cf6b40a3d8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.5 MB (230542185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f7e6a79136b95af481af9503fdaaa4cb19dc983225e59b060f2effacbf3878b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:09:15 GMT
ADD file:ee51bd8fcf2e02243de32c0f0e7899acebfa23bdceb783f13feb33c484ee98b8 in / 
# Wed, 22 Jul 2020 02:09:15 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 00:17:56 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 23 Jul 2020 00:18:08 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 00:18:59 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 23 Jul 2020 00:24:07 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:75157e9ef5a857d6b02d235e08a164737ad009bae299277f86131063e6204e0b`  
		Last Modified: Wed, 22 Jul 2020 02:15:45 GMT  
		Size: 27.8 MB (27754899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf3d2401f59eb0e901a248e7de7b81f6d0ce70dc8958450d9406575c5ae402a`  
		Last Modified: Thu, 23 Jul 2020 00:24:53 GMT  
		Size: 255.9 KB (255866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49c7cc3cfa683a1a7f140766f83ef1205f003c8f18a9e7dc6192211af762bdd`  
		Last Modified: Thu, 23 Jul 2020 00:25:12 GMT  
		Size: 71.1 MB (71134676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4814f34046c756d82b2e0956d1226d8adf44644864681f318e6d3cc6c3276b1a`  
		Last Modified: Thu, 23 Jul 2020 00:26:45 GMT  
		Size: 131.4 MB (131396744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; ppc64le

```console
$ docker pull mono@sha256:d869978f01d503070bd620fdbd1e1f69c88d9749580f61d4b81cf818f4c6958d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.1 MB (192091144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d9744232b7d0bd9e597e8dfaaf5e81c9ee17bc9a6fff9cf4b633939d80230fc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:16:05 GMT
ADD file:037dec996d9b742fc49f675272aa42ebd31f04226ba3d28836a6556cb61c29e7 in / 
# Wed, 22 Jul 2020 02:16:14 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 06:10:34 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 23 Jul 2020 06:12:20 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 06:14:21 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 23 Jul 2020 06:58:00 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d022338f917106731b8902d4c3d7009435a41381c11c8d210bbd6af007569f69`  
		Last Modified: Wed, 22 Jul 2020 02:26:01 GMT  
		Size: 30.5 MB (30524562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a35a0ce279229326ca6a3a4114458fe3e7a42a86875ae4b3f3e6a8a914127f`  
		Last Modified: Thu, 23 Jul 2020 06:59:10 GMT  
		Size: 256.2 KB (256204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c409da6637fbd5bae065a688f5b8fa5bca60053859e7f816079c977f9193411c`  
		Last Modified: Thu, 23 Jul 2020 06:59:18 GMT  
		Size: 29.3 MB (29349424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857181e3045e28d43363265a023c6a51347e982d06b1ce96ce27aae83e425231`  
		Last Modified: Thu, 23 Jul 2020 07:00:47 GMT  
		Size: 132.0 MB (131960954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:slim`

```console
$ docker pull mono@sha256:4c09ae1b53e6cb0f9c15da768c7d29a26b5c4cc1deead2fcad57bda4b6ee5ed3
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
$ docker pull mono@sha256:8662fe5f43ce6662afc770942a78620711529e22bfb3a6915d08de61f0391b0c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.2 MB (87227423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c8044236c95b15c23c907be455632697f74ca4ba4e6a5836dd26b5d9b5cbcd4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:07:07 GMT
ADD file:c11db0b135382f4c5b0f55b50740639bd8c1a22153b931b409cb9e41136734f2 in / 
# Wed, 22 Jul 2020 02:07:07 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 19:26:50 GMT
ENV MONO_VERSION=6.8.0.96
# Wed, 22 Jul 2020 19:26:59 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 22 Jul 2020 19:27:42 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:cbd31ae332794bb723708526045b062b2fe6a08ccc0f143ea7dc18e0ebe46dea`  
		Last Modified: Wed, 22 Jul 2020 02:12:25 GMT  
		Size: 22.5 MB (22515635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fa40bfbf0082f2bae5777ccd52f3ca2add17d21a2375de40cb7b6a738aee92a`  
		Last Modified: Wed, 22 Jul 2020 20:02:10 GMT  
		Size: 244.5 KB (244495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989dabcb56d661ce7dac9d54d0c22d40088fb13ced11ca7807786cd9cd61431d`  
		Last Modified: Wed, 22 Jul 2020 20:02:28 GMT  
		Size: 64.5 MB (64467293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:bfbf7d0dd6ec900bd4fb046e1171472d0cc6b4bc32c10095bcc1718d0d2fb4f3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51622762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0887bb40baf7e1ebaa4491740009839e418df248c2f18e393048574e7a3283aa`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:51:01 GMT
ADD file:4ea2d111c970d510f4eccf0fa08caafde1d227fc4c249d67c1b9d99998b0b906 in / 
# Wed, 22 Jul 2020 00:51:04 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 21:12:42 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 22 Jul 2020 21:13:14 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 22 Jul 2020 21:14:39 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7ae4223cfc253e8d54407ec654ed8fb606352daea8da124f33dacd17626259ad`  
		Last Modified: Wed, 22 Jul 2020 00:58:53 GMT  
		Size: 24.8 MB (24837461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b201b7c93f2f75a8f765155e3fd569dbc95a79c57c644b4595e1eff9afe8e9`  
		Last Modified: Wed, 22 Jul 2020 21:21:16 GMT  
		Size: 256.0 KB (255977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47783e7ea018044b2c75ce172154e65072809be55a95a291093f770a8c261e75`  
		Last Modified: Wed, 22 Jul 2020 21:21:27 GMT  
		Size: 26.5 MB (26529324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:43efe3765087680c99e00ef8f63dd9f8d1ba2a569c9a8af61dc54a18d82f9cc6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (44038309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:777fd2ade7d45508d862b53c0c85624224196846719397190648e897a2222b24`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 01:33:30 GMT
ADD file:49b1a1b4f5c2201b0e23e29dca24c4f6ffc14620196c4bd77770952500c4bee1 in / 
# Wed, 22 Jul 2020 01:33:38 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 02:15:12 GMT
ENV MONO_VERSION=6.8.0.96
# Wed, 22 Jul 2020 02:15:59 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 22 Jul 2020 02:17:08 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:cd38ad753522d120e27c5343b08f661ee3aebfe531d60102d7c624c16dba4d09`  
		Last Modified: Wed, 22 Jul 2020 01:44:24 GMT  
		Size: 19.3 MB (19298267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678b77b1123ed730afaccee19cb50f8fdf077e6011636b04af9cd365e6ebdf13`  
		Last Modified: Wed, 22 Jul 2020 02:32:32 GMT  
		Size: 244.6 KB (244569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ee2966b2ed591a8caba8af3012b33613fdcd2925dffc5f9eaa9328292c5af9`  
		Last Modified: Wed, 22 Jul 2020 02:32:40 GMT  
		Size: 24.5 MB (24495473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:90c6e2ff8ea8544e22e0263aff48c2e93d9b0d5744988b3450b239c9a01bce98
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57861852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9eaeca8f8945189ca2b07c8c7261bb0dcfea6c27e322fe4f79f9e4bbb082dbb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:41:09 GMT
ADD file:1efd5b51a56f36bcf79a1bcea1df36ef28299a42bc11e758f9e49066f2a1f085 in / 
# Wed, 22 Jul 2020 00:41:10 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 05:21:19 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 23 Jul 2020 05:21:40 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 05:22:18 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3999339def4d7591a8064bfc698302ae0e29bc5e0557ae392c122e1b3efa9305`  
		Last Modified: Wed, 22 Jul 2020 00:47:42 GMT  
		Size: 25.9 MB (25857826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072a4eb4e02ed79a5f02c37ff3909423a2376488a8c9f16c1d2a94ac58359078`  
		Last Modified: Thu, 23 Jul 2020 05:27:50 GMT  
		Size: 255.9 KB (255908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfeb41b8c951ba90f625eda71258c0aa6098d6281c21319a2db7cdf691d34fc`  
		Last Modified: Thu, 23 Jul 2020 05:28:00 GMT  
		Size: 31.7 MB (31748118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; 386

```console
$ docker pull mono@sha256:832edc5e755243979388a770f2a26b002ff53970f4d5980d4646408b83977600
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99145441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0acbbfdbc517756895fa8f98bd81276148a67102797ffbda89f1c47569e381a4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:09:15 GMT
ADD file:ee51bd8fcf2e02243de32c0f0e7899acebfa23bdceb783f13feb33c484ee98b8 in / 
# Wed, 22 Jul 2020 02:09:15 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 00:17:56 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 23 Jul 2020 00:18:08 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 00:18:59 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:75157e9ef5a857d6b02d235e08a164737ad009bae299277f86131063e6204e0b`  
		Last Modified: Wed, 22 Jul 2020 02:15:45 GMT  
		Size: 27.8 MB (27754899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf3d2401f59eb0e901a248e7de7b81f6d0ce70dc8958450d9406575c5ae402a`  
		Last Modified: Thu, 23 Jul 2020 00:24:53 GMT  
		Size: 255.9 KB (255866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49c7cc3cfa683a1a7f140766f83ef1205f003c8f18a9e7dc6192211af762bdd`  
		Last Modified: Thu, 23 Jul 2020 00:25:12 GMT  
		Size: 71.1 MB (71134676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; ppc64le

```console
$ docker pull mono@sha256:305c285592ef4afd7c1e21fc7f28ec09f07868e0d8f8fad13e56251960215f56
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60130190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe7500199f77ce97cf00689537fd03120b78b47c57f1894538baaf0659deafc3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:16:05 GMT
ADD file:037dec996d9b742fc49f675272aa42ebd31f04226ba3d28836a6556cb61c29e7 in / 
# Wed, 22 Jul 2020 02:16:14 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 06:10:34 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 23 Jul 2020 06:12:20 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 06:14:21 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d022338f917106731b8902d4c3d7009435a41381c11c8d210bbd6af007569f69`  
		Last Modified: Wed, 22 Jul 2020 02:26:01 GMT  
		Size: 30.5 MB (30524562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a35a0ce279229326ca6a3a4114458fe3e7a42a86875ae4b3f3e6a8a914127f`  
		Last Modified: Thu, 23 Jul 2020 06:59:10 GMT  
		Size: 256.2 KB (256204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c409da6637fbd5bae065a688f5b8fa5bca60053859e7f816079c977f9193411c`  
		Last Modified: Thu, 23 Jul 2020 06:59:18 GMT  
		Size: 29.3 MB (29349424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
