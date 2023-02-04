## `mono:slim`

```console
$ docker pull mono@sha256:a4e86f2ee3633143211181fa59a271b2de1b1d5c8a5458ddb30d9ca4f7a6685e
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
$ docker pull mono@sha256:4c8cef915fe6f55c9f074a717ab6b4745f41899bc03d18c49fdb544073023c88
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94694961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:517227dd9b43c398e361f8ad9b1d366216daf884dde1cafa071f4b65fe470a80`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 02:35:07 GMT
ADD file:67ceb946e54c26c505b5f9f393d77befbd5e9b3b5c069ca301e314ecc74456b0 in / 
# Wed, 11 Jan 2023 02:35:07 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 06:09:56 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 11 Jan 2023 06:10:06 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 11 Jan 2023 06:10:25 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:548fcab5fe888f589dd092c68b813bfd65359878bd1950d6b753f749e82ebd7c`  
		Last Modified: Wed, 11 Jan 2023 02:39:48 GMT  
		Size: 27.1 MB (27140352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c6b69a68130572161adf6789b703ac3278e118a380dcf9ef8c203efeb25d9e`  
		Last Modified: Wed, 11 Jan 2023 06:17:23 GMT  
		Size: 2.8 MB (2780379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69fe30b35d072335f48655a8764fc1efab5a7a1b15dd94ca7035b1a111d2bed5`  
		Last Modified: Wed, 11 Jan 2023 06:17:33 GMT  
		Size: 64.8 MB (64774230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:b45a5c3c13c4ed011186f4fe6e303db87e50f32e4ebbf90e02770189f508a89c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51860916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c92eb12b3e9f714a8f414cc71ec8ba5e4d448062a4e87a9cf6cd9886e6310530`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:49:37 GMT
ADD file:2ed7ca0d45c68b46a10ae186e8a03f98e72cadfeed17105668f53adf14d31e1f in / 
# Tue, 02 Aug 2022 00:49:38 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 03:10:22 GMT
ENV MONO_VERSION=6.12.0.182
# Tue, 06 Dec 2022 03:10:42 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 06 Dec 2022 03:11:08 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:187ecffbd1e0eae5de6567dff32bd58f28623635657779760c9d9539d6b7cc59`  
		Last Modified: Tue, 02 Aug 2022 00:57:06 GMT  
		Size: 24.9 MB (24889750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec08a53adab961841355c601fac2e1dc82cb2cc08b15bc1e0620e069c77f663`  
		Last Modified: Tue, 06 Dec 2022 03:16:27 GMT  
		Size: 2.5 MB (2467714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f721b36a800f3865e15022a1770168f7e1fb1b6615669eb6bd76251d52b525bb`  
		Last Modified: Tue, 06 Dec 2022 03:16:32 GMT  
		Size: 24.5 MB (24503452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:9a76268bff7a9c70d005cc1c4b2fd1d9ae4ca7ffbd85a5627a1863d55f4aa081
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48909012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e92560eb616c4c6928bf34872454be45839f741e9258ce6f42e7fdb562501d46`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 04:01:11 GMT
ADD file:360ea34974de7bba698a1a4e78149a2da671264dbf02678aef09bcd3f592c229 in / 
# Wed, 11 Jan 2023 04:01:12 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 07:03:24 GMT
ENV MONO_VERSION=6.12.0.182
# Wed, 11 Jan 2023 07:03:34 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 11 Jan 2023 07:03:52 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:75680cfdd833613d913b856d8c584fa88c596b93732050a582a5fe937df3a9e6`  
		Last Modified: Wed, 11 Jan 2023 04:08:41 GMT  
		Size: 22.7 MB (22748873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c52aa904cb2435d516c0ee4898417ad1d6c34cbbb2f50d81e1377c56a24cf1`  
		Last Modified: Wed, 11 Jan 2023 07:08:16 GMT  
		Size: 2.4 MB (2369697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ebd9066e084b64c33f1cd729ed9788ee07f089b473191456afe96e8281ecb7`  
		Last Modified: Wed, 11 Jan 2023 07:08:21 GMT  
		Size: 23.8 MB (23790442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:125e2d0c336ad320b478be88e7ae1dd56e3673489039f3f98da5a01cc6a304f3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.1 MB (58112827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:959883c3c167cc3ffcba665d5c477214242dee8c59a14f6e64e585a8c63d93c8`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:54 GMT
ADD file:cf6ecb1d6b034b0d4fc309542cb25fff0c997661b323f524ecc258ac323e43f6 in / 
# Sat, 04 Feb 2023 06:17:55 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:39:17 GMT
ENV MONO_VERSION=6.12.0.182
# Sat, 04 Feb 2023 08:39:24 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 04 Feb 2023 08:39:37 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:bd2853c1424a5596deda2f31e1f82920613a03c667c3ff58cb461340b7bb89cd`  
		Last Modified: Sat, 04 Feb 2023 06:22:04 GMT  
		Size: 25.9 MB (25922631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db163c8bce6f5740cbc4098d22ca7d2daf60f00794941e2aed44fa2abd4393f4`  
		Last Modified: Sat, 04 Feb 2023 08:43:04 GMT  
		Size: 2.6 MB (2645286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4fca2eba28651df8a1a6c055fb80117e3b5817641b7a4fb99e21b3ff23fb010`  
		Last Modified: Sat, 04 Feb 2023 08:43:08 GMT  
		Size: 29.5 MB (29544910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; 386

```console
$ docker pull mono@sha256:ccaa52ad6a519ada89660b7354d37cb562bc6016eb591c95dc860ad4a7b235c3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99176249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73513384a82d82c594129342d1f31312f764ba673347e264339e39b8a569180b`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 07:49:48 GMT
ADD file:060bbacc8df3d1b157ff409535b3ea29dd0b5667425e3dcf6e60556dcfa4e7f1 in / 
# Sat, 04 Feb 2023 07:49:48 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 10:10:43 GMT
ENV MONO_VERSION=6.12.0.182
# Sat, 04 Feb 2023 10:10:52 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 04 Feb 2023 10:11:14 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8e0d975bedf8c90406704c677df48435cd2d53449ac9ab15a876323ceb95ff8f`  
		Last Modified: Sat, 04 Feb 2023 07:55:52 GMT  
		Size: 27.8 MB (27798503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac5477e412c01e73ade39b033ad7bf7b8b0bde4bcbb6dbad5035e97cfe18da9`  
		Last Modified: Sat, 04 Feb 2023 10:14:45 GMT  
		Size: 2.8 MB (2791534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1ad438cd298ae0ce4c329beca0d038388f03a038a1accc54c4ea080f834fe4`  
		Last Modified: Sat, 04 Feb 2023 10:14:54 GMT  
		Size: 68.6 MB (68586212 bytes)  
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
