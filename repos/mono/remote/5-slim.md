## `mono:5-slim`

```console
$ docker pull mono@sha256:c94ce708f6486e0a84f12b1e43d1c5784d3661b3748e6f9b1da02834b2f2cd8e
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
$ docker pull mono@sha256:16162056f6d04d68d3b297f123edad3e7bba54f4e0ee84c5cd5012610935b7c9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.2 MB (78171634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd0eab449535c70e3a40b2293d483a0213d2426f5a4a6539ce69688dca0ddee0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:23:35 GMT
ADD file:57b431451a292755d0f13673f5f3bea9f62aea36c7a1b59d34d7d200ba134fea in / 
# Tue, 09 Jun 2020 01:23:35 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 07:25:19 GMT
ENV MONO_VERSION=5.20.1.34
# Tue, 09 Jun 2020 07:25:31 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 09 Jun 2020 07:25:58 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:7d2977b12acb33f192e3f20b7e15a467cc8f3f5124a15d975a6d4afe5fa3d258`  
		Last Modified: Tue, 09 Jun 2020 01:28:13 GMT  
		Size: 22.5 MB (22519600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a96016cede2bbab34292fab9e759f8d6e76cdccf5e984c01f8efd90e6df05b`  
		Last Modified: Tue, 09 Jun 2020 07:58:27 GMT  
		Size: 244.5 KB (244463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a6ab00376aa34c88796f85c2d808035931da42c558e6f9ff32907a9641b062`  
		Last Modified: Tue, 09 Jun 2020 07:58:43 GMT  
		Size: 55.4 MB (55407571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:ec3602c25a4a890750685bb5f19d7a34a20516a37059153579b68a4f74f17f3d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45584292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae3c8177fa72be71e59c5119b36ba1f5f0a9099f41a0d3032bd34b486c34c3f6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:55:12 GMT
ADD file:0b9f2b88887a8060402a052c243c31641d9c217edcdb232c7b7a057cf5a70d66 in / 
# Wed, 22 Jul 2020 00:55:13 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 04:50:57 GMT
ENV MONO_VERSION=5.20.1.34
# Wed, 22 Jul 2020 04:51:29 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 22 Jul 2020 04:52:30 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:319109fcb6fa9b08528c518426e7ce105aac7313066432efcea95f59ff6e6788`  
		Last Modified: Wed, 22 Jul 2020 01:03:27 GMT  
		Size: 21.2 MB (21189131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:214f724afb987f92ce9133d6327bf39c60bb2f5e639abe876e341a07f439d60e`  
		Last Modified: Wed, 22 Jul 2020 05:03:20 GMT  
		Size: 244.6 KB (244590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1738e5f6ebf3cc4543e52c88b7aa0fc6f9113fabde1e2980a289aafa5559d5b1`  
		Last Modified: Wed, 22 Jul 2020 05:03:29 GMT  
		Size: 24.2 MB (24150571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:4386b149b67f32efb634322ead66cbd1af15e940a4fdbed1096cea4a7b5c0e1e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.0 MB (42996393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f18852418937a80e1446631268ee77d13a3bc5e056f76139117a44a72ecdc3ca`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 01:33:30 GMT
ADD file:49b1a1b4f5c2201b0e23e29dca24c4f6ffc14620196c4bd77770952500c4bee1 in / 
# Wed, 22 Jul 2020 01:33:38 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 02:20:07 GMT
ENV MONO_VERSION=5.20.1.34
# Wed, 22 Jul 2020 02:20:49 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 22 Jul 2020 02:21:51 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:cd38ad753522d120e27c5343b08f661ee3aebfe531d60102d7c624c16dba4d09`  
		Last Modified: Wed, 22 Jul 2020 01:44:24 GMT  
		Size: 19.3 MB (19298267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae6961338dbeec44b6e92646723bb59c030769220b24193c12f7827ce9ca826f`  
		Last Modified: Wed, 22 Jul 2020 02:33:13 GMT  
		Size: 244.6 KB (244556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:829fd514f3675f9e41ec1f1bc082852015f100014cc48e3b90e1b3023c34fa51`  
		Last Modified: Wed, 22 Jul 2020 02:33:22 GMT  
		Size: 23.5 MB (23453570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:ef58fa9435a611d288114536f66587b41e43fda40ff6862ef66a710cacd55424
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48664948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2943d658466811aee63cc7bd02a2b7b8262be0b1643e43e2916e569747008123`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:44:08 GMT
ADD file:7a721f0a6a7d3eb45184986201740dc57ec00c3d3da61af70966d87f3675d2ef in / 
# Wed, 22 Jul 2020 00:44:10 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 05:44:23 GMT
ENV MONO_VERSION=5.20.1.34
# Wed, 22 Jul 2020 05:44:54 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 22 Jul 2020 05:45:37 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:3d187d5a7d59d9a1bf03dbd41bc2d56080ed75d089110b59508e3b246ae0e944`  
		Last Modified: Wed, 22 Jul 2020 00:50:16 GMT  
		Size: 20.4 MB (20371158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bbe9b29dfbdf82cc0e7bddeeb0c945769da83cf78b2e7800cb42ae3f6d8412`  
		Last Modified: Wed, 22 Jul 2020 05:55:02 GMT  
		Size: 244.4 KB (244397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8b62047984b5df91705425882147b3c0c745252929b362ec5689395274279e`  
		Last Modified: Wed, 22 Jul 2020 05:55:11 GMT  
		Size: 28.0 MB (28049393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:5-slim` - linux; 386

```console
$ docker pull mono@sha256:af88b48883f3971c9d88b37dd77ed0547ff73057302dcf0bfad4407b5cd9900a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.8 MB (81826014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa6b7f2644af5cdccb423356fed81e05f1b383495699371be1bac62b7f429a4b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:12:37 GMT
ADD file:9d59e7e41b146c16bca3047e3a0451abb508d22a91b64dfe2ce6d147381f800d in / 
# Wed, 22 Jul 2020 02:12:37 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 08:16:17 GMT
ENV MONO_VERSION=5.20.1.34
# Wed, 22 Jul 2020 08:16:30 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 22 Jul 2020 08:17:11 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:5562cfdfc3152571ce0700e9d6816dede132432ab48c7ef147e89863eac98d4d`  
		Last Modified: Wed, 22 Jul 2020 02:19:28 GMT  
		Size: 23.1 MB (23142189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abbc7bc3ccd85914ca218044ef698ec167facb5afca120d59a6f53a795c50a3`  
		Last Modified: Wed, 22 Jul 2020 08:27:29 GMT  
		Size: 244.5 KB (244528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac33c3358ab44f6ead7ae34979c53d5a83b08a9755b0096ac973c6c7696a73fe`  
		Last Modified: Wed, 22 Jul 2020 08:27:55 GMT  
		Size: 58.4 MB (58439297 bytes)  
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
