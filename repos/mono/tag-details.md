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
$ docker pull mono@sha256:c703c3cc3b1569eeed1d7ea79d7dcba14e25bcd6cad9689fae50addfef2d499d
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
$ docker pull mono@sha256:377607e4ad004a20debc74ccfc614e0cddf31d6c0f6cbcd4dd451354f49206c9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.3 MB (218278331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf689ed03c8271ede81e6f64cf82dca4dd69a91e612bb8c911e0561f112085ab`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 19:33:02 GMT
ENV MONO_VERSION=5.20.1.34
# Fri, 15 May 2020 19:33:14 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 19:33:43 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 15 May 2020 20:05:18 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c687daeabb9e1562a2e501ad178edbc1896eeba1bffa74ce303519407544c563`  
		Last Modified: Fri, 15 May 2020 20:06:34 GMT  
		Size: 244.5 KB (244489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfe077f97d524ba2135e5765f841cc99024ef058b62c32cc792f665c0c673e1`  
		Last Modified: Fri, 15 May 2020 20:06:50 GMT  
		Size: 55.5 MB (55519404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4185ec4ca513ec8f1a25c7e0529e004da55582aaf2c34f36c6f56ccb900614`  
		Last Modified: Fri, 15 May 2020 20:08:33 GMT  
		Size: 140.0 MB (139994551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5` - linux; arm variant v5

```console
$ docker pull mono@sha256:4b124dd6d74336938eead3dcc403c960e9a1b0e1039fd45ed98cc21b65287cce
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.8 MB (170834374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e809d95c92e63388701602eb14bd46453e4dbad3eeea280c1581c54baaf08a6e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 00:55:49 GMT
ADD file:af949d376cc9a2ac87d0052d22fe17be59dfe65905f0645d1a903b359208d26d in / 
# Tue, 09 Jun 2020 00:55:51 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:37:38 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 09 Jun 2020 02:38:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 02:39:06 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 02:48:44 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c9b35828d9245f0a85299b96b2d9b0d70390689cf7df0fe7ef29ca6028c0ab56`  
		Last Modified: Tue, 09 Jun 2020 01:03:09 GMT  
		Size: 21.2 MB (21197337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822ecad80b0922cb6f84e448afb45744aebd13f1bbfa587c873ccf3d48339bf8`  
		Last Modified: Tue, 09 Jun 2020 02:50:04 GMT  
		Size: 244.6 KB (244612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29babd4ca7636c0b81bd94c0fb7bc0af65ce0f1bf052ef66eefdee3d473a1144`  
		Last Modified: Tue, 09 Jun 2020 02:50:12 GMT  
		Size: 24.2 MB (24152312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f1631b36662a98efcaca68ff7bc7e92ffbfba70339fb58fcb98e03817687630`  
		Last Modified: Tue, 09 Jun 2020 02:53:14 GMT  
		Size: 125.2 MB (125240113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5` - linux; arm variant v7

```console
$ docker pull mono@sha256:47e798e8f059ea4993c554451a3517fc8a2786f19c35303531875fa6a4389c70
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.9 MB (166889669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:732f0c5b83272f228983879ebe35637591d8442982acb3899cde395063fa5927`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:06:35 GMT
ADD file:4a0a863669948b35130fcf8cdb52999c49f7b3ee0620a1eef5f1a2e850a42f05 in / 
# Tue, 09 Jun 2020 01:06:37 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:52:41 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 09 Jun 2020 04:53:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:53:50 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 05:01:51 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c439312a9c212b64af3c38cb326bb5fbe14bcf4a622115d59d44985e949bee82`  
		Last Modified: Tue, 09 Jun 2020 01:13:51 GMT  
		Size: 19.3 MB (19304370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0af396ec38b9993232419e5d9219f0077d7145f9b61c7c8920d173d0a618840`  
		Last Modified: Tue, 09 Jun 2020 05:02:59 GMT  
		Size: 244.6 KB (244627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3794bbc29c2fc1f0baf05649349a607118798dc12e37fe275a2d929ebc984a`  
		Last Modified: Tue, 09 Jun 2020 05:03:07 GMT  
		Size: 23.5 MB (23453440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44cae24e612597b8660d9b592587ea079637ccb1e12d4d2fba72bcc2af56397`  
		Last Modified: Tue, 09 Jun 2020 05:05:42 GMT  
		Size: 123.9 MB (123887232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:fd867443d6b38edb7b351a5f08f953107f530d3a0d9fc76a47ba6ab767ea21cc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.7 MB (187697331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61776a2e50d7b9d3c215e6d87d93742c511f700b26c7d724654df01daafcf8a3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:49 GMT
ADD file:c85d28567b6123deb660b71c8b60d92378b5ba15ba5dcf495d9388817dc3aa44 in / 
# Tue, 09 Jun 2020 01:54:52 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 03:26:55 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 09 Jun 2020 03:27:13 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 03:27:54 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 03:36:29 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:622dc742b82743ebf5607b215a65869096390ee41b0a61b5532f859fb94590b1`  
		Last Modified: Tue, 09 Jun 2020 02:00:28 GMT  
		Size: 20.4 MB (20375150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47cfdc0a506e196319f490a8bb5e0036dd589b207aa03c9571763b3ee8dea29f`  
		Last Modified: Tue, 09 Jun 2020 03:37:36 GMT  
		Size: 244.4 KB (244372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6b08527e586e0f80506a226402a72b5cf43e106073bc06aa87862249894d0a`  
		Last Modified: Tue, 09 Jun 2020 03:37:45 GMT  
		Size: 28.0 MB (28049990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da477870a6058bd59427cbbc64d0b14a9abebe5cd6b910fa3ddfe36f278837e0`  
		Last Modified: Tue, 09 Jun 2020 03:40:26 GMT  
		Size: 139.0 MB (139027819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5` - linux; 386

```console
$ docker pull mono@sha256:1ea82d19a0f7414cfe3e98105b310e8d63f06f8f277f3848c6a884b92b77f05b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.7 MB (227671637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bc71aebacae50bcaa4b4f804a23f5f230ae27e5ec7fb10a0f1dd08c3d429ffd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:42:33 GMT
ADD file:8ef252685ffefc58654053bf145c830928a2cf423a6c757180649df772f1523d in / 
# Tue, 09 Jun 2020 01:42:34 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 07:01:47 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 09 Jun 2020 07:02:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 07:02:35 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 07:09:48 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4ffbd6ec7974e514763a8d7d9fcf5e86e9440e2280e6e9561ea373b4bc50588e`  
		Last Modified: Tue, 09 Jun 2020 01:48:28 GMT  
		Size: 23.1 MB (23147892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f35120db9bc30d6de494b0e58b8a74d62fe7a85cdc188357ea98ca2797e839`  
		Last Modified: Tue, 09 Jun 2020 07:11:10 GMT  
		Size: 244.5 KB (244478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d12cec6c246292b2edce2de333f893fefd5d9460042faa8e270bfde498b21612`  
		Last Modified: Tue, 09 Jun 2020 07:11:24 GMT  
		Size: 58.4 MB (58439805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e5499fc7470d9d9b363a6494025ec430b6c28a85a563b44637506b9da2eca2`  
		Last Modified: Tue, 09 Jun 2020 07:13:37 GMT  
		Size: 145.8 MB (145839462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5` - linux; ppc64le

```console
$ docker pull mono@sha256:15c0c9e91312a3cbd18b060a447868b37ba4d2ef668c759b7e1c19f314bf9dd8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.2 MB (173185683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:065963fd30de2ed1faa7464809f20c63f66805ff3dad0867a93e21adeb544c22`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:25:38 GMT
ADD file:41ec53d65aa183c2835f73989c9e4922f818e59774811eaa6e7395e5a36d5eab in / 
# Tue, 09 Jun 2020 01:25:42 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:43:07 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 09 Jun 2020 04:44:25 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:45:52 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 05:04:54 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a29e28607c9b96acae7ff89e56214e4339a87c59e40a6f030fa4cbcaab753f2c`  
		Last Modified: Tue, 09 Jun 2020 01:37:25 GMT  
		Size: 22.8 MB (22791269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d9971248b8a3142c8d28700658bc11b1313694441bf51b7febefd26adddbe1`  
		Last Modified: Tue, 09 Jun 2020 05:06:08 GMT  
		Size: 244.6 KB (244636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c629efc5a0d859723a7100a060a51da7cbe12ff931fcd2edcb1be81b2d112240`  
		Last Modified: Tue, 09 Jun 2020 05:06:13 GMT  
		Size: 24.5 MB (24528005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2764189724404bbc9ecbb4c41c717a46e45a9dd50a25b2aaeaaccb46a9f95d48`  
		Last Modified: Tue, 09 Jun 2020 05:08:21 GMT  
		Size: 125.6 MB (125621773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.20`

```console
$ docker pull mono@sha256:c703c3cc3b1569eeed1d7ea79d7dcba14e25bcd6cad9689fae50addfef2d499d
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
$ docker pull mono@sha256:377607e4ad004a20debc74ccfc614e0cddf31d6c0f6cbcd4dd451354f49206c9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.3 MB (218278331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf689ed03c8271ede81e6f64cf82dca4dd69a91e612bb8c911e0561f112085ab`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 19:33:02 GMT
ENV MONO_VERSION=5.20.1.34
# Fri, 15 May 2020 19:33:14 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 19:33:43 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 15 May 2020 20:05:18 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c687daeabb9e1562a2e501ad178edbc1896eeba1bffa74ce303519407544c563`  
		Last Modified: Fri, 15 May 2020 20:06:34 GMT  
		Size: 244.5 KB (244489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfe077f97d524ba2135e5765f841cc99024ef058b62c32cc792f665c0c673e1`  
		Last Modified: Fri, 15 May 2020 20:06:50 GMT  
		Size: 55.5 MB (55519404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4185ec4ca513ec8f1a25c7e0529e004da55582aaf2c34f36c6f56ccb900614`  
		Last Modified: Fri, 15 May 2020 20:08:33 GMT  
		Size: 140.0 MB (139994551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20` - linux; arm variant v5

```console
$ docker pull mono@sha256:4b124dd6d74336938eead3dcc403c960e9a1b0e1039fd45ed98cc21b65287cce
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.8 MB (170834374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e809d95c92e63388701602eb14bd46453e4dbad3eeea280c1581c54baaf08a6e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 00:55:49 GMT
ADD file:af949d376cc9a2ac87d0052d22fe17be59dfe65905f0645d1a903b359208d26d in / 
# Tue, 09 Jun 2020 00:55:51 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:37:38 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 09 Jun 2020 02:38:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 02:39:06 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 02:48:44 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c9b35828d9245f0a85299b96b2d9b0d70390689cf7df0fe7ef29ca6028c0ab56`  
		Last Modified: Tue, 09 Jun 2020 01:03:09 GMT  
		Size: 21.2 MB (21197337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822ecad80b0922cb6f84e448afb45744aebd13f1bbfa587c873ccf3d48339bf8`  
		Last Modified: Tue, 09 Jun 2020 02:50:04 GMT  
		Size: 244.6 KB (244612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29babd4ca7636c0b81bd94c0fb7bc0af65ce0f1bf052ef66eefdee3d473a1144`  
		Last Modified: Tue, 09 Jun 2020 02:50:12 GMT  
		Size: 24.2 MB (24152312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f1631b36662a98efcaca68ff7bc7e92ffbfba70339fb58fcb98e03817687630`  
		Last Modified: Tue, 09 Jun 2020 02:53:14 GMT  
		Size: 125.2 MB (125240113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20` - linux; arm variant v7

```console
$ docker pull mono@sha256:47e798e8f059ea4993c554451a3517fc8a2786f19c35303531875fa6a4389c70
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.9 MB (166889669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:732f0c5b83272f228983879ebe35637591d8442982acb3899cde395063fa5927`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:06:35 GMT
ADD file:4a0a863669948b35130fcf8cdb52999c49f7b3ee0620a1eef5f1a2e850a42f05 in / 
# Tue, 09 Jun 2020 01:06:37 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:52:41 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 09 Jun 2020 04:53:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:53:50 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 05:01:51 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c439312a9c212b64af3c38cb326bb5fbe14bcf4a622115d59d44985e949bee82`  
		Last Modified: Tue, 09 Jun 2020 01:13:51 GMT  
		Size: 19.3 MB (19304370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0af396ec38b9993232419e5d9219f0077d7145f9b61c7c8920d173d0a618840`  
		Last Modified: Tue, 09 Jun 2020 05:02:59 GMT  
		Size: 244.6 KB (244627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3794bbc29c2fc1f0baf05649349a607118798dc12e37fe275a2d929ebc984a`  
		Last Modified: Tue, 09 Jun 2020 05:03:07 GMT  
		Size: 23.5 MB (23453440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44cae24e612597b8660d9b592587ea079637ccb1e12d4d2fba72bcc2af56397`  
		Last Modified: Tue, 09 Jun 2020 05:05:42 GMT  
		Size: 123.9 MB (123887232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:fd867443d6b38edb7b351a5f08f953107f530d3a0d9fc76a47ba6ab767ea21cc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.7 MB (187697331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61776a2e50d7b9d3c215e6d87d93742c511f700b26c7d724654df01daafcf8a3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:49 GMT
ADD file:c85d28567b6123deb660b71c8b60d92378b5ba15ba5dcf495d9388817dc3aa44 in / 
# Tue, 09 Jun 2020 01:54:52 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 03:26:55 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 09 Jun 2020 03:27:13 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 03:27:54 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 03:36:29 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:622dc742b82743ebf5607b215a65869096390ee41b0a61b5532f859fb94590b1`  
		Last Modified: Tue, 09 Jun 2020 02:00:28 GMT  
		Size: 20.4 MB (20375150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47cfdc0a506e196319f490a8bb5e0036dd589b207aa03c9571763b3ee8dea29f`  
		Last Modified: Tue, 09 Jun 2020 03:37:36 GMT  
		Size: 244.4 KB (244372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6b08527e586e0f80506a226402a72b5cf43e106073bc06aa87862249894d0a`  
		Last Modified: Tue, 09 Jun 2020 03:37:45 GMT  
		Size: 28.0 MB (28049990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da477870a6058bd59427cbbc64d0b14a9abebe5cd6b910fa3ddfe36f278837e0`  
		Last Modified: Tue, 09 Jun 2020 03:40:26 GMT  
		Size: 139.0 MB (139027819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20` - linux; 386

```console
$ docker pull mono@sha256:1ea82d19a0f7414cfe3e98105b310e8d63f06f8f277f3848c6a884b92b77f05b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.7 MB (227671637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bc71aebacae50bcaa4b4f804a23f5f230ae27e5ec7fb10a0f1dd08c3d429ffd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:42:33 GMT
ADD file:8ef252685ffefc58654053bf145c830928a2cf423a6c757180649df772f1523d in / 
# Tue, 09 Jun 2020 01:42:34 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 07:01:47 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 09 Jun 2020 07:02:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 07:02:35 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 07:09:48 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4ffbd6ec7974e514763a8d7d9fcf5e86e9440e2280e6e9561ea373b4bc50588e`  
		Last Modified: Tue, 09 Jun 2020 01:48:28 GMT  
		Size: 23.1 MB (23147892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f35120db9bc30d6de494b0e58b8a74d62fe7a85cdc188357ea98ca2797e839`  
		Last Modified: Tue, 09 Jun 2020 07:11:10 GMT  
		Size: 244.5 KB (244478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d12cec6c246292b2edce2de333f893fefd5d9460042faa8e270bfde498b21612`  
		Last Modified: Tue, 09 Jun 2020 07:11:24 GMT  
		Size: 58.4 MB (58439805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e5499fc7470d9d9b363a6494025ec430b6c28a85a563b44637506b9da2eca2`  
		Last Modified: Tue, 09 Jun 2020 07:13:37 GMT  
		Size: 145.8 MB (145839462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20` - linux; ppc64le

```console
$ docker pull mono@sha256:15c0c9e91312a3cbd18b060a447868b37ba4d2ef668c759b7e1c19f314bf9dd8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.2 MB (173185683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:065963fd30de2ed1faa7464809f20c63f66805ff3dad0867a93e21adeb544c22`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:25:38 GMT
ADD file:41ec53d65aa183c2835f73989c9e4922f818e59774811eaa6e7395e5a36d5eab in / 
# Tue, 09 Jun 2020 01:25:42 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:43:07 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 09 Jun 2020 04:44:25 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:45:52 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 05:04:54 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a29e28607c9b96acae7ff89e56214e4339a87c59e40a6f030fa4cbcaab753f2c`  
		Last Modified: Tue, 09 Jun 2020 01:37:25 GMT  
		Size: 22.8 MB (22791269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d9971248b8a3142c8d28700658bc11b1313694441bf51b7febefd26adddbe1`  
		Last Modified: Tue, 09 Jun 2020 05:06:08 GMT  
		Size: 244.6 KB (244636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c629efc5a0d859723a7100a060a51da7cbe12ff931fcd2edcb1be81b2d112240`  
		Last Modified: Tue, 09 Jun 2020 05:06:13 GMT  
		Size: 24.5 MB (24528005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2764189724404bbc9ecbb4c41c717a46e45a9dd50a25b2aaeaaccb46a9f95d48`  
		Last Modified: Tue, 09 Jun 2020 05:08:21 GMT  
		Size: 125.6 MB (125621773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.20.1`

```console
$ docker pull mono@sha256:c703c3cc3b1569eeed1d7ea79d7dcba14e25bcd6cad9689fae50addfef2d499d
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
$ docker pull mono@sha256:377607e4ad004a20debc74ccfc614e0cddf31d6c0f6cbcd4dd451354f49206c9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.3 MB (218278331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf689ed03c8271ede81e6f64cf82dca4dd69a91e612bb8c911e0561f112085ab`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 19:33:02 GMT
ENV MONO_VERSION=5.20.1.34
# Fri, 15 May 2020 19:33:14 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 19:33:43 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 15 May 2020 20:05:18 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c687daeabb9e1562a2e501ad178edbc1896eeba1bffa74ce303519407544c563`  
		Last Modified: Fri, 15 May 2020 20:06:34 GMT  
		Size: 244.5 KB (244489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfe077f97d524ba2135e5765f841cc99024ef058b62c32cc792f665c0c673e1`  
		Last Modified: Fri, 15 May 2020 20:06:50 GMT  
		Size: 55.5 MB (55519404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4185ec4ca513ec8f1a25c7e0529e004da55582aaf2c34f36c6f56ccb900614`  
		Last Modified: Fri, 15 May 2020 20:08:33 GMT  
		Size: 140.0 MB (139994551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1` - linux; arm variant v5

```console
$ docker pull mono@sha256:4b124dd6d74336938eead3dcc403c960e9a1b0e1039fd45ed98cc21b65287cce
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.8 MB (170834374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e809d95c92e63388701602eb14bd46453e4dbad3eeea280c1581c54baaf08a6e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 00:55:49 GMT
ADD file:af949d376cc9a2ac87d0052d22fe17be59dfe65905f0645d1a903b359208d26d in / 
# Tue, 09 Jun 2020 00:55:51 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:37:38 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 09 Jun 2020 02:38:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 02:39:06 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 02:48:44 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c9b35828d9245f0a85299b96b2d9b0d70390689cf7df0fe7ef29ca6028c0ab56`  
		Last Modified: Tue, 09 Jun 2020 01:03:09 GMT  
		Size: 21.2 MB (21197337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822ecad80b0922cb6f84e448afb45744aebd13f1bbfa587c873ccf3d48339bf8`  
		Last Modified: Tue, 09 Jun 2020 02:50:04 GMT  
		Size: 244.6 KB (244612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29babd4ca7636c0b81bd94c0fb7bc0af65ce0f1bf052ef66eefdee3d473a1144`  
		Last Modified: Tue, 09 Jun 2020 02:50:12 GMT  
		Size: 24.2 MB (24152312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f1631b36662a98efcaca68ff7bc7e92ffbfba70339fb58fcb98e03817687630`  
		Last Modified: Tue, 09 Jun 2020 02:53:14 GMT  
		Size: 125.2 MB (125240113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1` - linux; arm variant v7

```console
$ docker pull mono@sha256:47e798e8f059ea4993c554451a3517fc8a2786f19c35303531875fa6a4389c70
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.9 MB (166889669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:732f0c5b83272f228983879ebe35637591d8442982acb3899cde395063fa5927`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:06:35 GMT
ADD file:4a0a863669948b35130fcf8cdb52999c49f7b3ee0620a1eef5f1a2e850a42f05 in / 
# Tue, 09 Jun 2020 01:06:37 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:52:41 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 09 Jun 2020 04:53:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:53:50 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 05:01:51 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c439312a9c212b64af3c38cb326bb5fbe14bcf4a622115d59d44985e949bee82`  
		Last Modified: Tue, 09 Jun 2020 01:13:51 GMT  
		Size: 19.3 MB (19304370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0af396ec38b9993232419e5d9219f0077d7145f9b61c7c8920d173d0a618840`  
		Last Modified: Tue, 09 Jun 2020 05:02:59 GMT  
		Size: 244.6 KB (244627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3794bbc29c2fc1f0baf05649349a607118798dc12e37fe275a2d929ebc984a`  
		Last Modified: Tue, 09 Jun 2020 05:03:07 GMT  
		Size: 23.5 MB (23453440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44cae24e612597b8660d9b592587ea079637ccb1e12d4d2fba72bcc2af56397`  
		Last Modified: Tue, 09 Jun 2020 05:05:42 GMT  
		Size: 123.9 MB (123887232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:fd867443d6b38edb7b351a5f08f953107f530d3a0d9fc76a47ba6ab767ea21cc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.7 MB (187697331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61776a2e50d7b9d3c215e6d87d93742c511f700b26c7d724654df01daafcf8a3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:49 GMT
ADD file:c85d28567b6123deb660b71c8b60d92378b5ba15ba5dcf495d9388817dc3aa44 in / 
# Tue, 09 Jun 2020 01:54:52 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 03:26:55 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 09 Jun 2020 03:27:13 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 03:27:54 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 03:36:29 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:622dc742b82743ebf5607b215a65869096390ee41b0a61b5532f859fb94590b1`  
		Last Modified: Tue, 09 Jun 2020 02:00:28 GMT  
		Size: 20.4 MB (20375150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47cfdc0a506e196319f490a8bb5e0036dd589b207aa03c9571763b3ee8dea29f`  
		Last Modified: Tue, 09 Jun 2020 03:37:36 GMT  
		Size: 244.4 KB (244372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6b08527e586e0f80506a226402a72b5cf43e106073bc06aa87862249894d0a`  
		Last Modified: Tue, 09 Jun 2020 03:37:45 GMT  
		Size: 28.0 MB (28049990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da477870a6058bd59427cbbc64d0b14a9abebe5cd6b910fa3ddfe36f278837e0`  
		Last Modified: Tue, 09 Jun 2020 03:40:26 GMT  
		Size: 139.0 MB (139027819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1` - linux; 386

```console
$ docker pull mono@sha256:1ea82d19a0f7414cfe3e98105b310e8d63f06f8f277f3848c6a884b92b77f05b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.7 MB (227671637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bc71aebacae50bcaa4b4f804a23f5f230ae27e5ec7fb10a0f1dd08c3d429ffd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:42:33 GMT
ADD file:8ef252685ffefc58654053bf145c830928a2cf423a6c757180649df772f1523d in / 
# Tue, 09 Jun 2020 01:42:34 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 07:01:47 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 09 Jun 2020 07:02:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 07:02:35 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 07:09:48 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4ffbd6ec7974e514763a8d7d9fcf5e86e9440e2280e6e9561ea373b4bc50588e`  
		Last Modified: Tue, 09 Jun 2020 01:48:28 GMT  
		Size: 23.1 MB (23147892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f35120db9bc30d6de494b0e58b8a74d62fe7a85cdc188357ea98ca2797e839`  
		Last Modified: Tue, 09 Jun 2020 07:11:10 GMT  
		Size: 244.5 KB (244478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d12cec6c246292b2edce2de333f893fefd5d9460042faa8e270bfde498b21612`  
		Last Modified: Tue, 09 Jun 2020 07:11:24 GMT  
		Size: 58.4 MB (58439805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e5499fc7470d9d9b363a6494025ec430b6c28a85a563b44637506b9da2eca2`  
		Last Modified: Tue, 09 Jun 2020 07:13:37 GMT  
		Size: 145.8 MB (145839462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1` - linux; ppc64le

```console
$ docker pull mono@sha256:15c0c9e91312a3cbd18b060a447868b37ba4d2ef668c759b7e1c19f314bf9dd8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.2 MB (173185683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:065963fd30de2ed1faa7464809f20c63f66805ff3dad0867a93e21adeb544c22`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:25:38 GMT
ADD file:41ec53d65aa183c2835f73989c9e4922f818e59774811eaa6e7395e5a36d5eab in / 
# Tue, 09 Jun 2020 01:25:42 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:43:07 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 09 Jun 2020 04:44:25 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:45:52 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 05:04:54 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a29e28607c9b96acae7ff89e56214e4339a87c59e40a6f030fa4cbcaab753f2c`  
		Last Modified: Tue, 09 Jun 2020 01:37:25 GMT  
		Size: 22.8 MB (22791269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d9971248b8a3142c8d28700658bc11b1313694441bf51b7febefd26adddbe1`  
		Last Modified: Tue, 09 Jun 2020 05:06:08 GMT  
		Size: 244.6 KB (244636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c629efc5a0d859723a7100a060a51da7cbe12ff931fcd2edcb1be81b2d112240`  
		Last Modified: Tue, 09 Jun 2020 05:06:13 GMT  
		Size: 24.5 MB (24528005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2764189724404bbc9ecbb4c41c717a46e45a9dd50a25b2aaeaaccb46a9f95d48`  
		Last Modified: Tue, 09 Jun 2020 05:08:21 GMT  
		Size: 125.6 MB (125621773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.20.1.34`

```console
$ docker pull mono@sha256:c703c3cc3b1569eeed1d7ea79d7dcba14e25bcd6cad9689fae50addfef2d499d
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
$ docker pull mono@sha256:377607e4ad004a20debc74ccfc614e0cddf31d6c0f6cbcd4dd451354f49206c9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.3 MB (218278331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf689ed03c8271ede81e6f64cf82dca4dd69a91e612bb8c911e0561f112085ab`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 19:33:02 GMT
ENV MONO_VERSION=5.20.1.34
# Fri, 15 May 2020 19:33:14 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 19:33:43 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 15 May 2020 20:05:18 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c687daeabb9e1562a2e501ad178edbc1896eeba1bffa74ce303519407544c563`  
		Last Modified: Fri, 15 May 2020 20:06:34 GMT  
		Size: 244.5 KB (244489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfe077f97d524ba2135e5765f841cc99024ef058b62c32cc792f665c0c673e1`  
		Last Modified: Fri, 15 May 2020 20:06:50 GMT  
		Size: 55.5 MB (55519404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4185ec4ca513ec8f1a25c7e0529e004da55582aaf2c34f36c6f56ccb900614`  
		Last Modified: Fri, 15 May 2020 20:08:33 GMT  
		Size: 140.0 MB (139994551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1.34` - linux; arm variant v5

```console
$ docker pull mono@sha256:4b124dd6d74336938eead3dcc403c960e9a1b0e1039fd45ed98cc21b65287cce
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.8 MB (170834374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e809d95c92e63388701602eb14bd46453e4dbad3eeea280c1581c54baaf08a6e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 00:55:49 GMT
ADD file:af949d376cc9a2ac87d0052d22fe17be59dfe65905f0645d1a903b359208d26d in / 
# Tue, 09 Jun 2020 00:55:51 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:37:38 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 09 Jun 2020 02:38:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 02:39:06 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 02:48:44 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c9b35828d9245f0a85299b96b2d9b0d70390689cf7df0fe7ef29ca6028c0ab56`  
		Last Modified: Tue, 09 Jun 2020 01:03:09 GMT  
		Size: 21.2 MB (21197337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822ecad80b0922cb6f84e448afb45744aebd13f1bbfa587c873ccf3d48339bf8`  
		Last Modified: Tue, 09 Jun 2020 02:50:04 GMT  
		Size: 244.6 KB (244612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29babd4ca7636c0b81bd94c0fb7bc0af65ce0f1bf052ef66eefdee3d473a1144`  
		Last Modified: Tue, 09 Jun 2020 02:50:12 GMT  
		Size: 24.2 MB (24152312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f1631b36662a98efcaca68ff7bc7e92ffbfba70339fb58fcb98e03817687630`  
		Last Modified: Tue, 09 Jun 2020 02:53:14 GMT  
		Size: 125.2 MB (125240113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1.34` - linux; arm variant v7

```console
$ docker pull mono@sha256:47e798e8f059ea4993c554451a3517fc8a2786f19c35303531875fa6a4389c70
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.9 MB (166889669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:732f0c5b83272f228983879ebe35637591d8442982acb3899cde395063fa5927`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:06:35 GMT
ADD file:4a0a863669948b35130fcf8cdb52999c49f7b3ee0620a1eef5f1a2e850a42f05 in / 
# Tue, 09 Jun 2020 01:06:37 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:52:41 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 09 Jun 2020 04:53:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:53:50 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 05:01:51 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c439312a9c212b64af3c38cb326bb5fbe14bcf4a622115d59d44985e949bee82`  
		Last Modified: Tue, 09 Jun 2020 01:13:51 GMT  
		Size: 19.3 MB (19304370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0af396ec38b9993232419e5d9219f0077d7145f9b61c7c8920d173d0a618840`  
		Last Modified: Tue, 09 Jun 2020 05:02:59 GMT  
		Size: 244.6 KB (244627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3794bbc29c2fc1f0baf05649349a607118798dc12e37fe275a2d929ebc984a`  
		Last Modified: Tue, 09 Jun 2020 05:03:07 GMT  
		Size: 23.5 MB (23453440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44cae24e612597b8660d9b592587ea079637ccb1e12d4d2fba72bcc2af56397`  
		Last Modified: Tue, 09 Jun 2020 05:05:42 GMT  
		Size: 123.9 MB (123887232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1.34` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:fd867443d6b38edb7b351a5f08f953107f530d3a0d9fc76a47ba6ab767ea21cc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.7 MB (187697331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61776a2e50d7b9d3c215e6d87d93742c511f700b26c7d724654df01daafcf8a3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:49 GMT
ADD file:c85d28567b6123deb660b71c8b60d92378b5ba15ba5dcf495d9388817dc3aa44 in / 
# Tue, 09 Jun 2020 01:54:52 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 03:26:55 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 09 Jun 2020 03:27:13 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 03:27:54 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 03:36:29 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:622dc742b82743ebf5607b215a65869096390ee41b0a61b5532f859fb94590b1`  
		Last Modified: Tue, 09 Jun 2020 02:00:28 GMT  
		Size: 20.4 MB (20375150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47cfdc0a506e196319f490a8bb5e0036dd589b207aa03c9571763b3ee8dea29f`  
		Last Modified: Tue, 09 Jun 2020 03:37:36 GMT  
		Size: 244.4 KB (244372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6b08527e586e0f80506a226402a72b5cf43e106073bc06aa87862249894d0a`  
		Last Modified: Tue, 09 Jun 2020 03:37:45 GMT  
		Size: 28.0 MB (28049990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da477870a6058bd59427cbbc64d0b14a9abebe5cd6b910fa3ddfe36f278837e0`  
		Last Modified: Tue, 09 Jun 2020 03:40:26 GMT  
		Size: 139.0 MB (139027819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1.34` - linux; 386

```console
$ docker pull mono@sha256:1ea82d19a0f7414cfe3e98105b310e8d63f06f8f277f3848c6a884b92b77f05b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.7 MB (227671637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bc71aebacae50bcaa4b4f804a23f5f230ae27e5ec7fb10a0f1dd08c3d429ffd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:42:33 GMT
ADD file:8ef252685ffefc58654053bf145c830928a2cf423a6c757180649df772f1523d in / 
# Tue, 09 Jun 2020 01:42:34 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 07:01:47 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 09 Jun 2020 07:02:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 07:02:35 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 07:09:48 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4ffbd6ec7974e514763a8d7d9fcf5e86e9440e2280e6e9561ea373b4bc50588e`  
		Last Modified: Tue, 09 Jun 2020 01:48:28 GMT  
		Size: 23.1 MB (23147892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f35120db9bc30d6de494b0e58b8a74d62fe7a85cdc188357ea98ca2797e839`  
		Last Modified: Tue, 09 Jun 2020 07:11:10 GMT  
		Size: 244.5 KB (244478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d12cec6c246292b2edce2de333f893fefd5d9460042faa8e270bfde498b21612`  
		Last Modified: Tue, 09 Jun 2020 07:11:24 GMT  
		Size: 58.4 MB (58439805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e5499fc7470d9d9b363a6494025ec430b6c28a85a563b44637506b9da2eca2`  
		Last Modified: Tue, 09 Jun 2020 07:13:37 GMT  
		Size: 145.8 MB (145839462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1.34` - linux; ppc64le

```console
$ docker pull mono@sha256:15c0c9e91312a3cbd18b060a447868b37ba4d2ef668c759b7e1c19f314bf9dd8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.2 MB (173185683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:065963fd30de2ed1faa7464809f20c63f66805ff3dad0867a93e21adeb544c22`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:25:38 GMT
ADD file:41ec53d65aa183c2835f73989c9e4922f818e59774811eaa6e7395e5a36d5eab in / 
# Tue, 09 Jun 2020 01:25:42 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:43:07 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 09 Jun 2020 04:44:25 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:45:52 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 05:04:54 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a29e28607c9b96acae7ff89e56214e4339a87c59e40a6f030fa4cbcaab753f2c`  
		Last Modified: Tue, 09 Jun 2020 01:37:25 GMT  
		Size: 22.8 MB (22791269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d9971248b8a3142c8d28700658bc11b1313694441bf51b7febefd26adddbe1`  
		Last Modified: Tue, 09 Jun 2020 05:06:08 GMT  
		Size: 244.6 KB (244636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c629efc5a0d859723a7100a060a51da7cbe12ff931fcd2edcb1be81b2d112240`  
		Last Modified: Tue, 09 Jun 2020 05:06:13 GMT  
		Size: 24.5 MB (24528005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2764189724404bbc9ecbb4c41c717a46e45a9dd50a25b2aaeaaccb46a9f95d48`  
		Last Modified: Tue, 09 Jun 2020 05:08:21 GMT  
		Size: 125.6 MB (125621773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.20.1.34-slim`

```console
$ docker pull mono@sha256:eb687407e3866b90bbcbdf0989319656db2c4d419b1ac116a631a7da31b55c4b
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
$ docker pull mono@sha256:d9c9b346a27d528a42518d4ef2bab39267a82ae1df0c1e27ca9e444a03b55648
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78283780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8883015efde8b38b153a2d68418a8368d898879cbf16d21811f5229efaeae853`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 19:33:02 GMT
ENV MONO_VERSION=5.20.1.34
# Fri, 15 May 2020 19:33:14 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 19:33:43 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c687daeabb9e1562a2e501ad178edbc1896eeba1bffa74ce303519407544c563`  
		Last Modified: Fri, 15 May 2020 20:06:34 GMT  
		Size: 244.5 KB (244489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfe077f97d524ba2135e5765f841cc99024ef058b62c32cc792f665c0c673e1`  
		Last Modified: Fri, 15 May 2020 20:06:50 GMT  
		Size: 55.5 MB (55519404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1.34-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:d1f2f6bfe520121a7e691cf8e461231bbb14f1e5c3eb5ee47a35ef036f8417ea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45594261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69e15644afe22231412b14df325238c1e07e59bd7605e734dc01523501da96bd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 00:55:49 GMT
ADD file:af949d376cc9a2ac87d0052d22fe17be59dfe65905f0645d1a903b359208d26d in / 
# Tue, 09 Jun 2020 00:55:51 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:37:38 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 09 Jun 2020 02:38:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 02:39:06 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c9b35828d9245f0a85299b96b2d9b0d70390689cf7df0fe7ef29ca6028c0ab56`  
		Last Modified: Tue, 09 Jun 2020 01:03:09 GMT  
		Size: 21.2 MB (21197337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822ecad80b0922cb6f84e448afb45744aebd13f1bbfa587c873ccf3d48339bf8`  
		Last Modified: Tue, 09 Jun 2020 02:50:04 GMT  
		Size: 244.6 KB (244612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29babd4ca7636c0b81bd94c0fb7bc0af65ce0f1bf052ef66eefdee3d473a1144`  
		Last Modified: Tue, 09 Jun 2020 02:50:12 GMT  
		Size: 24.2 MB (24152312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1.34-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:31730ec67bfb195b239af6d38c20919b8393436676c52e52bfd9bad2b913213a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.0 MB (43002437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9aa26f1b857c100cd4b18663f267ac17dd83282d95d7b87ca6d279cf50b19b96`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:06:35 GMT
ADD file:4a0a863669948b35130fcf8cdb52999c49f7b3ee0620a1eef5f1a2e850a42f05 in / 
# Tue, 09 Jun 2020 01:06:37 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:52:41 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 09 Jun 2020 04:53:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:53:50 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c439312a9c212b64af3c38cb326bb5fbe14bcf4a622115d59d44985e949bee82`  
		Last Modified: Tue, 09 Jun 2020 01:13:51 GMT  
		Size: 19.3 MB (19304370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0af396ec38b9993232419e5d9219f0077d7145f9b61c7c8920d173d0a618840`  
		Last Modified: Tue, 09 Jun 2020 05:02:59 GMT  
		Size: 244.6 KB (244627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3794bbc29c2fc1f0baf05649349a607118798dc12e37fe275a2d929ebc984a`  
		Last Modified: Tue, 09 Jun 2020 05:03:07 GMT  
		Size: 23.5 MB (23453440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1.34-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:48d8d81739bb780c0f6f54e39773ed7239fa34117e4baed155af459bdc7bb08e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48669512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4ef5ae213ee661f770b0931778cc05a349d7bac270e37715b391431cb89a305`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:49 GMT
ADD file:c85d28567b6123deb660b71c8b60d92378b5ba15ba5dcf495d9388817dc3aa44 in / 
# Tue, 09 Jun 2020 01:54:52 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 03:26:55 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 09 Jun 2020 03:27:13 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 03:27:54 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:622dc742b82743ebf5607b215a65869096390ee41b0a61b5532f859fb94590b1`  
		Last Modified: Tue, 09 Jun 2020 02:00:28 GMT  
		Size: 20.4 MB (20375150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47cfdc0a506e196319f490a8bb5e0036dd589b207aa03c9571763b3ee8dea29f`  
		Last Modified: Tue, 09 Jun 2020 03:37:36 GMT  
		Size: 244.4 KB (244372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6b08527e586e0f80506a226402a72b5cf43e106073bc06aa87862249894d0a`  
		Last Modified: Tue, 09 Jun 2020 03:37:45 GMT  
		Size: 28.0 MB (28049990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1.34-slim` - linux; 386

```console
$ docker pull mono@sha256:4222a99c9b296042587b96f689ebbf6634a8d8d2c635c4cd04d351e97712e0b9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.8 MB (81832175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4614f168389960f66e555809e63b35524bfd333eae47ec3048ab9ceb067a573`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:42:33 GMT
ADD file:8ef252685ffefc58654053bf145c830928a2cf423a6c757180649df772f1523d in / 
# Tue, 09 Jun 2020 01:42:34 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 07:01:47 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 09 Jun 2020 07:02:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 07:02:35 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4ffbd6ec7974e514763a8d7d9fcf5e86e9440e2280e6e9561ea373b4bc50588e`  
		Last Modified: Tue, 09 Jun 2020 01:48:28 GMT  
		Size: 23.1 MB (23147892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f35120db9bc30d6de494b0e58b8a74d62fe7a85cdc188357ea98ca2797e839`  
		Last Modified: Tue, 09 Jun 2020 07:11:10 GMT  
		Size: 244.5 KB (244478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d12cec6c246292b2edce2de333f893fefd5d9460042faa8e270bfde498b21612`  
		Last Modified: Tue, 09 Jun 2020 07:11:24 GMT  
		Size: 58.4 MB (58439805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1.34-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:176998bc9e1646c37ff64d0d4f385f36e1f8922f56319d19bb3c38f981738c0d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47563910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:406b118562a7fad8d6cb5ebd56d606c3007c1d31422152f7a9d5141a7803798b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:25:38 GMT
ADD file:41ec53d65aa183c2835f73989c9e4922f818e59774811eaa6e7395e5a36d5eab in / 
# Tue, 09 Jun 2020 01:25:42 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:43:07 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 09 Jun 2020 04:44:25 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:45:52 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a29e28607c9b96acae7ff89e56214e4339a87c59e40a6f030fa4cbcaab753f2c`  
		Last Modified: Tue, 09 Jun 2020 01:37:25 GMT  
		Size: 22.8 MB (22791269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d9971248b8a3142c8d28700658bc11b1313694441bf51b7febefd26adddbe1`  
		Last Modified: Tue, 09 Jun 2020 05:06:08 GMT  
		Size: 244.6 KB (244636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c629efc5a0d859723a7100a060a51da7cbe12ff931fcd2edcb1be81b2d112240`  
		Last Modified: Tue, 09 Jun 2020 05:06:13 GMT  
		Size: 24.5 MB (24528005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.20.1-slim`

```console
$ docker pull mono@sha256:eb687407e3866b90bbcbdf0989319656db2c4d419b1ac116a631a7da31b55c4b
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
$ docker pull mono@sha256:d9c9b346a27d528a42518d4ef2bab39267a82ae1df0c1e27ca9e444a03b55648
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78283780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8883015efde8b38b153a2d68418a8368d898879cbf16d21811f5229efaeae853`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 19:33:02 GMT
ENV MONO_VERSION=5.20.1.34
# Fri, 15 May 2020 19:33:14 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 19:33:43 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c687daeabb9e1562a2e501ad178edbc1896eeba1bffa74ce303519407544c563`  
		Last Modified: Fri, 15 May 2020 20:06:34 GMT  
		Size: 244.5 KB (244489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfe077f97d524ba2135e5765f841cc99024ef058b62c32cc792f665c0c673e1`  
		Last Modified: Fri, 15 May 2020 20:06:50 GMT  
		Size: 55.5 MB (55519404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:d1f2f6bfe520121a7e691cf8e461231bbb14f1e5c3eb5ee47a35ef036f8417ea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45594261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69e15644afe22231412b14df325238c1e07e59bd7605e734dc01523501da96bd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 00:55:49 GMT
ADD file:af949d376cc9a2ac87d0052d22fe17be59dfe65905f0645d1a903b359208d26d in / 
# Tue, 09 Jun 2020 00:55:51 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:37:38 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 09 Jun 2020 02:38:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 02:39:06 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c9b35828d9245f0a85299b96b2d9b0d70390689cf7df0fe7ef29ca6028c0ab56`  
		Last Modified: Tue, 09 Jun 2020 01:03:09 GMT  
		Size: 21.2 MB (21197337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822ecad80b0922cb6f84e448afb45744aebd13f1bbfa587c873ccf3d48339bf8`  
		Last Modified: Tue, 09 Jun 2020 02:50:04 GMT  
		Size: 244.6 KB (244612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29babd4ca7636c0b81bd94c0fb7bc0af65ce0f1bf052ef66eefdee3d473a1144`  
		Last Modified: Tue, 09 Jun 2020 02:50:12 GMT  
		Size: 24.2 MB (24152312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:31730ec67bfb195b239af6d38c20919b8393436676c52e52bfd9bad2b913213a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.0 MB (43002437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9aa26f1b857c100cd4b18663f267ac17dd83282d95d7b87ca6d279cf50b19b96`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:06:35 GMT
ADD file:4a0a863669948b35130fcf8cdb52999c49f7b3ee0620a1eef5f1a2e850a42f05 in / 
# Tue, 09 Jun 2020 01:06:37 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:52:41 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 09 Jun 2020 04:53:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:53:50 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c439312a9c212b64af3c38cb326bb5fbe14bcf4a622115d59d44985e949bee82`  
		Last Modified: Tue, 09 Jun 2020 01:13:51 GMT  
		Size: 19.3 MB (19304370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0af396ec38b9993232419e5d9219f0077d7145f9b61c7c8920d173d0a618840`  
		Last Modified: Tue, 09 Jun 2020 05:02:59 GMT  
		Size: 244.6 KB (244627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3794bbc29c2fc1f0baf05649349a607118798dc12e37fe275a2d929ebc984a`  
		Last Modified: Tue, 09 Jun 2020 05:03:07 GMT  
		Size: 23.5 MB (23453440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:48d8d81739bb780c0f6f54e39773ed7239fa34117e4baed155af459bdc7bb08e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48669512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4ef5ae213ee661f770b0931778cc05a349d7bac270e37715b391431cb89a305`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:49 GMT
ADD file:c85d28567b6123deb660b71c8b60d92378b5ba15ba5dcf495d9388817dc3aa44 in / 
# Tue, 09 Jun 2020 01:54:52 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 03:26:55 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 09 Jun 2020 03:27:13 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 03:27:54 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:622dc742b82743ebf5607b215a65869096390ee41b0a61b5532f859fb94590b1`  
		Last Modified: Tue, 09 Jun 2020 02:00:28 GMT  
		Size: 20.4 MB (20375150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47cfdc0a506e196319f490a8bb5e0036dd589b207aa03c9571763b3ee8dea29f`  
		Last Modified: Tue, 09 Jun 2020 03:37:36 GMT  
		Size: 244.4 KB (244372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6b08527e586e0f80506a226402a72b5cf43e106073bc06aa87862249894d0a`  
		Last Modified: Tue, 09 Jun 2020 03:37:45 GMT  
		Size: 28.0 MB (28049990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1-slim` - linux; 386

```console
$ docker pull mono@sha256:4222a99c9b296042587b96f689ebbf6634a8d8d2c635c4cd04d351e97712e0b9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.8 MB (81832175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4614f168389960f66e555809e63b35524bfd333eae47ec3048ab9ceb067a573`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:42:33 GMT
ADD file:8ef252685ffefc58654053bf145c830928a2cf423a6c757180649df772f1523d in / 
# Tue, 09 Jun 2020 01:42:34 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 07:01:47 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 09 Jun 2020 07:02:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 07:02:35 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4ffbd6ec7974e514763a8d7d9fcf5e86e9440e2280e6e9561ea373b4bc50588e`  
		Last Modified: Tue, 09 Jun 2020 01:48:28 GMT  
		Size: 23.1 MB (23147892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f35120db9bc30d6de494b0e58b8a74d62fe7a85cdc188357ea98ca2797e839`  
		Last Modified: Tue, 09 Jun 2020 07:11:10 GMT  
		Size: 244.5 KB (244478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d12cec6c246292b2edce2de333f893fefd5d9460042faa8e270bfde498b21612`  
		Last Modified: Tue, 09 Jun 2020 07:11:24 GMT  
		Size: 58.4 MB (58439805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20.1-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:176998bc9e1646c37ff64d0d4f385f36e1f8922f56319d19bb3c38f981738c0d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47563910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:406b118562a7fad8d6cb5ebd56d606c3007c1d31422152f7a9d5141a7803798b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:25:38 GMT
ADD file:41ec53d65aa183c2835f73989c9e4922f818e59774811eaa6e7395e5a36d5eab in / 
# Tue, 09 Jun 2020 01:25:42 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:43:07 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 09 Jun 2020 04:44:25 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:45:52 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a29e28607c9b96acae7ff89e56214e4339a87c59e40a6f030fa4cbcaab753f2c`  
		Last Modified: Tue, 09 Jun 2020 01:37:25 GMT  
		Size: 22.8 MB (22791269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d9971248b8a3142c8d28700658bc11b1313694441bf51b7febefd26adddbe1`  
		Last Modified: Tue, 09 Jun 2020 05:06:08 GMT  
		Size: 244.6 KB (244636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c629efc5a0d859723a7100a060a51da7cbe12ff931fcd2edcb1be81b2d112240`  
		Last Modified: Tue, 09 Jun 2020 05:06:13 GMT  
		Size: 24.5 MB (24528005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5.20-slim`

```console
$ docker pull mono@sha256:eb687407e3866b90bbcbdf0989319656db2c4d419b1ac116a631a7da31b55c4b
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
$ docker pull mono@sha256:d9c9b346a27d528a42518d4ef2bab39267a82ae1df0c1e27ca9e444a03b55648
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78283780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8883015efde8b38b153a2d68418a8368d898879cbf16d21811f5229efaeae853`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 19:33:02 GMT
ENV MONO_VERSION=5.20.1.34
# Fri, 15 May 2020 19:33:14 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 19:33:43 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c687daeabb9e1562a2e501ad178edbc1896eeba1bffa74ce303519407544c563`  
		Last Modified: Fri, 15 May 2020 20:06:34 GMT  
		Size: 244.5 KB (244489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfe077f97d524ba2135e5765f841cc99024ef058b62c32cc792f665c0c673e1`  
		Last Modified: Fri, 15 May 2020 20:06:50 GMT  
		Size: 55.5 MB (55519404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:d1f2f6bfe520121a7e691cf8e461231bbb14f1e5c3eb5ee47a35ef036f8417ea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45594261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69e15644afe22231412b14df325238c1e07e59bd7605e734dc01523501da96bd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 00:55:49 GMT
ADD file:af949d376cc9a2ac87d0052d22fe17be59dfe65905f0645d1a903b359208d26d in / 
# Tue, 09 Jun 2020 00:55:51 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:37:38 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 09 Jun 2020 02:38:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 02:39:06 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c9b35828d9245f0a85299b96b2d9b0d70390689cf7df0fe7ef29ca6028c0ab56`  
		Last Modified: Tue, 09 Jun 2020 01:03:09 GMT  
		Size: 21.2 MB (21197337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822ecad80b0922cb6f84e448afb45744aebd13f1bbfa587c873ccf3d48339bf8`  
		Last Modified: Tue, 09 Jun 2020 02:50:04 GMT  
		Size: 244.6 KB (244612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29babd4ca7636c0b81bd94c0fb7bc0af65ce0f1bf052ef66eefdee3d473a1144`  
		Last Modified: Tue, 09 Jun 2020 02:50:12 GMT  
		Size: 24.2 MB (24152312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:31730ec67bfb195b239af6d38c20919b8393436676c52e52bfd9bad2b913213a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.0 MB (43002437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9aa26f1b857c100cd4b18663f267ac17dd83282d95d7b87ca6d279cf50b19b96`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:06:35 GMT
ADD file:4a0a863669948b35130fcf8cdb52999c49f7b3ee0620a1eef5f1a2e850a42f05 in / 
# Tue, 09 Jun 2020 01:06:37 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:52:41 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 09 Jun 2020 04:53:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:53:50 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c439312a9c212b64af3c38cb326bb5fbe14bcf4a622115d59d44985e949bee82`  
		Last Modified: Tue, 09 Jun 2020 01:13:51 GMT  
		Size: 19.3 MB (19304370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0af396ec38b9993232419e5d9219f0077d7145f9b61c7c8920d173d0a618840`  
		Last Modified: Tue, 09 Jun 2020 05:02:59 GMT  
		Size: 244.6 KB (244627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3794bbc29c2fc1f0baf05649349a607118798dc12e37fe275a2d929ebc984a`  
		Last Modified: Tue, 09 Jun 2020 05:03:07 GMT  
		Size: 23.5 MB (23453440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:48d8d81739bb780c0f6f54e39773ed7239fa34117e4baed155af459bdc7bb08e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48669512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4ef5ae213ee661f770b0931778cc05a349d7bac270e37715b391431cb89a305`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:49 GMT
ADD file:c85d28567b6123deb660b71c8b60d92378b5ba15ba5dcf495d9388817dc3aa44 in / 
# Tue, 09 Jun 2020 01:54:52 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 03:26:55 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 09 Jun 2020 03:27:13 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 03:27:54 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:622dc742b82743ebf5607b215a65869096390ee41b0a61b5532f859fb94590b1`  
		Last Modified: Tue, 09 Jun 2020 02:00:28 GMT  
		Size: 20.4 MB (20375150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47cfdc0a506e196319f490a8bb5e0036dd589b207aa03c9571763b3ee8dea29f`  
		Last Modified: Tue, 09 Jun 2020 03:37:36 GMT  
		Size: 244.4 KB (244372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6b08527e586e0f80506a226402a72b5cf43e106073bc06aa87862249894d0a`  
		Last Modified: Tue, 09 Jun 2020 03:37:45 GMT  
		Size: 28.0 MB (28049990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20-slim` - linux; 386

```console
$ docker pull mono@sha256:4222a99c9b296042587b96f689ebbf6634a8d8d2c635c4cd04d351e97712e0b9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.8 MB (81832175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4614f168389960f66e555809e63b35524bfd333eae47ec3048ab9ceb067a573`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:42:33 GMT
ADD file:8ef252685ffefc58654053bf145c830928a2cf423a6c757180649df772f1523d in / 
# Tue, 09 Jun 2020 01:42:34 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 07:01:47 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 09 Jun 2020 07:02:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 07:02:35 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4ffbd6ec7974e514763a8d7d9fcf5e86e9440e2280e6e9561ea373b4bc50588e`  
		Last Modified: Tue, 09 Jun 2020 01:48:28 GMT  
		Size: 23.1 MB (23147892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f35120db9bc30d6de494b0e58b8a74d62fe7a85cdc188357ea98ca2797e839`  
		Last Modified: Tue, 09 Jun 2020 07:11:10 GMT  
		Size: 244.5 KB (244478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d12cec6c246292b2edce2de333f893fefd5d9460042faa8e270bfde498b21612`  
		Last Modified: Tue, 09 Jun 2020 07:11:24 GMT  
		Size: 58.4 MB (58439805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5.20-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:176998bc9e1646c37ff64d0d4f385f36e1f8922f56319d19bb3c38f981738c0d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47563910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:406b118562a7fad8d6cb5ebd56d606c3007c1d31422152f7a9d5141a7803798b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:25:38 GMT
ADD file:41ec53d65aa183c2835f73989c9e4922f818e59774811eaa6e7395e5a36d5eab in / 
# Tue, 09 Jun 2020 01:25:42 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:43:07 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 09 Jun 2020 04:44:25 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:45:52 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a29e28607c9b96acae7ff89e56214e4339a87c59e40a6f030fa4cbcaab753f2c`  
		Last Modified: Tue, 09 Jun 2020 01:37:25 GMT  
		Size: 22.8 MB (22791269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d9971248b8a3142c8d28700658bc11b1313694441bf51b7febefd26adddbe1`  
		Last Modified: Tue, 09 Jun 2020 05:06:08 GMT  
		Size: 244.6 KB (244636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c629efc5a0d859723a7100a060a51da7cbe12ff931fcd2edcb1be81b2d112240`  
		Last Modified: Tue, 09 Jun 2020 05:06:13 GMT  
		Size: 24.5 MB (24528005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:5-slim`

```console
$ docker pull mono@sha256:eb687407e3866b90bbcbdf0989319656db2c4d419b1ac116a631a7da31b55c4b
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
$ docker pull mono@sha256:d9c9b346a27d528a42518d4ef2bab39267a82ae1df0c1e27ca9e444a03b55648
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78283780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8883015efde8b38b153a2d68418a8368d898879cbf16d21811f5229efaeae853`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 19:33:02 GMT
ENV MONO_VERSION=5.20.1.34
# Fri, 15 May 2020 19:33:14 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 19:33:43 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c687daeabb9e1562a2e501ad178edbc1896eeba1bffa74ce303519407544c563`  
		Last Modified: Fri, 15 May 2020 20:06:34 GMT  
		Size: 244.5 KB (244489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfe077f97d524ba2135e5765f841cc99024ef058b62c32cc792f665c0c673e1`  
		Last Modified: Fri, 15 May 2020 20:06:50 GMT  
		Size: 55.5 MB (55519404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:d1f2f6bfe520121a7e691cf8e461231bbb14f1e5c3eb5ee47a35ef036f8417ea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45594261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69e15644afe22231412b14df325238c1e07e59bd7605e734dc01523501da96bd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 00:55:49 GMT
ADD file:af949d376cc9a2ac87d0052d22fe17be59dfe65905f0645d1a903b359208d26d in / 
# Tue, 09 Jun 2020 00:55:51 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:37:38 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 09 Jun 2020 02:38:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 02:39:06 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c9b35828d9245f0a85299b96b2d9b0d70390689cf7df0fe7ef29ca6028c0ab56`  
		Last Modified: Tue, 09 Jun 2020 01:03:09 GMT  
		Size: 21.2 MB (21197337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822ecad80b0922cb6f84e448afb45744aebd13f1bbfa587c873ccf3d48339bf8`  
		Last Modified: Tue, 09 Jun 2020 02:50:04 GMT  
		Size: 244.6 KB (244612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29babd4ca7636c0b81bd94c0fb7bc0af65ce0f1bf052ef66eefdee3d473a1144`  
		Last Modified: Tue, 09 Jun 2020 02:50:12 GMT  
		Size: 24.2 MB (24152312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:31730ec67bfb195b239af6d38c20919b8393436676c52e52bfd9bad2b913213a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.0 MB (43002437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9aa26f1b857c100cd4b18663f267ac17dd83282d95d7b87ca6d279cf50b19b96`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:06:35 GMT
ADD file:4a0a863669948b35130fcf8cdb52999c49f7b3ee0620a1eef5f1a2e850a42f05 in / 
# Tue, 09 Jun 2020 01:06:37 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:52:41 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 09 Jun 2020 04:53:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:53:50 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c439312a9c212b64af3c38cb326bb5fbe14bcf4a622115d59d44985e949bee82`  
		Last Modified: Tue, 09 Jun 2020 01:13:51 GMT  
		Size: 19.3 MB (19304370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0af396ec38b9993232419e5d9219f0077d7145f9b61c7c8920d173d0a618840`  
		Last Modified: Tue, 09 Jun 2020 05:02:59 GMT  
		Size: 244.6 KB (244627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3794bbc29c2fc1f0baf05649349a607118798dc12e37fe275a2d929ebc984a`  
		Last Modified: Tue, 09 Jun 2020 05:03:07 GMT  
		Size: 23.5 MB (23453440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:48d8d81739bb780c0f6f54e39773ed7239fa34117e4baed155af459bdc7bb08e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48669512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4ef5ae213ee661f770b0931778cc05a349d7bac270e37715b391431cb89a305`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:49 GMT
ADD file:c85d28567b6123deb660b71c8b60d92378b5ba15ba5dcf495d9388817dc3aa44 in / 
# Tue, 09 Jun 2020 01:54:52 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 03:26:55 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 09 Jun 2020 03:27:13 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 03:27:54 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:622dc742b82743ebf5607b215a65869096390ee41b0a61b5532f859fb94590b1`  
		Last Modified: Tue, 09 Jun 2020 02:00:28 GMT  
		Size: 20.4 MB (20375150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47cfdc0a506e196319f490a8bb5e0036dd589b207aa03c9571763b3ee8dea29f`  
		Last Modified: Tue, 09 Jun 2020 03:37:36 GMT  
		Size: 244.4 KB (244372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6b08527e586e0f80506a226402a72b5cf43e106073bc06aa87862249894d0a`  
		Last Modified: Tue, 09 Jun 2020 03:37:45 GMT  
		Size: 28.0 MB (28049990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5-slim` - linux; 386

```console
$ docker pull mono@sha256:4222a99c9b296042587b96f689ebbf6634a8d8d2c635c4cd04d351e97712e0b9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.8 MB (81832175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4614f168389960f66e555809e63b35524bfd333eae47ec3048ab9ceb067a573`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:42:33 GMT
ADD file:8ef252685ffefc58654053bf145c830928a2cf423a6c757180649df772f1523d in / 
# Tue, 09 Jun 2020 01:42:34 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 07:01:47 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 09 Jun 2020 07:02:01 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 07:02:35 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4ffbd6ec7974e514763a8d7d9fcf5e86e9440e2280e6e9561ea373b4bc50588e`  
		Last Modified: Tue, 09 Jun 2020 01:48:28 GMT  
		Size: 23.1 MB (23147892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f35120db9bc30d6de494b0e58b8a74d62fe7a85cdc188357ea98ca2797e839`  
		Last Modified: Tue, 09 Jun 2020 07:11:10 GMT  
		Size: 244.5 KB (244478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d12cec6c246292b2edce2de333f893fefd5d9460042faa8e270bfde498b21612`  
		Last Modified: Tue, 09 Jun 2020 07:11:24 GMT  
		Size: 58.4 MB (58439805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:176998bc9e1646c37ff64d0d4f385f36e1f8922f56319d19bb3c38f981738c0d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47563910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:406b118562a7fad8d6cb5ebd56d606c3007c1d31422152f7a9d5141a7803798b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:25:38 GMT
ADD file:41ec53d65aa183c2835f73989c9e4922f818e59774811eaa6e7395e5a36d5eab in / 
# Tue, 09 Jun 2020 01:25:42 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:43:07 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 09 Jun 2020 04:44:25 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:45:52 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a29e28607c9b96acae7ff89e56214e4339a87c59e40a6f030fa4cbcaab753f2c`  
		Last Modified: Tue, 09 Jun 2020 01:37:25 GMT  
		Size: 22.8 MB (22791269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d9971248b8a3142c8d28700658bc11b1313694441bf51b7febefd26adddbe1`  
		Last Modified: Tue, 09 Jun 2020 05:06:08 GMT  
		Size: 244.6 KB (244636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c629efc5a0d859723a7100a060a51da7cbe12ff931fcd2edcb1be81b2d112240`  
		Last Modified: Tue, 09 Jun 2020 05:06:13 GMT  
		Size: 24.5 MB (24528005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6`

```console
$ docker pull mono@sha256:27d6a38bce172791c9b5961746b81b0cf95dc6d4b54500832427a5ee67fa9bfb
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
$ docker pull mono@sha256:21d11d8967f3ae2b3300a7dab5d5034fde699168cd2ef2da1322b7984c3b2b32
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.1 MB (235143779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b074d513c5cdfadffc24239c00962926b7b965e64cbc06b7c8ad4d110d77f4cd`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 19:31:02 GMT
ENV MONO_VERSION=6.8.0.96
# Fri, 15 May 2020 19:31:11 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 19:31:50 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 15 May 2020 19:44:52 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79aabb192e71d4e3020dd335c1061c5e9f915b73f367e8aeedf757b6adbc9c4`  
		Last Modified: Fri, 15 May 2020 20:05:47 GMT  
		Size: 244.5 KB (244497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96073affb70fefc051a7bb5f06242765faddc3114c900ccc1af9108910e6517`  
		Last Modified: Fri, 15 May 2020 20:06:04 GMT  
		Size: 64.6 MB (64584727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea44fa8b0fc1cfc5cfcf575269513b0ce648b1604436a20cc8c54fa2af29c32`  
		Last Modified: Fri, 15 May 2020 20:07:27 GMT  
		Size: 147.8 MB (147794668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; arm variant v5

```console
$ docker pull mono@sha256:d9c5ac0a34b9a4e40f2d5e63dcf776580e1f2be35ccfbe826b2da4e0441e15dc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.6 MB (176586764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad5f102651a6fa59023237fc450eb5316c9e92611685d7dcb277abdcefbd8390`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 00:55:49 GMT
ADD file:af949d376cc9a2ac87d0052d22fe17be59dfe65905f0645d1a903b359208d26d in / 
# Tue, 09 Jun 2020 00:55:51 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:34:30 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 02:35:00 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 02:35:52 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 02:42:32 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c9b35828d9245f0a85299b96b2d9b0d70390689cf7df0fe7ef29ca6028c0ab56`  
		Last Modified: Tue, 09 Jun 2020 01:03:09 GMT  
		Size: 21.2 MB (21197337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f2cf80f102f97dd711f97ed7ed659bbb653084b0446bec40197f89e4f2be8b`  
		Last Modified: Tue, 09 Jun 2020 02:49:21 GMT  
		Size: 244.6 KB (244566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4085e4a710b2483a23b0768a54b10e50906e0fcc4f4b76b767b7a24e17ffd4d2`  
		Last Modified: Tue, 09 Jun 2020 02:49:31 GMT  
		Size: 25.3 MB (25253616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff86f58b52cf2bb0b76c3e0c81032af953995ad8cabd583bda9636a431aebaa`  
		Last Modified: Tue, 09 Jun 2020 02:51:07 GMT  
		Size: 129.9 MB (129891245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; arm variant v7

```console
$ docker pull mono@sha256:f7ea0e55d8f6d089687e52455f05485d3f4611093df5cef5f0cb090f389beffd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.6 MB (172601822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2989d53c048f30bf6c564534beefa806c0e28eeb03d4a28905e9f05a715550c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:06:35 GMT
ADD file:4a0a863669948b35130fcf8cdb52999c49f7b3ee0620a1eef5f1a2e850a42f05 in / 
# Tue, 09 Jun 2020 01:06:37 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:50:02 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 04:50:28 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:51:11 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 04:56:20 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c439312a9c212b64af3c38cb326bb5fbe14bcf4a622115d59d44985e949bee82`  
		Last Modified: Tue, 09 Jun 2020 01:13:51 GMT  
		Size: 19.3 MB (19304370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0744b2f0bcb57875b07f1fa0fbcdfc6428593f823a41eb4698aab5b67ca5506f`  
		Last Modified: Tue, 09 Jun 2020 05:02:26 GMT  
		Size: 244.6 KB (244584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974d12d4793bb92f0ca8b3600115464d11bc0068af45f530f20adc882117d7bf`  
		Last Modified: Tue, 09 Jun 2020 05:02:36 GMT  
		Size: 24.5 MB (24498272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ec9f63e6708b28c4d538b45025dfbd0a318ab06d761ded9d48f44442c898a7`  
		Last Modified: Tue, 09 Jun 2020 05:04:00 GMT  
		Size: 128.6 MB (128554596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:68d1db7da63e2106ddea8d7850cf3badfaa16a94d8d23a12910f86785e4decc8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.6 MB (194642181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf6ff587bef5367449ceee09405f75d3b5a38e19c0d360ec43da1874b37497aa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:49 GMT
ADD file:c85d28567b6123deb660b71c8b60d92378b5ba15ba5dcf495d9388817dc3aa44 in / 
# Tue, 09 Jun 2020 01:54:52 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 03:24:02 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 03:24:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 03:25:06 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 03:30:31 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:622dc742b82743ebf5607b215a65869096390ee41b0a61b5532f859fb94590b1`  
		Last Modified: Tue, 09 Jun 2020 02:00:28 GMT  
		Size: 20.4 MB (20375150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334cf34398cfa7031d68bad42f6b2a8d870a4ad5c2b0454f3f6fdd0fb4433237`  
		Last Modified: Tue, 09 Jun 2020 03:37:02 GMT  
		Size: 244.4 KB (244374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa8cbd821b66a8c4a38ce3d6711cc1ee5489b04a017ab6a7fd368f08beec89e`  
		Last Modified: Tue, 09 Jun 2020 03:37:10 GMT  
		Size: 29.3 MB (29310269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f78bf65ea03cc9db2213ce7ff8e07d3a77604a43ef0a7d81b88b5c965515dfe`  
		Last Modified: Tue, 09 Jun 2020 03:38:38 GMT  
		Size: 144.7 MB (144712388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; 386

```console
$ docker pull mono@sha256:443376dd685b5fcd1e0b6b7a685c5b6a24a79fad8b9619e983293b70e84c8bb6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.4 MB (243401430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6948fdbf966360cb7a728eae30756da2daa5cc4b0362dd09e3a352f4ee44e5dc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:42:33 GMT
ADD file:8ef252685ffefc58654053bf145c830928a2cf423a6c757180649df772f1523d in / 
# Tue, 09 Jun 2020 01:42:34 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 06:59:35 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 06:59:46 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 07:00:24 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 07:05:03 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4ffbd6ec7974e514763a8d7d9fcf5e86e9440e2280e6e9561ea373b4bc50588e`  
		Last Modified: Tue, 09 Jun 2020 01:48:28 GMT  
		Size: 23.1 MB (23147892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b3a90700548ab3df378beb07af7fba67e7ea89ead888d8c78d529c40633c7ed`  
		Last Modified: Tue, 09 Jun 2020 07:10:23 GMT  
		Size: 244.5 KB (244462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbcec5e4a352eead9b06946ed8fb1855a57123b280b3941614dac805987d5b65`  
		Last Modified: Tue, 09 Jun 2020 07:10:41 GMT  
		Size: 68.5 MB (68517280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8167823b3a297ca26719112fd4ae0b1b90e5df5ef7edf3302022c64061697f`  
		Last Modified: Tue, 09 Jun 2020 07:12:09 GMT  
		Size: 151.5 MB (151491796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6` - linux; ppc64le

```console
$ docker pull mono@sha256:70c1fcea14ad2b7622978d2eb2d5626f8d5363e014b6f4974af4a4d5c15f7fac
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.9 MB (178895806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86adafe85745a7a969d3013f3ec3d1d66c603a377e21e1973c2c1eea147f78da`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:25:38 GMT
ADD file:41ec53d65aa183c2835f73989c9e4922f818e59774811eaa6e7395e5a36d5eab in / 
# Tue, 09 Jun 2020 01:25:42 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:37:42 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 04:39:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:40:39 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 04:51:22 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a29e28607c9b96acae7ff89e56214e4339a87c59e40a6f030fa4cbcaab753f2c`  
		Last Modified: Tue, 09 Jun 2020 01:37:25 GMT  
		Size: 22.8 MB (22791269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1fc192a4485fb46ca92b8e704feb4d02fab0a2a37cb4238017caf8d50239d5`  
		Last Modified: Tue, 09 Jun 2020 05:05:25 GMT  
		Size: 244.7 KB (244663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc43661bb843c17c3ae2b4bc4f6d7ffbc36d936efa982c85608c72360c89b849`  
		Last Modified: Tue, 09 Jun 2020 05:05:31 GMT  
		Size: 25.7 MB (25670188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:942f4a6a782ccadbdc03b5cda25e2632ae9bf2dbd213b5dfee3b75376ad65086`  
		Last Modified: Tue, 09 Jun 2020 05:06:55 GMT  
		Size: 130.2 MB (130189686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.6`

```console
$ docker pull mono@sha256:deb28228b114b3009c0a77a874b2429623b8e3a0a602dc634868ef7a7e5434cc
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
$ docker pull mono@sha256:a16eef5fc8e4f3c81e7f70a6662ffd30b32376db19fe3742b031d0d2f20e09b5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.0 MB (233045860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3d9995ebbe532a7fa650bab835486f977867a0f5a9fcd69a4adbd999f2bfb95`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 19:31:57 GMT
ENV MONO_VERSION=6.6.0.161
# Fri, 15 May 2020 19:32:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 19:32:54 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 15 May 2020 19:56:00 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba1f68e43fa7627c6e3b4600ce6d77ba6ffa44ee54e0d6ff37e287660ce6d98`  
		Last Modified: Fri, 15 May 2020 20:06:12 GMT  
		Size: 244.5 KB (244478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a19a53bf8d94f2994002e7ac9583e2930a4b87eb958cb057733523c9ab0426e`  
		Last Modified: Fri, 15 May 2020 20:06:29 GMT  
		Size: 63.0 MB (62972577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86749f70453599de8d16d5ba5dc08549d1598c22eabf307d9424ebe840a54b2c`  
		Last Modified: Fri, 15 May 2020 20:07:59 GMT  
		Size: 147.3 MB (147308918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6` - linux; arm variant v5

```console
$ docker pull mono@sha256:74a7c6c4a2ac4d800f2f19718a20bd950b385c5592915eed18e3bec787818284
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.4 MB (176402353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfb82cd2a6b9c1fce1a23a7273174935f22fb7f2a6795efe5d20b324b30d0bf6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 00:55:49 GMT
ADD file:af949d376cc9a2ac87d0052d22fe17be59dfe65905f0645d1a903b359208d26d in / 
# Tue, 09 Jun 2020 00:55:51 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:36:04 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 09 Jun 2020 02:36:30 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 02:37:25 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 02:45:38 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c9b35828d9245f0a85299b96b2d9b0d70390689cf7df0fe7ef29ca6028c0ab56`  
		Last Modified: Tue, 09 Jun 2020 01:03:09 GMT  
		Size: 21.2 MB (21197337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e5131ad86751562d7274ded73b46aef39545e363bd86513d9594fbc6309192`  
		Last Modified: Tue, 09 Jun 2020 02:49:42 GMT  
		Size: 244.6 KB (244587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f1083781c540ab53816710ad116bf747e31cebdd456afbcabbe9de3379a479`  
		Last Modified: Tue, 09 Jun 2020 02:49:56 GMT  
		Size: 25.3 MB (25311579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccdd9f15ce7cbe18d7e63ada902a17aa44d4021473688c3489345b77ebd486ce`  
		Last Modified: Tue, 09 Jun 2020 02:52:16 GMT  
		Size: 129.6 MB (129648850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6` - linux; arm variant v7

```console
$ docker pull mono@sha256:a261978360e6bd48cf86c99f184f10ee7d40ef4993da67157b219c9828ce3ddc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.4 MB (172407273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6985513d83d0e88b33d5997d25a6b91ada0453b756a9deb5688002842e32c8e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:06:35 GMT
ADD file:4a0a863669948b35130fcf8cdb52999c49f7b3ee0620a1eef5f1a2e850a42f05 in / 
# Tue, 09 Jun 2020 01:06:37 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:51:21 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 09 Jun 2020 04:51:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:52:25 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 04:59:01 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c439312a9c212b64af3c38cb326bb5fbe14bcf4a622115d59d44985e949bee82`  
		Last Modified: Tue, 09 Jun 2020 01:13:51 GMT  
		Size: 19.3 MB (19304370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac36da1b5bb82e6df780212e905bbc8029645394a747a28594275bc4062071c`  
		Last Modified: Tue, 09 Jun 2020 05:02:44 GMT  
		Size: 244.6 KB (244584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d329f47dbe526979620e12055cb42d1e2bf1e9f1a5f9ab13d7f1427edafe10f6`  
		Last Modified: Tue, 09 Jun 2020 05:02:52 GMT  
		Size: 24.5 MB (24544205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6e00459324f39454d7156a93bc4ee9182a3d4ec2c1b077ae022e8d88e98d50`  
		Last Modified: Tue, 09 Jun 2020 05:04:55 GMT  
		Size: 128.3 MB (128314114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:9ed842b0a7ac3cef21acce0287ae5ca88394337f09b62fa6db65b5363caff541
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.3 MB (194286054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01dcc3513017fae48738d43fcc06c221afbb7fdef66f67b4e66f956af21fba59`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:49 GMT
ADD file:c85d28567b6123deb660b71c8b60d92378b5ba15ba5dcf495d9388817dc3aa44 in / 
# Tue, 09 Jun 2020 01:54:52 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 03:25:21 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 09 Jun 2020 03:25:41 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 03:26:31 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 03:33:33 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:622dc742b82743ebf5607b215a65869096390ee41b0a61b5532f859fb94590b1`  
		Last Modified: Tue, 09 Jun 2020 02:00:28 GMT  
		Size: 20.4 MB (20375150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4290c2f990444deb0f93dd0ba68fc5d94357ce1cfdb252dec480eb8dc62df72`  
		Last Modified: Tue, 09 Jun 2020 03:37:19 GMT  
		Size: 244.4 KB (244381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7365212009d85dfb9bd0fefee678ef2259929ed35a819d5d1d63931c29d142`  
		Last Modified: Tue, 09 Jun 2020 03:37:29 GMT  
		Size: 29.3 MB (29326238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51ebbe9cd667dc8e9df498e44d5deeb4bac46ee95d4178ba191cd683a7b0224`  
		Last Modified: Tue, 09 Jun 2020 03:39:31 GMT  
		Size: 144.3 MB (144340285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6` - linux; 386

```console
$ docker pull mono@sha256:b9fda283e13398b40025d4368ac714e986347671b79ca74e5cca1d62d624730c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.2 MB (241191319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:219f26f416326e6efb9890d9950166c794593974d0ff38adc4c61421c81d6265`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:42:33 GMT
ADD file:8ef252685ffefc58654053bf145c830928a2cf423a6c757180649df772f1523d in / 
# Tue, 09 Jun 2020 01:42:34 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 07:00:31 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 09 Jun 2020 07:00:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 07:01:34 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 07:07:35 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4ffbd6ec7974e514763a8d7d9fcf5e86e9440e2280e6e9561ea373b4bc50588e`  
		Last Modified: Tue, 09 Jun 2020 01:48:28 GMT  
		Size: 23.1 MB (23147892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac86da952cf07d4efdc128f7ad526f39026bebd6fd96ce97f984d213ff33beb`  
		Last Modified: Tue, 09 Jun 2020 07:10:48 GMT  
		Size: 244.5 KB (244473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44aea1cbf2eb9bf3490c39e0036b585c6bd70cb027e4d67779122b5337b7eec8`  
		Last Modified: Tue, 09 Jun 2020 07:11:04 GMT  
		Size: 66.6 MB (66638665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53f7b67e9ddb24f8be1459afa90a46f0c2d0fab6eb67b6e0113781b8a896b8e`  
		Last Modified: Tue, 09 Jun 2020 07:12:55 GMT  
		Size: 151.2 MB (151160289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6` - linux; ppc64le

```console
$ docker pull mono@sha256:c0eb7651cb590936ee508d9f2c9118e01890e604f4ea77eb9f09f4a747b0267a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.7 MB (178692095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d66a6cad95995cff3f64cf89aab342aab7fc0ae29ec2b3cfc6b732b6c326a80`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:25:38 GMT
ADD file:41ec53d65aa183c2835f73989c9e4922f818e59774811eaa6e7395e5a36d5eab in / 
# Tue, 09 Jun 2020 01:25:42 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:40:54 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 09 Jun 2020 04:41:50 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:42:57 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 04:57:13 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a29e28607c9b96acae7ff89e56214e4339a87c59e40a6f030fa4cbcaab753f2c`  
		Last Modified: Tue, 09 Jun 2020 01:37:25 GMT  
		Size: 22.8 MB (22791269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f61e53535e34c8ba847db7a0b997284c1aa54e60b26ed23e5bfa4cab2fcd91`  
		Last Modified: Tue, 09 Jun 2020 05:05:48 GMT  
		Size: 244.6 KB (244568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:563625e3974512d700bb578934524f8dbbb23413ac33824ac5c60129e7c109d7`  
		Last Modified: Tue, 09 Jun 2020 05:05:55 GMT  
		Size: 25.7 MB (25715556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60af5c37498a2f246576decb845b382d75e96ceac5eea1f395585d7eebca979`  
		Last Modified: Tue, 09 Jun 2020 05:07:41 GMT  
		Size: 129.9 MB (129940702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.6.0`

```console
$ docker pull mono@sha256:deb28228b114b3009c0a77a874b2429623b8e3a0a602dc634868ef7a7e5434cc
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
$ docker pull mono@sha256:a16eef5fc8e4f3c81e7f70a6662ffd30b32376db19fe3742b031d0d2f20e09b5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.0 MB (233045860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3d9995ebbe532a7fa650bab835486f977867a0f5a9fcd69a4adbd999f2bfb95`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 19:31:57 GMT
ENV MONO_VERSION=6.6.0.161
# Fri, 15 May 2020 19:32:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 19:32:54 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 15 May 2020 19:56:00 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba1f68e43fa7627c6e3b4600ce6d77ba6ffa44ee54e0d6ff37e287660ce6d98`  
		Last Modified: Fri, 15 May 2020 20:06:12 GMT  
		Size: 244.5 KB (244478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a19a53bf8d94f2994002e7ac9583e2930a4b87eb958cb057733523c9ab0426e`  
		Last Modified: Fri, 15 May 2020 20:06:29 GMT  
		Size: 63.0 MB (62972577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86749f70453599de8d16d5ba5dc08549d1598c22eabf307d9424ebe840a54b2c`  
		Last Modified: Fri, 15 May 2020 20:07:59 GMT  
		Size: 147.3 MB (147308918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0` - linux; arm variant v5

```console
$ docker pull mono@sha256:74a7c6c4a2ac4d800f2f19718a20bd950b385c5592915eed18e3bec787818284
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.4 MB (176402353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfb82cd2a6b9c1fce1a23a7273174935f22fb7f2a6795efe5d20b324b30d0bf6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 00:55:49 GMT
ADD file:af949d376cc9a2ac87d0052d22fe17be59dfe65905f0645d1a903b359208d26d in / 
# Tue, 09 Jun 2020 00:55:51 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:36:04 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 09 Jun 2020 02:36:30 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 02:37:25 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 02:45:38 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c9b35828d9245f0a85299b96b2d9b0d70390689cf7df0fe7ef29ca6028c0ab56`  
		Last Modified: Tue, 09 Jun 2020 01:03:09 GMT  
		Size: 21.2 MB (21197337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e5131ad86751562d7274ded73b46aef39545e363bd86513d9594fbc6309192`  
		Last Modified: Tue, 09 Jun 2020 02:49:42 GMT  
		Size: 244.6 KB (244587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f1083781c540ab53816710ad116bf747e31cebdd456afbcabbe9de3379a479`  
		Last Modified: Tue, 09 Jun 2020 02:49:56 GMT  
		Size: 25.3 MB (25311579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccdd9f15ce7cbe18d7e63ada902a17aa44d4021473688c3489345b77ebd486ce`  
		Last Modified: Tue, 09 Jun 2020 02:52:16 GMT  
		Size: 129.6 MB (129648850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0` - linux; arm variant v7

```console
$ docker pull mono@sha256:a261978360e6bd48cf86c99f184f10ee7d40ef4993da67157b219c9828ce3ddc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.4 MB (172407273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6985513d83d0e88b33d5997d25a6b91ada0453b756a9deb5688002842e32c8e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:06:35 GMT
ADD file:4a0a863669948b35130fcf8cdb52999c49f7b3ee0620a1eef5f1a2e850a42f05 in / 
# Tue, 09 Jun 2020 01:06:37 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:51:21 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 09 Jun 2020 04:51:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:52:25 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 04:59:01 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c439312a9c212b64af3c38cb326bb5fbe14bcf4a622115d59d44985e949bee82`  
		Last Modified: Tue, 09 Jun 2020 01:13:51 GMT  
		Size: 19.3 MB (19304370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac36da1b5bb82e6df780212e905bbc8029645394a747a28594275bc4062071c`  
		Last Modified: Tue, 09 Jun 2020 05:02:44 GMT  
		Size: 244.6 KB (244584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d329f47dbe526979620e12055cb42d1e2bf1e9f1a5f9ab13d7f1427edafe10f6`  
		Last Modified: Tue, 09 Jun 2020 05:02:52 GMT  
		Size: 24.5 MB (24544205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6e00459324f39454d7156a93bc4ee9182a3d4ec2c1b077ae022e8d88e98d50`  
		Last Modified: Tue, 09 Jun 2020 05:04:55 GMT  
		Size: 128.3 MB (128314114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:9ed842b0a7ac3cef21acce0287ae5ca88394337f09b62fa6db65b5363caff541
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.3 MB (194286054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01dcc3513017fae48738d43fcc06c221afbb7fdef66f67b4e66f956af21fba59`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:49 GMT
ADD file:c85d28567b6123deb660b71c8b60d92378b5ba15ba5dcf495d9388817dc3aa44 in / 
# Tue, 09 Jun 2020 01:54:52 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 03:25:21 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 09 Jun 2020 03:25:41 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 03:26:31 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 03:33:33 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:622dc742b82743ebf5607b215a65869096390ee41b0a61b5532f859fb94590b1`  
		Last Modified: Tue, 09 Jun 2020 02:00:28 GMT  
		Size: 20.4 MB (20375150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4290c2f990444deb0f93dd0ba68fc5d94357ce1cfdb252dec480eb8dc62df72`  
		Last Modified: Tue, 09 Jun 2020 03:37:19 GMT  
		Size: 244.4 KB (244381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7365212009d85dfb9bd0fefee678ef2259929ed35a819d5d1d63931c29d142`  
		Last Modified: Tue, 09 Jun 2020 03:37:29 GMT  
		Size: 29.3 MB (29326238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51ebbe9cd667dc8e9df498e44d5deeb4bac46ee95d4178ba191cd683a7b0224`  
		Last Modified: Tue, 09 Jun 2020 03:39:31 GMT  
		Size: 144.3 MB (144340285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0` - linux; 386

```console
$ docker pull mono@sha256:b9fda283e13398b40025d4368ac714e986347671b79ca74e5cca1d62d624730c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.2 MB (241191319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:219f26f416326e6efb9890d9950166c794593974d0ff38adc4c61421c81d6265`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:42:33 GMT
ADD file:8ef252685ffefc58654053bf145c830928a2cf423a6c757180649df772f1523d in / 
# Tue, 09 Jun 2020 01:42:34 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 07:00:31 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 09 Jun 2020 07:00:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 07:01:34 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 07:07:35 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4ffbd6ec7974e514763a8d7d9fcf5e86e9440e2280e6e9561ea373b4bc50588e`  
		Last Modified: Tue, 09 Jun 2020 01:48:28 GMT  
		Size: 23.1 MB (23147892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac86da952cf07d4efdc128f7ad526f39026bebd6fd96ce97f984d213ff33beb`  
		Last Modified: Tue, 09 Jun 2020 07:10:48 GMT  
		Size: 244.5 KB (244473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44aea1cbf2eb9bf3490c39e0036b585c6bd70cb027e4d67779122b5337b7eec8`  
		Last Modified: Tue, 09 Jun 2020 07:11:04 GMT  
		Size: 66.6 MB (66638665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53f7b67e9ddb24f8be1459afa90a46f0c2d0fab6eb67b6e0113781b8a896b8e`  
		Last Modified: Tue, 09 Jun 2020 07:12:55 GMT  
		Size: 151.2 MB (151160289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0` - linux; ppc64le

```console
$ docker pull mono@sha256:c0eb7651cb590936ee508d9f2c9118e01890e604f4ea77eb9f09f4a747b0267a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.7 MB (178692095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d66a6cad95995cff3f64cf89aab342aab7fc0ae29ec2b3cfc6b732b6c326a80`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:25:38 GMT
ADD file:41ec53d65aa183c2835f73989c9e4922f818e59774811eaa6e7395e5a36d5eab in / 
# Tue, 09 Jun 2020 01:25:42 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:40:54 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 09 Jun 2020 04:41:50 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:42:57 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 04:57:13 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a29e28607c9b96acae7ff89e56214e4339a87c59e40a6f030fa4cbcaab753f2c`  
		Last Modified: Tue, 09 Jun 2020 01:37:25 GMT  
		Size: 22.8 MB (22791269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f61e53535e34c8ba847db7a0b997284c1aa54e60b26ed23e5bfa4cab2fcd91`  
		Last Modified: Tue, 09 Jun 2020 05:05:48 GMT  
		Size: 244.6 KB (244568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:563625e3974512d700bb578934524f8dbbb23413ac33824ac5c60129e7c109d7`  
		Last Modified: Tue, 09 Jun 2020 05:05:55 GMT  
		Size: 25.7 MB (25715556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60af5c37498a2f246576decb845b382d75e96ceac5eea1f395585d7eebca979`  
		Last Modified: Tue, 09 Jun 2020 05:07:41 GMT  
		Size: 129.9 MB (129940702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.6.0.161`

```console
$ docker pull mono@sha256:deb28228b114b3009c0a77a874b2429623b8e3a0a602dc634868ef7a7e5434cc
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
$ docker pull mono@sha256:a16eef5fc8e4f3c81e7f70a6662ffd30b32376db19fe3742b031d0d2f20e09b5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.0 MB (233045860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3d9995ebbe532a7fa650bab835486f977867a0f5a9fcd69a4adbd999f2bfb95`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 19:31:57 GMT
ENV MONO_VERSION=6.6.0.161
# Fri, 15 May 2020 19:32:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 19:32:54 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 15 May 2020 19:56:00 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba1f68e43fa7627c6e3b4600ce6d77ba6ffa44ee54e0d6ff37e287660ce6d98`  
		Last Modified: Fri, 15 May 2020 20:06:12 GMT  
		Size: 244.5 KB (244478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a19a53bf8d94f2994002e7ac9583e2930a4b87eb958cb057733523c9ab0426e`  
		Last Modified: Fri, 15 May 2020 20:06:29 GMT  
		Size: 63.0 MB (62972577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86749f70453599de8d16d5ba5dc08549d1598c22eabf307d9424ebe840a54b2c`  
		Last Modified: Fri, 15 May 2020 20:07:59 GMT  
		Size: 147.3 MB (147308918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0.161` - linux; arm variant v5

```console
$ docker pull mono@sha256:74a7c6c4a2ac4d800f2f19718a20bd950b385c5592915eed18e3bec787818284
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.4 MB (176402353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfb82cd2a6b9c1fce1a23a7273174935f22fb7f2a6795efe5d20b324b30d0bf6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 00:55:49 GMT
ADD file:af949d376cc9a2ac87d0052d22fe17be59dfe65905f0645d1a903b359208d26d in / 
# Tue, 09 Jun 2020 00:55:51 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:36:04 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 09 Jun 2020 02:36:30 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 02:37:25 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 02:45:38 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c9b35828d9245f0a85299b96b2d9b0d70390689cf7df0fe7ef29ca6028c0ab56`  
		Last Modified: Tue, 09 Jun 2020 01:03:09 GMT  
		Size: 21.2 MB (21197337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e5131ad86751562d7274ded73b46aef39545e363bd86513d9594fbc6309192`  
		Last Modified: Tue, 09 Jun 2020 02:49:42 GMT  
		Size: 244.6 KB (244587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f1083781c540ab53816710ad116bf747e31cebdd456afbcabbe9de3379a479`  
		Last Modified: Tue, 09 Jun 2020 02:49:56 GMT  
		Size: 25.3 MB (25311579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccdd9f15ce7cbe18d7e63ada902a17aa44d4021473688c3489345b77ebd486ce`  
		Last Modified: Tue, 09 Jun 2020 02:52:16 GMT  
		Size: 129.6 MB (129648850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0.161` - linux; arm variant v7

```console
$ docker pull mono@sha256:a261978360e6bd48cf86c99f184f10ee7d40ef4993da67157b219c9828ce3ddc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.4 MB (172407273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6985513d83d0e88b33d5997d25a6b91ada0453b756a9deb5688002842e32c8e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:06:35 GMT
ADD file:4a0a863669948b35130fcf8cdb52999c49f7b3ee0620a1eef5f1a2e850a42f05 in / 
# Tue, 09 Jun 2020 01:06:37 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:51:21 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 09 Jun 2020 04:51:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:52:25 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 04:59:01 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c439312a9c212b64af3c38cb326bb5fbe14bcf4a622115d59d44985e949bee82`  
		Last Modified: Tue, 09 Jun 2020 01:13:51 GMT  
		Size: 19.3 MB (19304370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac36da1b5bb82e6df780212e905bbc8029645394a747a28594275bc4062071c`  
		Last Modified: Tue, 09 Jun 2020 05:02:44 GMT  
		Size: 244.6 KB (244584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d329f47dbe526979620e12055cb42d1e2bf1e9f1a5f9ab13d7f1427edafe10f6`  
		Last Modified: Tue, 09 Jun 2020 05:02:52 GMT  
		Size: 24.5 MB (24544205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6e00459324f39454d7156a93bc4ee9182a3d4ec2c1b077ae022e8d88e98d50`  
		Last Modified: Tue, 09 Jun 2020 05:04:55 GMT  
		Size: 128.3 MB (128314114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0.161` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:9ed842b0a7ac3cef21acce0287ae5ca88394337f09b62fa6db65b5363caff541
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.3 MB (194286054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01dcc3513017fae48738d43fcc06c221afbb7fdef66f67b4e66f956af21fba59`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:49 GMT
ADD file:c85d28567b6123deb660b71c8b60d92378b5ba15ba5dcf495d9388817dc3aa44 in / 
# Tue, 09 Jun 2020 01:54:52 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 03:25:21 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 09 Jun 2020 03:25:41 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 03:26:31 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 03:33:33 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:622dc742b82743ebf5607b215a65869096390ee41b0a61b5532f859fb94590b1`  
		Last Modified: Tue, 09 Jun 2020 02:00:28 GMT  
		Size: 20.4 MB (20375150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4290c2f990444deb0f93dd0ba68fc5d94357ce1cfdb252dec480eb8dc62df72`  
		Last Modified: Tue, 09 Jun 2020 03:37:19 GMT  
		Size: 244.4 KB (244381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7365212009d85dfb9bd0fefee678ef2259929ed35a819d5d1d63931c29d142`  
		Last Modified: Tue, 09 Jun 2020 03:37:29 GMT  
		Size: 29.3 MB (29326238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51ebbe9cd667dc8e9df498e44d5deeb4bac46ee95d4178ba191cd683a7b0224`  
		Last Modified: Tue, 09 Jun 2020 03:39:31 GMT  
		Size: 144.3 MB (144340285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0.161` - linux; 386

```console
$ docker pull mono@sha256:b9fda283e13398b40025d4368ac714e986347671b79ca74e5cca1d62d624730c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.2 MB (241191319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:219f26f416326e6efb9890d9950166c794593974d0ff38adc4c61421c81d6265`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:42:33 GMT
ADD file:8ef252685ffefc58654053bf145c830928a2cf423a6c757180649df772f1523d in / 
# Tue, 09 Jun 2020 01:42:34 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 07:00:31 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 09 Jun 2020 07:00:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 07:01:34 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 07:07:35 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4ffbd6ec7974e514763a8d7d9fcf5e86e9440e2280e6e9561ea373b4bc50588e`  
		Last Modified: Tue, 09 Jun 2020 01:48:28 GMT  
		Size: 23.1 MB (23147892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac86da952cf07d4efdc128f7ad526f39026bebd6fd96ce97f984d213ff33beb`  
		Last Modified: Tue, 09 Jun 2020 07:10:48 GMT  
		Size: 244.5 KB (244473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44aea1cbf2eb9bf3490c39e0036b585c6bd70cb027e4d67779122b5337b7eec8`  
		Last Modified: Tue, 09 Jun 2020 07:11:04 GMT  
		Size: 66.6 MB (66638665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53f7b67e9ddb24f8be1459afa90a46f0c2d0fab6eb67b6e0113781b8a896b8e`  
		Last Modified: Tue, 09 Jun 2020 07:12:55 GMT  
		Size: 151.2 MB (151160289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0.161` - linux; ppc64le

```console
$ docker pull mono@sha256:c0eb7651cb590936ee508d9f2c9118e01890e604f4ea77eb9f09f4a747b0267a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.7 MB (178692095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d66a6cad95995cff3f64cf89aab342aab7fc0ae29ec2b3cfc6b732b6c326a80`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:25:38 GMT
ADD file:41ec53d65aa183c2835f73989c9e4922f818e59774811eaa6e7395e5a36d5eab in / 
# Tue, 09 Jun 2020 01:25:42 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:40:54 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 09 Jun 2020 04:41:50 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:42:57 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 04:57:13 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a29e28607c9b96acae7ff89e56214e4339a87c59e40a6f030fa4cbcaab753f2c`  
		Last Modified: Tue, 09 Jun 2020 01:37:25 GMT  
		Size: 22.8 MB (22791269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f61e53535e34c8ba847db7a0b997284c1aa54e60b26ed23e5bfa4cab2fcd91`  
		Last Modified: Tue, 09 Jun 2020 05:05:48 GMT  
		Size: 244.6 KB (244568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:563625e3974512d700bb578934524f8dbbb23413ac33824ac5c60129e7c109d7`  
		Last Modified: Tue, 09 Jun 2020 05:05:55 GMT  
		Size: 25.7 MB (25715556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60af5c37498a2f246576decb845b382d75e96ceac5eea1f395585d7eebca979`  
		Last Modified: Tue, 09 Jun 2020 05:07:41 GMT  
		Size: 129.9 MB (129940702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.6.0.161-slim`

```console
$ docker pull mono@sha256:6291c3331a0291c62d9fceed1ea77782bc93cc891b15d85803d158073a89d32e
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
$ docker pull mono@sha256:7fed3b02a746360dbc19a95d7f42127fac9846948b92b919dfb82998df0695e2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.7 MB (85736942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85f5c5bebebc33e92809686f686c32f88e30849892ee9f6e447f2b71bbde561a`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 19:31:57 GMT
ENV MONO_VERSION=6.6.0.161
# Fri, 15 May 2020 19:32:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 19:32:54 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba1f68e43fa7627c6e3b4600ce6d77ba6ffa44ee54e0d6ff37e287660ce6d98`  
		Last Modified: Fri, 15 May 2020 20:06:12 GMT  
		Size: 244.5 KB (244478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a19a53bf8d94f2994002e7ac9583e2930a4b87eb958cb057733523c9ab0426e`  
		Last Modified: Fri, 15 May 2020 20:06:29 GMT  
		Size: 63.0 MB (62972577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0.161-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:8fd2dbab88fcb41f165e9b05c077fbe51547cac2d55df4e591f9208b255fa9cc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.8 MB (46753503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b9c9404bec27f0fd07b858c0106491f22afc2b5f5c9f0b74bf5d24bc4cf3e95`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 00:55:49 GMT
ADD file:af949d376cc9a2ac87d0052d22fe17be59dfe65905f0645d1a903b359208d26d in / 
# Tue, 09 Jun 2020 00:55:51 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:36:04 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 09 Jun 2020 02:36:30 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 02:37:25 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c9b35828d9245f0a85299b96b2d9b0d70390689cf7df0fe7ef29ca6028c0ab56`  
		Last Modified: Tue, 09 Jun 2020 01:03:09 GMT  
		Size: 21.2 MB (21197337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e5131ad86751562d7274ded73b46aef39545e363bd86513d9594fbc6309192`  
		Last Modified: Tue, 09 Jun 2020 02:49:42 GMT  
		Size: 244.6 KB (244587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f1083781c540ab53816710ad116bf747e31cebdd456afbcabbe9de3379a479`  
		Last Modified: Tue, 09 Jun 2020 02:49:56 GMT  
		Size: 25.3 MB (25311579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0.161-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:67fa1ea6f7a6d3a71a0b25f26023dbd11a7e1d839959c5143b16c22347c5f8f3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44093159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4347c91a3f8e170ae42638614f019f918d2367490e085cea933786b2de75f3bf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:06:35 GMT
ADD file:4a0a863669948b35130fcf8cdb52999c49f7b3ee0620a1eef5f1a2e850a42f05 in / 
# Tue, 09 Jun 2020 01:06:37 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:51:21 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 09 Jun 2020 04:51:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:52:25 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c439312a9c212b64af3c38cb326bb5fbe14bcf4a622115d59d44985e949bee82`  
		Last Modified: Tue, 09 Jun 2020 01:13:51 GMT  
		Size: 19.3 MB (19304370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac36da1b5bb82e6df780212e905bbc8029645394a747a28594275bc4062071c`  
		Last Modified: Tue, 09 Jun 2020 05:02:44 GMT  
		Size: 244.6 KB (244584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d329f47dbe526979620e12055cb42d1e2bf1e9f1a5f9ab13d7f1427edafe10f6`  
		Last Modified: Tue, 09 Jun 2020 05:02:52 GMT  
		Size: 24.5 MB (24544205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0.161-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:0548c64057ccda46f006db6e0a843bc84ef1a1933a2d648f1375bae2a789afc9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 MB (49945769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f97dae24f93657a335b68d01bd3b74f8aff6ade8e76d786837880b0fbe8b64e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:49 GMT
ADD file:c85d28567b6123deb660b71c8b60d92378b5ba15ba5dcf495d9388817dc3aa44 in / 
# Tue, 09 Jun 2020 01:54:52 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 03:25:21 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 09 Jun 2020 03:25:41 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 03:26:31 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:622dc742b82743ebf5607b215a65869096390ee41b0a61b5532f859fb94590b1`  
		Last Modified: Tue, 09 Jun 2020 02:00:28 GMT  
		Size: 20.4 MB (20375150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4290c2f990444deb0f93dd0ba68fc5d94357ce1cfdb252dec480eb8dc62df72`  
		Last Modified: Tue, 09 Jun 2020 03:37:19 GMT  
		Size: 244.4 KB (244381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7365212009d85dfb9bd0fefee678ef2259929ed35a819d5d1d63931c29d142`  
		Last Modified: Tue, 09 Jun 2020 03:37:29 GMT  
		Size: 29.3 MB (29326238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0.161-slim` - linux; 386

```console
$ docker pull mono@sha256:932000e44cdd35e26b77f4c0c5677f1628fc274a874d3d582b6308b5582a1908
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.0 MB (90031030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07cc18c7941b425b71c3f02fae3f465e1e968dd84e133e4c9fb08c67b10fd434`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:42:33 GMT
ADD file:8ef252685ffefc58654053bf145c830928a2cf423a6c757180649df772f1523d in / 
# Tue, 09 Jun 2020 01:42:34 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 07:00:31 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 09 Jun 2020 07:00:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 07:01:34 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4ffbd6ec7974e514763a8d7d9fcf5e86e9440e2280e6e9561ea373b4bc50588e`  
		Last Modified: Tue, 09 Jun 2020 01:48:28 GMT  
		Size: 23.1 MB (23147892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac86da952cf07d4efdc128f7ad526f39026bebd6fd96ce97f984d213ff33beb`  
		Last Modified: Tue, 09 Jun 2020 07:10:48 GMT  
		Size: 244.5 KB (244473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44aea1cbf2eb9bf3490c39e0036b585c6bd70cb027e4d67779122b5337b7eec8`  
		Last Modified: Tue, 09 Jun 2020 07:11:04 GMT  
		Size: 66.6 MB (66638665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0.161-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:57d9303ed37696b8b21c488b4aca34261b07a9c5a1acf2568a56cf10ef898de5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48751393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4aa115ab28661971a7391f318eae5c36b475f431e9cd1085efb4a3f7f4338a8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:25:38 GMT
ADD file:41ec53d65aa183c2835f73989c9e4922f818e59774811eaa6e7395e5a36d5eab in / 
# Tue, 09 Jun 2020 01:25:42 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:40:54 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 09 Jun 2020 04:41:50 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:42:57 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a29e28607c9b96acae7ff89e56214e4339a87c59e40a6f030fa4cbcaab753f2c`  
		Last Modified: Tue, 09 Jun 2020 01:37:25 GMT  
		Size: 22.8 MB (22791269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f61e53535e34c8ba847db7a0b997284c1aa54e60b26ed23e5bfa4cab2fcd91`  
		Last Modified: Tue, 09 Jun 2020 05:05:48 GMT  
		Size: 244.6 KB (244568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:563625e3974512d700bb578934524f8dbbb23413ac33824ac5c60129e7c109d7`  
		Last Modified: Tue, 09 Jun 2020 05:05:55 GMT  
		Size: 25.7 MB (25715556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.6.0-slim`

```console
$ docker pull mono@sha256:6291c3331a0291c62d9fceed1ea77782bc93cc891b15d85803d158073a89d32e
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
$ docker pull mono@sha256:7fed3b02a746360dbc19a95d7f42127fac9846948b92b919dfb82998df0695e2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.7 MB (85736942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85f5c5bebebc33e92809686f686c32f88e30849892ee9f6e447f2b71bbde561a`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 19:31:57 GMT
ENV MONO_VERSION=6.6.0.161
# Fri, 15 May 2020 19:32:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 19:32:54 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba1f68e43fa7627c6e3b4600ce6d77ba6ffa44ee54e0d6ff37e287660ce6d98`  
		Last Modified: Fri, 15 May 2020 20:06:12 GMT  
		Size: 244.5 KB (244478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a19a53bf8d94f2994002e7ac9583e2930a4b87eb958cb057733523c9ab0426e`  
		Last Modified: Fri, 15 May 2020 20:06:29 GMT  
		Size: 63.0 MB (62972577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:8fd2dbab88fcb41f165e9b05c077fbe51547cac2d55df4e591f9208b255fa9cc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.8 MB (46753503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b9c9404bec27f0fd07b858c0106491f22afc2b5f5c9f0b74bf5d24bc4cf3e95`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 00:55:49 GMT
ADD file:af949d376cc9a2ac87d0052d22fe17be59dfe65905f0645d1a903b359208d26d in / 
# Tue, 09 Jun 2020 00:55:51 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:36:04 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 09 Jun 2020 02:36:30 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 02:37:25 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c9b35828d9245f0a85299b96b2d9b0d70390689cf7df0fe7ef29ca6028c0ab56`  
		Last Modified: Tue, 09 Jun 2020 01:03:09 GMT  
		Size: 21.2 MB (21197337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e5131ad86751562d7274ded73b46aef39545e363bd86513d9594fbc6309192`  
		Last Modified: Tue, 09 Jun 2020 02:49:42 GMT  
		Size: 244.6 KB (244587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f1083781c540ab53816710ad116bf747e31cebdd456afbcabbe9de3379a479`  
		Last Modified: Tue, 09 Jun 2020 02:49:56 GMT  
		Size: 25.3 MB (25311579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:67fa1ea6f7a6d3a71a0b25f26023dbd11a7e1d839959c5143b16c22347c5f8f3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44093159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4347c91a3f8e170ae42638614f019f918d2367490e085cea933786b2de75f3bf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:06:35 GMT
ADD file:4a0a863669948b35130fcf8cdb52999c49f7b3ee0620a1eef5f1a2e850a42f05 in / 
# Tue, 09 Jun 2020 01:06:37 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:51:21 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 09 Jun 2020 04:51:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:52:25 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c439312a9c212b64af3c38cb326bb5fbe14bcf4a622115d59d44985e949bee82`  
		Last Modified: Tue, 09 Jun 2020 01:13:51 GMT  
		Size: 19.3 MB (19304370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac36da1b5bb82e6df780212e905bbc8029645394a747a28594275bc4062071c`  
		Last Modified: Tue, 09 Jun 2020 05:02:44 GMT  
		Size: 244.6 KB (244584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d329f47dbe526979620e12055cb42d1e2bf1e9f1a5f9ab13d7f1427edafe10f6`  
		Last Modified: Tue, 09 Jun 2020 05:02:52 GMT  
		Size: 24.5 MB (24544205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:0548c64057ccda46f006db6e0a843bc84ef1a1933a2d648f1375bae2a789afc9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 MB (49945769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f97dae24f93657a335b68d01bd3b74f8aff6ade8e76d786837880b0fbe8b64e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:49 GMT
ADD file:c85d28567b6123deb660b71c8b60d92378b5ba15ba5dcf495d9388817dc3aa44 in / 
# Tue, 09 Jun 2020 01:54:52 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 03:25:21 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 09 Jun 2020 03:25:41 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 03:26:31 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:622dc742b82743ebf5607b215a65869096390ee41b0a61b5532f859fb94590b1`  
		Last Modified: Tue, 09 Jun 2020 02:00:28 GMT  
		Size: 20.4 MB (20375150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4290c2f990444deb0f93dd0ba68fc5d94357ce1cfdb252dec480eb8dc62df72`  
		Last Modified: Tue, 09 Jun 2020 03:37:19 GMT  
		Size: 244.4 KB (244381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7365212009d85dfb9bd0fefee678ef2259929ed35a819d5d1d63931c29d142`  
		Last Modified: Tue, 09 Jun 2020 03:37:29 GMT  
		Size: 29.3 MB (29326238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0-slim` - linux; 386

```console
$ docker pull mono@sha256:932000e44cdd35e26b77f4c0c5677f1628fc274a874d3d582b6308b5582a1908
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.0 MB (90031030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07cc18c7941b425b71c3f02fae3f465e1e968dd84e133e4c9fb08c67b10fd434`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:42:33 GMT
ADD file:8ef252685ffefc58654053bf145c830928a2cf423a6c757180649df772f1523d in / 
# Tue, 09 Jun 2020 01:42:34 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 07:00:31 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 09 Jun 2020 07:00:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 07:01:34 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4ffbd6ec7974e514763a8d7d9fcf5e86e9440e2280e6e9561ea373b4bc50588e`  
		Last Modified: Tue, 09 Jun 2020 01:48:28 GMT  
		Size: 23.1 MB (23147892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac86da952cf07d4efdc128f7ad526f39026bebd6fd96ce97f984d213ff33beb`  
		Last Modified: Tue, 09 Jun 2020 07:10:48 GMT  
		Size: 244.5 KB (244473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44aea1cbf2eb9bf3490c39e0036b585c6bd70cb027e4d67779122b5337b7eec8`  
		Last Modified: Tue, 09 Jun 2020 07:11:04 GMT  
		Size: 66.6 MB (66638665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6.0-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:57d9303ed37696b8b21c488b4aca34261b07a9c5a1acf2568a56cf10ef898de5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48751393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4aa115ab28661971a7391f318eae5c36b475f431e9cd1085efb4a3f7f4338a8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:25:38 GMT
ADD file:41ec53d65aa183c2835f73989c9e4922f818e59774811eaa6e7395e5a36d5eab in / 
# Tue, 09 Jun 2020 01:25:42 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:40:54 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 09 Jun 2020 04:41:50 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:42:57 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a29e28607c9b96acae7ff89e56214e4339a87c59e40a6f030fa4cbcaab753f2c`  
		Last Modified: Tue, 09 Jun 2020 01:37:25 GMT  
		Size: 22.8 MB (22791269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f61e53535e34c8ba847db7a0b997284c1aa54e60b26ed23e5bfa4cab2fcd91`  
		Last Modified: Tue, 09 Jun 2020 05:05:48 GMT  
		Size: 244.6 KB (244568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:563625e3974512d700bb578934524f8dbbb23413ac33824ac5c60129e7c109d7`  
		Last Modified: Tue, 09 Jun 2020 05:05:55 GMT  
		Size: 25.7 MB (25715556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.6-slim`

```console
$ docker pull mono@sha256:6291c3331a0291c62d9fceed1ea77782bc93cc891b15d85803d158073a89d32e
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
$ docker pull mono@sha256:7fed3b02a746360dbc19a95d7f42127fac9846948b92b919dfb82998df0695e2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.7 MB (85736942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85f5c5bebebc33e92809686f686c32f88e30849892ee9f6e447f2b71bbde561a`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 19:31:57 GMT
ENV MONO_VERSION=6.6.0.161
# Fri, 15 May 2020 19:32:09 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 19:32:54 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba1f68e43fa7627c6e3b4600ce6d77ba6ffa44ee54e0d6ff37e287660ce6d98`  
		Last Modified: Fri, 15 May 2020 20:06:12 GMT  
		Size: 244.5 KB (244478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a19a53bf8d94f2994002e7ac9583e2930a4b87eb958cb057733523c9ab0426e`  
		Last Modified: Fri, 15 May 2020 20:06:29 GMT  
		Size: 63.0 MB (62972577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:8fd2dbab88fcb41f165e9b05c077fbe51547cac2d55df4e591f9208b255fa9cc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.8 MB (46753503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b9c9404bec27f0fd07b858c0106491f22afc2b5f5c9f0b74bf5d24bc4cf3e95`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 00:55:49 GMT
ADD file:af949d376cc9a2ac87d0052d22fe17be59dfe65905f0645d1a903b359208d26d in / 
# Tue, 09 Jun 2020 00:55:51 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:36:04 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 09 Jun 2020 02:36:30 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 02:37:25 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c9b35828d9245f0a85299b96b2d9b0d70390689cf7df0fe7ef29ca6028c0ab56`  
		Last Modified: Tue, 09 Jun 2020 01:03:09 GMT  
		Size: 21.2 MB (21197337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e5131ad86751562d7274ded73b46aef39545e363bd86513d9594fbc6309192`  
		Last Modified: Tue, 09 Jun 2020 02:49:42 GMT  
		Size: 244.6 KB (244587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f1083781c540ab53816710ad116bf747e31cebdd456afbcabbe9de3379a479`  
		Last Modified: Tue, 09 Jun 2020 02:49:56 GMT  
		Size: 25.3 MB (25311579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:67fa1ea6f7a6d3a71a0b25f26023dbd11a7e1d839959c5143b16c22347c5f8f3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44093159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4347c91a3f8e170ae42638614f019f918d2367490e085cea933786b2de75f3bf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:06:35 GMT
ADD file:4a0a863669948b35130fcf8cdb52999c49f7b3ee0620a1eef5f1a2e850a42f05 in / 
# Tue, 09 Jun 2020 01:06:37 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:51:21 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 09 Jun 2020 04:51:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:52:25 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c439312a9c212b64af3c38cb326bb5fbe14bcf4a622115d59d44985e949bee82`  
		Last Modified: Tue, 09 Jun 2020 01:13:51 GMT  
		Size: 19.3 MB (19304370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac36da1b5bb82e6df780212e905bbc8029645394a747a28594275bc4062071c`  
		Last Modified: Tue, 09 Jun 2020 05:02:44 GMT  
		Size: 244.6 KB (244584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d329f47dbe526979620e12055cb42d1e2bf1e9f1a5f9ab13d7f1427edafe10f6`  
		Last Modified: Tue, 09 Jun 2020 05:02:52 GMT  
		Size: 24.5 MB (24544205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:0548c64057ccda46f006db6e0a843bc84ef1a1933a2d648f1375bae2a789afc9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 MB (49945769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f97dae24f93657a335b68d01bd3b74f8aff6ade8e76d786837880b0fbe8b64e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:49 GMT
ADD file:c85d28567b6123deb660b71c8b60d92378b5ba15ba5dcf495d9388817dc3aa44 in / 
# Tue, 09 Jun 2020 01:54:52 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 03:25:21 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 09 Jun 2020 03:25:41 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 03:26:31 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:622dc742b82743ebf5607b215a65869096390ee41b0a61b5532f859fb94590b1`  
		Last Modified: Tue, 09 Jun 2020 02:00:28 GMT  
		Size: 20.4 MB (20375150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4290c2f990444deb0f93dd0ba68fc5d94357ce1cfdb252dec480eb8dc62df72`  
		Last Modified: Tue, 09 Jun 2020 03:37:19 GMT  
		Size: 244.4 KB (244381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7365212009d85dfb9bd0fefee678ef2259929ed35a819d5d1d63931c29d142`  
		Last Modified: Tue, 09 Jun 2020 03:37:29 GMT  
		Size: 29.3 MB (29326238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6-slim` - linux; 386

```console
$ docker pull mono@sha256:932000e44cdd35e26b77f4c0c5677f1628fc274a874d3d582b6308b5582a1908
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.0 MB (90031030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07cc18c7941b425b71c3f02fae3f465e1e968dd84e133e4c9fb08c67b10fd434`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:42:33 GMT
ADD file:8ef252685ffefc58654053bf145c830928a2cf423a6c757180649df772f1523d in / 
# Tue, 09 Jun 2020 01:42:34 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 07:00:31 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 09 Jun 2020 07:00:43 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 07:01:34 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4ffbd6ec7974e514763a8d7d9fcf5e86e9440e2280e6e9561ea373b4bc50588e`  
		Last Modified: Tue, 09 Jun 2020 01:48:28 GMT  
		Size: 23.1 MB (23147892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac86da952cf07d4efdc128f7ad526f39026bebd6fd96ce97f984d213ff33beb`  
		Last Modified: Tue, 09 Jun 2020 07:10:48 GMT  
		Size: 244.5 KB (244473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44aea1cbf2eb9bf3490c39e0036b585c6bd70cb027e4d67779122b5337b7eec8`  
		Last Modified: Tue, 09 Jun 2020 07:11:04 GMT  
		Size: 66.6 MB (66638665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.6-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:57d9303ed37696b8b21c488b4aca34261b07a9c5a1acf2568a56cf10ef898de5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48751393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4aa115ab28661971a7391f318eae5c36b475f431e9cd1085efb4a3f7f4338a8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:25:38 GMT
ADD file:41ec53d65aa183c2835f73989c9e4922f818e59774811eaa6e7395e5a36d5eab in / 
# Tue, 09 Jun 2020 01:25:42 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:40:54 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 09 Jun 2020 04:41:50 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:42:57 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a29e28607c9b96acae7ff89e56214e4339a87c59e40a6f030fa4cbcaab753f2c`  
		Last Modified: Tue, 09 Jun 2020 01:37:25 GMT  
		Size: 22.8 MB (22791269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f61e53535e34c8ba847db7a0b997284c1aa54e60b26ed23e5bfa4cab2fcd91`  
		Last Modified: Tue, 09 Jun 2020 05:05:48 GMT  
		Size: 244.6 KB (244568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:563625e3974512d700bb578934524f8dbbb23413ac33824ac5c60129e7c109d7`  
		Last Modified: Tue, 09 Jun 2020 05:05:55 GMT  
		Size: 25.7 MB (25715556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.8`

```console
$ docker pull mono@sha256:27d6a38bce172791c9b5961746b81b0cf95dc6d4b54500832427a5ee67fa9bfb
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
$ docker pull mono@sha256:21d11d8967f3ae2b3300a7dab5d5034fde699168cd2ef2da1322b7984c3b2b32
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.1 MB (235143779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b074d513c5cdfadffc24239c00962926b7b965e64cbc06b7c8ad4d110d77f4cd`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 19:31:02 GMT
ENV MONO_VERSION=6.8.0.96
# Fri, 15 May 2020 19:31:11 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 19:31:50 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 15 May 2020 19:44:52 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79aabb192e71d4e3020dd335c1061c5e9f915b73f367e8aeedf757b6adbc9c4`  
		Last Modified: Fri, 15 May 2020 20:05:47 GMT  
		Size: 244.5 KB (244497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96073affb70fefc051a7bb5f06242765faddc3114c900ccc1af9108910e6517`  
		Last Modified: Fri, 15 May 2020 20:06:04 GMT  
		Size: 64.6 MB (64584727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea44fa8b0fc1cfc5cfcf575269513b0ce648b1604436a20cc8c54fa2af29c32`  
		Last Modified: Fri, 15 May 2020 20:07:27 GMT  
		Size: 147.8 MB (147794668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8` - linux; arm variant v5

```console
$ docker pull mono@sha256:d9c5ac0a34b9a4e40f2d5e63dcf776580e1f2be35ccfbe826b2da4e0441e15dc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.6 MB (176586764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad5f102651a6fa59023237fc450eb5316c9e92611685d7dcb277abdcefbd8390`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 00:55:49 GMT
ADD file:af949d376cc9a2ac87d0052d22fe17be59dfe65905f0645d1a903b359208d26d in / 
# Tue, 09 Jun 2020 00:55:51 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:34:30 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 02:35:00 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 02:35:52 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 02:42:32 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c9b35828d9245f0a85299b96b2d9b0d70390689cf7df0fe7ef29ca6028c0ab56`  
		Last Modified: Tue, 09 Jun 2020 01:03:09 GMT  
		Size: 21.2 MB (21197337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f2cf80f102f97dd711f97ed7ed659bbb653084b0446bec40197f89e4f2be8b`  
		Last Modified: Tue, 09 Jun 2020 02:49:21 GMT  
		Size: 244.6 KB (244566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4085e4a710b2483a23b0768a54b10e50906e0fcc4f4b76b767b7a24e17ffd4d2`  
		Last Modified: Tue, 09 Jun 2020 02:49:31 GMT  
		Size: 25.3 MB (25253616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff86f58b52cf2bb0b76c3e0c81032af953995ad8cabd583bda9636a431aebaa`  
		Last Modified: Tue, 09 Jun 2020 02:51:07 GMT  
		Size: 129.9 MB (129891245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8` - linux; arm variant v7

```console
$ docker pull mono@sha256:f7ea0e55d8f6d089687e52455f05485d3f4611093df5cef5f0cb090f389beffd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.6 MB (172601822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2989d53c048f30bf6c564534beefa806c0e28eeb03d4a28905e9f05a715550c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:06:35 GMT
ADD file:4a0a863669948b35130fcf8cdb52999c49f7b3ee0620a1eef5f1a2e850a42f05 in / 
# Tue, 09 Jun 2020 01:06:37 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:50:02 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 04:50:28 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:51:11 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 04:56:20 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c439312a9c212b64af3c38cb326bb5fbe14bcf4a622115d59d44985e949bee82`  
		Last Modified: Tue, 09 Jun 2020 01:13:51 GMT  
		Size: 19.3 MB (19304370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0744b2f0bcb57875b07f1fa0fbcdfc6428593f823a41eb4698aab5b67ca5506f`  
		Last Modified: Tue, 09 Jun 2020 05:02:26 GMT  
		Size: 244.6 KB (244584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974d12d4793bb92f0ca8b3600115464d11bc0068af45f530f20adc882117d7bf`  
		Last Modified: Tue, 09 Jun 2020 05:02:36 GMT  
		Size: 24.5 MB (24498272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ec9f63e6708b28c4d538b45025dfbd0a318ab06d761ded9d48f44442c898a7`  
		Last Modified: Tue, 09 Jun 2020 05:04:00 GMT  
		Size: 128.6 MB (128554596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:68d1db7da63e2106ddea8d7850cf3badfaa16a94d8d23a12910f86785e4decc8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.6 MB (194642181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf6ff587bef5367449ceee09405f75d3b5a38e19c0d360ec43da1874b37497aa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:49 GMT
ADD file:c85d28567b6123deb660b71c8b60d92378b5ba15ba5dcf495d9388817dc3aa44 in / 
# Tue, 09 Jun 2020 01:54:52 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 03:24:02 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 03:24:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 03:25:06 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 03:30:31 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:622dc742b82743ebf5607b215a65869096390ee41b0a61b5532f859fb94590b1`  
		Last Modified: Tue, 09 Jun 2020 02:00:28 GMT  
		Size: 20.4 MB (20375150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334cf34398cfa7031d68bad42f6b2a8d870a4ad5c2b0454f3f6fdd0fb4433237`  
		Last Modified: Tue, 09 Jun 2020 03:37:02 GMT  
		Size: 244.4 KB (244374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa8cbd821b66a8c4a38ce3d6711cc1ee5489b04a017ab6a7fd368f08beec89e`  
		Last Modified: Tue, 09 Jun 2020 03:37:10 GMT  
		Size: 29.3 MB (29310269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f78bf65ea03cc9db2213ce7ff8e07d3a77604a43ef0a7d81b88b5c965515dfe`  
		Last Modified: Tue, 09 Jun 2020 03:38:38 GMT  
		Size: 144.7 MB (144712388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8` - linux; 386

```console
$ docker pull mono@sha256:443376dd685b5fcd1e0b6b7a685c5b6a24a79fad8b9619e983293b70e84c8bb6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.4 MB (243401430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6948fdbf966360cb7a728eae30756da2daa5cc4b0362dd09e3a352f4ee44e5dc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:42:33 GMT
ADD file:8ef252685ffefc58654053bf145c830928a2cf423a6c757180649df772f1523d in / 
# Tue, 09 Jun 2020 01:42:34 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 06:59:35 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 06:59:46 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 07:00:24 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 07:05:03 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4ffbd6ec7974e514763a8d7d9fcf5e86e9440e2280e6e9561ea373b4bc50588e`  
		Last Modified: Tue, 09 Jun 2020 01:48:28 GMT  
		Size: 23.1 MB (23147892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b3a90700548ab3df378beb07af7fba67e7ea89ead888d8c78d529c40633c7ed`  
		Last Modified: Tue, 09 Jun 2020 07:10:23 GMT  
		Size: 244.5 KB (244462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbcec5e4a352eead9b06946ed8fb1855a57123b280b3941614dac805987d5b65`  
		Last Modified: Tue, 09 Jun 2020 07:10:41 GMT  
		Size: 68.5 MB (68517280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8167823b3a297ca26719112fd4ae0b1b90e5df5ef7edf3302022c64061697f`  
		Last Modified: Tue, 09 Jun 2020 07:12:09 GMT  
		Size: 151.5 MB (151491796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8` - linux; ppc64le

```console
$ docker pull mono@sha256:70c1fcea14ad2b7622978d2eb2d5626f8d5363e014b6f4974af4a4d5c15f7fac
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.9 MB (178895806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86adafe85745a7a969d3013f3ec3d1d66c603a377e21e1973c2c1eea147f78da`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:25:38 GMT
ADD file:41ec53d65aa183c2835f73989c9e4922f818e59774811eaa6e7395e5a36d5eab in / 
# Tue, 09 Jun 2020 01:25:42 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:37:42 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 04:39:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:40:39 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 04:51:22 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a29e28607c9b96acae7ff89e56214e4339a87c59e40a6f030fa4cbcaab753f2c`  
		Last Modified: Tue, 09 Jun 2020 01:37:25 GMT  
		Size: 22.8 MB (22791269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1fc192a4485fb46ca92b8e704feb4d02fab0a2a37cb4238017caf8d50239d5`  
		Last Modified: Tue, 09 Jun 2020 05:05:25 GMT  
		Size: 244.7 KB (244663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc43661bb843c17c3ae2b4bc4f6d7ffbc36d936efa982c85608c72360c89b849`  
		Last Modified: Tue, 09 Jun 2020 05:05:31 GMT  
		Size: 25.7 MB (25670188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:942f4a6a782ccadbdc03b5cda25e2632ae9bf2dbd213b5dfee3b75376ad65086`  
		Last Modified: Tue, 09 Jun 2020 05:06:55 GMT  
		Size: 130.2 MB (130189686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.8.0`

```console
$ docker pull mono@sha256:27d6a38bce172791c9b5961746b81b0cf95dc6d4b54500832427a5ee67fa9bfb
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
$ docker pull mono@sha256:21d11d8967f3ae2b3300a7dab5d5034fde699168cd2ef2da1322b7984c3b2b32
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.1 MB (235143779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b074d513c5cdfadffc24239c00962926b7b965e64cbc06b7c8ad4d110d77f4cd`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 19:31:02 GMT
ENV MONO_VERSION=6.8.0.96
# Fri, 15 May 2020 19:31:11 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 19:31:50 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 15 May 2020 19:44:52 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79aabb192e71d4e3020dd335c1061c5e9f915b73f367e8aeedf757b6adbc9c4`  
		Last Modified: Fri, 15 May 2020 20:05:47 GMT  
		Size: 244.5 KB (244497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96073affb70fefc051a7bb5f06242765faddc3114c900ccc1af9108910e6517`  
		Last Modified: Fri, 15 May 2020 20:06:04 GMT  
		Size: 64.6 MB (64584727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea44fa8b0fc1cfc5cfcf575269513b0ce648b1604436a20cc8c54fa2af29c32`  
		Last Modified: Fri, 15 May 2020 20:07:27 GMT  
		Size: 147.8 MB (147794668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0` - linux; arm variant v5

```console
$ docker pull mono@sha256:d9c5ac0a34b9a4e40f2d5e63dcf776580e1f2be35ccfbe826b2da4e0441e15dc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.6 MB (176586764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad5f102651a6fa59023237fc450eb5316c9e92611685d7dcb277abdcefbd8390`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 00:55:49 GMT
ADD file:af949d376cc9a2ac87d0052d22fe17be59dfe65905f0645d1a903b359208d26d in / 
# Tue, 09 Jun 2020 00:55:51 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:34:30 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 02:35:00 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 02:35:52 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 02:42:32 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c9b35828d9245f0a85299b96b2d9b0d70390689cf7df0fe7ef29ca6028c0ab56`  
		Last Modified: Tue, 09 Jun 2020 01:03:09 GMT  
		Size: 21.2 MB (21197337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f2cf80f102f97dd711f97ed7ed659bbb653084b0446bec40197f89e4f2be8b`  
		Last Modified: Tue, 09 Jun 2020 02:49:21 GMT  
		Size: 244.6 KB (244566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4085e4a710b2483a23b0768a54b10e50906e0fcc4f4b76b767b7a24e17ffd4d2`  
		Last Modified: Tue, 09 Jun 2020 02:49:31 GMT  
		Size: 25.3 MB (25253616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff86f58b52cf2bb0b76c3e0c81032af953995ad8cabd583bda9636a431aebaa`  
		Last Modified: Tue, 09 Jun 2020 02:51:07 GMT  
		Size: 129.9 MB (129891245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0` - linux; arm variant v7

```console
$ docker pull mono@sha256:f7ea0e55d8f6d089687e52455f05485d3f4611093df5cef5f0cb090f389beffd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.6 MB (172601822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2989d53c048f30bf6c564534beefa806c0e28eeb03d4a28905e9f05a715550c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:06:35 GMT
ADD file:4a0a863669948b35130fcf8cdb52999c49f7b3ee0620a1eef5f1a2e850a42f05 in / 
# Tue, 09 Jun 2020 01:06:37 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:50:02 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 04:50:28 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:51:11 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 04:56:20 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c439312a9c212b64af3c38cb326bb5fbe14bcf4a622115d59d44985e949bee82`  
		Last Modified: Tue, 09 Jun 2020 01:13:51 GMT  
		Size: 19.3 MB (19304370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0744b2f0bcb57875b07f1fa0fbcdfc6428593f823a41eb4698aab5b67ca5506f`  
		Last Modified: Tue, 09 Jun 2020 05:02:26 GMT  
		Size: 244.6 KB (244584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974d12d4793bb92f0ca8b3600115464d11bc0068af45f530f20adc882117d7bf`  
		Last Modified: Tue, 09 Jun 2020 05:02:36 GMT  
		Size: 24.5 MB (24498272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ec9f63e6708b28c4d538b45025dfbd0a318ab06d761ded9d48f44442c898a7`  
		Last Modified: Tue, 09 Jun 2020 05:04:00 GMT  
		Size: 128.6 MB (128554596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:68d1db7da63e2106ddea8d7850cf3badfaa16a94d8d23a12910f86785e4decc8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.6 MB (194642181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf6ff587bef5367449ceee09405f75d3b5a38e19c0d360ec43da1874b37497aa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:49 GMT
ADD file:c85d28567b6123deb660b71c8b60d92378b5ba15ba5dcf495d9388817dc3aa44 in / 
# Tue, 09 Jun 2020 01:54:52 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 03:24:02 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 03:24:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 03:25:06 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 03:30:31 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:622dc742b82743ebf5607b215a65869096390ee41b0a61b5532f859fb94590b1`  
		Last Modified: Tue, 09 Jun 2020 02:00:28 GMT  
		Size: 20.4 MB (20375150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334cf34398cfa7031d68bad42f6b2a8d870a4ad5c2b0454f3f6fdd0fb4433237`  
		Last Modified: Tue, 09 Jun 2020 03:37:02 GMT  
		Size: 244.4 KB (244374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa8cbd821b66a8c4a38ce3d6711cc1ee5489b04a017ab6a7fd368f08beec89e`  
		Last Modified: Tue, 09 Jun 2020 03:37:10 GMT  
		Size: 29.3 MB (29310269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f78bf65ea03cc9db2213ce7ff8e07d3a77604a43ef0a7d81b88b5c965515dfe`  
		Last Modified: Tue, 09 Jun 2020 03:38:38 GMT  
		Size: 144.7 MB (144712388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0` - linux; 386

```console
$ docker pull mono@sha256:443376dd685b5fcd1e0b6b7a685c5b6a24a79fad8b9619e983293b70e84c8bb6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.4 MB (243401430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6948fdbf966360cb7a728eae30756da2daa5cc4b0362dd09e3a352f4ee44e5dc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:42:33 GMT
ADD file:8ef252685ffefc58654053bf145c830928a2cf423a6c757180649df772f1523d in / 
# Tue, 09 Jun 2020 01:42:34 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 06:59:35 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 06:59:46 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 07:00:24 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 07:05:03 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4ffbd6ec7974e514763a8d7d9fcf5e86e9440e2280e6e9561ea373b4bc50588e`  
		Last Modified: Tue, 09 Jun 2020 01:48:28 GMT  
		Size: 23.1 MB (23147892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b3a90700548ab3df378beb07af7fba67e7ea89ead888d8c78d529c40633c7ed`  
		Last Modified: Tue, 09 Jun 2020 07:10:23 GMT  
		Size: 244.5 KB (244462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbcec5e4a352eead9b06946ed8fb1855a57123b280b3941614dac805987d5b65`  
		Last Modified: Tue, 09 Jun 2020 07:10:41 GMT  
		Size: 68.5 MB (68517280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8167823b3a297ca26719112fd4ae0b1b90e5df5ef7edf3302022c64061697f`  
		Last Modified: Tue, 09 Jun 2020 07:12:09 GMT  
		Size: 151.5 MB (151491796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0` - linux; ppc64le

```console
$ docker pull mono@sha256:70c1fcea14ad2b7622978d2eb2d5626f8d5363e014b6f4974af4a4d5c15f7fac
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.9 MB (178895806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86adafe85745a7a969d3013f3ec3d1d66c603a377e21e1973c2c1eea147f78da`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:25:38 GMT
ADD file:41ec53d65aa183c2835f73989c9e4922f818e59774811eaa6e7395e5a36d5eab in / 
# Tue, 09 Jun 2020 01:25:42 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:37:42 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 04:39:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:40:39 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 04:51:22 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a29e28607c9b96acae7ff89e56214e4339a87c59e40a6f030fa4cbcaab753f2c`  
		Last Modified: Tue, 09 Jun 2020 01:37:25 GMT  
		Size: 22.8 MB (22791269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1fc192a4485fb46ca92b8e704feb4d02fab0a2a37cb4238017caf8d50239d5`  
		Last Modified: Tue, 09 Jun 2020 05:05:25 GMT  
		Size: 244.7 KB (244663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc43661bb843c17c3ae2b4bc4f6d7ffbc36d936efa982c85608c72360c89b849`  
		Last Modified: Tue, 09 Jun 2020 05:05:31 GMT  
		Size: 25.7 MB (25670188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:942f4a6a782ccadbdc03b5cda25e2632ae9bf2dbd213b5dfee3b75376ad65086`  
		Last Modified: Tue, 09 Jun 2020 05:06:55 GMT  
		Size: 130.2 MB (130189686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.8.0.96`

```console
$ docker pull mono@sha256:27d6a38bce172791c9b5961746b81b0cf95dc6d4b54500832427a5ee67fa9bfb
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
$ docker pull mono@sha256:21d11d8967f3ae2b3300a7dab5d5034fde699168cd2ef2da1322b7984c3b2b32
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.1 MB (235143779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b074d513c5cdfadffc24239c00962926b7b965e64cbc06b7c8ad4d110d77f4cd`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 19:31:02 GMT
ENV MONO_VERSION=6.8.0.96
# Fri, 15 May 2020 19:31:11 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 19:31:50 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 15 May 2020 19:44:52 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79aabb192e71d4e3020dd335c1061c5e9f915b73f367e8aeedf757b6adbc9c4`  
		Last Modified: Fri, 15 May 2020 20:05:47 GMT  
		Size: 244.5 KB (244497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96073affb70fefc051a7bb5f06242765faddc3114c900ccc1af9108910e6517`  
		Last Modified: Fri, 15 May 2020 20:06:04 GMT  
		Size: 64.6 MB (64584727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea44fa8b0fc1cfc5cfcf575269513b0ce648b1604436a20cc8c54fa2af29c32`  
		Last Modified: Fri, 15 May 2020 20:07:27 GMT  
		Size: 147.8 MB (147794668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.96` - linux; arm variant v5

```console
$ docker pull mono@sha256:d9c5ac0a34b9a4e40f2d5e63dcf776580e1f2be35ccfbe826b2da4e0441e15dc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.6 MB (176586764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad5f102651a6fa59023237fc450eb5316c9e92611685d7dcb277abdcefbd8390`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 00:55:49 GMT
ADD file:af949d376cc9a2ac87d0052d22fe17be59dfe65905f0645d1a903b359208d26d in / 
# Tue, 09 Jun 2020 00:55:51 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:34:30 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 02:35:00 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 02:35:52 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 02:42:32 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c9b35828d9245f0a85299b96b2d9b0d70390689cf7df0fe7ef29ca6028c0ab56`  
		Last Modified: Tue, 09 Jun 2020 01:03:09 GMT  
		Size: 21.2 MB (21197337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f2cf80f102f97dd711f97ed7ed659bbb653084b0446bec40197f89e4f2be8b`  
		Last Modified: Tue, 09 Jun 2020 02:49:21 GMT  
		Size: 244.6 KB (244566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4085e4a710b2483a23b0768a54b10e50906e0fcc4f4b76b767b7a24e17ffd4d2`  
		Last Modified: Tue, 09 Jun 2020 02:49:31 GMT  
		Size: 25.3 MB (25253616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff86f58b52cf2bb0b76c3e0c81032af953995ad8cabd583bda9636a431aebaa`  
		Last Modified: Tue, 09 Jun 2020 02:51:07 GMT  
		Size: 129.9 MB (129891245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.96` - linux; arm variant v7

```console
$ docker pull mono@sha256:f7ea0e55d8f6d089687e52455f05485d3f4611093df5cef5f0cb090f389beffd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.6 MB (172601822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2989d53c048f30bf6c564534beefa806c0e28eeb03d4a28905e9f05a715550c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:06:35 GMT
ADD file:4a0a863669948b35130fcf8cdb52999c49f7b3ee0620a1eef5f1a2e850a42f05 in / 
# Tue, 09 Jun 2020 01:06:37 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:50:02 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 04:50:28 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:51:11 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 04:56:20 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c439312a9c212b64af3c38cb326bb5fbe14bcf4a622115d59d44985e949bee82`  
		Last Modified: Tue, 09 Jun 2020 01:13:51 GMT  
		Size: 19.3 MB (19304370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0744b2f0bcb57875b07f1fa0fbcdfc6428593f823a41eb4698aab5b67ca5506f`  
		Last Modified: Tue, 09 Jun 2020 05:02:26 GMT  
		Size: 244.6 KB (244584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974d12d4793bb92f0ca8b3600115464d11bc0068af45f530f20adc882117d7bf`  
		Last Modified: Tue, 09 Jun 2020 05:02:36 GMT  
		Size: 24.5 MB (24498272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ec9f63e6708b28c4d538b45025dfbd0a318ab06d761ded9d48f44442c898a7`  
		Last Modified: Tue, 09 Jun 2020 05:04:00 GMT  
		Size: 128.6 MB (128554596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.96` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:68d1db7da63e2106ddea8d7850cf3badfaa16a94d8d23a12910f86785e4decc8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.6 MB (194642181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf6ff587bef5367449ceee09405f75d3b5a38e19c0d360ec43da1874b37497aa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:49 GMT
ADD file:c85d28567b6123deb660b71c8b60d92378b5ba15ba5dcf495d9388817dc3aa44 in / 
# Tue, 09 Jun 2020 01:54:52 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 03:24:02 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 03:24:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 03:25:06 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 03:30:31 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:622dc742b82743ebf5607b215a65869096390ee41b0a61b5532f859fb94590b1`  
		Last Modified: Tue, 09 Jun 2020 02:00:28 GMT  
		Size: 20.4 MB (20375150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334cf34398cfa7031d68bad42f6b2a8d870a4ad5c2b0454f3f6fdd0fb4433237`  
		Last Modified: Tue, 09 Jun 2020 03:37:02 GMT  
		Size: 244.4 KB (244374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa8cbd821b66a8c4a38ce3d6711cc1ee5489b04a017ab6a7fd368f08beec89e`  
		Last Modified: Tue, 09 Jun 2020 03:37:10 GMT  
		Size: 29.3 MB (29310269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f78bf65ea03cc9db2213ce7ff8e07d3a77604a43ef0a7d81b88b5c965515dfe`  
		Last Modified: Tue, 09 Jun 2020 03:38:38 GMT  
		Size: 144.7 MB (144712388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.96` - linux; 386

```console
$ docker pull mono@sha256:443376dd685b5fcd1e0b6b7a685c5b6a24a79fad8b9619e983293b70e84c8bb6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.4 MB (243401430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6948fdbf966360cb7a728eae30756da2daa5cc4b0362dd09e3a352f4ee44e5dc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:42:33 GMT
ADD file:8ef252685ffefc58654053bf145c830928a2cf423a6c757180649df772f1523d in / 
# Tue, 09 Jun 2020 01:42:34 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 06:59:35 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 06:59:46 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 07:00:24 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 07:05:03 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4ffbd6ec7974e514763a8d7d9fcf5e86e9440e2280e6e9561ea373b4bc50588e`  
		Last Modified: Tue, 09 Jun 2020 01:48:28 GMT  
		Size: 23.1 MB (23147892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b3a90700548ab3df378beb07af7fba67e7ea89ead888d8c78d529c40633c7ed`  
		Last Modified: Tue, 09 Jun 2020 07:10:23 GMT  
		Size: 244.5 KB (244462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbcec5e4a352eead9b06946ed8fb1855a57123b280b3941614dac805987d5b65`  
		Last Modified: Tue, 09 Jun 2020 07:10:41 GMT  
		Size: 68.5 MB (68517280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8167823b3a297ca26719112fd4ae0b1b90e5df5ef7edf3302022c64061697f`  
		Last Modified: Tue, 09 Jun 2020 07:12:09 GMT  
		Size: 151.5 MB (151491796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.96` - linux; ppc64le

```console
$ docker pull mono@sha256:70c1fcea14ad2b7622978d2eb2d5626f8d5363e014b6f4974af4a4d5c15f7fac
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.9 MB (178895806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86adafe85745a7a969d3013f3ec3d1d66c603a377e21e1973c2c1eea147f78da`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:25:38 GMT
ADD file:41ec53d65aa183c2835f73989c9e4922f818e59774811eaa6e7395e5a36d5eab in / 
# Tue, 09 Jun 2020 01:25:42 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:37:42 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 04:39:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:40:39 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 04:51:22 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a29e28607c9b96acae7ff89e56214e4339a87c59e40a6f030fa4cbcaab753f2c`  
		Last Modified: Tue, 09 Jun 2020 01:37:25 GMT  
		Size: 22.8 MB (22791269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1fc192a4485fb46ca92b8e704feb4d02fab0a2a37cb4238017caf8d50239d5`  
		Last Modified: Tue, 09 Jun 2020 05:05:25 GMT  
		Size: 244.7 KB (244663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc43661bb843c17c3ae2b4bc4f6d7ffbc36d936efa982c85608c72360c89b849`  
		Last Modified: Tue, 09 Jun 2020 05:05:31 GMT  
		Size: 25.7 MB (25670188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:942f4a6a782ccadbdc03b5cda25e2632ae9bf2dbd213b5dfee3b75376ad65086`  
		Last Modified: Tue, 09 Jun 2020 05:06:55 GMT  
		Size: 130.2 MB (130189686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.8.0.96-slim`

```console
$ docker pull mono@sha256:b575faa4607afa6dbdbafeecf0142953a6e125b1fed1e82e7928327f4ceb628e
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
$ docker pull mono@sha256:71b58b88ce426661d7e4d0741c99c0f0696f727104b1526868dabb58746ea880
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.3 MB (87349111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f20894fd43d160c828a47baf344a1a7bb2b70fcc3ffa98531b571c5043af2910`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 19:31:02 GMT
ENV MONO_VERSION=6.8.0.96
# Fri, 15 May 2020 19:31:11 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 19:31:50 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79aabb192e71d4e3020dd335c1061c5e9f915b73f367e8aeedf757b6adbc9c4`  
		Last Modified: Fri, 15 May 2020 20:05:47 GMT  
		Size: 244.5 KB (244497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96073affb70fefc051a7bb5f06242765faddc3114c900ccc1af9108910e6517`  
		Last Modified: Fri, 15 May 2020 20:06:04 GMT  
		Size: 64.6 MB (64584727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.96-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:de05d2ff43714ddd9e033377d758bc9464db4e95fa409e8f1c0fdf6c679bc827
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46695519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7a5341e68dbc97765d2a7b2eb4ddba90915fe57a702fadac48b4823463a7934`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 00:55:49 GMT
ADD file:af949d376cc9a2ac87d0052d22fe17be59dfe65905f0645d1a903b359208d26d in / 
# Tue, 09 Jun 2020 00:55:51 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:34:30 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 02:35:00 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 02:35:52 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c9b35828d9245f0a85299b96b2d9b0d70390689cf7df0fe7ef29ca6028c0ab56`  
		Last Modified: Tue, 09 Jun 2020 01:03:09 GMT  
		Size: 21.2 MB (21197337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f2cf80f102f97dd711f97ed7ed659bbb653084b0446bec40197f89e4f2be8b`  
		Last Modified: Tue, 09 Jun 2020 02:49:21 GMT  
		Size: 244.6 KB (244566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4085e4a710b2483a23b0768a54b10e50906e0fcc4f4b76b767b7a24e17ffd4d2`  
		Last Modified: Tue, 09 Jun 2020 02:49:31 GMT  
		Size: 25.3 MB (25253616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.96-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:87f0fbcfcbfcb2ab20602ca0819f0e1020cd9bd7176594b72d9c88c2304c7272
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (44047226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e75eb00ebe1466aff449d4a9b760038e7c9839a04d1b9cc68da510a74af6233e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:06:35 GMT
ADD file:4a0a863669948b35130fcf8cdb52999c49f7b3ee0620a1eef5f1a2e850a42f05 in / 
# Tue, 09 Jun 2020 01:06:37 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:50:02 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 04:50:28 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:51:11 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c439312a9c212b64af3c38cb326bb5fbe14bcf4a622115d59d44985e949bee82`  
		Last Modified: Tue, 09 Jun 2020 01:13:51 GMT  
		Size: 19.3 MB (19304370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0744b2f0bcb57875b07f1fa0fbcdfc6428593f823a41eb4698aab5b67ca5506f`  
		Last Modified: Tue, 09 Jun 2020 05:02:26 GMT  
		Size: 244.6 KB (244584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974d12d4793bb92f0ca8b3600115464d11bc0068af45f530f20adc882117d7bf`  
		Last Modified: Tue, 09 Jun 2020 05:02:36 GMT  
		Size: 24.5 MB (24498272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.96-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:24d8471bd7e59cc38ba65db018794a92fc6d54960784f86d52c913e4a8f5c9a9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 MB (49929793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb86494c128abaa467fc19a192852bfde9ae94e0d13aa1f9f1b70d9adb68697d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:49 GMT
ADD file:c85d28567b6123deb660b71c8b60d92378b5ba15ba5dcf495d9388817dc3aa44 in / 
# Tue, 09 Jun 2020 01:54:52 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 03:24:02 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 03:24:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 03:25:06 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:622dc742b82743ebf5607b215a65869096390ee41b0a61b5532f859fb94590b1`  
		Last Modified: Tue, 09 Jun 2020 02:00:28 GMT  
		Size: 20.4 MB (20375150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334cf34398cfa7031d68bad42f6b2a8d870a4ad5c2b0454f3f6fdd0fb4433237`  
		Last Modified: Tue, 09 Jun 2020 03:37:02 GMT  
		Size: 244.4 KB (244374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa8cbd821b66a8c4a38ce3d6711cc1ee5489b04a017ab6a7fd368f08beec89e`  
		Last Modified: Tue, 09 Jun 2020 03:37:10 GMT  
		Size: 29.3 MB (29310269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.96-slim` - linux; 386

```console
$ docker pull mono@sha256:e78d5446f93beef2216681d481890fe6388d64c704eb5cd4cc2e7010748818bd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.9 MB (91909634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ebdb565c91f1fbc53a06cbfb5b9c374ab82f491c6934131ce4f1ae6524b43cf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:42:33 GMT
ADD file:8ef252685ffefc58654053bf145c830928a2cf423a6c757180649df772f1523d in / 
# Tue, 09 Jun 2020 01:42:34 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 06:59:35 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 06:59:46 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 07:00:24 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4ffbd6ec7974e514763a8d7d9fcf5e86e9440e2280e6e9561ea373b4bc50588e`  
		Last Modified: Tue, 09 Jun 2020 01:48:28 GMT  
		Size: 23.1 MB (23147892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b3a90700548ab3df378beb07af7fba67e7ea89ead888d8c78d529c40633c7ed`  
		Last Modified: Tue, 09 Jun 2020 07:10:23 GMT  
		Size: 244.5 KB (244462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbcec5e4a352eead9b06946ed8fb1855a57123b280b3941614dac805987d5b65`  
		Last Modified: Tue, 09 Jun 2020 07:10:41 GMT  
		Size: 68.5 MB (68517280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0.96-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:2c4949379a4b86afc1273f4a7339ff7bc658bc7749205fb8df632bfb7a7f1d63
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48706120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17986d4009e9231ade165cd631103027df60340b2b4b6fa078cdb34805a602ba`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:25:38 GMT
ADD file:41ec53d65aa183c2835f73989c9e4922f818e59774811eaa6e7395e5a36d5eab in / 
# Tue, 09 Jun 2020 01:25:42 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:37:42 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 04:39:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:40:39 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a29e28607c9b96acae7ff89e56214e4339a87c59e40a6f030fa4cbcaab753f2c`  
		Last Modified: Tue, 09 Jun 2020 01:37:25 GMT  
		Size: 22.8 MB (22791269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1fc192a4485fb46ca92b8e704feb4d02fab0a2a37cb4238017caf8d50239d5`  
		Last Modified: Tue, 09 Jun 2020 05:05:25 GMT  
		Size: 244.7 KB (244663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc43661bb843c17c3ae2b4bc4f6d7ffbc36d936efa982c85608c72360c89b849`  
		Last Modified: Tue, 09 Jun 2020 05:05:31 GMT  
		Size: 25.7 MB (25670188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.8.0-slim`

```console
$ docker pull mono@sha256:b575faa4607afa6dbdbafeecf0142953a6e125b1fed1e82e7928327f4ceb628e
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
$ docker pull mono@sha256:71b58b88ce426661d7e4d0741c99c0f0696f727104b1526868dabb58746ea880
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.3 MB (87349111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f20894fd43d160c828a47baf344a1a7bb2b70fcc3ffa98531b571c5043af2910`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 19:31:02 GMT
ENV MONO_VERSION=6.8.0.96
# Fri, 15 May 2020 19:31:11 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 19:31:50 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79aabb192e71d4e3020dd335c1061c5e9f915b73f367e8aeedf757b6adbc9c4`  
		Last Modified: Fri, 15 May 2020 20:05:47 GMT  
		Size: 244.5 KB (244497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96073affb70fefc051a7bb5f06242765faddc3114c900ccc1af9108910e6517`  
		Last Modified: Fri, 15 May 2020 20:06:04 GMT  
		Size: 64.6 MB (64584727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:de05d2ff43714ddd9e033377d758bc9464db4e95fa409e8f1c0fdf6c679bc827
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46695519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7a5341e68dbc97765d2a7b2eb4ddba90915fe57a702fadac48b4823463a7934`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 00:55:49 GMT
ADD file:af949d376cc9a2ac87d0052d22fe17be59dfe65905f0645d1a903b359208d26d in / 
# Tue, 09 Jun 2020 00:55:51 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:34:30 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 02:35:00 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 02:35:52 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c9b35828d9245f0a85299b96b2d9b0d70390689cf7df0fe7ef29ca6028c0ab56`  
		Last Modified: Tue, 09 Jun 2020 01:03:09 GMT  
		Size: 21.2 MB (21197337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f2cf80f102f97dd711f97ed7ed659bbb653084b0446bec40197f89e4f2be8b`  
		Last Modified: Tue, 09 Jun 2020 02:49:21 GMT  
		Size: 244.6 KB (244566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4085e4a710b2483a23b0768a54b10e50906e0fcc4f4b76b767b7a24e17ffd4d2`  
		Last Modified: Tue, 09 Jun 2020 02:49:31 GMT  
		Size: 25.3 MB (25253616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:87f0fbcfcbfcb2ab20602ca0819f0e1020cd9bd7176594b72d9c88c2304c7272
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (44047226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e75eb00ebe1466aff449d4a9b760038e7c9839a04d1b9cc68da510a74af6233e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:06:35 GMT
ADD file:4a0a863669948b35130fcf8cdb52999c49f7b3ee0620a1eef5f1a2e850a42f05 in / 
# Tue, 09 Jun 2020 01:06:37 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:50:02 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 04:50:28 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:51:11 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c439312a9c212b64af3c38cb326bb5fbe14bcf4a622115d59d44985e949bee82`  
		Last Modified: Tue, 09 Jun 2020 01:13:51 GMT  
		Size: 19.3 MB (19304370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0744b2f0bcb57875b07f1fa0fbcdfc6428593f823a41eb4698aab5b67ca5506f`  
		Last Modified: Tue, 09 Jun 2020 05:02:26 GMT  
		Size: 244.6 KB (244584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974d12d4793bb92f0ca8b3600115464d11bc0068af45f530f20adc882117d7bf`  
		Last Modified: Tue, 09 Jun 2020 05:02:36 GMT  
		Size: 24.5 MB (24498272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:24d8471bd7e59cc38ba65db018794a92fc6d54960784f86d52c913e4a8f5c9a9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 MB (49929793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb86494c128abaa467fc19a192852bfde9ae94e0d13aa1f9f1b70d9adb68697d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:49 GMT
ADD file:c85d28567b6123deb660b71c8b60d92378b5ba15ba5dcf495d9388817dc3aa44 in / 
# Tue, 09 Jun 2020 01:54:52 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 03:24:02 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 03:24:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 03:25:06 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:622dc742b82743ebf5607b215a65869096390ee41b0a61b5532f859fb94590b1`  
		Last Modified: Tue, 09 Jun 2020 02:00:28 GMT  
		Size: 20.4 MB (20375150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334cf34398cfa7031d68bad42f6b2a8d870a4ad5c2b0454f3f6fdd0fb4433237`  
		Last Modified: Tue, 09 Jun 2020 03:37:02 GMT  
		Size: 244.4 KB (244374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa8cbd821b66a8c4a38ce3d6711cc1ee5489b04a017ab6a7fd368f08beec89e`  
		Last Modified: Tue, 09 Jun 2020 03:37:10 GMT  
		Size: 29.3 MB (29310269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0-slim` - linux; 386

```console
$ docker pull mono@sha256:e78d5446f93beef2216681d481890fe6388d64c704eb5cd4cc2e7010748818bd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.9 MB (91909634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ebdb565c91f1fbc53a06cbfb5b9c374ab82f491c6934131ce4f1ae6524b43cf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:42:33 GMT
ADD file:8ef252685ffefc58654053bf145c830928a2cf423a6c757180649df772f1523d in / 
# Tue, 09 Jun 2020 01:42:34 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 06:59:35 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 06:59:46 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 07:00:24 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4ffbd6ec7974e514763a8d7d9fcf5e86e9440e2280e6e9561ea373b4bc50588e`  
		Last Modified: Tue, 09 Jun 2020 01:48:28 GMT  
		Size: 23.1 MB (23147892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b3a90700548ab3df378beb07af7fba67e7ea89ead888d8c78d529c40633c7ed`  
		Last Modified: Tue, 09 Jun 2020 07:10:23 GMT  
		Size: 244.5 KB (244462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbcec5e4a352eead9b06946ed8fb1855a57123b280b3941614dac805987d5b65`  
		Last Modified: Tue, 09 Jun 2020 07:10:41 GMT  
		Size: 68.5 MB (68517280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8.0-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:2c4949379a4b86afc1273f4a7339ff7bc658bc7749205fb8df632bfb7a7f1d63
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48706120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17986d4009e9231ade165cd631103027df60340b2b4b6fa078cdb34805a602ba`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:25:38 GMT
ADD file:41ec53d65aa183c2835f73989c9e4922f818e59774811eaa6e7395e5a36d5eab in / 
# Tue, 09 Jun 2020 01:25:42 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:37:42 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 04:39:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:40:39 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a29e28607c9b96acae7ff89e56214e4339a87c59e40a6f030fa4cbcaab753f2c`  
		Last Modified: Tue, 09 Jun 2020 01:37:25 GMT  
		Size: 22.8 MB (22791269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1fc192a4485fb46ca92b8e704feb4d02fab0a2a37cb4238017caf8d50239d5`  
		Last Modified: Tue, 09 Jun 2020 05:05:25 GMT  
		Size: 244.7 KB (244663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc43661bb843c17c3ae2b4bc4f6d7ffbc36d936efa982c85608c72360c89b849`  
		Last Modified: Tue, 09 Jun 2020 05:05:31 GMT  
		Size: 25.7 MB (25670188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6.8-slim`

```console
$ docker pull mono@sha256:b575faa4607afa6dbdbafeecf0142953a6e125b1fed1e82e7928327f4ceb628e
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
$ docker pull mono@sha256:71b58b88ce426661d7e4d0741c99c0f0696f727104b1526868dabb58746ea880
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.3 MB (87349111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f20894fd43d160c828a47baf344a1a7bb2b70fcc3ffa98531b571c5043af2910`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 19:31:02 GMT
ENV MONO_VERSION=6.8.0.96
# Fri, 15 May 2020 19:31:11 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 19:31:50 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79aabb192e71d4e3020dd335c1061c5e9f915b73f367e8aeedf757b6adbc9c4`  
		Last Modified: Fri, 15 May 2020 20:05:47 GMT  
		Size: 244.5 KB (244497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96073affb70fefc051a7bb5f06242765faddc3114c900ccc1af9108910e6517`  
		Last Modified: Fri, 15 May 2020 20:06:04 GMT  
		Size: 64.6 MB (64584727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:de05d2ff43714ddd9e033377d758bc9464db4e95fa409e8f1c0fdf6c679bc827
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46695519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7a5341e68dbc97765d2a7b2eb4ddba90915fe57a702fadac48b4823463a7934`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 00:55:49 GMT
ADD file:af949d376cc9a2ac87d0052d22fe17be59dfe65905f0645d1a903b359208d26d in / 
# Tue, 09 Jun 2020 00:55:51 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:34:30 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 02:35:00 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 02:35:52 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c9b35828d9245f0a85299b96b2d9b0d70390689cf7df0fe7ef29ca6028c0ab56`  
		Last Modified: Tue, 09 Jun 2020 01:03:09 GMT  
		Size: 21.2 MB (21197337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f2cf80f102f97dd711f97ed7ed659bbb653084b0446bec40197f89e4f2be8b`  
		Last Modified: Tue, 09 Jun 2020 02:49:21 GMT  
		Size: 244.6 KB (244566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4085e4a710b2483a23b0768a54b10e50906e0fcc4f4b76b767b7a24e17ffd4d2`  
		Last Modified: Tue, 09 Jun 2020 02:49:31 GMT  
		Size: 25.3 MB (25253616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:87f0fbcfcbfcb2ab20602ca0819f0e1020cd9bd7176594b72d9c88c2304c7272
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (44047226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e75eb00ebe1466aff449d4a9b760038e7c9839a04d1b9cc68da510a74af6233e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:06:35 GMT
ADD file:4a0a863669948b35130fcf8cdb52999c49f7b3ee0620a1eef5f1a2e850a42f05 in / 
# Tue, 09 Jun 2020 01:06:37 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:50:02 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 04:50:28 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:51:11 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c439312a9c212b64af3c38cb326bb5fbe14bcf4a622115d59d44985e949bee82`  
		Last Modified: Tue, 09 Jun 2020 01:13:51 GMT  
		Size: 19.3 MB (19304370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0744b2f0bcb57875b07f1fa0fbcdfc6428593f823a41eb4698aab5b67ca5506f`  
		Last Modified: Tue, 09 Jun 2020 05:02:26 GMT  
		Size: 244.6 KB (244584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974d12d4793bb92f0ca8b3600115464d11bc0068af45f530f20adc882117d7bf`  
		Last Modified: Tue, 09 Jun 2020 05:02:36 GMT  
		Size: 24.5 MB (24498272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:24d8471bd7e59cc38ba65db018794a92fc6d54960784f86d52c913e4a8f5c9a9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 MB (49929793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb86494c128abaa467fc19a192852bfde9ae94e0d13aa1f9f1b70d9adb68697d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:49 GMT
ADD file:c85d28567b6123deb660b71c8b60d92378b5ba15ba5dcf495d9388817dc3aa44 in / 
# Tue, 09 Jun 2020 01:54:52 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 03:24:02 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 03:24:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 03:25:06 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:622dc742b82743ebf5607b215a65869096390ee41b0a61b5532f859fb94590b1`  
		Last Modified: Tue, 09 Jun 2020 02:00:28 GMT  
		Size: 20.4 MB (20375150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334cf34398cfa7031d68bad42f6b2a8d870a4ad5c2b0454f3f6fdd0fb4433237`  
		Last Modified: Tue, 09 Jun 2020 03:37:02 GMT  
		Size: 244.4 KB (244374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa8cbd821b66a8c4a38ce3d6711cc1ee5489b04a017ab6a7fd368f08beec89e`  
		Last Modified: Tue, 09 Jun 2020 03:37:10 GMT  
		Size: 29.3 MB (29310269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8-slim` - linux; 386

```console
$ docker pull mono@sha256:e78d5446f93beef2216681d481890fe6388d64c704eb5cd4cc2e7010748818bd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.9 MB (91909634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ebdb565c91f1fbc53a06cbfb5b9c374ab82f491c6934131ce4f1ae6524b43cf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:42:33 GMT
ADD file:8ef252685ffefc58654053bf145c830928a2cf423a6c757180649df772f1523d in / 
# Tue, 09 Jun 2020 01:42:34 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 06:59:35 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 06:59:46 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 07:00:24 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4ffbd6ec7974e514763a8d7d9fcf5e86e9440e2280e6e9561ea373b4bc50588e`  
		Last Modified: Tue, 09 Jun 2020 01:48:28 GMT  
		Size: 23.1 MB (23147892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b3a90700548ab3df378beb07af7fba67e7ea89ead888d8c78d529c40633c7ed`  
		Last Modified: Tue, 09 Jun 2020 07:10:23 GMT  
		Size: 244.5 KB (244462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbcec5e4a352eead9b06946ed8fb1855a57123b280b3941614dac805987d5b65`  
		Last Modified: Tue, 09 Jun 2020 07:10:41 GMT  
		Size: 68.5 MB (68517280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6.8-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:2c4949379a4b86afc1273f4a7339ff7bc658bc7749205fb8df632bfb7a7f1d63
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48706120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17986d4009e9231ade165cd631103027df60340b2b4b6fa078cdb34805a602ba`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:25:38 GMT
ADD file:41ec53d65aa183c2835f73989c9e4922f818e59774811eaa6e7395e5a36d5eab in / 
# Tue, 09 Jun 2020 01:25:42 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:37:42 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 04:39:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:40:39 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a29e28607c9b96acae7ff89e56214e4339a87c59e40a6f030fa4cbcaab753f2c`  
		Last Modified: Tue, 09 Jun 2020 01:37:25 GMT  
		Size: 22.8 MB (22791269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1fc192a4485fb46ca92b8e704feb4d02fab0a2a37cb4238017caf8d50239d5`  
		Last Modified: Tue, 09 Jun 2020 05:05:25 GMT  
		Size: 244.7 KB (244663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc43661bb843c17c3ae2b4bc4f6d7ffbc36d936efa982c85608c72360c89b849`  
		Last Modified: Tue, 09 Jun 2020 05:05:31 GMT  
		Size: 25.7 MB (25670188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:6-slim`

```console
$ docker pull mono@sha256:b575faa4607afa6dbdbafeecf0142953a6e125b1fed1e82e7928327f4ceb628e
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
$ docker pull mono@sha256:71b58b88ce426661d7e4d0741c99c0f0696f727104b1526868dabb58746ea880
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.3 MB (87349111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f20894fd43d160c828a47baf344a1a7bb2b70fcc3ffa98531b571c5043af2910`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 19:31:02 GMT
ENV MONO_VERSION=6.8.0.96
# Fri, 15 May 2020 19:31:11 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 19:31:50 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79aabb192e71d4e3020dd335c1061c5e9f915b73f367e8aeedf757b6adbc9c4`  
		Last Modified: Fri, 15 May 2020 20:05:47 GMT  
		Size: 244.5 KB (244497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96073affb70fefc051a7bb5f06242765faddc3114c900ccc1af9108910e6517`  
		Last Modified: Fri, 15 May 2020 20:06:04 GMT  
		Size: 64.6 MB (64584727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:de05d2ff43714ddd9e033377d758bc9464db4e95fa409e8f1c0fdf6c679bc827
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46695519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7a5341e68dbc97765d2a7b2eb4ddba90915fe57a702fadac48b4823463a7934`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 00:55:49 GMT
ADD file:af949d376cc9a2ac87d0052d22fe17be59dfe65905f0645d1a903b359208d26d in / 
# Tue, 09 Jun 2020 00:55:51 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:34:30 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 02:35:00 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 02:35:52 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c9b35828d9245f0a85299b96b2d9b0d70390689cf7df0fe7ef29ca6028c0ab56`  
		Last Modified: Tue, 09 Jun 2020 01:03:09 GMT  
		Size: 21.2 MB (21197337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f2cf80f102f97dd711f97ed7ed659bbb653084b0446bec40197f89e4f2be8b`  
		Last Modified: Tue, 09 Jun 2020 02:49:21 GMT  
		Size: 244.6 KB (244566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4085e4a710b2483a23b0768a54b10e50906e0fcc4f4b76b767b7a24e17ffd4d2`  
		Last Modified: Tue, 09 Jun 2020 02:49:31 GMT  
		Size: 25.3 MB (25253616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:87f0fbcfcbfcb2ab20602ca0819f0e1020cd9bd7176594b72d9c88c2304c7272
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (44047226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e75eb00ebe1466aff449d4a9b760038e7c9839a04d1b9cc68da510a74af6233e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:06:35 GMT
ADD file:4a0a863669948b35130fcf8cdb52999c49f7b3ee0620a1eef5f1a2e850a42f05 in / 
# Tue, 09 Jun 2020 01:06:37 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:50:02 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 04:50:28 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:51:11 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c439312a9c212b64af3c38cb326bb5fbe14bcf4a622115d59d44985e949bee82`  
		Last Modified: Tue, 09 Jun 2020 01:13:51 GMT  
		Size: 19.3 MB (19304370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0744b2f0bcb57875b07f1fa0fbcdfc6428593f823a41eb4698aab5b67ca5506f`  
		Last Modified: Tue, 09 Jun 2020 05:02:26 GMT  
		Size: 244.6 KB (244584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974d12d4793bb92f0ca8b3600115464d11bc0068af45f530f20adc882117d7bf`  
		Last Modified: Tue, 09 Jun 2020 05:02:36 GMT  
		Size: 24.5 MB (24498272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:24d8471bd7e59cc38ba65db018794a92fc6d54960784f86d52c913e4a8f5c9a9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 MB (49929793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb86494c128abaa467fc19a192852bfde9ae94e0d13aa1f9f1b70d9adb68697d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:49 GMT
ADD file:c85d28567b6123deb660b71c8b60d92378b5ba15ba5dcf495d9388817dc3aa44 in / 
# Tue, 09 Jun 2020 01:54:52 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 03:24:02 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 03:24:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 03:25:06 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:622dc742b82743ebf5607b215a65869096390ee41b0a61b5532f859fb94590b1`  
		Last Modified: Tue, 09 Jun 2020 02:00:28 GMT  
		Size: 20.4 MB (20375150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334cf34398cfa7031d68bad42f6b2a8d870a4ad5c2b0454f3f6fdd0fb4433237`  
		Last Modified: Tue, 09 Jun 2020 03:37:02 GMT  
		Size: 244.4 KB (244374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa8cbd821b66a8c4a38ce3d6711cc1ee5489b04a017ab6a7fd368f08beec89e`  
		Last Modified: Tue, 09 Jun 2020 03:37:10 GMT  
		Size: 29.3 MB (29310269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; 386

```console
$ docker pull mono@sha256:e78d5446f93beef2216681d481890fe6388d64c704eb5cd4cc2e7010748818bd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.9 MB (91909634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ebdb565c91f1fbc53a06cbfb5b9c374ab82f491c6934131ce4f1ae6524b43cf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:42:33 GMT
ADD file:8ef252685ffefc58654053bf145c830928a2cf423a6c757180649df772f1523d in / 
# Tue, 09 Jun 2020 01:42:34 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 06:59:35 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 06:59:46 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 07:00:24 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4ffbd6ec7974e514763a8d7d9fcf5e86e9440e2280e6e9561ea373b4bc50588e`  
		Last Modified: Tue, 09 Jun 2020 01:48:28 GMT  
		Size: 23.1 MB (23147892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b3a90700548ab3df378beb07af7fba67e7ea89ead888d8c78d529c40633c7ed`  
		Last Modified: Tue, 09 Jun 2020 07:10:23 GMT  
		Size: 244.5 KB (244462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbcec5e4a352eead9b06946ed8fb1855a57123b280b3941614dac805987d5b65`  
		Last Modified: Tue, 09 Jun 2020 07:10:41 GMT  
		Size: 68.5 MB (68517280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:2c4949379a4b86afc1273f4a7339ff7bc658bc7749205fb8df632bfb7a7f1d63
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48706120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17986d4009e9231ade165cd631103027df60340b2b4b6fa078cdb34805a602ba`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:25:38 GMT
ADD file:41ec53d65aa183c2835f73989c9e4922f818e59774811eaa6e7395e5a36d5eab in / 
# Tue, 09 Jun 2020 01:25:42 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:37:42 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 04:39:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:40:39 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a29e28607c9b96acae7ff89e56214e4339a87c59e40a6f030fa4cbcaab753f2c`  
		Last Modified: Tue, 09 Jun 2020 01:37:25 GMT  
		Size: 22.8 MB (22791269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1fc192a4485fb46ca92b8e704feb4d02fab0a2a37cb4238017caf8d50239d5`  
		Last Modified: Tue, 09 Jun 2020 05:05:25 GMT  
		Size: 244.7 KB (244663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc43661bb843c17c3ae2b4bc4f6d7ffbc36d936efa982c85608c72360c89b849`  
		Last Modified: Tue, 09 Jun 2020 05:05:31 GMT  
		Size: 25.7 MB (25670188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:latest`

```console
$ docker pull mono@sha256:27d6a38bce172791c9b5961746b81b0cf95dc6d4b54500832427a5ee67fa9bfb
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
$ docker pull mono@sha256:21d11d8967f3ae2b3300a7dab5d5034fde699168cd2ef2da1322b7984c3b2b32
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.1 MB (235143779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b074d513c5cdfadffc24239c00962926b7b965e64cbc06b7c8ad4d110d77f4cd`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 19:31:02 GMT
ENV MONO_VERSION=6.8.0.96
# Fri, 15 May 2020 19:31:11 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 19:31:50 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 15 May 2020 19:44:52 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79aabb192e71d4e3020dd335c1061c5e9f915b73f367e8aeedf757b6adbc9c4`  
		Last Modified: Fri, 15 May 2020 20:05:47 GMT  
		Size: 244.5 KB (244497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96073affb70fefc051a7bb5f06242765faddc3114c900ccc1af9108910e6517`  
		Last Modified: Fri, 15 May 2020 20:06:04 GMT  
		Size: 64.6 MB (64584727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea44fa8b0fc1cfc5cfcf575269513b0ce648b1604436a20cc8c54fa2af29c32`  
		Last Modified: Fri, 15 May 2020 20:07:27 GMT  
		Size: 147.8 MB (147794668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm variant v5

```console
$ docker pull mono@sha256:d9c5ac0a34b9a4e40f2d5e63dcf776580e1f2be35ccfbe826b2da4e0441e15dc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.6 MB (176586764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad5f102651a6fa59023237fc450eb5316c9e92611685d7dcb277abdcefbd8390`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 00:55:49 GMT
ADD file:af949d376cc9a2ac87d0052d22fe17be59dfe65905f0645d1a903b359208d26d in / 
# Tue, 09 Jun 2020 00:55:51 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:34:30 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 02:35:00 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 02:35:52 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 02:42:32 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c9b35828d9245f0a85299b96b2d9b0d70390689cf7df0fe7ef29ca6028c0ab56`  
		Last Modified: Tue, 09 Jun 2020 01:03:09 GMT  
		Size: 21.2 MB (21197337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f2cf80f102f97dd711f97ed7ed659bbb653084b0446bec40197f89e4f2be8b`  
		Last Modified: Tue, 09 Jun 2020 02:49:21 GMT  
		Size: 244.6 KB (244566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4085e4a710b2483a23b0768a54b10e50906e0fcc4f4b76b767b7a24e17ffd4d2`  
		Last Modified: Tue, 09 Jun 2020 02:49:31 GMT  
		Size: 25.3 MB (25253616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff86f58b52cf2bb0b76c3e0c81032af953995ad8cabd583bda9636a431aebaa`  
		Last Modified: Tue, 09 Jun 2020 02:51:07 GMT  
		Size: 129.9 MB (129891245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm variant v7

```console
$ docker pull mono@sha256:f7ea0e55d8f6d089687e52455f05485d3f4611093df5cef5f0cb090f389beffd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.6 MB (172601822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2989d53c048f30bf6c564534beefa806c0e28eeb03d4a28905e9f05a715550c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:06:35 GMT
ADD file:4a0a863669948b35130fcf8cdb52999c49f7b3ee0620a1eef5f1a2e850a42f05 in / 
# Tue, 09 Jun 2020 01:06:37 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:50:02 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 04:50:28 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:51:11 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 04:56:20 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c439312a9c212b64af3c38cb326bb5fbe14bcf4a622115d59d44985e949bee82`  
		Last Modified: Tue, 09 Jun 2020 01:13:51 GMT  
		Size: 19.3 MB (19304370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0744b2f0bcb57875b07f1fa0fbcdfc6428593f823a41eb4698aab5b67ca5506f`  
		Last Modified: Tue, 09 Jun 2020 05:02:26 GMT  
		Size: 244.6 KB (244584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974d12d4793bb92f0ca8b3600115464d11bc0068af45f530f20adc882117d7bf`  
		Last Modified: Tue, 09 Jun 2020 05:02:36 GMT  
		Size: 24.5 MB (24498272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ec9f63e6708b28c4d538b45025dfbd0a318ab06d761ded9d48f44442c898a7`  
		Last Modified: Tue, 09 Jun 2020 05:04:00 GMT  
		Size: 128.6 MB (128554596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:68d1db7da63e2106ddea8d7850cf3badfaa16a94d8d23a12910f86785e4decc8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.6 MB (194642181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf6ff587bef5367449ceee09405f75d3b5a38e19c0d360ec43da1874b37497aa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:49 GMT
ADD file:c85d28567b6123deb660b71c8b60d92378b5ba15ba5dcf495d9388817dc3aa44 in / 
# Tue, 09 Jun 2020 01:54:52 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 03:24:02 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 03:24:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 03:25:06 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 03:30:31 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:622dc742b82743ebf5607b215a65869096390ee41b0a61b5532f859fb94590b1`  
		Last Modified: Tue, 09 Jun 2020 02:00:28 GMT  
		Size: 20.4 MB (20375150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334cf34398cfa7031d68bad42f6b2a8d870a4ad5c2b0454f3f6fdd0fb4433237`  
		Last Modified: Tue, 09 Jun 2020 03:37:02 GMT  
		Size: 244.4 KB (244374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa8cbd821b66a8c4a38ce3d6711cc1ee5489b04a017ab6a7fd368f08beec89e`  
		Last Modified: Tue, 09 Jun 2020 03:37:10 GMT  
		Size: 29.3 MB (29310269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f78bf65ea03cc9db2213ce7ff8e07d3a77604a43ef0a7d81b88b5c965515dfe`  
		Last Modified: Tue, 09 Jun 2020 03:38:38 GMT  
		Size: 144.7 MB (144712388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; 386

```console
$ docker pull mono@sha256:443376dd685b5fcd1e0b6b7a685c5b6a24a79fad8b9619e983293b70e84c8bb6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.4 MB (243401430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6948fdbf966360cb7a728eae30756da2daa5cc4b0362dd09e3a352f4ee44e5dc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:42:33 GMT
ADD file:8ef252685ffefc58654053bf145c830928a2cf423a6c757180649df772f1523d in / 
# Tue, 09 Jun 2020 01:42:34 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 06:59:35 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 06:59:46 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 07:00:24 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 07:05:03 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4ffbd6ec7974e514763a8d7d9fcf5e86e9440e2280e6e9561ea373b4bc50588e`  
		Last Modified: Tue, 09 Jun 2020 01:48:28 GMT  
		Size: 23.1 MB (23147892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b3a90700548ab3df378beb07af7fba67e7ea89ead888d8c78d529c40633c7ed`  
		Last Modified: Tue, 09 Jun 2020 07:10:23 GMT  
		Size: 244.5 KB (244462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbcec5e4a352eead9b06946ed8fb1855a57123b280b3941614dac805987d5b65`  
		Last Modified: Tue, 09 Jun 2020 07:10:41 GMT  
		Size: 68.5 MB (68517280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8167823b3a297ca26719112fd4ae0b1b90e5df5ef7edf3302022c64061697f`  
		Last Modified: Tue, 09 Jun 2020 07:12:09 GMT  
		Size: 151.5 MB (151491796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; ppc64le

```console
$ docker pull mono@sha256:70c1fcea14ad2b7622978d2eb2d5626f8d5363e014b6f4974af4a4d5c15f7fac
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.9 MB (178895806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86adafe85745a7a969d3013f3ec3d1d66c603a377e21e1973c2c1eea147f78da`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:25:38 GMT
ADD file:41ec53d65aa183c2835f73989c9e4922f818e59774811eaa6e7395e5a36d5eab in / 
# Tue, 09 Jun 2020 01:25:42 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:37:42 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 04:39:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:40:39 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 09 Jun 2020 04:51:22 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a29e28607c9b96acae7ff89e56214e4339a87c59e40a6f030fa4cbcaab753f2c`  
		Last Modified: Tue, 09 Jun 2020 01:37:25 GMT  
		Size: 22.8 MB (22791269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1fc192a4485fb46ca92b8e704feb4d02fab0a2a37cb4238017caf8d50239d5`  
		Last Modified: Tue, 09 Jun 2020 05:05:25 GMT  
		Size: 244.7 KB (244663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc43661bb843c17c3ae2b4bc4f6d7ffbc36d936efa982c85608c72360c89b849`  
		Last Modified: Tue, 09 Jun 2020 05:05:31 GMT  
		Size: 25.7 MB (25670188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:942f4a6a782ccadbdc03b5cda25e2632ae9bf2dbd213b5dfee3b75376ad65086`  
		Last Modified: Tue, 09 Jun 2020 05:06:55 GMT  
		Size: 130.2 MB (130189686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mono:slim`

```console
$ docker pull mono@sha256:b575faa4607afa6dbdbafeecf0142953a6e125b1fed1e82e7928327f4ceb628e
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
$ docker pull mono@sha256:71b58b88ce426661d7e4d0741c99c0f0696f727104b1526868dabb58746ea880
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.3 MB (87349111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f20894fd43d160c828a47baf344a1a7bb2b70fcc3ffa98531b571c5043af2910`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 19:31:02 GMT
ENV MONO_VERSION=6.8.0.96
# Fri, 15 May 2020 19:31:11 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 15 May 2020 19:31:50 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79aabb192e71d4e3020dd335c1061c5e9f915b73f367e8aeedf757b6adbc9c4`  
		Last Modified: Fri, 15 May 2020 20:05:47 GMT  
		Size: 244.5 KB (244497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96073affb70fefc051a7bb5f06242765faddc3114c900ccc1af9108910e6517`  
		Last Modified: Fri, 15 May 2020 20:06:04 GMT  
		Size: 64.6 MB (64584727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:de05d2ff43714ddd9e033377d758bc9464db4e95fa409e8f1c0fdf6c679bc827
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46695519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7a5341e68dbc97765d2a7b2eb4ddba90915fe57a702fadac48b4823463a7934`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 00:55:49 GMT
ADD file:af949d376cc9a2ac87d0052d22fe17be59dfe65905f0645d1a903b359208d26d in / 
# Tue, 09 Jun 2020 00:55:51 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:34:30 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 02:35:00 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 02:35:52 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c9b35828d9245f0a85299b96b2d9b0d70390689cf7df0fe7ef29ca6028c0ab56`  
		Last Modified: Tue, 09 Jun 2020 01:03:09 GMT  
		Size: 21.2 MB (21197337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f2cf80f102f97dd711f97ed7ed659bbb653084b0446bec40197f89e4f2be8b`  
		Last Modified: Tue, 09 Jun 2020 02:49:21 GMT  
		Size: 244.6 KB (244566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4085e4a710b2483a23b0768a54b10e50906e0fcc4f4b76b767b7a24e17ffd4d2`  
		Last Modified: Tue, 09 Jun 2020 02:49:31 GMT  
		Size: 25.3 MB (25253616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:87f0fbcfcbfcb2ab20602ca0819f0e1020cd9bd7176594b72d9c88c2304c7272
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (44047226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e75eb00ebe1466aff449d4a9b760038e7c9839a04d1b9cc68da510a74af6233e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:06:35 GMT
ADD file:4a0a863669948b35130fcf8cdb52999c49f7b3ee0620a1eef5f1a2e850a42f05 in / 
# Tue, 09 Jun 2020 01:06:37 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:50:02 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 04:50:28 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:51:11 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c439312a9c212b64af3c38cb326bb5fbe14bcf4a622115d59d44985e949bee82`  
		Last Modified: Tue, 09 Jun 2020 01:13:51 GMT  
		Size: 19.3 MB (19304370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0744b2f0bcb57875b07f1fa0fbcdfc6428593f823a41eb4698aab5b67ca5506f`  
		Last Modified: Tue, 09 Jun 2020 05:02:26 GMT  
		Size: 244.6 KB (244584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974d12d4793bb92f0ca8b3600115464d11bc0068af45f530f20adc882117d7bf`  
		Last Modified: Tue, 09 Jun 2020 05:02:36 GMT  
		Size: 24.5 MB (24498272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:24d8471bd7e59cc38ba65db018794a92fc6d54960784f86d52c913e4a8f5c9a9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 MB (49929793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb86494c128abaa467fc19a192852bfde9ae94e0d13aa1f9f1b70d9adb68697d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:54:49 GMT
ADD file:c85d28567b6123deb660b71c8b60d92378b5ba15ba5dcf495d9388817dc3aa44 in / 
# Tue, 09 Jun 2020 01:54:52 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 03:24:02 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 03:24:21 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 03:25:06 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:622dc742b82743ebf5607b215a65869096390ee41b0a61b5532f859fb94590b1`  
		Last Modified: Tue, 09 Jun 2020 02:00:28 GMT  
		Size: 20.4 MB (20375150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334cf34398cfa7031d68bad42f6b2a8d870a4ad5c2b0454f3f6fdd0fb4433237`  
		Last Modified: Tue, 09 Jun 2020 03:37:02 GMT  
		Size: 244.4 KB (244374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa8cbd821b66a8c4a38ce3d6711cc1ee5489b04a017ab6a7fd368f08beec89e`  
		Last Modified: Tue, 09 Jun 2020 03:37:10 GMT  
		Size: 29.3 MB (29310269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; 386

```console
$ docker pull mono@sha256:e78d5446f93beef2216681d481890fe6388d64c704eb5cd4cc2e7010748818bd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.9 MB (91909634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ebdb565c91f1fbc53a06cbfb5b9c374ab82f491c6934131ce4f1ae6524b43cf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:42:33 GMT
ADD file:8ef252685ffefc58654053bf145c830928a2cf423a6c757180649df772f1523d in / 
# Tue, 09 Jun 2020 01:42:34 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 06:59:35 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 06:59:46 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 07:00:24 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4ffbd6ec7974e514763a8d7d9fcf5e86e9440e2280e6e9561ea373b4bc50588e`  
		Last Modified: Tue, 09 Jun 2020 01:48:28 GMT  
		Size: 23.1 MB (23147892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b3a90700548ab3df378beb07af7fba67e7ea89ead888d8c78d529c40633c7ed`  
		Last Modified: Tue, 09 Jun 2020 07:10:23 GMT  
		Size: 244.5 KB (244462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbcec5e4a352eead9b06946ed8fb1855a57123b280b3941614dac805987d5b65`  
		Last Modified: Tue, 09 Jun 2020 07:10:41 GMT  
		Size: 68.5 MB (68517280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; ppc64le

```console
$ docker pull mono@sha256:2c4949379a4b86afc1273f4a7339ff7bc658bc7749205fb8df632bfb7a7f1d63
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48706120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17986d4009e9231ade165cd631103027df60340b2b4b6fa078cdb34805a602ba`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:25:38 GMT
ADD file:41ec53d65aa183c2835f73989c9e4922f818e59774811eaa6e7395e5a36d5eab in / 
# Tue, 09 Jun 2020 01:25:42 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:37:42 GMT
ENV MONO_VERSION=6.8.0.96
# Tue, 09 Jun 2020 04:39:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 04:40:39 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-vs.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a29e28607c9b96acae7ff89e56214e4339a87c59e40a6f030fa4cbcaab753f2c`  
		Last Modified: Tue, 09 Jun 2020 01:37:25 GMT  
		Size: 22.8 MB (22791269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1fc192a4485fb46ca92b8e704feb4d02fab0a2a37cb4238017caf8d50239d5`  
		Last Modified: Tue, 09 Jun 2020 05:05:25 GMT  
		Size: 244.7 KB (244663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc43661bb843c17c3ae2b4bc4f6d7ffbc36d936efa982c85608c72360c89b849`  
		Last Modified: Tue, 09 Jun 2020 05:05:31 GMT  
		Size: 25.7 MB (25670188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
