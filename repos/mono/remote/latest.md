## `mono:latest`

```console
$ docker pull mono@sha256:c8585cd71a14f778e340143ef2d7550ac1ff148c79da37ef95c5955cf80881d4
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
$ docker pull mono@sha256:af72ed05e0ac706c53968ff8674d30bb94f551cf19a5daf0bb556a53e380f54d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.0 MB (235971671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6eae37be12fa01142c2e26df198d0506b43f0a477f0b7be827ea4d2f1a0c5034`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 11:11:50 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 17 Aug 2021 11:12:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 17 Aug 2021 11:12:45 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 17 Aug 2021 11:20:19 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a18edb497dc51f816f20de5aa698599b30084cfd1240770f6986788b7e1deba`  
		Last Modified: Tue, 17 Aug 2021 11:27:05 GMT  
		Size: 256.1 KB (256074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d26b2b043ba0f428a2732ac83728a54615be9b4e2ed8e8935c67bf4320b9c2`  
		Last Modified: Tue, 17 Aug 2021 11:27:18 GMT  
		Size: 67.1 MB (67128207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a5f3f23f3647cc1c1818fd41790be554595127babc0cf697e6913c1b907a92`  
		Last Modified: Tue, 17 Aug 2021 11:28:37 GMT  
		Size: 141.4 MB (141441405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm variant v5

```console
$ docker pull mono@sha256:eb7b5bbaae6db94ff8d2a676c5b68723d8fe7678dc68e479d2457b1becff7a84
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.8 MB (191787440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f75e29edb7b289c13437230f282ded61a4e72909edc89724517216eb21ed87ce`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:51:26 GMT
ADD file:350748a564076da397b991745cd42e0688d15c72b9fd5c81f8ea0bb8938a2b3d in / 
# Fri, 03 Sep 2021 00:51:27 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 03:04:06 GMT
ENV MONO_VERSION=6.12.0.107
# Fri, 03 Sep 2021 03:04:29 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 03 Sep 2021 03:05:22 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 03 Sep 2021 03:10:14 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:b019db4b5197128481d48d92ecacd6bb356c027a3d08393f6567a6fa183ba769`  
		Last Modified: Fri, 03 Sep 2021 01:07:12 GMT  
		Size: 24.9 MB (24879114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828064d1142810d6abe00b2e08d14bbf4420ee169359b192d08b40d8aae10e5f`  
		Last Modified: Fri, 03 Sep 2021 03:14:59 GMT  
		Size: 256.0 KB (255970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c465dd0ac4c8ce158165e98366d0ba4306a911e1b2d2bd390d257461e51a3c`  
		Last Modified: Fri, 03 Sep 2021 03:15:19 GMT  
		Size: 26.6 MB (26551271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7feb670c33feb82bdc841fe53acd103290ce80a5b567da313dc43bafca9e9dd`  
		Last Modified: Fri, 03 Sep 2021 03:18:02 GMT  
		Size: 140.1 MB (140101085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm variant v7

```console
$ docker pull mono@sha256:d6054367f74ef4d09276fb8dda40aa980c9be29f475394ba7ac06a638b6f4eef
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.7 MB (187689222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cca19ff00a66ab1490a6aaf8f774f86eabc4275931128b19f5c794b04fb23d8f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 02:14:25 GMT
ADD file:ca8cc4b509e305fa07662fbf2234ed78f0056569f6ca047305dc02bcd60f1558 in / 
# Tue, 17 Aug 2021 02:14:26 GMT
CMD ["bash"]
# Wed, 18 Aug 2021 01:59:47 GMT
ENV MONO_VERSION=6.12.0.107
# Wed, 18 Aug 2021 02:00:08 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 18 Aug 2021 02:02:30 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 18 Aug 2021 02:06:58 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:13e3f03410ff211945a725435c13065288d48a8cb740f0530e7588012c2679a4`  
		Last Modified: Tue, 17 Aug 2021 02:30:58 GMT  
		Size: 22.7 MB (22746254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e77c4894d97074306e64eb7149d09e4e3d3325aac2aba5446dc99106833c16`  
		Last Modified: Wed, 18 Aug 2021 02:11:43 GMT  
		Size: 256.0 KB (256037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:640bfafc25108ce735ff4f4df912358dc9b84baf60fd05c9248412058852e9d5`  
		Last Modified: Wed, 18 Aug 2021 02:12:02 GMT  
		Size: 25.7 MB (25737984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3e0cd4e5dcf69b0af43e21e7c1097d99b9930d64e50327dc71f93751eff8f0`  
		Last Modified: Wed, 18 Aug 2021 02:14:31 GMT  
		Size: 138.9 MB (138948947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:f16a392b76f9be0082212541fb960f9516b92cdb858d97d3eecf6a97ac045cb1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.5 MB (214538345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e599256e37fdb6e6bf4b08f4954726cd20e99e4d053b311558a61df54a642135`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:58 GMT
ADD file:4a1d7f2d989aee6bd83da076b6e9dd3da2da97cf5654bd37568e9baec30ac4b1 in / 
# Fri, 03 Sep 2021 00:40:58 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:12:51 GMT
ENV MONO_VERSION=6.12.0.107
# Fri, 03 Sep 2021 01:13:07 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Fri, 03 Sep 2021 01:13:31 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Fri, 03 Sep 2021 01:16:08 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d10c227306ce3db344a8399cbc02bbf0dcb36519318efbde3c6027c00be8b40e`  
		Last Modified: Fri, 03 Sep 2021 00:49:47 GMT  
		Size: 25.9 MB (25914860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30e374ba39adf873bbba8da77f7dc58c7c43b81b4b8e3170dc8901f66cb04d7`  
		Last Modified: Fri, 03 Sep 2021 01:18:52 GMT  
		Size: 255.9 KB (255882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25150f9518e1111254618ae1d69456bf511922e2f0d7e186fb8ee12717e3f30b`  
		Last Modified: Fri, 03 Sep 2021 01:18:58 GMT  
		Size: 31.8 MB (31770057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624df4a01bc0ac2d25f15ef9c373a29a7d68bc294238fd6c33c7e3e50e06024e`  
		Last Modified: Fri, 03 Sep 2021 01:20:06 GMT  
		Size: 156.6 MB (156597546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; 386

```console
$ docker pull mono@sha256:09028cfa432f95f54098aa9d1102f43a0726bc5c851c9a8155b27faaf467d82e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.8 MB (241754130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6afecb4321c7bce4d40e5f56ef638a3636209597a4df0082875067278e6d2974`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:41:16 GMT
ADD file:0418032b55cd0a6dd515ac277fb9f92354397503cab212d446d3a3d8c647a60f in / 
# Tue, 17 Aug 2021 01:41:17 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 12:43:34 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 17 Aug 2021 12:43:45 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 17 Aug 2021 12:44:27 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Tue, 17 Aug 2021 12:46:45 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c1c94e1f2523d69effaa463d64fc9962cfc67e2a956f0476c94200e7cf19edf0`  
		Last Modified: Tue, 17 Aug 2021 01:50:57 GMT  
		Size: 27.8 MB (27797627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d987925313615e02773a946ac9b42951a723a3eb017b11b24a34e521f284c451`  
		Last Modified: Tue, 17 Aug 2021 12:49:07 GMT  
		Size: 255.9 KB (255915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b9127e6bbd6fddf8d5c7ecfb229059a795bb645868b3f3a281db9cc08867d79`  
		Last Modified: Tue, 17 Aug 2021 12:49:28 GMT  
		Size: 71.2 MB (71153146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19dc7ee9b290a2c781180d3ae89398c93cb36fe6dbad95b0b6e4b358b35a619`  
		Last Modified: Tue, 17 Aug 2021 12:51:20 GMT  
		Size: 142.5 MB (142547442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:latest` - linux; ppc64le

```console
$ docker pull mono@sha256:25f162067ea30fd8da0953ba5a31b58d7f03a129642407347de33a1abf0c6c59
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.4 MB (203419471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e745b065195114db1e7e155298e523a4fb8b42f5ec9bbbedc68195c40ea0023`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:34:13 GMT
ADD file:8b9b12a994a2519f725d1ed1f4ab5a444665262678fd8e6c42cf78f32dacb7fa in / 
# Tue, 17 Aug 2021 01:34:20 GMT
CMD ["bash"]
# Wed, 18 Aug 2021 02:04:45 GMT
ENV MONO_VERSION=6.12.0.107
# Wed, 18 Aug 2021 02:06:52 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 18 Aug 2021 02:11:43 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
# Wed, 18 Aug 2021 02:35:12 GMT
RUN apt-get update   && apt-get install -y binutils curl mono-devel ca-certificates-mono fsharp mono-vbnc nuget referenceassemblies-pcl   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c3e09f0e3e7f6fcb741a4c9214b63e341e1d9b53d7689a5ad6ff640b61a82541`  
		Last Modified: Tue, 17 Aug 2021 01:48:22 GMT  
		Size: 30.6 MB (30553721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed938d51ca87d416c43d2d04357f0d1346c8e343194bb33ca657edb0fd0b4c2`  
		Last Modified: Wed, 18 Aug 2021 02:46:40 GMT  
		Size: 256.3 KB (256264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b53e30ca4a1119ce2d014ce5b3e941270cfc0975a53f4312713d175a4b09df6`  
		Last Modified: Wed, 18 Aug 2021 02:46:47 GMT  
		Size: 29.4 MB (29358307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3cb82cd25a8775e5573edf47252ae84b998d672ddb5a148b99c27372cf6a973`  
		Last Modified: Wed, 18 Aug 2021 02:47:56 GMT  
		Size: 143.3 MB (143251179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
