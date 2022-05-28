## `mono:6-slim`

```console
$ docker pull mono@sha256:5c87be81163e8e463ad72356d2bec0e4470fa7e06c89fedece68cbe3ab4fbe89
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
$ docker pull mono@sha256:263f35d48a6ff831025751ba8ad63db763b36018298ea61da11cb5ee0917733c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94677584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c30460dc1d16c412692fc59135f88b3ced725caf8d8f5f3ee83a8e34e3706bc9`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:20:43 GMT
ADD file:0513eda9512e010cb9459591b62e0c9d9319750923df091b64250ad6e98c2878 in / 
# Sat, 28 May 2022 01:20:43 GMT
CMD ["bash"]
# Sat, 28 May 2022 11:35:02 GMT
ENV MONO_VERSION=6.12.0.122
# Sat, 28 May 2022 11:35:10 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 May 2022 11:35:38 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:c1ad9731b2c7bf7fddea67f2f3f553515179a375c489e591e2372700fcaca766`  
		Last Modified: Sat, 28 May 2022 01:26:05 GMT  
		Size: 27.1 MB (27140144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d83e829864ffe1d3e8e8013e50d81c17226075b248525f29649c9972933b833e`  
		Last Modified: Sat, 28 May 2022 11:47:12 GMT  
		Size: 2.8 MB (2777562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4869636bcfc5c8d20940c1500acc491e8eb70ca73d6be03efccf597b60782f`  
		Last Modified: Sat, 28 May 2022 11:47:21 GMT  
		Size: 64.8 MB (64759878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:3266405269ac8f4ba4c6e1d19ecb45b7537bf20bacd1354b924aa4a03cc981b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51851134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3135a6ee2a5a1910138836cd5699964c3edd2692087e0890da4d481016571ab7`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 02:04:06 GMT
ADD file:26e9ed6c41ec12bf5fd602b7f86b924d34537bbc82442f630763f9f6c48bf3b3 in / 
# Sat, 28 May 2022 02:04:07 GMT
CMD ["bash"]
# Sat, 28 May 2022 04:01:37 GMT
ENV MONO_VERSION=6.12.0.122
# Sat, 28 May 2022 04:02:05 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 May 2022 04:02:54 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:19389fd1100abdedaa775b43242838cdd2d5c8c3388643a7e52da2b7b4399c15`  
		Last Modified: Sat, 28 May 2022 02:20:06 GMT  
		Size: 24.9 MB (24890069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f3c375660319e072421a4f56d7cfb824f2c73a0fbbda346398732732f72ce2`  
		Last Modified: Sat, 28 May 2022 04:12:53 GMT  
		Size: 2.5 MB (2467796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e598b5fa648877f191c78e4de71a54989855bf4cb077b04d0120de7936dff0e4`  
		Last Modified: Sat, 28 May 2022 04:13:10 GMT  
		Size: 24.5 MB (24493269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:fa0eb567a6cd201cab00f51c108cb1f2e995dcc8d789d03a9eb6d9814f05bf19
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48897665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bbf95a0a01172b3f5121a94b07937dc8173c900de9ff9df56636e9abf1a94eb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:50:13 GMT
ADD file:bccd1898e72cc79621c20ba59061d318521fbd2a8f10806cc3a1561fcbc9daad in / 
# Wed, 11 May 2022 01:50:14 GMT
CMD ["bash"]
# Wed, 11 May 2022 08:17:25 GMT
ENV MONO_VERSION=6.12.0.122
# Wed, 11 May 2022 08:17:50 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Wed, 11 May 2022 08:18:34 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:8f4c08df22a944142862818447616fff8b15d3a7ba383d4eeab678af698c2c43`  
		Last Modified: Wed, 11 May 2022 02:06:00 GMT  
		Size: 22.7 MB (22747864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597a66b2da4420288927cac588b8e2219103ebafaa35704088d77066e24897be`  
		Last Modified: Wed, 11 May 2022 08:28:03 GMT  
		Size: 2.4 MB (2366929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a1059b35d6a81e47da80666397a906d4e2dcb2f8ac60da0ac9aedeeb6a84b2`  
		Last Modified: Wed, 11 May 2022 08:28:20 GMT  
		Size: 23.8 MB (23782872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:feed5590d47253c23bace72f219976d655a21106785a7a097d90ccfa19672c6b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57873710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4464d7e64afef18920e6c2f8be537d8a93ee2ae1437ea00270ae34d6eb8a2b0d`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:41:05 GMT
ADD file:d0e42d603f275c040783ec7b6c051200815492fc35b73110234dfcd584e6cdec in / 
# Sat, 28 May 2022 00:41:05 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:46:00 GMT
ENV MONO_VERSION=6.12.0.122
# Sat, 28 May 2022 02:46:13 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 May 2022 02:46:33 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:4931fb8ba4223cb35034141162105ee5482122692b2931eb69eec912ce64606d`  
		Last Modified: Sat, 28 May 2022 00:48:26 GMT  
		Size: 25.9 MB (25914033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45248ad9aad4be4975eb3bc46f3ce5cb69786d8453b113b5627ee10e93fa80d7`  
		Last Modified: Sat, 28 May 2022 02:50:22 GMT  
		Size: 2.6 MB (2641265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0d42c9e855d1c2134d95bdab130280f5cfeb27d74d53212b6073b6bf54e3c7`  
		Last Modified: Sat, 28 May 2022 02:50:27 GMT  
		Size: 29.3 MB (29318412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; 386

```console
$ docker pull mono@sha256:c38d6790d93dada769f37f48901bb24557510056d681df81819595a144eb3016
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99158365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5d4d1ec3119ba20f8cb575fd277d0fb5b986be067c93fb702e2568d37831295`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:40:01 GMT
ADD file:9aea7a35c215cdd778adec1dd5213973ef9b4830110e4550f2ead85679551ee5 in / 
# Sat, 28 May 2022 00:40:01 GMT
CMD ["bash"]
# Sat, 28 May 2022 03:45:42 GMT
ENV MONO_VERSION=6.12.0.122
# Sat, 28 May 2022 03:45:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 May 2022 03:46:16 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:40837b3d848885c0b0c031d6d950b38e6a26962a5ee49704cb3ca2d2db535617`  
		Last Modified: Sat, 28 May 2022 00:47:36 GMT  
		Size: 27.8 MB (27799572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35de8140668b4241a3e12acfcd19178784d89a55cf9f862e5d9f3f4c5f64f8e1`  
		Last Modified: Sat, 28 May 2022 03:49:52 GMT  
		Size: 2.8 MB (2789357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b94ec9f5bfa3cc0d51596b15c314d897c67c7d3bc34df031386ce7783b7c1fe`  
		Last Modified: Sat, 28 May 2022 03:50:01 GMT  
		Size: 68.6 MB (68569436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:5b9a399daeb519d23f1ccae04c37783cb22c9dc723fa396de1b52e0d1ad8d3e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.3 MB (60326676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f74ca226c5e373ff3236930ad3b22779cef1082df8efab312f1c3d4476f08df`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:23:57 GMT
ADD file:a8c6c897bc64da424049ad04a354d123b0622abda1a56b2725f72de5e4569df8 in / 
# Sat, 28 May 2022 01:24:04 GMT
CMD ["bash"]
# Sat, 28 May 2022 06:58:38 GMT
ENV MONO_VERSION=6.12.0.122
# Sat, 28 May 2022 07:00:20 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr ca-certificates   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 May 2022 07:01:23 GMT
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:087d40850259bdcd3bee3d5d30d5a2070216727f72c1c9731b514ac3dbf7573e`  
		Last Modified: Sat, 28 May 2022 01:33:30 GMT  
		Size: 30.6 MB (30560238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e152c4faa2cb2bf2e15d23a8f5c7c862e9ddecfe4a0e5ac502b9e541865967`  
		Last Modified: Sat, 28 May 2022 07:18:30 GMT  
		Size: 2.9 MB (2892793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34489a9a680aaa76b6e1402289bf21135f719d2d80a90211577e7b2c9462903`  
		Last Modified: Sat, 28 May 2022 07:18:35 GMT  
		Size: 26.9 MB (26873645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
