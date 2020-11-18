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
$ docker pull mono@sha256:e1c39d26dc47f212bc8ba5bfd282526987f2c9f7a1a124fb7dd2badb9c3e44dc
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
$ docker pull mono@sha256:0beb1b5ba9a0cc0efaaa1148c2682d02351ffb94d77ee74ec5e2fedb625bdd17
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.7 MB (224728267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ffb04a492e34192512ff718aaf68247effd38c5ee58e852b67e750455ca46a3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:07:49 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 08:08:00 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 08:08:57 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Oct 2020 08:28:43 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f42b4ad878bfc3887ec056c31544fe7c67286e2cbf905efd97752fb01bf7cf`  
		Last Modified: Tue, 13 Oct 2020 08:29:21 GMT  
		Size: 255.9 KB (255885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595630826b1b79ee45e4c4202b61c61ada9c53bf1352e06571dbaa4624660c6f`  
		Last Modified: Tue, 13 Oct 2020 08:29:34 GMT  
		Size: 67.1 MB (67092282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f179adbd59957f8069efb25f4b87a0c78f7120ca6935479e58a6c9f0d0f75253`  
		Last Modified: Tue, 13 Oct 2020 08:30:39 GMT  
		Size: 130.3 MB (130287872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; arm variant v5

```console
$ docker pull mono@sha256:3e601afbb4577fd538dfa06145643ef0c370d3b98b7fdbdeb8e69e6e7c3cc44b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180580641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0b1583a0f54587294ef3fb13293551714e84d35168baa3b742491aac91dc394`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:52:17 GMT
ADD file:b71c0fa4957d6b65af37231a105f3d17cdbafe5c7d6c37b5843ebf619c608aaa in / 
# Tue, 13 Oct 2020 01:52:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:36:19 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 02:36:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 02:37:31 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Oct 2020 02:44:00 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f991c1e1ee2c48f16625b6b61310bf3c0616c0dbda4762019117e86fd29cf9ce`  
		Last Modified: Tue, 13 Oct 2020 02:01:27 GMT  
		Size: 24.8 MB (24835992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27e131b9898d8f02267f410169b8627b889f6585ad9300d14a4775194301b55`  
		Last Modified: Tue, 13 Oct 2020 02:44:49 GMT  
		Size: 255.9 KB (255938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b82cc14a51474e2d05a0fd59b3fde70aa8fda539de5a302992983e4ffce7b8`  
		Last Modified: Tue, 13 Oct 2020 02:45:01 GMT  
		Size: 26.5 MB (26530650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94ad0d9899e6c5c16486a97103eb9bbff1261c084ef2366534ae27653b23704`  
		Last Modified: Tue, 13 Oct 2020 02:46:59 GMT  
		Size: 129.0 MB (128958061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; arm variant v7

```console
$ docker pull mono@sha256:0e797969122f94b85e9178dd9bece13c7ebd2cacf124520f4275e0ac7cd2b15d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.5 MB (176483530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b81a3bb43255d115e920754f87906a5cd00c5c5ae23a85f06c756f2c42a455b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 00:59:29 GMT
ADD file:e423f30ca19eb205a98de21b0545d0a764cfc4f832a9a9631542354d914d98d9 in / 
# Tue, 13 Oct 2020 00:59:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 04:43:09 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 04:43:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 04:44:11 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Oct 2020 04:49:53 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d6d8411ad43db0022fa0fce094cd2e8b1dd2f8a09d6880ed9beb6b4204867027`  
		Last Modified: Tue, 13 Oct 2020 01:08:28 GMT  
		Size: 22.7 MB (22699849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5228b93feed3135603bc1b4bbda140b6e3e712167c9dd5ccaad1732370cd6b93`  
		Last Modified: Tue, 13 Oct 2020 04:50:37 GMT  
		Size: 255.9 KB (255921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e85494910fa31cd3bb70be77361cab8fa0b333de462a10ce0e2181ee165c0a`  
		Last Modified: Tue, 13 Oct 2020 04:50:46 GMT  
		Size: 25.7 MB (25729327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0179ccf237338944b3401bc8ed480a53bd10956472cd41d05647aeb7fa46ee`  
		Last Modified: Tue, 13 Oct 2020 04:52:43 GMT  
		Size: 127.8 MB (127798433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:0b5ce90bc0624cc3be76e2f4faa9b5ece9459fbda3fd2d1e600b0d03a6693710
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.3 MB (203308506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:684f822e67b92095a97967c053ec1acb78c5d01f5ca24b36822f3fee9136d53f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:31 GMT
ADD file:a70d8c01f8f04f36038968567af779883f3b5ba3147b662b7d170d80418bc23c in / 
# Tue, 17 Nov 2020 20:23:32 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 01:28:53 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 18 Nov 2020 01:29:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 18 Nov 2020 01:29:56 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 18 Nov 2020 01:35:25 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:29ade854e0dcedde295dd89890d45271e9df839e42124558eb5283508ca70f5c`  
		Last Modified: Tue, 17 Nov 2020 20:32:02 GMT  
		Size: 25.9 MB (25862532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808368e9cd11971fa6e53b4a3fbb5559d120515e05c721adff9b9e493870a0f5`  
		Last Modified: Wed, 18 Nov 2020 01:36:25 GMT  
		Size: 255.9 KB (255886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cdf6ac0c679ba4beaf9bad32b903763540d340a1b59395c930a56b288947efe`  
		Last Modified: Wed, 18 Nov 2020 01:36:35 GMT  
		Size: 31.8 MB (31750189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85a8c7edd4b4a3cbd35f220923da50329be4d48bbff3d793963214b91d5e4c9`  
		Last Modified: Wed, 18 Nov 2020 01:38:19 GMT  
		Size: 145.4 MB (145439899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; 386

```console
$ docker pull mono@sha256:134601059016d772aac04e8b006c0467d93094aac62ec0a5a003779f5efb06d0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.5 MB (230532788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c942123328c3a3ae3a83555749eec2e9c668cc58f1cf9a219c5fbff2e472441`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:03 GMT
ADD file:51108b89c70ce0773c897be520c84454660f38b84ba556da49c7fe77e5d52416 in / 
# Tue, 13 Oct 2020 01:41:03 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 07:38:18 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 07:38:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 07:39:07 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Oct 2020 07:44:16 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:97e4efec21eea92209464547d0f52a0f773c505cf4ea9d8090cef667bde145b8`  
		Last Modified: Tue, 13 Oct 2020 01:48:54 GMT  
		Size: 27.8 MB (27750243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9588b02c60fba169bd9cad455764e725c295ddf21085d904d732ef4892d6375f`  
		Last Modified: Tue, 13 Oct 2020 07:45:04 GMT  
		Size: 255.8 KB (255832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf75edd8ea102d6fbbdb5609df6a19925523bdb561e696bd0fb665b5bb2c5a7`  
		Last Modified: Tue, 13 Oct 2020 07:45:21 GMT  
		Size: 71.1 MB (71136124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6087ce14b6fee3f871defe577ae84bcf6db5fe3226dc585305fa9ce5c625d41`  
		Last Modified: Tue, 13 Oct 2020 07:46:42 GMT  
		Size: 131.4 MB (131390589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; ppc64le

```console
$ docker pull mono@sha256:5d8d2256088dfe9d8870d0ad3a58c3bd5428ae3f6f47046f14c4009fad3cdddc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.1 MB (192080743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee6e47cfbad6be2c8b92dd6b5d33888766804f9cdc59ee9042f56068e1499de9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:54 GMT
ADD file:9992867f855c9bed54df6d26f3d8076689aff8a51e808fefba7d3b66dab250e5 in / 
# Tue, 13 Oct 2020 01:38:59 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 10:20:33 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 10:21:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 10:23:38 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Oct 2020 10:40:36 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:523555c6877c72cfcdec912b4d0053c298b1c97835efc7c6b0211585a06bd563`  
		Last Modified: Tue, 13 Oct 2020 01:50:10 GMT  
		Size: 30.5 MB (30517878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6778a79cc5707eb6c5a21cff2f3f04a05c0ba40bc48c3b3b97f695441e2695fe`  
		Last Modified: Tue, 13 Oct 2020 10:42:46 GMT  
		Size: 256.1 KB (256132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29be084b2430b8c354483c0ac192dd08a2e22fd9687a53e928bf6126d0703187`  
		Last Modified: Tue, 13 Oct 2020 10:43:40 GMT  
		Size: 29.3 MB (29349822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89fb777ba4b2b8e659779b45eedfc16ba2052f25ece387db17ba60fd460c08d4`  
		Last Modified: Tue, 13 Oct 2020 10:47:49 GMT  
		Size: 132.0 MB (131956911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10`

```console
$ docker pull mono@sha256:e1c39d26dc47f212bc8ba5bfd282526987f2c9f7a1a124fb7dd2badb9c3e44dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.10` - linux; amd64

```console
$ docker pull mono@sha256:0beb1b5ba9a0cc0efaaa1148c2682d02351ffb94d77ee74ec5e2fedb625bdd17
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.7 MB (224728267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ffb04a492e34192512ff718aaf68247effd38c5ee58e852b67e750455ca46a3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:07:49 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 08:08:00 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 08:08:57 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Oct 2020 08:28:43 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f42b4ad878bfc3887ec056c31544fe7c67286e2cbf905efd97752fb01bf7cf`  
		Last Modified: Tue, 13 Oct 2020 08:29:21 GMT  
		Size: 255.9 KB (255885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595630826b1b79ee45e4c4202b61c61ada9c53bf1352e06571dbaa4624660c6f`  
		Last Modified: Tue, 13 Oct 2020 08:29:34 GMT  
		Size: 67.1 MB (67092282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f179adbd59957f8069efb25f4b87a0c78f7120ca6935479e58a6c9f0d0f75253`  
		Last Modified: Tue, 13 Oct 2020 08:30:39 GMT  
		Size: 130.3 MB (130287872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; arm variant v5

```console
$ docker pull mono@sha256:3e601afbb4577fd538dfa06145643ef0c370d3b98b7fdbdeb8e69e6e7c3cc44b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180580641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0b1583a0f54587294ef3fb13293551714e84d35168baa3b742491aac91dc394`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:52:17 GMT
ADD file:b71c0fa4957d6b65af37231a105f3d17cdbafe5c7d6c37b5843ebf619c608aaa in / 
# Tue, 13 Oct 2020 01:52:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:36:19 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 02:36:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 02:37:31 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Oct 2020 02:44:00 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f991c1e1ee2c48f16625b6b61310bf3c0616c0dbda4762019117e86fd29cf9ce`  
		Last Modified: Tue, 13 Oct 2020 02:01:27 GMT  
		Size: 24.8 MB (24835992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27e131b9898d8f02267f410169b8627b889f6585ad9300d14a4775194301b55`  
		Last Modified: Tue, 13 Oct 2020 02:44:49 GMT  
		Size: 255.9 KB (255938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b82cc14a51474e2d05a0fd59b3fde70aa8fda539de5a302992983e4ffce7b8`  
		Last Modified: Tue, 13 Oct 2020 02:45:01 GMT  
		Size: 26.5 MB (26530650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94ad0d9899e6c5c16486a97103eb9bbff1261c084ef2366534ae27653b23704`  
		Last Modified: Tue, 13 Oct 2020 02:46:59 GMT  
		Size: 129.0 MB (128958061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; arm variant v7

```console
$ docker pull mono@sha256:0e797969122f94b85e9178dd9bece13c7ebd2cacf124520f4275e0ac7cd2b15d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.5 MB (176483530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b81a3bb43255d115e920754f87906a5cd00c5c5ae23a85f06c756f2c42a455b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 00:59:29 GMT
ADD file:e423f30ca19eb205a98de21b0545d0a764cfc4f832a9a9631542354d914d98d9 in / 
# Tue, 13 Oct 2020 00:59:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 04:43:09 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 04:43:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 04:44:11 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Oct 2020 04:49:53 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d6d8411ad43db0022fa0fce094cd2e8b1dd2f8a09d6880ed9beb6b4204867027`  
		Last Modified: Tue, 13 Oct 2020 01:08:28 GMT  
		Size: 22.7 MB (22699849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5228b93feed3135603bc1b4bbda140b6e3e712167c9dd5ccaad1732370cd6b93`  
		Last Modified: Tue, 13 Oct 2020 04:50:37 GMT  
		Size: 255.9 KB (255921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e85494910fa31cd3bb70be77361cab8fa0b333de462a10ce0e2181ee165c0a`  
		Last Modified: Tue, 13 Oct 2020 04:50:46 GMT  
		Size: 25.7 MB (25729327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0179ccf237338944b3401bc8ed480a53bd10956472cd41d05647aeb7fa46ee`  
		Last Modified: Tue, 13 Oct 2020 04:52:43 GMT  
		Size: 127.8 MB (127798433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:0b5ce90bc0624cc3be76e2f4faa9b5ece9459fbda3fd2d1e600b0d03a6693710
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.3 MB (203308506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:684f822e67b92095a97967c053ec1acb78c5d01f5ca24b36822f3fee9136d53f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:31 GMT
ADD file:a70d8c01f8f04f36038968567af779883f3b5ba3147b662b7d170d80418bc23c in / 
# Tue, 17 Nov 2020 20:23:32 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 01:28:53 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 18 Nov 2020 01:29:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 18 Nov 2020 01:29:56 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 18 Nov 2020 01:35:25 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:29ade854e0dcedde295dd89890d45271e9df839e42124558eb5283508ca70f5c`  
		Last Modified: Tue, 17 Nov 2020 20:32:02 GMT  
		Size: 25.9 MB (25862532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808368e9cd11971fa6e53b4a3fbb5559d120515e05c721adff9b9e493870a0f5`  
		Last Modified: Wed, 18 Nov 2020 01:36:25 GMT  
		Size: 255.9 KB (255886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cdf6ac0c679ba4beaf9bad32b903763540d340a1b59395c930a56b288947efe`  
		Last Modified: Wed, 18 Nov 2020 01:36:35 GMT  
		Size: 31.8 MB (31750189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85a8c7edd4b4a3cbd35f220923da50329be4d48bbff3d793963214b91d5e4c9`  
		Last Modified: Wed, 18 Nov 2020 01:38:19 GMT  
		Size: 145.4 MB (145439899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; 386

```console
$ docker pull mono@sha256:134601059016d772aac04e8b006c0467d93094aac62ec0a5a003779f5efb06d0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.5 MB (230532788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c942123328c3a3ae3a83555749eec2e9c668cc58f1cf9a219c5fbff2e472441`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:03 GMT
ADD file:51108b89c70ce0773c897be520c84454660f38b84ba556da49c7fe77e5d52416 in / 
# Tue, 13 Oct 2020 01:41:03 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 07:38:18 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 07:38:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 07:39:07 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Oct 2020 07:44:16 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:97e4efec21eea92209464547d0f52a0f773c505cf4ea9d8090cef667bde145b8`  
		Last Modified: Tue, 13 Oct 2020 01:48:54 GMT  
		Size: 27.8 MB (27750243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9588b02c60fba169bd9cad455764e725c295ddf21085d904d732ef4892d6375f`  
		Last Modified: Tue, 13 Oct 2020 07:45:04 GMT  
		Size: 255.8 KB (255832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf75edd8ea102d6fbbdb5609df6a19925523bdb561e696bd0fb665b5bb2c5a7`  
		Last Modified: Tue, 13 Oct 2020 07:45:21 GMT  
		Size: 71.1 MB (71136124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6087ce14b6fee3f871defe577ae84bcf6db5fe3226dc585305fa9ce5c625d41`  
		Last Modified: Tue, 13 Oct 2020 07:46:42 GMT  
		Size: 131.4 MB (131390589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; ppc64le

```console
$ docker pull mono@sha256:5d8d2256088dfe9d8870d0ad3a58c3bd5428ae3f6f47046f14c4009fad3cdddc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.1 MB (192080743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee6e47cfbad6be2c8b92dd6b5d33888766804f9cdc59ee9042f56068e1499de9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:54 GMT
ADD file:9992867f855c9bed54df6d26f3d8076689aff8a51e808fefba7d3b66dab250e5 in / 
# Tue, 13 Oct 2020 01:38:59 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 10:20:33 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 10:21:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 10:23:38 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Oct 2020 10:40:36 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:523555c6877c72cfcdec912b4d0053c298b1c97835efc7c6b0211585a06bd563`  
		Last Modified: Tue, 13 Oct 2020 01:50:10 GMT  
		Size: 30.5 MB (30517878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6778a79cc5707eb6c5a21cff2f3f04a05c0ba40bc48c3b3b97f695441e2695fe`  
		Last Modified: Tue, 13 Oct 2020 10:42:46 GMT  
		Size: 256.1 KB (256132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29be084b2430b8c354483c0ac192dd08a2e22fd9687a53e928bf6126d0703187`  
		Last Modified: Tue, 13 Oct 2020 10:43:40 GMT  
		Size: 29.3 MB (29349822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89fb777ba4b2b8e659779b45eedfc16ba2052f25ece387db17ba60fd460c08d4`  
		Last Modified: Tue, 13 Oct 2020 10:47:49 GMT  
		Size: 132.0 MB (131956911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10.0`

```console
$ docker pull mono@sha256:e1c39d26dc47f212bc8ba5bfd282526987f2c9f7a1a124fb7dd2badb9c3e44dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.10.0` - linux; amd64

```console
$ docker pull mono@sha256:0beb1b5ba9a0cc0efaaa1148c2682d02351ffb94d77ee74ec5e2fedb625bdd17
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.7 MB (224728267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ffb04a492e34192512ff718aaf68247effd38c5ee58e852b67e750455ca46a3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:07:49 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 08:08:00 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 08:08:57 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Oct 2020 08:28:43 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f42b4ad878bfc3887ec056c31544fe7c67286e2cbf905efd97752fb01bf7cf`  
		Last Modified: Tue, 13 Oct 2020 08:29:21 GMT  
		Size: 255.9 KB (255885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595630826b1b79ee45e4c4202b61c61ada9c53bf1352e06571dbaa4624660c6f`  
		Last Modified: Tue, 13 Oct 2020 08:29:34 GMT  
		Size: 67.1 MB (67092282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f179adbd59957f8069efb25f4b87a0c78f7120ca6935479e58a6c9f0d0f75253`  
		Last Modified: Tue, 13 Oct 2020 08:30:39 GMT  
		Size: 130.3 MB (130287872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; arm variant v5

```console
$ docker pull mono@sha256:3e601afbb4577fd538dfa06145643ef0c370d3b98b7fdbdeb8e69e6e7c3cc44b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180580641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0b1583a0f54587294ef3fb13293551714e84d35168baa3b742491aac91dc394`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:52:17 GMT
ADD file:b71c0fa4957d6b65af37231a105f3d17cdbafe5c7d6c37b5843ebf619c608aaa in / 
# Tue, 13 Oct 2020 01:52:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:36:19 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 02:36:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 02:37:31 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Oct 2020 02:44:00 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f991c1e1ee2c48f16625b6b61310bf3c0616c0dbda4762019117e86fd29cf9ce`  
		Last Modified: Tue, 13 Oct 2020 02:01:27 GMT  
		Size: 24.8 MB (24835992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27e131b9898d8f02267f410169b8627b889f6585ad9300d14a4775194301b55`  
		Last Modified: Tue, 13 Oct 2020 02:44:49 GMT  
		Size: 255.9 KB (255938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b82cc14a51474e2d05a0fd59b3fde70aa8fda539de5a302992983e4ffce7b8`  
		Last Modified: Tue, 13 Oct 2020 02:45:01 GMT  
		Size: 26.5 MB (26530650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94ad0d9899e6c5c16486a97103eb9bbff1261c084ef2366534ae27653b23704`  
		Last Modified: Tue, 13 Oct 2020 02:46:59 GMT  
		Size: 129.0 MB (128958061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; arm variant v7

```console
$ docker pull mono@sha256:0e797969122f94b85e9178dd9bece13c7ebd2cacf124520f4275e0ac7cd2b15d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.5 MB (176483530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b81a3bb43255d115e920754f87906a5cd00c5c5ae23a85f06c756f2c42a455b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 00:59:29 GMT
ADD file:e423f30ca19eb205a98de21b0545d0a764cfc4f832a9a9631542354d914d98d9 in / 
# Tue, 13 Oct 2020 00:59:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 04:43:09 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 04:43:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 04:44:11 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Oct 2020 04:49:53 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d6d8411ad43db0022fa0fce094cd2e8b1dd2f8a09d6880ed9beb6b4204867027`  
		Last Modified: Tue, 13 Oct 2020 01:08:28 GMT  
		Size: 22.7 MB (22699849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5228b93feed3135603bc1b4bbda140b6e3e712167c9dd5ccaad1732370cd6b93`  
		Last Modified: Tue, 13 Oct 2020 04:50:37 GMT  
		Size: 255.9 KB (255921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e85494910fa31cd3bb70be77361cab8fa0b333de462a10ce0e2181ee165c0a`  
		Last Modified: Tue, 13 Oct 2020 04:50:46 GMT  
		Size: 25.7 MB (25729327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0179ccf237338944b3401bc8ed480a53bd10956472cd41d05647aeb7fa46ee`  
		Last Modified: Tue, 13 Oct 2020 04:52:43 GMT  
		Size: 127.8 MB (127798433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:0b5ce90bc0624cc3be76e2f4faa9b5ece9459fbda3fd2d1e600b0d03a6693710
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.3 MB (203308506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:684f822e67b92095a97967c053ec1acb78c5d01f5ca24b36822f3fee9136d53f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:31 GMT
ADD file:a70d8c01f8f04f36038968567af779883f3b5ba3147b662b7d170d80418bc23c in / 
# Tue, 17 Nov 2020 20:23:32 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 01:28:53 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 18 Nov 2020 01:29:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 18 Nov 2020 01:29:56 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 18 Nov 2020 01:35:25 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:29ade854e0dcedde295dd89890d45271e9df839e42124558eb5283508ca70f5c`  
		Last Modified: Tue, 17 Nov 2020 20:32:02 GMT  
		Size: 25.9 MB (25862532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808368e9cd11971fa6e53b4a3fbb5559d120515e05c721adff9b9e493870a0f5`  
		Last Modified: Wed, 18 Nov 2020 01:36:25 GMT  
		Size: 255.9 KB (255886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cdf6ac0c679ba4beaf9bad32b903763540d340a1b59395c930a56b288947efe`  
		Last Modified: Wed, 18 Nov 2020 01:36:35 GMT  
		Size: 31.8 MB (31750189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85a8c7edd4b4a3cbd35f220923da50329be4d48bbff3d793963214b91d5e4c9`  
		Last Modified: Wed, 18 Nov 2020 01:38:19 GMT  
		Size: 145.4 MB (145439899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; 386

```console
$ docker pull mono@sha256:134601059016d772aac04e8b006c0467d93094aac62ec0a5a003779f5efb06d0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.5 MB (230532788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c942123328c3a3ae3a83555749eec2e9c668cc58f1cf9a219c5fbff2e472441`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:03 GMT
ADD file:51108b89c70ce0773c897be520c84454660f38b84ba556da49c7fe77e5d52416 in / 
# Tue, 13 Oct 2020 01:41:03 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 07:38:18 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 07:38:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 07:39:07 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Oct 2020 07:44:16 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:97e4efec21eea92209464547d0f52a0f773c505cf4ea9d8090cef667bde145b8`  
		Last Modified: Tue, 13 Oct 2020 01:48:54 GMT  
		Size: 27.8 MB (27750243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9588b02c60fba169bd9cad455764e725c295ddf21085d904d732ef4892d6375f`  
		Last Modified: Tue, 13 Oct 2020 07:45:04 GMT  
		Size: 255.8 KB (255832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf75edd8ea102d6fbbdb5609df6a19925523bdb561e696bd0fb665b5bb2c5a7`  
		Last Modified: Tue, 13 Oct 2020 07:45:21 GMT  
		Size: 71.1 MB (71136124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6087ce14b6fee3f871defe577ae84bcf6db5fe3226dc585305fa9ce5c625d41`  
		Last Modified: Tue, 13 Oct 2020 07:46:42 GMT  
		Size: 131.4 MB (131390589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; ppc64le

```console
$ docker pull mono@sha256:5d8d2256088dfe9d8870d0ad3a58c3bd5428ae3f6f47046f14c4009fad3cdddc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.1 MB (192080743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee6e47cfbad6be2c8b92dd6b5d33888766804f9cdc59ee9042f56068e1499de9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:54 GMT
ADD file:9992867f855c9bed54df6d26f3d8076689aff8a51e808fefba7d3b66dab250e5 in / 
# Tue, 13 Oct 2020 01:38:59 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 10:20:33 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 10:21:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 10:23:38 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Oct 2020 10:40:36 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:523555c6877c72cfcdec912b4d0053c298b1c97835efc7c6b0211585a06bd563`  
		Last Modified: Tue, 13 Oct 2020 01:50:10 GMT  
		Size: 30.5 MB (30517878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6778a79cc5707eb6c5a21cff2f3f04a05c0ba40bc48c3b3b97f695441e2695fe`  
		Last Modified: Tue, 13 Oct 2020 10:42:46 GMT  
		Size: 256.1 KB (256132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29be084b2430b8c354483c0ac192dd08a2e22fd9687a53e928bf6126d0703187`  
		Last Modified: Tue, 13 Oct 2020 10:43:40 GMT  
		Size: 29.3 MB (29349822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89fb777ba4b2b8e659779b45eedfc16ba2052f25ece387db17ba60fd460c08d4`  
		Last Modified: Tue, 13 Oct 2020 10:47:49 GMT  
		Size: 132.0 MB (131956911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10.0.104`

```console
$ docker pull mono@sha256:e1c39d26dc47f212bc8ba5bfd282526987f2c9f7a1a124fb7dd2badb9c3e44dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.10.0.104` - linux; amd64

```console
$ docker pull mono@sha256:0beb1b5ba9a0cc0efaaa1148c2682d02351ffb94d77ee74ec5e2fedb625bdd17
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.7 MB (224728267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ffb04a492e34192512ff718aaf68247effd38c5ee58e852b67e750455ca46a3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:07:49 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 08:08:00 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 08:08:57 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Oct 2020 08:28:43 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f42b4ad878bfc3887ec056c31544fe7c67286e2cbf905efd97752fb01bf7cf`  
		Last Modified: Tue, 13 Oct 2020 08:29:21 GMT  
		Size: 255.9 KB (255885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595630826b1b79ee45e4c4202b61c61ada9c53bf1352e06571dbaa4624660c6f`  
		Last Modified: Tue, 13 Oct 2020 08:29:34 GMT  
		Size: 67.1 MB (67092282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f179adbd59957f8069efb25f4b87a0c78f7120ca6935479e58a6c9f0d0f75253`  
		Last Modified: Tue, 13 Oct 2020 08:30:39 GMT  
		Size: 130.3 MB (130287872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; arm variant v5

```console
$ docker pull mono@sha256:3e601afbb4577fd538dfa06145643ef0c370d3b98b7fdbdeb8e69e6e7c3cc44b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180580641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0b1583a0f54587294ef3fb13293551714e84d35168baa3b742491aac91dc394`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:52:17 GMT
ADD file:b71c0fa4957d6b65af37231a105f3d17cdbafe5c7d6c37b5843ebf619c608aaa in / 
# Tue, 13 Oct 2020 01:52:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:36:19 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 02:36:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 02:37:31 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Oct 2020 02:44:00 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f991c1e1ee2c48f16625b6b61310bf3c0616c0dbda4762019117e86fd29cf9ce`  
		Last Modified: Tue, 13 Oct 2020 02:01:27 GMT  
		Size: 24.8 MB (24835992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27e131b9898d8f02267f410169b8627b889f6585ad9300d14a4775194301b55`  
		Last Modified: Tue, 13 Oct 2020 02:44:49 GMT  
		Size: 255.9 KB (255938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b82cc14a51474e2d05a0fd59b3fde70aa8fda539de5a302992983e4ffce7b8`  
		Last Modified: Tue, 13 Oct 2020 02:45:01 GMT  
		Size: 26.5 MB (26530650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94ad0d9899e6c5c16486a97103eb9bbff1261c084ef2366534ae27653b23704`  
		Last Modified: Tue, 13 Oct 2020 02:46:59 GMT  
		Size: 129.0 MB (128958061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; arm variant v7

```console
$ docker pull mono@sha256:0e797969122f94b85e9178dd9bece13c7ebd2cacf124520f4275e0ac7cd2b15d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.5 MB (176483530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b81a3bb43255d115e920754f87906a5cd00c5c5ae23a85f06c756f2c42a455b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 00:59:29 GMT
ADD file:e423f30ca19eb205a98de21b0545d0a764cfc4f832a9a9631542354d914d98d9 in / 
# Tue, 13 Oct 2020 00:59:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 04:43:09 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 04:43:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 04:44:11 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Oct 2020 04:49:53 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d6d8411ad43db0022fa0fce094cd2e8b1dd2f8a09d6880ed9beb6b4204867027`  
		Last Modified: Tue, 13 Oct 2020 01:08:28 GMT  
		Size: 22.7 MB (22699849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5228b93feed3135603bc1b4bbda140b6e3e712167c9dd5ccaad1732370cd6b93`  
		Last Modified: Tue, 13 Oct 2020 04:50:37 GMT  
		Size: 255.9 KB (255921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e85494910fa31cd3bb70be77361cab8fa0b333de462a10ce0e2181ee165c0a`  
		Last Modified: Tue, 13 Oct 2020 04:50:46 GMT  
		Size: 25.7 MB (25729327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0179ccf237338944b3401bc8ed480a53bd10956472cd41d05647aeb7fa46ee`  
		Last Modified: Tue, 13 Oct 2020 04:52:43 GMT  
		Size: 127.8 MB (127798433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:0b5ce90bc0624cc3be76e2f4faa9b5ece9459fbda3fd2d1e600b0d03a6693710
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.3 MB (203308506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:684f822e67b92095a97967c053ec1acb78c5d01f5ca24b36822f3fee9136d53f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:31 GMT
ADD file:a70d8c01f8f04f36038968567af779883f3b5ba3147b662b7d170d80418bc23c in / 
# Tue, 17 Nov 2020 20:23:32 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 01:28:53 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 18 Nov 2020 01:29:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 18 Nov 2020 01:29:56 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 18 Nov 2020 01:35:25 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:29ade854e0dcedde295dd89890d45271e9df839e42124558eb5283508ca70f5c`  
		Last Modified: Tue, 17 Nov 2020 20:32:02 GMT  
		Size: 25.9 MB (25862532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808368e9cd11971fa6e53b4a3fbb5559d120515e05c721adff9b9e493870a0f5`  
		Last Modified: Wed, 18 Nov 2020 01:36:25 GMT  
		Size: 255.9 KB (255886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cdf6ac0c679ba4beaf9bad32b903763540d340a1b59395c930a56b288947efe`  
		Last Modified: Wed, 18 Nov 2020 01:36:35 GMT  
		Size: 31.8 MB (31750189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85a8c7edd4b4a3cbd35f220923da50329be4d48bbff3d793963214b91d5e4c9`  
		Last Modified: Wed, 18 Nov 2020 01:38:19 GMT  
		Size: 145.4 MB (145439899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; 386

```console
$ docker pull mono@sha256:134601059016d772aac04e8b006c0467d93094aac62ec0a5a003779f5efb06d0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.5 MB (230532788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c942123328c3a3ae3a83555749eec2e9c668cc58f1cf9a219c5fbff2e472441`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:03 GMT
ADD file:51108b89c70ce0773c897be520c84454660f38b84ba556da49c7fe77e5d52416 in / 
# Tue, 13 Oct 2020 01:41:03 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 07:38:18 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 07:38:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 07:39:07 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Oct 2020 07:44:16 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:97e4efec21eea92209464547d0f52a0f773c505cf4ea9d8090cef667bde145b8`  
		Last Modified: Tue, 13 Oct 2020 01:48:54 GMT  
		Size: 27.8 MB (27750243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9588b02c60fba169bd9cad455764e725c295ddf21085d904d732ef4892d6375f`  
		Last Modified: Tue, 13 Oct 2020 07:45:04 GMT  
		Size: 255.8 KB (255832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf75edd8ea102d6fbbdb5609df6a19925523bdb561e696bd0fb665b5bb2c5a7`  
		Last Modified: Tue, 13 Oct 2020 07:45:21 GMT  
		Size: 71.1 MB (71136124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6087ce14b6fee3f871defe577ae84bcf6db5fe3226dc585305fa9ce5c625d41`  
		Last Modified: Tue, 13 Oct 2020 07:46:42 GMT  
		Size: 131.4 MB (131390589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; ppc64le

```console
$ docker pull mono@sha256:5d8d2256088dfe9d8870d0ad3a58c3bd5428ae3f6f47046f14c4009fad3cdddc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.1 MB (192080743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee6e47cfbad6be2c8b92dd6b5d33888766804f9cdc59ee9042f56068e1499de9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:54 GMT
ADD file:9992867f855c9bed54df6d26f3d8076689aff8a51e808fefba7d3b66dab250e5 in / 
# Tue, 13 Oct 2020 01:38:59 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 10:20:33 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 10:21:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 10:23:38 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Oct 2020 10:40:36 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:523555c6877c72cfcdec912b4d0053c298b1c97835efc7c6b0211585a06bd563`  
		Last Modified: Tue, 13 Oct 2020 01:50:10 GMT  
		Size: 30.5 MB (30517878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6778a79cc5707eb6c5a21cff2f3f04a05c0ba40bc48c3b3b97f695441e2695fe`  
		Last Modified: Tue, 13 Oct 2020 10:42:46 GMT  
		Size: 256.1 KB (256132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29be084b2430b8c354483c0ac192dd08a2e22fd9687a53e928bf6126d0703187`  
		Last Modified: Tue, 13 Oct 2020 10:43:40 GMT  
		Size: 29.3 MB (29349822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89fb777ba4b2b8e659779b45eedfc16ba2052f25ece387db17ba60fd460c08d4`  
		Last Modified: Tue, 13 Oct 2020 10:47:49 GMT  
		Size: 132.0 MB (131956911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10.0.104-slim`

```console
$ docker pull mono@sha256:f9cc1d4ca9b6182ddbf6a41a03bed096f663b26dd9c9350d980d83f2e90f7742
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.10.0.104-slim` - linux; amd64

```console
$ docker pull mono@sha256:3765ac28d39147593372198431028d6b330f0fcf662347678d75205cae7d21f6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.4 MB (94440395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f7e8e7920f90e20657bcacaea38bf659ee3e6001ef3da7e6df0494c995367bb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:07:49 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 08:08:00 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 08:08:57 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f42b4ad878bfc3887ec056c31544fe7c67286e2cbf905efd97752fb01bf7cf`  
		Last Modified: Tue, 13 Oct 2020 08:29:21 GMT  
		Size: 255.9 KB (255885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595630826b1b79ee45e4c4202b61c61ada9c53bf1352e06571dbaa4624660c6f`  
		Last Modified: Tue, 13 Oct 2020 08:29:34 GMT  
		Size: 67.1 MB (67092282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:4f1935b74f258609d63b31cd01cabf54f735b72c77385b4d0486116f7b9ef1db
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51622580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8aaea1ec0574bca839c762a7724f248e6384ba44765e12d60a1eeb21f04760d2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:52:17 GMT
ADD file:b71c0fa4957d6b65af37231a105f3d17cdbafe5c7d6c37b5843ebf619c608aaa in / 
# Tue, 13 Oct 2020 01:52:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:36:19 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 02:36:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 02:37:31 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f991c1e1ee2c48f16625b6b61310bf3c0616c0dbda4762019117e86fd29cf9ce`  
		Last Modified: Tue, 13 Oct 2020 02:01:27 GMT  
		Size: 24.8 MB (24835992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27e131b9898d8f02267f410169b8627b889f6585ad9300d14a4775194301b55`  
		Last Modified: Tue, 13 Oct 2020 02:44:49 GMT  
		Size: 255.9 KB (255938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b82cc14a51474e2d05a0fd59b3fde70aa8fda539de5a302992983e4ffce7b8`  
		Last Modified: Tue, 13 Oct 2020 02:45:01 GMT  
		Size: 26.5 MB (26530650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:bf61cbd2fff2e9323d1f89b46e33accc00aa6aef0f7f4ab533d44ff2d3672097
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48685097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4593f3eb7182d83642b75181ed79a20590556ea1d6460aef0cad9e805bef1e10`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 00:59:29 GMT
ADD file:e423f30ca19eb205a98de21b0545d0a764cfc4f832a9a9631542354d914d98d9 in / 
# Tue, 13 Oct 2020 00:59:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 04:43:09 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 04:43:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 04:44:11 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d6d8411ad43db0022fa0fce094cd2e8b1dd2f8a09d6880ed9beb6b4204867027`  
		Last Modified: Tue, 13 Oct 2020 01:08:28 GMT  
		Size: 22.7 MB (22699849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5228b93feed3135603bc1b4bbda140b6e3e712167c9dd5ccaad1732370cd6b93`  
		Last Modified: Tue, 13 Oct 2020 04:50:37 GMT  
		Size: 255.9 KB (255921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e85494910fa31cd3bb70be77361cab8fa0b333de462a10ce0e2181ee165c0a`  
		Last Modified: Tue, 13 Oct 2020 04:50:46 GMT  
		Size: 25.7 MB (25729327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:f61a1980078fd63569530291f822a8b6ae13ad45b2b80ab0966e6e274bd43760
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57868607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecd1dcf4046ccc6dd611bd3d6b63c8138e7d813b6c0ccd08cd1606e395148fe1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:31 GMT
ADD file:a70d8c01f8f04f36038968567af779883f3b5ba3147b662b7d170d80418bc23c in / 
# Tue, 17 Nov 2020 20:23:32 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 01:28:53 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 18 Nov 2020 01:29:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 18 Nov 2020 01:29:56 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:29ade854e0dcedde295dd89890d45271e9df839e42124558eb5283508ca70f5c`  
		Last Modified: Tue, 17 Nov 2020 20:32:02 GMT  
		Size: 25.9 MB (25862532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808368e9cd11971fa6e53b4a3fbb5559d120515e05c721adff9b9e493870a0f5`  
		Last Modified: Wed, 18 Nov 2020 01:36:25 GMT  
		Size: 255.9 KB (255886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cdf6ac0c679ba4beaf9bad32b903763540d340a1b59395c930a56b288947efe`  
		Last Modified: Wed, 18 Nov 2020 01:36:35 GMT  
		Size: 31.8 MB (31750189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; 386

```console
$ docker pull mono@sha256:30595710e290d4c665ddfdd6521b718f784a35d9a7f951deaa1c50cd12c26d99
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99142199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60ded9fb25b4db7c9c4f48c126b26c7c9188e0b124c54bdc3b8cafb366982817`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:03 GMT
ADD file:51108b89c70ce0773c897be520c84454660f38b84ba556da49c7fe77e5d52416 in / 
# Tue, 13 Oct 2020 01:41:03 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 07:38:18 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 07:38:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 07:39:07 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:97e4efec21eea92209464547d0f52a0f773c505cf4ea9d8090cef667bde145b8`  
		Last Modified: Tue, 13 Oct 2020 01:48:54 GMT  
		Size: 27.8 MB (27750243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9588b02c60fba169bd9cad455764e725c295ddf21085d904d732ef4892d6375f`  
		Last Modified: Tue, 13 Oct 2020 07:45:04 GMT  
		Size: 255.8 KB (255832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf75edd8ea102d6fbbdb5609df6a19925523bdb561e696bd0fb665b5bb2c5a7`  
		Last Modified: Tue, 13 Oct 2020 07:45:21 GMT  
		Size: 71.1 MB (71136124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:445fd5d23b080f1f1a4c37154a548fbc232319eca35a596fc5e3b0f9ec60c409
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60123832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44ccc1548e965ff3511e623f5d42c04512024e85ff17bf5945dcbe2eb2ee1234`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:54 GMT
ADD file:9992867f855c9bed54df6d26f3d8076689aff8a51e808fefba7d3b66dab250e5 in / 
# Tue, 13 Oct 2020 01:38:59 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 10:20:33 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 10:21:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 10:23:38 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:523555c6877c72cfcdec912b4d0053c298b1c97835efc7c6b0211585a06bd563`  
		Last Modified: Tue, 13 Oct 2020 01:50:10 GMT  
		Size: 30.5 MB (30517878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6778a79cc5707eb6c5a21cff2f3f04a05c0ba40bc48c3b3b97f695441e2695fe`  
		Last Modified: Tue, 13 Oct 2020 10:42:46 GMT  
		Size: 256.1 KB (256132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29be084b2430b8c354483c0ac192dd08a2e22fd9687a53e928bf6126d0703187`  
		Last Modified: Tue, 13 Oct 2020 10:43:40 GMT  
		Size: 29.3 MB (29349822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10.0-slim`

```console
$ docker pull mono@sha256:f9cc1d4ca9b6182ddbf6a41a03bed096f663b26dd9c9350d980d83f2e90f7742
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.10.0-slim` - linux; amd64

```console
$ docker pull mono@sha256:3765ac28d39147593372198431028d6b330f0fcf662347678d75205cae7d21f6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.4 MB (94440395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f7e8e7920f90e20657bcacaea38bf659ee3e6001ef3da7e6df0494c995367bb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:07:49 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 08:08:00 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 08:08:57 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f42b4ad878bfc3887ec056c31544fe7c67286e2cbf905efd97752fb01bf7cf`  
		Last Modified: Tue, 13 Oct 2020 08:29:21 GMT  
		Size: 255.9 KB (255885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595630826b1b79ee45e4c4202b61c61ada9c53bf1352e06571dbaa4624660c6f`  
		Last Modified: Tue, 13 Oct 2020 08:29:34 GMT  
		Size: 67.1 MB (67092282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:4f1935b74f258609d63b31cd01cabf54f735b72c77385b4d0486116f7b9ef1db
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51622580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8aaea1ec0574bca839c762a7724f248e6384ba44765e12d60a1eeb21f04760d2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:52:17 GMT
ADD file:b71c0fa4957d6b65af37231a105f3d17cdbafe5c7d6c37b5843ebf619c608aaa in / 
# Tue, 13 Oct 2020 01:52:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:36:19 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 02:36:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 02:37:31 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f991c1e1ee2c48f16625b6b61310bf3c0616c0dbda4762019117e86fd29cf9ce`  
		Last Modified: Tue, 13 Oct 2020 02:01:27 GMT  
		Size: 24.8 MB (24835992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27e131b9898d8f02267f410169b8627b889f6585ad9300d14a4775194301b55`  
		Last Modified: Tue, 13 Oct 2020 02:44:49 GMT  
		Size: 255.9 KB (255938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b82cc14a51474e2d05a0fd59b3fde70aa8fda539de5a302992983e4ffce7b8`  
		Last Modified: Tue, 13 Oct 2020 02:45:01 GMT  
		Size: 26.5 MB (26530650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:bf61cbd2fff2e9323d1f89b46e33accc00aa6aef0f7f4ab533d44ff2d3672097
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48685097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4593f3eb7182d83642b75181ed79a20590556ea1d6460aef0cad9e805bef1e10`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 00:59:29 GMT
ADD file:e423f30ca19eb205a98de21b0545d0a764cfc4f832a9a9631542354d914d98d9 in / 
# Tue, 13 Oct 2020 00:59:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 04:43:09 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 04:43:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 04:44:11 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d6d8411ad43db0022fa0fce094cd2e8b1dd2f8a09d6880ed9beb6b4204867027`  
		Last Modified: Tue, 13 Oct 2020 01:08:28 GMT  
		Size: 22.7 MB (22699849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5228b93feed3135603bc1b4bbda140b6e3e712167c9dd5ccaad1732370cd6b93`  
		Last Modified: Tue, 13 Oct 2020 04:50:37 GMT  
		Size: 255.9 KB (255921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e85494910fa31cd3bb70be77361cab8fa0b333de462a10ce0e2181ee165c0a`  
		Last Modified: Tue, 13 Oct 2020 04:50:46 GMT  
		Size: 25.7 MB (25729327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:f61a1980078fd63569530291f822a8b6ae13ad45b2b80ab0966e6e274bd43760
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57868607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecd1dcf4046ccc6dd611bd3d6b63c8138e7d813b6c0ccd08cd1606e395148fe1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:31 GMT
ADD file:a70d8c01f8f04f36038968567af779883f3b5ba3147b662b7d170d80418bc23c in / 
# Tue, 17 Nov 2020 20:23:32 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 01:28:53 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 18 Nov 2020 01:29:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 18 Nov 2020 01:29:56 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:29ade854e0dcedde295dd89890d45271e9df839e42124558eb5283508ca70f5c`  
		Last Modified: Tue, 17 Nov 2020 20:32:02 GMT  
		Size: 25.9 MB (25862532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808368e9cd11971fa6e53b4a3fbb5559d120515e05c721adff9b9e493870a0f5`  
		Last Modified: Wed, 18 Nov 2020 01:36:25 GMT  
		Size: 255.9 KB (255886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cdf6ac0c679ba4beaf9bad32b903763540d340a1b59395c930a56b288947efe`  
		Last Modified: Wed, 18 Nov 2020 01:36:35 GMT  
		Size: 31.8 MB (31750189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; 386

```console
$ docker pull mono@sha256:30595710e290d4c665ddfdd6521b718f784a35d9a7f951deaa1c50cd12c26d99
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99142199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60ded9fb25b4db7c9c4f48c126b26c7c9188e0b124c54bdc3b8cafb366982817`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:03 GMT
ADD file:51108b89c70ce0773c897be520c84454660f38b84ba556da49c7fe77e5d52416 in / 
# Tue, 13 Oct 2020 01:41:03 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 07:38:18 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 07:38:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 07:39:07 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:97e4efec21eea92209464547d0f52a0f773c505cf4ea9d8090cef667bde145b8`  
		Last Modified: Tue, 13 Oct 2020 01:48:54 GMT  
		Size: 27.8 MB (27750243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9588b02c60fba169bd9cad455764e725c295ddf21085d904d732ef4892d6375f`  
		Last Modified: Tue, 13 Oct 2020 07:45:04 GMT  
		Size: 255.8 KB (255832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf75edd8ea102d6fbbdb5609df6a19925523bdb561e696bd0fb665b5bb2c5a7`  
		Last Modified: Tue, 13 Oct 2020 07:45:21 GMT  
		Size: 71.1 MB (71136124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:445fd5d23b080f1f1a4c37154a548fbc232319eca35a596fc5e3b0f9ec60c409
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60123832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44ccc1548e965ff3511e623f5d42c04512024e85ff17bf5945dcbe2eb2ee1234`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:54 GMT
ADD file:9992867f855c9bed54df6d26f3d8076689aff8a51e808fefba7d3b66dab250e5 in / 
# Tue, 13 Oct 2020 01:38:59 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 10:20:33 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 10:21:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 10:23:38 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:523555c6877c72cfcdec912b4d0053c298b1c97835efc7c6b0211585a06bd563`  
		Last Modified: Tue, 13 Oct 2020 01:50:10 GMT  
		Size: 30.5 MB (30517878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6778a79cc5707eb6c5a21cff2f3f04a05c0ba40bc48c3b3b97f695441e2695fe`  
		Last Modified: Tue, 13 Oct 2020 10:42:46 GMT  
		Size: 256.1 KB (256132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29be084b2430b8c354483c0ac192dd08a2e22fd9687a53e928bf6126d0703187`  
		Last Modified: Tue, 13 Oct 2020 10:43:40 GMT  
		Size: 29.3 MB (29349822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10-slim`

```console
$ docker pull mono@sha256:f9cc1d4ca9b6182ddbf6a41a03bed096f663b26dd9c9350d980d83f2e90f7742
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.10-slim` - linux; amd64

```console
$ docker pull mono@sha256:3765ac28d39147593372198431028d6b330f0fcf662347678d75205cae7d21f6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.4 MB (94440395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f7e8e7920f90e20657bcacaea38bf659ee3e6001ef3da7e6df0494c995367bb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:07:49 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 08:08:00 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 08:08:57 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f42b4ad878bfc3887ec056c31544fe7c67286e2cbf905efd97752fb01bf7cf`  
		Last Modified: Tue, 13 Oct 2020 08:29:21 GMT  
		Size: 255.9 KB (255885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595630826b1b79ee45e4c4202b61c61ada9c53bf1352e06571dbaa4624660c6f`  
		Last Modified: Tue, 13 Oct 2020 08:29:34 GMT  
		Size: 67.1 MB (67092282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:4f1935b74f258609d63b31cd01cabf54f735b72c77385b4d0486116f7b9ef1db
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51622580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8aaea1ec0574bca839c762a7724f248e6384ba44765e12d60a1eeb21f04760d2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:52:17 GMT
ADD file:b71c0fa4957d6b65af37231a105f3d17cdbafe5c7d6c37b5843ebf619c608aaa in / 
# Tue, 13 Oct 2020 01:52:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:36:19 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 02:36:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 02:37:31 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f991c1e1ee2c48f16625b6b61310bf3c0616c0dbda4762019117e86fd29cf9ce`  
		Last Modified: Tue, 13 Oct 2020 02:01:27 GMT  
		Size: 24.8 MB (24835992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27e131b9898d8f02267f410169b8627b889f6585ad9300d14a4775194301b55`  
		Last Modified: Tue, 13 Oct 2020 02:44:49 GMT  
		Size: 255.9 KB (255938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b82cc14a51474e2d05a0fd59b3fde70aa8fda539de5a302992983e4ffce7b8`  
		Last Modified: Tue, 13 Oct 2020 02:45:01 GMT  
		Size: 26.5 MB (26530650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:bf61cbd2fff2e9323d1f89b46e33accc00aa6aef0f7f4ab533d44ff2d3672097
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48685097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4593f3eb7182d83642b75181ed79a20590556ea1d6460aef0cad9e805bef1e10`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 00:59:29 GMT
ADD file:e423f30ca19eb205a98de21b0545d0a764cfc4f832a9a9631542354d914d98d9 in / 
# Tue, 13 Oct 2020 00:59:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 04:43:09 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 04:43:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 04:44:11 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d6d8411ad43db0022fa0fce094cd2e8b1dd2f8a09d6880ed9beb6b4204867027`  
		Last Modified: Tue, 13 Oct 2020 01:08:28 GMT  
		Size: 22.7 MB (22699849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5228b93feed3135603bc1b4bbda140b6e3e712167c9dd5ccaad1732370cd6b93`  
		Last Modified: Tue, 13 Oct 2020 04:50:37 GMT  
		Size: 255.9 KB (255921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e85494910fa31cd3bb70be77361cab8fa0b333de462a10ce0e2181ee165c0a`  
		Last Modified: Tue, 13 Oct 2020 04:50:46 GMT  
		Size: 25.7 MB (25729327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:f61a1980078fd63569530291f822a8b6ae13ad45b2b80ab0966e6e274bd43760
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57868607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecd1dcf4046ccc6dd611bd3d6b63c8138e7d813b6c0ccd08cd1606e395148fe1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:31 GMT
ADD file:a70d8c01f8f04f36038968567af779883f3b5ba3147b662b7d170d80418bc23c in / 
# Tue, 17 Nov 2020 20:23:32 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 01:28:53 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 18 Nov 2020 01:29:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 18 Nov 2020 01:29:56 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:29ade854e0dcedde295dd89890d45271e9df839e42124558eb5283508ca70f5c`  
		Last Modified: Tue, 17 Nov 2020 20:32:02 GMT  
		Size: 25.9 MB (25862532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808368e9cd11971fa6e53b4a3fbb5559d120515e05c721adff9b9e493870a0f5`  
		Last Modified: Wed, 18 Nov 2020 01:36:25 GMT  
		Size: 255.9 KB (255886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cdf6ac0c679ba4beaf9bad32b903763540d340a1b59395c930a56b288947efe`  
		Last Modified: Wed, 18 Nov 2020 01:36:35 GMT  
		Size: 31.8 MB (31750189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; 386

```console
$ docker pull mono@sha256:30595710e290d4c665ddfdd6521b718f784a35d9a7f951deaa1c50cd12c26d99
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99142199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60ded9fb25b4db7c9c4f48c126b26c7c9188e0b124c54bdc3b8cafb366982817`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:03 GMT
ADD file:51108b89c70ce0773c897be520c84454660f38b84ba556da49c7fe77e5d52416 in / 
# Tue, 13 Oct 2020 01:41:03 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 07:38:18 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 07:38:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 07:39:07 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:97e4efec21eea92209464547d0f52a0f773c505cf4ea9d8090cef667bde145b8`  
		Last Modified: Tue, 13 Oct 2020 01:48:54 GMT  
		Size: 27.8 MB (27750243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9588b02c60fba169bd9cad455764e725c295ddf21085d904d732ef4892d6375f`  
		Last Modified: Tue, 13 Oct 2020 07:45:04 GMT  
		Size: 255.8 KB (255832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf75edd8ea102d6fbbdb5609df6a19925523bdb561e696bd0fb665b5bb2c5a7`  
		Last Modified: Tue, 13 Oct 2020 07:45:21 GMT  
		Size: 71.1 MB (71136124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:445fd5d23b080f1f1a4c37154a548fbc232319eca35a596fc5e3b0f9ec60c409
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60123832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44ccc1548e965ff3511e623f5d42c04512024e85ff17bf5945dcbe2eb2ee1234`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:54 GMT
ADD file:9992867f855c9bed54df6d26f3d8076689aff8a51e808fefba7d3b66dab250e5 in / 
# Tue, 13 Oct 2020 01:38:59 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 10:20:33 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 10:21:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 10:23:38 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:523555c6877c72cfcdec912b4d0053c298b1c97835efc7c6b0211585a06bd563`  
		Last Modified: Tue, 13 Oct 2020 01:50:10 GMT  
		Size: 30.5 MB (30517878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6778a79cc5707eb6c5a21cff2f3f04a05c0ba40bc48c3b3b97f695441e2695fe`  
		Last Modified: Tue, 13 Oct 2020 10:42:46 GMT  
		Size: 256.1 KB (256132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29be084b2430b8c354483c0ac192dd08a2e22fd9687a53e928bf6126d0703187`  
		Last Modified: Tue, 13 Oct 2020 10:43:40 GMT  
		Size: 29.3 MB (29349822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.8`

```console
$ docker pull mono@sha256:94d77654f73a1cc710978a793f850cf738a38ae3145cb40a82b641b1efaad6d0
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
$ docker pull mono@sha256:4cd801687baa5dc0e1bb4270d77d32161592a5a28f7ac59bc480b92f06446360
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.6 MB (240618215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b27fb3a052d421fb038ce1f84d930e5c15048aacc6d7675c803d30e34669ac7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:06:44 GMT
ENV MONO_VERSION=6.8.0.123
# Tue, 13 Oct 2020 08:06:55 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 08:07:40 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Oct 2020 08:19:51 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23366ca64f7a24bbe3e1609f8d66b5ebc452f78998573e407f88f528c39528a3`  
		Last Modified: Tue, 13 Oct 2020 08:29:04 GMT  
		Size: 255.9 KB (255878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc110778513890ac2d5223325778aae22dc42890ed6c8495ff7ecf4801024643`  
		Last Modified: Tue, 13 Oct 2020 08:29:17 GMT  
		Size: 67.1 MB (67084013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed91b51157b0c155a7154ee624236e1439c88b18107b8014f0a1adebe965da5f`  
		Last Modified: Tue, 13 Oct 2020 08:30:08 GMT  
		Size: 146.2 MB (146186096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8` - linux; arm variant v5

```console
$ docker pull mono@sha256:a0a1a561f24b8db06e703f007caa49771a3ded79bfc07da63a4266618839a4df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.9 MB (179921571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b41e1c51d61456193c2e5b4ac15db06ad90625b510bd72e08fe44315a015aba6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:52:17 GMT
ADD file:b71c0fa4957d6b65af37231a105f3d17cdbafe5c7d6c37b5843ebf619c608aaa in / 
# Tue, 13 Oct 2020 01:52:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:34:46 GMT
ENV MONO_VERSION=6.8.0.123
# Tue, 13 Oct 2020 02:35:14 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 02:36:05 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Oct 2020 02:40:37 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f991c1e1ee2c48f16625b6b61310bf3c0616c0dbda4762019117e86fd29cf9ce`  
		Last Modified: Tue, 13 Oct 2020 02:01:27 GMT  
		Size: 24.8 MB (24835992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58c01c93058384dcced83ee11026a0e5e2652432af5c3eaa02592a2cebdfdf6`  
		Last Modified: Tue, 13 Oct 2020 02:44:29 GMT  
		Size: 256.0 KB (255998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd8d0a31f42e3311b822b7c94bb005cf72849efb2f5c39943b70702c6631de9`  
		Last Modified: Tue, 13 Oct 2020 02:44:40 GMT  
		Size: 26.5 MB (26542426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a0dc85b1e28eca63d1eca67c1f5eb3106274e0105c3c7a0472772c6a1a29ef`  
		Last Modified: Tue, 13 Oct 2020 02:46:02 GMT  
		Size: 128.3 MB (128287155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8` - linux; arm variant v7

```console
$ docker pull mono@sha256:1ebaea3f991a9b92059fd344af338b680011d16745947186b7cd73741eba7157
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.8 MB (175801368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75ea12bfc2cc9a20e0025697f00d3707f17f0e2d0501f3ea8ebe292614dd72ec`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 00:59:29 GMT
ADD file:e423f30ca19eb205a98de21b0545d0a764cfc4f832a9a9631542354d914d98d9 in / 
# Tue, 13 Oct 2020 00:59:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 04:42:00 GMT
ENV MONO_VERSION=6.8.0.123
# Tue, 13 Oct 2020 04:42:16 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 04:43:00 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Oct 2020 04:47:05 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d6d8411ad43db0022fa0fce094cd2e8b1dd2f8a09d6880ed9beb6b4204867027`  
		Last Modified: Tue, 13 Oct 2020 01:08:28 GMT  
		Size: 22.7 MB (22699849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053722f7b6b8ff8b79ff2487965425c4a35e48783e16f602bac9cc463f1514c7`  
		Last Modified: Tue, 13 Oct 2020 04:50:17 GMT  
		Size: 255.9 KB (255908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3dc69451bafa4aa4ed7b7eed809f3e7039f7e9362c96bff1bb37179a1f035e`  
		Last Modified: Tue, 13 Oct 2020 04:50:28 GMT  
		Size: 25.7 MB (25726500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc49c6d1dda18c03351b7935d16b6e3eceddcc30881a4f5416d9f147a3e4ac4`  
		Last Modified: Tue, 13 Oct 2020 04:51:47 GMT  
		Size: 127.1 MB (127119111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:425b07fb96a126e8a06ced456be94b58613d0ec51231280bb0b5ddd02bff67c9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.5 MB (202452069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6c5b8be3c6fc7616da91b2ce0465086fdc0bdb291e77102e3e97f5b8fe21abd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:31 GMT
ADD file:a70d8c01f8f04f36038968567af779883f3b5ba3147b662b7d170d80418bc23c in / 
# Tue, 17 Nov 2020 20:23:32 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 01:27:35 GMT
ENV MONO_VERSION=6.8.0.123
# Wed, 18 Nov 2020 01:27:56 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 18 Nov 2020 01:28:37 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 18 Nov 2020 01:32:49 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:29ade854e0dcedde295dd89890d45271e9df839e42124558eb5283508ca70f5c`  
		Last Modified: Tue, 17 Nov 2020 20:32:02 GMT  
		Size: 25.9 MB (25862532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3ec8e5e3abeb88b50e538233a25dcc55fee6941e17c640df3d1c5e0721c663`  
		Last Modified: Wed, 18 Nov 2020 01:36:06 GMT  
		Size: 255.9 KB (255915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df287fd6b7b7749b3830988992ff21aa14dad6f7b628d3616f06d111fa1965b`  
		Last Modified: Wed, 18 Nov 2020 01:36:16 GMT  
		Size: 31.7 MB (31694938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed12936859322d04f77d41179ae3c17b90c7c452f0dda9fba41090d729dec054`  
		Last Modified: Wed, 18 Nov 2020 01:37:27 GMT  
		Size: 144.6 MB (144638684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8` - linux; 386

```console
$ docker pull mono@sha256:9c0fabdd8a0b23c945e608ec6e869a165233675fc99ec087766d4322121aca96
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.2 MB (249226048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb76221d39145da116f26c366777ec637fcda6882a5b706ef308ae725d4a1638`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:03 GMT
ADD file:51108b89c70ce0773c897be520c84454660f38b84ba556da49c7fe77e5d52416 in / 
# Tue, 13 Oct 2020 01:41:03 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 07:37:13 GMT
ENV MONO_VERSION=6.8.0.123
# Tue, 13 Oct 2020 07:37:25 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 07:38:04 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Oct 2020 07:41:43 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:97e4efec21eea92209464547d0f52a0f773c505cf4ea9d8090cef667bde145b8`  
		Last Modified: Tue, 13 Oct 2020 01:48:54 GMT  
		Size: 27.8 MB (27750243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5017c5054d34dd5350eadd54ec5d96301cc5c8130e1310f6e8022e87fa0ae8ce`  
		Last Modified: Tue, 13 Oct 2020 07:44:39 GMT  
		Size: 255.8 KB (255833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cef04a59545f975fe314d6e732658db45b6c0c2ad188869d117e721dadcf7249`  
		Last Modified: Tue, 13 Oct 2020 07:44:59 GMT  
		Size: 71.1 MB (71105659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22fbdd8e8387158397489a3220f64b39b32142d73a1bf4d95b5f35c5584ecde1`  
		Last Modified: Tue, 13 Oct 2020 07:46:05 GMT  
		Size: 150.1 MB (150114313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8` - linux; ppc64le

```console
$ docker pull mono@sha256:1ebff08506571b472ecc718226b06eab8d2bfefd070bb8ecef02ce797155c6be
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.3 MB (191344287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2948f2870dd4f66360363b39cc2fe6a49791f58a4d30c82817a3349f58efa0ee`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:54 GMT
ADD file:9992867f855c9bed54df6d26f3d8076689aff8a51e808fefba7d3b66dab250e5 in / 
# Tue, 13 Oct 2020 01:38:59 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 10:17:07 GMT
ENV MONO_VERSION=6.8.0.123
# Tue, 13 Oct 2020 10:18:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 10:20:14 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Oct 2020 10:32:00 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:523555c6877c72cfcdec912b4d0053c298b1c97835efc7c6b0211585a06bd563`  
		Last Modified: Tue, 13 Oct 2020 01:50:10 GMT  
		Size: 30.5 MB (30517878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86abab555672e6bfb7c95499bac6717588d8a7630837df56b62caac93e492678`  
		Last Modified: Tue, 13 Oct 2020 10:41:26 GMT  
		Size: 256.1 KB (256072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e455e89a2ebbcda939883181d1f8c8c8b1f22a85f4fedc80a4045074ba40adb`  
		Last Modified: Tue, 13 Oct 2020 10:42:32 GMT  
		Size: 29.3 MB (29330698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80af505d4d58c33dc420a5a8b4bce69d0e76b91c2abfda3adf1573a2819d67f4`  
		Last Modified: Tue, 13 Oct 2020 10:46:58 GMT  
		Size: 131.2 MB (131239639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.8.0`

```console
$ docker pull mono@sha256:94d77654f73a1cc710978a793f850cf738a38ae3145cb40a82b641b1efaad6d0
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
$ docker pull mono@sha256:4cd801687baa5dc0e1bb4270d77d32161592a5a28f7ac59bc480b92f06446360
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.6 MB (240618215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b27fb3a052d421fb038ce1f84d930e5c15048aacc6d7675c803d30e34669ac7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:06:44 GMT
ENV MONO_VERSION=6.8.0.123
# Tue, 13 Oct 2020 08:06:55 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 08:07:40 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Oct 2020 08:19:51 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23366ca64f7a24bbe3e1609f8d66b5ebc452f78998573e407f88f528c39528a3`  
		Last Modified: Tue, 13 Oct 2020 08:29:04 GMT  
		Size: 255.9 KB (255878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc110778513890ac2d5223325778aae22dc42890ed6c8495ff7ecf4801024643`  
		Last Modified: Tue, 13 Oct 2020 08:29:17 GMT  
		Size: 67.1 MB (67084013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed91b51157b0c155a7154ee624236e1439c88b18107b8014f0a1adebe965da5f`  
		Last Modified: Tue, 13 Oct 2020 08:30:08 GMT  
		Size: 146.2 MB (146186096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0` - linux; arm variant v5

```console
$ docker pull mono@sha256:a0a1a561f24b8db06e703f007caa49771a3ded79bfc07da63a4266618839a4df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.9 MB (179921571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b41e1c51d61456193c2e5b4ac15db06ad90625b510bd72e08fe44315a015aba6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:52:17 GMT
ADD file:b71c0fa4957d6b65af37231a105f3d17cdbafe5c7d6c37b5843ebf619c608aaa in / 
# Tue, 13 Oct 2020 01:52:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:34:46 GMT
ENV MONO_VERSION=6.8.0.123
# Tue, 13 Oct 2020 02:35:14 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 02:36:05 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Oct 2020 02:40:37 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f991c1e1ee2c48f16625b6b61310bf3c0616c0dbda4762019117e86fd29cf9ce`  
		Last Modified: Tue, 13 Oct 2020 02:01:27 GMT  
		Size: 24.8 MB (24835992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58c01c93058384dcced83ee11026a0e5e2652432af5c3eaa02592a2cebdfdf6`  
		Last Modified: Tue, 13 Oct 2020 02:44:29 GMT  
		Size: 256.0 KB (255998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd8d0a31f42e3311b822b7c94bb005cf72849efb2f5c39943b70702c6631de9`  
		Last Modified: Tue, 13 Oct 2020 02:44:40 GMT  
		Size: 26.5 MB (26542426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a0dc85b1e28eca63d1eca67c1f5eb3106274e0105c3c7a0472772c6a1a29ef`  
		Last Modified: Tue, 13 Oct 2020 02:46:02 GMT  
		Size: 128.3 MB (128287155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0` - linux; arm variant v7

```console
$ docker pull mono@sha256:1ebaea3f991a9b92059fd344af338b680011d16745947186b7cd73741eba7157
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.8 MB (175801368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75ea12bfc2cc9a20e0025697f00d3707f17f0e2d0501f3ea8ebe292614dd72ec`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 00:59:29 GMT
ADD file:e423f30ca19eb205a98de21b0545d0a764cfc4f832a9a9631542354d914d98d9 in / 
# Tue, 13 Oct 2020 00:59:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 04:42:00 GMT
ENV MONO_VERSION=6.8.0.123
# Tue, 13 Oct 2020 04:42:16 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 04:43:00 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Oct 2020 04:47:05 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d6d8411ad43db0022fa0fce094cd2e8b1dd2f8a09d6880ed9beb6b4204867027`  
		Last Modified: Tue, 13 Oct 2020 01:08:28 GMT  
		Size: 22.7 MB (22699849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053722f7b6b8ff8b79ff2487965425c4a35e48783e16f602bac9cc463f1514c7`  
		Last Modified: Tue, 13 Oct 2020 04:50:17 GMT  
		Size: 255.9 KB (255908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3dc69451bafa4aa4ed7b7eed809f3e7039f7e9362c96bff1bb37179a1f035e`  
		Last Modified: Tue, 13 Oct 2020 04:50:28 GMT  
		Size: 25.7 MB (25726500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc49c6d1dda18c03351b7935d16b6e3eceddcc30881a4f5416d9f147a3e4ac4`  
		Last Modified: Tue, 13 Oct 2020 04:51:47 GMT  
		Size: 127.1 MB (127119111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:425b07fb96a126e8a06ced456be94b58613d0ec51231280bb0b5ddd02bff67c9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.5 MB (202452069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6c5b8be3c6fc7616da91b2ce0465086fdc0bdb291e77102e3e97f5b8fe21abd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:31 GMT
ADD file:a70d8c01f8f04f36038968567af779883f3b5ba3147b662b7d170d80418bc23c in / 
# Tue, 17 Nov 2020 20:23:32 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 01:27:35 GMT
ENV MONO_VERSION=6.8.0.123
# Wed, 18 Nov 2020 01:27:56 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 18 Nov 2020 01:28:37 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 18 Nov 2020 01:32:49 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:29ade854e0dcedde295dd89890d45271e9df839e42124558eb5283508ca70f5c`  
		Last Modified: Tue, 17 Nov 2020 20:32:02 GMT  
		Size: 25.9 MB (25862532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3ec8e5e3abeb88b50e538233a25dcc55fee6941e17c640df3d1c5e0721c663`  
		Last Modified: Wed, 18 Nov 2020 01:36:06 GMT  
		Size: 255.9 KB (255915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df287fd6b7b7749b3830988992ff21aa14dad6f7b628d3616f06d111fa1965b`  
		Last Modified: Wed, 18 Nov 2020 01:36:16 GMT  
		Size: 31.7 MB (31694938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed12936859322d04f77d41179ae3c17b90c7c452f0dda9fba41090d729dec054`  
		Last Modified: Wed, 18 Nov 2020 01:37:27 GMT  
		Size: 144.6 MB (144638684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0` - linux; 386

```console
$ docker pull mono@sha256:9c0fabdd8a0b23c945e608ec6e869a165233675fc99ec087766d4322121aca96
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.2 MB (249226048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb76221d39145da116f26c366777ec637fcda6882a5b706ef308ae725d4a1638`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:03 GMT
ADD file:51108b89c70ce0773c897be520c84454660f38b84ba556da49c7fe77e5d52416 in / 
# Tue, 13 Oct 2020 01:41:03 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 07:37:13 GMT
ENV MONO_VERSION=6.8.0.123
# Tue, 13 Oct 2020 07:37:25 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 07:38:04 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Oct 2020 07:41:43 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:97e4efec21eea92209464547d0f52a0f773c505cf4ea9d8090cef667bde145b8`  
		Last Modified: Tue, 13 Oct 2020 01:48:54 GMT  
		Size: 27.8 MB (27750243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5017c5054d34dd5350eadd54ec5d96301cc5c8130e1310f6e8022e87fa0ae8ce`  
		Last Modified: Tue, 13 Oct 2020 07:44:39 GMT  
		Size: 255.8 KB (255833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cef04a59545f975fe314d6e732658db45b6c0c2ad188869d117e721dadcf7249`  
		Last Modified: Tue, 13 Oct 2020 07:44:59 GMT  
		Size: 71.1 MB (71105659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22fbdd8e8387158397489a3220f64b39b32142d73a1bf4d95b5f35c5584ecde1`  
		Last Modified: Tue, 13 Oct 2020 07:46:05 GMT  
		Size: 150.1 MB (150114313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0` - linux; ppc64le

```console
$ docker pull mono@sha256:1ebff08506571b472ecc718226b06eab8d2bfefd070bb8ecef02ce797155c6be
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.3 MB (191344287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2948f2870dd4f66360363b39cc2fe6a49791f58a4d30c82817a3349f58efa0ee`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:54 GMT
ADD file:9992867f855c9bed54df6d26f3d8076689aff8a51e808fefba7d3b66dab250e5 in / 
# Tue, 13 Oct 2020 01:38:59 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 10:17:07 GMT
ENV MONO_VERSION=6.8.0.123
# Tue, 13 Oct 2020 10:18:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 10:20:14 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Oct 2020 10:32:00 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:523555c6877c72cfcdec912b4d0053c298b1c97835efc7c6b0211585a06bd563`  
		Last Modified: Tue, 13 Oct 2020 01:50:10 GMT  
		Size: 30.5 MB (30517878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86abab555672e6bfb7c95499bac6717588d8a7630837df56b62caac93e492678`  
		Last Modified: Tue, 13 Oct 2020 10:41:26 GMT  
		Size: 256.1 KB (256072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e455e89a2ebbcda939883181d1f8c8c8b1f22a85f4fedc80a4045074ba40adb`  
		Last Modified: Tue, 13 Oct 2020 10:42:32 GMT  
		Size: 29.3 MB (29330698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80af505d4d58c33dc420a5a8b4bce69d0e76b91c2abfda3adf1573a2819d67f4`  
		Last Modified: Tue, 13 Oct 2020 10:46:58 GMT  
		Size: 131.2 MB (131239639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.8.0.123`

```console
$ docker pull mono@sha256:94d77654f73a1cc710978a793f850cf738a38ae3145cb40a82b641b1efaad6d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.8.0.123` - linux; amd64

```console
$ docker pull mono@sha256:4cd801687baa5dc0e1bb4270d77d32161592a5a28f7ac59bc480b92f06446360
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.6 MB (240618215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b27fb3a052d421fb038ce1f84d930e5c15048aacc6d7675c803d30e34669ac7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:06:44 GMT
ENV MONO_VERSION=6.8.0.123
# Tue, 13 Oct 2020 08:06:55 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 08:07:40 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Oct 2020 08:19:51 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23366ca64f7a24bbe3e1609f8d66b5ebc452f78998573e407f88f528c39528a3`  
		Last Modified: Tue, 13 Oct 2020 08:29:04 GMT  
		Size: 255.9 KB (255878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc110778513890ac2d5223325778aae22dc42890ed6c8495ff7ecf4801024643`  
		Last Modified: Tue, 13 Oct 2020 08:29:17 GMT  
		Size: 67.1 MB (67084013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed91b51157b0c155a7154ee624236e1439c88b18107b8014f0a1adebe965da5f`  
		Last Modified: Tue, 13 Oct 2020 08:30:08 GMT  
		Size: 146.2 MB (146186096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.123` - linux; arm variant v5

```console
$ docker pull mono@sha256:a0a1a561f24b8db06e703f007caa49771a3ded79bfc07da63a4266618839a4df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.9 MB (179921571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b41e1c51d61456193c2e5b4ac15db06ad90625b510bd72e08fe44315a015aba6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:52:17 GMT
ADD file:b71c0fa4957d6b65af37231a105f3d17cdbafe5c7d6c37b5843ebf619c608aaa in / 
# Tue, 13 Oct 2020 01:52:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:34:46 GMT
ENV MONO_VERSION=6.8.0.123
# Tue, 13 Oct 2020 02:35:14 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 02:36:05 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Oct 2020 02:40:37 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f991c1e1ee2c48f16625b6b61310bf3c0616c0dbda4762019117e86fd29cf9ce`  
		Last Modified: Tue, 13 Oct 2020 02:01:27 GMT  
		Size: 24.8 MB (24835992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58c01c93058384dcced83ee11026a0e5e2652432af5c3eaa02592a2cebdfdf6`  
		Last Modified: Tue, 13 Oct 2020 02:44:29 GMT  
		Size: 256.0 KB (255998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd8d0a31f42e3311b822b7c94bb005cf72849efb2f5c39943b70702c6631de9`  
		Last Modified: Tue, 13 Oct 2020 02:44:40 GMT  
		Size: 26.5 MB (26542426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a0dc85b1e28eca63d1eca67c1f5eb3106274e0105c3c7a0472772c6a1a29ef`  
		Last Modified: Tue, 13 Oct 2020 02:46:02 GMT  
		Size: 128.3 MB (128287155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.123` - linux; arm variant v7

```console
$ docker pull mono@sha256:1ebaea3f991a9b92059fd344af338b680011d16745947186b7cd73741eba7157
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.8 MB (175801368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75ea12bfc2cc9a20e0025697f00d3707f17f0e2d0501f3ea8ebe292614dd72ec`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 00:59:29 GMT
ADD file:e423f30ca19eb205a98de21b0545d0a764cfc4f832a9a9631542354d914d98d9 in / 
# Tue, 13 Oct 2020 00:59:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 04:42:00 GMT
ENV MONO_VERSION=6.8.0.123
# Tue, 13 Oct 2020 04:42:16 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 04:43:00 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Oct 2020 04:47:05 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d6d8411ad43db0022fa0fce094cd2e8b1dd2f8a09d6880ed9beb6b4204867027`  
		Last Modified: Tue, 13 Oct 2020 01:08:28 GMT  
		Size: 22.7 MB (22699849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053722f7b6b8ff8b79ff2487965425c4a35e48783e16f602bac9cc463f1514c7`  
		Last Modified: Tue, 13 Oct 2020 04:50:17 GMT  
		Size: 255.9 KB (255908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3dc69451bafa4aa4ed7b7eed809f3e7039f7e9362c96bff1bb37179a1f035e`  
		Last Modified: Tue, 13 Oct 2020 04:50:28 GMT  
		Size: 25.7 MB (25726500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc49c6d1dda18c03351b7935d16b6e3eceddcc30881a4f5416d9f147a3e4ac4`  
		Last Modified: Tue, 13 Oct 2020 04:51:47 GMT  
		Size: 127.1 MB (127119111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.123` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:425b07fb96a126e8a06ced456be94b58613d0ec51231280bb0b5ddd02bff67c9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.5 MB (202452069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6c5b8be3c6fc7616da91b2ce0465086fdc0bdb291e77102e3e97f5b8fe21abd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:31 GMT
ADD file:a70d8c01f8f04f36038968567af779883f3b5ba3147b662b7d170d80418bc23c in / 
# Tue, 17 Nov 2020 20:23:32 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 01:27:35 GMT
ENV MONO_VERSION=6.8.0.123
# Wed, 18 Nov 2020 01:27:56 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 18 Nov 2020 01:28:37 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 18 Nov 2020 01:32:49 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:29ade854e0dcedde295dd89890d45271e9df839e42124558eb5283508ca70f5c`  
		Last Modified: Tue, 17 Nov 2020 20:32:02 GMT  
		Size: 25.9 MB (25862532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3ec8e5e3abeb88b50e538233a25dcc55fee6941e17c640df3d1c5e0721c663`  
		Last Modified: Wed, 18 Nov 2020 01:36:06 GMT  
		Size: 255.9 KB (255915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df287fd6b7b7749b3830988992ff21aa14dad6f7b628d3616f06d111fa1965b`  
		Last Modified: Wed, 18 Nov 2020 01:36:16 GMT  
		Size: 31.7 MB (31694938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed12936859322d04f77d41179ae3c17b90c7c452f0dda9fba41090d729dec054`  
		Last Modified: Wed, 18 Nov 2020 01:37:27 GMT  
		Size: 144.6 MB (144638684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.123` - linux; 386

```console
$ docker pull mono@sha256:9c0fabdd8a0b23c945e608ec6e869a165233675fc99ec087766d4322121aca96
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.2 MB (249226048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb76221d39145da116f26c366777ec637fcda6882a5b706ef308ae725d4a1638`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:03 GMT
ADD file:51108b89c70ce0773c897be520c84454660f38b84ba556da49c7fe77e5d52416 in / 
# Tue, 13 Oct 2020 01:41:03 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 07:37:13 GMT
ENV MONO_VERSION=6.8.0.123
# Tue, 13 Oct 2020 07:37:25 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 07:38:04 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Oct 2020 07:41:43 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:97e4efec21eea92209464547d0f52a0f773c505cf4ea9d8090cef667bde145b8`  
		Last Modified: Tue, 13 Oct 2020 01:48:54 GMT  
		Size: 27.8 MB (27750243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5017c5054d34dd5350eadd54ec5d96301cc5c8130e1310f6e8022e87fa0ae8ce`  
		Last Modified: Tue, 13 Oct 2020 07:44:39 GMT  
		Size: 255.8 KB (255833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cef04a59545f975fe314d6e732658db45b6c0c2ad188869d117e721dadcf7249`  
		Last Modified: Tue, 13 Oct 2020 07:44:59 GMT  
		Size: 71.1 MB (71105659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22fbdd8e8387158397489a3220f64b39b32142d73a1bf4d95b5f35c5584ecde1`  
		Last Modified: Tue, 13 Oct 2020 07:46:05 GMT  
		Size: 150.1 MB (150114313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.123` - linux; ppc64le

```console
$ docker pull mono@sha256:1ebff08506571b472ecc718226b06eab8d2bfefd070bb8ecef02ce797155c6be
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.3 MB (191344287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2948f2870dd4f66360363b39cc2fe6a49791f58a4d30c82817a3349f58efa0ee`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:54 GMT
ADD file:9992867f855c9bed54df6d26f3d8076689aff8a51e808fefba7d3b66dab250e5 in / 
# Tue, 13 Oct 2020 01:38:59 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 10:17:07 GMT
ENV MONO_VERSION=6.8.0.123
# Tue, 13 Oct 2020 10:18:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 10:20:14 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Oct 2020 10:32:00 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:523555c6877c72cfcdec912b4d0053c298b1c97835efc7c6b0211585a06bd563`  
		Last Modified: Tue, 13 Oct 2020 01:50:10 GMT  
		Size: 30.5 MB (30517878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86abab555672e6bfb7c95499bac6717588d8a7630837df56b62caac93e492678`  
		Last Modified: Tue, 13 Oct 2020 10:41:26 GMT  
		Size: 256.1 KB (256072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e455e89a2ebbcda939883181d1f8c8c8b1f22a85f4fedc80a4045074ba40adb`  
		Last Modified: Tue, 13 Oct 2020 10:42:32 GMT  
		Size: 29.3 MB (29330698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80af505d4d58c33dc420a5a8b4bce69d0e76b91c2abfda3adf1573a2819d67f4`  
		Last Modified: Tue, 13 Oct 2020 10:46:58 GMT  
		Size: 131.2 MB (131239639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.8.0.123-slim`

```console
$ docker pull mono@sha256:9a4f9ab7eb87475f4040ef5b254218331d7d2199167bd199ad77e4090c2cbe53
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.8.0.123-slim` - linux; amd64

```console
$ docker pull mono@sha256:f644c3da31661298224f7e4d5702d96ef7e6aa7bd1a6194b78c98cf68734756b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.4 MB (94432119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c38349a5287494d54c3ca7a3993fcd1f8d99f73c876fec674e35c1efc9d7983`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:06:44 GMT
ENV MONO_VERSION=6.8.0.123
# Tue, 13 Oct 2020 08:06:55 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 08:07:40 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23366ca64f7a24bbe3e1609f8d66b5ebc452f78998573e407f88f528c39528a3`  
		Last Modified: Tue, 13 Oct 2020 08:29:04 GMT  
		Size: 255.9 KB (255878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc110778513890ac2d5223325778aae22dc42890ed6c8495ff7ecf4801024643`  
		Last Modified: Tue, 13 Oct 2020 08:29:17 GMT  
		Size: 67.1 MB (67084013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.123-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:251f066260187f7daae44d2b0e1c18197b67dc6275508075ae0d2dafa72c2bb8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51634416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bf6a0e393f1c11eff16fe15845a386c8de46aac69339c4113f206093c491b7e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:52:17 GMT
ADD file:b71c0fa4957d6b65af37231a105f3d17cdbafe5c7d6c37b5843ebf619c608aaa in / 
# Tue, 13 Oct 2020 01:52:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:34:46 GMT
ENV MONO_VERSION=6.8.0.123
# Tue, 13 Oct 2020 02:35:14 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 02:36:05 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f991c1e1ee2c48f16625b6b61310bf3c0616c0dbda4762019117e86fd29cf9ce`  
		Last Modified: Tue, 13 Oct 2020 02:01:27 GMT  
		Size: 24.8 MB (24835992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58c01c93058384dcced83ee11026a0e5e2652432af5c3eaa02592a2cebdfdf6`  
		Last Modified: Tue, 13 Oct 2020 02:44:29 GMT  
		Size: 256.0 KB (255998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd8d0a31f42e3311b822b7c94bb005cf72849efb2f5c39943b70702c6631de9`  
		Last Modified: Tue, 13 Oct 2020 02:44:40 GMT  
		Size: 26.5 MB (26542426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.123-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:c84e88fc96c15e99d24c04f88bbbc4b73ff77f7a9bfa07c45f384136199087fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48682257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6f5defcf8cb930642b2a9728a83524bbf0e39ae20d2f0e63aa786a2b8d1a0e0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 00:59:29 GMT
ADD file:e423f30ca19eb205a98de21b0545d0a764cfc4f832a9a9631542354d914d98d9 in / 
# Tue, 13 Oct 2020 00:59:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 04:42:00 GMT
ENV MONO_VERSION=6.8.0.123
# Tue, 13 Oct 2020 04:42:16 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 04:43:00 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d6d8411ad43db0022fa0fce094cd2e8b1dd2f8a09d6880ed9beb6b4204867027`  
		Last Modified: Tue, 13 Oct 2020 01:08:28 GMT  
		Size: 22.7 MB (22699849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053722f7b6b8ff8b79ff2487965425c4a35e48783e16f602bac9cc463f1514c7`  
		Last Modified: Tue, 13 Oct 2020 04:50:17 GMT  
		Size: 255.9 KB (255908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3dc69451bafa4aa4ed7b7eed809f3e7039f7e9362c96bff1bb37179a1f035e`  
		Last Modified: Tue, 13 Oct 2020 04:50:28 GMT  
		Size: 25.7 MB (25726500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.123-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:6bd885bff156f3ba093c0e9c5c84bb566cff37829bf5c89a64bfc8a7eea67e55
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.8 MB (57813385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7189a284f5129368968186f70de9dbc8b1ba9c09966eba00a988f4a3793c4481`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:31 GMT
ADD file:a70d8c01f8f04f36038968567af779883f3b5ba3147b662b7d170d80418bc23c in / 
# Tue, 17 Nov 2020 20:23:32 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 01:27:35 GMT
ENV MONO_VERSION=6.8.0.123
# Wed, 18 Nov 2020 01:27:56 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 18 Nov 2020 01:28:37 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:29ade854e0dcedde295dd89890d45271e9df839e42124558eb5283508ca70f5c`  
		Last Modified: Tue, 17 Nov 2020 20:32:02 GMT  
		Size: 25.9 MB (25862532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3ec8e5e3abeb88b50e538233a25dcc55fee6941e17c640df3d1c5e0721c663`  
		Last Modified: Wed, 18 Nov 2020 01:36:06 GMT  
		Size: 255.9 KB (255915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df287fd6b7b7749b3830988992ff21aa14dad6f7b628d3616f06d111fa1965b`  
		Last Modified: Wed, 18 Nov 2020 01:36:16 GMT  
		Size: 31.7 MB (31694938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.123-slim` - linux; 386

```console
$ docker pull mono@sha256:7408af128b1227eca68617e6701d448a5eb9bc24aa617e36e1523505bcafd32a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99111735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bba47036df0f4565deac3afa71d5d52b577105edc62e57a528370a0f3af2d643`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:03 GMT
ADD file:51108b89c70ce0773c897be520c84454660f38b84ba556da49c7fe77e5d52416 in / 
# Tue, 13 Oct 2020 01:41:03 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 07:37:13 GMT
ENV MONO_VERSION=6.8.0.123
# Tue, 13 Oct 2020 07:37:25 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 07:38:04 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:97e4efec21eea92209464547d0f52a0f773c505cf4ea9d8090cef667bde145b8`  
		Last Modified: Tue, 13 Oct 2020 01:48:54 GMT  
		Size: 27.8 MB (27750243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5017c5054d34dd5350eadd54ec5d96301cc5c8130e1310f6e8022e87fa0ae8ce`  
		Last Modified: Tue, 13 Oct 2020 07:44:39 GMT  
		Size: 255.8 KB (255833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cef04a59545f975fe314d6e732658db45b6c0c2ad188869d117e721dadcf7249`  
		Last Modified: Tue, 13 Oct 2020 07:44:59 GMT  
		Size: 71.1 MB (71105659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.123-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:8bb18faf02415085f748dfbde98f4222861e1a77ea235d8035cb251d49b86590
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60104648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a583a11099657dd12feee41139ba60e6ece23b38f684b047b8e72d97f62bbd9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:54 GMT
ADD file:9992867f855c9bed54df6d26f3d8076689aff8a51e808fefba7d3b66dab250e5 in / 
# Tue, 13 Oct 2020 01:38:59 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 10:17:07 GMT
ENV MONO_VERSION=6.8.0.123
# Tue, 13 Oct 2020 10:18:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 10:20:14 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:523555c6877c72cfcdec912b4d0053c298b1c97835efc7c6b0211585a06bd563`  
		Last Modified: Tue, 13 Oct 2020 01:50:10 GMT  
		Size: 30.5 MB (30517878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86abab555672e6bfb7c95499bac6717588d8a7630837df56b62caac93e492678`  
		Last Modified: Tue, 13 Oct 2020 10:41:26 GMT  
		Size: 256.1 KB (256072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e455e89a2ebbcda939883181d1f8c8c8b1f22a85f4fedc80a4045074ba40adb`  
		Last Modified: Tue, 13 Oct 2020 10:42:32 GMT  
		Size: 29.3 MB (29330698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.8.0-slim`

```console
$ docker pull mono@sha256:9a4f9ab7eb87475f4040ef5b254218331d7d2199167bd199ad77e4090c2cbe53
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
$ docker pull mono@sha256:f644c3da31661298224f7e4d5702d96ef7e6aa7bd1a6194b78c98cf68734756b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.4 MB (94432119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c38349a5287494d54c3ca7a3993fcd1f8d99f73c876fec674e35c1efc9d7983`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:06:44 GMT
ENV MONO_VERSION=6.8.0.123
# Tue, 13 Oct 2020 08:06:55 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 08:07:40 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23366ca64f7a24bbe3e1609f8d66b5ebc452f78998573e407f88f528c39528a3`  
		Last Modified: Tue, 13 Oct 2020 08:29:04 GMT  
		Size: 255.9 KB (255878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc110778513890ac2d5223325778aae22dc42890ed6c8495ff7ecf4801024643`  
		Last Modified: Tue, 13 Oct 2020 08:29:17 GMT  
		Size: 67.1 MB (67084013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:251f066260187f7daae44d2b0e1c18197b67dc6275508075ae0d2dafa72c2bb8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51634416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bf6a0e393f1c11eff16fe15845a386c8de46aac69339c4113f206093c491b7e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:52:17 GMT
ADD file:b71c0fa4957d6b65af37231a105f3d17cdbafe5c7d6c37b5843ebf619c608aaa in / 
# Tue, 13 Oct 2020 01:52:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:34:46 GMT
ENV MONO_VERSION=6.8.0.123
# Tue, 13 Oct 2020 02:35:14 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 02:36:05 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f991c1e1ee2c48f16625b6b61310bf3c0616c0dbda4762019117e86fd29cf9ce`  
		Last Modified: Tue, 13 Oct 2020 02:01:27 GMT  
		Size: 24.8 MB (24835992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58c01c93058384dcced83ee11026a0e5e2652432af5c3eaa02592a2cebdfdf6`  
		Last Modified: Tue, 13 Oct 2020 02:44:29 GMT  
		Size: 256.0 KB (255998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd8d0a31f42e3311b822b7c94bb005cf72849efb2f5c39943b70702c6631de9`  
		Last Modified: Tue, 13 Oct 2020 02:44:40 GMT  
		Size: 26.5 MB (26542426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:c84e88fc96c15e99d24c04f88bbbc4b73ff77f7a9bfa07c45f384136199087fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48682257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6f5defcf8cb930642b2a9728a83524bbf0e39ae20d2f0e63aa786a2b8d1a0e0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 00:59:29 GMT
ADD file:e423f30ca19eb205a98de21b0545d0a764cfc4f832a9a9631542354d914d98d9 in / 
# Tue, 13 Oct 2020 00:59:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 04:42:00 GMT
ENV MONO_VERSION=6.8.0.123
# Tue, 13 Oct 2020 04:42:16 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 04:43:00 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d6d8411ad43db0022fa0fce094cd2e8b1dd2f8a09d6880ed9beb6b4204867027`  
		Last Modified: Tue, 13 Oct 2020 01:08:28 GMT  
		Size: 22.7 MB (22699849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053722f7b6b8ff8b79ff2487965425c4a35e48783e16f602bac9cc463f1514c7`  
		Last Modified: Tue, 13 Oct 2020 04:50:17 GMT  
		Size: 255.9 KB (255908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3dc69451bafa4aa4ed7b7eed809f3e7039f7e9362c96bff1bb37179a1f035e`  
		Last Modified: Tue, 13 Oct 2020 04:50:28 GMT  
		Size: 25.7 MB (25726500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:6bd885bff156f3ba093c0e9c5c84bb566cff37829bf5c89a64bfc8a7eea67e55
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.8 MB (57813385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7189a284f5129368968186f70de9dbc8b1ba9c09966eba00a988f4a3793c4481`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:31 GMT
ADD file:a70d8c01f8f04f36038968567af779883f3b5ba3147b662b7d170d80418bc23c in / 
# Tue, 17 Nov 2020 20:23:32 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 01:27:35 GMT
ENV MONO_VERSION=6.8.0.123
# Wed, 18 Nov 2020 01:27:56 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 18 Nov 2020 01:28:37 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:29ade854e0dcedde295dd89890d45271e9df839e42124558eb5283508ca70f5c`  
		Last Modified: Tue, 17 Nov 2020 20:32:02 GMT  
		Size: 25.9 MB (25862532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3ec8e5e3abeb88b50e538233a25dcc55fee6941e17c640df3d1c5e0721c663`  
		Last Modified: Wed, 18 Nov 2020 01:36:06 GMT  
		Size: 255.9 KB (255915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df287fd6b7b7749b3830988992ff21aa14dad6f7b628d3616f06d111fa1965b`  
		Last Modified: Wed, 18 Nov 2020 01:36:16 GMT  
		Size: 31.7 MB (31694938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0-slim` - linux; 386

```console
$ docker pull mono@sha256:7408af128b1227eca68617e6701d448a5eb9bc24aa617e36e1523505bcafd32a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99111735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bba47036df0f4565deac3afa71d5d52b577105edc62e57a528370a0f3af2d643`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:03 GMT
ADD file:51108b89c70ce0773c897be520c84454660f38b84ba556da49c7fe77e5d52416 in / 
# Tue, 13 Oct 2020 01:41:03 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 07:37:13 GMT
ENV MONO_VERSION=6.8.0.123
# Tue, 13 Oct 2020 07:37:25 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 07:38:04 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:97e4efec21eea92209464547d0f52a0f773c505cf4ea9d8090cef667bde145b8`  
		Last Modified: Tue, 13 Oct 2020 01:48:54 GMT  
		Size: 27.8 MB (27750243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5017c5054d34dd5350eadd54ec5d96301cc5c8130e1310f6e8022e87fa0ae8ce`  
		Last Modified: Tue, 13 Oct 2020 07:44:39 GMT  
		Size: 255.8 KB (255833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cef04a59545f975fe314d6e732658db45b6c0c2ad188869d117e721dadcf7249`  
		Last Modified: Tue, 13 Oct 2020 07:44:59 GMT  
		Size: 71.1 MB (71105659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:8bb18faf02415085f748dfbde98f4222861e1a77ea235d8035cb251d49b86590
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60104648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a583a11099657dd12feee41139ba60e6ece23b38f684b047b8e72d97f62bbd9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:54 GMT
ADD file:9992867f855c9bed54df6d26f3d8076689aff8a51e808fefba7d3b66dab250e5 in / 
# Tue, 13 Oct 2020 01:38:59 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 10:17:07 GMT
ENV MONO_VERSION=6.8.0.123
# Tue, 13 Oct 2020 10:18:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 10:20:14 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:523555c6877c72cfcdec912b4d0053c298b1c97835efc7c6b0211585a06bd563`  
		Last Modified: Tue, 13 Oct 2020 01:50:10 GMT  
		Size: 30.5 MB (30517878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86abab555672e6bfb7c95499bac6717588d8a7630837df56b62caac93e492678`  
		Last Modified: Tue, 13 Oct 2020 10:41:26 GMT  
		Size: 256.1 KB (256072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e455e89a2ebbcda939883181d1f8c8c8b1f22a85f4fedc80a4045074ba40adb`  
		Last Modified: Tue, 13 Oct 2020 10:42:32 GMT  
		Size: 29.3 MB (29330698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.8-slim`

```console
$ docker pull mono@sha256:9a4f9ab7eb87475f4040ef5b254218331d7d2199167bd199ad77e4090c2cbe53
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
$ docker pull mono@sha256:f644c3da31661298224f7e4d5702d96ef7e6aa7bd1a6194b78c98cf68734756b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.4 MB (94432119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c38349a5287494d54c3ca7a3993fcd1f8d99f73c876fec674e35c1efc9d7983`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:06:44 GMT
ENV MONO_VERSION=6.8.0.123
# Tue, 13 Oct 2020 08:06:55 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 08:07:40 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23366ca64f7a24bbe3e1609f8d66b5ebc452f78998573e407f88f528c39528a3`  
		Last Modified: Tue, 13 Oct 2020 08:29:04 GMT  
		Size: 255.9 KB (255878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc110778513890ac2d5223325778aae22dc42890ed6c8495ff7ecf4801024643`  
		Last Modified: Tue, 13 Oct 2020 08:29:17 GMT  
		Size: 67.1 MB (67084013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:251f066260187f7daae44d2b0e1c18197b67dc6275508075ae0d2dafa72c2bb8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51634416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bf6a0e393f1c11eff16fe15845a386c8de46aac69339c4113f206093c491b7e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:52:17 GMT
ADD file:b71c0fa4957d6b65af37231a105f3d17cdbafe5c7d6c37b5843ebf619c608aaa in / 
# Tue, 13 Oct 2020 01:52:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:34:46 GMT
ENV MONO_VERSION=6.8.0.123
# Tue, 13 Oct 2020 02:35:14 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 02:36:05 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f991c1e1ee2c48f16625b6b61310bf3c0616c0dbda4762019117e86fd29cf9ce`  
		Last Modified: Tue, 13 Oct 2020 02:01:27 GMT  
		Size: 24.8 MB (24835992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58c01c93058384dcced83ee11026a0e5e2652432af5c3eaa02592a2cebdfdf6`  
		Last Modified: Tue, 13 Oct 2020 02:44:29 GMT  
		Size: 256.0 KB (255998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd8d0a31f42e3311b822b7c94bb005cf72849efb2f5c39943b70702c6631de9`  
		Last Modified: Tue, 13 Oct 2020 02:44:40 GMT  
		Size: 26.5 MB (26542426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:c84e88fc96c15e99d24c04f88bbbc4b73ff77f7a9bfa07c45f384136199087fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48682257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6f5defcf8cb930642b2a9728a83524bbf0e39ae20d2f0e63aa786a2b8d1a0e0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 00:59:29 GMT
ADD file:e423f30ca19eb205a98de21b0545d0a764cfc4f832a9a9631542354d914d98d9 in / 
# Tue, 13 Oct 2020 00:59:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 04:42:00 GMT
ENV MONO_VERSION=6.8.0.123
# Tue, 13 Oct 2020 04:42:16 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 04:43:00 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d6d8411ad43db0022fa0fce094cd2e8b1dd2f8a09d6880ed9beb6b4204867027`  
		Last Modified: Tue, 13 Oct 2020 01:08:28 GMT  
		Size: 22.7 MB (22699849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053722f7b6b8ff8b79ff2487965425c4a35e48783e16f602bac9cc463f1514c7`  
		Last Modified: Tue, 13 Oct 2020 04:50:17 GMT  
		Size: 255.9 KB (255908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3dc69451bafa4aa4ed7b7eed809f3e7039f7e9362c96bff1bb37179a1f035e`  
		Last Modified: Tue, 13 Oct 2020 04:50:28 GMT  
		Size: 25.7 MB (25726500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:6bd885bff156f3ba093c0e9c5c84bb566cff37829bf5c89a64bfc8a7eea67e55
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.8 MB (57813385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7189a284f5129368968186f70de9dbc8b1ba9c09966eba00a988f4a3793c4481`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:31 GMT
ADD file:a70d8c01f8f04f36038968567af779883f3b5ba3147b662b7d170d80418bc23c in / 
# Tue, 17 Nov 2020 20:23:32 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 01:27:35 GMT
ENV MONO_VERSION=6.8.0.123
# Wed, 18 Nov 2020 01:27:56 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 18 Nov 2020 01:28:37 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:29ade854e0dcedde295dd89890d45271e9df839e42124558eb5283508ca70f5c`  
		Last Modified: Tue, 17 Nov 2020 20:32:02 GMT  
		Size: 25.9 MB (25862532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3ec8e5e3abeb88b50e538233a25dcc55fee6941e17c640df3d1c5e0721c663`  
		Last Modified: Wed, 18 Nov 2020 01:36:06 GMT  
		Size: 255.9 KB (255915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df287fd6b7b7749b3830988992ff21aa14dad6f7b628d3616f06d111fa1965b`  
		Last Modified: Wed, 18 Nov 2020 01:36:16 GMT  
		Size: 31.7 MB (31694938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8-slim` - linux; 386

```console
$ docker pull mono@sha256:7408af128b1227eca68617e6701d448a5eb9bc24aa617e36e1523505bcafd32a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99111735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bba47036df0f4565deac3afa71d5d52b577105edc62e57a528370a0f3af2d643`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:03 GMT
ADD file:51108b89c70ce0773c897be520c84454660f38b84ba556da49c7fe77e5d52416 in / 
# Tue, 13 Oct 2020 01:41:03 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 07:37:13 GMT
ENV MONO_VERSION=6.8.0.123
# Tue, 13 Oct 2020 07:37:25 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 07:38:04 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:97e4efec21eea92209464547d0f52a0f773c505cf4ea9d8090cef667bde145b8`  
		Last Modified: Tue, 13 Oct 2020 01:48:54 GMT  
		Size: 27.8 MB (27750243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5017c5054d34dd5350eadd54ec5d96301cc5c8130e1310f6e8022e87fa0ae8ce`  
		Last Modified: Tue, 13 Oct 2020 07:44:39 GMT  
		Size: 255.8 KB (255833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cef04a59545f975fe314d6e732658db45b6c0c2ad188869d117e721dadcf7249`  
		Last Modified: Tue, 13 Oct 2020 07:44:59 GMT  
		Size: 71.1 MB (71105659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:8bb18faf02415085f748dfbde98f4222861e1a77ea235d8035cb251d49b86590
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60104648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a583a11099657dd12feee41139ba60e6ece23b38f684b047b8e72d97f62bbd9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:54 GMT
ADD file:9992867f855c9bed54df6d26f3d8076689aff8a51e808fefba7d3b66dab250e5 in / 
# Tue, 13 Oct 2020 01:38:59 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 10:17:07 GMT
ENV MONO_VERSION=6.8.0.123
# Tue, 13 Oct 2020 10:18:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 10:20:14 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:523555c6877c72cfcdec912b4d0053c298b1c97835efc7c6b0211585a06bd563`  
		Last Modified: Tue, 13 Oct 2020 01:50:10 GMT  
		Size: 30.5 MB (30517878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86abab555672e6bfb7c95499bac6717588d8a7630837df56b62caac93e492678`  
		Last Modified: Tue, 13 Oct 2020 10:41:26 GMT  
		Size: 256.1 KB (256072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e455e89a2ebbcda939883181d1f8c8c8b1f22a85f4fedc80a4045074ba40adb`  
		Last Modified: Tue, 13 Oct 2020 10:42:32 GMT  
		Size: 29.3 MB (29330698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6-slim`

```console
$ docker pull mono@sha256:f9cc1d4ca9b6182ddbf6a41a03bed096f663b26dd9c9350d980d83f2e90f7742
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
$ docker pull mono@sha256:3765ac28d39147593372198431028d6b330f0fcf662347678d75205cae7d21f6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.4 MB (94440395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f7e8e7920f90e20657bcacaea38bf659ee3e6001ef3da7e6df0494c995367bb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:07:49 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 08:08:00 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 08:08:57 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f42b4ad878bfc3887ec056c31544fe7c67286e2cbf905efd97752fb01bf7cf`  
		Last Modified: Tue, 13 Oct 2020 08:29:21 GMT  
		Size: 255.9 KB (255885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595630826b1b79ee45e4c4202b61c61ada9c53bf1352e06571dbaa4624660c6f`  
		Last Modified: Tue, 13 Oct 2020 08:29:34 GMT  
		Size: 67.1 MB (67092282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:4f1935b74f258609d63b31cd01cabf54f735b72c77385b4d0486116f7b9ef1db
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51622580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8aaea1ec0574bca839c762a7724f248e6384ba44765e12d60a1eeb21f04760d2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:52:17 GMT
ADD file:b71c0fa4957d6b65af37231a105f3d17cdbafe5c7d6c37b5843ebf619c608aaa in / 
# Tue, 13 Oct 2020 01:52:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:36:19 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 02:36:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 02:37:31 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f991c1e1ee2c48f16625b6b61310bf3c0616c0dbda4762019117e86fd29cf9ce`  
		Last Modified: Tue, 13 Oct 2020 02:01:27 GMT  
		Size: 24.8 MB (24835992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27e131b9898d8f02267f410169b8627b889f6585ad9300d14a4775194301b55`  
		Last Modified: Tue, 13 Oct 2020 02:44:49 GMT  
		Size: 255.9 KB (255938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b82cc14a51474e2d05a0fd59b3fde70aa8fda539de5a302992983e4ffce7b8`  
		Last Modified: Tue, 13 Oct 2020 02:45:01 GMT  
		Size: 26.5 MB (26530650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:bf61cbd2fff2e9323d1f89b46e33accc00aa6aef0f7f4ab533d44ff2d3672097
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48685097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4593f3eb7182d83642b75181ed79a20590556ea1d6460aef0cad9e805bef1e10`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 00:59:29 GMT
ADD file:e423f30ca19eb205a98de21b0545d0a764cfc4f832a9a9631542354d914d98d9 in / 
# Tue, 13 Oct 2020 00:59:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 04:43:09 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 04:43:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 04:44:11 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d6d8411ad43db0022fa0fce094cd2e8b1dd2f8a09d6880ed9beb6b4204867027`  
		Last Modified: Tue, 13 Oct 2020 01:08:28 GMT  
		Size: 22.7 MB (22699849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5228b93feed3135603bc1b4bbda140b6e3e712167c9dd5ccaad1732370cd6b93`  
		Last Modified: Tue, 13 Oct 2020 04:50:37 GMT  
		Size: 255.9 KB (255921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e85494910fa31cd3bb70be77361cab8fa0b333de462a10ce0e2181ee165c0a`  
		Last Modified: Tue, 13 Oct 2020 04:50:46 GMT  
		Size: 25.7 MB (25729327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:f61a1980078fd63569530291f822a8b6ae13ad45b2b80ab0966e6e274bd43760
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57868607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecd1dcf4046ccc6dd611bd3d6b63c8138e7d813b6c0ccd08cd1606e395148fe1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:31 GMT
ADD file:a70d8c01f8f04f36038968567af779883f3b5ba3147b662b7d170d80418bc23c in / 
# Tue, 17 Nov 2020 20:23:32 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 01:28:53 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 18 Nov 2020 01:29:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 18 Nov 2020 01:29:56 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:29ade854e0dcedde295dd89890d45271e9df839e42124558eb5283508ca70f5c`  
		Last Modified: Tue, 17 Nov 2020 20:32:02 GMT  
		Size: 25.9 MB (25862532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808368e9cd11971fa6e53b4a3fbb5559d120515e05c721adff9b9e493870a0f5`  
		Last Modified: Wed, 18 Nov 2020 01:36:25 GMT  
		Size: 255.9 KB (255886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cdf6ac0c679ba4beaf9bad32b903763540d340a1b59395c930a56b288947efe`  
		Last Modified: Wed, 18 Nov 2020 01:36:35 GMT  
		Size: 31.8 MB (31750189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; 386

```console
$ docker pull mono@sha256:30595710e290d4c665ddfdd6521b718f784a35d9a7f951deaa1c50cd12c26d99
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99142199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60ded9fb25b4db7c9c4f48c126b26c7c9188e0b124c54bdc3b8cafb366982817`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:03 GMT
ADD file:51108b89c70ce0773c897be520c84454660f38b84ba556da49c7fe77e5d52416 in / 
# Tue, 13 Oct 2020 01:41:03 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 07:38:18 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 07:38:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 07:39:07 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:97e4efec21eea92209464547d0f52a0f773c505cf4ea9d8090cef667bde145b8`  
		Last Modified: Tue, 13 Oct 2020 01:48:54 GMT  
		Size: 27.8 MB (27750243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9588b02c60fba169bd9cad455764e725c295ddf21085d904d732ef4892d6375f`  
		Last Modified: Tue, 13 Oct 2020 07:45:04 GMT  
		Size: 255.8 KB (255832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf75edd8ea102d6fbbdb5609df6a19925523bdb561e696bd0fb665b5bb2c5a7`  
		Last Modified: Tue, 13 Oct 2020 07:45:21 GMT  
		Size: 71.1 MB (71136124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:445fd5d23b080f1f1a4c37154a548fbc232319eca35a596fc5e3b0f9ec60c409
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60123832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44ccc1548e965ff3511e623f5d42c04512024e85ff17bf5945dcbe2eb2ee1234`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:54 GMT
ADD file:9992867f855c9bed54df6d26f3d8076689aff8a51e808fefba7d3b66dab250e5 in / 
# Tue, 13 Oct 2020 01:38:59 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 10:20:33 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 10:21:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 10:23:38 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:523555c6877c72cfcdec912b4d0053c298b1c97835efc7c6b0211585a06bd563`  
		Last Modified: Tue, 13 Oct 2020 01:50:10 GMT  
		Size: 30.5 MB (30517878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6778a79cc5707eb6c5a21cff2f3f04a05c0ba40bc48c3b3b97f695441e2695fe`  
		Last Modified: Tue, 13 Oct 2020 10:42:46 GMT  
		Size: 256.1 KB (256132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29be084b2430b8c354483c0ac192dd08a2e22fd9687a53e928bf6126d0703187`  
		Last Modified: Tue, 13 Oct 2020 10:43:40 GMT  
		Size: 29.3 MB (29349822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:latest`

```console
$ docker pull mono@sha256:e1c39d26dc47f212bc8ba5bfd282526987f2c9f7a1a124fb7dd2badb9c3e44dc
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
$ docker pull mono@sha256:0beb1b5ba9a0cc0efaaa1148c2682d02351ffb94d77ee74ec5e2fedb625bdd17
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.7 MB (224728267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ffb04a492e34192512ff718aaf68247effd38c5ee58e852b67e750455ca46a3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:07:49 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 08:08:00 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 08:08:57 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Oct 2020 08:28:43 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f42b4ad878bfc3887ec056c31544fe7c67286e2cbf905efd97752fb01bf7cf`  
		Last Modified: Tue, 13 Oct 2020 08:29:21 GMT  
		Size: 255.9 KB (255885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595630826b1b79ee45e4c4202b61c61ada9c53bf1352e06571dbaa4624660c6f`  
		Last Modified: Tue, 13 Oct 2020 08:29:34 GMT  
		Size: 67.1 MB (67092282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f179adbd59957f8069efb25f4b87a0c78f7120ca6935479e58a6c9f0d0f75253`  
		Last Modified: Tue, 13 Oct 2020 08:30:39 GMT  
		Size: 130.3 MB (130287872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm variant v5

```console
$ docker pull mono@sha256:3e601afbb4577fd538dfa06145643ef0c370d3b98b7fdbdeb8e69e6e7c3cc44b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180580641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0b1583a0f54587294ef3fb13293551714e84d35168baa3b742491aac91dc394`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:52:17 GMT
ADD file:b71c0fa4957d6b65af37231a105f3d17cdbafe5c7d6c37b5843ebf619c608aaa in / 
# Tue, 13 Oct 2020 01:52:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:36:19 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 02:36:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 02:37:31 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Oct 2020 02:44:00 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f991c1e1ee2c48f16625b6b61310bf3c0616c0dbda4762019117e86fd29cf9ce`  
		Last Modified: Tue, 13 Oct 2020 02:01:27 GMT  
		Size: 24.8 MB (24835992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27e131b9898d8f02267f410169b8627b889f6585ad9300d14a4775194301b55`  
		Last Modified: Tue, 13 Oct 2020 02:44:49 GMT  
		Size: 255.9 KB (255938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b82cc14a51474e2d05a0fd59b3fde70aa8fda539de5a302992983e4ffce7b8`  
		Last Modified: Tue, 13 Oct 2020 02:45:01 GMT  
		Size: 26.5 MB (26530650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94ad0d9899e6c5c16486a97103eb9bbff1261c084ef2366534ae27653b23704`  
		Last Modified: Tue, 13 Oct 2020 02:46:59 GMT  
		Size: 129.0 MB (128958061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm variant v7

```console
$ docker pull mono@sha256:0e797969122f94b85e9178dd9bece13c7ebd2cacf124520f4275e0ac7cd2b15d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.5 MB (176483530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b81a3bb43255d115e920754f87906a5cd00c5c5ae23a85f06c756f2c42a455b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 00:59:29 GMT
ADD file:e423f30ca19eb205a98de21b0545d0a764cfc4f832a9a9631542354d914d98d9 in / 
# Tue, 13 Oct 2020 00:59:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 04:43:09 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 04:43:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 04:44:11 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Oct 2020 04:49:53 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d6d8411ad43db0022fa0fce094cd2e8b1dd2f8a09d6880ed9beb6b4204867027`  
		Last Modified: Tue, 13 Oct 2020 01:08:28 GMT  
		Size: 22.7 MB (22699849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5228b93feed3135603bc1b4bbda140b6e3e712167c9dd5ccaad1732370cd6b93`  
		Last Modified: Tue, 13 Oct 2020 04:50:37 GMT  
		Size: 255.9 KB (255921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e85494910fa31cd3bb70be77361cab8fa0b333de462a10ce0e2181ee165c0a`  
		Last Modified: Tue, 13 Oct 2020 04:50:46 GMT  
		Size: 25.7 MB (25729327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0179ccf237338944b3401bc8ed480a53bd10956472cd41d05647aeb7fa46ee`  
		Last Modified: Tue, 13 Oct 2020 04:52:43 GMT  
		Size: 127.8 MB (127798433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:0b5ce90bc0624cc3be76e2f4faa9b5ece9459fbda3fd2d1e600b0d03a6693710
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.3 MB (203308506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:684f822e67b92095a97967c053ec1acb78c5d01f5ca24b36822f3fee9136d53f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:31 GMT
ADD file:a70d8c01f8f04f36038968567af779883f3b5ba3147b662b7d170d80418bc23c in / 
# Tue, 17 Nov 2020 20:23:32 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 01:28:53 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 18 Nov 2020 01:29:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 18 Nov 2020 01:29:56 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 18 Nov 2020 01:35:25 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:29ade854e0dcedde295dd89890d45271e9df839e42124558eb5283508ca70f5c`  
		Last Modified: Tue, 17 Nov 2020 20:32:02 GMT  
		Size: 25.9 MB (25862532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808368e9cd11971fa6e53b4a3fbb5559d120515e05c721adff9b9e493870a0f5`  
		Last Modified: Wed, 18 Nov 2020 01:36:25 GMT  
		Size: 255.9 KB (255886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cdf6ac0c679ba4beaf9bad32b903763540d340a1b59395c930a56b288947efe`  
		Last Modified: Wed, 18 Nov 2020 01:36:35 GMT  
		Size: 31.8 MB (31750189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85a8c7edd4b4a3cbd35f220923da50329be4d48bbff3d793963214b91d5e4c9`  
		Last Modified: Wed, 18 Nov 2020 01:38:19 GMT  
		Size: 145.4 MB (145439899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; 386

```console
$ docker pull mono@sha256:134601059016d772aac04e8b006c0467d93094aac62ec0a5a003779f5efb06d0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.5 MB (230532788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c942123328c3a3ae3a83555749eec2e9c668cc58f1cf9a219c5fbff2e472441`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:03 GMT
ADD file:51108b89c70ce0773c897be520c84454660f38b84ba556da49c7fe77e5d52416 in / 
# Tue, 13 Oct 2020 01:41:03 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 07:38:18 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 07:38:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 07:39:07 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Oct 2020 07:44:16 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:97e4efec21eea92209464547d0f52a0f773c505cf4ea9d8090cef667bde145b8`  
		Last Modified: Tue, 13 Oct 2020 01:48:54 GMT  
		Size: 27.8 MB (27750243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9588b02c60fba169bd9cad455764e725c295ddf21085d904d732ef4892d6375f`  
		Last Modified: Tue, 13 Oct 2020 07:45:04 GMT  
		Size: 255.8 KB (255832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf75edd8ea102d6fbbdb5609df6a19925523bdb561e696bd0fb665b5bb2c5a7`  
		Last Modified: Tue, 13 Oct 2020 07:45:21 GMT  
		Size: 71.1 MB (71136124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6087ce14b6fee3f871defe577ae84bcf6db5fe3226dc585305fa9ce5c625d41`  
		Last Modified: Tue, 13 Oct 2020 07:46:42 GMT  
		Size: 131.4 MB (131390589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; ppc64le

```console
$ docker pull mono@sha256:5d8d2256088dfe9d8870d0ad3a58c3bd5428ae3f6f47046f14c4009fad3cdddc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.1 MB (192080743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee6e47cfbad6be2c8b92dd6b5d33888766804f9cdc59ee9042f56068e1499de9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:54 GMT
ADD file:9992867f855c9bed54df6d26f3d8076689aff8a51e808fefba7d3b66dab250e5 in / 
# Tue, 13 Oct 2020 01:38:59 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 10:20:33 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 10:21:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 10:23:38 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 13 Oct 2020 10:40:36 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:523555c6877c72cfcdec912b4d0053c298b1c97835efc7c6b0211585a06bd563`  
		Last Modified: Tue, 13 Oct 2020 01:50:10 GMT  
		Size: 30.5 MB (30517878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6778a79cc5707eb6c5a21cff2f3f04a05c0ba40bc48c3b3b97f695441e2695fe`  
		Last Modified: Tue, 13 Oct 2020 10:42:46 GMT  
		Size: 256.1 KB (256132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29be084b2430b8c354483c0ac192dd08a2e22fd9687a53e928bf6126d0703187`  
		Last Modified: Tue, 13 Oct 2020 10:43:40 GMT  
		Size: 29.3 MB (29349822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89fb777ba4b2b8e659779b45eedfc16ba2052f25ece387db17ba60fd460c08d4`  
		Last Modified: Tue, 13 Oct 2020 10:47:49 GMT  
		Size: 132.0 MB (131956911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:slim`

```console
$ docker pull mono@sha256:f9cc1d4ca9b6182ddbf6a41a03bed096f663b26dd9c9350d980d83f2e90f7742
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
$ docker pull mono@sha256:3765ac28d39147593372198431028d6b330f0fcf662347678d75205cae7d21f6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.4 MB (94440395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f7e8e7920f90e20657bcacaea38bf659ee3e6001ef3da7e6df0494c995367bb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:07:49 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 08:08:00 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 08:08:57 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f42b4ad878bfc3887ec056c31544fe7c67286e2cbf905efd97752fb01bf7cf`  
		Last Modified: Tue, 13 Oct 2020 08:29:21 GMT  
		Size: 255.9 KB (255885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595630826b1b79ee45e4c4202b61c61ada9c53bf1352e06571dbaa4624660c6f`  
		Last Modified: Tue, 13 Oct 2020 08:29:34 GMT  
		Size: 67.1 MB (67092282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:4f1935b74f258609d63b31cd01cabf54f735b72c77385b4d0486116f7b9ef1db
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51622580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8aaea1ec0574bca839c762a7724f248e6384ba44765e12d60a1eeb21f04760d2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:52:17 GMT
ADD file:b71c0fa4957d6b65af37231a105f3d17cdbafe5c7d6c37b5843ebf619c608aaa in / 
# Tue, 13 Oct 2020 01:52:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:36:19 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 02:36:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 02:37:31 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f991c1e1ee2c48f16625b6b61310bf3c0616c0dbda4762019117e86fd29cf9ce`  
		Last Modified: Tue, 13 Oct 2020 02:01:27 GMT  
		Size: 24.8 MB (24835992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27e131b9898d8f02267f410169b8627b889f6585ad9300d14a4775194301b55`  
		Last Modified: Tue, 13 Oct 2020 02:44:49 GMT  
		Size: 255.9 KB (255938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b82cc14a51474e2d05a0fd59b3fde70aa8fda539de5a302992983e4ffce7b8`  
		Last Modified: Tue, 13 Oct 2020 02:45:01 GMT  
		Size: 26.5 MB (26530650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:bf61cbd2fff2e9323d1f89b46e33accc00aa6aef0f7f4ab533d44ff2d3672097
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48685097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4593f3eb7182d83642b75181ed79a20590556ea1d6460aef0cad9e805bef1e10`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 00:59:29 GMT
ADD file:e423f30ca19eb205a98de21b0545d0a764cfc4f832a9a9631542354d914d98d9 in / 
# Tue, 13 Oct 2020 00:59:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 04:43:09 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 04:43:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 04:44:11 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d6d8411ad43db0022fa0fce094cd2e8b1dd2f8a09d6880ed9beb6b4204867027`  
		Last Modified: Tue, 13 Oct 2020 01:08:28 GMT  
		Size: 22.7 MB (22699849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5228b93feed3135603bc1b4bbda140b6e3e712167c9dd5ccaad1732370cd6b93`  
		Last Modified: Tue, 13 Oct 2020 04:50:37 GMT  
		Size: 255.9 KB (255921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e85494910fa31cd3bb70be77361cab8fa0b333de462a10ce0e2181ee165c0a`  
		Last Modified: Tue, 13 Oct 2020 04:50:46 GMT  
		Size: 25.7 MB (25729327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:f61a1980078fd63569530291f822a8b6ae13ad45b2b80ab0966e6e274bd43760
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57868607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecd1dcf4046ccc6dd611bd3d6b63c8138e7d813b6c0ccd08cd1606e395148fe1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:31 GMT
ADD file:a70d8c01f8f04f36038968567af779883f3b5ba3147b662b7d170d80418bc23c in / 
# Tue, 17 Nov 2020 20:23:32 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 01:28:53 GMT
ENV MONO_VERSION=6.10.0.104
# Wed, 18 Nov 2020 01:29:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 18 Nov 2020 01:29:56 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:29ade854e0dcedde295dd89890d45271e9df839e42124558eb5283508ca70f5c`  
		Last Modified: Tue, 17 Nov 2020 20:32:02 GMT  
		Size: 25.9 MB (25862532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808368e9cd11971fa6e53b4a3fbb5559d120515e05c721adff9b9e493870a0f5`  
		Last Modified: Wed, 18 Nov 2020 01:36:25 GMT  
		Size: 255.9 KB (255886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cdf6ac0c679ba4beaf9bad32b903763540d340a1b59395c930a56b288947efe`  
		Last Modified: Wed, 18 Nov 2020 01:36:35 GMT  
		Size: 31.8 MB (31750189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; 386

```console
$ docker pull mono@sha256:30595710e290d4c665ddfdd6521b718f784a35d9a7f951deaa1c50cd12c26d99
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99142199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60ded9fb25b4db7c9c4f48c126b26c7c9188e0b124c54bdc3b8cafb366982817`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:03 GMT
ADD file:51108b89c70ce0773c897be520c84454660f38b84ba556da49c7fe77e5d52416 in / 
# Tue, 13 Oct 2020 01:41:03 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 07:38:18 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 07:38:27 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 07:39:07 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:97e4efec21eea92209464547d0f52a0f773c505cf4ea9d8090cef667bde145b8`  
		Last Modified: Tue, 13 Oct 2020 01:48:54 GMT  
		Size: 27.8 MB (27750243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9588b02c60fba169bd9cad455764e725c295ddf21085d904d732ef4892d6375f`  
		Last Modified: Tue, 13 Oct 2020 07:45:04 GMT  
		Size: 255.8 KB (255832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf75edd8ea102d6fbbdb5609df6a19925523bdb561e696bd0fb665b5bb2c5a7`  
		Last Modified: Tue, 13 Oct 2020 07:45:21 GMT  
		Size: 71.1 MB (71136124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; ppc64le

```console
$ docker pull mono@sha256:445fd5d23b080f1f1a4c37154a548fbc232319eca35a596fc5e3b0f9ec60c409
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60123832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44ccc1548e965ff3511e623f5d42c04512024e85ff17bf5945dcbe2eb2ee1234`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:54 GMT
ADD file:9992867f855c9bed54df6d26f3d8076689aff8a51e808fefba7d3b66dab250e5 in / 
# Tue, 13 Oct 2020 01:38:59 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 10:20:33 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 13 Oct 2020 10:21:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 13 Oct 2020 10:23:38 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:523555c6877c72cfcdec912b4d0053c298b1c97835efc7c6b0211585a06bd563`  
		Last Modified: Tue, 13 Oct 2020 01:50:10 GMT  
		Size: 30.5 MB (30517878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6778a79cc5707eb6c5a21cff2f3f04a05c0ba40bc48c3b3b97f695441e2695fe`  
		Last Modified: Tue, 13 Oct 2020 10:42:46 GMT  
		Size: 256.1 KB (256132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29be084b2430b8c354483c0ac192dd08a2e22fd9687a53e928bf6126d0703187`  
		Last Modified: Tue, 13 Oct 2020 10:43:40 GMT  
		Size: 29.3 MB (29349822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
