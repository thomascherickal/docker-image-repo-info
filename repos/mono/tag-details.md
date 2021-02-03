<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mono`

-	[`mono:6`](#mono6)
-	[`mono:6.10`](#mono610)
-	[`mono:6.10.0`](#mono6100)
-	[`mono:6.10.0.104`](#mono6100104)
-	[`mono:6.10.0.104-slim`](#mono6100104-slim)
-	[`mono:6.10.0-slim`](#mono6100-slim)
-	[`mono:6.10-slim`](#mono610-slim)
-	[`mono:6.12`](#mono612)
-	[`mono:6.12.0`](#mono6120)
-	[`mono:6.12.0.107`](#mono6120107)
-	[`mono:6.12.0.107-slim`](#mono6120107-slim)
-	[`mono:6.12.0-slim`](#mono6120-slim)
-	[`mono:6.12-slim`](#mono612-slim)
-	[`mono:6-slim`](#mono6-slim)
-	[`mono:latest`](#monolatest)
-	[`mono:slim`](#monoslim)

## `mono:6`

```console
$ docker pull mono@sha256:fee59facbee3c69f535f506910bbac808643a8f91f5a80ddc79e478fa5982f58
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
$ docker pull mono@sha256:e3c3faa1e0eccfec442341c7260bfb1faeccf40581fe8a00e77e794cf27d150b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.9 MB (235856726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d02da61afa912e62ef7cdc2e3b89fb6915716c72eccd75293b5c784ba17e5ce`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:40:56 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 09:41:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 09:41:33 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 09:48:29 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe02677df6f8831edfcea8a4558dcbb344dda0a234033ce403a445f71bb95e04`  
		Last Modified: Tue, 12 Jan 2021 09:56:50 GMT  
		Size: 255.9 KB (255924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6f0c1d36d945478bb94f4061ab9e9570a42d064b1bac55d482cc3d9eefdc1b`  
		Last Modified: Tue, 12 Jan 2021 09:57:04 GMT  
		Size: 67.1 MB (67079218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55acb8a81f9716f19bc8b425a4f2f9778868a086ced2c38a0d232c7e149e260b`  
		Last Modified: Tue, 12 Jan 2021 09:58:10 GMT  
		Size: 141.4 MB (141413515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; arm variant v5

```console
$ docker pull mono@sha256:93e07bd0966ba3af8e1265a2976fa87cf142485c7984e221d5bd1900b1129c04
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.7 MB (191715473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d675a592f2dd1ff1c3d27b04a2e5373c8d8d9fd42ea3e202cf2f0deeabc4a11b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:51:34 GMT
ADD file:57136a762436a5d41e60c61db0d89baea17a289845ea55565e45cc79a9e81e23 in / 
# Tue, 12 Jan 2021 00:51:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:58:10 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 01:58:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 01:59:18 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 02:04:03 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2e2535e18472e7491a1d935b1f44ac842e4cc5c4d3de40cecb77b56b44515910`  
		Last Modified: Tue, 12 Jan 2021 01:00:19 GMT  
		Size: 24.9 MB (24851909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781b0df29588b1d712497221b09542f9b882364892a46ecf5521b50115ffe045`  
		Last Modified: Tue, 12 Jan 2021 02:07:54 GMT  
		Size: 255.9 KB (255947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ccd7e036e1bf04d2229ab088bc370548d6b63d0540abdfa03ab614ff643669e`  
		Last Modified: Tue, 12 Jan 2021 02:08:01 GMT  
		Size: 26.5 MB (26499381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057e315d7d334759ab98965930ff1540b0ca7c9ae700b6bbb74fa1506fed258a`  
		Last Modified: Tue, 12 Jan 2021 02:09:34 GMT  
		Size: 140.1 MB (140108236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; arm variant v7

```console
$ docker pull mono@sha256:172236fea866d1b739364ba9049c97abc885743e420322f6df0dd72c617ab1d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.6 MB (187612230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f579c6e6d6132fc34dcf39db01f217918a65e0cf5889c53e939eb89bd3453d13`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:01:09 GMT
ADD file:1db27e410cc7caf4a97a7313c57260fd01aa134b84306914ef0948dcca27372d in / 
# Tue, 12 Jan 2021 00:01:12 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:53:47 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 03:54:04 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:54:42 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 03:58:38 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:be493c6a598447fe5f46a390f3bee10f2d2ba2215d39829fe84eb40a7add18fc`  
		Last Modified: Tue, 12 Jan 2021 00:11:14 GMT  
		Size: 22.7 MB (22715905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c33bdc53ec4d57ecf8d4565fca28d67f043f4855d49b01e900e8ef3c8bb9d6`  
		Last Modified: Tue, 12 Jan 2021 04:03:03 GMT  
		Size: 255.9 KB (255942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d9304eb6e55e2cd3920831bd0dec33588ea625b97a60aa2b06301f9351de819`  
		Last Modified: Tue, 12 Jan 2021 04:03:11 GMT  
		Size: 25.7 MB (25697506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1168b3f3ae6bc53dbe989dc4db4fad0b76b83fcb4d4db9dd33f685342c886c`  
		Last Modified: Tue, 12 Jan 2021 04:04:41 GMT  
		Size: 138.9 MB (138942877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:bb8bcb03c776a1d69c8402a77aeb49e7302fca102ab82e11002ca319287ae33a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.4 MB (214424611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a8b3b0d88c8a2f9826ad928f5035cd23a14395c38e57da6f376205bb25ac8d2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:41:13 GMT
ADD file:0252dccbbfb76766e0e189783d38f6a6afd13f44daa7c5370ffd094adea0f583 in / 
# Tue, 12 Jan 2021 00:41:21 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 05:07:35 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 05:07:52 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 05:08:28 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 05:12:14 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f8be76fcf2062bd14a3a78f858da701db8bcd907a2d0f33716d89d9329df2b1f`  
		Last Modified: Tue, 12 Jan 2021 00:51:54 GMT  
		Size: 25.9 MB (25864492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c624bef28ff9228422eef122ec713693eb2e8d2ed78aa41f319bd0678a607c`  
		Last Modified: Tue, 12 Jan 2021 05:15:20 GMT  
		Size: 255.9 KB (255923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ec950da6523b4cb54939edc61c6460d64327528adc05f607fbf005ff508a88`  
		Last Modified: Tue, 12 Jan 2021 05:15:34 GMT  
		Size: 31.7 MB (31720550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0470c4fa675956b4e41164ba69e70c7c53cbf56fa1fde6ca99247fd30d63182`  
		Last Modified: Tue, 12 Jan 2021 05:16:54 GMT  
		Size: 156.6 MB (156583646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; 386

```console
$ docker pull mono@sha256:3f6d7e510f3c7e210af3336de41288b7e8971519c559d7994389b5aaab7ca0d6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.6 MB (241641989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d7d8ae0005ba40c7547dfff94755167dba0e74f722bd8583e10d292d8cc13d2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:55:14 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 03:55:23 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:56:00 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 03:59:02 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ae7e24292b47c5c54d019f27f833b4d1fd06c6c1760426a915f4626d13ebb5`  
		Last Modified: Tue, 12 Jan 2021 04:01:42 GMT  
		Size: 255.9 KB (255867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723f6fae6c251aafe4f2903014f5ca67d695cd2f74f87cc46b0b9b5e50650a9f`  
		Last Modified: Tue, 12 Jan 2021 04:02:03 GMT  
		Size: 71.1 MB (71105792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a6a59d3738ce8d2e6bad95e51859928eac584152411a872b1dfd4ec6cbffe4`  
		Last Modified: Tue, 12 Jan 2021 04:03:29 GMT  
		Size: 142.5 MB (142512339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; ppc64le

```console
$ docker pull mono@sha256:8cd03e8a315754c3631020ef221a2d0cbd0992577901c899c47ce5e69d61dd49
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.3 MB (203325644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be23bd3cc106fdd913dd4eff53c1f46dabb535e753abef0f566dae2c69eaea9d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:25:06 GMT
ADD file:9d7252c169da9a089a0caa2f26cea24678267c15c0e129e7320d4defe0d4637b in / 
# Tue, 12 Jan 2021 00:25:16 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:34:09 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 03:35:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:37:38 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 03:52:04 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:cb701c1e59a3b25dcb09b089f31d61af3065659cd29a7c748f66f3e3c8a96d58`  
		Last Modified: Tue, 12 Jan 2021 00:34:11 GMT  
		Size: 30.5 MB (30532837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e77824b16d99ee079aa03b8aabec031637265f7380c082326eaf48d078a93e7`  
		Last Modified: Tue, 12 Jan 2021 04:01:02 GMT  
		Size: 256.1 KB (256146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8e3bf2452dcba3a8621830f987ddbcc051bd5b6d5817e6d595c1cd93497f67`  
		Last Modified: Tue, 12 Jan 2021 04:01:08 GMT  
		Size: 29.3 MB (29311088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be798b1b9507d975e13d056b87d688839b0f83115176be62486731bf9cac3ed7`  
		Last Modified: Tue, 12 Jan 2021 04:02:25 GMT  
		Size: 143.2 MB (143225573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10`

```console
$ docker pull mono@sha256:475ab0ab2b7c6aba62a508982bcad7f1fbb8b1efe08450ab9a50f979b4070985
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
$ docker pull mono@sha256:4310626243c7cb039164506a632955ff6f88b33d9cd7ca81821248f14134bd92
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.7 MB (224747979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c04af7238369a5f5f0c473aad5bff633bea9a4d1b45ac888947f38d34d19bd0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:41:43 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 12 Jan 2021 09:41:50 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 09:42:22 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 09:56:24 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e54505e49395a0d6a43f271952bf307a05153f6510a80ae27038c50df0efa46`  
		Last Modified: Tue, 12 Jan 2021 09:57:16 GMT  
		Size: 255.9 KB (255924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187e7566eb41f21ec1afcdd35f44280fdc2057d58a74789bd9affda7da2084a4`  
		Last Modified: Tue, 12 Jan 2021 09:57:29 GMT  
		Size: 67.1 MB (67092827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:045d12fef3a002ecc26a8a290b60da3b7e004e0102ad78ea21be87c04ea4b331`  
		Last Modified: Tue, 12 Jan 2021 09:58:59 GMT  
		Size: 130.3 MB (130291159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; arm variant v5

```console
$ docker pull mono@sha256:c2d6eb605b7d09f4aa4ec06f825d82ea9d365df1fa69e690b4b6bc18fde21a8a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180601054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9e842cf0b335d70c2e19cb5a353a4f4448d8df4e0fc519ea38a10cff676eb60`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:51:34 GMT
ADD file:57136a762436a5d41e60c61db0d89baea17a289845ea55565e45cc79a9e81e23 in / 
# Tue, 12 Jan 2021 00:51:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:59:29 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 12 Jan 2021 01:59:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 02:00:51 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 02:07:11 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2e2535e18472e7491a1d935b1f44ac842e4cc5c4d3de40cecb77b56b44515910`  
		Last Modified: Tue, 12 Jan 2021 01:00:19 GMT  
		Size: 24.9 MB (24851909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc75979d12aa60a81b3a6594a6f4d26e2bdd6261e0ca573176aebc974404f41`  
		Last Modified: Tue, 12 Jan 2021 02:08:19 GMT  
		Size: 256.0 KB (255959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce86ffd97c996edf2f5f32f5b54a3724e5fa9455e589ca9ff57e1fdc85117a28`  
		Last Modified: Tue, 12 Jan 2021 02:08:34 GMT  
		Size: 26.5 MB (26531461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8210b5a932249d8515d0c2e694cd0a1d59f177bc7a7ec1d1b7e5a3a262990ca8`  
		Last Modified: Tue, 12 Jan 2021 02:10:38 GMT  
		Size: 129.0 MB (128961725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; arm variant v7

```console
$ docker pull mono@sha256:a7c76747cab342ff93088965fadbb9835cb549f7d60ab322235df5c3141ddd2e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.5 MB (176516036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8168fd7bcf107028225551cfe3d3d6a7d5b37f4313f093505efa41e3f9ddb904`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:01:09 GMT
ADD file:1db27e410cc7caf4a97a7313c57260fd01aa134b84306914ef0948dcca27372d in / 
# Tue, 12 Jan 2021 00:01:12 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:54:53 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 12 Jan 2021 03:55:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:55:53 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 04:02:12 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:be493c6a598447fe5f46a390f3bee10f2d2ba2215d39829fe84eb40a7add18fc`  
		Last Modified: Tue, 12 Jan 2021 00:11:14 GMT  
		Size: 22.7 MB (22715905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae41c04538a5197d9ce78432fa39191029ba0de2e0c89683471ee6a3599bbc9`  
		Last Modified: Tue, 12 Jan 2021 04:03:26 GMT  
		Size: 255.9 KB (255917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1677a1ffb68e5ae64625415689b4a2ff66f49acec6ae83b19f7834c082e4ff9`  
		Last Modified: Tue, 12 Jan 2021 04:03:35 GMT  
		Size: 25.7 MB (25729576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac8aed1725d65219c05b6cea8e50daee97b103ed762cf005af2c6aeae7f221`  
		Last Modified: Tue, 12 Jan 2021 04:05:48 GMT  
		Size: 127.8 MB (127814638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:cb1208b1b962d03ac3d2de8aa234bd08e1f8586a273ace18118ea9915b28a088
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.3 MB (203319469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da43b28377f75813f7cfcf7e574e53c7a3e8ed73f7cf24058c27d860e10db29e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:41:13 GMT
ADD file:0252dccbbfb76766e0e189783d38f6a6afd13f44daa7c5370ffd094adea0f583 in / 
# Tue, 12 Jan 2021 00:41:21 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 05:08:43 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 12 Jan 2021 05:08:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 05:09:36 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 05:14:35 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f8be76fcf2062bd14a3a78f858da701db8bcd907a2d0f33716d89d9329df2b1f`  
		Last Modified: Tue, 12 Jan 2021 00:51:54 GMT  
		Size: 25.9 MB (25864492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6179e732b6b6a778fbe4321833a5ba71f60a206504e6a1a93efe345ec9aedf3e`  
		Last Modified: Tue, 12 Jan 2021 05:15:48 GMT  
		Size: 255.9 KB (255937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79964378e1ae7824bc19481d96933ec96cd27ade28c334215d53bafbab3e5d53`  
		Last Modified: Tue, 12 Jan 2021 05:15:59 GMT  
		Size: 31.7 MB (31749798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6950b481095c08dd42a719f4427100df6a0eb94de69f3c82e5aa3f666570601d`  
		Last Modified: Tue, 12 Jan 2021 05:17:57 GMT  
		Size: 145.4 MB (145449242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; 386

```console
$ docker pull mono@sha256:53975b45852e0214be6a8f7a4451adad23a40b2457fd5c40e7239ad2dfa47dc8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.6 MB (230551724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e3e85181b4a6d18083325fd95e4472863ede71e1b0857650c9621564e9a3e98`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:56:09 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 12 Jan 2021 03:56:18 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:56:56 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 04:01:14 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae604efc877a26d5e9ef47c0ce73f76fc847780ddc3fc4f4fa2dae62aebc1b79`  
		Last Modified: Tue, 12 Jan 2021 04:02:20 GMT  
		Size: 255.8 KB (255850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb5562f2f87a9508fba6e611a28b8bc7747b5368845e5cfa71f1a25a457f2c1e`  
		Last Modified: Tue, 12 Jan 2021 04:02:42 GMT  
		Size: 71.1 MB (71136255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10581e73388ee9a7aa52a53d415eaa9b6ecc1a57fb2426de84e028895c80d7aa`  
		Last Modified: Tue, 12 Jan 2021 04:04:16 GMT  
		Size: 131.4 MB (131391628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10` - linux; ppc64le

```console
$ docker pull mono@sha256:582dd336e9dfac08b00f63738182f127e766f6e207a3914f47c35a44ca9c1f20
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.1 MB (192117601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eae166434ad1e239a83259bd86e49e76bc0f5aa0071cef7683034da040d80b53`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:25:06 GMT
ADD file:9d7252c169da9a089a0caa2f26cea24678267c15c0e129e7320d4defe0d4637b in / 
# Tue, 12 Jan 2021 00:25:16 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:37:52 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 12 Jan 2021 03:39:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:41:49 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 04:00:12 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:cb701c1e59a3b25dcb09b089f31d61af3065659cd29a7c748f66f3e3c8a96d58`  
		Last Modified: Tue, 12 Jan 2021 00:34:11 GMT  
		Size: 30.5 MB (30532837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a6b5cd501f71da14d37bddd625494e7a2de28217c260bc74553a9b4bc12b0f`  
		Last Modified: Tue, 12 Jan 2021 04:01:26 GMT  
		Size: 256.3 KB (256256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e85b5bce279ec9104f3a75e8c3a74fbd322ee4fff6244ab3046f12df7348d2a`  
		Last Modified: Tue, 12 Jan 2021 04:01:38 GMT  
		Size: 29.4 MB (29350170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ab9db45435abc9c30283f6ff37a0801fe81b852dca5ecad333bd338711bf55`  
		Last Modified: Tue, 12 Jan 2021 04:03:22 GMT  
		Size: 132.0 MB (131978338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10.0`

```console
$ docker pull mono@sha256:475ab0ab2b7c6aba62a508982bcad7f1fbb8b1efe08450ab9a50f979b4070985
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
$ docker pull mono@sha256:4310626243c7cb039164506a632955ff6f88b33d9cd7ca81821248f14134bd92
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.7 MB (224747979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c04af7238369a5f5f0c473aad5bff633bea9a4d1b45ac888947f38d34d19bd0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:41:43 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 12 Jan 2021 09:41:50 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 09:42:22 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 09:56:24 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e54505e49395a0d6a43f271952bf307a05153f6510a80ae27038c50df0efa46`  
		Last Modified: Tue, 12 Jan 2021 09:57:16 GMT  
		Size: 255.9 KB (255924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187e7566eb41f21ec1afcdd35f44280fdc2057d58a74789bd9affda7da2084a4`  
		Last Modified: Tue, 12 Jan 2021 09:57:29 GMT  
		Size: 67.1 MB (67092827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:045d12fef3a002ecc26a8a290b60da3b7e004e0102ad78ea21be87c04ea4b331`  
		Last Modified: Tue, 12 Jan 2021 09:58:59 GMT  
		Size: 130.3 MB (130291159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; arm variant v5

```console
$ docker pull mono@sha256:c2d6eb605b7d09f4aa4ec06f825d82ea9d365df1fa69e690b4b6bc18fde21a8a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180601054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9e842cf0b335d70c2e19cb5a353a4f4448d8df4e0fc519ea38a10cff676eb60`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:51:34 GMT
ADD file:57136a762436a5d41e60c61db0d89baea17a289845ea55565e45cc79a9e81e23 in / 
# Tue, 12 Jan 2021 00:51:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:59:29 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 12 Jan 2021 01:59:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 02:00:51 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 02:07:11 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2e2535e18472e7491a1d935b1f44ac842e4cc5c4d3de40cecb77b56b44515910`  
		Last Modified: Tue, 12 Jan 2021 01:00:19 GMT  
		Size: 24.9 MB (24851909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc75979d12aa60a81b3a6594a6f4d26e2bdd6261e0ca573176aebc974404f41`  
		Last Modified: Tue, 12 Jan 2021 02:08:19 GMT  
		Size: 256.0 KB (255959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce86ffd97c996edf2f5f32f5b54a3724e5fa9455e589ca9ff57e1fdc85117a28`  
		Last Modified: Tue, 12 Jan 2021 02:08:34 GMT  
		Size: 26.5 MB (26531461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8210b5a932249d8515d0c2e694cd0a1d59f177bc7a7ec1d1b7e5a3a262990ca8`  
		Last Modified: Tue, 12 Jan 2021 02:10:38 GMT  
		Size: 129.0 MB (128961725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; arm variant v7

```console
$ docker pull mono@sha256:a7c76747cab342ff93088965fadbb9835cb549f7d60ab322235df5c3141ddd2e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.5 MB (176516036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8168fd7bcf107028225551cfe3d3d6a7d5b37f4313f093505efa41e3f9ddb904`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:01:09 GMT
ADD file:1db27e410cc7caf4a97a7313c57260fd01aa134b84306914ef0948dcca27372d in / 
# Tue, 12 Jan 2021 00:01:12 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:54:53 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 12 Jan 2021 03:55:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:55:53 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 04:02:12 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:be493c6a598447fe5f46a390f3bee10f2d2ba2215d39829fe84eb40a7add18fc`  
		Last Modified: Tue, 12 Jan 2021 00:11:14 GMT  
		Size: 22.7 MB (22715905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae41c04538a5197d9ce78432fa39191029ba0de2e0c89683471ee6a3599bbc9`  
		Last Modified: Tue, 12 Jan 2021 04:03:26 GMT  
		Size: 255.9 KB (255917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1677a1ffb68e5ae64625415689b4a2ff66f49acec6ae83b19f7834c082e4ff9`  
		Last Modified: Tue, 12 Jan 2021 04:03:35 GMT  
		Size: 25.7 MB (25729576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac8aed1725d65219c05b6cea8e50daee97b103ed762cf005af2c6aeae7f221`  
		Last Modified: Tue, 12 Jan 2021 04:05:48 GMT  
		Size: 127.8 MB (127814638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:cb1208b1b962d03ac3d2de8aa234bd08e1f8586a273ace18118ea9915b28a088
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.3 MB (203319469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da43b28377f75813f7cfcf7e574e53c7a3e8ed73f7cf24058c27d860e10db29e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:41:13 GMT
ADD file:0252dccbbfb76766e0e189783d38f6a6afd13f44daa7c5370ffd094adea0f583 in / 
# Tue, 12 Jan 2021 00:41:21 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 05:08:43 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 12 Jan 2021 05:08:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 05:09:36 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 05:14:35 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f8be76fcf2062bd14a3a78f858da701db8bcd907a2d0f33716d89d9329df2b1f`  
		Last Modified: Tue, 12 Jan 2021 00:51:54 GMT  
		Size: 25.9 MB (25864492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6179e732b6b6a778fbe4321833a5ba71f60a206504e6a1a93efe345ec9aedf3e`  
		Last Modified: Tue, 12 Jan 2021 05:15:48 GMT  
		Size: 255.9 KB (255937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79964378e1ae7824bc19481d96933ec96cd27ade28c334215d53bafbab3e5d53`  
		Last Modified: Tue, 12 Jan 2021 05:15:59 GMT  
		Size: 31.7 MB (31749798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6950b481095c08dd42a719f4427100df6a0eb94de69f3c82e5aa3f666570601d`  
		Last Modified: Tue, 12 Jan 2021 05:17:57 GMT  
		Size: 145.4 MB (145449242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; 386

```console
$ docker pull mono@sha256:53975b45852e0214be6a8f7a4451adad23a40b2457fd5c40e7239ad2dfa47dc8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.6 MB (230551724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e3e85181b4a6d18083325fd95e4472863ede71e1b0857650c9621564e9a3e98`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:56:09 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 12 Jan 2021 03:56:18 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:56:56 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 04:01:14 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae604efc877a26d5e9ef47c0ce73f76fc847780ddc3fc4f4fa2dae62aebc1b79`  
		Last Modified: Tue, 12 Jan 2021 04:02:20 GMT  
		Size: 255.8 KB (255850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb5562f2f87a9508fba6e611a28b8bc7747b5368845e5cfa71f1a25a457f2c1e`  
		Last Modified: Tue, 12 Jan 2021 04:02:42 GMT  
		Size: 71.1 MB (71136255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10581e73388ee9a7aa52a53d415eaa9b6ecc1a57fb2426de84e028895c80d7aa`  
		Last Modified: Tue, 12 Jan 2021 04:04:16 GMT  
		Size: 131.4 MB (131391628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0` - linux; ppc64le

```console
$ docker pull mono@sha256:582dd336e9dfac08b00f63738182f127e766f6e207a3914f47c35a44ca9c1f20
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.1 MB (192117601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eae166434ad1e239a83259bd86e49e76bc0f5aa0071cef7683034da040d80b53`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:25:06 GMT
ADD file:9d7252c169da9a089a0caa2f26cea24678267c15c0e129e7320d4defe0d4637b in / 
# Tue, 12 Jan 2021 00:25:16 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:37:52 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 12 Jan 2021 03:39:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:41:49 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 04:00:12 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:cb701c1e59a3b25dcb09b089f31d61af3065659cd29a7c748f66f3e3c8a96d58`  
		Last Modified: Tue, 12 Jan 2021 00:34:11 GMT  
		Size: 30.5 MB (30532837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a6b5cd501f71da14d37bddd625494e7a2de28217c260bc74553a9b4bc12b0f`  
		Last Modified: Tue, 12 Jan 2021 04:01:26 GMT  
		Size: 256.3 KB (256256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e85b5bce279ec9104f3a75e8c3a74fbd322ee4fff6244ab3046f12df7348d2a`  
		Last Modified: Tue, 12 Jan 2021 04:01:38 GMT  
		Size: 29.4 MB (29350170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ab9db45435abc9c30283f6ff37a0801fe81b852dca5ecad333bd338711bf55`  
		Last Modified: Tue, 12 Jan 2021 04:03:22 GMT  
		Size: 132.0 MB (131978338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10.0.104`

```console
$ docker pull mono@sha256:475ab0ab2b7c6aba62a508982bcad7f1fbb8b1efe08450ab9a50f979b4070985
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
$ docker pull mono@sha256:4310626243c7cb039164506a632955ff6f88b33d9cd7ca81821248f14134bd92
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.7 MB (224747979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c04af7238369a5f5f0c473aad5bff633bea9a4d1b45ac888947f38d34d19bd0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:41:43 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 12 Jan 2021 09:41:50 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 09:42:22 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 09:56:24 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e54505e49395a0d6a43f271952bf307a05153f6510a80ae27038c50df0efa46`  
		Last Modified: Tue, 12 Jan 2021 09:57:16 GMT  
		Size: 255.9 KB (255924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187e7566eb41f21ec1afcdd35f44280fdc2057d58a74789bd9affda7da2084a4`  
		Last Modified: Tue, 12 Jan 2021 09:57:29 GMT  
		Size: 67.1 MB (67092827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:045d12fef3a002ecc26a8a290b60da3b7e004e0102ad78ea21be87c04ea4b331`  
		Last Modified: Tue, 12 Jan 2021 09:58:59 GMT  
		Size: 130.3 MB (130291159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; arm variant v5

```console
$ docker pull mono@sha256:c2d6eb605b7d09f4aa4ec06f825d82ea9d365df1fa69e690b4b6bc18fde21a8a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180601054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9e842cf0b335d70c2e19cb5a353a4f4448d8df4e0fc519ea38a10cff676eb60`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:51:34 GMT
ADD file:57136a762436a5d41e60c61db0d89baea17a289845ea55565e45cc79a9e81e23 in / 
# Tue, 12 Jan 2021 00:51:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:59:29 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 12 Jan 2021 01:59:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 02:00:51 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 02:07:11 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2e2535e18472e7491a1d935b1f44ac842e4cc5c4d3de40cecb77b56b44515910`  
		Last Modified: Tue, 12 Jan 2021 01:00:19 GMT  
		Size: 24.9 MB (24851909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc75979d12aa60a81b3a6594a6f4d26e2bdd6261e0ca573176aebc974404f41`  
		Last Modified: Tue, 12 Jan 2021 02:08:19 GMT  
		Size: 256.0 KB (255959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce86ffd97c996edf2f5f32f5b54a3724e5fa9455e589ca9ff57e1fdc85117a28`  
		Last Modified: Tue, 12 Jan 2021 02:08:34 GMT  
		Size: 26.5 MB (26531461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8210b5a932249d8515d0c2e694cd0a1d59f177bc7a7ec1d1b7e5a3a262990ca8`  
		Last Modified: Tue, 12 Jan 2021 02:10:38 GMT  
		Size: 129.0 MB (128961725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; arm variant v7

```console
$ docker pull mono@sha256:a7c76747cab342ff93088965fadbb9835cb549f7d60ab322235df5c3141ddd2e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.5 MB (176516036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8168fd7bcf107028225551cfe3d3d6a7d5b37f4313f093505efa41e3f9ddb904`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:01:09 GMT
ADD file:1db27e410cc7caf4a97a7313c57260fd01aa134b84306914ef0948dcca27372d in / 
# Tue, 12 Jan 2021 00:01:12 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:54:53 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 12 Jan 2021 03:55:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:55:53 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 04:02:12 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:be493c6a598447fe5f46a390f3bee10f2d2ba2215d39829fe84eb40a7add18fc`  
		Last Modified: Tue, 12 Jan 2021 00:11:14 GMT  
		Size: 22.7 MB (22715905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae41c04538a5197d9ce78432fa39191029ba0de2e0c89683471ee6a3599bbc9`  
		Last Modified: Tue, 12 Jan 2021 04:03:26 GMT  
		Size: 255.9 KB (255917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1677a1ffb68e5ae64625415689b4a2ff66f49acec6ae83b19f7834c082e4ff9`  
		Last Modified: Tue, 12 Jan 2021 04:03:35 GMT  
		Size: 25.7 MB (25729576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac8aed1725d65219c05b6cea8e50daee97b103ed762cf005af2c6aeae7f221`  
		Last Modified: Tue, 12 Jan 2021 04:05:48 GMT  
		Size: 127.8 MB (127814638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:cb1208b1b962d03ac3d2de8aa234bd08e1f8586a273ace18118ea9915b28a088
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.3 MB (203319469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da43b28377f75813f7cfcf7e574e53c7a3e8ed73f7cf24058c27d860e10db29e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:41:13 GMT
ADD file:0252dccbbfb76766e0e189783d38f6a6afd13f44daa7c5370ffd094adea0f583 in / 
# Tue, 12 Jan 2021 00:41:21 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 05:08:43 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 12 Jan 2021 05:08:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 05:09:36 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 05:14:35 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f8be76fcf2062bd14a3a78f858da701db8bcd907a2d0f33716d89d9329df2b1f`  
		Last Modified: Tue, 12 Jan 2021 00:51:54 GMT  
		Size: 25.9 MB (25864492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6179e732b6b6a778fbe4321833a5ba71f60a206504e6a1a93efe345ec9aedf3e`  
		Last Modified: Tue, 12 Jan 2021 05:15:48 GMT  
		Size: 255.9 KB (255937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79964378e1ae7824bc19481d96933ec96cd27ade28c334215d53bafbab3e5d53`  
		Last Modified: Tue, 12 Jan 2021 05:15:59 GMT  
		Size: 31.7 MB (31749798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6950b481095c08dd42a719f4427100df6a0eb94de69f3c82e5aa3f666570601d`  
		Last Modified: Tue, 12 Jan 2021 05:17:57 GMT  
		Size: 145.4 MB (145449242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; 386

```console
$ docker pull mono@sha256:53975b45852e0214be6a8f7a4451adad23a40b2457fd5c40e7239ad2dfa47dc8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.6 MB (230551724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e3e85181b4a6d18083325fd95e4472863ede71e1b0857650c9621564e9a3e98`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:56:09 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 12 Jan 2021 03:56:18 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:56:56 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 04:01:14 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae604efc877a26d5e9ef47c0ce73f76fc847780ddc3fc4f4fa2dae62aebc1b79`  
		Last Modified: Tue, 12 Jan 2021 04:02:20 GMT  
		Size: 255.8 KB (255850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb5562f2f87a9508fba6e611a28b8bc7747b5368845e5cfa71f1a25a457f2c1e`  
		Last Modified: Tue, 12 Jan 2021 04:02:42 GMT  
		Size: 71.1 MB (71136255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10581e73388ee9a7aa52a53d415eaa9b6ecc1a57fb2426de84e028895c80d7aa`  
		Last Modified: Tue, 12 Jan 2021 04:04:16 GMT  
		Size: 131.4 MB (131391628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104` - linux; ppc64le

```console
$ docker pull mono@sha256:582dd336e9dfac08b00f63738182f127e766f6e207a3914f47c35a44ca9c1f20
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.1 MB (192117601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eae166434ad1e239a83259bd86e49e76bc0f5aa0071cef7683034da040d80b53`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:25:06 GMT
ADD file:9d7252c169da9a089a0caa2f26cea24678267c15c0e129e7320d4defe0d4637b in / 
# Tue, 12 Jan 2021 00:25:16 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:37:52 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 12 Jan 2021 03:39:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:41:49 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 04:00:12 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:cb701c1e59a3b25dcb09b089f31d61af3065659cd29a7c748f66f3e3c8a96d58`  
		Last Modified: Tue, 12 Jan 2021 00:34:11 GMT  
		Size: 30.5 MB (30532837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a6b5cd501f71da14d37bddd625494e7a2de28217c260bc74553a9b4bc12b0f`  
		Last Modified: Tue, 12 Jan 2021 04:01:26 GMT  
		Size: 256.3 KB (256256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e85b5bce279ec9104f3a75e8c3a74fbd322ee4fff6244ab3046f12df7348d2a`  
		Last Modified: Tue, 12 Jan 2021 04:01:38 GMT  
		Size: 29.4 MB (29350170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ab9db45435abc9c30283f6ff37a0801fe81b852dca5ecad333bd338711bf55`  
		Last Modified: Tue, 12 Jan 2021 04:03:22 GMT  
		Size: 132.0 MB (131978338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10.0.104-slim`

```console
$ docker pull mono@sha256:181129afdf4074dd92b22706b22d33d3f2c052efd7a97884f9aad35e53186a26
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
$ docker pull mono@sha256:c844ff3b7ee54eaba943c75712d14160804ef3ab8dabdc1e1c3272e74608a541
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.5 MB (94456820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb1c7db5380987c54d84126cba76a6a6dccfaf004120eea20a3d79214279ab2d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:41:43 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 12 Jan 2021 09:41:50 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 09:42:22 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e54505e49395a0d6a43f271952bf307a05153f6510a80ae27038c50df0efa46`  
		Last Modified: Tue, 12 Jan 2021 09:57:16 GMT  
		Size: 255.9 KB (255924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187e7566eb41f21ec1afcdd35f44280fdc2057d58a74789bd9affda7da2084a4`  
		Last Modified: Tue, 12 Jan 2021 09:57:29 GMT  
		Size: 67.1 MB (67092827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:2c1b9f2574119a23ba08d3979be9838c569afcc86a3160db45a5b5c19083ac93
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51639329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07f97fb320bc3fc2e03010e1abaf0e5ae1e9e95c4f506ed16e674f7e1226f054`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:51:34 GMT
ADD file:57136a762436a5d41e60c61db0d89baea17a289845ea55565e45cc79a9e81e23 in / 
# Tue, 12 Jan 2021 00:51:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:59:29 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 12 Jan 2021 01:59:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 02:00:51 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2e2535e18472e7491a1d935b1f44ac842e4cc5c4d3de40cecb77b56b44515910`  
		Last Modified: Tue, 12 Jan 2021 01:00:19 GMT  
		Size: 24.9 MB (24851909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc75979d12aa60a81b3a6594a6f4d26e2bdd6261e0ca573176aebc974404f41`  
		Last Modified: Tue, 12 Jan 2021 02:08:19 GMT  
		Size: 256.0 KB (255959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce86ffd97c996edf2f5f32f5b54a3724e5fa9455e589ca9ff57e1fdc85117a28`  
		Last Modified: Tue, 12 Jan 2021 02:08:34 GMT  
		Size: 26.5 MB (26531461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:0be5365386dbc1532247663bf66fdd04a863371856ca5aca49a5b70b156da9f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48701398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44834f929c71beaf0f8d464170e4c359ff828c227e09f2e8547a033c113d6f82`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:01:09 GMT
ADD file:1db27e410cc7caf4a97a7313c57260fd01aa134b84306914ef0948dcca27372d in / 
# Tue, 12 Jan 2021 00:01:12 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:54:53 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 12 Jan 2021 03:55:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:55:53 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:be493c6a598447fe5f46a390f3bee10f2d2ba2215d39829fe84eb40a7add18fc`  
		Last Modified: Tue, 12 Jan 2021 00:11:14 GMT  
		Size: 22.7 MB (22715905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae41c04538a5197d9ce78432fa39191029ba0de2e0c89683471ee6a3599bbc9`  
		Last Modified: Tue, 12 Jan 2021 04:03:26 GMT  
		Size: 255.9 KB (255917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1677a1ffb68e5ae64625415689b4a2ff66f49acec6ae83b19f7834c082e4ff9`  
		Last Modified: Tue, 12 Jan 2021 04:03:35 GMT  
		Size: 25.7 MB (25729576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:6948940e8f06496863e933abbc4535ffbf2a6809be7a8ad57ba0472a7e425757
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57870227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48136d057bf03e9368936fd11090def9dea2ab83438eeb50225f1c3b77208e98`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:41:13 GMT
ADD file:0252dccbbfb76766e0e189783d38f6a6afd13f44daa7c5370ffd094adea0f583 in / 
# Tue, 12 Jan 2021 00:41:21 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 05:08:43 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 12 Jan 2021 05:08:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 05:09:36 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f8be76fcf2062bd14a3a78f858da701db8bcd907a2d0f33716d89d9329df2b1f`  
		Last Modified: Tue, 12 Jan 2021 00:51:54 GMT  
		Size: 25.9 MB (25864492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6179e732b6b6a778fbe4321833a5ba71f60a206504e6a1a93efe345ec9aedf3e`  
		Last Modified: Tue, 12 Jan 2021 05:15:48 GMT  
		Size: 255.9 KB (255937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79964378e1ae7824bc19481d96933ec96cd27ade28c334215d53bafbab3e5d53`  
		Last Modified: Tue, 12 Jan 2021 05:15:59 GMT  
		Size: 31.7 MB (31749798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; 386

```console
$ docker pull mono@sha256:23a7d61d14921fb6cdac9af3089bbe43d4802f95e94f5783e68d8665d14f9ed8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99160096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1183437f303f6695f81fc122467d5294b0b29e6038bafbce0e5afb2e84dc8ac`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:56:09 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 12 Jan 2021 03:56:18 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:56:56 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae604efc877a26d5e9ef47c0ce73f76fc847780ddc3fc4f4fa2dae62aebc1b79`  
		Last Modified: Tue, 12 Jan 2021 04:02:20 GMT  
		Size: 255.8 KB (255850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb5562f2f87a9508fba6e611a28b8bc7747b5368845e5cfa71f1a25a457f2c1e`  
		Last Modified: Tue, 12 Jan 2021 04:02:42 GMT  
		Size: 71.1 MB (71136255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0.104-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:dcf3bae1c6fc5c089a7c08cc5d902422dbe8047387242a2f451937b6bc571788
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60139263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9427fdc99870b74f065955ba37c7bac20a528e45dd0092c6cd6f305c7181ea22`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:25:06 GMT
ADD file:9d7252c169da9a089a0caa2f26cea24678267c15c0e129e7320d4defe0d4637b in / 
# Tue, 12 Jan 2021 00:25:16 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:37:52 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 12 Jan 2021 03:39:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:41:49 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:cb701c1e59a3b25dcb09b089f31d61af3065659cd29a7c748f66f3e3c8a96d58`  
		Last Modified: Tue, 12 Jan 2021 00:34:11 GMT  
		Size: 30.5 MB (30532837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a6b5cd501f71da14d37bddd625494e7a2de28217c260bc74553a9b4bc12b0f`  
		Last Modified: Tue, 12 Jan 2021 04:01:26 GMT  
		Size: 256.3 KB (256256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e85b5bce279ec9104f3a75e8c3a74fbd322ee4fff6244ab3046f12df7348d2a`  
		Last Modified: Tue, 12 Jan 2021 04:01:38 GMT  
		Size: 29.4 MB (29350170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10.0-slim`

```console
$ docker pull mono@sha256:181129afdf4074dd92b22706b22d33d3f2c052efd7a97884f9aad35e53186a26
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
$ docker pull mono@sha256:c844ff3b7ee54eaba943c75712d14160804ef3ab8dabdc1e1c3272e74608a541
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.5 MB (94456820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb1c7db5380987c54d84126cba76a6a6dccfaf004120eea20a3d79214279ab2d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:41:43 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 12 Jan 2021 09:41:50 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 09:42:22 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e54505e49395a0d6a43f271952bf307a05153f6510a80ae27038c50df0efa46`  
		Last Modified: Tue, 12 Jan 2021 09:57:16 GMT  
		Size: 255.9 KB (255924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187e7566eb41f21ec1afcdd35f44280fdc2057d58a74789bd9affda7da2084a4`  
		Last Modified: Tue, 12 Jan 2021 09:57:29 GMT  
		Size: 67.1 MB (67092827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:2c1b9f2574119a23ba08d3979be9838c569afcc86a3160db45a5b5c19083ac93
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51639329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07f97fb320bc3fc2e03010e1abaf0e5ae1e9e95c4f506ed16e674f7e1226f054`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:51:34 GMT
ADD file:57136a762436a5d41e60c61db0d89baea17a289845ea55565e45cc79a9e81e23 in / 
# Tue, 12 Jan 2021 00:51:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:59:29 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 12 Jan 2021 01:59:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 02:00:51 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2e2535e18472e7491a1d935b1f44ac842e4cc5c4d3de40cecb77b56b44515910`  
		Last Modified: Tue, 12 Jan 2021 01:00:19 GMT  
		Size: 24.9 MB (24851909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc75979d12aa60a81b3a6594a6f4d26e2bdd6261e0ca573176aebc974404f41`  
		Last Modified: Tue, 12 Jan 2021 02:08:19 GMT  
		Size: 256.0 KB (255959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce86ffd97c996edf2f5f32f5b54a3724e5fa9455e589ca9ff57e1fdc85117a28`  
		Last Modified: Tue, 12 Jan 2021 02:08:34 GMT  
		Size: 26.5 MB (26531461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:0be5365386dbc1532247663bf66fdd04a863371856ca5aca49a5b70b156da9f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48701398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44834f929c71beaf0f8d464170e4c359ff828c227e09f2e8547a033c113d6f82`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:01:09 GMT
ADD file:1db27e410cc7caf4a97a7313c57260fd01aa134b84306914ef0948dcca27372d in / 
# Tue, 12 Jan 2021 00:01:12 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:54:53 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 12 Jan 2021 03:55:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:55:53 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:be493c6a598447fe5f46a390f3bee10f2d2ba2215d39829fe84eb40a7add18fc`  
		Last Modified: Tue, 12 Jan 2021 00:11:14 GMT  
		Size: 22.7 MB (22715905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae41c04538a5197d9ce78432fa39191029ba0de2e0c89683471ee6a3599bbc9`  
		Last Modified: Tue, 12 Jan 2021 04:03:26 GMT  
		Size: 255.9 KB (255917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1677a1ffb68e5ae64625415689b4a2ff66f49acec6ae83b19f7834c082e4ff9`  
		Last Modified: Tue, 12 Jan 2021 04:03:35 GMT  
		Size: 25.7 MB (25729576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:6948940e8f06496863e933abbc4535ffbf2a6809be7a8ad57ba0472a7e425757
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57870227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48136d057bf03e9368936fd11090def9dea2ab83438eeb50225f1c3b77208e98`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:41:13 GMT
ADD file:0252dccbbfb76766e0e189783d38f6a6afd13f44daa7c5370ffd094adea0f583 in / 
# Tue, 12 Jan 2021 00:41:21 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 05:08:43 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 12 Jan 2021 05:08:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 05:09:36 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f8be76fcf2062bd14a3a78f858da701db8bcd907a2d0f33716d89d9329df2b1f`  
		Last Modified: Tue, 12 Jan 2021 00:51:54 GMT  
		Size: 25.9 MB (25864492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6179e732b6b6a778fbe4321833a5ba71f60a206504e6a1a93efe345ec9aedf3e`  
		Last Modified: Tue, 12 Jan 2021 05:15:48 GMT  
		Size: 255.9 KB (255937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79964378e1ae7824bc19481d96933ec96cd27ade28c334215d53bafbab3e5d53`  
		Last Modified: Tue, 12 Jan 2021 05:15:59 GMT  
		Size: 31.7 MB (31749798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; 386

```console
$ docker pull mono@sha256:23a7d61d14921fb6cdac9af3089bbe43d4802f95e94f5783e68d8665d14f9ed8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99160096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1183437f303f6695f81fc122467d5294b0b29e6038bafbce0e5afb2e84dc8ac`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:56:09 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 12 Jan 2021 03:56:18 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:56:56 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae604efc877a26d5e9ef47c0ce73f76fc847780ddc3fc4f4fa2dae62aebc1b79`  
		Last Modified: Tue, 12 Jan 2021 04:02:20 GMT  
		Size: 255.8 KB (255850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb5562f2f87a9508fba6e611a28b8bc7747b5368845e5cfa71f1a25a457f2c1e`  
		Last Modified: Tue, 12 Jan 2021 04:02:42 GMT  
		Size: 71.1 MB (71136255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10.0-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:dcf3bae1c6fc5c089a7c08cc5d902422dbe8047387242a2f451937b6bc571788
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60139263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9427fdc99870b74f065955ba37c7bac20a528e45dd0092c6cd6f305c7181ea22`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:25:06 GMT
ADD file:9d7252c169da9a089a0caa2f26cea24678267c15c0e129e7320d4defe0d4637b in / 
# Tue, 12 Jan 2021 00:25:16 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:37:52 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 12 Jan 2021 03:39:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:41:49 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:cb701c1e59a3b25dcb09b089f31d61af3065659cd29a7c748f66f3e3c8a96d58`  
		Last Modified: Tue, 12 Jan 2021 00:34:11 GMT  
		Size: 30.5 MB (30532837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a6b5cd501f71da14d37bddd625494e7a2de28217c260bc74553a9b4bc12b0f`  
		Last Modified: Tue, 12 Jan 2021 04:01:26 GMT  
		Size: 256.3 KB (256256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e85b5bce279ec9104f3a75e8c3a74fbd322ee4fff6244ab3046f12df7348d2a`  
		Last Modified: Tue, 12 Jan 2021 04:01:38 GMT  
		Size: 29.4 MB (29350170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.10-slim`

```console
$ docker pull mono@sha256:181129afdf4074dd92b22706b22d33d3f2c052efd7a97884f9aad35e53186a26
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
$ docker pull mono@sha256:c844ff3b7ee54eaba943c75712d14160804ef3ab8dabdc1e1c3272e74608a541
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.5 MB (94456820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb1c7db5380987c54d84126cba76a6a6dccfaf004120eea20a3d79214279ab2d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:41:43 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 12 Jan 2021 09:41:50 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 09:42:22 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e54505e49395a0d6a43f271952bf307a05153f6510a80ae27038c50df0efa46`  
		Last Modified: Tue, 12 Jan 2021 09:57:16 GMT  
		Size: 255.9 KB (255924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187e7566eb41f21ec1afcdd35f44280fdc2057d58a74789bd9affda7da2084a4`  
		Last Modified: Tue, 12 Jan 2021 09:57:29 GMT  
		Size: 67.1 MB (67092827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:2c1b9f2574119a23ba08d3979be9838c569afcc86a3160db45a5b5c19083ac93
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51639329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07f97fb320bc3fc2e03010e1abaf0e5ae1e9e95c4f506ed16e674f7e1226f054`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:51:34 GMT
ADD file:57136a762436a5d41e60c61db0d89baea17a289845ea55565e45cc79a9e81e23 in / 
# Tue, 12 Jan 2021 00:51:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:59:29 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 12 Jan 2021 01:59:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 02:00:51 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2e2535e18472e7491a1d935b1f44ac842e4cc5c4d3de40cecb77b56b44515910`  
		Last Modified: Tue, 12 Jan 2021 01:00:19 GMT  
		Size: 24.9 MB (24851909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc75979d12aa60a81b3a6594a6f4d26e2bdd6261e0ca573176aebc974404f41`  
		Last Modified: Tue, 12 Jan 2021 02:08:19 GMT  
		Size: 256.0 KB (255959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce86ffd97c996edf2f5f32f5b54a3724e5fa9455e589ca9ff57e1fdc85117a28`  
		Last Modified: Tue, 12 Jan 2021 02:08:34 GMT  
		Size: 26.5 MB (26531461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:0be5365386dbc1532247663bf66fdd04a863371856ca5aca49a5b70b156da9f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48701398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44834f929c71beaf0f8d464170e4c359ff828c227e09f2e8547a033c113d6f82`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:01:09 GMT
ADD file:1db27e410cc7caf4a97a7313c57260fd01aa134b84306914ef0948dcca27372d in / 
# Tue, 12 Jan 2021 00:01:12 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:54:53 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 12 Jan 2021 03:55:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:55:53 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:be493c6a598447fe5f46a390f3bee10f2d2ba2215d39829fe84eb40a7add18fc`  
		Last Modified: Tue, 12 Jan 2021 00:11:14 GMT  
		Size: 22.7 MB (22715905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae41c04538a5197d9ce78432fa39191029ba0de2e0c89683471ee6a3599bbc9`  
		Last Modified: Tue, 12 Jan 2021 04:03:26 GMT  
		Size: 255.9 KB (255917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1677a1ffb68e5ae64625415689b4a2ff66f49acec6ae83b19f7834c082e4ff9`  
		Last Modified: Tue, 12 Jan 2021 04:03:35 GMT  
		Size: 25.7 MB (25729576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:6948940e8f06496863e933abbc4535ffbf2a6809be7a8ad57ba0472a7e425757
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57870227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48136d057bf03e9368936fd11090def9dea2ab83438eeb50225f1c3b77208e98`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:41:13 GMT
ADD file:0252dccbbfb76766e0e189783d38f6a6afd13f44daa7c5370ffd094adea0f583 in / 
# Tue, 12 Jan 2021 00:41:21 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 05:08:43 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 12 Jan 2021 05:08:58 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 05:09:36 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f8be76fcf2062bd14a3a78f858da701db8bcd907a2d0f33716d89d9329df2b1f`  
		Last Modified: Tue, 12 Jan 2021 00:51:54 GMT  
		Size: 25.9 MB (25864492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6179e732b6b6a778fbe4321833a5ba71f60a206504e6a1a93efe345ec9aedf3e`  
		Last Modified: Tue, 12 Jan 2021 05:15:48 GMT  
		Size: 255.9 KB (255937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79964378e1ae7824bc19481d96933ec96cd27ade28c334215d53bafbab3e5d53`  
		Last Modified: Tue, 12 Jan 2021 05:15:59 GMT  
		Size: 31.7 MB (31749798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; 386

```console
$ docker pull mono@sha256:23a7d61d14921fb6cdac9af3089bbe43d4802f95e94f5783e68d8665d14f9ed8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99160096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1183437f303f6695f81fc122467d5294b0b29e6038bafbce0e5afb2e84dc8ac`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:56:09 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 12 Jan 2021 03:56:18 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:56:56 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae604efc877a26d5e9ef47c0ce73f76fc847780ddc3fc4f4fa2dae62aebc1b79`  
		Last Modified: Tue, 12 Jan 2021 04:02:20 GMT  
		Size: 255.8 KB (255850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb5562f2f87a9508fba6e611a28b8bc7747b5368845e5cfa71f1a25a457f2c1e`  
		Last Modified: Tue, 12 Jan 2021 04:02:42 GMT  
		Size: 71.1 MB (71136255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.10-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:dcf3bae1c6fc5c089a7c08cc5d902422dbe8047387242a2f451937b6bc571788
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60139263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9427fdc99870b74f065955ba37c7bac20a528e45dd0092c6cd6f305c7181ea22`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:25:06 GMT
ADD file:9d7252c169da9a089a0caa2f26cea24678267c15c0e129e7320d4defe0d4637b in / 
# Tue, 12 Jan 2021 00:25:16 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:37:52 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 12 Jan 2021 03:39:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:41:49 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:cb701c1e59a3b25dcb09b089f31d61af3065659cd29a7c748f66f3e3c8a96d58`  
		Last Modified: Tue, 12 Jan 2021 00:34:11 GMT  
		Size: 30.5 MB (30532837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a6b5cd501f71da14d37bddd625494e7a2de28217c260bc74553a9b4bc12b0f`  
		Last Modified: Tue, 12 Jan 2021 04:01:26 GMT  
		Size: 256.3 KB (256256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e85b5bce279ec9104f3a75e8c3a74fbd322ee4fff6244ab3046f12df7348d2a`  
		Last Modified: Tue, 12 Jan 2021 04:01:38 GMT  
		Size: 29.4 MB (29350170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.12`

```console
$ docker pull mono@sha256:fee59facbee3c69f535f506910bbac808643a8f91f5a80ddc79e478fa5982f58
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.12` - linux; amd64

```console
$ docker pull mono@sha256:e3c3faa1e0eccfec442341c7260bfb1faeccf40581fe8a00e77e794cf27d150b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.9 MB (235856726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d02da61afa912e62ef7cdc2e3b89fb6915716c72eccd75293b5c784ba17e5ce`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:40:56 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 09:41:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 09:41:33 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 09:48:29 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe02677df6f8831edfcea8a4558dcbb344dda0a234033ce403a445f71bb95e04`  
		Last Modified: Tue, 12 Jan 2021 09:56:50 GMT  
		Size: 255.9 KB (255924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6f0c1d36d945478bb94f4061ab9e9570a42d064b1bac55d482cc3d9eefdc1b`  
		Last Modified: Tue, 12 Jan 2021 09:57:04 GMT  
		Size: 67.1 MB (67079218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55acb8a81f9716f19bc8b425a4f2f9778868a086ced2c38a0d232c7e149e260b`  
		Last Modified: Tue, 12 Jan 2021 09:58:10 GMT  
		Size: 141.4 MB (141413515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12` - linux; arm variant v5

```console
$ docker pull mono@sha256:93e07bd0966ba3af8e1265a2976fa87cf142485c7984e221d5bd1900b1129c04
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.7 MB (191715473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d675a592f2dd1ff1c3d27b04a2e5373c8d8d9fd42ea3e202cf2f0deeabc4a11b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:51:34 GMT
ADD file:57136a762436a5d41e60c61db0d89baea17a289845ea55565e45cc79a9e81e23 in / 
# Tue, 12 Jan 2021 00:51:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:58:10 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 01:58:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 01:59:18 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 02:04:03 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2e2535e18472e7491a1d935b1f44ac842e4cc5c4d3de40cecb77b56b44515910`  
		Last Modified: Tue, 12 Jan 2021 01:00:19 GMT  
		Size: 24.9 MB (24851909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781b0df29588b1d712497221b09542f9b882364892a46ecf5521b50115ffe045`  
		Last Modified: Tue, 12 Jan 2021 02:07:54 GMT  
		Size: 255.9 KB (255947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ccd7e036e1bf04d2229ab088bc370548d6b63d0540abdfa03ab614ff643669e`  
		Last Modified: Tue, 12 Jan 2021 02:08:01 GMT  
		Size: 26.5 MB (26499381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057e315d7d334759ab98965930ff1540b0ca7c9ae700b6bbb74fa1506fed258a`  
		Last Modified: Tue, 12 Jan 2021 02:09:34 GMT  
		Size: 140.1 MB (140108236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12` - linux; arm variant v7

```console
$ docker pull mono@sha256:172236fea866d1b739364ba9049c97abc885743e420322f6df0dd72c617ab1d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.6 MB (187612230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f579c6e6d6132fc34dcf39db01f217918a65e0cf5889c53e939eb89bd3453d13`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:01:09 GMT
ADD file:1db27e410cc7caf4a97a7313c57260fd01aa134b84306914ef0948dcca27372d in / 
# Tue, 12 Jan 2021 00:01:12 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:53:47 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 03:54:04 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:54:42 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 03:58:38 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:be493c6a598447fe5f46a390f3bee10f2d2ba2215d39829fe84eb40a7add18fc`  
		Last Modified: Tue, 12 Jan 2021 00:11:14 GMT  
		Size: 22.7 MB (22715905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c33bdc53ec4d57ecf8d4565fca28d67f043f4855d49b01e900e8ef3c8bb9d6`  
		Last Modified: Tue, 12 Jan 2021 04:03:03 GMT  
		Size: 255.9 KB (255942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d9304eb6e55e2cd3920831bd0dec33588ea625b97a60aa2b06301f9351de819`  
		Last Modified: Tue, 12 Jan 2021 04:03:11 GMT  
		Size: 25.7 MB (25697506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1168b3f3ae6bc53dbe989dc4db4fad0b76b83fcb4d4db9dd33f685342c886c`  
		Last Modified: Tue, 12 Jan 2021 04:04:41 GMT  
		Size: 138.9 MB (138942877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:bb8bcb03c776a1d69c8402a77aeb49e7302fca102ab82e11002ca319287ae33a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.4 MB (214424611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a8b3b0d88c8a2f9826ad928f5035cd23a14395c38e57da6f376205bb25ac8d2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:41:13 GMT
ADD file:0252dccbbfb76766e0e189783d38f6a6afd13f44daa7c5370ffd094adea0f583 in / 
# Tue, 12 Jan 2021 00:41:21 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 05:07:35 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 05:07:52 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 05:08:28 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 05:12:14 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f8be76fcf2062bd14a3a78f858da701db8bcd907a2d0f33716d89d9329df2b1f`  
		Last Modified: Tue, 12 Jan 2021 00:51:54 GMT  
		Size: 25.9 MB (25864492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c624bef28ff9228422eef122ec713693eb2e8d2ed78aa41f319bd0678a607c`  
		Last Modified: Tue, 12 Jan 2021 05:15:20 GMT  
		Size: 255.9 KB (255923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ec950da6523b4cb54939edc61c6460d64327528adc05f607fbf005ff508a88`  
		Last Modified: Tue, 12 Jan 2021 05:15:34 GMT  
		Size: 31.7 MB (31720550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0470c4fa675956b4e41164ba69e70c7c53cbf56fa1fde6ca99247fd30d63182`  
		Last Modified: Tue, 12 Jan 2021 05:16:54 GMT  
		Size: 156.6 MB (156583646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12` - linux; 386

```console
$ docker pull mono@sha256:3f6d7e510f3c7e210af3336de41288b7e8971519c559d7994389b5aaab7ca0d6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.6 MB (241641989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d7d8ae0005ba40c7547dfff94755167dba0e74f722bd8583e10d292d8cc13d2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:55:14 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 03:55:23 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:56:00 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 03:59:02 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ae7e24292b47c5c54d019f27f833b4d1fd06c6c1760426a915f4626d13ebb5`  
		Last Modified: Tue, 12 Jan 2021 04:01:42 GMT  
		Size: 255.9 KB (255867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723f6fae6c251aafe4f2903014f5ca67d695cd2f74f87cc46b0b9b5e50650a9f`  
		Last Modified: Tue, 12 Jan 2021 04:02:03 GMT  
		Size: 71.1 MB (71105792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a6a59d3738ce8d2e6bad95e51859928eac584152411a872b1dfd4ec6cbffe4`  
		Last Modified: Tue, 12 Jan 2021 04:03:29 GMT  
		Size: 142.5 MB (142512339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12` - linux; ppc64le

```console
$ docker pull mono@sha256:8cd03e8a315754c3631020ef221a2d0cbd0992577901c899c47ce5e69d61dd49
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.3 MB (203325644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be23bd3cc106fdd913dd4eff53c1f46dabb535e753abef0f566dae2c69eaea9d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:25:06 GMT
ADD file:9d7252c169da9a089a0caa2f26cea24678267c15c0e129e7320d4defe0d4637b in / 
# Tue, 12 Jan 2021 00:25:16 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:34:09 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 03:35:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:37:38 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 03:52:04 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:cb701c1e59a3b25dcb09b089f31d61af3065659cd29a7c748f66f3e3c8a96d58`  
		Last Modified: Tue, 12 Jan 2021 00:34:11 GMT  
		Size: 30.5 MB (30532837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e77824b16d99ee079aa03b8aabec031637265f7380c082326eaf48d078a93e7`  
		Last Modified: Tue, 12 Jan 2021 04:01:02 GMT  
		Size: 256.1 KB (256146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8e3bf2452dcba3a8621830f987ddbcc051bd5b6d5817e6d595c1cd93497f67`  
		Last Modified: Tue, 12 Jan 2021 04:01:08 GMT  
		Size: 29.3 MB (29311088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be798b1b9507d975e13d056b87d688839b0f83115176be62486731bf9cac3ed7`  
		Last Modified: Tue, 12 Jan 2021 04:02:25 GMT  
		Size: 143.2 MB (143225573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.12.0`

```console
$ docker pull mono@sha256:fee59facbee3c69f535f506910bbac808643a8f91f5a80ddc79e478fa5982f58
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.12.0` - linux; amd64

```console
$ docker pull mono@sha256:e3c3faa1e0eccfec442341c7260bfb1faeccf40581fe8a00e77e794cf27d150b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.9 MB (235856726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d02da61afa912e62ef7cdc2e3b89fb6915716c72eccd75293b5c784ba17e5ce`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:40:56 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 09:41:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 09:41:33 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 09:48:29 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe02677df6f8831edfcea8a4558dcbb344dda0a234033ce403a445f71bb95e04`  
		Last Modified: Tue, 12 Jan 2021 09:56:50 GMT  
		Size: 255.9 KB (255924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6f0c1d36d945478bb94f4061ab9e9570a42d064b1bac55d482cc3d9eefdc1b`  
		Last Modified: Tue, 12 Jan 2021 09:57:04 GMT  
		Size: 67.1 MB (67079218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55acb8a81f9716f19bc8b425a4f2f9778868a086ced2c38a0d232c7e149e260b`  
		Last Modified: Tue, 12 Jan 2021 09:58:10 GMT  
		Size: 141.4 MB (141413515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0` - linux; arm variant v5

```console
$ docker pull mono@sha256:93e07bd0966ba3af8e1265a2976fa87cf142485c7984e221d5bd1900b1129c04
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.7 MB (191715473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d675a592f2dd1ff1c3d27b04a2e5373c8d8d9fd42ea3e202cf2f0deeabc4a11b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:51:34 GMT
ADD file:57136a762436a5d41e60c61db0d89baea17a289845ea55565e45cc79a9e81e23 in / 
# Tue, 12 Jan 2021 00:51:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:58:10 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 01:58:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 01:59:18 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 02:04:03 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2e2535e18472e7491a1d935b1f44ac842e4cc5c4d3de40cecb77b56b44515910`  
		Last Modified: Tue, 12 Jan 2021 01:00:19 GMT  
		Size: 24.9 MB (24851909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781b0df29588b1d712497221b09542f9b882364892a46ecf5521b50115ffe045`  
		Last Modified: Tue, 12 Jan 2021 02:07:54 GMT  
		Size: 255.9 KB (255947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ccd7e036e1bf04d2229ab088bc370548d6b63d0540abdfa03ab614ff643669e`  
		Last Modified: Tue, 12 Jan 2021 02:08:01 GMT  
		Size: 26.5 MB (26499381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057e315d7d334759ab98965930ff1540b0ca7c9ae700b6bbb74fa1506fed258a`  
		Last Modified: Tue, 12 Jan 2021 02:09:34 GMT  
		Size: 140.1 MB (140108236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0` - linux; arm variant v7

```console
$ docker pull mono@sha256:172236fea866d1b739364ba9049c97abc885743e420322f6df0dd72c617ab1d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.6 MB (187612230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f579c6e6d6132fc34dcf39db01f217918a65e0cf5889c53e939eb89bd3453d13`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:01:09 GMT
ADD file:1db27e410cc7caf4a97a7313c57260fd01aa134b84306914ef0948dcca27372d in / 
# Tue, 12 Jan 2021 00:01:12 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:53:47 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 03:54:04 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:54:42 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 03:58:38 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:be493c6a598447fe5f46a390f3bee10f2d2ba2215d39829fe84eb40a7add18fc`  
		Last Modified: Tue, 12 Jan 2021 00:11:14 GMT  
		Size: 22.7 MB (22715905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c33bdc53ec4d57ecf8d4565fca28d67f043f4855d49b01e900e8ef3c8bb9d6`  
		Last Modified: Tue, 12 Jan 2021 04:03:03 GMT  
		Size: 255.9 KB (255942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d9304eb6e55e2cd3920831bd0dec33588ea625b97a60aa2b06301f9351de819`  
		Last Modified: Tue, 12 Jan 2021 04:03:11 GMT  
		Size: 25.7 MB (25697506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1168b3f3ae6bc53dbe989dc4db4fad0b76b83fcb4d4db9dd33f685342c886c`  
		Last Modified: Tue, 12 Jan 2021 04:04:41 GMT  
		Size: 138.9 MB (138942877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:bb8bcb03c776a1d69c8402a77aeb49e7302fca102ab82e11002ca319287ae33a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.4 MB (214424611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a8b3b0d88c8a2f9826ad928f5035cd23a14395c38e57da6f376205bb25ac8d2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:41:13 GMT
ADD file:0252dccbbfb76766e0e189783d38f6a6afd13f44daa7c5370ffd094adea0f583 in / 
# Tue, 12 Jan 2021 00:41:21 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 05:07:35 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 05:07:52 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 05:08:28 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 05:12:14 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f8be76fcf2062bd14a3a78f858da701db8bcd907a2d0f33716d89d9329df2b1f`  
		Last Modified: Tue, 12 Jan 2021 00:51:54 GMT  
		Size: 25.9 MB (25864492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c624bef28ff9228422eef122ec713693eb2e8d2ed78aa41f319bd0678a607c`  
		Last Modified: Tue, 12 Jan 2021 05:15:20 GMT  
		Size: 255.9 KB (255923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ec950da6523b4cb54939edc61c6460d64327528adc05f607fbf005ff508a88`  
		Last Modified: Tue, 12 Jan 2021 05:15:34 GMT  
		Size: 31.7 MB (31720550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0470c4fa675956b4e41164ba69e70c7c53cbf56fa1fde6ca99247fd30d63182`  
		Last Modified: Tue, 12 Jan 2021 05:16:54 GMT  
		Size: 156.6 MB (156583646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0` - linux; 386

```console
$ docker pull mono@sha256:3f6d7e510f3c7e210af3336de41288b7e8971519c559d7994389b5aaab7ca0d6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.6 MB (241641989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d7d8ae0005ba40c7547dfff94755167dba0e74f722bd8583e10d292d8cc13d2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:55:14 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 03:55:23 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:56:00 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 03:59:02 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ae7e24292b47c5c54d019f27f833b4d1fd06c6c1760426a915f4626d13ebb5`  
		Last Modified: Tue, 12 Jan 2021 04:01:42 GMT  
		Size: 255.9 KB (255867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723f6fae6c251aafe4f2903014f5ca67d695cd2f74f87cc46b0b9b5e50650a9f`  
		Last Modified: Tue, 12 Jan 2021 04:02:03 GMT  
		Size: 71.1 MB (71105792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a6a59d3738ce8d2e6bad95e51859928eac584152411a872b1dfd4ec6cbffe4`  
		Last Modified: Tue, 12 Jan 2021 04:03:29 GMT  
		Size: 142.5 MB (142512339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0` - linux; ppc64le

```console
$ docker pull mono@sha256:8cd03e8a315754c3631020ef221a2d0cbd0992577901c899c47ce5e69d61dd49
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.3 MB (203325644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be23bd3cc106fdd913dd4eff53c1f46dabb535e753abef0f566dae2c69eaea9d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:25:06 GMT
ADD file:9d7252c169da9a089a0caa2f26cea24678267c15c0e129e7320d4defe0d4637b in / 
# Tue, 12 Jan 2021 00:25:16 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:34:09 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 03:35:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:37:38 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 03:52:04 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:cb701c1e59a3b25dcb09b089f31d61af3065659cd29a7c748f66f3e3c8a96d58`  
		Last Modified: Tue, 12 Jan 2021 00:34:11 GMT  
		Size: 30.5 MB (30532837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e77824b16d99ee079aa03b8aabec031637265f7380c082326eaf48d078a93e7`  
		Last Modified: Tue, 12 Jan 2021 04:01:02 GMT  
		Size: 256.1 KB (256146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8e3bf2452dcba3a8621830f987ddbcc051bd5b6d5817e6d595c1cd93497f67`  
		Last Modified: Tue, 12 Jan 2021 04:01:08 GMT  
		Size: 29.3 MB (29311088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be798b1b9507d975e13d056b87d688839b0f83115176be62486731bf9cac3ed7`  
		Last Modified: Tue, 12 Jan 2021 04:02:25 GMT  
		Size: 143.2 MB (143225573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.12.0.107`

```console
$ docker pull mono@sha256:fee59facbee3c69f535f506910bbac808643a8f91f5a80ddc79e478fa5982f58
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.12.0.107` - linux; amd64

```console
$ docker pull mono@sha256:e3c3faa1e0eccfec442341c7260bfb1faeccf40581fe8a00e77e794cf27d150b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.9 MB (235856726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d02da61afa912e62ef7cdc2e3b89fb6915716c72eccd75293b5c784ba17e5ce`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:40:56 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 09:41:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 09:41:33 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 09:48:29 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe02677df6f8831edfcea8a4558dcbb344dda0a234033ce403a445f71bb95e04`  
		Last Modified: Tue, 12 Jan 2021 09:56:50 GMT  
		Size: 255.9 KB (255924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6f0c1d36d945478bb94f4061ab9e9570a42d064b1bac55d482cc3d9eefdc1b`  
		Last Modified: Tue, 12 Jan 2021 09:57:04 GMT  
		Size: 67.1 MB (67079218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55acb8a81f9716f19bc8b425a4f2f9778868a086ced2c38a0d232c7e149e260b`  
		Last Modified: Tue, 12 Jan 2021 09:58:10 GMT  
		Size: 141.4 MB (141413515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.107` - linux; arm variant v5

```console
$ docker pull mono@sha256:93e07bd0966ba3af8e1265a2976fa87cf142485c7984e221d5bd1900b1129c04
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.7 MB (191715473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d675a592f2dd1ff1c3d27b04a2e5373c8d8d9fd42ea3e202cf2f0deeabc4a11b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:51:34 GMT
ADD file:57136a762436a5d41e60c61db0d89baea17a289845ea55565e45cc79a9e81e23 in / 
# Tue, 12 Jan 2021 00:51:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:58:10 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 01:58:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 01:59:18 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 02:04:03 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2e2535e18472e7491a1d935b1f44ac842e4cc5c4d3de40cecb77b56b44515910`  
		Last Modified: Tue, 12 Jan 2021 01:00:19 GMT  
		Size: 24.9 MB (24851909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781b0df29588b1d712497221b09542f9b882364892a46ecf5521b50115ffe045`  
		Last Modified: Tue, 12 Jan 2021 02:07:54 GMT  
		Size: 255.9 KB (255947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ccd7e036e1bf04d2229ab088bc370548d6b63d0540abdfa03ab614ff643669e`  
		Last Modified: Tue, 12 Jan 2021 02:08:01 GMT  
		Size: 26.5 MB (26499381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057e315d7d334759ab98965930ff1540b0ca7c9ae700b6bbb74fa1506fed258a`  
		Last Modified: Tue, 12 Jan 2021 02:09:34 GMT  
		Size: 140.1 MB (140108236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.107` - linux; arm variant v7

```console
$ docker pull mono@sha256:172236fea866d1b739364ba9049c97abc885743e420322f6df0dd72c617ab1d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.6 MB (187612230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f579c6e6d6132fc34dcf39db01f217918a65e0cf5889c53e939eb89bd3453d13`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:01:09 GMT
ADD file:1db27e410cc7caf4a97a7313c57260fd01aa134b84306914ef0948dcca27372d in / 
# Tue, 12 Jan 2021 00:01:12 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:53:47 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 03:54:04 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:54:42 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 03:58:38 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:be493c6a598447fe5f46a390f3bee10f2d2ba2215d39829fe84eb40a7add18fc`  
		Last Modified: Tue, 12 Jan 2021 00:11:14 GMT  
		Size: 22.7 MB (22715905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c33bdc53ec4d57ecf8d4565fca28d67f043f4855d49b01e900e8ef3c8bb9d6`  
		Last Modified: Tue, 12 Jan 2021 04:03:03 GMT  
		Size: 255.9 KB (255942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d9304eb6e55e2cd3920831bd0dec33588ea625b97a60aa2b06301f9351de819`  
		Last Modified: Tue, 12 Jan 2021 04:03:11 GMT  
		Size: 25.7 MB (25697506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1168b3f3ae6bc53dbe989dc4db4fad0b76b83fcb4d4db9dd33f685342c886c`  
		Last Modified: Tue, 12 Jan 2021 04:04:41 GMT  
		Size: 138.9 MB (138942877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.107` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:bb8bcb03c776a1d69c8402a77aeb49e7302fca102ab82e11002ca319287ae33a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.4 MB (214424611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a8b3b0d88c8a2f9826ad928f5035cd23a14395c38e57da6f376205bb25ac8d2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:41:13 GMT
ADD file:0252dccbbfb76766e0e189783d38f6a6afd13f44daa7c5370ffd094adea0f583 in / 
# Tue, 12 Jan 2021 00:41:21 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 05:07:35 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 05:07:52 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 05:08:28 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 05:12:14 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f8be76fcf2062bd14a3a78f858da701db8bcd907a2d0f33716d89d9329df2b1f`  
		Last Modified: Tue, 12 Jan 2021 00:51:54 GMT  
		Size: 25.9 MB (25864492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c624bef28ff9228422eef122ec713693eb2e8d2ed78aa41f319bd0678a607c`  
		Last Modified: Tue, 12 Jan 2021 05:15:20 GMT  
		Size: 255.9 KB (255923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ec950da6523b4cb54939edc61c6460d64327528adc05f607fbf005ff508a88`  
		Last Modified: Tue, 12 Jan 2021 05:15:34 GMT  
		Size: 31.7 MB (31720550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0470c4fa675956b4e41164ba69e70c7c53cbf56fa1fde6ca99247fd30d63182`  
		Last Modified: Tue, 12 Jan 2021 05:16:54 GMT  
		Size: 156.6 MB (156583646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.107` - linux; 386

```console
$ docker pull mono@sha256:3f6d7e510f3c7e210af3336de41288b7e8971519c559d7994389b5aaab7ca0d6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.6 MB (241641989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d7d8ae0005ba40c7547dfff94755167dba0e74f722bd8583e10d292d8cc13d2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:55:14 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 03:55:23 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:56:00 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 03:59:02 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ae7e24292b47c5c54d019f27f833b4d1fd06c6c1760426a915f4626d13ebb5`  
		Last Modified: Tue, 12 Jan 2021 04:01:42 GMT  
		Size: 255.9 KB (255867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723f6fae6c251aafe4f2903014f5ca67d695cd2f74f87cc46b0b9b5e50650a9f`  
		Last Modified: Tue, 12 Jan 2021 04:02:03 GMT  
		Size: 71.1 MB (71105792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a6a59d3738ce8d2e6bad95e51859928eac584152411a872b1dfd4ec6cbffe4`  
		Last Modified: Tue, 12 Jan 2021 04:03:29 GMT  
		Size: 142.5 MB (142512339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.107` - linux; ppc64le

```console
$ docker pull mono@sha256:8cd03e8a315754c3631020ef221a2d0cbd0992577901c899c47ce5e69d61dd49
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.3 MB (203325644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be23bd3cc106fdd913dd4eff53c1f46dabb535e753abef0f566dae2c69eaea9d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:25:06 GMT
ADD file:9d7252c169da9a089a0caa2f26cea24678267c15c0e129e7320d4defe0d4637b in / 
# Tue, 12 Jan 2021 00:25:16 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:34:09 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 03:35:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:37:38 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 03:52:04 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:cb701c1e59a3b25dcb09b089f31d61af3065659cd29a7c748f66f3e3c8a96d58`  
		Last Modified: Tue, 12 Jan 2021 00:34:11 GMT  
		Size: 30.5 MB (30532837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e77824b16d99ee079aa03b8aabec031637265f7380c082326eaf48d078a93e7`  
		Last Modified: Tue, 12 Jan 2021 04:01:02 GMT  
		Size: 256.1 KB (256146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8e3bf2452dcba3a8621830f987ddbcc051bd5b6d5817e6d595c1cd93497f67`  
		Last Modified: Tue, 12 Jan 2021 04:01:08 GMT  
		Size: 29.3 MB (29311088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be798b1b9507d975e13d056b87d688839b0f83115176be62486731bf9cac3ed7`  
		Last Modified: Tue, 12 Jan 2021 04:02:25 GMT  
		Size: 143.2 MB (143225573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.12.0.107-slim`

```console
$ docker pull mono@sha256:28d3578057e16483bef3cb7d9b30c54fa672b8ced049268ad11d96652864336a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.12.0.107-slim` - linux; amd64

```console
$ docker pull mono@sha256:8769207b9677e6f3f0e95b6423c76cdfd5e450f6b32c051db7b91db5577d7e21
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.4 MB (94443211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:348b7e1144c12af5295b3c38dd57ef1b5c6e171ee9409efbbe2bacd0c680eae5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:40:56 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 09:41:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 09:41:33 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe02677df6f8831edfcea8a4558dcbb344dda0a234033ce403a445f71bb95e04`  
		Last Modified: Tue, 12 Jan 2021 09:56:50 GMT  
		Size: 255.9 KB (255924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6f0c1d36d945478bb94f4061ab9e9570a42d064b1bac55d482cc3d9eefdc1b`  
		Last Modified: Tue, 12 Jan 2021 09:57:04 GMT  
		Size: 67.1 MB (67079218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.107-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:fbdc9066c014b9853957843c45f789b61596294919443a607a8ccf5749442c7a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51607237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d35599162358d092829e97e4858f0a1073436f41099f7a5b983df6c1b4956954`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:51:34 GMT
ADD file:57136a762436a5d41e60c61db0d89baea17a289845ea55565e45cc79a9e81e23 in / 
# Tue, 12 Jan 2021 00:51:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:58:10 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 01:58:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 01:59:18 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2e2535e18472e7491a1d935b1f44ac842e4cc5c4d3de40cecb77b56b44515910`  
		Last Modified: Tue, 12 Jan 2021 01:00:19 GMT  
		Size: 24.9 MB (24851909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781b0df29588b1d712497221b09542f9b882364892a46ecf5521b50115ffe045`  
		Last Modified: Tue, 12 Jan 2021 02:07:54 GMT  
		Size: 255.9 KB (255947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ccd7e036e1bf04d2229ab088bc370548d6b63d0540abdfa03ab614ff643669e`  
		Last Modified: Tue, 12 Jan 2021 02:08:01 GMT  
		Size: 26.5 MB (26499381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.107-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:5feb406d1ce80dd86fc2db709ca76f30c7120ee7a40a712fd7e32899e4bdffb7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48669353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f15fcf95ecaebe203ce057c5d16cbfff554c6d24084bef88355b180812987040`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:01:09 GMT
ADD file:1db27e410cc7caf4a97a7313c57260fd01aa134b84306914ef0948dcca27372d in / 
# Tue, 12 Jan 2021 00:01:12 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:53:47 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 03:54:04 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:54:42 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:be493c6a598447fe5f46a390f3bee10f2d2ba2215d39829fe84eb40a7add18fc`  
		Last Modified: Tue, 12 Jan 2021 00:11:14 GMT  
		Size: 22.7 MB (22715905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c33bdc53ec4d57ecf8d4565fca28d67f043f4855d49b01e900e8ef3c8bb9d6`  
		Last Modified: Tue, 12 Jan 2021 04:03:03 GMT  
		Size: 255.9 KB (255942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d9304eb6e55e2cd3920831bd0dec33588ea625b97a60aa2b06301f9351de819`  
		Last Modified: Tue, 12 Jan 2021 04:03:11 GMT  
		Size: 25.7 MB (25697506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.107-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:90a25ba70e6af84267801fd4cbeb308a72f614df951c6c33e9782e140e373538
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.8 MB (57840965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b69b6854e1856fe6d38217029a566ca928db10d685c520adb43f1ecd510f16d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:41:13 GMT
ADD file:0252dccbbfb76766e0e189783d38f6a6afd13f44daa7c5370ffd094adea0f583 in / 
# Tue, 12 Jan 2021 00:41:21 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 05:07:35 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 05:07:52 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 05:08:28 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f8be76fcf2062bd14a3a78f858da701db8bcd907a2d0f33716d89d9329df2b1f`  
		Last Modified: Tue, 12 Jan 2021 00:51:54 GMT  
		Size: 25.9 MB (25864492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c624bef28ff9228422eef122ec713693eb2e8d2ed78aa41f319bd0678a607c`  
		Last Modified: Tue, 12 Jan 2021 05:15:20 GMT  
		Size: 255.9 KB (255923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ec950da6523b4cb54939edc61c6460d64327528adc05f607fbf005ff508a88`  
		Last Modified: Tue, 12 Jan 2021 05:15:34 GMT  
		Size: 31.7 MB (31720550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.107-slim` - linux; 386

```console
$ docker pull mono@sha256:521020ecd687652f6d5c2e2de3a818db2510b049378854f835bfc7caa058746e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99129650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a612a9ed794b39d2f1751626f377d4fe36630334994f4e592e859b2370d5d37`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:55:14 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 03:55:23 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:56:00 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ae7e24292b47c5c54d019f27f833b4d1fd06c6c1760426a915f4626d13ebb5`  
		Last Modified: Tue, 12 Jan 2021 04:01:42 GMT  
		Size: 255.9 KB (255867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723f6fae6c251aafe4f2903014f5ca67d695cd2f74f87cc46b0b9b5e50650a9f`  
		Last Modified: Tue, 12 Jan 2021 04:02:03 GMT  
		Size: 71.1 MB (71105792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0.107-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:fe8b241787171b74a2fd43cd5f13bd303c637bf330e80f289245b9c27b8eb306
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60100071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:638800145fd3d9c6b9e6088d6dd2118832963e6457e99a6a04bfd75078bebd50`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:25:06 GMT
ADD file:9d7252c169da9a089a0caa2f26cea24678267c15c0e129e7320d4defe0d4637b in / 
# Tue, 12 Jan 2021 00:25:16 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:34:09 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 03:35:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:37:38 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:cb701c1e59a3b25dcb09b089f31d61af3065659cd29a7c748f66f3e3c8a96d58`  
		Last Modified: Tue, 12 Jan 2021 00:34:11 GMT  
		Size: 30.5 MB (30532837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e77824b16d99ee079aa03b8aabec031637265f7380c082326eaf48d078a93e7`  
		Last Modified: Tue, 12 Jan 2021 04:01:02 GMT  
		Size: 256.1 KB (256146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8e3bf2452dcba3a8621830f987ddbcc051bd5b6d5817e6d595c1cd93497f67`  
		Last Modified: Tue, 12 Jan 2021 04:01:08 GMT  
		Size: 29.3 MB (29311088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.12.0-slim`

```console
$ docker pull mono@sha256:28d3578057e16483bef3cb7d9b30c54fa672b8ced049268ad11d96652864336a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.12.0-slim` - linux; amd64

```console
$ docker pull mono@sha256:8769207b9677e6f3f0e95b6423c76cdfd5e450f6b32c051db7b91db5577d7e21
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.4 MB (94443211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:348b7e1144c12af5295b3c38dd57ef1b5c6e171ee9409efbbe2bacd0c680eae5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:40:56 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 09:41:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 09:41:33 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe02677df6f8831edfcea8a4558dcbb344dda0a234033ce403a445f71bb95e04`  
		Last Modified: Tue, 12 Jan 2021 09:56:50 GMT  
		Size: 255.9 KB (255924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6f0c1d36d945478bb94f4061ab9e9570a42d064b1bac55d482cc3d9eefdc1b`  
		Last Modified: Tue, 12 Jan 2021 09:57:04 GMT  
		Size: 67.1 MB (67079218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:fbdc9066c014b9853957843c45f789b61596294919443a607a8ccf5749442c7a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51607237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d35599162358d092829e97e4858f0a1073436f41099f7a5b983df6c1b4956954`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:51:34 GMT
ADD file:57136a762436a5d41e60c61db0d89baea17a289845ea55565e45cc79a9e81e23 in / 
# Tue, 12 Jan 2021 00:51:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:58:10 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 01:58:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 01:59:18 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2e2535e18472e7491a1d935b1f44ac842e4cc5c4d3de40cecb77b56b44515910`  
		Last Modified: Tue, 12 Jan 2021 01:00:19 GMT  
		Size: 24.9 MB (24851909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781b0df29588b1d712497221b09542f9b882364892a46ecf5521b50115ffe045`  
		Last Modified: Tue, 12 Jan 2021 02:07:54 GMT  
		Size: 255.9 KB (255947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ccd7e036e1bf04d2229ab088bc370548d6b63d0540abdfa03ab614ff643669e`  
		Last Modified: Tue, 12 Jan 2021 02:08:01 GMT  
		Size: 26.5 MB (26499381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:5feb406d1ce80dd86fc2db709ca76f30c7120ee7a40a712fd7e32899e4bdffb7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48669353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f15fcf95ecaebe203ce057c5d16cbfff554c6d24084bef88355b180812987040`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:01:09 GMT
ADD file:1db27e410cc7caf4a97a7313c57260fd01aa134b84306914ef0948dcca27372d in / 
# Tue, 12 Jan 2021 00:01:12 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:53:47 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 03:54:04 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:54:42 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:be493c6a598447fe5f46a390f3bee10f2d2ba2215d39829fe84eb40a7add18fc`  
		Last Modified: Tue, 12 Jan 2021 00:11:14 GMT  
		Size: 22.7 MB (22715905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c33bdc53ec4d57ecf8d4565fca28d67f043f4855d49b01e900e8ef3c8bb9d6`  
		Last Modified: Tue, 12 Jan 2021 04:03:03 GMT  
		Size: 255.9 KB (255942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d9304eb6e55e2cd3920831bd0dec33588ea625b97a60aa2b06301f9351de819`  
		Last Modified: Tue, 12 Jan 2021 04:03:11 GMT  
		Size: 25.7 MB (25697506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:90a25ba70e6af84267801fd4cbeb308a72f614df951c6c33e9782e140e373538
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.8 MB (57840965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b69b6854e1856fe6d38217029a566ca928db10d685c520adb43f1ecd510f16d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:41:13 GMT
ADD file:0252dccbbfb76766e0e189783d38f6a6afd13f44daa7c5370ffd094adea0f583 in / 
# Tue, 12 Jan 2021 00:41:21 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 05:07:35 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 05:07:52 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 05:08:28 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f8be76fcf2062bd14a3a78f858da701db8bcd907a2d0f33716d89d9329df2b1f`  
		Last Modified: Tue, 12 Jan 2021 00:51:54 GMT  
		Size: 25.9 MB (25864492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c624bef28ff9228422eef122ec713693eb2e8d2ed78aa41f319bd0678a607c`  
		Last Modified: Tue, 12 Jan 2021 05:15:20 GMT  
		Size: 255.9 KB (255923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ec950da6523b4cb54939edc61c6460d64327528adc05f607fbf005ff508a88`  
		Last Modified: Tue, 12 Jan 2021 05:15:34 GMT  
		Size: 31.7 MB (31720550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0-slim` - linux; 386

```console
$ docker pull mono@sha256:521020ecd687652f6d5c2e2de3a818db2510b049378854f835bfc7caa058746e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99129650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a612a9ed794b39d2f1751626f377d4fe36630334994f4e592e859b2370d5d37`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:55:14 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 03:55:23 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:56:00 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ae7e24292b47c5c54d019f27f833b4d1fd06c6c1760426a915f4626d13ebb5`  
		Last Modified: Tue, 12 Jan 2021 04:01:42 GMT  
		Size: 255.9 KB (255867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723f6fae6c251aafe4f2903014f5ca67d695cd2f74f87cc46b0b9b5e50650a9f`  
		Last Modified: Tue, 12 Jan 2021 04:02:03 GMT  
		Size: 71.1 MB (71105792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12.0-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:fe8b241787171b74a2fd43cd5f13bd303c637bf330e80f289245b9c27b8eb306
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60100071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:638800145fd3d9c6b9e6088d6dd2118832963e6457e99a6a04bfd75078bebd50`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:25:06 GMT
ADD file:9d7252c169da9a089a0caa2f26cea24678267c15c0e129e7320d4defe0d4637b in / 
# Tue, 12 Jan 2021 00:25:16 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:34:09 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 03:35:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:37:38 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:cb701c1e59a3b25dcb09b089f31d61af3065659cd29a7c748f66f3e3c8a96d58`  
		Last Modified: Tue, 12 Jan 2021 00:34:11 GMT  
		Size: 30.5 MB (30532837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e77824b16d99ee079aa03b8aabec031637265f7380c082326eaf48d078a93e7`  
		Last Modified: Tue, 12 Jan 2021 04:01:02 GMT  
		Size: 256.1 KB (256146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8e3bf2452dcba3a8621830f987ddbcc051bd5b6d5817e6d595c1cd93497f67`  
		Last Modified: Tue, 12 Jan 2021 04:01:08 GMT  
		Size: 29.3 MB (29311088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.12-slim`

```console
$ docker pull mono@sha256:28d3578057e16483bef3cb7d9b30c54fa672b8ced049268ad11d96652864336a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6.12-slim` - linux; amd64

```console
$ docker pull mono@sha256:8769207b9677e6f3f0e95b6423c76cdfd5e450f6b32c051db7b91db5577d7e21
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.4 MB (94443211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:348b7e1144c12af5295b3c38dd57ef1b5c6e171ee9409efbbe2bacd0c680eae5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:40:56 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 09:41:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 09:41:33 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe02677df6f8831edfcea8a4558dcbb344dda0a234033ce403a445f71bb95e04`  
		Last Modified: Tue, 12 Jan 2021 09:56:50 GMT  
		Size: 255.9 KB (255924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6f0c1d36d945478bb94f4061ab9e9570a42d064b1bac55d482cc3d9eefdc1b`  
		Last Modified: Tue, 12 Jan 2021 09:57:04 GMT  
		Size: 67.1 MB (67079218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:fbdc9066c014b9853957843c45f789b61596294919443a607a8ccf5749442c7a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51607237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d35599162358d092829e97e4858f0a1073436f41099f7a5b983df6c1b4956954`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:51:34 GMT
ADD file:57136a762436a5d41e60c61db0d89baea17a289845ea55565e45cc79a9e81e23 in / 
# Tue, 12 Jan 2021 00:51:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:58:10 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 01:58:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 01:59:18 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2e2535e18472e7491a1d935b1f44ac842e4cc5c4d3de40cecb77b56b44515910`  
		Last Modified: Tue, 12 Jan 2021 01:00:19 GMT  
		Size: 24.9 MB (24851909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781b0df29588b1d712497221b09542f9b882364892a46ecf5521b50115ffe045`  
		Last Modified: Tue, 12 Jan 2021 02:07:54 GMT  
		Size: 255.9 KB (255947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ccd7e036e1bf04d2229ab088bc370548d6b63d0540abdfa03ab614ff643669e`  
		Last Modified: Tue, 12 Jan 2021 02:08:01 GMT  
		Size: 26.5 MB (26499381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:5feb406d1ce80dd86fc2db709ca76f30c7120ee7a40a712fd7e32899e4bdffb7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48669353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f15fcf95ecaebe203ce057c5d16cbfff554c6d24084bef88355b180812987040`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:01:09 GMT
ADD file:1db27e410cc7caf4a97a7313c57260fd01aa134b84306914ef0948dcca27372d in / 
# Tue, 12 Jan 2021 00:01:12 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:53:47 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 03:54:04 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:54:42 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:be493c6a598447fe5f46a390f3bee10f2d2ba2215d39829fe84eb40a7add18fc`  
		Last Modified: Tue, 12 Jan 2021 00:11:14 GMT  
		Size: 22.7 MB (22715905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c33bdc53ec4d57ecf8d4565fca28d67f043f4855d49b01e900e8ef3c8bb9d6`  
		Last Modified: Tue, 12 Jan 2021 04:03:03 GMT  
		Size: 255.9 KB (255942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d9304eb6e55e2cd3920831bd0dec33588ea625b97a60aa2b06301f9351de819`  
		Last Modified: Tue, 12 Jan 2021 04:03:11 GMT  
		Size: 25.7 MB (25697506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:90a25ba70e6af84267801fd4cbeb308a72f614df951c6c33e9782e140e373538
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.8 MB (57840965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b69b6854e1856fe6d38217029a566ca928db10d685c520adb43f1ecd510f16d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:41:13 GMT
ADD file:0252dccbbfb76766e0e189783d38f6a6afd13f44daa7c5370ffd094adea0f583 in / 
# Tue, 12 Jan 2021 00:41:21 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 05:07:35 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 05:07:52 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 05:08:28 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f8be76fcf2062bd14a3a78f858da701db8bcd907a2d0f33716d89d9329df2b1f`  
		Last Modified: Tue, 12 Jan 2021 00:51:54 GMT  
		Size: 25.9 MB (25864492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c624bef28ff9228422eef122ec713693eb2e8d2ed78aa41f319bd0678a607c`  
		Last Modified: Tue, 12 Jan 2021 05:15:20 GMT  
		Size: 255.9 KB (255923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ec950da6523b4cb54939edc61c6460d64327528adc05f607fbf005ff508a88`  
		Last Modified: Tue, 12 Jan 2021 05:15:34 GMT  
		Size: 31.7 MB (31720550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12-slim` - linux; 386

```console
$ docker pull mono@sha256:521020ecd687652f6d5c2e2de3a818db2510b049378854f835bfc7caa058746e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99129650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a612a9ed794b39d2f1751626f377d4fe36630334994f4e592e859b2370d5d37`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:55:14 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 03:55:23 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:56:00 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ae7e24292b47c5c54d019f27f833b4d1fd06c6c1760426a915f4626d13ebb5`  
		Last Modified: Tue, 12 Jan 2021 04:01:42 GMT  
		Size: 255.9 KB (255867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723f6fae6c251aafe4f2903014f5ca67d695cd2f74f87cc46b0b9b5e50650a9f`  
		Last Modified: Tue, 12 Jan 2021 04:02:03 GMT  
		Size: 71.1 MB (71105792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.12-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:fe8b241787171b74a2fd43cd5f13bd303c637bf330e80f289245b9c27b8eb306
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60100071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:638800145fd3d9c6b9e6088d6dd2118832963e6457e99a6a04bfd75078bebd50`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:25:06 GMT
ADD file:9d7252c169da9a089a0caa2f26cea24678267c15c0e129e7320d4defe0d4637b in / 
# Tue, 12 Jan 2021 00:25:16 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:34:09 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 03:35:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:37:38 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:cb701c1e59a3b25dcb09b089f31d61af3065659cd29a7c748f66f3e3c8a96d58`  
		Last Modified: Tue, 12 Jan 2021 00:34:11 GMT  
		Size: 30.5 MB (30532837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e77824b16d99ee079aa03b8aabec031637265f7380c082326eaf48d078a93e7`  
		Last Modified: Tue, 12 Jan 2021 04:01:02 GMT  
		Size: 256.1 KB (256146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8e3bf2452dcba3a8621830f987ddbcc051bd5b6d5817e6d595c1cd93497f67`  
		Last Modified: Tue, 12 Jan 2021 04:01:08 GMT  
		Size: 29.3 MB (29311088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6-slim`

```console
$ docker pull mono@sha256:28d3578057e16483bef3cb7d9b30c54fa672b8ced049268ad11d96652864336a
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
$ docker pull mono@sha256:8769207b9677e6f3f0e95b6423c76cdfd5e450f6b32c051db7b91db5577d7e21
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.4 MB (94443211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:348b7e1144c12af5295b3c38dd57ef1b5c6e171ee9409efbbe2bacd0c680eae5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:40:56 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 09:41:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 09:41:33 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe02677df6f8831edfcea8a4558dcbb344dda0a234033ce403a445f71bb95e04`  
		Last Modified: Tue, 12 Jan 2021 09:56:50 GMT  
		Size: 255.9 KB (255924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6f0c1d36d945478bb94f4061ab9e9570a42d064b1bac55d482cc3d9eefdc1b`  
		Last Modified: Tue, 12 Jan 2021 09:57:04 GMT  
		Size: 67.1 MB (67079218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:fbdc9066c014b9853957843c45f789b61596294919443a607a8ccf5749442c7a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51607237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d35599162358d092829e97e4858f0a1073436f41099f7a5b983df6c1b4956954`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:51:34 GMT
ADD file:57136a762436a5d41e60c61db0d89baea17a289845ea55565e45cc79a9e81e23 in / 
# Tue, 12 Jan 2021 00:51:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:58:10 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 01:58:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 01:59:18 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2e2535e18472e7491a1d935b1f44ac842e4cc5c4d3de40cecb77b56b44515910`  
		Last Modified: Tue, 12 Jan 2021 01:00:19 GMT  
		Size: 24.9 MB (24851909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781b0df29588b1d712497221b09542f9b882364892a46ecf5521b50115ffe045`  
		Last Modified: Tue, 12 Jan 2021 02:07:54 GMT  
		Size: 255.9 KB (255947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ccd7e036e1bf04d2229ab088bc370548d6b63d0540abdfa03ab614ff643669e`  
		Last Modified: Tue, 12 Jan 2021 02:08:01 GMT  
		Size: 26.5 MB (26499381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:5feb406d1ce80dd86fc2db709ca76f30c7120ee7a40a712fd7e32899e4bdffb7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48669353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f15fcf95ecaebe203ce057c5d16cbfff554c6d24084bef88355b180812987040`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:01:09 GMT
ADD file:1db27e410cc7caf4a97a7313c57260fd01aa134b84306914ef0948dcca27372d in / 
# Tue, 12 Jan 2021 00:01:12 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:53:47 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 03:54:04 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:54:42 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:be493c6a598447fe5f46a390f3bee10f2d2ba2215d39829fe84eb40a7add18fc`  
		Last Modified: Tue, 12 Jan 2021 00:11:14 GMT  
		Size: 22.7 MB (22715905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c33bdc53ec4d57ecf8d4565fca28d67f043f4855d49b01e900e8ef3c8bb9d6`  
		Last Modified: Tue, 12 Jan 2021 04:03:03 GMT  
		Size: 255.9 KB (255942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d9304eb6e55e2cd3920831bd0dec33588ea625b97a60aa2b06301f9351de819`  
		Last Modified: Tue, 12 Jan 2021 04:03:11 GMT  
		Size: 25.7 MB (25697506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:90a25ba70e6af84267801fd4cbeb308a72f614df951c6c33e9782e140e373538
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.8 MB (57840965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b69b6854e1856fe6d38217029a566ca928db10d685c520adb43f1ecd510f16d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:41:13 GMT
ADD file:0252dccbbfb76766e0e189783d38f6a6afd13f44daa7c5370ffd094adea0f583 in / 
# Tue, 12 Jan 2021 00:41:21 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 05:07:35 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 05:07:52 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 05:08:28 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f8be76fcf2062bd14a3a78f858da701db8bcd907a2d0f33716d89d9329df2b1f`  
		Last Modified: Tue, 12 Jan 2021 00:51:54 GMT  
		Size: 25.9 MB (25864492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c624bef28ff9228422eef122ec713693eb2e8d2ed78aa41f319bd0678a607c`  
		Last Modified: Tue, 12 Jan 2021 05:15:20 GMT  
		Size: 255.9 KB (255923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ec950da6523b4cb54939edc61c6460d64327528adc05f607fbf005ff508a88`  
		Last Modified: Tue, 12 Jan 2021 05:15:34 GMT  
		Size: 31.7 MB (31720550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; 386

```console
$ docker pull mono@sha256:521020ecd687652f6d5c2e2de3a818db2510b049378854f835bfc7caa058746e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99129650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a612a9ed794b39d2f1751626f377d4fe36630334994f4e592e859b2370d5d37`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:55:14 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 03:55:23 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:56:00 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ae7e24292b47c5c54d019f27f833b4d1fd06c6c1760426a915f4626d13ebb5`  
		Last Modified: Tue, 12 Jan 2021 04:01:42 GMT  
		Size: 255.9 KB (255867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723f6fae6c251aafe4f2903014f5ca67d695cd2f74f87cc46b0b9b5e50650a9f`  
		Last Modified: Tue, 12 Jan 2021 04:02:03 GMT  
		Size: 71.1 MB (71105792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:fe8b241787171b74a2fd43cd5f13bd303c637bf330e80f289245b9c27b8eb306
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60100071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:638800145fd3d9c6b9e6088d6dd2118832963e6457e99a6a04bfd75078bebd50`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:25:06 GMT
ADD file:9d7252c169da9a089a0caa2f26cea24678267c15c0e129e7320d4defe0d4637b in / 
# Tue, 12 Jan 2021 00:25:16 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:34:09 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 03:35:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:37:38 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:cb701c1e59a3b25dcb09b089f31d61af3065659cd29a7c748f66f3e3c8a96d58`  
		Last Modified: Tue, 12 Jan 2021 00:34:11 GMT  
		Size: 30.5 MB (30532837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e77824b16d99ee079aa03b8aabec031637265f7380c082326eaf48d078a93e7`  
		Last Modified: Tue, 12 Jan 2021 04:01:02 GMT  
		Size: 256.1 KB (256146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8e3bf2452dcba3a8621830f987ddbcc051bd5b6d5817e6d595c1cd93497f67`  
		Last Modified: Tue, 12 Jan 2021 04:01:08 GMT  
		Size: 29.3 MB (29311088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:latest`

```console
$ docker pull mono@sha256:fee59facbee3c69f535f506910bbac808643a8f91f5a80ddc79e478fa5982f58
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
$ docker pull mono@sha256:e3c3faa1e0eccfec442341c7260bfb1faeccf40581fe8a00e77e794cf27d150b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.9 MB (235856726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d02da61afa912e62ef7cdc2e3b89fb6915716c72eccd75293b5c784ba17e5ce`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:40:56 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 09:41:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 09:41:33 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 09:48:29 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe02677df6f8831edfcea8a4558dcbb344dda0a234033ce403a445f71bb95e04`  
		Last Modified: Tue, 12 Jan 2021 09:56:50 GMT  
		Size: 255.9 KB (255924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6f0c1d36d945478bb94f4061ab9e9570a42d064b1bac55d482cc3d9eefdc1b`  
		Last Modified: Tue, 12 Jan 2021 09:57:04 GMT  
		Size: 67.1 MB (67079218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55acb8a81f9716f19bc8b425a4f2f9778868a086ced2c38a0d232c7e149e260b`  
		Last Modified: Tue, 12 Jan 2021 09:58:10 GMT  
		Size: 141.4 MB (141413515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm variant v5

```console
$ docker pull mono@sha256:93e07bd0966ba3af8e1265a2976fa87cf142485c7984e221d5bd1900b1129c04
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.7 MB (191715473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d675a592f2dd1ff1c3d27b04a2e5373c8d8d9fd42ea3e202cf2f0deeabc4a11b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:51:34 GMT
ADD file:57136a762436a5d41e60c61db0d89baea17a289845ea55565e45cc79a9e81e23 in / 
# Tue, 12 Jan 2021 00:51:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:58:10 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 01:58:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 01:59:18 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 02:04:03 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2e2535e18472e7491a1d935b1f44ac842e4cc5c4d3de40cecb77b56b44515910`  
		Last Modified: Tue, 12 Jan 2021 01:00:19 GMT  
		Size: 24.9 MB (24851909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781b0df29588b1d712497221b09542f9b882364892a46ecf5521b50115ffe045`  
		Last Modified: Tue, 12 Jan 2021 02:07:54 GMT  
		Size: 255.9 KB (255947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ccd7e036e1bf04d2229ab088bc370548d6b63d0540abdfa03ab614ff643669e`  
		Last Modified: Tue, 12 Jan 2021 02:08:01 GMT  
		Size: 26.5 MB (26499381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057e315d7d334759ab98965930ff1540b0ca7c9ae700b6bbb74fa1506fed258a`  
		Last Modified: Tue, 12 Jan 2021 02:09:34 GMT  
		Size: 140.1 MB (140108236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm variant v7

```console
$ docker pull mono@sha256:172236fea866d1b739364ba9049c97abc885743e420322f6df0dd72c617ab1d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.6 MB (187612230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f579c6e6d6132fc34dcf39db01f217918a65e0cf5889c53e939eb89bd3453d13`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:01:09 GMT
ADD file:1db27e410cc7caf4a97a7313c57260fd01aa134b84306914ef0948dcca27372d in / 
# Tue, 12 Jan 2021 00:01:12 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:53:47 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 03:54:04 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:54:42 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 03:58:38 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:be493c6a598447fe5f46a390f3bee10f2d2ba2215d39829fe84eb40a7add18fc`  
		Last Modified: Tue, 12 Jan 2021 00:11:14 GMT  
		Size: 22.7 MB (22715905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c33bdc53ec4d57ecf8d4565fca28d67f043f4855d49b01e900e8ef3c8bb9d6`  
		Last Modified: Tue, 12 Jan 2021 04:03:03 GMT  
		Size: 255.9 KB (255942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d9304eb6e55e2cd3920831bd0dec33588ea625b97a60aa2b06301f9351de819`  
		Last Modified: Tue, 12 Jan 2021 04:03:11 GMT  
		Size: 25.7 MB (25697506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1168b3f3ae6bc53dbe989dc4db4fad0b76b83fcb4d4db9dd33f685342c886c`  
		Last Modified: Tue, 12 Jan 2021 04:04:41 GMT  
		Size: 138.9 MB (138942877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:bb8bcb03c776a1d69c8402a77aeb49e7302fca102ab82e11002ca319287ae33a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.4 MB (214424611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a8b3b0d88c8a2f9826ad928f5035cd23a14395c38e57da6f376205bb25ac8d2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:41:13 GMT
ADD file:0252dccbbfb76766e0e189783d38f6a6afd13f44daa7c5370ffd094adea0f583 in / 
# Tue, 12 Jan 2021 00:41:21 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 05:07:35 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 05:07:52 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 05:08:28 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 05:12:14 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f8be76fcf2062bd14a3a78f858da701db8bcd907a2d0f33716d89d9329df2b1f`  
		Last Modified: Tue, 12 Jan 2021 00:51:54 GMT  
		Size: 25.9 MB (25864492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c624bef28ff9228422eef122ec713693eb2e8d2ed78aa41f319bd0678a607c`  
		Last Modified: Tue, 12 Jan 2021 05:15:20 GMT  
		Size: 255.9 KB (255923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ec950da6523b4cb54939edc61c6460d64327528adc05f607fbf005ff508a88`  
		Last Modified: Tue, 12 Jan 2021 05:15:34 GMT  
		Size: 31.7 MB (31720550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0470c4fa675956b4e41164ba69e70c7c53cbf56fa1fde6ca99247fd30d63182`  
		Last Modified: Tue, 12 Jan 2021 05:16:54 GMT  
		Size: 156.6 MB (156583646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; 386

```console
$ docker pull mono@sha256:3f6d7e510f3c7e210af3336de41288b7e8971519c559d7994389b5aaab7ca0d6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.6 MB (241641989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d7d8ae0005ba40c7547dfff94755167dba0e74f722bd8583e10d292d8cc13d2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:55:14 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 03:55:23 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:56:00 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 03:59:02 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ae7e24292b47c5c54d019f27f833b4d1fd06c6c1760426a915f4626d13ebb5`  
		Last Modified: Tue, 12 Jan 2021 04:01:42 GMT  
		Size: 255.9 KB (255867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723f6fae6c251aafe4f2903014f5ca67d695cd2f74f87cc46b0b9b5e50650a9f`  
		Last Modified: Tue, 12 Jan 2021 04:02:03 GMT  
		Size: 71.1 MB (71105792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a6a59d3738ce8d2e6bad95e51859928eac584152411a872b1dfd4ec6cbffe4`  
		Last Modified: Tue, 12 Jan 2021 04:03:29 GMT  
		Size: 142.5 MB (142512339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; ppc64le

```console
$ docker pull mono@sha256:8cd03e8a315754c3631020ef221a2d0cbd0992577901c899c47ce5e69d61dd49
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.3 MB (203325644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be23bd3cc106fdd913dd4eff53c1f46dabb535e753abef0f566dae2c69eaea9d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:25:06 GMT
ADD file:9d7252c169da9a089a0caa2f26cea24678267c15c0e129e7320d4defe0d4637b in / 
# Tue, 12 Jan 2021 00:25:16 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:34:09 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 03:35:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:37:38 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 12 Jan 2021 03:52:04 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:cb701c1e59a3b25dcb09b089f31d61af3065659cd29a7c748f66f3e3c8a96d58`  
		Last Modified: Tue, 12 Jan 2021 00:34:11 GMT  
		Size: 30.5 MB (30532837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e77824b16d99ee079aa03b8aabec031637265f7380c082326eaf48d078a93e7`  
		Last Modified: Tue, 12 Jan 2021 04:01:02 GMT  
		Size: 256.1 KB (256146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8e3bf2452dcba3a8621830f987ddbcc051bd5b6d5817e6d595c1cd93497f67`  
		Last Modified: Tue, 12 Jan 2021 04:01:08 GMT  
		Size: 29.3 MB (29311088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be798b1b9507d975e13d056b87d688839b0f83115176be62486731bf9cac3ed7`  
		Last Modified: Tue, 12 Jan 2021 04:02:25 GMT  
		Size: 143.2 MB (143225573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:slim`

```console
$ docker pull mono@sha256:28d3578057e16483bef3cb7d9b30c54fa672b8ced049268ad11d96652864336a
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
$ docker pull mono@sha256:8769207b9677e6f3f0e95b6423c76cdfd5e450f6b32c051db7b91db5577d7e21
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.4 MB (94443211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:348b7e1144c12af5295b3c38dd57ef1b5c6e171ee9409efbbe2bacd0c680eae5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:40:56 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 09:41:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 09:41:33 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe02677df6f8831edfcea8a4558dcbb344dda0a234033ce403a445f71bb95e04`  
		Last Modified: Tue, 12 Jan 2021 09:56:50 GMT  
		Size: 255.9 KB (255924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6f0c1d36d945478bb94f4061ab9e9570a42d064b1bac55d482cc3d9eefdc1b`  
		Last Modified: Tue, 12 Jan 2021 09:57:04 GMT  
		Size: 67.1 MB (67079218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:fbdc9066c014b9853957843c45f789b61596294919443a607a8ccf5749442c7a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51607237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d35599162358d092829e97e4858f0a1073436f41099f7a5b983df6c1b4956954`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:51:34 GMT
ADD file:57136a762436a5d41e60c61db0d89baea17a289845ea55565e45cc79a9e81e23 in / 
# Tue, 12 Jan 2021 00:51:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:58:10 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 01:58:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 01:59:18 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2e2535e18472e7491a1d935b1f44ac842e4cc5c4d3de40cecb77b56b44515910`  
		Last Modified: Tue, 12 Jan 2021 01:00:19 GMT  
		Size: 24.9 MB (24851909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781b0df29588b1d712497221b09542f9b882364892a46ecf5521b50115ffe045`  
		Last Modified: Tue, 12 Jan 2021 02:07:54 GMT  
		Size: 255.9 KB (255947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ccd7e036e1bf04d2229ab088bc370548d6b63d0540abdfa03ab614ff643669e`  
		Last Modified: Tue, 12 Jan 2021 02:08:01 GMT  
		Size: 26.5 MB (26499381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:5feb406d1ce80dd86fc2db709ca76f30c7120ee7a40a712fd7e32899e4bdffb7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48669353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f15fcf95ecaebe203ce057c5d16cbfff554c6d24084bef88355b180812987040`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:01:09 GMT
ADD file:1db27e410cc7caf4a97a7313c57260fd01aa134b84306914ef0948dcca27372d in / 
# Tue, 12 Jan 2021 00:01:12 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:53:47 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 03:54:04 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:54:42 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:be493c6a598447fe5f46a390f3bee10f2d2ba2215d39829fe84eb40a7add18fc`  
		Last Modified: Tue, 12 Jan 2021 00:11:14 GMT  
		Size: 22.7 MB (22715905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c33bdc53ec4d57ecf8d4565fca28d67f043f4855d49b01e900e8ef3c8bb9d6`  
		Last Modified: Tue, 12 Jan 2021 04:03:03 GMT  
		Size: 255.9 KB (255942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d9304eb6e55e2cd3920831bd0dec33588ea625b97a60aa2b06301f9351de819`  
		Last Modified: Tue, 12 Jan 2021 04:03:11 GMT  
		Size: 25.7 MB (25697506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:90a25ba70e6af84267801fd4cbeb308a72f614df951c6c33e9782e140e373538
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.8 MB (57840965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b69b6854e1856fe6d38217029a566ca928db10d685c520adb43f1ecd510f16d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:41:13 GMT
ADD file:0252dccbbfb76766e0e189783d38f6a6afd13f44daa7c5370ffd094adea0f583 in / 
# Tue, 12 Jan 2021 00:41:21 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 05:07:35 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 05:07:52 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 05:08:28 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f8be76fcf2062bd14a3a78f858da701db8bcd907a2d0f33716d89d9329df2b1f`  
		Last Modified: Tue, 12 Jan 2021 00:51:54 GMT  
		Size: 25.9 MB (25864492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c624bef28ff9228422eef122ec713693eb2e8d2ed78aa41f319bd0678a607c`  
		Last Modified: Tue, 12 Jan 2021 05:15:20 GMT  
		Size: 255.9 KB (255923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ec950da6523b4cb54939edc61c6460d64327528adc05f607fbf005ff508a88`  
		Last Modified: Tue, 12 Jan 2021 05:15:34 GMT  
		Size: 31.7 MB (31720550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; 386

```console
$ docker pull mono@sha256:521020ecd687652f6d5c2e2de3a818db2510b049378854f835bfc7caa058746e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99129650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a612a9ed794b39d2f1751626f377d4fe36630334994f4e592e859b2370d5d37`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:55:14 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 03:55:23 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:56:00 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ae7e24292b47c5c54d019f27f833b4d1fd06c6c1760426a915f4626d13ebb5`  
		Last Modified: Tue, 12 Jan 2021 04:01:42 GMT  
		Size: 255.9 KB (255867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723f6fae6c251aafe4f2903014f5ca67d695cd2f74f87cc46b0b9b5e50650a9f`  
		Last Modified: Tue, 12 Jan 2021 04:02:03 GMT  
		Size: 71.1 MB (71105792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; ppc64le

```console
$ docker pull mono@sha256:fe8b241787171b74a2fd43cd5f13bd303c637bf330e80f289245b9c27b8eb306
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60100071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:638800145fd3d9c6b9e6088d6dd2118832963e6457e99a6a04bfd75078bebd50`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:25:06 GMT
ADD file:9d7252c169da9a089a0caa2f26cea24678267c15c0e129e7320d4defe0d4637b in / 
# Tue, 12 Jan 2021 00:25:16 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:34:09 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 03:35:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:37:38 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:cb701c1e59a3b25dcb09b089f31d61af3065659cd29a7c748f66f3e3c8a96d58`  
		Last Modified: Tue, 12 Jan 2021 00:34:11 GMT  
		Size: 30.5 MB (30532837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e77824b16d99ee079aa03b8aabec031637265f7380c082326eaf48d078a93e7`  
		Last Modified: Tue, 12 Jan 2021 04:01:02 GMT  
		Size: 256.1 KB (256146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8e3bf2452dcba3a8621830f987ddbcc051bd5b6d5817e6d595c1cd93497f67`  
		Last Modified: Tue, 12 Jan 2021 04:01:08 GMT  
		Size: 29.3 MB (29311088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
