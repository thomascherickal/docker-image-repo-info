## `mono:latest`

```console
$ docker pull mono@sha256:5efd70a6392a705e644e8e53120a25816778a22a81857a561f191dd06e487249
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
$ docker pull mono@sha256:011bc9105144620819cd18f049f9e1859ea1e4033d3d620e97a52f597f3b3326
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.7 MB (224731353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:528598d6f13a8ff5e2e75af166a5384897688f0ed91952ed68d39a94495094a6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:03:37 GMT
ADD file:6ccb3bbcc69b0d44c48a8ef1bfa08d835444ea13b8a93701bd37d86b81b13ac2 in / 
# Wed, 22 Jul 2020 02:03:37 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 07:15:10 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 23 Jul 2020 07:15:17 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 07:15:46 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 23 Jul 2020 07:29:16 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:6ec8c9369e08152361a01729f2c8a1e7aae898426c6e67267f41894bf9524827`  
		Last Modified: Wed, 22 Jul 2020 02:09:51 GMT  
		Size: 27.1 MB (27098544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e14d8748ae26c65d79706fbdd81cf65f0201253e891019d2b4cba589d2e24e9f`  
		Last Modified: Thu, 23 Jul 2020 07:29:58 GMT  
		Size: 255.9 KB (255898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bce2bffa73ed42f4b5e095c7d5a62681311863af0c9edcbbdf7dfdaec4c0c14`  
		Last Modified: Thu, 23 Jul 2020 07:30:11 GMT  
		Size: 67.1 MB (67086664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa34d97760265bb644bdefc0db468b264d7f47d72c9616077ab06727c375297`  
		Last Modified: Thu, 23 Jul 2020 07:31:09 GMT  
		Size: 130.3 MB (130290247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm variant v5

```console
$ docker pull mono@sha256:abd03a3bce56227091939305195b4388bdac90dee6537d5e76cb90dd900eb440
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180581034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af2284bc85712ff475bc80cf6cbf97a0db00fd1c87d401c3d303cc1d405e7a42`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:13:17 GMT
ADD file:1a4c984d1bdb683e240e8bbdfeae45b146e1f8003444ce04a84096e58a437853 in / 
# Tue, 04 Aug 2020 03:13:27 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 07:34:42 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 04 Aug 2020 07:35:04 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 04 Aug 2020 07:35:52 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 04 Aug 2020 07:41:48 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4eb4ac68461c572fdc826bae247c43484a232f91f165666714ce0f5f052b0bab`  
		Last Modified: Tue, 04 Aug 2020 03:34:09 GMT  
		Size: 24.8 MB (24836059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef442c358905f225964173487185464d18e56eb5bd3c79350910627b668a1fa7`  
		Last Modified: Tue, 04 Aug 2020 07:42:21 GMT  
		Size: 256.0 KB (255997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6e76ab6ff753f0e6c2a8298336ba7e05c6713eda2dd0d539b48131be528d0a`  
		Last Modified: Tue, 04 Aug 2020 07:42:32 GMT  
		Size: 26.5 MB (26530777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f549576139b955fa9f9ba3f969f3118e4554b2ffb3906f27d64b169c0afa4b5a`  
		Last Modified: Tue, 04 Aug 2020 07:44:26 GMT  
		Size: 129.0 MB (128958201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm variant v7

```console
$ docker pull mono@sha256:fe070c3d448b6b57dbcff95f650578974b93d7b3840d8b2d6f640cadf0112c9b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.5 MB (176480036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6306c48d3b57c9c09e107d2183e41347cd99404764d75adcaddb3ce19674dc3f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 01:19:50 GMT
ADD file:c47f7b84c9113624f53d9c52e13f649f1e5d739665b5a5a5df6b1d5b5274d71b in / 
# Wed, 22 Jul 2020 01:19:58 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 07:18:12 GMT
ENV MONO_VERSION=6.10.0.104
# Thu, 23 Jul 2020 07:18:40 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Thu, 23 Jul 2020 07:19:33 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Thu, 23 Jul 2020 07:24:43 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:0c4667eb56da53c2c07c288a210a70fb8d6089f57ce32a2cd88c2a75ae9ad8af`  
		Last Modified: Wed, 22 Jul 2020 01:40:34 GMT  
		Size: 22.7 MB (22705906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ebbb424ecee90e481613bd0a6cb2819d74b90f5fb81c9654915464ef100f8cb`  
		Last Modified: Thu, 23 Jul 2020 07:25:39 GMT  
		Size: 255.9 KB (255927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302255f89a1a2734302115bac08e711d4b8204710f3a23dcf03fa23995eca478`  
		Last Modified: Thu, 23 Jul 2020 07:25:49 GMT  
		Size: 25.7 MB (25729495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5bcdd55231f6ba08fa4118e109a4a525a44238d0f735595e9d60fbea0ad4aea`  
		Last Modified: Thu, 23 Jul 2020 07:27:39 GMT  
		Size: 127.8 MB (127788708 bytes)  
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
$ docker pull mono@sha256:b4c73a49a23f7dd1fa0d9faf0e67556bd5cc65c015555d106d7271029b4b9fab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.5 MB (230534893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cea84fd71596e43d37707e474992dd1420fbe723514f73542b20510fe695b139`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:37:35 GMT
ADD file:cc791c21e6022a12dd1445a35f4cca9392ad8edfe34ea5852f3e87862c943628 in / 
# Tue, 04 Aug 2020 03:37:35 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 06:09:25 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 04 Aug 2020 06:09:33 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 04 Aug 2020 06:10:06 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 04 Aug 2020 06:14:12 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:23ad22c16ab9d635a179d5d341096c34912941507b0c77ac97083b9795d8516f`  
		Last Modified: Tue, 04 Aug 2020 03:42:33 GMT  
		Size: 27.8 MB (27750435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c072f523dda851f155ace5b16dd3bd7af78d63113cd5a9b95305baa69169cb15`  
		Last Modified: Tue, 04 Aug 2020 06:14:57 GMT  
		Size: 255.8 KB (255796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5754f6f3f7020bbac00a743958c7ed3a354f2c674d9763ea0462bac758f96744`  
		Last Modified: Tue, 04 Aug 2020 06:15:14 GMT  
		Size: 71.1 MB (71136222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a4fe81d9b6dc70ff5d8a5eafa467d560c8708d7740e8b6e4f26274d7b425ac`  
		Last Modified: Tue, 04 Aug 2020 06:16:56 GMT  
		Size: 131.4 MB (131392440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; ppc64le

```console
$ docker pull mono@sha256:62912aaadfc996b2e153f528812ceb6a2c074565deb9c97485f51d4d74e40612
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.1 MB (192083470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13ee9bc4061ae057ad9a252dd67dd5a8ce7e58ba14becc7b87dfbb80bf812008`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 04:45:34 GMT
ADD file:3bab6d2b62fe6a548ee28480d9eebf3251e942c4bb66362b87396b73af7aa586 in / 
# Tue, 04 Aug 2020 04:45:40 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 09:29:15 GMT
ENV MONO_VERSION=6.10.0.104
# Tue, 04 Aug 2020 09:30:12 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 04 Aug 2020 09:31:33 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 04 Aug 2020 09:45:39 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:0827434caf9c0b71f95b3bcbe29d60f4f887199db59b3994d9315c478def41c3`  
		Last Modified: Tue, 04 Aug 2020 04:53:24 GMT  
		Size: 30.5 MB (30517844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd17d4162fa0172eeb1ffbb8a68bbbd3e8cd9d7807b60534c8715d78b939a5fd`  
		Last Modified: Tue, 04 Aug 2020 09:46:37 GMT  
		Size: 256.0 KB (256040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d11a57362d5a6f3eed02468a4517dcb2653afa80dfbdff1a90725d784884963`  
		Last Modified: Tue, 04 Aug 2020 09:46:44 GMT  
		Size: 29.3 MB (29349935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0919fec4e424098a16af1cfc29104b97cabaace0158514dd3e83a7d414135fa8`  
		Last Modified: Tue, 04 Aug 2020 09:48:14 GMT  
		Size: 132.0 MB (131959651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
