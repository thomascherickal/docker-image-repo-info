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
$ docker pull mono@sha256:465112ebaf92fd33d9560a26e74848a07d18046f50f9c025d3837681f026d172
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
$ docker pull mono@sha256:089c69437f670a34d6d2faa7d15e29f3395a354b8ff3073598e76279cb9ba5d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.7 MB (254674329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f97afc4690efd1650c1d74e46a929a04e32f8d6c731f5958d15ef41826db0f4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:35 GMT
ADD file:9c8b7c79fbbb19d308d151785d178e19bfa7b83257f38d03fa7f30cd41d58530 in / 
# Thu, 07 Sep 2023 00:21:35 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:53:20 GMT
ENV MONO_VERSION=6.12.0.182
# Thu, 07 Sep 2023 01:53:30 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 01:53:54 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 07 Sep 2023 01:55:46 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:91f01557fe0da558070d4f24631c94e91a80877a24621b52b8b13009b62d8d96`  
		Last Modified: Thu, 07 Sep 2023 00:26:44 GMT  
		Size: 27.2 MB (27187385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12132fc81fdf72f5e5905edc96ba6db064fb390345d3f9c4a04b0aa7ff243e17`  
		Last Modified: Thu, 07 Sep 2023 02:01:44 GMT  
		Size: 2.8 MB (2780987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa4cf5e71acb35ad398b3bdf0cb7e63ba3591f8b633a45b2de4cd67d205f009`  
		Last Modified: Thu, 07 Sep 2023 02:01:53 GMT  
		Size: 64.8 MB (64774202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3bf7c27d69e706c535fab335198d46ba19e96cfe916e4116406ad5e1783746c`  
		Last Modified: Thu, 07 Sep 2023 02:02:51 GMT  
		Size: 159.9 MB (159931755 bytes)  
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
$ docker pull mono@sha256:3f2c50251c47c6e8daf7af30af91621870ae8d4bfed30819f452eac8026bbc53
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.0 MB (189021480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a2e8c2751e838c4f926991046e298b87181672c53a47b727e2749fcf1b8f8bb`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:58:32 GMT
ADD file:fa060a900723a2fce017a38b08be3eb2c27d4768d40c61cd1f6292a7f28a8bdc in / 
# Thu, 07 Sep 2023 00:58:33 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 04:03:37 GMT
ENV MONO_VERSION=6.12.0.182
# Thu, 07 Sep 2023 04:03:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 04:04:15 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 07 Sep 2023 04:07:12 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7e54f06c680feaf82a31a34e7453d765f332f671cfecacb622c3046561dcc572`  
		Last Modified: Thu, 07 Sep 2023 01:03:53 GMT  
		Size: 22.8 MB (22795752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896cf2b79eb9e448095cab03cb5968875cc5fb527a67d79649025441961efd82`  
		Last Modified: Thu, 07 Sep 2023 04:09:43 GMT  
		Size: 2.4 MB (2370781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a2303b2c37a5342143c8d7bceadf10352b40615dd417f3b04a47a83cde7b61`  
		Last Modified: Thu, 07 Sep 2023 04:09:47 GMT  
		Size: 23.8 MB (23791111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ef087b8af56f6ad24f17f51ab214d3d95a09c5048d36d54b9d3baa3c3ee8c7`  
		Last Modified: Thu, 07 Sep 2023 04:10:40 GMT  
		Size: 140.1 MB (140063836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:85439cb4fbff445b7a7a5c9857be3eb18a25f0c00ab310ca7597931b9f3357bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.4 MB (216404975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99b3fc85c61b2f9fefe7369de60ce845f2863ba714bb8aef6ff5d23a056af68e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:08 GMT
ADD file:3521159cdea23e107a3e194ebc9b8f9a6a37ea8188236a267b6ec26e87cf498a in / 
# Thu, 07 Sep 2023 00:40:08 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 07:04:02 GMT
ENV MONO_VERSION=6.12.0.182
# Thu, 07 Sep 2023 07:04:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 07:04:31 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 07 Sep 2023 07:06:47 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d7cc66d62b738dea27e341b7322194f45ab1be2e548fe11d8ad953d9d56caaa8`  
		Last Modified: Thu, 07 Sep 2023 00:44:18 GMT  
		Size: 26.0 MB (25967748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53037d9952d0efe71a5774348f92d173432e8dbdf95ceb18450c7c07c6c9e9f`  
		Last Modified: Thu, 07 Sep 2023 07:08:07 GMT  
		Size: 2.6 MB (2645888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f85155c32dab21f86975a13ba62dbc5410813df3fcafba56051eec44247a61`  
		Last Modified: Thu, 07 Sep 2023 07:08:10 GMT  
		Size: 29.5 MB (29545041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54bf7f84fb7a3b3125859753112a10e4bb673ae6d6ee00e235ac568ca6a4d15f`  
		Last Modified: Thu, 07 Sep 2023 07:08:58 GMT  
		Size: 158.2 MB (158246298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; 386

```console
$ docker pull mono@sha256:d914db5bbe9949453c7c8cdb8ef643d53db6a920a0d2f341a8ba6c5119117000
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.6 MB (259560153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1750b1ccddddd0725b37eccca344d9e8b827165b132275486ab1908759b2b4ca`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:46 GMT
ADD file:e5916da683bdcea27e31e6fbb29e61d1f8457a3bebe4a83278e4f0181e5ac49f in / 
# Thu, 07 Sep 2023 00:39:47 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 20:02:37 GMT
ENV MONO_VERSION=6.12.0.182
# Thu, 07 Sep 2023 20:02:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 20:03:19 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 07 Sep 2023 20:05:40 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:453c610c7d8be388b9a8559dc654a2def01e71f776e0608ae46db51ae50d10a0`  
		Last Modified: Thu, 07 Sep 2023 00:45:26 GMT  
		Size: 27.8 MB (27846798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d6396be6afdd9df4ac1ad90d0ab9aaef68b9759a6d4ec028aa8c4963970ca3`  
		Last Modified: Thu, 07 Sep 2023 20:07:31 GMT  
		Size: 2.8 MB (2792479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58c12dba60a13a57b5648614b665be3d02ce9e747541083ab284b2a34873e6c`  
		Last Modified: Thu, 07 Sep 2023 20:07:45 GMT  
		Size: 68.8 MB (68800678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45574f7922a18c136182a845a84aa83dbaa55b270403803504630217c6dc1223`  
		Last Modified: Thu, 07 Sep 2023 20:09:11 GMT  
		Size: 160.1 MB (160120198 bytes)  
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
$ docker pull mono@sha256:4ac0e6a9361a55b14456a63130b931ea563ab6281f8bede836d29892544554b8
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
$ docker pull mono@sha256:84cc79f2e8be438c04f8eade849b8757727be784faca8efa67f7e1c38ea24633
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94742574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdb686b94af3d0fe092a2df584b75557331d28d1de5050abbd456bba31475781`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:35 GMT
ADD file:9c8b7c79fbbb19d308d151785d178e19bfa7b83257f38d03fa7f30cd41d58530 in / 
# Thu, 07 Sep 2023 00:21:35 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:53:20 GMT
ENV MONO_VERSION=6.12.0.182
# Thu, 07 Sep 2023 01:53:30 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 01:53:54 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:91f01557fe0da558070d4f24631c94e91a80877a24621b52b8b13009b62d8d96`  
		Last Modified: Thu, 07 Sep 2023 00:26:44 GMT  
		Size: 27.2 MB (27187385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12132fc81fdf72f5e5905edc96ba6db064fb390345d3f9c4a04b0aa7ff243e17`  
		Last Modified: Thu, 07 Sep 2023 02:01:44 GMT  
		Size: 2.8 MB (2780987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa4cf5e71acb35ad398b3bdf0cb7e63ba3591f8b633a45b2de4cd67d205f009`  
		Last Modified: Thu, 07 Sep 2023 02:01:53 GMT  
		Size: 64.8 MB (64774202 bytes)  
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
$ docker pull mono@sha256:f92793d95509dc30e2d40b85171aece1c5a1aff00d70062e9e2fc646b1a7ead0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48957644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b101a66aff317c6451bacbe4d8db8760c98060d12d5bc238f97322dc5cd418f7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:58:32 GMT
ADD file:fa060a900723a2fce017a38b08be3eb2c27d4768d40c61cd1f6292a7f28a8bdc in / 
# Thu, 07 Sep 2023 00:58:33 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 04:03:37 GMT
ENV MONO_VERSION=6.12.0.182
# Thu, 07 Sep 2023 04:03:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 04:04:15 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7e54f06c680feaf82a31a34e7453d765f332f671cfecacb622c3046561dcc572`  
		Last Modified: Thu, 07 Sep 2023 01:03:53 GMT  
		Size: 22.8 MB (22795752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896cf2b79eb9e448095cab03cb5968875cc5fb527a67d79649025441961efd82`  
		Last Modified: Thu, 07 Sep 2023 04:09:43 GMT  
		Size: 2.4 MB (2370781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a2303b2c37a5342143c8d7bceadf10352b40615dd417f3b04a47a83cde7b61`  
		Last Modified: Thu, 07 Sep 2023 04:09:47 GMT  
		Size: 23.8 MB (23791111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:6a13402decdc835e814b8a9d08ca232a924b5a436a6e1aceb23980ea7cc0d770
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.2 MB (58158677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1633b0a05c1e8711d19da02dc723dffbef9d8e4d6f7f07b39eb54d46b8d2df0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:08 GMT
ADD file:3521159cdea23e107a3e194ebc9b8f9a6a37ea8188236a267b6ec26e87cf498a in / 
# Thu, 07 Sep 2023 00:40:08 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 07:04:02 GMT
ENV MONO_VERSION=6.12.0.182
# Thu, 07 Sep 2023 07:04:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 07:04:31 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d7cc66d62b738dea27e341b7322194f45ab1be2e548fe11d8ad953d9d56caaa8`  
		Last Modified: Thu, 07 Sep 2023 00:44:18 GMT  
		Size: 26.0 MB (25967748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53037d9952d0efe71a5774348f92d173432e8dbdf95ceb18450c7c07c6c9e9f`  
		Last Modified: Thu, 07 Sep 2023 07:08:07 GMT  
		Size: 2.6 MB (2645888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f85155c32dab21f86975a13ba62dbc5410813df3fcafba56051eec44247a61`  
		Last Modified: Thu, 07 Sep 2023 07:08:10 GMT  
		Size: 29.5 MB (29545041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; 386

```console
$ docker pull mono@sha256:1e331750b2de2f768b2b3359c5cb5ff9d777f02907ae9f9610d1c7bd86c29385
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99439955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dde61adb84e6642ed59730f8251c19a89212a3b608e7905770466bf8ad8b3a45`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:46 GMT
ADD file:e5916da683bdcea27e31e6fbb29e61d1f8457a3bebe4a83278e4f0181e5ac49f in / 
# Thu, 07 Sep 2023 00:39:47 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 20:02:37 GMT
ENV MONO_VERSION=6.12.0.182
# Thu, 07 Sep 2023 20:02:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 20:03:19 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:453c610c7d8be388b9a8559dc654a2def01e71f776e0608ae46db51ae50d10a0`  
		Last Modified: Thu, 07 Sep 2023 00:45:26 GMT  
		Size: 27.8 MB (27846798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d6396be6afdd9df4ac1ad90d0ab9aaef68b9759a6d4ec028aa8c4963970ca3`  
		Last Modified: Thu, 07 Sep 2023 20:07:31 GMT  
		Size: 2.8 MB (2792479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58c12dba60a13a57b5648614b665be3d02ce9e747541083ab284b2a34873e6c`  
		Last Modified: Thu, 07 Sep 2023 20:07:45 GMT  
		Size: 68.8 MB (68800678 bytes)  
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
$ docker pull mono@sha256:a50ed72d1e926e69f254583815ec6f9e1477d384ad172994b1f5fba8cc1e863c
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
$ docker pull mono@sha256:c81d20ab3c2cfa34908994640e4d54bb8785e74010828e7cc020085224d45d7a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.1 MB (225071705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39a523f59310718cb5b5c20bfe19390093eb45b349c200dc8ec03ffffb9d92d4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:35 GMT
ADD file:9c8b7c79fbbb19d308d151785d178e19bfa7b83257f38d03fa7f30cd41d58530 in / 
# Thu, 07 Sep 2023 00:21:35 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:54:01 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 07 Sep 2023 01:54:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 01:54:38 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 07 Sep 2023 02:01:13 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:91f01557fe0da558070d4f24631c94e91a80877a24621b52b8b13009b62d8d96`  
		Last Modified: Thu, 07 Sep 2023 00:26:44 GMT  
		Size: 27.2 MB (27187385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc5d89a2c6ca09bf688d79ac5db4246fdefa27e5e615596e38d98a3d7004085`  
		Last Modified: Thu, 07 Sep 2023 02:02:09 GMT  
		Size: 2.8 MB (2780979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b2e5ea4b1f22e2732556eaaffe5b7a63ff534cbb8bc4c7f4bfa0ef7a4006c8`  
		Last Modified: Thu, 07 Sep 2023 02:02:18 GMT  
		Size: 64.8 MB (64780737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00cd284208b62e734ff0717a5633b34ad6ab7c75ce996c806d44d0dfd7442174`  
		Last Modified: Thu, 07 Sep 2023 02:03:23 GMT  
		Size: 130.3 MB (130322604 bytes)  
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
$ docker pull mono@sha256:585d4b784434eaac45129926e950b9e54f50959656696a701a9e350e23563b23
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.8 MB (176819763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e02cb6480ffc6e1d91d3de5ebdb1211a64aa76f58e3050ac7b1926128b4ad5cc`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:58:32 GMT
ADD file:fa060a900723a2fce017a38b08be3eb2c27d4768d40c61cd1f6292a7f28a8bdc in / 
# Thu, 07 Sep 2023 00:58:33 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 04:04:24 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 07 Sep 2023 04:04:37 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 04:05:03 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 07 Sep 2023 04:09:14 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7e54f06c680feaf82a31a34e7453d765f332f671cfecacb622c3046561dcc572`  
		Last Modified: Thu, 07 Sep 2023 01:03:53 GMT  
		Size: 22.8 MB (22795752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa71da295adc94cd16f1b3e01841dcdddb62864fc9db081db98e9e2af5edd0ab`  
		Last Modified: Thu, 07 Sep 2023 04:10:01 GMT  
		Size: 2.4 MB (2370843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4357100575ec4e026c17ea214d62ab407b12a41766650a2286dc66f725d4b3`  
		Last Modified: Thu, 07 Sep 2023 04:10:05 GMT  
		Size: 23.8 MB (23816244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1990aeeabed38bc3b4ea26c80cb6199198960c34f7493b7f5de84433338dc3e`  
		Last Modified: Thu, 07 Sep 2023 04:11:17 GMT  
		Size: 127.8 MB (127836924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:aa8f522fc82cc03531069007821d86482f435372ce9166c8f42717faa57217e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.7 MB (203679473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3e7cd60933858135626c238424e3e14c7c76512cf8ec355002765003a5e90bd`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:08 GMT
ADD file:3521159cdea23e107a3e194ebc9b8f9a6a37ea8188236a267b6ec26e87cf498a in / 
# Thu, 07 Sep 2023 00:40:08 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 07:04:36 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 07 Sep 2023 07:04:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 07:04:59 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 07 Sep 2023 07:07:48 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d7cc66d62b738dea27e341b7322194f45ab1be2e548fe11d8ad953d9d56caaa8`  
		Last Modified: Thu, 07 Sep 2023 00:44:18 GMT  
		Size: 26.0 MB (25967748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1595a1cccc3b44c5745fc712d26904327dbd3ff8e753c8300d1787f754b3c7`  
		Last Modified: Thu, 07 Sep 2023 07:08:25 GMT  
		Size: 2.6 MB (2645837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e254e11541fd91f2cbf884ccc172b5bf85091f11525af10efbb731b988a7ea`  
		Last Modified: Thu, 07 Sep 2023 07:08:29 GMT  
		Size: 29.6 MB (29575307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d350ab45b73413a3bed763e99f41182dc4457ff9e748a4c552c3a6758e0c71`  
		Last Modified: Thu, 07 Sep 2023 07:09:30 GMT  
		Size: 145.5 MB (145490581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; 386

```console
$ docker pull mono@sha256:d7f5051a9ffffbe7ba1492d5b5d90f0fb2534215e24d6cfe6953e3b8ef507867
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.9 MB (230912227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94159b274f52570585dd17d2fd66b0d304e28e8b3dcfeac09e57a040eecb243b`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:46 GMT
ADD file:e5916da683bdcea27e31e6fbb29e61d1f8457a3bebe4a83278e4f0181e5ac49f in / 
# Thu, 07 Sep 2023 00:39:47 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 20:03:26 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 07 Sep 2023 20:03:37 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 20:04:07 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 07 Sep 2023 20:07:04 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:453c610c7d8be388b9a8559dc654a2def01e71f776e0608ae46db51ae50d10a0`  
		Last Modified: Thu, 07 Sep 2023 00:45:26 GMT  
		Size: 27.8 MB (27846798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49a411b92496b09252a7bc9307636e321a65e7e5b69404cf4963dde5e312918`  
		Last Modified: Thu, 07 Sep 2023 20:08:09 GMT  
		Size: 2.8 MB (2792494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72f421756be6061e4ef3c6d514f4a5de79f29d240754f90387065ffd7af38a0`  
		Last Modified: Thu, 07 Sep 2023 20:08:24 GMT  
		Size: 68.8 MB (68810224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8bdd28cc5ec0fd10f08b7d982e6281078eb0c901145eb3697527cc03d4bb0f`  
		Last Modified: Thu, 07 Sep 2023 20:09:56 GMT  
		Size: 131.5 MB (131462711 bytes)  
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
$ docker pull mono@sha256:10ad89d7a60030a8f6f18d20f15efaa00f20b2d57877f7cf33445b5101680fb8
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
$ docker pull mono@sha256:4ad616f20a88b6db041b9b527ba05c57edfc1d59fe38be506ca6d6cda41c6e36
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94749101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7dbc470c7bfc374f3693ac0dce9c5bbcd8b7316e25a7037affdea1aa126b989`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:35 GMT
ADD file:9c8b7c79fbbb19d308d151785d178e19bfa7b83257f38d03fa7f30cd41d58530 in / 
# Thu, 07 Sep 2023 00:21:35 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:54:01 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 07 Sep 2023 01:54:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 01:54:38 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:91f01557fe0da558070d4f24631c94e91a80877a24621b52b8b13009b62d8d96`  
		Last Modified: Thu, 07 Sep 2023 00:26:44 GMT  
		Size: 27.2 MB (27187385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc5d89a2c6ca09bf688d79ac5db4246fdefa27e5e615596e38d98a3d7004085`  
		Last Modified: Thu, 07 Sep 2023 02:02:09 GMT  
		Size: 2.8 MB (2780979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b2e5ea4b1f22e2732556eaaffe5b7a63ff534cbb8bc4c7f4bfa0ef7a4006c8`  
		Last Modified: Thu, 07 Sep 2023 02:02:18 GMT  
		Size: 64.8 MB (64780737 bytes)  
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
$ docker pull mono@sha256:8a53e999e0d3f853d39cfee9d3b50044952aa86e2c3a644e2bcd5959d54736da
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48982839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dd3702c7d1ecb59e85a74d0d88b40f468b8f0c63aad29827499a35159022d24`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:58:32 GMT
ADD file:fa060a900723a2fce017a38b08be3eb2c27d4768d40c61cd1f6292a7f28a8bdc in / 
# Thu, 07 Sep 2023 00:58:33 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 04:04:24 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 07 Sep 2023 04:04:37 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 04:05:03 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7e54f06c680feaf82a31a34e7453d765f332f671cfecacb622c3046561dcc572`  
		Last Modified: Thu, 07 Sep 2023 01:03:53 GMT  
		Size: 22.8 MB (22795752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa71da295adc94cd16f1b3e01841dcdddb62864fc9db081db98e9e2af5edd0ab`  
		Last Modified: Thu, 07 Sep 2023 04:10:01 GMT  
		Size: 2.4 MB (2370843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4357100575ec4e026c17ea214d62ab407b12a41766650a2286dc66f725d4b3`  
		Last Modified: Thu, 07 Sep 2023 04:10:05 GMT  
		Size: 23.8 MB (23816244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:3cbbba9bce7f3997ad3096fd27bc1a267670dae18a75d224b0d43f305c255339
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.2 MB (58188892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81355dd1459418e965f6e723af0bf0e17fce76ac8b740d9db11846b6f174a87a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:08 GMT
ADD file:3521159cdea23e107a3e194ebc9b8f9a6a37ea8188236a267b6ec26e87cf498a in / 
# Thu, 07 Sep 2023 00:40:08 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 07:04:36 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 07 Sep 2023 07:04:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 07:04:59 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d7cc66d62b738dea27e341b7322194f45ab1be2e548fe11d8ad953d9d56caaa8`  
		Last Modified: Thu, 07 Sep 2023 00:44:18 GMT  
		Size: 26.0 MB (25967748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1595a1cccc3b44c5745fc712d26904327dbd3ff8e753c8300d1787f754b3c7`  
		Last Modified: Thu, 07 Sep 2023 07:08:25 GMT  
		Size: 2.6 MB (2645837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e254e11541fd91f2cbf884ccc172b5bf85091f11525af10efbb731b988a7ea`  
		Last Modified: Thu, 07 Sep 2023 07:08:29 GMT  
		Size: 29.6 MB (29575307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; 386

```console
$ docker pull mono@sha256:8ca2a0a252b5f280b301bdec97fcc0c2401ce3ff9dc936226b9fc152157af416
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99449516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1982032d75d0f0362ac653f5f8a88b8adbb56475ac1cdd86db81ffbaa3e0893`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:46 GMT
ADD file:e5916da683bdcea27e31e6fbb29e61d1f8457a3bebe4a83278e4f0181e5ac49f in / 
# Thu, 07 Sep 2023 00:39:47 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 20:03:26 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 07 Sep 2023 20:03:37 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 20:04:07 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:453c610c7d8be388b9a8559dc654a2def01e71f776e0608ae46db51ae50d10a0`  
		Last Modified: Thu, 07 Sep 2023 00:45:26 GMT  
		Size: 27.8 MB (27846798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49a411b92496b09252a7bc9307636e321a65e7e5b69404cf4963dde5e312918`  
		Last Modified: Thu, 07 Sep 2023 20:08:09 GMT  
		Size: 2.8 MB (2792494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72f421756be6061e4ef3c6d514f4a5de79f29d240754f90387065ffd7af38a0`  
		Last Modified: Thu, 07 Sep 2023 20:08:24 GMT  
		Size: 68.8 MB (68810224 bytes)  
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
$ docker pull mono@sha256:a50ed72d1e926e69f254583815ec6f9e1477d384ad172994b1f5fba8cc1e863c
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
$ docker pull mono@sha256:c81d20ab3c2cfa34908994640e4d54bb8785e74010828e7cc020085224d45d7a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.1 MB (225071705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39a523f59310718cb5b5c20bfe19390093eb45b349c200dc8ec03ffffb9d92d4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:35 GMT
ADD file:9c8b7c79fbbb19d308d151785d178e19bfa7b83257f38d03fa7f30cd41d58530 in / 
# Thu, 07 Sep 2023 00:21:35 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:54:01 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 07 Sep 2023 01:54:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 01:54:38 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 07 Sep 2023 02:01:13 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:91f01557fe0da558070d4f24631c94e91a80877a24621b52b8b13009b62d8d96`  
		Last Modified: Thu, 07 Sep 2023 00:26:44 GMT  
		Size: 27.2 MB (27187385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc5d89a2c6ca09bf688d79ac5db4246fdefa27e5e615596e38d98a3d7004085`  
		Last Modified: Thu, 07 Sep 2023 02:02:09 GMT  
		Size: 2.8 MB (2780979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b2e5ea4b1f22e2732556eaaffe5b7a63ff534cbb8bc4c7f4bfa0ef7a4006c8`  
		Last Modified: Thu, 07 Sep 2023 02:02:18 GMT  
		Size: 64.8 MB (64780737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00cd284208b62e734ff0717a5633b34ad6ab7c75ce996c806d44d0dfd7442174`  
		Last Modified: Thu, 07 Sep 2023 02:03:23 GMT  
		Size: 130.3 MB (130322604 bytes)  
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
$ docker pull mono@sha256:585d4b784434eaac45129926e950b9e54f50959656696a701a9e350e23563b23
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.8 MB (176819763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e02cb6480ffc6e1d91d3de5ebdb1211a64aa76f58e3050ac7b1926128b4ad5cc`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:58:32 GMT
ADD file:fa060a900723a2fce017a38b08be3eb2c27d4768d40c61cd1f6292a7f28a8bdc in / 
# Thu, 07 Sep 2023 00:58:33 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 04:04:24 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 07 Sep 2023 04:04:37 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 04:05:03 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 07 Sep 2023 04:09:14 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7e54f06c680feaf82a31a34e7453d765f332f671cfecacb622c3046561dcc572`  
		Last Modified: Thu, 07 Sep 2023 01:03:53 GMT  
		Size: 22.8 MB (22795752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa71da295adc94cd16f1b3e01841dcdddb62864fc9db081db98e9e2af5edd0ab`  
		Last Modified: Thu, 07 Sep 2023 04:10:01 GMT  
		Size: 2.4 MB (2370843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4357100575ec4e026c17ea214d62ab407b12a41766650a2286dc66f725d4b3`  
		Last Modified: Thu, 07 Sep 2023 04:10:05 GMT  
		Size: 23.8 MB (23816244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1990aeeabed38bc3b4ea26c80cb6199198960c34f7493b7f5de84433338dc3e`  
		Last Modified: Thu, 07 Sep 2023 04:11:17 GMT  
		Size: 127.8 MB (127836924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:aa8f522fc82cc03531069007821d86482f435372ce9166c8f42717faa57217e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.7 MB (203679473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3e7cd60933858135626c238424e3e14c7c76512cf8ec355002765003a5e90bd`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:08 GMT
ADD file:3521159cdea23e107a3e194ebc9b8f9a6a37ea8188236a267b6ec26e87cf498a in / 
# Thu, 07 Sep 2023 00:40:08 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 07:04:36 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 07 Sep 2023 07:04:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 07:04:59 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 07 Sep 2023 07:07:48 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d7cc66d62b738dea27e341b7322194f45ab1be2e548fe11d8ad953d9d56caaa8`  
		Last Modified: Thu, 07 Sep 2023 00:44:18 GMT  
		Size: 26.0 MB (25967748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1595a1cccc3b44c5745fc712d26904327dbd3ff8e753c8300d1787f754b3c7`  
		Last Modified: Thu, 07 Sep 2023 07:08:25 GMT  
		Size: 2.6 MB (2645837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e254e11541fd91f2cbf884ccc172b5bf85091f11525af10efbb731b988a7ea`  
		Last Modified: Thu, 07 Sep 2023 07:08:29 GMT  
		Size: 29.6 MB (29575307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d350ab45b73413a3bed763e99f41182dc4457ff9e748a4c552c3a6758e0c71`  
		Last Modified: Thu, 07 Sep 2023 07:09:30 GMT  
		Size: 145.5 MB (145490581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; 386

```console
$ docker pull mono@sha256:d7f5051a9ffffbe7ba1492d5b5d90f0fb2534215e24d6cfe6953e3b8ef507867
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.9 MB (230912227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94159b274f52570585dd17d2fd66b0d304e28e8b3dcfeac09e57a040eecb243b`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:46 GMT
ADD file:e5916da683bdcea27e31e6fbb29e61d1f8457a3bebe4a83278e4f0181e5ac49f in / 
# Thu, 07 Sep 2023 00:39:47 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 20:03:26 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 07 Sep 2023 20:03:37 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 20:04:07 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 07 Sep 2023 20:07:04 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:453c610c7d8be388b9a8559dc654a2def01e71f776e0608ae46db51ae50d10a0`  
		Last Modified: Thu, 07 Sep 2023 00:45:26 GMT  
		Size: 27.8 MB (27846798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49a411b92496b09252a7bc9307636e321a65e7e5b69404cf4963dde5e312918`  
		Last Modified: Thu, 07 Sep 2023 20:08:09 GMT  
		Size: 2.8 MB (2792494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72f421756be6061e4ef3c6d514f4a5de79f29d240754f90387065ffd7af38a0`  
		Last Modified: Thu, 07 Sep 2023 20:08:24 GMT  
		Size: 68.8 MB (68810224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8bdd28cc5ec0fd10f08b7d982e6281078eb0c901145eb3697527cc03d4bb0f`  
		Last Modified: Thu, 07 Sep 2023 20:09:56 GMT  
		Size: 131.5 MB (131462711 bytes)  
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
$ docker pull mono@sha256:10ad89d7a60030a8f6f18d20f15efaa00f20b2d57877f7cf33445b5101680fb8
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
$ docker pull mono@sha256:4ad616f20a88b6db041b9b527ba05c57edfc1d59fe38be506ca6d6cda41c6e36
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94749101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7dbc470c7bfc374f3693ac0dce9c5bbcd8b7316e25a7037affdea1aa126b989`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:35 GMT
ADD file:9c8b7c79fbbb19d308d151785d178e19bfa7b83257f38d03fa7f30cd41d58530 in / 
# Thu, 07 Sep 2023 00:21:35 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:54:01 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 07 Sep 2023 01:54:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 01:54:38 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:91f01557fe0da558070d4f24631c94e91a80877a24621b52b8b13009b62d8d96`  
		Last Modified: Thu, 07 Sep 2023 00:26:44 GMT  
		Size: 27.2 MB (27187385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc5d89a2c6ca09bf688d79ac5db4246fdefa27e5e615596e38d98a3d7004085`  
		Last Modified: Thu, 07 Sep 2023 02:02:09 GMT  
		Size: 2.8 MB (2780979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b2e5ea4b1f22e2732556eaaffe5b7a63ff534cbb8bc4c7f4bfa0ef7a4006c8`  
		Last Modified: Thu, 07 Sep 2023 02:02:18 GMT  
		Size: 64.8 MB (64780737 bytes)  
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
$ docker pull mono@sha256:8a53e999e0d3f853d39cfee9d3b50044952aa86e2c3a644e2bcd5959d54736da
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48982839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dd3702c7d1ecb59e85a74d0d88b40f468b8f0c63aad29827499a35159022d24`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:58:32 GMT
ADD file:fa060a900723a2fce017a38b08be3eb2c27d4768d40c61cd1f6292a7f28a8bdc in / 
# Thu, 07 Sep 2023 00:58:33 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 04:04:24 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 07 Sep 2023 04:04:37 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 04:05:03 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7e54f06c680feaf82a31a34e7453d765f332f671cfecacb622c3046561dcc572`  
		Last Modified: Thu, 07 Sep 2023 01:03:53 GMT  
		Size: 22.8 MB (22795752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa71da295adc94cd16f1b3e01841dcdddb62864fc9db081db98e9e2af5edd0ab`  
		Last Modified: Thu, 07 Sep 2023 04:10:01 GMT  
		Size: 2.4 MB (2370843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4357100575ec4e026c17ea214d62ab407b12a41766650a2286dc66f725d4b3`  
		Last Modified: Thu, 07 Sep 2023 04:10:05 GMT  
		Size: 23.8 MB (23816244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:3cbbba9bce7f3997ad3096fd27bc1a267670dae18a75d224b0d43f305c255339
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.2 MB (58188892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81355dd1459418e965f6e723af0bf0e17fce76ac8b740d9db11846b6f174a87a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:08 GMT
ADD file:3521159cdea23e107a3e194ebc9b8f9a6a37ea8188236a267b6ec26e87cf498a in / 
# Thu, 07 Sep 2023 00:40:08 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 07:04:36 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 07 Sep 2023 07:04:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 07:04:59 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d7cc66d62b738dea27e341b7322194f45ab1be2e548fe11d8ad953d9d56caaa8`  
		Last Modified: Thu, 07 Sep 2023 00:44:18 GMT  
		Size: 26.0 MB (25967748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1595a1cccc3b44c5745fc712d26904327dbd3ff8e753c8300d1787f754b3c7`  
		Last Modified: Thu, 07 Sep 2023 07:08:25 GMT  
		Size: 2.6 MB (2645837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e254e11541fd91f2cbf884ccc172b5bf85091f11525af10efbb731b988a7ea`  
		Last Modified: Thu, 07 Sep 2023 07:08:29 GMT  
		Size: 29.6 MB (29575307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; 386

```console
$ docker pull mono@sha256:8ca2a0a252b5f280b301bdec97fcc0c2401ce3ff9dc936226b9fc152157af416
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99449516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1982032d75d0f0362ac653f5f8a88b8adbb56475ac1cdd86db81ffbaa3e0893`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:46 GMT
ADD file:e5916da683bdcea27e31e6fbb29e61d1f8457a3bebe4a83278e4f0181e5ac49f in / 
# Thu, 07 Sep 2023 00:39:47 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 20:03:26 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 07 Sep 2023 20:03:37 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 20:04:07 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:453c610c7d8be388b9a8559dc654a2def01e71f776e0608ae46db51ae50d10a0`  
		Last Modified: Thu, 07 Sep 2023 00:45:26 GMT  
		Size: 27.8 MB (27846798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49a411b92496b09252a7bc9307636e321a65e7e5b69404cf4963dde5e312918`  
		Last Modified: Thu, 07 Sep 2023 20:08:09 GMT  
		Size: 2.8 MB (2792494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72f421756be6061e4ef3c6d514f4a5de79f29d240754f90387065ffd7af38a0`  
		Last Modified: Thu, 07 Sep 2023 20:08:24 GMT  
		Size: 68.8 MB (68810224 bytes)  
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
$ docker pull mono@sha256:a50ed72d1e926e69f254583815ec6f9e1477d384ad172994b1f5fba8cc1e863c
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
$ docker pull mono@sha256:c81d20ab3c2cfa34908994640e4d54bb8785e74010828e7cc020085224d45d7a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.1 MB (225071705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39a523f59310718cb5b5c20bfe19390093eb45b349c200dc8ec03ffffb9d92d4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:35 GMT
ADD file:9c8b7c79fbbb19d308d151785d178e19bfa7b83257f38d03fa7f30cd41d58530 in / 
# Thu, 07 Sep 2023 00:21:35 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:54:01 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 07 Sep 2023 01:54:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 01:54:38 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 07 Sep 2023 02:01:13 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:91f01557fe0da558070d4f24631c94e91a80877a24621b52b8b13009b62d8d96`  
		Last Modified: Thu, 07 Sep 2023 00:26:44 GMT  
		Size: 27.2 MB (27187385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc5d89a2c6ca09bf688d79ac5db4246fdefa27e5e615596e38d98a3d7004085`  
		Last Modified: Thu, 07 Sep 2023 02:02:09 GMT  
		Size: 2.8 MB (2780979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b2e5ea4b1f22e2732556eaaffe5b7a63ff534cbb8bc4c7f4bfa0ef7a4006c8`  
		Last Modified: Thu, 07 Sep 2023 02:02:18 GMT  
		Size: 64.8 MB (64780737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00cd284208b62e734ff0717a5633b34ad6ab7c75ce996c806d44d0dfd7442174`  
		Last Modified: Thu, 07 Sep 2023 02:03:23 GMT  
		Size: 130.3 MB (130322604 bytes)  
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
$ docker pull mono@sha256:585d4b784434eaac45129926e950b9e54f50959656696a701a9e350e23563b23
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.8 MB (176819763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e02cb6480ffc6e1d91d3de5ebdb1211a64aa76f58e3050ac7b1926128b4ad5cc`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:58:32 GMT
ADD file:fa060a900723a2fce017a38b08be3eb2c27d4768d40c61cd1f6292a7f28a8bdc in / 
# Thu, 07 Sep 2023 00:58:33 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 04:04:24 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 07 Sep 2023 04:04:37 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 04:05:03 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 07 Sep 2023 04:09:14 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7e54f06c680feaf82a31a34e7453d765f332f671cfecacb622c3046561dcc572`  
		Last Modified: Thu, 07 Sep 2023 01:03:53 GMT  
		Size: 22.8 MB (22795752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa71da295adc94cd16f1b3e01841dcdddb62864fc9db081db98e9e2af5edd0ab`  
		Last Modified: Thu, 07 Sep 2023 04:10:01 GMT  
		Size: 2.4 MB (2370843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4357100575ec4e026c17ea214d62ab407b12a41766650a2286dc66f725d4b3`  
		Last Modified: Thu, 07 Sep 2023 04:10:05 GMT  
		Size: 23.8 MB (23816244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1990aeeabed38bc3b4ea26c80cb6199198960c34f7493b7f5de84433338dc3e`  
		Last Modified: Thu, 07 Sep 2023 04:11:17 GMT  
		Size: 127.8 MB (127836924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:aa8f522fc82cc03531069007821d86482f435372ce9166c8f42717faa57217e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.7 MB (203679473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3e7cd60933858135626c238424e3e14c7c76512cf8ec355002765003a5e90bd`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:08 GMT
ADD file:3521159cdea23e107a3e194ebc9b8f9a6a37ea8188236a267b6ec26e87cf498a in / 
# Thu, 07 Sep 2023 00:40:08 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 07:04:36 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 07 Sep 2023 07:04:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 07:04:59 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 07 Sep 2023 07:07:48 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d7cc66d62b738dea27e341b7322194f45ab1be2e548fe11d8ad953d9d56caaa8`  
		Last Modified: Thu, 07 Sep 2023 00:44:18 GMT  
		Size: 26.0 MB (25967748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1595a1cccc3b44c5745fc712d26904327dbd3ff8e753c8300d1787f754b3c7`  
		Last Modified: Thu, 07 Sep 2023 07:08:25 GMT  
		Size: 2.6 MB (2645837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e254e11541fd91f2cbf884ccc172b5bf85091f11525af10efbb731b988a7ea`  
		Last Modified: Thu, 07 Sep 2023 07:08:29 GMT  
		Size: 29.6 MB (29575307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d350ab45b73413a3bed763e99f41182dc4457ff9e748a4c552c3a6758e0c71`  
		Last Modified: Thu, 07 Sep 2023 07:09:30 GMT  
		Size: 145.5 MB (145490581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; 386

```console
$ docker pull mono@sha256:d7f5051a9ffffbe7ba1492d5b5d90f0fb2534215e24d6cfe6953e3b8ef507867
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.9 MB (230912227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94159b274f52570585dd17d2fd66b0d304e28e8b3dcfeac09e57a040eecb243b`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:46 GMT
ADD file:e5916da683bdcea27e31e6fbb29e61d1f8457a3bebe4a83278e4f0181e5ac49f in / 
# Thu, 07 Sep 2023 00:39:47 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 20:03:26 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 07 Sep 2023 20:03:37 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 20:04:07 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 07 Sep 2023 20:07:04 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:453c610c7d8be388b9a8559dc654a2def01e71f776e0608ae46db51ae50d10a0`  
		Last Modified: Thu, 07 Sep 2023 00:45:26 GMT  
		Size: 27.8 MB (27846798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49a411b92496b09252a7bc9307636e321a65e7e5b69404cf4963dde5e312918`  
		Last Modified: Thu, 07 Sep 2023 20:08:09 GMT  
		Size: 2.8 MB (2792494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72f421756be6061e4ef3c6d514f4a5de79f29d240754f90387065ffd7af38a0`  
		Last Modified: Thu, 07 Sep 2023 20:08:24 GMT  
		Size: 68.8 MB (68810224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8bdd28cc5ec0fd10f08b7d982e6281078eb0c901145eb3697527cc03d4bb0f`  
		Last Modified: Thu, 07 Sep 2023 20:09:56 GMT  
		Size: 131.5 MB (131462711 bytes)  
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
$ docker pull mono@sha256:10ad89d7a60030a8f6f18d20f15efaa00f20b2d57877f7cf33445b5101680fb8
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
$ docker pull mono@sha256:4ad616f20a88b6db041b9b527ba05c57edfc1d59fe38be506ca6d6cda41c6e36
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94749101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7dbc470c7bfc374f3693ac0dce9c5bbcd8b7316e25a7037affdea1aa126b989`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:35 GMT
ADD file:9c8b7c79fbbb19d308d151785d178e19bfa7b83257f38d03fa7f30cd41d58530 in / 
# Thu, 07 Sep 2023 00:21:35 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:54:01 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 07 Sep 2023 01:54:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 01:54:38 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:91f01557fe0da558070d4f24631c94e91a80877a24621b52b8b13009b62d8d96`  
		Last Modified: Thu, 07 Sep 2023 00:26:44 GMT  
		Size: 27.2 MB (27187385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc5d89a2c6ca09bf688d79ac5db4246fdefa27e5e615596e38d98a3d7004085`  
		Last Modified: Thu, 07 Sep 2023 02:02:09 GMT  
		Size: 2.8 MB (2780979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b2e5ea4b1f22e2732556eaaffe5b7a63ff534cbb8bc4c7f4bfa0ef7a4006c8`  
		Last Modified: Thu, 07 Sep 2023 02:02:18 GMT  
		Size: 64.8 MB (64780737 bytes)  
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
$ docker pull mono@sha256:8a53e999e0d3f853d39cfee9d3b50044952aa86e2c3a644e2bcd5959d54736da
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48982839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dd3702c7d1ecb59e85a74d0d88b40f468b8f0c63aad29827499a35159022d24`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:58:32 GMT
ADD file:fa060a900723a2fce017a38b08be3eb2c27d4768d40c61cd1f6292a7f28a8bdc in / 
# Thu, 07 Sep 2023 00:58:33 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 04:04:24 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 07 Sep 2023 04:04:37 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 04:05:03 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7e54f06c680feaf82a31a34e7453d765f332f671cfecacb622c3046561dcc572`  
		Last Modified: Thu, 07 Sep 2023 01:03:53 GMT  
		Size: 22.8 MB (22795752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa71da295adc94cd16f1b3e01841dcdddb62864fc9db081db98e9e2af5edd0ab`  
		Last Modified: Thu, 07 Sep 2023 04:10:01 GMT  
		Size: 2.4 MB (2370843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4357100575ec4e026c17ea214d62ab407b12a41766650a2286dc66f725d4b3`  
		Last Modified: Thu, 07 Sep 2023 04:10:05 GMT  
		Size: 23.8 MB (23816244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:3cbbba9bce7f3997ad3096fd27bc1a267670dae18a75d224b0d43f305c255339
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.2 MB (58188892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81355dd1459418e965f6e723af0bf0e17fce76ac8b740d9db11846b6f174a87a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:08 GMT
ADD file:3521159cdea23e107a3e194ebc9b8f9a6a37ea8188236a267b6ec26e87cf498a in / 
# Thu, 07 Sep 2023 00:40:08 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 07:04:36 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 07 Sep 2023 07:04:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 07:04:59 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d7cc66d62b738dea27e341b7322194f45ab1be2e548fe11d8ad953d9d56caaa8`  
		Last Modified: Thu, 07 Sep 2023 00:44:18 GMT  
		Size: 26.0 MB (25967748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1595a1cccc3b44c5745fc712d26904327dbd3ff8e753c8300d1787f754b3c7`  
		Last Modified: Thu, 07 Sep 2023 07:08:25 GMT  
		Size: 2.6 MB (2645837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e254e11541fd91f2cbf884ccc172b5bf85091f11525af10efbb731b988a7ea`  
		Last Modified: Thu, 07 Sep 2023 07:08:29 GMT  
		Size: 29.6 MB (29575307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; 386

```console
$ docker pull mono@sha256:8ca2a0a252b5f280b301bdec97fcc0c2401ce3ff9dc936226b9fc152157af416
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99449516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1982032d75d0f0362ac653f5f8a88b8adbb56475ac1cdd86db81ffbaa3e0893`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:46 GMT
ADD file:e5916da683bdcea27e31e6fbb29e61d1f8457a3bebe4a83278e4f0181e5ac49f in / 
# Thu, 07 Sep 2023 00:39:47 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 20:03:26 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 07 Sep 2023 20:03:37 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 20:04:07 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:453c610c7d8be388b9a8559dc654a2def01e71f776e0608ae46db51ae50d10a0`  
		Last Modified: Thu, 07 Sep 2023 00:45:26 GMT  
		Size: 27.8 MB (27846798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49a411b92496b09252a7bc9307636e321a65e7e5b69404cf4963dde5e312918`  
		Last Modified: Thu, 07 Sep 2023 20:08:09 GMT  
		Size: 2.8 MB (2792494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72f421756be6061e4ef3c6d514f4a5de79f29d240754f90387065ffd7af38a0`  
		Last Modified: Thu, 07 Sep 2023 20:08:24 GMT  
		Size: 68.8 MB (68810224 bytes)  
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
$ docker pull mono@sha256:465112ebaf92fd33d9560a26e74848a07d18046f50f9c025d3837681f026d172
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
$ docker pull mono@sha256:089c69437f670a34d6d2faa7d15e29f3395a354b8ff3073598e76279cb9ba5d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.7 MB (254674329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f97afc4690efd1650c1d74e46a929a04e32f8d6c731f5958d15ef41826db0f4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:35 GMT
ADD file:9c8b7c79fbbb19d308d151785d178e19bfa7b83257f38d03fa7f30cd41d58530 in / 
# Thu, 07 Sep 2023 00:21:35 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:53:20 GMT
ENV MONO_VERSION=6.12.0.182
# Thu, 07 Sep 2023 01:53:30 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 01:53:54 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 07 Sep 2023 01:55:46 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:91f01557fe0da558070d4f24631c94e91a80877a24621b52b8b13009b62d8d96`  
		Last Modified: Thu, 07 Sep 2023 00:26:44 GMT  
		Size: 27.2 MB (27187385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12132fc81fdf72f5e5905edc96ba6db064fb390345d3f9c4a04b0aa7ff243e17`  
		Last Modified: Thu, 07 Sep 2023 02:01:44 GMT  
		Size: 2.8 MB (2780987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa4cf5e71acb35ad398b3bdf0cb7e63ba3591f8b633a45b2de4cd67d205f009`  
		Last Modified: Thu, 07 Sep 2023 02:01:53 GMT  
		Size: 64.8 MB (64774202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3bf7c27d69e706c535fab335198d46ba19e96cfe916e4116406ad5e1783746c`  
		Last Modified: Thu, 07 Sep 2023 02:02:51 GMT  
		Size: 159.9 MB (159931755 bytes)  
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
$ docker pull mono@sha256:3f2c50251c47c6e8daf7af30af91621870ae8d4bfed30819f452eac8026bbc53
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.0 MB (189021480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a2e8c2751e838c4f926991046e298b87181672c53a47b727e2749fcf1b8f8bb`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:58:32 GMT
ADD file:fa060a900723a2fce017a38b08be3eb2c27d4768d40c61cd1f6292a7f28a8bdc in / 
# Thu, 07 Sep 2023 00:58:33 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 04:03:37 GMT
ENV MONO_VERSION=6.12.0.182
# Thu, 07 Sep 2023 04:03:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 04:04:15 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 07 Sep 2023 04:07:12 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7e54f06c680feaf82a31a34e7453d765f332f671cfecacb622c3046561dcc572`  
		Last Modified: Thu, 07 Sep 2023 01:03:53 GMT  
		Size: 22.8 MB (22795752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896cf2b79eb9e448095cab03cb5968875cc5fb527a67d79649025441961efd82`  
		Last Modified: Thu, 07 Sep 2023 04:09:43 GMT  
		Size: 2.4 MB (2370781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a2303b2c37a5342143c8d7bceadf10352b40615dd417f3b04a47a83cde7b61`  
		Last Modified: Thu, 07 Sep 2023 04:09:47 GMT  
		Size: 23.8 MB (23791111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ef087b8af56f6ad24f17f51ab214d3d95a09c5048d36d54b9d3baa3c3ee8c7`  
		Last Modified: Thu, 07 Sep 2023 04:10:40 GMT  
		Size: 140.1 MB (140063836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:85439cb4fbff445b7a7a5c9857be3eb18a25f0c00ab310ca7597931b9f3357bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.4 MB (216404975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99b3fc85c61b2f9fefe7369de60ce845f2863ba714bb8aef6ff5d23a056af68e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:08 GMT
ADD file:3521159cdea23e107a3e194ebc9b8f9a6a37ea8188236a267b6ec26e87cf498a in / 
# Thu, 07 Sep 2023 00:40:08 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 07:04:02 GMT
ENV MONO_VERSION=6.12.0.182
# Thu, 07 Sep 2023 07:04:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 07:04:31 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 07 Sep 2023 07:06:47 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d7cc66d62b738dea27e341b7322194f45ab1be2e548fe11d8ad953d9d56caaa8`  
		Last Modified: Thu, 07 Sep 2023 00:44:18 GMT  
		Size: 26.0 MB (25967748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53037d9952d0efe71a5774348f92d173432e8dbdf95ceb18450c7c07c6c9e9f`  
		Last Modified: Thu, 07 Sep 2023 07:08:07 GMT  
		Size: 2.6 MB (2645888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f85155c32dab21f86975a13ba62dbc5410813df3fcafba56051eec44247a61`  
		Last Modified: Thu, 07 Sep 2023 07:08:10 GMT  
		Size: 29.5 MB (29545041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54bf7f84fb7a3b3125859753112a10e4bb673ae6d6ee00e235ac568ca6a4d15f`  
		Last Modified: Thu, 07 Sep 2023 07:08:58 GMT  
		Size: 158.2 MB (158246298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12` - linux; 386

```console
$ docker pull mono@sha256:d914db5bbe9949453c7c8cdb8ef643d53db6a920a0d2f341a8ba6c5119117000
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.6 MB (259560153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1750b1ccddddd0725b37eccca344d9e8b827165b132275486ab1908759b2b4ca`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:46 GMT
ADD file:e5916da683bdcea27e31e6fbb29e61d1f8457a3bebe4a83278e4f0181e5ac49f in / 
# Thu, 07 Sep 2023 00:39:47 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 20:02:37 GMT
ENV MONO_VERSION=6.12.0.182
# Thu, 07 Sep 2023 20:02:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 20:03:19 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 07 Sep 2023 20:05:40 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:453c610c7d8be388b9a8559dc654a2def01e71f776e0608ae46db51ae50d10a0`  
		Last Modified: Thu, 07 Sep 2023 00:45:26 GMT  
		Size: 27.8 MB (27846798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d6396be6afdd9df4ac1ad90d0ab9aaef68b9759a6d4ec028aa8c4963970ca3`  
		Last Modified: Thu, 07 Sep 2023 20:07:31 GMT  
		Size: 2.8 MB (2792479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58c12dba60a13a57b5648614b665be3d02ce9e747541083ab284b2a34873e6c`  
		Last Modified: Thu, 07 Sep 2023 20:07:45 GMT  
		Size: 68.8 MB (68800678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45574f7922a18c136182a845a84aa83dbaa55b270403803504630217c6dc1223`  
		Last Modified: Thu, 07 Sep 2023 20:09:11 GMT  
		Size: 160.1 MB (160120198 bytes)  
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
$ docker pull mono@sha256:4ac0e6a9361a55b14456a63130b931ea563ab6281f8bede836d29892544554b8
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
$ docker pull mono@sha256:84cc79f2e8be438c04f8eade849b8757727be784faca8efa67f7e1c38ea24633
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94742574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdb686b94af3d0fe092a2df584b75557331d28d1de5050abbd456bba31475781`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:35 GMT
ADD file:9c8b7c79fbbb19d308d151785d178e19bfa7b83257f38d03fa7f30cd41d58530 in / 
# Thu, 07 Sep 2023 00:21:35 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:53:20 GMT
ENV MONO_VERSION=6.12.0.182
# Thu, 07 Sep 2023 01:53:30 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 01:53:54 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:91f01557fe0da558070d4f24631c94e91a80877a24621b52b8b13009b62d8d96`  
		Last Modified: Thu, 07 Sep 2023 00:26:44 GMT  
		Size: 27.2 MB (27187385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12132fc81fdf72f5e5905edc96ba6db064fb390345d3f9c4a04b0aa7ff243e17`  
		Last Modified: Thu, 07 Sep 2023 02:01:44 GMT  
		Size: 2.8 MB (2780987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa4cf5e71acb35ad398b3bdf0cb7e63ba3591f8b633a45b2de4cd67d205f009`  
		Last Modified: Thu, 07 Sep 2023 02:01:53 GMT  
		Size: 64.8 MB (64774202 bytes)  
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
$ docker pull mono@sha256:f92793d95509dc30e2d40b85171aece1c5a1aff00d70062e9e2fc646b1a7ead0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48957644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b101a66aff317c6451bacbe4d8db8760c98060d12d5bc238f97322dc5cd418f7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:58:32 GMT
ADD file:fa060a900723a2fce017a38b08be3eb2c27d4768d40c61cd1f6292a7f28a8bdc in / 
# Thu, 07 Sep 2023 00:58:33 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 04:03:37 GMT
ENV MONO_VERSION=6.12.0.182
# Thu, 07 Sep 2023 04:03:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 04:04:15 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7e54f06c680feaf82a31a34e7453d765f332f671cfecacb622c3046561dcc572`  
		Last Modified: Thu, 07 Sep 2023 01:03:53 GMT  
		Size: 22.8 MB (22795752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896cf2b79eb9e448095cab03cb5968875cc5fb527a67d79649025441961efd82`  
		Last Modified: Thu, 07 Sep 2023 04:09:43 GMT  
		Size: 2.4 MB (2370781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a2303b2c37a5342143c8d7bceadf10352b40615dd417f3b04a47a83cde7b61`  
		Last Modified: Thu, 07 Sep 2023 04:09:47 GMT  
		Size: 23.8 MB (23791111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:6a13402decdc835e814b8a9d08ca232a924b5a436a6e1aceb23980ea7cc0d770
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.2 MB (58158677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1633b0a05c1e8711d19da02dc723dffbef9d8e4d6f7f07b39eb54d46b8d2df0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:08 GMT
ADD file:3521159cdea23e107a3e194ebc9b8f9a6a37ea8188236a267b6ec26e87cf498a in / 
# Thu, 07 Sep 2023 00:40:08 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 07:04:02 GMT
ENV MONO_VERSION=6.12.0.182
# Thu, 07 Sep 2023 07:04:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 07:04:31 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d7cc66d62b738dea27e341b7322194f45ab1be2e548fe11d8ad953d9d56caaa8`  
		Last Modified: Thu, 07 Sep 2023 00:44:18 GMT  
		Size: 26.0 MB (25967748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53037d9952d0efe71a5774348f92d173432e8dbdf95ceb18450c7c07c6c9e9f`  
		Last Modified: Thu, 07 Sep 2023 07:08:07 GMT  
		Size: 2.6 MB (2645888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f85155c32dab21f86975a13ba62dbc5410813df3fcafba56051eec44247a61`  
		Last Modified: Thu, 07 Sep 2023 07:08:10 GMT  
		Size: 29.5 MB (29545041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12-slim` - linux; 386

```console
$ docker pull mono@sha256:1e331750b2de2f768b2b3359c5cb5ff9d777f02907ae9f9610d1c7bd86c29385
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99439955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dde61adb84e6642ed59730f8251c19a89212a3b608e7905770466bf8ad8b3a45`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:46 GMT
ADD file:e5916da683bdcea27e31e6fbb29e61d1f8457a3bebe4a83278e4f0181e5ac49f in / 
# Thu, 07 Sep 2023 00:39:47 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 20:02:37 GMT
ENV MONO_VERSION=6.12.0.182
# Thu, 07 Sep 2023 20:02:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 20:03:19 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:453c610c7d8be388b9a8559dc654a2def01e71f776e0608ae46db51ae50d10a0`  
		Last Modified: Thu, 07 Sep 2023 00:45:26 GMT  
		Size: 27.8 MB (27846798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d6396be6afdd9df4ac1ad90d0ab9aaef68b9759a6d4ec028aa8c4963970ca3`  
		Last Modified: Thu, 07 Sep 2023 20:07:31 GMT  
		Size: 2.8 MB (2792479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58c12dba60a13a57b5648614b665be3d02ce9e747541083ab284b2a34873e6c`  
		Last Modified: Thu, 07 Sep 2023 20:07:45 GMT  
		Size: 68.8 MB (68800678 bytes)  
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
$ docker pull mono@sha256:465112ebaf92fd33d9560a26e74848a07d18046f50f9c025d3837681f026d172
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
$ docker pull mono@sha256:089c69437f670a34d6d2faa7d15e29f3395a354b8ff3073598e76279cb9ba5d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.7 MB (254674329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f97afc4690efd1650c1d74e46a929a04e32f8d6c731f5958d15ef41826db0f4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:35 GMT
ADD file:9c8b7c79fbbb19d308d151785d178e19bfa7b83257f38d03fa7f30cd41d58530 in / 
# Thu, 07 Sep 2023 00:21:35 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:53:20 GMT
ENV MONO_VERSION=6.12.0.182
# Thu, 07 Sep 2023 01:53:30 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 01:53:54 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 07 Sep 2023 01:55:46 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:91f01557fe0da558070d4f24631c94e91a80877a24621b52b8b13009b62d8d96`  
		Last Modified: Thu, 07 Sep 2023 00:26:44 GMT  
		Size: 27.2 MB (27187385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12132fc81fdf72f5e5905edc96ba6db064fb390345d3f9c4a04b0aa7ff243e17`  
		Last Modified: Thu, 07 Sep 2023 02:01:44 GMT  
		Size: 2.8 MB (2780987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa4cf5e71acb35ad398b3bdf0cb7e63ba3591f8b633a45b2de4cd67d205f009`  
		Last Modified: Thu, 07 Sep 2023 02:01:53 GMT  
		Size: 64.8 MB (64774202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3bf7c27d69e706c535fab335198d46ba19e96cfe916e4116406ad5e1783746c`  
		Last Modified: Thu, 07 Sep 2023 02:02:51 GMT  
		Size: 159.9 MB (159931755 bytes)  
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
$ docker pull mono@sha256:3f2c50251c47c6e8daf7af30af91621870ae8d4bfed30819f452eac8026bbc53
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.0 MB (189021480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a2e8c2751e838c4f926991046e298b87181672c53a47b727e2749fcf1b8f8bb`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:58:32 GMT
ADD file:fa060a900723a2fce017a38b08be3eb2c27d4768d40c61cd1f6292a7f28a8bdc in / 
# Thu, 07 Sep 2023 00:58:33 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 04:03:37 GMT
ENV MONO_VERSION=6.12.0.182
# Thu, 07 Sep 2023 04:03:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 04:04:15 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 07 Sep 2023 04:07:12 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7e54f06c680feaf82a31a34e7453d765f332f671cfecacb622c3046561dcc572`  
		Last Modified: Thu, 07 Sep 2023 01:03:53 GMT  
		Size: 22.8 MB (22795752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896cf2b79eb9e448095cab03cb5968875cc5fb527a67d79649025441961efd82`  
		Last Modified: Thu, 07 Sep 2023 04:09:43 GMT  
		Size: 2.4 MB (2370781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a2303b2c37a5342143c8d7bceadf10352b40615dd417f3b04a47a83cde7b61`  
		Last Modified: Thu, 07 Sep 2023 04:09:47 GMT  
		Size: 23.8 MB (23791111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ef087b8af56f6ad24f17f51ab214d3d95a09c5048d36d54b9d3baa3c3ee8c7`  
		Last Modified: Thu, 07 Sep 2023 04:10:40 GMT  
		Size: 140.1 MB (140063836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:85439cb4fbff445b7a7a5c9857be3eb18a25f0c00ab310ca7597931b9f3357bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.4 MB (216404975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99b3fc85c61b2f9fefe7369de60ce845f2863ba714bb8aef6ff5d23a056af68e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:08 GMT
ADD file:3521159cdea23e107a3e194ebc9b8f9a6a37ea8188236a267b6ec26e87cf498a in / 
# Thu, 07 Sep 2023 00:40:08 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 07:04:02 GMT
ENV MONO_VERSION=6.12.0.182
# Thu, 07 Sep 2023 07:04:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 07:04:31 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 07 Sep 2023 07:06:47 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d7cc66d62b738dea27e341b7322194f45ab1be2e548fe11d8ad953d9d56caaa8`  
		Last Modified: Thu, 07 Sep 2023 00:44:18 GMT  
		Size: 26.0 MB (25967748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53037d9952d0efe71a5774348f92d173432e8dbdf95ceb18450c7c07c6c9e9f`  
		Last Modified: Thu, 07 Sep 2023 07:08:07 GMT  
		Size: 2.6 MB (2645888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f85155c32dab21f86975a13ba62dbc5410813df3fcafba56051eec44247a61`  
		Last Modified: Thu, 07 Sep 2023 07:08:10 GMT  
		Size: 29.5 MB (29545041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54bf7f84fb7a3b3125859753112a10e4bb673ae6d6ee00e235ac568ca6a4d15f`  
		Last Modified: Thu, 07 Sep 2023 07:08:58 GMT  
		Size: 158.2 MB (158246298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0` - linux; 386

```console
$ docker pull mono@sha256:d914db5bbe9949453c7c8cdb8ef643d53db6a920a0d2f341a8ba6c5119117000
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.6 MB (259560153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1750b1ccddddd0725b37eccca344d9e8b827165b132275486ab1908759b2b4ca`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:46 GMT
ADD file:e5916da683bdcea27e31e6fbb29e61d1f8457a3bebe4a83278e4f0181e5ac49f in / 
# Thu, 07 Sep 2023 00:39:47 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 20:02:37 GMT
ENV MONO_VERSION=6.12.0.182
# Thu, 07 Sep 2023 20:02:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 20:03:19 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 07 Sep 2023 20:05:40 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:453c610c7d8be388b9a8559dc654a2def01e71f776e0608ae46db51ae50d10a0`  
		Last Modified: Thu, 07 Sep 2023 00:45:26 GMT  
		Size: 27.8 MB (27846798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d6396be6afdd9df4ac1ad90d0ab9aaef68b9759a6d4ec028aa8c4963970ca3`  
		Last Modified: Thu, 07 Sep 2023 20:07:31 GMT  
		Size: 2.8 MB (2792479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58c12dba60a13a57b5648614b665be3d02ce9e747541083ab284b2a34873e6c`  
		Last Modified: Thu, 07 Sep 2023 20:07:45 GMT  
		Size: 68.8 MB (68800678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45574f7922a18c136182a845a84aa83dbaa55b270403803504630217c6dc1223`  
		Last Modified: Thu, 07 Sep 2023 20:09:11 GMT  
		Size: 160.1 MB (160120198 bytes)  
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
$ docker pull mono@sha256:4ac0e6a9361a55b14456a63130b931ea563ab6281f8bede836d29892544554b8
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
$ docker pull mono@sha256:84cc79f2e8be438c04f8eade849b8757727be784faca8efa67f7e1c38ea24633
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94742574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdb686b94af3d0fe092a2df584b75557331d28d1de5050abbd456bba31475781`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:35 GMT
ADD file:9c8b7c79fbbb19d308d151785d178e19bfa7b83257f38d03fa7f30cd41d58530 in / 
# Thu, 07 Sep 2023 00:21:35 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:53:20 GMT
ENV MONO_VERSION=6.12.0.182
# Thu, 07 Sep 2023 01:53:30 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 01:53:54 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:91f01557fe0da558070d4f24631c94e91a80877a24621b52b8b13009b62d8d96`  
		Last Modified: Thu, 07 Sep 2023 00:26:44 GMT  
		Size: 27.2 MB (27187385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12132fc81fdf72f5e5905edc96ba6db064fb390345d3f9c4a04b0aa7ff243e17`  
		Last Modified: Thu, 07 Sep 2023 02:01:44 GMT  
		Size: 2.8 MB (2780987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa4cf5e71acb35ad398b3bdf0cb7e63ba3591f8b633a45b2de4cd67d205f009`  
		Last Modified: Thu, 07 Sep 2023 02:01:53 GMT  
		Size: 64.8 MB (64774202 bytes)  
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
$ docker pull mono@sha256:f92793d95509dc30e2d40b85171aece1c5a1aff00d70062e9e2fc646b1a7ead0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48957644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b101a66aff317c6451bacbe4d8db8760c98060d12d5bc238f97322dc5cd418f7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:58:32 GMT
ADD file:fa060a900723a2fce017a38b08be3eb2c27d4768d40c61cd1f6292a7f28a8bdc in / 
# Thu, 07 Sep 2023 00:58:33 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 04:03:37 GMT
ENV MONO_VERSION=6.12.0.182
# Thu, 07 Sep 2023 04:03:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 04:04:15 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7e54f06c680feaf82a31a34e7453d765f332f671cfecacb622c3046561dcc572`  
		Last Modified: Thu, 07 Sep 2023 01:03:53 GMT  
		Size: 22.8 MB (22795752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896cf2b79eb9e448095cab03cb5968875cc5fb527a67d79649025441961efd82`  
		Last Modified: Thu, 07 Sep 2023 04:09:43 GMT  
		Size: 2.4 MB (2370781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a2303b2c37a5342143c8d7bceadf10352b40615dd417f3b04a47a83cde7b61`  
		Last Modified: Thu, 07 Sep 2023 04:09:47 GMT  
		Size: 23.8 MB (23791111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:6a13402decdc835e814b8a9d08ca232a924b5a436a6e1aceb23980ea7cc0d770
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.2 MB (58158677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1633b0a05c1e8711d19da02dc723dffbef9d8e4d6f7f07b39eb54d46b8d2df0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:08 GMT
ADD file:3521159cdea23e107a3e194ebc9b8f9a6a37ea8188236a267b6ec26e87cf498a in / 
# Thu, 07 Sep 2023 00:40:08 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 07:04:02 GMT
ENV MONO_VERSION=6.12.0.182
# Thu, 07 Sep 2023 07:04:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 07:04:31 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d7cc66d62b738dea27e341b7322194f45ab1be2e548fe11d8ad953d9d56caaa8`  
		Last Modified: Thu, 07 Sep 2023 00:44:18 GMT  
		Size: 26.0 MB (25967748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53037d9952d0efe71a5774348f92d173432e8dbdf95ceb18450c7c07c6c9e9f`  
		Last Modified: Thu, 07 Sep 2023 07:08:07 GMT  
		Size: 2.6 MB (2645888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f85155c32dab21f86975a13ba62dbc5410813df3fcafba56051eec44247a61`  
		Last Modified: Thu, 07 Sep 2023 07:08:10 GMT  
		Size: 29.5 MB (29545041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0-slim` - linux; 386

```console
$ docker pull mono@sha256:1e331750b2de2f768b2b3359c5cb5ff9d777f02907ae9f9610d1c7bd86c29385
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99439955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dde61adb84e6642ed59730f8251c19a89212a3b608e7905770466bf8ad8b3a45`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:46 GMT
ADD file:e5916da683bdcea27e31e6fbb29e61d1f8457a3bebe4a83278e4f0181e5ac49f in / 
# Thu, 07 Sep 2023 00:39:47 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 20:02:37 GMT
ENV MONO_VERSION=6.12.0.182
# Thu, 07 Sep 2023 20:02:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 20:03:19 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:453c610c7d8be388b9a8559dc654a2def01e71f776e0608ae46db51ae50d10a0`  
		Last Modified: Thu, 07 Sep 2023 00:45:26 GMT  
		Size: 27.8 MB (27846798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d6396be6afdd9df4ac1ad90d0ab9aaef68b9759a6d4ec028aa8c4963970ca3`  
		Last Modified: Thu, 07 Sep 2023 20:07:31 GMT  
		Size: 2.8 MB (2792479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58c12dba60a13a57b5648614b665be3d02ce9e747541083ab284b2a34873e6c`  
		Last Modified: Thu, 07 Sep 2023 20:07:45 GMT  
		Size: 68.8 MB (68800678 bytes)  
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
$ docker pull mono@sha256:465112ebaf92fd33d9560a26e74848a07d18046f50f9c025d3837681f026d172
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
$ docker pull mono@sha256:089c69437f670a34d6d2faa7d15e29f3395a354b8ff3073598e76279cb9ba5d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.7 MB (254674329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f97afc4690efd1650c1d74e46a929a04e32f8d6c731f5958d15ef41826db0f4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:35 GMT
ADD file:9c8b7c79fbbb19d308d151785d178e19bfa7b83257f38d03fa7f30cd41d58530 in / 
# Thu, 07 Sep 2023 00:21:35 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:53:20 GMT
ENV MONO_VERSION=6.12.0.182
# Thu, 07 Sep 2023 01:53:30 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 01:53:54 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 07 Sep 2023 01:55:46 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:91f01557fe0da558070d4f24631c94e91a80877a24621b52b8b13009b62d8d96`  
		Last Modified: Thu, 07 Sep 2023 00:26:44 GMT  
		Size: 27.2 MB (27187385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12132fc81fdf72f5e5905edc96ba6db064fb390345d3f9c4a04b0aa7ff243e17`  
		Last Modified: Thu, 07 Sep 2023 02:01:44 GMT  
		Size: 2.8 MB (2780987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa4cf5e71acb35ad398b3bdf0cb7e63ba3591f8b633a45b2de4cd67d205f009`  
		Last Modified: Thu, 07 Sep 2023 02:01:53 GMT  
		Size: 64.8 MB (64774202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3bf7c27d69e706c535fab335198d46ba19e96cfe916e4116406ad5e1783746c`  
		Last Modified: Thu, 07 Sep 2023 02:02:51 GMT  
		Size: 159.9 MB (159931755 bytes)  
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
$ docker pull mono@sha256:3f2c50251c47c6e8daf7af30af91621870ae8d4bfed30819f452eac8026bbc53
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.0 MB (189021480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a2e8c2751e838c4f926991046e298b87181672c53a47b727e2749fcf1b8f8bb`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:58:32 GMT
ADD file:fa060a900723a2fce017a38b08be3eb2c27d4768d40c61cd1f6292a7f28a8bdc in / 
# Thu, 07 Sep 2023 00:58:33 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 04:03:37 GMT
ENV MONO_VERSION=6.12.0.182
# Thu, 07 Sep 2023 04:03:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 04:04:15 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 07 Sep 2023 04:07:12 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7e54f06c680feaf82a31a34e7453d765f332f671cfecacb622c3046561dcc572`  
		Last Modified: Thu, 07 Sep 2023 01:03:53 GMT  
		Size: 22.8 MB (22795752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896cf2b79eb9e448095cab03cb5968875cc5fb527a67d79649025441961efd82`  
		Last Modified: Thu, 07 Sep 2023 04:09:43 GMT  
		Size: 2.4 MB (2370781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a2303b2c37a5342143c8d7bceadf10352b40615dd417f3b04a47a83cde7b61`  
		Last Modified: Thu, 07 Sep 2023 04:09:47 GMT  
		Size: 23.8 MB (23791111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ef087b8af56f6ad24f17f51ab214d3d95a09c5048d36d54b9d3baa3c3ee8c7`  
		Last Modified: Thu, 07 Sep 2023 04:10:40 GMT  
		Size: 140.1 MB (140063836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.182` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:85439cb4fbff445b7a7a5c9857be3eb18a25f0c00ab310ca7597931b9f3357bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.4 MB (216404975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99b3fc85c61b2f9fefe7369de60ce845f2863ba714bb8aef6ff5d23a056af68e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:08 GMT
ADD file:3521159cdea23e107a3e194ebc9b8f9a6a37ea8188236a267b6ec26e87cf498a in / 
# Thu, 07 Sep 2023 00:40:08 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 07:04:02 GMT
ENV MONO_VERSION=6.12.0.182
# Thu, 07 Sep 2023 07:04:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 07:04:31 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 07 Sep 2023 07:06:47 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d7cc66d62b738dea27e341b7322194f45ab1be2e548fe11d8ad953d9d56caaa8`  
		Last Modified: Thu, 07 Sep 2023 00:44:18 GMT  
		Size: 26.0 MB (25967748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53037d9952d0efe71a5774348f92d173432e8dbdf95ceb18450c7c07c6c9e9f`  
		Last Modified: Thu, 07 Sep 2023 07:08:07 GMT  
		Size: 2.6 MB (2645888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f85155c32dab21f86975a13ba62dbc5410813df3fcafba56051eec44247a61`  
		Last Modified: Thu, 07 Sep 2023 07:08:10 GMT  
		Size: 29.5 MB (29545041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54bf7f84fb7a3b3125859753112a10e4bb673ae6d6ee00e235ac568ca6a4d15f`  
		Last Modified: Thu, 07 Sep 2023 07:08:58 GMT  
		Size: 158.2 MB (158246298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.182` - linux; 386

```console
$ docker pull mono@sha256:d914db5bbe9949453c7c8cdb8ef643d53db6a920a0d2f341a8ba6c5119117000
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.6 MB (259560153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1750b1ccddddd0725b37eccca344d9e8b827165b132275486ab1908759b2b4ca`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:46 GMT
ADD file:e5916da683bdcea27e31e6fbb29e61d1f8457a3bebe4a83278e4f0181e5ac49f in / 
# Thu, 07 Sep 2023 00:39:47 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 20:02:37 GMT
ENV MONO_VERSION=6.12.0.182
# Thu, 07 Sep 2023 20:02:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 20:03:19 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 07 Sep 2023 20:05:40 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:453c610c7d8be388b9a8559dc654a2def01e71f776e0608ae46db51ae50d10a0`  
		Last Modified: Thu, 07 Sep 2023 00:45:26 GMT  
		Size: 27.8 MB (27846798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d6396be6afdd9df4ac1ad90d0ab9aaef68b9759a6d4ec028aa8c4963970ca3`  
		Last Modified: Thu, 07 Sep 2023 20:07:31 GMT  
		Size: 2.8 MB (2792479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58c12dba60a13a57b5648614b665be3d02ce9e747541083ab284b2a34873e6c`  
		Last Modified: Thu, 07 Sep 2023 20:07:45 GMT  
		Size: 68.8 MB (68800678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45574f7922a18c136182a845a84aa83dbaa55b270403803504630217c6dc1223`  
		Last Modified: Thu, 07 Sep 2023 20:09:11 GMT  
		Size: 160.1 MB (160120198 bytes)  
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
$ docker pull mono@sha256:4ac0e6a9361a55b14456a63130b931ea563ab6281f8bede836d29892544554b8
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
$ docker pull mono@sha256:84cc79f2e8be438c04f8eade849b8757727be784faca8efa67f7e1c38ea24633
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94742574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdb686b94af3d0fe092a2df584b75557331d28d1de5050abbd456bba31475781`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:35 GMT
ADD file:9c8b7c79fbbb19d308d151785d178e19bfa7b83257f38d03fa7f30cd41d58530 in / 
# Thu, 07 Sep 2023 00:21:35 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:53:20 GMT
ENV MONO_VERSION=6.12.0.182
# Thu, 07 Sep 2023 01:53:30 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 01:53:54 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:91f01557fe0da558070d4f24631c94e91a80877a24621b52b8b13009b62d8d96`  
		Last Modified: Thu, 07 Sep 2023 00:26:44 GMT  
		Size: 27.2 MB (27187385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12132fc81fdf72f5e5905edc96ba6db064fb390345d3f9c4a04b0aa7ff243e17`  
		Last Modified: Thu, 07 Sep 2023 02:01:44 GMT  
		Size: 2.8 MB (2780987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa4cf5e71acb35ad398b3bdf0cb7e63ba3591f8b633a45b2de4cd67d205f009`  
		Last Modified: Thu, 07 Sep 2023 02:01:53 GMT  
		Size: 64.8 MB (64774202 bytes)  
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
$ docker pull mono@sha256:f92793d95509dc30e2d40b85171aece1c5a1aff00d70062e9e2fc646b1a7ead0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48957644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b101a66aff317c6451bacbe4d8db8760c98060d12d5bc238f97322dc5cd418f7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:58:32 GMT
ADD file:fa060a900723a2fce017a38b08be3eb2c27d4768d40c61cd1f6292a7f28a8bdc in / 
# Thu, 07 Sep 2023 00:58:33 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 04:03:37 GMT
ENV MONO_VERSION=6.12.0.182
# Thu, 07 Sep 2023 04:03:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 04:04:15 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7e54f06c680feaf82a31a34e7453d765f332f671cfecacb622c3046561dcc572`  
		Last Modified: Thu, 07 Sep 2023 01:03:53 GMT  
		Size: 22.8 MB (22795752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896cf2b79eb9e448095cab03cb5968875cc5fb527a67d79649025441961efd82`  
		Last Modified: Thu, 07 Sep 2023 04:09:43 GMT  
		Size: 2.4 MB (2370781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a2303b2c37a5342143c8d7bceadf10352b40615dd417f3b04a47a83cde7b61`  
		Last Modified: Thu, 07 Sep 2023 04:09:47 GMT  
		Size: 23.8 MB (23791111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.182-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:6a13402decdc835e814b8a9d08ca232a924b5a436a6e1aceb23980ea7cc0d770
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.2 MB (58158677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1633b0a05c1e8711d19da02dc723dffbef9d8e4d6f7f07b39eb54d46b8d2df0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:08 GMT
ADD file:3521159cdea23e107a3e194ebc9b8f9a6a37ea8188236a267b6ec26e87cf498a in / 
# Thu, 07 Sep 2023 00:40:08 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 07:04:02 GMT
ENV MONO_VERSION=6.12.0.182
# Thu, 07 Sep 2023 07:04:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 07:04:31 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d7cc66d62b738dea27e341b7322194f45ab1be2e548fe11d8ad953d9d56caaa8`  
		Last Modified: Thu, 07 Sep 2023 00:44:18 GMT  
		Size: 26.0 MB (25967748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53037d9952d0efe71a5774348f92d173432e8dbdf95ceb18450c7c07c6c9e9f`  
		Last Modified: Thu, 07 Sep 2023 07:08:07 GMT  
		Size: 2.6 MB (2645888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f85155c32dab21f86975a13ba62dbc5410813df3fcafba56051eec44247a61`  
		Last Modified: Thu, 07 Sep 2023 07:08:10 GMT  
		Size: 29.5 MB (29545041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.182-slim` - linux; 386

```console
$ docker pull mono@sha256:1e331750b2de2f768b2b3359c5cb5ff9d777f02907ae9f9610d1c7bd86c29385
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99439955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dde61adb84e6642ed59730f8251c19a89212a3b608e7905770466bf8ad8b3a45`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:46 GMT
ADD file:e5916da683bdcea27e31e6fbb29e61d1f8457a3bebe4a83278e4f0181e5ac49f in / 
# Thu, 07 Sep 2023 00:39:47 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 20:02:37 GMT
ENV MONO_VERSION=6.12.0.182
# Thu, 07 Sep 2023 20:02:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 20:03:19 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:453c610c7d8be388b9a8559dc654a2def01e71f776e0608ae46db51ae50d10a0`  
		Last Modified: Thu, 07 Sep 2023 00:45:26 GMT  
		Size: 27.8 MB (27846798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d6396be6afdd9df4ac1ad90d0ab9aaef68b9759a6d4ec028aa8c4963970ca3`  
		Last Modified: Thu, 07 Sep 2023 20:07:31 GMT  
		Size: 2.8 MB (2792479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58c12dba60a13a57b5648614b665be3d02ce9e747541083ab284b2a34873e6c`  
		Last Modified: Thu, 07 Sep 2023 20:07:45 GMT  
		Size: 68.8 MB (68800678 bytes)  
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
$ docker pull mono@sha256:465112ebaf92fd33d9560a26e74848a07d18046f50f9c025d3837681f026d172
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
$ docker pull mono@sha256:089c69437f670a34d6d2faa7d15e29f3395a354b8ff3073598e76279cb9ba5d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.7 MB (254674329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f97afc4690efd1650c1d74e46a929a04e32f8d6c731f5958d15ef41826db0f4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:35 GMT
ADD file:9c8b7c79fbbb19d308d151785d178e19bfa7b83257f38d03fa7f30cd41d58530 in / 
# Thu, 07 Sep 2023 00:21:35 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:53:20 GMT
ENV MONO_VERSION=6.12.0.182
# Thu, 07 Sep 2023 01:53:30 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 01:53:54 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 07 Sep 2023 01:55:46 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:91f01557fe0da558070d4f24631c94e91a80877a24621b52b8b13009b62d8d96`  
		Last Modified: Thu, 07 Sep 2023 00:26:44 GMT  
		Size: 27.2 MB (27187385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12132fc81fdf72f5e5905edc96ba6db064fb390345d3f9c4a04b0aa7ff243e17`  
		Last Modified: Thu, 07 Sep 2023 02:01:44 GMT  
		Size: 2.8 MB (2780987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa4cf5e71acb35ad398b3bdf0cb7e63ba3591f8b633a45b2de4cd67d205f009`  
		Last Modified: Thu, 07 Sep 2023 02:01:53 GMT  
		Size: 64.8 MB (64774202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3bf7c27d69e706c535fab335198d46ba19e96cfe916e4116406ad5e1783746c`  
		Last Modified: Thu, 07 Sep 2023 02:02:51 GMT  
		Size: 159.9 MB (159931755 bytes)  
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
$ docker pull mono@sha256:3f2c50251c47c6e8daf7af30af91621870ae8d4bfed30819f452eac8026bbc53
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.0 MB (189021480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a2e8c2751e838c4f926991046e298b87181672c53a47b727e2749fcf1b8f8bb`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:58:32 GMT
ADD file:fa060a900723a2fce017a38b08be3eb2c27d4768d40c61cd1f6292a7f28a8bdc in / 
# Thu, 07 Sep 2023 00:58:33 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 04:03:37 GMT
ENV MONO_VERSION=6.12.0.182
# Thu, 07 Sep 2023 04:03:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 04:04:15 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 07 Sep 2023 04:07:12 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7e54f06c680feaf82a31a34e7453d765f332f671cfecacb622c3046561dcc572`  
		Last Modified: Thu, 07 Sep 2023 01:03:53 GMT  
		Size: 22.8 MB (22795752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896cf2b79eb9e448095cab03cb5968875cc5fb527a67d79649025441961efd82`  
		Last Modified: Thu, 07 Sep 2023 04:09:43 GMT  
		Size: 2.4 MB (2370781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a2303b2c37a5342143c8d7bceadf10352b40615dd417f3b04a47a83cde7b61`  
		Last Modified: Thu, 07 Sep 2023 04:09:47 GMT  
		Size: 23.8 MB (23791111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ef087b8af56f6ad24f17f51ab214d3d95a09c5048d36d54b9d3baa3c3ee8c7`  
		Last Modified: Thu, 07 Sep 2023 04:10:40 GMT  
		Size: 140.1 MB (140063836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:85439cb4fbff445b7a7a5c9857be3eb18a25f0c00ab310ca7597931b9f3357bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.4 MB (216404975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99b3fc85c61b2f9fefe7369de60ce845f2863ba714bb8aef6ff5d23a056af68e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:08 GMT
ADD file:3521159cdea23e107a3e194ebc9b8f9a6a37ea8188236a267b6ec26e87cf498a in / 
# Thu, 07 Sep 2023 00:40:08 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 07:04:02 GMT
ENV MONO_VERSION=6.12.0.182
# Thu, 07 Sep 2023 07:04:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 07:04:31 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 07 Sep 2023 07:06:47 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d7cc66d62b738dea27e341b7322194f45ab1be2e548fe11d8ad953d9d56caaa8`  
		Last Modified: Thu, 07 Sep 2023 00:44:18 GMT  
		Size: 26.0 MB (25967748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53037d9952d0efe71a5774348f92d173432e8dbdf95ceb18450c7c07c6c9e9f`  
		Last Modified: Thu, 07 Sep 2023 07:08:07 GMT  
		Size: 2.6 MB (2645888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f85155c32dab21f86975a13ba62dbc5410813df3fcafba56051eec44247a61`  
		Last Modified: Thu, 07 Sep 2023 07:08:10 GMT  
		Size: 29.5 MB (29545041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54bf7f84fb7a3b3125859753112a10e4bb673ae6d6ee00e235ac568ca6a4d15f`  
		Last Modified: Thu, 07 Sep 2023 07:08:58 GMT  
		Size: 158.2 MB (158246298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; 386

```console
$ docker pull mono@sha256:d914db5bbe9949453c7c8cdb8ef643d53db6a920a0d2f341a8ba6c5119117000
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.6 MB (259560153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1750b1ccddddd0725b37eccca344d9e8b827165b132275486ab1908759b2b4ca`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:46 GMT
ADD file:e5916da683bdcea27e31e6fbb29e61d1f8457a3bebe4a83278e4f0181e5ac49f in / 
# Thu, 07 Sep 2023 00:39:47 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 20:02:37 GMT
ENV MONO_VERSION=6.12.0.182
# Thu, 07 Sep 2023 20:02:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 20:03:19 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 07 Sep 2023 20:05:40 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:453c610c7d8be388b9a8559dc654a2def01e71f776e0608ae46db51ae50d10a0`  
		Last Modified: Thu, 07 Sep 2023 00:45:26 GMT  
		Size: 27.8 MB (27846798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d6396be6afdd9df4ac1ad90d0ab9aaef68b9759a6d4ec028aa8c4963970ca3`  
		Last Modified: Thu, 07 Sep 2023 20:07:31 GMT  
		Size: 2.8 MB (2792479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58c12dba60a13a57b5648614b665be3d02ce9e747541083ab284b2a34873e6c`  
		Last Modified: Thu, 07 Sep 2023 20:07:45 GMT  
		Size: 68.8 MB (68800678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45574f7922a18c136182a845a84aa83dbaa55b270403803504630217c6dc1223`  
		Last Modified: Thu, 07 Sep 2023 20:09:11 GMT  
		Size: 160.1 MB (160120198 bytes)  
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
$ docker pull mono@sha256:4ac0e6a9361a55b14456a63130b931ea563ab6281f8bede836d29892544554b8
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
$ docker pull mono@sha256:84cc79f2e8be438c04f8eade849b8757727be784faca8efa67f7e1c38ea24633
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94742574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdb686b94af3d0fe092a2df584b75557331d28d1de5050abbd456bba31475781`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:35 GMT
ADD file:9c8b7c79fbbb19d308d151785d178e19bfa7b83257f38d03fa7f30cd41d58530 in / 
# Thu, 07 Sep 2023 00:21:35 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:53:20 GMT
ENV MONO_VERSION=6.12.0.182
# Thu, 07 Sep 2023 01:53:30 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 01:53:54 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:91f01557fe0da558070d4f24631c94e91a80877a24621b52b8b13009b62d8d96`  
		Last Modified: Thu, 07 Sep 2023 00:26:44 GMT  
		Size: 27.2 MB (27187385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12132fc81fdf72f5e5905edc96ba6db064fb390345d3f9c4a04b0aa7ff243e17`  
		Last Modified: Thu, 07 Sep 2023 02:01:44 GMT  
		Size: 2.8 MB (2780987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa4cf5e71acb35ad398b3bdf0cb7e63ba3591f8b633a45b2de4cd67d205f009`  
		Last Modified: Thu, 07 Sep 2023 02:01:53 GMT  
		Size: 64.8 MB (64774202 bytes)  
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
$ docker pull mono@sha256:f92793d95509dc30e2d40b85171aece1c5a1aff00d70062e9e2fc646b1a7ead0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48957644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b101a66aff317c6451bacbe4d8db8760c98060d12d5bc238f97322dc5cd418f7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:58:32 GMT
ADD file:fa060a900723a2fce017a38b08be3eb2c27d4768d40c61cd1f6292a7f28a8bdc in / 
# Thu, 07 Sep 2023 00:58:33 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 04:03:37 GMT
ENV MONO_VERSION=6.12.0.182
# Thu, 07 Sep 2023 04:03:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 04:04:15 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7e54f06c680feaf82a31a34e7453d765f332f671cfecacb622c3046561dcc572`  
		Last Modified: Thu, 07 Sep 2023 01:03:53 GMT  
		Size: 22.8 MB (22795752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896cf2b79eb9e448095cab03cb5968875cc5fb527a67d79649025441961efd82`  
		Last Modified: Thu, 07 Sep 2023 04:09:43 GMT  
		Size: 2.4 MB (2370781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a2303b2c37a5342143c8d7bceadf10352b40615dd417f3b04a47a83cde7b61`  
		Last Modified: Thu, 07 Sep 2023 04:09:47 GMT  
		Size: 23.8 MB (23791111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:6a13402decdc835e814b8a9d08ca232a924b5a436a6e1aceb23980ea7cc0d770
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.2 MB (58158677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1633b0a05c1e8711d19da02dc723dffbef9d8e4d6f7f07b39eb54d46b8d2df0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:08 GMT
ADD file:3521159cdea23e107a3e194ebc9b8f9a6a37ea8188236a267b6ec26e87cf498a in / 
# Thu, 07 Sep 2023 00:40:08 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 07:04:02 GMT
ENV MONO_VERSION=6.12.0.182
# Thu, 07 Sep 2023 07:04:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 07:04:31 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d7cc66d62b738dea27e341b7322194f45ab1be2e548fe11d8ad953d9d56caaa8`  
		Last Modified: Thu, 07 Sep 2023 00:44:18 GMT  
		Size: 26.0 MB (25967748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53037d9952d0efe71a5774348f92d173432e8dbdf95ceb18450c7c07c6c9e9f`  
		Last Modified: Thu, 07 Sep 2023 07:08:07 GMT  
		Size: 2.6 MB (2645888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f85155c32dab21f86975a13ba62dbc5410813df3fcafba56051eec44247a61`  
		Last Modified: Thu, 07 Sep 2023 07:08:10 GMT  
		Size: 29.5 MB (29545041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; 386

```console
$ docker pull mono@sha256:1e331750b2de2f768b2b3359c5cb5ff9d777f02907ae9f9610d1c7bd86c29385
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99439955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dde61adb84e6642ed59730f8251c19a89212a3b608e7905770466bf8ad8b3a45`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:46 GMT
ADD file:e5916da683bdcea27e31e6fbb29e61d1f8457a3bebe4a83278e4f0181e5ac49f in / 
# Thu, 07 Sep 2023 00:39:47 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 20:02:37 GMT
ENV MONO_VERSION=6.12.0.182
# Thu, 07 Sep 2023 20:02:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 07 Sep 2023 20:03:19 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:453c610c7d8be388b9a8559dc654a2def01e71f776e0608ae46db51ae50d10a0`  
		Last Modified: Thu, 07 Sep 2023 00:45:26 GMT  
		Size: 27.8 MB (27846798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d6396be6afdd9df4ac1ad90d0ab9aaef68b9759a6d4ec028aa8c4963970ca3`  
		Last Modified: Thu, 07 Sep 2023 20:07:31 GMT  
		Size: 2.8 MB (2792479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58c12dba60a13a57b5648614b665be3d02ce9e747541083ab284b2a34873e6c`  
		Last Modified: Thu, 07 Sep 2023 20:07:45 GMT  
		Size: 68.8 MB (68800678 bytes)  
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
