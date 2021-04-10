## `mono:latest`

```console
$ docker pull mono@sha256:bd266fa809c7e9b148a53aa7c36157cd4a22a05ec631843019cd5345317bef22
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
$ docker pull mono@sha256:a907f08ee7b97b99076416102612a62ecc128c575bdf9f17ae4b75316fdb54b1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.0 MB (235965128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e97654e2d018e2693f321317dd3f3deb9f4b92364bf7e67bdee6fe9d92f097c`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 07:05:13 GMT
ENV MONO_VERSION=6.12.0.107
# Sat, 10 Apr 2021 07:05:23 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 10 Apr 2021 07:05:50 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 10 Apr 2021 07:12:24 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1999a1b7f77598c21d19a1e89d7b913e457ac0a17d81d92123b65de90b07930`  
		Last Modified: Sat, 10 Apr 2021 07:19:03 GMT  
		Size: 256.0 KB (256040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d013baec2808005a044268ed2ca1dad601ca737e0964ea26eb1c02b109fd6a5`  
		Last Modified: Sat, 10 Apr 2021 07:19:18 GMT  
		Size: 67.1 MB (67128789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809cff9cd7596c2dcd1a99dca66dd24ff93577a1668b1bafeb8b186ac9c53751`  
		Last Modified: Sat, 10 Apr 2021 07:20:36 GMT  
		Size: 141.4 MB (141440926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm variant v5

```console
$ docker pull mono@sha256:c4d39e8b29becc80d28151f430c3c27d8c7793819d1e74efd983d96682acdad6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.8 MB (191786558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:018c393fc188c91d03021c37f548e320f8ca728a07c262ef913b6b911ea11b7b`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 00:51:31 GMT
ADD file:926533a23a69aa2481a9122b667bb6300a347154eea366c9e679a230aa7f373a in / 
# Sat, 10 Apr 2021 00:51:34 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:52:52 GMT
ENV MONO_VERSION=6.12.0.107
# Sat, 10 Apr 2021 02:53:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 10 Apr 2021 02:54:23 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 10 Apr 2021 02:59:49 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:33d77752597b664d047cc829e58a223d6fb077b61f69ca0462fcfb9b78d5f69b`  
		Last Modified: Sat, 10 Apr 2021 00:59:22 GMT  
		Size: 24.9 MB (24873199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:720e2aaceefa4a873c7c857f40468834c05412aad1c2b0a15ae0dc0769d0f919`  
		Last Modified: Sat, 10 Apr 2021 03:03:49 GMT  
		Size: 256.0 KB (256010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e892e552e01288c895d951dd62438acfd38809f969cbf59ad1d6a90e4e55cbdb`  
		Last Modified: Sat, 10 Apr 2021 03:03:59 GMT  
		Size: 26.6 MB (26550285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457156801dee2ad1168b42679714d72b71bae44a51b362d7f72c8a72d7c0185f`  
		Last Modified: Sat, 10 Apr 2021 03:05:18 GMT  
		Size: 140.1 MB (140107064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm variant v7

```console
$ docker pull mono@sha256:37bed4aae0165bf8cdc2ec35cda4585aa3d45675d6210cc2b5e4a99b27a995d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.7 MB (187672912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ba418b8af22818a8aaaa279b7b2f7808af5c9f847c1e94d8f9079ce48175839`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 23:08:38 GMT
ADD file:c1eeb99fc8ec483e175d4948a58d7f7b246b0d6b887f435a5fef07ef43699f76 in / 
# Tue, 30 Mar 2021 23:08:41 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 02:09:19 GMT
ENV MONO_VERSION=6.12.0.107
# Wed, 31 Mar 2021 02:09:39 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 31 Mar 2021 02:10:22 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 31 Mar 2021 02:14:21 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:ee0a2cc24f2963b99b1d30dc2613f196b7c9e38337cf99332d6c4efe07f01ef2`  
		Last Modified: Tue, 30 Mar 2021 23:16:25 GMT  
		Size: 22.7 MB (22739814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2630b9e89b3f8e8bf5cf459714f0533e6965dd6f7a15c681f983fd753a5052`  
		Last Modified: Wed, 31 Mar 2021 02:17:26 GMT  
		Size: 256.0 KB (256007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:688600d68f090a392c73014c7e4218a813575f2ab38e51dbe586c894b269087d`  
		Last Modified: Wed, 31 Mar 2021 02:17:36 GMT  
		Size: 25.7 MB (25738177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2c49c3ba5fae015dc4d96f60186f4f4130581809c6f9b54c601500bc7876cb`  
		Last Modified: Wed, 31 Mar 2021 02:18:55 GMT  
		Size: 138.9 MB (138938914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:d784042772d2e3cb6e1e241ea78e8686b9770e0b762ba7df39e78921c0ed1410
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.5 MB (214513898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e70979a0507c5de77bbd1a9feeb71cb8197cb233cbdbca67b9ce1cf48b85b18b`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 04:54:39 GMT
ENV MONO_VERSION=6.12.0.107
# Sat, 10 Apr 2021 04:54:56 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 10 Apr 2021 04:55:32 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 10 Apr 2021 04:59:03 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd73d6fc5dac446511d3a48cff332c18151a90a2576c1bfd72c9fbd0b1d83941`  
		Last Modified: Sat, 10 Apr 2021 05:03:05 GMT  
		Size: 256.0 KB (255975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1344864508837079b091b1985cbd427cf50cc7fd4c9db89bb63794c0c37d45e1`  
		Last Modified: Sat, 10 Apr 2021 05:03:17 GMT  
		Size: 31.8 MB (31769620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027318f7594b4b43c325c83d7b7af05cdcdc7724376a525e30c89281cfa2d25e`  
		Last Modified: Sat, 10 Apr 2021 05:04:26 GMT  
		Size: 156.6 MB (156583721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; 386

```console
$ docker pull mono@sha256:f4cb1db0d040dd5b85d46b394d0c63b669ab9470562febc1ce578ae4d4aab49b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.7 MB (241744613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f97b84c3680a0620d995a7d5b8bbc4f257ce8fdf83631ab872b799b3e582de08`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 03:36:04 GMT
ENV MONO_VERSION=6.12.0.107
# Sat, 10 Apr 2021 03:36:14 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 10 Apr 2021 03:37:03 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 10 Apr 2021 03:40:41 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7162f55592356e6498db09350cbd0eed4d3ca9241f21e7ddf9640db656dde818`  
		Last Modified: Sat, 10 Apr 2021 03:44:06 GMT  
		Size: 256.0 KB (255986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01be4b47ded17f73764615cb010652d1c1b5dd07ce2b85946c2380761eb688e`  
		Last Modified: Sat, 10 Apr 2021 03:44:22 GMT  
		Size: 71.2 MB (71153041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a28ff6a785da4117ae9f222c8ef9d22fdea41fcf637c85ea3debba87c2977528`  
		Last Modified: Sat, 10 Apr 2021 03:46:10 GMT  
		Size: 142.5 MB (142546599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; ppc64le

```console
$ docker pull mono@sha256:e83bfecb77a4d1a3ff95873841da5f72e0500e73cd3160b8acdfdb4e4b4725e2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.4 MB (203383810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4d31fce9c515dacbd574c76a19c91e0c76e026062a93a65ba8530955ab93e51`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 05:29:52 GMT
ENV MONO_VERSION=6.12.0.107
# Sat, 10 Apr 2021 05:31:38 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 10 Apr 2021 05:33:15 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Sat, 10 Apr 2021 05:47:09 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3e1e599482ca47095f85e429b346b76375aa85015ddcca050e85c2a8b1fdda9c`  
		Last Modified: Sat, 10 Apr 2021 01:33:57 GMT  
		Size: 30.5 MB (30545933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fa3e7238a242e143bbbc08aa959435df2e54e74e3489d8ab16d3913518fb586`  
		Last Modified: Sat, 10 Apr 2021 05:56:05 GMT  
		Size: 256.2 KB (256195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce7b7af0750c311ddcedf2058d1ccf03b2ef0f98c006d70cfcc73a1662d7e60`  
		Last Modified: Sat, 10 Apr 2021 05:56:11 GMT  
		Size: 29.4 MB (29358138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25d10b4273c3857550ad27aec4d23b961ec7acecec6eab1650dd1bd82f06e9f`  
		Last Modified: Sat, 10 Apr 2021 05:57:16 GMT  
		Size: 143.2 MB (143223544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
