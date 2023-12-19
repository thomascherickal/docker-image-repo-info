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
$ docker pull mono@sha256:29abff00ed65eac77557bdb52dca143d5e4670294ab69325b6cc7aa88dc26bd9
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
$ docker pull mono@sha256:246cbaec50ac5ada0821fec2574500aa9f4eac32343bf30bcf536a9b8411d940
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.7 MB (254676997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17e7291203f4ceb144558b61d792902b5a7320a780ea0b3f98de0fdfa868e47a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:21:12 GMT
ADD file:ae5c65eea20f7ddcf93a0aa255b6a08a906ac1a1a65cd2c4b5d1529bf9f6eaf8 in / 
# Tue, 19 Dec 2023 01:21:13 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:02:30 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 19 Dec 2023 02:02:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 02:03:10 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 19 Dec 2023 02:05:07 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:faac0b3889808c27af96e662a1082eef35772c35dcee1c7334f5f5a22b4149d7`  
		Last Modified: Tue, 19 Dec 2023 01:26:21 GMT  
		Size: 27.2 MB (27188221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9316d6ecf4d9ac6063dcc2781466cb9a8b78507bcb06a93963294c8e0c9840a`  
		Last Modified: Tue, 19 Dec 2023 02:11:01 GMT  
		Size: 2.8 MB (2781014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b6e0a2edd3ab1f5afa00ec7a0f6800cf95e79ed10115be03872814aa843752`  
		Last Modified: Tue, 19 Dec 2023 02:11:10 GMT  
		Size: 64.8 MB (64774640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ce8ee7410abd8de3b88f04973391b7d04baf4c65c4b6ba0c165bc051de22f9`  
		Last Modified: Tue, 19 Dec 2023 02:12:08 GMT  
		Size: 159.9 MB (159933122 bytes)  
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
$ docker pull mono@sha256:2592075e4bfe076daddbf021eb176ed18c83c3b57e827be89f81f1b4a80b399d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.0 MB (189019378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a53516a4dd4f7e5b653db5f989d90522b2d3e975f55417fee52a7596d12ef77`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 02:08:27 GMT
ADD file:24df0653e55efc5ba9ec22911758d187c26dbe6bda2d417ff56bc3d9a9072dd4 in / 
# Tue, 19 Dec 2023 02:08:27 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:35:05 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 19 Dec 2023 02:35:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 02:35:41 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 19 Dec 2023 02:37:34 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:99a10db9a1b078c63980e0e4fc7242bdb6d9ba7c91dd8e0883a55756584bea0f`  
		Last Modified: Tue, 19 Dec 2023 02:13:13 GMT  
		Size: 22.8 MB (22795803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3a3e904e68d35ee1e1d34ea1cac63c5011da52b9dabafcbb69468cd863ce5e`  
		Last Modified: Tue, 19 Dec 2023 02:40:07 GMT  
		Size: 2.4 MB (2370806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0bf50e7a2d398d44cc9c9dbdbaea5d96b90aed33dd8fd650e005295e14419dd`  
		Last Modified: Tue, 19 Dec 2023 02:40:12 GMT  
		Size: 23.8 MB (23790518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3feab922704c054c6bb93b29b588fa47af922eaf51b4c556ef14803944df8cc`  
		Last Modified: Tue, 19 Dec 2023 02:41:10 GMT  
		Size: 140.1 MB (140062251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:931a0b2f42bfe790d4e3fe8a2eced807dacf61419ed6c7d9918ce9f4c10e0610
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.4 MB (216408077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91698d8fd69cdd3b5b14611e736194d5553f50ddfe44553a2cefc5b468587a1b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:39 GMT
ADD file:f60673c303a98b4e4c676e3403bc1b7cb316335aba1202205188176810494c07 in / 
# Tue, 19 Dec 2023 01:41:40 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 07:45:01 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 19 Dec 2023 07:45:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 07:45:22 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 19 Dec 2023 07:46:37 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c0b0171eefd1c6d7f85c54d4a609269c9b5e19a0fd8cd787a49c808c6b73cf74`  
		Last Modified: Tue, 19 Dec 2023 01:46:01 GMT  
		Size: 26.0 MB (25969827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866041d2ba1a760a96ca9bf3322602594a35eb1312c1c3c40c5ae3078f61766e`  
		Last Modified: Tue, 19 Dec 2023 07:47:54 GMT  
		Size: 2.6 MB (2645863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfeb9226e7a30640d245f72ba1c26e2bcb224a880d0fddd8423a74d1fc4981e8`  
		Last Modified: Tue, 19 Dec 2023 07:47:58 GMT  
		Size: 29.5 MB (29545120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b5347da712f33dab552d0221a89bd94977f82b9c9583c5edf4d178a4cff373`  
		Last Modified: Tue, 19 Dec 2023 07:48:43 GMT  
		Size: 158.2 MB (158247267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; 386

```console
$ docker pull mono@sha256:568f9b0d910d6c249c7717c6c9c953e5631dd3b00639e0514fbb57ea74d361ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.6 MB (259559822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4663b11a49195455a3b8eb22821e6095a32e9b96120305303316f5a2539c5f8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:39:52 GMT
ADD file:334e70a7f093f24a0d8e3b87a26edb95d1a12e2dc805ddbcf4e75e3e406803a0 in / 
# Tue, 19 Dec 2023 01:39:52 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:43:20 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 19 Dec 2023 03:43:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 03:44:00 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 19 Dec 2023 03:46:15 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:92f20691effe39d2fd17b271760acef5ac648490cb2e2d292d69ce7f39589f17`  
		Last Modified: Tue, 19 Dec 2023 01:45:18 GMT  
		Size: 27.8 MB (27846883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2eee6d230be6ff9e02dfcc5cf0c2007a1cb25419d0d505782510ff2edb870ac`  
		Last Modified: Tue, 19 Dec 2023 03:48:09 GMT  
		Size: 2.8 MB (2792509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4625069d528cf9adc60ffdd7ec17343c361d8cae5329590ef15dad49108594af`  
		Last Modified: Tue, 19 Dec 2023 03:48:24 GMT  
		Size: 68.8 MB (68800526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed1fe186dc5fb79d1535cfcfe78713b75fcafdd4966ac94bf453e4e792207964`  
		Last Modified: Tue, 19 Dec 2023 03:49:41 GMT  
		Size: 160.1 MB (160119904 bytes)  
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
$ docker pull mono@sha256:c1663267870224db329f049113b817370c9459dacc3f11434a2782c5981c7398
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
$ docker pull mono@sha256:5d9397aca3eaf3f6aa14ce7be85a5928ccbefe8553b91ab61949af68b39848eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94743875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd33b75bff8d671d09cf06d52ec2a5a40037113105e4897cdb8f78574918086b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:21:12 GMT
ADD file:ae5c65eea20f7ddcf93a0aa255b6a08a906ac1a1a65cd2c4b5d1529bf9f6eaf8 in / 
# Tue, 19 Dec 2023 01:21:13 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:02:30 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 19 Dec 2023 02:02:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 02:03:10 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:faac0b3889808c27af96e662a1082eef35772c35dcee1c7334f5f5a22b4149d7`  
		Last Modified: Tue, 19 Dec 2023 01:26:21 GMT  
		Size: 27.2 MB (27188221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9316d6ecf4d9ac6063dcc2781466cb9a8b78507bcb06a93963294c8e0c9840a`  
		Last Modified: Tue, 19 Dec 2023 02:11:01 GMT  
		Size: 2.8 MB (2781014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b6e0a2edd3ab1f5afa00ec7a0f6800cf95e79ed10115be03872814aa843752`  
		Last Modified: Tue, 19 Dec 2023 02:11:10 GMT  
		Size: 64.8 MB (64774640 bytes)  
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
$ docker pull mono@sha256:4cb0e804635c105dc75dd91df98fcf599bd882a9e6e082c8673f82b4ade79cfc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48957127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0ac45316a47d4e84353fea61fb7c0f000143904c4a545518f5caf1165ad95b5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 02:08:27 GMT
ADD file:24df0653e55efc5ba9ec22911758d187c26dbe6bda2d417ff56bc3d9a9072dd4 in / 
# Tue, 19 Dec 2023 02:08:27 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:35:05 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 19 Dec 2023 02:35:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 02:35:41 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:99a10db9a1b078c63980e0e4fc7242bdb6d9ba7c91dd8e0883a55756584bea0f`  
		Last Modified: Tue, 19 Dec 2023 02:13:13 GMT  
		Size: 22.8 MB (22795803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3a3e904e68d35ee1e1d34ea1cac63c5011da52b9dabafcbb69468cd863ce5e`  
		Last Modified: Tue, 19 Dec 2023 02:40:07 GMT  
		Size: 2.4 MB (2370806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0bf50e7a2d398d44cc9c9dbdbaea5d96b90aed33dd8fd650e005295e14419dd`  
		Last Modified: Tue, 19 Dec 2023 02:40:12 GMT  
		Size: 23.8 MB (23790518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:3bad9ad63df49a2d1bb2cb885ccdb13dd48df8902d0335dc2d4a499c8eee30f0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.2 MB (58160810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb659361160878c522d144fd8029d9d6f35aa9ee3f64ce39ad2cef260e741107`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:39 GMT
ADD file:f60673c303a98b4e4c676e3403bc1b7cb316335aba1202205188176810494c07 in / 
# Tue, 19 Dec 2023 01:41:40 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 07:45:01 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 19 Dec 2023 07:45:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 07:45:22 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c0b0171eefd1c6d7f85c54d4a609269c9b5e19a0fd8cd787a49c808c6b73cf74`  
		Last Modified: Tue, 19 Dec 2023 01:46:01 GMT  
		Size: 26.0 MB (25969827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866041d2ba1a760a96ca9bf3322602594a35eb1312c1c3c40c5ae3078f61766e`  
		Last Modified: Tue, 19 Dec 2023 07:47:54 GMT  
		Size: 2.6 MB (2645863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfeb9226e7a30640d245f72ba1c26e2bcb224a880d0fddd8423a74d1fc4981e8`  
		Last Modified: Tue, 19 Dec 2023 07:47:58 GMT  
		Size: 29.5 MB (29545120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; 386

```console
$ docker pull mono@sha256:e282710f806fb5b21e940f885dd799a58b43d1464523f86362e58804301bb37c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99439918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec32a3ab39c90a3290469d2be3ee88721bfb84fbbcfb5227498e42967b7cfdf2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:39:52 GMT
ADD file:334e70a7f093f24a0d8e3b87a26edb95d1a12e2dc805ddbcf4e75e3e406803a0 in / 
# Tue, 19 Dec 2023 01:39:52 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:43:20 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 19 Dec 2023 03:43:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 03:44:00 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:92f20691effe39d2fd17b271760acef5ac648490cb2e2d292d69ce7f39589f17`  
		Last Modified: Tue, 19 Dec 2023 01:45:18 GMT  
		Size: 27.8 MB (27846883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2eee6d230be6ff9e02dfcc5cf0c2007a1cb25419d0d505782510ff2edb870ac`  
		Last Modified: Tue, 19 Dec 2023 03:48:09 GMT  
		Size: 2.8 MB (2792509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4625069d528cf9adc60ffdd7ec17343c361d8cae5329590ef15dad49108594af`  
		Last Modified: Tue, 19 Dec 2023 03:48:24 GMT  
		Size: 68.8 MB (68800526 bytes)  
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
$ docker pull mono@sha256:d96cb7625a99a0bb92dc84ab4d5f9d465f9459b5165486d33dc478ee29d5357f
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
$ docker pull mono@sha256:9b6dc2e7992deab34dd5b40dcd42b6f661ad912bb09da8194a630dd98d3bd305
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.1 MB (225081238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d746b4229642bed7b44d4f757f14dced4111b1188ace9d4afd1c6a050a7d99ca`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:21:12 GMT
ADD file:ae5c65eea20f7ddcf93a0aa255b6a08a906ac1a1a65cd2c4b5d1529bf9f6eaf8 in / 
# Tue, 19 Dec 2023 01:21:13 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:03:20 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 19 Dec 2023 02:03:29 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 02:03:55 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 19 Dec 2023 02:10:41 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:faac0b3889808c27af96e662a1082eef35772c35dcee1c7334f5f5a22b4149d7`  
		Last Modified: Tue, 19 Dec 2023 01:26:21 GMT  
		Size: 27.2 MB (27188221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f13f3dd59fe3a246ff4bbcb364491dbbbd1d6f0b46a07a195cd2d3eb4bd0f1`  
		Last Modified: Tue, 19 Dec 2023 02:11:25 GMT  
		Size: 2.8 MB (2781078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671d741e80ab59cd7c96f18cc4d63581ab89129d502b7009ec7913d688224da2`  
		Last Modified: Tue, 19 Dec 2023 02:11:34 GMT  
		Size: 64.8 MB (64780693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4486ee34ad120f7818eafa46fbccb3f6b80b4d1947f47f5dfc9f56b821794785`  
		Last Modified: Tue, 19 Dec 2023 02:12:40 GMT  
		Size: 130.3 MB (130331246 bytes)  
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
$ docker pull mono@sha256:0f23e8c018c14f6c045ede531a6f4f383f041ea48bb8a3ee9f95dc6866733b9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.8 MB (176808080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:418c72ef7529264d26dcf09340c2529d160a761d10c34388cddba329e5af3de1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 02:08:27 GMT
ADD file:24df0653e55efc5ba9ec22911758d187c26dbe6bda2d417ff56bc3d9a9072dd4 in / 
# Tue, 19 Dec 2023 02:08:27 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:35:45 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 19 Dec 2023 02:35:56 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 02:36:21 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 19 Dec 2023 02:39:45 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:99a10db9a1b078c63980e0e4fc7242bdb6d9ba7c91dd8e0883a55756584bea0f`  
		Last Modified: Tue, 19 Dec 2023 02:13:13 GMT  
		Size: 22.8 MB (22795803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da142ddd8cd8157b552d8120bf46aa5785f99cdf1b6677f8d97efd7394ef551f`  
		Last Modified: Tue, 19 Dec 2023 02:40:26 GMT  
		Size: 2.4 MB (2370801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5237f4b09ba1df2fb098913b9c311152a493ba1a1653a1ff6a4cf11535cfd5`  
		Last Modified: Tue, 19 Dec 2023 02:40:31 GMT  
		Size: 23.8 MB (23816124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6023d0613f843d3aa374376733934fad97350ee6379a106dcac89446620ed7f3`  
		Last Modified: Tue, 19 Dec 2023 02:41:50 GMT  
		Size: 127.8 MB (127825352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:61a1008a503bd65d405a1f022f6ad8e3a2ca42532d3e1b6bf25abf4437ae866a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.7 MB (203695626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb51c87c9f02eec247046bdbd3e0e0cec18272649d2b8ee37b036315ac9fcd56`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:39 GMT
ADD file:f60673c303a98b4e4c676e3403bc1b7cb316335aba1202205188176810494c07 in / 
# Tue, 19 Dec 2023 01:41:40 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 07:45:24 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 19 Dec 2023 07:45:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 07:45:45 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 19 Dec 2023 07:47:33 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c0b0171eefd1c6d7f85c54d4a609269c9b5e19a0fd8cd787a49c808c6b73cf74`  
		Last Modified: Tue, 19 Dec 2023 01:46:01 GMT  
		Size: 26.0 MB (25969827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01bbc15c5e3ce1e7ce5ea3e09a23a407046f4775e5dc2dd52883b6311840a55`  
		Last Modified: Tue, 19 Dec 2023 07:48:11 GMT  
		Size: 2.6 MB (2645836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d898d5ff28952a1d776a0ecb2b2e7acc8ff675e56cdfd13cd6d18333ec5adc`  
		Last Modified: Tue, 19 Dec 2023 07:48:14 GMT  
		Size: 29.6 MB (29575268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e33e32f4c7e55a403f54106f680bb7db8c1728546356e896cd38b0e227ba845`  
		Last Modified: Tue, 19 Dec 2023 07:49:14 GMT  
		Size: 145.5 MB (145504695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; 386

```console
$ docker pull mono@sha256:119f9727f09292f5ac439da089835a10b0bbe049bb55d9a95d29c5ef5d13398d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.9 MB (230903797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:278257dbf749c24c411290cb504a0f8958ff5fda349edce6c7581328c883d012`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:39:52 GMT
ADD file:334e70a7f093f24a0d8e3b87a26edb95d1a12e2dc805ddbcf4e75e3e406803a0 in / 
# Tue, 19 Dec 2023 01:39:52 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:44:08 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 19 Dec 2023 03:44:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 03:44:46 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 19 Dec 2023 03:47:40 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:92f20691effe39d2fd17b271760acef5ac648490cb2e2d292d69ce7f39589f17`  
		Last Modified: Tue, 19 Dec 2023 01:45:18 GMT  
		Size: 27.8 MB (27846883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb2baa046720d9e160895f85db22371357624a08c1c46ceacd4e2ab3ac2bfd3`  
		Last Modified: Tue, 19 Dec 2023 03:48:40 GMT  
		Size: 2.8 MB (2792512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44bc92d1ce0d747f75bc783f617496d7838a75df36701b922aee6c7812ebc812`  
		Last Modified: Tue, 19 Dec 2023 03:48:54 GMT  
		Size: 68.8 MB (68809993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e522c564bab3c2bc67cc68e95490d9082da771b86a1344b7cc64a618d7fe39bc`  
		Last Modified: Tue, 19 Dec 2023 03:50:25 GMT  
		Size: 131.5 MB (131454409 bytes)  
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
$ docker pull mono@sha256:a65c462cff7e805518b7883a2fd76bf3d06c3359aaa0ba6cc474141038058e02
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
$ docker pull mono@sha256:66aaa770ddf55a9142fc1ff24c4fb47678b339d891ad5b7dd24f06160fac5e18
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94749992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:209e8faf67757ac88e1ce97747798356384787d2abfc1722747a5d2fdd232950`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:21:12 GMT
ADD file:ae5c65eea20f7ddcf93a0aa255b6a08a906ac1a1a65cd2c4b5d1529bf9f6eaf8 in / 
# Tue, 19 Dec 2023 01:21:13 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:03:20 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 19 Dec 2023 02:03:29 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 02:03:55 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:faac0b3889808c27af96e662a1082eef35772c35dcee1c7334f5f5a22b4149d7`  
		Last Modified: Tue, 19 Dec 2023 01:26:21 GMT  
		Size: 27.2 MB (27188221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f13f3dd59fe3a246ff4bbcb364491dbbbd1d6f0b46a07a195cd2d3eb4bd0f1`  
		Last Modified: Tue, 19 Dec 2023 02:11:25 GMT  
		Size: 2.8 MB (2781078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671d741e80ab59cd7c96f18cc4d63581ab89129d502b7009ec7913d688224da2`  
		Last Modified: Tue, 19 Dec 2023 02:11:34 GMT  
		Size: 64.8 MB (64780693 bytes)  
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
$ docker pull mono@sha256:1c8e9d762ce5c29d5b237e18b3c565e3af13f8a1c308e6a43c796aa7dabf8666
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48982728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2069d099641a34b1509c835974b23bb1848f0c4347b5d48dec8d232fd963e071`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 02:08:27 GMT
ADD file:24df0653e55efc5ba9ec22911758d187c26dbe6bda2d417ff56bc3d9a9072dd4 in / 
# Tue, 19 Dec 2023 02:08:27 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:35:45 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 19 Dec 2023 02:35:56 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 02:36:21 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:99a10db9a1b078c63980e0e4fc7242bdb6d9ba7c91dd8e0883a55756584bea0f`  
		Last Modified: Tue, 19 Dec 2023 02:13:13 GMT  
		Size: 22.8 MB (22795803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da142ddd8cd8157b552d8120bf46aa5785f99cdf1b6677f8d97efd7394ef551f`  
		Last Modified: Tue, 19 Dec 2023 02:40:26 GMT  
		Size: 2.4 MB (2370801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5237f4b09ba1df2fb098913b9c311152a493ba1a1653a1ff6a4cf11535cfd5`  
		Last Modified: Tue, 19 Dec 2023 02:40:31 GMT  
		Size: 23.8 MB (23816124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:a43c98f423fbf6ccae42c790565f0ca5b5f1e24ab9362920d3d0915019a0fe53
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.2 MB (58190931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c4ef2ea49e0a9f2dab129eb2d46b00bc37376aa38e9fc53008ff429f1ccd80a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:39 GMT
ADD file:f60673c303a98b4e4c676e3403bc1b7cb316335aba1202205188176810494c07 in / 
# Tue, 19 Dec 2023 01:41:40 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 07:45:24 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 19 Dec 2023 07:45:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 07:45:45 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c0b0171eefd1c6d7f85c54d4a609269c9b5e19a0fd8cd787a49c808c6b73cf74`  
		Last Modified: Tue, 19 Dec 2023 01:46:01 GMT  
		Size: 26.0 MB (25969827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01bbc15c5e3ce1e7ce5ea3e09a23a407046f4775e5dc2dd52883b6311840a55`  
		Last Modified: Tue, 19 Dec 2023 07:48:11 GMT  
		Size: 2.6 MB (2645836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d898d5ff28952a1d776a0ecb2b2e7acc8ff675e56cdfd13cd6d18333ec5adc`  
		Last Modified: Tue, 19 Dec 2023 07:48:14 GMT  
		Size: 29.6 MB (29575268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; 386

```console
$ docker pull mono@sha256:6a7ce04f7e59d9116767ad0be42a79ee1599331d4248182090770e2d22a8c4be
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99449388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6620d90b0c60f8875dcbc081357d45eea5eff420c3c537715ff6ee3e2341b5cf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:39:52 GMT
ADD file:334e70a7f093f24a0d8e3b87a26edb95d1a12e2dc805ddbcf4e75e3e406803a0 in / 
# Tue, 19 Dec 2023 01:39:52 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:44:08 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 19 Dec 2023 03:44:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 03:44:46 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:92f20691effe39d2fd17b271760acef5ac648490cb2e2d292d69ce7f39589f17`  
		Last Modified: Tue, 19 Dec 2023 01:45:18 GMT  
		Size: 27.8 MB (27846883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb2baa046720d9e160895f85db22371357624a08c1c46ceacd4e2ab3ac2bfd3`  
		Last Modified: Tue, 19 Dec 2023 03:48:40 GMT  
		Size: 2.8 MB (2792512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44bc92d1ce0d747f75bc783f617496d7838a75df36701b922aee6c7812ebc812`  
		Last Modified: Tue, 19 Dec 2023 03:48:54 GMT  
		Size: 68.8 MB (68809993 bytes)  
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
$ docker pull mono@sha256:d96cb7625a99a0bb92dc84ab4d5f9d465f9459b5165486d33dc478ee29d5357f
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
$ docker pull mono@sha256:9b6dc2e7992deab34dd5b40dcd42b6f661ad912bb09da8194a630dd98d3bd305
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.1 MB (225081238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d746b4229642bed7b44d4f757f14dced4111b1188ace9d4afd1c6a050a7d99ca`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:21:12 GMT
ADD file:ae5c65eea20f7ddcf93a0aa255b6a08a906ac1a1a65cd2c4b5d1529bf9f6eaf8 in / 
# Tue, 19 Dec 2023 01:21:13 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:03:20 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 19 Dec 2023 02:03:29 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 02:03:55 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 19 Dec 2023 02:10:41 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:faac0b3889808c27af96e662a1082eef35772c35dcee1c7334f5f5a22b4149d7`  
		Last Modified: Tue, 19 Dec 2023 01:26:21 GMT  
		Size: 27.2 MB (27188221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f13f3dd59fe3a246ff4bbcb364491dbbbd1d6f0b46a07a195cd2d3eb4bd0f1`  
		Last Modified: Tue, 19 Dec 2023 02:11:25 GMT  
		Size: 2.8 MB (2781078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671d741e80ab59cd7c96f18cc4d63581ab89129d502b7009ec7913d688224da2`  
		Last Modified: Tue, 19 Dec 2023 02:11:34 GMT  
		Size: 64.8 MB (64780693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4486ee34ad120f7818eafa46fbccb3f6b80b4d1947f47f5dfc9f56b821794785`  
		Last Modified: Tue, 19 Dec 2023 02:12:40 GMT  
		Size: 130.3 MB (130331246 bytes)  
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
$ docker pull mono@sha256:0f23e8c018c14f6c045ede531a6f4f383f041ea48bb8a3ee9f95dc6866733b9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.8 MB (176808080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:418c72ef7529264d26dcf09340c2529d160a761d10c34388cddba329e5af3de1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 02:08:27 GMT
ADD file:24df0653e55efc5ba9ec22911758d187c26dbe6bda2d417ff56bc3d9a9072dd4 in / 
# Tue, 19 Dec 2023 02:08:27 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:35:45 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 19 Dec 2023 02:35:56 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 02:36:21 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 19 Dec 2023 02:39:45 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:99a10db9a1b078c63980e0e4fc7242bdb6d9ba7c91dd8e0883a55756584bea0f`  
		Last Modified: Tue, 19 Dec 2023 02:13:13 GMT  
		Size: 22.8 MB (22795803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da142ddd8cd8157b552d8120bf46aa5785f99cdf1b6677f8d97efd7394ef551f`  
		Last Modified: Tue, 19 Dec 2023 02:40:26 GMT  
		Size: 2.4 MB (2370801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5237f4b09ba1df2fb098913b9c311152a493ba1a1653a1ff6a4cf11535cfd5`  
		Last Modified: Tue, 19 Dec 2023 02:40:31 GMT  
		Size: 23.8 MB (23816124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6023d0613f843d3aa374376733934fad97350ee6379a106dcac89446620ed7f3`  
		Last Modified: Tue, 19 Dec 2023 02:41:50 GMT  
		Size: 127.8 MB (127825352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:61a1008a503bd65d405a1f022f6ad8e3a2ca42532d3e1b6bf25abf4437ae866a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.7 MB (203695626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb51c87c9f02eec247046bdbd3e0e0cec18272649d2b8ee37b036315ac9fcd56`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:39 GMT
ADD file:f60673c303a98b4e4c676e3403bc1b7cb316335aba1202205188176810494c07 in / 
# Tue, 19 Dec 2023 01:41:40 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 07:45:24 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 19 Dec 2023 07:45:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 07:45:45 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 19 Dec 2023 07:47:33 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c0b0171eefd1c6d7f85c54d4a609269c9b5e19a0fd8cd787a49c808c6b73cf74`  
		Last Modified: Tue, 19 Dec 2023 01:46:01 GMT  
		Size: 26.0 MB (25969827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01bbc15c5e3ce1e7ce5ea3e09a23a407046f4775e5dc2dd52883b6311840a55`  
		Last Modified: Tue, 19 Dec 2023 07:48:11 GMT  
		Size: 2.6 MB (2645836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d898d5ff28952a1d776a0ecb2b2e7acc8ff675e56cdfd13cd6d18333ec5adc`  
		Last Modified: Tue, 19 Dec 2023 07:48:14 GMT  
		Size: 29.6 MB (29575268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e33e32f4c7e55a403f54106f680bb7db8c1728546356e896cd38b0e227ba845`  
		Last Modified: Tue, 19 Dec 2023 07:49:14 GMT  
		Size: 145.5 MB (145504695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; 386

```console
$ docker pull mono@sha256:119f9727f09292f5ac439da089835a10b0bbe049bb55d9a95d29c5ef5d13398d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.9 MB (230903797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:278257dbf749c24c411290cb504a0f8958ff5fda349edce6c7581328c883d012`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:39:52 GMT
ADD file:334e70a7f093f24a0d8e3b87a26edb95d1a12e2dc805ddbcf4e75e3e406803a0 in / 
# Tue, 19 Dec 2023 01:39:52 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:44:08 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 19 Dec 2023 03:44:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 03:44:46 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 19 Dec 2023 03:47:40 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:92f20691effe39d2fd17b271760acef5ac648490cb2e2d292d69ce7f39589f17`  
		Last Modified: Tue, 19 Dec 2023 01:45:18 GMT  
		Size: 27.8 MB (27846883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb2baa046720d9e160895f85db22371357624a08c1c46ceacd4e2ab3ac2bfd3`  
		Last Modified: Tue, 19 Dec 2023 03:48:40 GMT  
		Size: 2.8 MB (2792512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44bc92d1ce0d747f75bc783f617496d7838a75df36701b922aee6c7812ebc812`  
		Last Modified: Tue, 19 Dec 2023 03:48:54 GMT  
		Size: 68.8 MB (68809993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e522c564bab3c2bc67cc68e95490d9082da771b86a1344b7cc64a618d7fe39bc`  
		Last Modified: Tue, 19 Dec 2023 03:50:25 GMT  
		Size: 131.5 MB (131454409 bytes)  
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
$ docker pull mono@sha256:a65c462cff7e805518b7883a2fd76bf3d06c3359aaa0ba6cc474141038058e02
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
$ docker pull mono@sha256:66aaa770ddf55a9142fc1ff24c4fb47678b339d891ad5b7dd24f06160fac5e18
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94749992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:209e8faf67757ac88e1ce97747798356384787d2abfc1722747a5d2fdd232950`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:21:12 GMT
ADD file:ae5c65eea20f7ddcf93a0aa255b6a08a906ac1a1a65cd2c4b5d1529bf9f6eaf8 in / 
# Tue, 19 Dec 2023 01:21:13 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:03:20 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 19 Dec 2023 02:03:29 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 02:03:55 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:faac0b3889808c27af96e662a1082eef35772c35dcee1c7334f5f5a22b4149d7`  
		Last Modified: Tue, 19 Dec 2023 01:26:21 GMT  
		Size: 27.2 MB (27188221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f13f3dd59fe3a246ff4bbcb364491dbbbd1d6f0b46a07a195cd2d3eb4bd0f1`  
		Last Modified: Tue, 19 Dec 2023 02:11:25 GMT  
		Size: 2.8 MB (2781078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671d741e80ab59cd7c96f18cc4d63581ab89129d502b7009ec7913d688224da2`  
		Last Modified: Tue, 19 Dec 2023 02:11:34 GMT  
		Size: 64.8 MB (64780693 bytes)  
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
$ docker pull mono@sha256:1c8e9d762ce5c29d5b237e18b3c565e3af13f8a1c308e6a43c796aa7dabf8666
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48982728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2069d099641a34b1509c835974b23bb1848f0c4347b5d48dec8d232fd963e071`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 02:08:27 GMT
ADD file:24df0653e55efc5ba9ec22911758d187c26dbe6bda2d417ff56bc3d9a9072dd4 in / 
# Tue, 19 Dec 2023 02:08:27 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:35:45 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 19 Dec 2023 02:35:56 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 02:36:21 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:99a10db9a1b078c63980e0e4fc7242bdb6d9ba7c91dd8e0883a55756584bea0f`  
		Last Modified: Tue, 19 Dec 2023 02:13:13 GMT  
		Size: 22.8 MB (22795803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da142ddd8cd8157b552d8120bf46aa5785f99cdf1b6677f8d97efd7394ef551f`  
		Last Modified: Tue, 19 Dec 2023 02:40:26 GMT  
		Size: 2.4 MB (2370801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5237f4b09ba1df2fb098913b9c311152a493ba1a1653a1ff6a4cf11535cfd5`  
		Last Modified: Tue, 19 Dec 2023 02:40:31 GMT  
		Size: 23.8 MB (23816124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:a43c98f423fbf6ccae42c790565f0ca5b5f1e24ab9362920d3d0915019a0fe53
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.2 MB (58190931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c4ef2ea49e0a9f2dab129eb2d46b00bc37376aa38e9fc53008ff429f1ccd80a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:39 GMT
ADD file:f60673c303a98b4e4c676e3403bc1b7cb316335aba1202205188176810494c07 in / 
# Tue, 19 Dec 2023 01:41:40 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 07:45:24 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 19 Dec 2023 07:45:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 07:45:45 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c0b0171eefd1c6d7f85c54d4a609269c9b5e19a0fd8cd787a49c808c6b73cf74`  
		Last Modified: Tue, 19 Dec 2023 01:46:01 GMT  
		Size: 26.0 MB (25969827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01bbc15c5e3ce1e7ce5ea3e09a23a407046f4775e5dc2dd52883b6311840a55`  
		Last Modified: Tue, 19 Dec 2023 07:48:11 GMT  
		Size: 2.6 MB (2645836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d898d5ff28952a1d776a0ecb2b2e7acc8ff675e56cdfd13cd6d18333ec5adc`  
		Last Modified: Tue, 19 Dec 2023 07:48:14 GMT  
		Size: 29.6 MB (29575268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; 386

```console
$ docker pull mono@sha256:6a7ce04f7e59d9116767ad0be42a79ee1599331d4248182090770e2d22a8c4be
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99449388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6620d90b0c60f8875dcbc081357d45eea5eff420c3c537715ff6ee3e2341b5cf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:39:52 GMT
ADD file:334e70a7f093f24a0d8e3b87a26edb95d1a12e2dc805ddbcf4e75e3e406803a0 in / 
# Tue, 19 Dec 2023 01:39:52 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:44:08 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 19 Dec 2023 03:44:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 03:44:46 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:92f20691effe39d2fd17b271760acef5ac648490cb2e2d292d69ce7f39589f17`  
		Last Modified: Tue, 19 Dec 2023 01:45:18 GMT  
		Size: 27.8 MB (27846883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb2baa046720d9e160895f85db22371357624a08c1c46ceacd4e2ab3ac2bfd3`  
		Last Modified: Tue, 19 Dec 2023 03:48:40 GMT  
		Size: 2.8 MB (2792512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44bc92d1ce0d747f75bc783f617496d7838a75df36701b922aee6c7812ebc812`  
		Last Modified: Tue, 19 Dec 2023 03:48:54 GMT  
		Size: 68.8 MB (68809993 bytes)  
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
$ docker pull mono@sha256:d96cb7625a99a0bb92dc84ab4d5f9d465f9459b5165486d33dc478ee29d5357f
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
$ docker pull mono@sha256:9b6dc2e7992deab34dd5b40dcd42b6f661ad912bb09da8194a630dd98d3bd305
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.1 MB (225081238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d746b4229642bed7b44d4f757f14dced4111b1188ace9d4afd1c6a050a7d99ca`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:21:12 GMT
ADD file:ae5c65eea20f7ddcf93a0aa255b6a08a906ac1a1a65cd2c4b5d1529bf9f6eaf8 in / 
# Tue, 19 Dec 2023 01:21:13 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:03:20 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 19 Dec 2023 02:03:29 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 02:03:55 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 19 Dec 2023 02:10:41 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:faac0b3889808c27af96e662a1082eef35772c35dcee1c7334f5f5a22b4149d7`  
		Last Modified: Tue, 19 Dec 2023 01:26:21 GMT  
		Size: 27.2 MB (27188221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f13f3dd59fe3a246ff4bbcb364491dbbbd1d6f0b46a07a195cd2d3eb4bd0f1`  
		Last Modified: Tue, 19 Dec 2023 02:11:25 GMT  
		Size: 2.8 MB (2781078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671d741e80ab59cd7c96f18cc4d63581ab89129d502b7009ec7913d688224da2`  
		Last Modified: Tue, 19 Dec 2023 02:11:34 GMT  
		Size: 64.8 MB (64780693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4486ee34ad120f7818eafa46fbccb3f6b80b4d1947f47f5dfc9f56b821794785`  
		Last Modified: Tue, 19 Dec 2023 02:12:40 GMT  
		Size: 130.3 MB (130331246 bytes)  
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
$ docker pull mono@sha256:0f23e8c018c14f6c045ede531a6f4f383f041ea48bb8a3ee9f95dc6866733b9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.8 MB (176808080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:418c72ef7529264d26dcf09340c2529d160a761d10c34388cddba329e5af3de1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 02:08:27 GMT
ADD file:24df0653e55efc5ba9ec22911758d187c26dbe6bda2d417ff56bc3d9a9072dd4 in / 
# Tue, 19 Dec 2023 02:08:27 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:35:45 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 19 Dec 2023 02:35:56 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 02:36:21 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 19 Dec 2023 02:39:45 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:99a10db9a1b078c63980e0e4fc7242bdb6d9ba7c91dd8e0883a55756584bea0f`  
		Last Modified: Tue, 19 Dec 2023 02:13:13 GMT  
		Size: 22.8 MB (22795803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da142ddd8cd8157b552d8120bf46aa5785f99cdf1b6677f8d97efd7394ef551f`  
		Last Modified: Tue, 19 Dec 2023 02:40:26 GMT  
		Size: 2.4 MB (2370801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5237f4b09ba1df2fb098913b9c311152a493ba1a1653a1ff6a4cf11535cfd5`  
		Last Modified: Tue, 19 Dec 2023 02:40:31 GMT  
		Size: 23.8 MB (23816124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6023d0613f843d3aa374376733934fad97350ee6379a106dcac89446620ed7f3`  
		Last Modified: Tue, 19 Dec 2023 02:41:50 GMT  
		Size: 127.8 MB (127825352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:61a1008a503bd65d405a1f022f6ad8e3a2ca42532d3e1b6bf25abf4437ae866a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.7 MB (203695626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb51c87c9f02eec247046bdbd3e0e0cec18272649d2b8ee37b036315ac9fcd56`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:39 GMT
ADD file:f60673c303a98b4e4c676e3403bc1b7cb316335aba1202205188176810494c07 in / 
# Tue, 19 Dec 2023 01:41:40 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 07:45:24 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 19 Dec 2023 07:45:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 07:45:45 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 19 Dec 2023 07:47:33 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c0b0171eefd1c6d7f85c54d4a609269c9b5e19a0fd8cd787a49c808c6b73cf74`  
		Last Modified: Tue, 19 Dec 2023 01:46:01 GMT  
		Size: 26.0 MB (25969827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01bbc15c5e3ce1e7ce5ea3e09a23a407046f4775e5dc2dd52883b6311840a55`  
		Last Modified: Tue, 19 Dec 2023 07:48:11 GMT  
		Size: 2.6 MB (2645836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d898d5ff28952a1d776a0ecb2b2e7acc8ff675e56cdfd13cd6d18333ec5adc`  
		Last Modified: Tue, 19 Dec 2023 07:48:14 GMT  
		Size: 29.6 MB (29575268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e33e32f4c7e55a403f54106f680bb7db8c1728546356e896cd38b0e227ba845`  
		Last Modified: Tue, 19 Dec 2023 07:49:14 GMT  
		Size: 145.5 MB (145504695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; 386

```console
$ docker pull mono@sha256:119f9727f09292f5ac439da089835a10b0bbe049bb55d9a95d29c5ef5d13398d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.9 MB (230903797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:278257dbf749c24c411290cb504a0f8958ff5fda349edce6c7581328c883d012`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:39:52 GMT
ADD file:334e70a7f093f24a0d8e3b87a26edb95d1a12e2dc805ddbcf4e75e3e406803a0 in / 
# Tue, 19 Dec 2023 01:39:52 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:44:08 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 19 Dec 2023 03:44:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 03:44:46 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 19 Dec 2023 03:47:40 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:92f20691effe39d2fd17b271760acef5ac648490cb2e2d292d69ce7f39589f17`  
		Last Modified: Tue, 19 Dec 2023 01:45:18 GMT  
		Size: 27.8 MB (27846883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb2baa046720d9e160895f85db22371357624a08c1c46ceacd4e2ab3ac2bfd3`  
		Last Modified: Tue, 19 Dec 2023 03:48:40 GMT  
		Size: 2.8 MB (2792512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44bc92d1ce0d747f75bc783f617496d7838a75df36701b922aee6c7812ebc812`  
		Last Modified: Tue, 19 Dec 2023 03:48:54 GMT  
		Size: 68.8 MB (68809993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e522c564bab3c2bc67cc68e95490d9082da771b86a1344b7cc64a618d7fe39bc`  
		Last Modified: Tue, 19 Dec 2023 03:50:25 GMT  
		Size: 131.5 MB (131454409 bytes)  
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
$ docker pull mono@sha256:a65c462cff7e805518b7883a2fd76bf3d06c3359aaa0ba6cc474141038058e02
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
$ docker pull mono@sha256:66aaa770ddf55a9142fc1ff24c4fb47678b339d891ad5b7dd24f06160fac5e18
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94749992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:209e8faf67757ac88e1ce97747798356384787d2abfc1722747a5d2fdd232950`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:21:12 GMT
ADD file:ae5c65eea20f7ddcf93a0aa255b6a08a906ac1a1a65cd2c4b5d1529bf9f6eaf8 in / 
# Tue, 19 Dec 2023 01:21:13 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:03:20 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 19 Dec 2023 02:03:29 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 02:03:55 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:faac0b3889808c27af96e662a1082eef35772c35dcee1c7334f5f5a22b4149d7`  
		Last Modified: Tue, 19 Dec 2023 01:26:21 GMT  
		Size: 27.2 MB (27188221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f13f3dd59fe3a246ff4bbcb364491dbbbd1d6f0b46a07a195cd2d3eb4bd0f1`  
		Last Modified: Tue, 19 Dec 2023 02:11:25 GMT  
		Size: 2.8 MB (2781078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671d741e80ab59cd7c96f18cc4d63581ab89129d502b7009ec7913d688224da2`  
		Last Modified: Tue, 19 Dec 2023 02:11:34 GMT  
		Size: 64.8 MB (64780693 bytes)  
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
$ docker pull mono@sha256:1c8e9d762ce5c29d5b237e18b3c565e3af13f8a1c308e6a43c796aa7dabf8666
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48982728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2069d099641a34b1509c835974b23bb1848f0c4347b5d48dec8d232fd963e071`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 02:08:27 GMT
ADD file:24df0653e55efc5ba9ec22911758d187c26dbe6bda2d417ff56bc3d9a9072dd4 in / 
# Tue, 19 Dec 2023 02:08:27 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:35:45 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 19 Dec 2023 02:35:56 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 02:36:21 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:99a10db9a1b078c63980e0e4fc7242bdb6d9ba7c91dd8e0883a55756584bea0f`  
		Last Modified: Tue, 19 Dec 2023 02:13:13 GMT  
		Size: 22.8 MB (22795803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da142ddd8cd8157b552d8120bf46aa5785f99cdf1b6677f8d97efd7394ef551f`  
		Last Modified: Tue, 19 Dec 2023 02:40:26 GMT  
		Size: 2.4 MB (2370801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5237f4b09ba1df2fb098913b9c311152a493ba1a1653a1ff6a4cf11535cfd5`  
		Last Modified: Tue, 19 Dec 2023 02:40:31 GMT  
		Size: 23.8 MB (23816124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:a43c98f423fbf6ccae42c790565f0ca5b5f1e24ab9362920d3d0915019a0fe53
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.2 MB (58190931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c4ef2ea49e0a9f2dab129eb2d46b00bc37376aa38e9fc53008ff429f1ccd80a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:39 GMT
ADD file:f60673c303a98b4e4c676e3403bc1b7cb316335aba1202205188176810494c07 in / 
# Tue, 19 Dec 2023 01:41:40 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 07:45:24 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 19 Dec 2023 07:45:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 07:45:45 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c0b0171eefd1c6d7f85c54d4a609269c9b5e19a0fd8cd787a49c808c6b73cf74`  
		Last Modified: Tue, 19 Dec 2023 01:46:01 GMT  
		Size: 26.0 MB (25969827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01bbc15c5e3ce1e7ce5ea3e09a23a407046f4775e5dc2dd52883b6311840a55`  
		Last Modified: Tue, 19 Dec 2023 07:48:11 GMT  
		Size: 2.6 MB (2645836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d898d5ff28952a1d776a0ecb2b2e7acc8ff675e56cdfd13cd6d18333ec5adc`  
		Last Modified: Tue, 19 Dec 2023 07:48:14 GMT  
		Size: 29.6 MB (29575268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; 386

```console
$ docker pull mono@sha256:6a7ce04f7e59d9116767ad0be42a79ee1599331d4248182090770e2d22a8c4be
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99449388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6620d90b0c60f8875dcbc081357d45eea5eff420c3c537715ff6ee3e2341b5cf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:39:52 GMT
ADD file:334e70a7f093f24a0d8e3b87a26edb95d1a12e2dc805ddbcf4e75e3e406803a0 in / 
# Tue, 19 Dec 2023 01:39:52 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:44:08 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 19 Dec 2023 03:44:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 03:44:46 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:92f20691effe39d2fd17b271760acef5ac648490cb2e2d292d69ce7f39589f17`  
		Last Modified: Tue, 19 Dec 2023 01:45:18 GMT  
		Size: 27.8 MB (27846883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb2baa046720d9e160895f85db22371357624a08c1c46ceacd4e2ab3ac2bfd3`  
		Last Modified: Tue, 19 Dec 2023 03:48:40 GMT  
		Size: 2.8 MB (2792512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44bc92d1ce0d747f75bc783f617496d7838a75df36701b922aee6c7812ebc812`  
		Last Modified: Tue, 19 Dec 2023 03:48:54 GMT  
		Size: 68.8 MB (68809993 bytes)  
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
$ docker pull mono@sha256:29abff00ed65eac77557bdb52dca143d5e4670294ab69325b6cc7aa88dc26bd9
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
$ docker pull mono@sha256:246cbaec50ac5ada0821fec2574500aa9f4eac32343bf30bcf536a9b8411d940
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.7 MB (254676997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17e7291203f4ceb144558b61d792902b5a7320a780ea0b3f98de0fdfa868e47a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:21:12 GMT
ADD file:ae5c65eea20f7ddcf93a0aa255b6a08a906ac1a1a65cd2c4b5d1529bf9f6eaf8 in / 
# Tue, 19 Dec 2023 01:21:13 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:02:30 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 19 Dec 2023 02:02:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 02:03:10 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 19 Dec 2023 02:05:07 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:faac0b3889808c27af96e662a1082eef35772c35dcee1c7334f5f5a22b4149d7`  
		Last Modified: Tue, 19 Dec 2023 01:26:21 GMT  
		Size: 27.2 MB (27188221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9316d6ecf4d9ac6063dcc2781466cb9a8b78507bcb06a93963294c8e0c9840a`  
		Last Modified: Tue, 19 Dec 2023 02:11:01 GMT  
		Size: 2.8 MB (2781014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b6e0a2edd3ab1f5afa00ec7a0f6800cf95e79ed10115be03872814aa843752`  
		Last Modified: Tue, 19 Dec 2023 02:11:10 GMT  
		Size: 64.8 MB (64774640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ce8ee7410abd8de3b88f04973391b7d04baf4c65c4b6ba0c165bc051de22f9`  
		Last Modified: Tue, 19 Dec 2023 02:12:08 GMT  
		Size: 159.9 MB (159933122 bytes)  
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
$ docker pull mono@sha256:2592075e4bfe076daddbf021eb176ed18c83c3b57e827be89f81f1b4a80b399d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.0 MB (189019378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a53516a4dd4f7e5b653db5f989d90522b2d3e975f55417fee52a7596d12ef77`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 02:08:27 GMT
ADD file:24df0653e55efc5ba9ec22911758d187c26dbe6bda2d417ff56bc3d9a9072dd4 in / 
# Tue, 19 Dec 2023 02:08:27 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:35:05 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 19 Dec 2023 02:35:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 02:35:41 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 19 Dec 2023 02:37:34 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:99a10db9a1b078c63980e0e4fc7242bdb6d9ba7c91dd8e0883a55756584bea0f`  
		Last Modified: Tue, 19 Dec 2023 02:13:13 GMT  
		Size: 22.8 MB (22795803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3a3e904e68d35ee1e1d34ea1cac63c5011da52b9dabafcbb69468cd863ce5e`  
		Last Modified: Tue, 19 Dec 2023 02:40:07 GMT  
		Size: 2.4 MB (2370806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0bf50e7a2d398d44cc9c9dbdbaea5d96b90aed33dd8fd650e005295e14419dd`  
		Last Modified: Tue, 19 Dec 2023 02:40:12 GMT  
		Size: 23.8 MB (23790518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3feab922704c054c6bb93b29b588fa47af922eaf51b4c556ef14803944df8cc`  
		Last Modified: Tue, 19 Dec 2023 02:41:10 GMT  
		Size: 140.1 MB (140062251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:931a0b2f42bfe790d4e3fe8a2eced807dacf61419ed6c7d9918ce9f4c10e0610
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.4 MB (216408077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91698d8fd69cdd3b5b14611e736194d5553f50ddfe44553a2cefc5b468587a1b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:39 GMT
ADD file:f60673c303a98b4e4c676e3403bc1b7cb316335aba1202205188176810494c07 in / 
# Tue, 19 Dec 2023 01:41:40 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 07:45:01 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 19 Dec 2023 07:45:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 07:45:22 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 19 Dec 2023 07:46:37 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c0b0171eefd1c6d7f85c54d4a609269c9b5e19a0fd8cd787a49c808c6b73cf74`  
		Last Modified: Tue, 19 Dec 2023 01:46:01 GMT  
		Size: 26.0 MB (25969827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866041d2ba1a760a96ca9bf3322602594a35eb1312c1c3c40c5ae3078f61766e`  
		Last Modified: Tue, 19 Dec 2023 07:47:54 GMT  
		Size: 2.6 MB (2645863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfeb9226e7a30640d245f72ba1c26e2bcb224a880d0fddd8423a74d1fc4981e8`  
		Last Modified: Tue, 19 Dec 2023 07:47:58 GMT  
		Size: 29.5 MB (29545120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b5347da712f33dab552d0221a89bd94977f82b9c9583c5edf4d178a4cff373`  
		Last Modified: Tue, 19 Dec 2023 07:48:43 GMT  
		Size: 158.2 MB (158247267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12` - linux; 386

```console
$ docker pull mono@sha256:568f9b0d910d6c249c7717c6c9c953e5631dd3b00639e0514fbb57ea74d361ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.6 MB (259559822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4663b11a49195455a3b8eb22821e6095a32e9b96120305303316f5a2539c5f8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:39:52 GMT
ADD file:334e70a7f093f24a0d8e3b87a26edb95d1a12e2dc805ddbcf4e75e3e406803a0 in / 
# Tue, 19 Dec 2023 01:39:52 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:43:20 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 19 Dec 2023 03:43:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 03:44:00 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 19 Dec 2023 03:46:15 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:92f20691effe39d2fd17b271760acef5ac648490cb2e2d292d69ce7f39589f17`  
		Last Modified: Tue, 19 Dec 2023 01:45:18 GMT  
		Size: 27.8 MB (27846883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2eee6d230be6ff9e02dfcc5cf0c2007a1cb25419d0d505782510ff2edb870ac`  
		Last Modified: Tue, 19 Dec 2023 03:48:09 GMT  
		Size: 2.8 MB (2792509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4625069d528cf9adc60ffdd7ec17343c361d8cae5329590ef15dad49108594af`  
		Last Modified: Tue, 19 Dec 2023 03:48:24 GMT  
		Size: 68.8 MB (68800526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed1fe186dc5fb79d1535cfcfe78713b75fcafdd4966ac94bf453e4e792207964`  
		Last Modified: Tue, 19 Dec 2023 03:49:41 GMT  
		Size: 160.1 MB (160119904 bytes)  
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
$ docker pull mono@sha256:c1663267870224db329f049113b817370c9459dacc3f11434a2782c5981c7398
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
$ docker pull mono@sha256:5d9397aca3eaf3f6aa14ce7be85a5928ccbefe8553b91ab61949af68b39848eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94743875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd33b75bff8d671d09cf06d52ec2a5a40037113105e4897cdb8f78574918086b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:21:12 GMT
ADD file:ae5c65eea20f7ddcf93a0aa255b6a08a906ac1a1a65cd2c4b5d1529bf9f6eaf8 in / 
# Tue, 19 Dec 2023 01:21:13 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:02:30 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 19 Dec 2023 02:02:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 02:03:10 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:faac0b3889808c27af96e662a1082eef35772c35dcee1c7334f5f5a22b4149d7`  
		Last Modified: Tue, 19 Dec 2023 01:26:21 GMT  
		Size: 27.2 MB (27188221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9316d6ecf4d9ac6063dcc2781466cb9a8b78507bcb06a93963294c8e0c9840a`  
		Last Modified: Tue, 19 Dec 2023 02:11:01 GMT  
		Size: 2.8 MB (2781014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b6e0a2edd3ab1f5afa00ec7a0f6800cf95e79ed10115be03872814aa843752`  
		Last Modified: Tue, 19 Dec 2023 02:11:10 GMT  
		Size: 64.8 MB (64774640 bytes)  
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
$ docker pull mono@sha256:4cb0e804635c105dc75dd91df98fcf599bd882a9e6e082c8673f82b4ade79cfc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48957127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0ac45316a47d4e84353fea61fb7c0f000143904c4a545518f5caf1165ad95b5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 02:08:27 GMT
ADD file:24df0653e55efc5ba9ec22911758d187c26dbe6bda2d417ff56bc3d9a9072dd4 in / 
# Tue, 19 Dec 2023 02:08:27 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:35:05 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 19 Dec 2023 02:35:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 02:35:41 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:99a10db9a1b078c63980e0e4fc7242bdb6d9ba7c91dd8e0883a55756584bea0f`  
		Last Modified: Tue, 19 Dec 2023 02:13:13 GMT  
		Size: 22.8 MB (22795803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3a3e904e68d35ee1e1d34ea1cac63c5011da52b9dabafcbb69468cd863ce5e`  
		Last Modified: Tue, 19 Dec 2023 02:40:07 GMT  
		Size: 2.4 MB (2370806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0bf50e7a2d398d44cc9c9dbdbaea5d96b90aed33dd8fd650e005295e14419dd`  
		Last Modified: Tue, 19 Dec 2023 02:40:12 GMT  
		Size: 23.8 MB (23790518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:3bad9ad63df49a2d1bb2cb885ccdb13dd48df8902d0335dc2d4a499c8eee30f0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.2 MB (58160810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb659361160878c522d144fd8029d9d6f35aa9ee3f64ce39ad2cef260e741107`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:39 GMT
ADD file:f60673c303a98b4e4c676e3403bc1b7cb316335aba1202205188176810494c07 in / 
# Tue, 19 Dec 2023 01:41:40 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 07:45:01 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 19 Dec 2023 07:45:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 07:45:22 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c0b0171eefd1c6d7f85c54d4a609269c9b5e19a0fd8cd787a49c808c6b73cf74`  
		Last Modified: Tue, 19 Dec 2023 01:46:01 GMT  
		Size: 26.0 MB (25969827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866041d2ba1a760a96ca9bf3322602594a35eb1312c1c3c40c5ae3078f61766e`  
		Last Modified: Tue, 19 Dec 2023 07:47:54 GMT  
		Size: 2.6 MB (2645863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfeb9226e7a30640d245f72ba1c26e2bcb224a880d0fddd8423a74d1fc4981e8`  
		Last Modified: Tue, 19 Dec 2023 07:47:58 GMT  
		Size: 29.5 MB (29545120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12-slim` - linux; 386

```console
$ docker pull mono@sha256:e282710f806fb5b21e940f885dd799a58b43d1464523f86362e58804301bb37c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99439918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec32a3ab39c90a3290469d2be3ee88721bfb84fbbcfb5227498e42967b7cfdf2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:39:52 GMT
ADD file:334e70a7f093f24a0d8e3b87a26edb95d1a12e2dc805ddbcf4e75e3e406803a0 in / 
# Tue, 19 Dec 2023 01:39:52 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:43:20 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 19 Dec 2023 03:43:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 03:44:00 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:92f20691effe39d2fd17b271760acef5ac648490cb2e2d292d69ce7f39589f17`  
		Last Modified: Tue, 19 Dec 2023 01:45:18 GMT  
		Size: 27.8 MB (27846883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2eee6d230be6ff9e02dfcc5cf0c2007a1cb25419d0d505782510ff2edb870ac`  
		Last Modified: Tue, 19 Dec 2023 03:48:09 GMT  
		Size: 2.8 MB (2792509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4625069d528cf9adc60ffdd7ec17343c361d8cae5329590ef15dad49108594af`  
		Last Modified: Tue, 19 Dec 2023 03:48:24 GMT  
		Size: 68.8 MB (68800526 bytes)  
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
$ docker pull mono@sha256:29abff00ed65eac77557bdb52dca143d5e4670294ab69325b6cc7aa88dc26bd9
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
$ docker pull mono@sha256:246cbaec50ac5ada0821fec2574500aa9f4eac32343bf30bcf536a9b8411d940
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.7 MB (254676997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17e7291203f4ceb144558b61d792902b5a7320a780ea0b3f98de0fdfa868e47a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:21:12 GMT
ADD file:ae5c65eea20f7ddcf93a0aa255b6a08a906ac1a1a65cd2c4b5d1529bf9f6eaf8 in / 
# Tue, 19 Dec 2023 01:21:13 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:02:30 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 19 Dec 2023 02:02:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 02:03:10 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 19 Dec 2023 02:05:07 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:faac0b3889808c27af96e662a1082eef35772c35dcee1c7334f5f5a22b4149d7`  
		Last Modified: Tue, 19 Dec 2023 01:26:21 GMT  
		Size: 27.2 MB (27188221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9316d6ecf4d9ac6063dcc2781466cb9a8b78507bcb06a93963294c8e0c9840a`  
		Last Modified: Tue, 19 Dec 2023 02:11:01 GMT  
		Size: 2.8 MB (2781014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b6e0a2edd3ab1f5afa00ec7a0f6800cf95e79ed10115be03872814aa843752`  
		Last Modified: Tue, 19 Dec 2023 02:11:10 GMT  
		Size: 64.8 MB (64774640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ce8ee7410abd8de3b88f04973391b7d04baf4c65c4b6ba0c165bc051de22f9`  
		Last Modified: Tue, 19 Dec 2023 02:12:08 GMT  
		Size: 159.9 MB (159933122 bytes)  
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
$ docker pull mono@sha256:2592075e4bfe076daddbf021eb176ed18c83c3b57e827be89f81f1b4a80b399d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.0 MB (189019378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a53516a4dd4f7e5b653db5f989d90522b2d3e975f55417fee52a7596d12ef77`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 02:08:27 GMT
ADD file:24df0653e55efc5ba9ec22911758d187c26dbe6bda2d417ff56bc3d9a9072dd4 in / 
# Tue, 19 Dec 2023 02:08:27 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:35:05 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 19 Dec 2023 02:35:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 02:35:41 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 19 Dec 2023 02:37:34 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:99a10db9a1b078c63980e0e4fc7242bdb6d9ba7c91dd8e0883a55756584bea0f`  
		Last Modified: Tue, 19 Dec 2023 02:13:13 GMT  
		Size: 22.8 MB (22795803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3a3e904e68d35ee1e1d34ea1cac63c5011da52b9dabafcbb69468cd863ce5e`  
		Last Modified: Tue, 19 Dec 2023 02:40:07 GMT  
		Size: 2.4 MB (2370806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0bf50e7a2d398d44cc9c9dbdbaea5d96b90aed33dd8fd650e005295e14419dd`  
		Last Modified: Tue, 19 Dec 2023 02:40:12 GMT  
		Size: 23.8 MB (23790518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3feab922704c054c6bb93b29b588fa47af922eaf51b4c556ef14803944df8cc`  
		Last Modified: Tue, 19 Dec 2023 02:41:10 GMT  
		Size: 140.1 MB (140062251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:931a0b2f42bfe790d4e3fe8a2eced807dacf61419ed6c7d9918ce9f4c10e0610
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.4 MB (216408077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91698d8fd69cdd3b5b14611e736194d5553f50ddfe44553a2cefc5b468587a1b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:39 GMT
ADD file:f60673c303a98b4e4c676e3403bc1b7cb316335aba1202205188176810494c07 in / 
# Tue, 19 Dec 2023 01:41:40 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 07:45:01 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 19 Dec 2023 07:45:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 07:45:22 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 19 Dec 2023 07:46:37 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c0b0171eefd1c6d7f85c54d4a609269c9b5e19a0fd8cd787a49c808c6b73cf74`  
		Last Modified: Tue, 19 Dec 2023 01:46:01 GMT  
		Size: 26.0 MB (25969827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866041d2ba1a760a96ca9bf3322602594a35eb1312c1c3c40c5ae3078f61766e`  
		Last Modified: Tue, 19 Dec 2023 07:47:54 GMT  
		Size: 2.6 MB (2645863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfeb9226e7a30640d245f72ba1c26e2bcb224a880d0fddd8423a74d1fc4981e8`  
		Last Modified: Tue, 19 Dec 2023 07:47:58 GMT  
		Size: 29.5 MB (29545120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b5347da712f33dab552d0221a89bd94977f82b9c9583c5edf4d178a4cff373`  
		Last Modified: Tue, 19 Dec 2023 07:48:43 GMT  
		Size: 158.2 MB (158247267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0` - linux; 386

```console
$ docker pull mono@sha256:568f9b0d910d6c249c7717c6c9c953e5631dd3b00639e0514fbb57ea74d361ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.6 MB (259559822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4663b11a49195455a3b8eb22821e6095a32e9b96120305303316f5a2539c5f8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:39:52 GMT
ADD file:334e70a7f093f24a0d8e3b87a26edb95d1a12e2dc805ddbcf4e75e3e406803a0 in / 
# Tue, 19 Dec 2023 01:39:52 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:43:20 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 19 Dec 2023 03:43:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 03:44:00 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 19 Dec 2023 03:46:15 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:92f20691effe39d2fd17b271760acef5ac648490cb2e2d292d69ce7f39589f17`  
		Last Modified: Tue, 19 Dec 2023 01:45:18 GMT  
		Size: 27.8 MB (27846883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2eee6d230be6ff9e02dfcc5cf0c2007a1cb25419d0d505782510ff2edb870ac`  
		Last Modified: Tue, 19 Dec 2023 03:48:09 GMT  
		Size: 2.8 MB (2792509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4625069d528cf9adc60ffdd7ec17343c361d8cae5329590ef15dad49108594af`  
		Last Modified: Tue, 19 Dec 2023 03:48:24 GMT  
		Size: 68.8 MB (68800526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed1fe186dc5fb79d1535cfcfe78713b75fcafdd4966ac94bf453e4e792207964`  
		Last Modified: Tue, 19 Dec 2023 03:49:41 GMT  
		Size: 160.1 MB (160119904 bytes)  
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
$ docker pull mono@sha256:c1663267870224db329f049113b817370c9459dacc3f11434a2782c5981c7398
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
$ docker pull mono@sha256:5d9397aca3eaf3f6aa14ce7be85a5928ccbefe8553b91ab61949af68b39848eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94743875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd33b75bff8d671d09cf06d52ec2a5a40037113105e4897cdb8f78574918086b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:21:12 GMT
ADD file:ae5c65eea20f7ddcf93a0aa255b6a08a906ac1a1a65cd2c4b5d1529bf9f6eaf8 in / 
# Tue, 19 Dec 2023 01:21:13 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:02:30 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 19 Dec 2023 02:02:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 02:03:10 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:faac0b3889808c27af96e662a1082eef35772c35dcee1c7334f5f5a22b4149d7`  
		Last Modified: Tue, 19 Dec 2023 01:26:21 GMT  
		Size: 27.2 MB (27188221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9316d6ecf4d9ac6063dcc2781466cb9a8b78507bcb06a93963294c8e0c9840a`  
		Last Modified: Tue, 19 Dec 2023 02:11:01 GMT  
		Size: 2.8 MB (2781014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b6e0a2edd3ab1f5afa00ec7a0f6800cf95e79ed10115be03872814aa843752`  
		Last Modified: Tue, 19 Dec 2023 02:11:10 GMT  
		Size: 64.8 MB (64774640 bytes)  
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
$ docker pull mono@sha256:4cb0e804635c105dc75dd91df98fcf599bd882a9e6e082c8673f82b4ade79cfc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48957127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0ac45316a47d4e84353fea61fb7c0f000143904c4a545518f5caf1165ad95b5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 02:08:27 GMT
ADD file:24df0653e55efc5ba9ec22911758d187c26dbe6bda2d417ff56bc3d9a9072dd4 in / 
# Tue, 19 Dec 2023 02:08:27 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:35:05 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 19 Dec 2023 02:35:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 02:35:41 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:99a10db9a1b078c63980e0e4fc7242bdb6d9ba7c91dd8e0883a55756584bea0f`  
		Last Modified: Tue, 19 Dec 2023 02:13:13 GMT  
		Size: 22.8 MB (22795803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3a3e904e68d35ee1e1d34ea1cac63c5011da52b9dabafcbb69468cd863ce5e`  
		Last Modified: Tue, 19 Dec 2023 02:40:07 GMT  
		Size: 2.4 MB (2370806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0bf50e7a2d398d44cc9c9dbdbaea5d96b90aed33dd8fd650e005295e14419dd`  
		Last Modified: Tue, 19 Dec 2023 02:40:12 GMT  
		Size: 23.8 MB (23790518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:3bad9ad63df49a2d1bb2cb885ccdb13dd48df8902d0335dc2d4a499c8eee30f0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.2 MB (58160810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb659361160878c522d144fd8029d9d6f35aa9ee3f64ce39ad2cef260e741107`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:39 GMT
ADD file:f60673c303a98b4e4c676e3403bc1b7cb316335aba1202205188176810494c07 in / 
# Tue, 19 Dec 2023 01:41:40 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 07:45:01 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 19 Dec 2023 07:45:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 07:45:22 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c0b0171eefd1c6d7f85c54d4a609269c9b5e19a0fd8cd787a49c808c6b73cf74`  
		Last Modified: Tue, 19 Dec 2023 01:46:01 GMT  
		Size: 26.0 MB (25969827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866041d2ba1a760a96ca9bf3322602594a35eb1312c1c3c40c5ae3078f61766e`  
		Last Modified: Tue, 19 Dec 2023 07:47:54 GMT  
		Size: 2.6 MB (2645863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfeb9226e7a30640d245f72ba1c26e2bcb224a880d0fddd8423a74d1fc4981e8`  
		Last Modified: Tue, 19 Dec 2023 07:47:58 GMT  
		Size: 29.5 MB (29545120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0-slim` - linux; 386

```console
$ docker pull mono@sha256:e282710f806fb5b21e940f885dd799a58b43d1464523f86362e58804301bb37c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99439918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec32a3ab39c90a3290469d2be3ee88721bfb84fbbcfb5227498e42967b7cfdf2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:39:52 GMT
ADD file:334e70a7f093f24a0d8e3b87a26edb95d1a12e2dc805ddbcf4e75e3e406803a0 in / 
# Tue, 19 Dec 2023 01:39:52 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:43:20 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 19 Dec 2023 03:43:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 03:44:00 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:92f20691effe39d2fd17b271760acef5ac648490cb2e2d292d69ce7f39589f17`  
		Last Modified: Tue, 19 Dec 2023 01:45:18 GMT  
		Size: 27.8 MB (27846883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2eee6d230be6ff9e02dfcc5cf0c2007a1cb25419d0d505782510ff2edb870ac`  
		Last Modified: Tue, 19 Dec 2023 03:48:09 GMT  
		Size: 2.8 MB (2792509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4625069d528cf9adc60ffdd7ec17343c361d8cae5329590ef15dad49108594af`  
		Last Modified: Tue, 19 Dec 2023 03:48:24 GMT  
		Size: 68.8 MB (68800526 bytes)  
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
$ docker pull mono@sha256:29abff00ed65eac77557bdb52dca143d5e4670294ab69325b6cc7aa88dc26bd9
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
$ docker pull mono@sha256:246cbaec50ac5ada0821fec2574500aa9f4eac32343bf30bcf536a9b8411d940
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.7 MB (254676997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17e7291203f4ceb144558b61d792902b5a7320a780ea0b3f98de0fdfa868e47a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:21:12 GMT
ADD file:ae5c65eea20f7ddcf93a0aa255b6a08a906ac1a1a65cd2c4b5d1529bf9f6eaf8 in / 
# Tue, 19 Dec 2023 01:21:13 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:02:30 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 19 Dec 2023 02:02:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 02:03:10 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 19 Dec 2023 02:05:07 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:faac0b3889808c27af96e662a1082eef35772c35dcee1c7334f5f5a22b4149d7`  
		Last Modified: Tue, 19 Dec 2023 01:26:21 GMT  
		Size: 27.2 MB (27188221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9316d6ecf4d9ac6063dcc2781466cb9a8b78507bcb06a93963294c8e0c9840a`  
		Last Modified: Tue, 19 Dec 2023 02:11:01 GMT  
		Size: 2.8 MB (2781014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b6e0a2edd3ab1f5afa00ec7a0f6800cf95e79ed10115be03872814aa843752`  
		Last Modified: Tue, 19 Dec 2023 02:11:10 GMT  
		Size: 64.8 MB (64774640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ce8ee7410abd8de3b88f04973391b7d04baf4c65c4b6ba0c165bc051de22f9`  
		Last Modified: Tue, 19 Dec 2023 02:12:08 GMT  
		Size: 159.9 MB (159933122 bytes)  
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
$ docker pull mono@sha256:2592075e4bfe076daddbf021eb176ed18c83c3b57e827be89f81f1b4a80b399d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.0 MB (189019378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a53516a4dd4f7e5b653db5f989d90522b2d3e975f55417fee52a7596d12ef77`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 02:08:27 GMT
ADD file:24df0653e55efc5ba9ec22911758d187c26dbe6bda2d417ff56bc3d9a9072dd4 in / 
# Tue, 19 Dec 2023 02:08:27 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:35:05 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 19 Dec 2023 02:35:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 02:35:41 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 19 Dec 2023 02:37:34 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:99a10db9a1b078c63980e0e4fc7242bdb6d9ba7c91dd8e0883a55756584bea0f`  
		Last Modified: Tue, 19 Dec 2023 02:13:13 GMT  
		Size: 22.8 MB (22795803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3a3e904e68d35ee1e1d34ea1cac63c5011da52b9dabafcbb69468cd863ce5e`  
		Last Modified: Tue, 19 Dec 2023 02:40:07 GMT  
		Size: 2.4 MB (2370806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0bf50e7a2d398d44cc9c9dbdbaea5d96b90aed33dd8fd650e005295e14419dd`  
		Last Modified: Tue, 19 Dec 2023 02:40:12 GMT  
		Size: 23.8 MB (23790518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3feab922704c054c6bb93b29b588fa47af922eaf51b4c556ef14803944df8cc`  
		Last Modified: Tue, 19 Dec 2023 02:41:10 GMT  
		Size: 140.1 MB (140062251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.182` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:931a0b2f42bfe790d4e3fe8a2eced807dacf61419ed6c7d9918ce9f4c10e0610
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.4 MB (216408077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91698d8fd69cdd3b5b14611e736194d5553f50ddfe44553a2cefc5b468587a1b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:39 GMT
ADD file:f60673c303a98b4e4c676e3403bc1b7cb316335aba1202205188176810494c07 in / 
# Tue, 19 Dec 2023 01:41:40 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 07:45:01 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 19 Dec 2023 07:45:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 07:45:22 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 19 Dec 2023 07:46:37 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c0b0171eefd1c6d7f85c54d4a609269c9b5e19a0fd8cd787a49c808c6b73cf74`  
		Last Modified: Tue, 19 Dec 2023 01:46:01 GMT  
		Size: 26.0 MB (25969827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866041d2ba1a760a96ca9bf3322602594a35eb1312c1c3c40c5ae3078f61766e`  
		Last Modified: Tue, 19 Dec 2023 07:47:54 GMT  
		Size: 2.6 MB (2645863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfeb9226e7a30640d245f72ba1c26e2bcb224a880d0fddd8423a74d1fc4981e8`  
		Last Modified: Tue, 19 Dec 2023 07:47:58 GMT  
		Size: 29.5 MB (29545120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b5347da712f33dab552d0221a89bd94977f82b9c9583c5edf4d178a4cff373`  
		Last Modified: Tue, 19 Dec 2023 07:48:43 GMT  
		Size: 158.2 MB (158247267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.182` - linux; 386

```console
$ docker pull mono@sha256:568f9b0d910d6c249c7717c6c9c953e5631dd3b00639e0514fbb57ea74d361ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.6 MB (259559822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4663b11a49195455a3b8eb22821e6095a32e9b96120305303316f5a2539c5f8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:39:52 GMT
ADD file:334e70a7f093f24a0d8e3b87a26edb95d1a12e2dc805ddbcf4e75e3e406803a0 in / 
# Tue, 19 Dec 2023 01:39:52 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:43:20 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 19 Dec 2023 03:43:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 03:44:00 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 19 Dec 2023 03:46:15 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:92f20691effe39d2fd17b271760acef5ac648490cb2e2d292d69ce7f39589f17`  
		Last Modified: Tue, 19 Dec 2023 01:45:18 GMT  
		Size: 27.8 MB (27846883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2eee6d230be6ff9e02dfcc5cf0c2007a1cb25419d0d505782510ff2edb870ac`  
		Last Modified: Tue, 19 Dec 2023 03:48:09 GMT  
		Size: 2.8 MB (2792509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4625069d528cf9adc60ffdd7ec17343c361d8cae5329590ef15dad49108594af`  
		Last Modified: Tue, 19 Dec 2023 03:48:24 GMT  
		Size: 68.8 MB (68800526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed1fe186dc5fb79d1535cfcfe78713b75fcafdd4966ac94bf453e4e792207964`  
		Last Modified: Tue, 19 Dec 2023 03:49:41 GMT  
		Size: 160.1 MB (160119904 bytes)  
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
$ docker pull mono@sha256:c1663267870224db329f049113b817370c9459dacc3f11434a2782c5981c7398
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
$ docker pull mono@sha256:5d9397aca3eaf3f6aa14ce7be85a5928ccbefe8553b91ab61949af68b39848eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94743875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd33b75bff8d671d09cf06d52ec2a5a40037113105e4897cdb8f78574918086b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:21:12 GMT
ADD file:ae5c65eea20f7ddcf93a0aa255b6a08a906ac1a1a65cd2c4b5d1529bf9f6eaf8 in / 
# Tue, 19 Dec 2023 01:21:13 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:02:30 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 19 Dec 2023 02:02:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 02:03:10 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:faac0b3889808c27af96e662a1082eef35772c35dcee1c7334f5f5a22b4149d7`  
		Last Modified: Tue, 19 Dec 2023 01:26:21 GMT  
		Size: 27.2 MB (27188221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9316d6ecf4d9ac6063dcc2781466cb9a8b78507bcb06a93963294c8e0c9840a`  
		Last Modified: Tue, 19 Dec 2023 02:11:01 GMT  
		Size: 2.8 MB (2781014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b6e0a2edd3ab1f5afa00ec7a0f6800cf95e79ed10115be03872814aa843752`  
		Last Modified: Tue, 19 Dec 2023 02:11:10 GMT  
		Size: 64.8 MB (64774640 bytes)  
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
$ docker pull mono@sha256:4cb0e804635c105dc75dd91df98fcf599bd882a9e6e082c8673f82b4ade79cfc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48957127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0ac45316a47d4e84353fea61fb7c0f000143904c4a545518f5caf1165ad95b5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 02:08:27 GMT
ADD file:24df0653e55efc5ba9ec22911758d187c26dbe6bda2d417ff56bc3d9a9072dd4 in / 
# Tue, 19 Dec 2023 02:08:27 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:35:05 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 19 Dec 2023 02:35:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 02:35:41 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:99a10db9a1b078c63980e0e4fc7242bdb6d9ba7c91dd8e0883a55756584bea0f`  
		Last Modified: Tue, 19 Dec 2023 02:13:13 GMT  
		Size: 22.8 MB (22795803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3a3e904e68d35ee1e1d34ea1cac63c5011da52b9dabafcbb69468cd863ce5e`  
		Last Modified: Tue, 19 Dec 2023 02:40:07 GMT  
		Size: 2.4 MB (2370806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0bf50e7a2d398d44cc9c9dbdbaea5d96b90aed33dd8fd650e005295e14419dd`  
		Last Modified: Tue, 19 Dec 2023 02:40:12 GMT  
		Size: 23.8 MB (23790518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.182-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:3bad9ad63df49a2d1bb2cb885ccdb13dd48df8902d0335dc2d4a499c8eee30f0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.2 MB (58160810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb659361160878c522d144fd8029d9d6f35aa9ee3f64ce39ad2cef260e741107`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:39 GMT
ADD file:f60673c303a98b4e4c676e3403bc1b7cb316335aba1202205188176810494c07 in / 
# Tue, 19 Dec 2023 01:41:40 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 07:45:01 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 19 Dec 2023 07:45:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 07:45:22 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c0b0171eefd1c6d7f85c54d4a609269c9b5e19a0fd8cd787a49c808c6b73cf74`  
		Last Modified: Tue, 19 Dec 2023 01:46:01 GMT  
		Size: 26.0 MB (25969827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866041d2ba1a760a96ca9bf3322602594a35eb1312c1c3c40c5ae3078f61766e`  
		Last Modified: Tue, 19 Dec 2023 07:47:54 GMT  
		Size: 2.6 MB (2645863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfeb9226e7a30640d245f72ba1c26e2bcb224a880d0fddd8423a74d1fc4981e8`  
		Last Modified: Tue, 19 Dec 2023 07:47:58 GMT  
		Size: 29.5 MB (29545120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.182-slim` - linux; 386

```console
$ docker pull mono@sha256:e282710f806fb5b21e940f885dd799a58b43d1464523f86362e58804301bb37c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99439918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec32a3ab39c90a3290469d2be3ee88721bfb84fbbcfb5227498e42967b7cfdf2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:39:52 GMT
ADD file:334e70a7f093f24a0d8e3b87a26edb95d1a12e2dc805ddbcf4e75e3e406803a0 in / 
# Tue, 19 Dec 2023 01:39:52 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:43:20 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 19 Dec 2023 03:43:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 03:44:00 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:92f20691effe39d2fd17b271760acef5ac648490cb2e2d292d69ce7f39589f17`  
		Last Modified: Tue, 19 Dec 2023 01:45:18 GMT  
		Size: 27.8 MB (27846883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2eee6d230be6ff9e02dfcc5cf0c2007a1cb25419d0d505782510ff2edb870ac`  
		Last Modified: Tue, 19 Dec 2023 03:48:09 GMT  
		Size: 2.8 MB (2792509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4625069d528cf9adc60ffdd7ec17343c361d8cae5329590ef15dad49108594af`  
		Last Modified: Tue, 19 Dec 2023 03:48:24 GMT  
		Size: 68.8 MB (68800526 bytes)  
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
$ docker pull mono@sha256:29abff00ed65eac77557bdb52dca143d5e4670294ab69325b6cc7aa88dc26bd9
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
$ docker pull mono@sha256:246cbaec50ac5ada0821fec2574500aa9f4eac32343bf30bcf536a9b8411d940
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.7 MB (254676997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17e7291203f4ceb144558b61d792902b5a7320a780ea0b3f98de0fdfa868e47a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:21:12 GMT
ADD file:ae5c65eea20f7ddcf93a0aa255b6a08a906ac1a1a65cd2c4b5d1529bf9f6eaf8 in / 
# Tue, 19 Dec 2023 01:21:13 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:02:30 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 19 Dec 2023 02:02:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 02:03:10 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 19 Dec 2023 02:05:07 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:faac0b3889808c27af96e662a1082eef35772c35dcee1c7334f5f5a22b4149d7`  
		Last Modified: Tue, 19 Dec 2023 01:26:21 GMT  
		Size: 27.2 MB (27188221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9316d6ecf4d9ac6063dcc2781466cb9a8b78507bcb06a93963294c8e0c9840a`  
		Last Modified: Tue, 19 Dec 2023 02:11:01 GMT  
		Size: 2.8 MB (2781014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b6e0a2edd3ab1f5afa00ec7a0f6800cf95e79ed10115be03872814aa843752`  
		Last Modified: Tue, 19 Dec 2023 02:11:10 GMT  
		Size: 64.8 MB (64774640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ce8ee7410abd8de3b88f04973391b7d04baf4c65c4b6ba0c165bc051de22f9`  
		Last Modified: Tue, 19 Dec 2023 02:12:08 GMT  
		Size: 159.9 MB (159933122 bytes)  
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
$ docker pull mono@sha256:2592075e4bfe076daddbf021eb176ed18c83c3b57e827be89f81f1b4a80b399d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.0 MB (189019378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a53516a4dd4f7e5b653db5f989d90522b2d3e975f55417fee52a7596d12ef77`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 02:08:27 GMT
ADD file:24df0653e55efc5ba9ec22911758d187c26dbe6bda2d417ff56bc3d9a9072dd4 in / 
# Tue, 19 Dec 2023 02:08:27 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:35:05 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 19 Dec 2023 02:35:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 02:35:41 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 19 Dec 2023 02:37:34 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:99a10db9a1b078c63980e0e4fc7242bdb6d9ba7c91dd8e0883a55756584bea0f`  
		Last Modified: Tue, 19 Dec 2023 02:13:13 GMT  
		Size: 22.8 MB (22795803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3a3e904e68d35ee1e1d34ea1cac63c5011da52b9dabafcbb69468cd863ce5e`  
		Last Modified: Tue, 19 Dec 2023 02:40:07 GMT  
		Size: 2.4 MB (2370806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0bf50e7a2d398d44cc9c9dbdbaea5d96b90aed33dd8fd650e005295e14419dd`  
		Last Modified: Tue, 19 Dec 2023 02:40:12 GMT  
		Size: 23.8 MB (23790518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3feab922704c054c6bb93b29b588fa47af922eaf51b4c556ef14803944df8cc`  
		Last Modified: Tue, 19 Dec 2023 02:41:10 GMT  
		Size: 140.1 MB (140062251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:931a0b2f42bfe790d4e3fe8a2eced807dacf61419ed6c7d9918ce9f4c10e0610
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.4 MB (216408077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91698d8fd69cdd3b5b14611e736194d5553f50ddfe44553a2cefc5b468587a1b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:39 GMT
ADD file:f60673c303a98b4e4c676e3403bc1b7cb316335aba1202205188176810494c07 in / 
# Tue, 19 Dec 2023 01:41:40 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 07:45:01 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 19 Dec 2023 07:45:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 07:45:22 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 19 Dec 2023 07:46:37 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c0b0171eefd1c6d7f85c54d4a609269c9b5e19a0fd8cd787a49c808c6b73cf74`  
		Last Modified: Tue, 19 Dec 2023 01:46:01 GMT  
		Size: 26.0 MB (25969827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866041d2ba1a760a96ca9bf3322602594a35eb1312c1c3c40c5ae3078f61766e`  
		Last Modified: Tue, 19 Dec 2023 07:47:54 GMT  
		Size: 2.6 MB (2645863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfeb9226e7a30640d245f72ba1c26e2bcb224a880d0fddd8423a74d1fc4981e8`  
		Last Modified: Tue, 19 Dec 2023 07:47:58 GMT  
		Size: 29.5 MB (29545120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b5347da712f33dab552d0221a89bd94977f82b9c9583c5edf4d178a4cff373`  
		Last Modified: Tue, 19 Dec 2023 07:48:43 GMT  
		Size: 158.2 MB (158247267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; 386

```console
$ docker pull mono@sha256:568f9b0d910d6c249c7717c6c9c953e5631dd3b00639e0514fbb57ea74d361ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.6 MB (259559822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4663b11a49195455a3b8eb22821e6095a32e9b96120305303316f5a2539c5f8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:39:52 GMT
ADD file:334e70a7f093f24a0d8e3b87a26edb95d1a12e2dc805ddbcf4e75e3e406803a0 in / 
# Tue, 19 Dec 2023 01:39:52 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:43:20 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 19 Dec 2023 03:43:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 03:44:00 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 19 Dec 2023 03:46:15 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:92f20691effe39d2fd17b271760acef5ac648490cb2e2d292d69ce7f39589f17`  
		Last Modified: Tue, 19 Dec 2023 01:45:18 GMT  
		Size: 27.8 MB (27846883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2eee6d230be6ff9e02dfcc5cf0c2007a1cb25419d0d505782510ff2edb870ac`  
		Last Modified: Tue, 19 Dec 2023 03:48:09 GMT  
		Size: 2.8 MB (2792509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4625069d528cf9adc60ffdd7ec17343c361d8cae5329590ef15dad49108594af`  
		Last Modified: Tue, 19 Dec 2023 03:48:24 GMT  
		Size: 68.8 MB (68800526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed1fe186dc5fb79d1535cfcfe78713b75fcafdd4966ac94bf453e4e792207964`  
		Last Modified: Tue, 19 Dec 2023 03:49:41 GMT  
		Size: 160.1 MB (160119904 bytes)  
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
$ docker pull mono@sha256:c1663267870224db329f049113b817370c9459dacc3f11434a2782c5981c7398
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
$ docker pull mono@sha256:5d9397aca3eaf3f6aa14ce7be85a5928ccbefe8553b91ab61949af68b39848eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94743875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd33b75bff8d671d09cf06d52ec2a5a40037113105e4897cdb8f78574918086b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:21:12 GMT
ADD file:ae5c65eea20f7ddcf93a0aa255b6a08a906ac1a1a65cd2c4b5d1529bf9f6eaf8 in / 
# Tue, 19 Dec 2023 01:21:13 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:02:30 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 19 Dec 2023 02:02:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 02:03:10 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:faac0b3889808c27af96e662a1082eef35772c35dcee1c7334f5f5a22b4149d7`  
		Last Modified: Tue, 19 Dec 2023 01:26:21 GMT  
		Size: 27.2 MB (27188221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9316d6ecf4d9ac6063dcc2781466cb9a8b78507bcb06a93963294c8e0c9840a`  
		Last Modified: Tue, 19 Dec 2023 02:11:01 GMT  
		Size: 2.8 MB (2781014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b6e0a2edd3ab1f5afa00ec7a0f6800cf95e79ed10115be03872814aa843752`  
		Last Modified: Tue, 19 Dec 2023 02:11:10 GMT  
		Size: 64.8 MB (64774640 bytes)  
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
$ docker pull mono@sha256:4cb0e804635c105dc75dd91df98fcf599bd882a9e6e082c8673f82b4ade79cfc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48957127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0ac45316a47d4e84353fea61fb7c0f000143904c4a545518f5caf1165ad95b5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 02:08:27 GMT
ADD file:24df0653e55efc5ba9ec22911758d187c26dbe6bda2d417ff56bc3d9a9072dd4 in / 
# Tue, 19 Dec 2023 02:08:27 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:35:05 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 19 Dec 2023 02:35:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 02:35:41 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:99a10db9a1b078c63980e0e4fc7242bdb6d9ba7c91dd8e0883a55756584bea0f`  
		Last Modified: Tue, 19 Dec 2023 02:13:13 GMT  
		Size: 22.8 MB (22795803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3a3e904e68d35ee1e1d34ea1cac63c5011da52b9dabafcbb69468cd863ce5e`  
		Last Modified: Tue, 19 Dec 2023 02:40:07 GMT  
		Size: 2.4 MB (2370806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0bf50e7a2d398d44cc9c9dbdbaea5d96b90aed33dd8fd650e005295e14419dd`  
		Last Modified: Tue, 19 Dec 2023 02:40:12 GMT  
		Size: 23.8 MB (23790518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:3bad9ad63df49a2d1bb2cb885ccdb13dd48df8902d0335dc2d4a499c8eee30f0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.2 MB (58160810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb659361160878c522d144fd8029d9d6f35aa9ee3f64ce39ad2cef260e741107`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:39 GMT
ADD file:f60673c303a98b4e4c676e3403bc1b7cb316335aba1202205188176810494c07 in / 
# Tue, 19 Dec 2023 01:41:40 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 07:45:01 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 19 Dec 2023 07:45:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 07:45:22 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c0b0171eefd1c6d7f85c54d4a609269c9b5e19a0fd8cd787a49c808c6b73cf74`  
		Last Modified: Tue, 19 Dec 2023 01:46:01 GMT  
		Size: 26.0 MB (25969827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866041d2ba1a760a96ca9bf3322602594a35eb1312c1c3c40c5ae3078f61766e`  
		Last Modified: Tue, 19 Dec 2023 07:47:54 GMT  
		Size: 2.6 MB (2645863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfeb9226e7a30640d245f72ba1c26e2bcb224a880d0fddd8423a74d1fc4981e8`  
		Last Modified: Tue, 19 Dec 2023 07:47:58 GMT  
		Size: 29.5 MB (29545120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; 386

```console
$ docker pull mono@sha256:e282710f806fb5b21e940f885dd799a58b43d1464523f86362e58804301bb37c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99439918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec32a3ab39c90a3290469d2be3ee88721bfb84fbbcfb5227498e42967b7cfdf2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:39:52 GMT
ADD file:334e70a7f093f24a0d8e3b87a26edb95d1a12e2dc805ddbcf4e75e3e406803a0 in / 
# Tue, 19 Dec 2023 01:39:52 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:43:20 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 19 Dec 2023 03:43:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 19 Dec 2023 03:44:00 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:92f20691effe39d2fd17b271760acef5ac648490cb2e2d292d69ce7f39589f17`  
		Last Modified: Tue, 19 Dec 2023 01:45:18 GMT  
		Size: 27.8 MB (27846883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2eee6d230be6ff9e02dfcc5cf0c2007a1cb25419d0d505782510ff2edb870ac`  
		Last Modified: Tue, 19 Dec 2023 03:48:09 GMT  
		Size: 2.8 MB (2792509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4625069d528cf9adc60ffdd7ec17343c361d8cae5329590ef15dad49108594af`  
		Last Modified: Tue, 19 Dec 2023 03:48:24 GMT  
		Size: 68.8 MB (68800526 bytes)  
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
