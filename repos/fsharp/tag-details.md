<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `fsharp`

-	[`fsharp:10`](#fsharp10)
-	[`fsharp:10.7`](#fsharp107)
-	[`fsharp:10.7.0`](#fsharp1070)
-	[`fsharp:10.7.0-netcore`](#fsharp1070-netcore)
-	[`fsharp:10.7-netcore`](#fsharp107-netcore)
-	[`fsharp:10-netcore`](#fsharp10-netcore)
-	[`fsharp:4`](#fsharp4)
-	[`fsharp:4.1`](#fsharp41)
-	[`fsharp:4.1.34`](#fsharp4134)
-	[`fsharp:latest`](#fsharplatest)
-	[`fsharp:netcore`](#fsharpnetcore)

## `fsharp:10`

```console
$ docker pull fsharp@sha256:d74735abb48ce5e5830569b3cc12fe2b8a0e40a8c02b5c48b2db0ced6faec0aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `fsharp:10` - linux; amd64

```console
$ docker pull fsharp@sha256:76053ebd0f47351e7d2fd8647da6fb4f704c9b4f1d90cd1d76de4e6a2501d902
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.6 MB (186618716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07f1afa4082ad795eab7950031c098175b84369e3242e8ae984126f4e3acc441`
-	Default Command: `["fsharpi"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 18:16:03 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Fri, 15 May 2020 18:16:03 GMT
ENV MONO_THREADS_PER_CPU=50
# Fri, 15 May 2020 18:25:33 GMT
RUN MONO_VERSION=6.8.0.105 &&     FSHARP_VERSION=10.2.3 &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     apt-get update && apt-get --no-install-recommends install -y gnupg dirmngr ca-certificates apt-transport-https &&     apt-key adv --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" | tee /etc/apt/sources.list.d/mono-official-stable.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y pkg-config make nuget mono-devel msbuild ca-certificates-mono locales &&     rm -rf /var/lib/apt/lists/* &&     echo 'en_US.UTF-8 UTF-8' > /etc/locale.gen && /usr/sbin/locale-gen &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local "$GNUPGHOME" &&     apt-get purge -y make gnupg dirmngr &&     apt-get clean
# Fri, 15 May 2020 18:25:33 GMT
WORKDIR /root
# Fri, 15 May 2020 18:25:33 GMT
CMD ["fsharpi"]
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74fe1ed6bb8e743af51a92cb071b53473eb49ba5abc8b134ee57da16c97a8c3e`  
		Last Modified: Fri, 15 May 2020 18:43:24 GMT  
		Size: 159.5 MB (159519960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fsharp:10` - linux; arm64 variant v8

```console
$ docker pull fsharp@sha256:703500113022afbd42119ea3e95d85404c2e61a3872cc43851f6ff872ffb1835
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.6 MB (183637080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc2dd8a49dfc0d4b3f98f61c4c3cf7d37d97e65433fb28c53e45cf5272e02f1c`
-	Default Command: `["fsharpi"]`

```dockerfile
# Wed, 13 May 2020 21:43:44 GMT
ADD file:37b141a882e9c33a09f7554ab39e3ba9c7f2b12e916c721436bd85817951eb4c in / 
# Wed, 13 May 2020 21:43:47 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:52:12 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Thu, 14 May 2020 00:52:13 GMT
ENV MONO_THREADS_PER_CPU=50
# Thu, 14 May 2020 01:10:21 GMT
RUN MONO_VERSION=6.8.0.105 &&     FSHARP_VERSION=10.2.3 &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     apt-get update && apt-get --no-install-recommends install -y gnupg dirmngr ca-certificates apt-transport-https &&     apt-key adv --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" | tee /etc/apt/sources.list.d/mono-official-stable.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y pkg-config make nuget mono-devel msbuild ca-certificates-mono locales &&     rm -rf /var/lib/apt/lists/* &&     echo 'en_US.UTF-8 UTF-8' > /etc/locale.gen && /usr/sbin/locale-gen &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local "$GNUPGHOME" &&     apt-get purge -y make gnupg dirmngr &&     apt-get clean
# Thu, 14 May 2020 01:10:36 GMT
WORKDIR /root
# Thu, 14 May 2020 01:10:38 GMT
CMD ["fsharpi"]
```

-	Layers:
	-	`sha256:b24dc5b5f4f0ffe0f8a33241aa35f3d74ee4213bc2b87eb3ec4b72a6e70ba7bc`  
		Last Modified: Wed, 13 May 2020 21:53:15 GMT  
		Size: 25.9 MB (25851785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4c3526a3ff4107662914bbca00c466fa6c0bd17772c578e1b14e0a456da8710`  
		Last Modified: Thu, 14 May 2020 01:11:52 GMT  
		Size: 157.8 MB (157785295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fsharp:10.7`

```console
$ docker pull fsharp@sha256:d74735abb48ce5e5830569b3cc12fe2b8a0e40a8c02b5c48b2db0ced6faec0aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `fsharp:10.7` - linux; amd64

```console
$ docker pull fsharp@sha256:76053ebd0f47351e7d2fd8647da6fb4f704c9b4f1d90cd1d76de4e6a2501d902
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.6 MB (186618716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07f1afa4082ad795eab7950031c098175b84369e3242e8ae984126f4e3acc441`
-	Default Command: `["fsharpi"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 18:16:03 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Fri, 15 May 2020 18:16:03 GMT
ENV MONO_THREADS_PER_CPU=50
# Fri, 15 May 2020 18:25:33 GMT
RUN MONO_VERSION=6.8.0.105 &&     FSHARP_VERSION=10.2.3 &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     apt-get update && apt-get --no-install-recommends install -y gnupg dirmngr ca-certificates apt-transport-https &&     apt-key adv --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" | tee /etc/apt/sources.list.d/mono-official-stable.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y pkg-config make nuget mono-devel msbuild ca-certificates-mono locales &&     rm -rf /var/lib/apt/lists/* &&     echo 'en_US.UTF-8 UTF-8' > /etc/locale.gen && /usr/sbin/locale-gen &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local "$GNUPGHOME" &&     apt-get purge -y make gnupg dirmngr &&     apt-get clean
# Fri, 15 May 2020 18:25:33 GMT
WORKDIR /root
# Fri, 15 May 2020 18:25:33 GMT
CMD ["fsharpi"]
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74fe1ed6bb8e743af51a92cb071b53473eb49ba5abc8b134ee57da16c97a8c3e`  
		Last Modified: Fri, 15 May 2020 18:43:24 GMT  
		Size: 159.5 MB (159519960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fsharp:10.7` - linux; arm64 variant v8

```console
$ docker pull fsharp@sha256:703500113022afbd42119ea3e95d85404c2e61a3872cc43851f6ff872ffb1835
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.6 MB (183637080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc2dd8a49dfc0d4b3f98f61c4c3cf7d37d97e65433fb28c53e45cf5272e02f1c`
-	Default Command: `["fsharpi"]`

```dockerfile
# Wed, 13 May 2020 21:43:44 GMT
ADD file:37b141a882e9c33a09f7554ab39e3ba9c7f2b12e916c721436bd85817951eb4c in / 
# Wed, 13 May 2020 21:43:47 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:52:12 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Thu, 14 May 2020 00:52:13 GMT
ENV MONO_THREADS_PER_CPU=50
# Thu, 14 May 2020 01:10:21 GMT
RUN MONO_VERSION=6.8.0.105 &&     FSHARP_VERSION=10.2.3 &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     apt-get update && apt-get --no-install-recommends install -y gnupg dirmngr ca-certificates apt-transport-https &&     apt-key adv --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" | tee /etc/apt/sources.list.d/mono-official-stable.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y pkg-config make nuget mono-devel msbuild ca-certificates-mono locales &&     rm -rf /var/lib/apt/lists/* &&     echo 'en_US.UTF-8 UTF-8' > /etc/locale.gen && /usr/sbin/locale-gen &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local "$GNUPGHOME" &&     apt-get purge -y make gnupg dirmngr &&     apt-get clean
# Thu, 14 May 2020 01:10:36 GMT
WORKDIR /root
# Thu, 14 May 2020 01:10:38 GMT
CMD ["fsharpi"]
```

-	Layers:
	-	`sha256:b24dc5b5f4f0ffe0f8a33241aa35f3d74ee4213bc2b87eb3ec4b72a6e70ba7bc`  
		Last Modified: Wed, 13 May 2020 21:53:15 GMT  
		Size: 25.9 MB (25851785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4c3526a3ff4107662914bbca00c466fa6c0bd17772c578e1b14e0a456da8710`  
		Last Modified: Thu, 14 May 2020 01:11:52 GMT  
		Size: 157.8 MB (157785295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fsharp:10.7.0`

```console
$ docker pull fsharp@sha256:d74735abb48ce5e5830569b3cc12fe2b8a0e40a8c02b5c48b2db0ced6faec0aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `fsharp:10.7.0` - linux; amd64

```console
$ docker pull fsharp@sha256:76053ebd0f47351e7d2fd8647da6fb4f704c9b4f1d90cd1d76de4e6a2501d902
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.6 MB (186618716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07f1afa4082ad795eab7950031c098175b84369e3242e8ae984126f4e3acc441`
-	Default Command: `["fsharpi"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 18:16:03 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Fri, 15 May 2020 18:16:03 GMT
ENV MONO_THREADS_PER_CPU=50
# Fri, 15 May 2020 18:25:33 GMT
RUN MONO_VERSION=6.8.0.105 &&     FSHARP_VERSION=10.2.3 &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     apt-get update && apt-get --no-install-recommends install -y gnupg dirmngr ca-certificates apt-transport-https &&     apt-key adv --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" | tee /etc/apt/sources.list.d/mono-official-stable.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y pkg-config make nuget mono-devel msbuild ca-certificates-mono locales &&     rm -rf /var/lib/apt/lists/* &&     echo 'en_US.UTF-8 UTF-8' > /etc/locale.gen && /usr/sbin/locale-gen &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local "$GNUPGHOME" &&     apt-get purge -y make gnupg dirmngr &&     apt-get clean
# Fri, 15 May 2020 18:25:33 GMT
WORKDIR /root
# Fri, 15 May 2020 18:25:33 GMT
CMD ["fsharpi"]
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74fe1ed6bb8e743af51a92cb071b53473eb49ba5abc8b134ee57da16c97a8c3e`  
		Last Modified: Fri, 15 May 2020 18:43:24 GMT  
		Size: 159.5 MB (159519960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fsharp:10.7.0` - linux; arm64 variant v8

```console
$ docker pull fsharp@sha256:703500113022afbd42119ea3e95d85404c2e61a3872cc43851f6ff872ffb1835
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.6 MB (183637080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc2dd8a49dfc0d4b3f98f61c4c3cf7d37d97e65433fb28c53e45cf5272e02f1c`
-	Default Command: `["fsharpi"]`

```dockerfile
# Wed, 13 May 2020 21:43:44 GMT
ADD file:37b141a882e9c33a09f7554ab39e3ba9c7f2b12e916c721436bd85817951eb4c in / 
# Wed, 13 May 2020 21:43:47 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:52:12 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Thu, 14 May 2020 00:52:13 GMT
ENV MONO_THREADS_PER_CPU=50
# Thu, 14 May 2020 01:10:21 GMT
RUN MONO_VERSION=6.8.0.105 &&     FSHARP_VERSION=10.2.3 &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     apt-get update && apt-get --no-install-recommends install -y gnupg dirmngr ca-certificates apt-transport-https &&     apt-key adv --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" | tee /etc/apt/sources.list.d/mono-official-stable.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y pkg-config make nuget mono-devel msbuild ca-certificates-mono locales &&     rm -rf /var/lib/apt/lists/* &&     echo 'en_US.UTF-8 UTF-8' > /etc/locale.gen && /usr/sbin/locale-gen &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local "$GNUPGHOME" &&     apt-get purge -y make gnupg dirmngr &&     apt-get clean
# Thu, 14 May 2020 01:10:36 GMT
WORKDIR /root
# Thu, 14 May 2020 01:10:38 GMT
CMD ["fsharpi"]
```

-	Layers:
	-	`sha256:b24dc5b5f4f0ffe0f8a33241aa35f3d74ee4213bc2b87eb3ec4b72a6e70ba7bc`  
		Last Modified: Wed, 13 May 2020 21:53:15 GMT  
		Size: 25.9 MB (25851785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4c3526a3ff4107662914bbca00c466fa6c0bd17772c578e1b14e0a456da8710`  
		Last Modified: Thu, 14 May 2020 01:11:52 GMT  
		Size: 157.8 MB (157785295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fsharp:10.7.0-netcore`

```console
$ docker pull fsharp@sha256:fac2fb64dd348a9b553d9744f37e5cbdc815a71308c7c5424df69fa7f3c3dc37
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `fsharp:10.7.0-netcore` - linux; amd64

```console
$ docker pull fsharp@sha256:6e1a36d58bf3ae7d6290967c2dd89521ec5b96ee2bfa69effbc38f1f35c53552
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.7 MB (323681588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b58060dddba748160f27e9036737add43a27c5c5418917972e799c9a591627cb`
-	Default Command: `["dotnet","fsi"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 18:16:03 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Fri, 15 May 2020 18:16:03 GMT
ENV MONO_THREADS_PER_CPU=50
# Fri, 15 May 2020 18:25:33 GMT
RUN MONO_VERSION=6.8.0.105 &&     FSHARP_VERSION=10.2.3 &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     apt-get update && apt-get --no-install-recommends install -y gnupg dirmngr ca-certificates apt-transport-https &&     apt-key adv --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" | tee /etc/apt/sources.list.d/mono-official-stable.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y pkg-config make nuget mono-devel msbuild ca-certificates-mono locales &&     rm -rf /var/lib/apt/lists/* &&     echo 'en_US.UTF-8 UTF-8' > /etc/locale.gen && /usr/sbin/locale-gen &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local "$GNUPGHOME" &&     apt-get purge -y make gnupg dirmngr &&     apt-get clean
# Fri, 15 May 2020 18:25:33 GMT
WORKDIR /root
# Fri, 15 May 2020 18:25:33 GMT
CMD ["fsharpi"]
# Fri, 15 May 2020 18:41:41 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Fri, 15 May 2020 18:41:42 GMT
ENV FrameworkPathOverride=/usr/lib/mono/4.7.2-api/
# Fri, 15 May 2020 18:41:42 GMT
ENV NUGET_XMLDOC_MODE=skip DOTNET_RUNNING_IN_CONTAINER=true DOTNET_USE_POLLING_FILE_WATCHER=true
# Fri, 15 May 2020 18:41:50 GMT
RUN apt-get update &&     apt-get --no-install-recommends install -y     curl     libunwind8     gettext     apt-transport-https     libc6     libcurl4     libgcc1     libgssapi-krb5-2     libicu63     liblttng-ust0     libssl1.1     libstdc++6     libunwind8     libuuid1     zlib1g &&     rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 18:42:09 GMT
RUN DOTNET_SDK_VERSION=3.1.102 &&     DOTNET_SDK_DOWNLOAD_URL=https://dotnetcli.blob.core.windows.net/dotnet/Sdk/$DOTNET_SDK_VERSION/dotnet-sdk-$DOTNET_SDK_VERSION-linux-x64.tar.gz &&     DOTNET_SDK_DOWNLOAD_SHA=9cacdc9700468a915e6fa51a3e5539b3519dd35b13e7f9d6c4dd0077e298baac0e50ad1880181df6781ef1dc64a232e9f78ad8e4494022987d12812c4ca15f29 &&     curl -SL $DOTNET_SDK_DOWNLOAD_URL --output dotnet.tar.gz &&     echo "$DOTNET_SDK_DOWNLOAD_SHA dotnet.tar.gz" | sha512sum -c - &&     mkdir -p /usr/share/dotnet &&     tar -zxf dotnet.tar.gz -C /usr/share/dotnet &&     rm dotnet.tar.gz &&     ln -s /usr/share/dotnet/dotnet /usr/bin/dotnet
# Fri, 15 May 2020 18:42:12 GMT
RUN mkdir warmup &&     cd warmup &&     dotnet new &&     cd - &&     rm -rf warmup /tmp/NuGetScratch
# Fri, 15 May 2020 18:42:12 GMT
WORKDIR /root
# Fri, 15 May 2020 18:42:13 GMT
CMD ["dotnet" "fsi"]
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74fe1ed6bb8e743af51a92cb071b53473eb49ba5abc8b134ee57da16c97a8c3e`  
		Last Modified: Fri, 15 May 2020 18:43:24 GMT  
		Size: 159.5 MB (159519960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16e515bde9e6a2dc65dd91aff7df88f3211f60f6530ed06a675d142e2e1a8b7`  
		Last Modified: Fri, 15 May 2020 18:44:24 GMT  
		Size: 17.2 MB (17202106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0cad3a34065b68dcf2be73336e175f225380b3e30303a6814646985b15d246f`  
		Last Modified: Fri, 15 May 2020 18:44:49 GMT  
		Size: 115.9 MB (115919150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ccdf5bc4037ddb48d0201a5d94402d5ae2b1145cb01a43a426e49f36aed4b7`  
		Last Modified: Fri, 15 May 2020 18:44:19 GMT  
		Size: 3.9 MB (3941616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fsharp:10.7-netcore`

```console
$ docker pull fsharp@sha256:fac2fb64dd348a9b553d9744f37e5cbdc815a71308c7c5424df69fa7f3c3dc37
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `fsharp:10.7-netcore` - linux; amd64

```console
$ docker pull fsharp@sha256:6e1a36d58bf3ae7d6290967c2dd89521ec5b96ee2bfa69effbc38f1f35c53552
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.7 MB (323681588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b58060dddba748160f27e9036737add43a27c5c5418917972e799c9a591627cb`
-	Default Command: `["dotnet","fsi"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 18:16:03 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Fri, 15 May 2020 18:16:03 GMT
ENV MONO_THREADS_PER_CPU=50
# Fri, 15 May 2020 18:25:33 GMT
RUN MONO_VERSION=6.8.0.105 &&     FSHARP_VERSION=10.2.3 &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     apt-get update && apt-get --no-install-recommends install -y gnupg dirmngr ca-certificates apt-transport-https &&     apt-key adv --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" | tee /etc/apt/sources.list.d/mono-official-stable.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y pkg-config make nuget mono-devel msbuild ca-certificates-mono locales &&     rm -rf /var/lib/apt/lists/* &&     echo 'en_US.UTF-8 UTF-8' > /etc/locale.gen && /usr/sbin/locale-gen &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local "$GNUPGHOME" &&     apt-get purge -y make gnupg dirmngr &&     apt-get clean
# Fri, 15 May 2020 18:25:33 GMT
WORKDIR /root
# Fri, 15 May 2020 18:25:33 GMT
CMD ["fsharpi"]
# Fri, 15 May 2020 18:41:41 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Fri, 15 May 2020 18:41:42 GMT
ENV FrameworkPathOverride=/usr/lib/mono/4.7.2-api/
# Fri, 15 May 2020 18:41:42 GMT
ENV NUGET_XMLDOC_MODE=skip DOTNET_RUNNING_IN_CONTAINER=true DOTNET_USE_POLLING_FILE_WATCHER=true
# Fri, 15 May 2020 18:41:50 GMT
RUN apt-get update &&     apt-get --no-install-recommends install -y     curl     libunwind8     gettext     apt-transport-https     libc6     libcurl4     libgcc1     libgssapi-krb5-2     libicu63     liblttng-ust0     libssl1.1     libstdc++6     libunwind8     libuuid1     zlib1g &&     rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 18:42:09 GMT
RUN DOTNET_SDK_VERSION=3.1.102 &&     DOTNET_SDK_DOWNLOAD_URL=https://dotnetcli.blob.core.windows.net/dotnet/Sdk/$DOTNET_SDK_VERSION/dotnet-sdk-$DOTNET_SDK_VERSION-linux-x64.tar.gz &&     DOTNET_SDK_DOWNLOAD_SHA=9cacdc9700468a915e6fa51a3e5539b3519dd35b13e7f9d6c4dd0077e298baac0e50ad1880181df6781ef1dc64a232e9f78ad8e4494022987d12812c4ca15f29 &&     curl -SL $DOTNET_SDK_DOWNLOAD_URL --output dotnet.tar.gz &&     echo "$DOTNET_SDK_DOWNLOAD_SHA dotnet.tar.gz" | sha512sum -c - &&     mkdir -p /usr/share/dotnet &&     tar -zxf dotnet.tar.gz -C /usr/share/dotnet &&     rm dotnet.tar.gz &&     ln -s /usr/share/dotnet/dotnet /usr/bin/dotnet
# Fri, 15 May 2020 18:42:12 GMT
RUN mkdir warmup &&     cd warmup &&     dotnet new &&     cd - &&     rm -rf warmup /tmp/NuGetScratch
# Fri, 15 May 2020 18:42:12 GMT
WORKDIR /root
# Fri, 15 May 2020 18:42:13 GMT
CMD ["dotnet" "fsi"]
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74fe1ed6bb8e743af51a92cb071b53473eb49ba5abc8b134ee57da16c97a8c3e`  
		Last Modified: Fri, 15 May 2020 18:43:24 GMT  
		Size: 159.5 MB (159519960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16e515bde9e6a2dc65dd91aff7df88f3211f60f6530ed06a675d142e2e1a8b7`  
		Last Modified: Fri, 15 May 2020 18:44:24 GMT  
		Size: 17.2 MB (17202106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0cad3a34065b68dcf2be73336e175f225380b3e30303a6814646985b15d246f`  
		Last Modified: Fri, 15 May 2020 18:44:49 GMT  
		Size: 115.9 MB (115919150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ccdf5bc4037ddb48d0201a5d94402d5ae2b1145cb01a43a426e49f36aed4b7`  
		Last Modified: Fri, 15 May 2020 18:44:19 GMT  
		Size: 3.9 MB (3941616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fsharp:10-netcore`

```console
$ docker pull fsharp@sha256:fac2fb64dd348a9b553d9744f37e5cbdc815a71308c7c5424df69fa7f3c3dc37
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `fsharp:10-netcore` - linux; amd64

```console
$ docker pull fsharp@sha256:6e1a36d58bf3ae7d6290967c2dd89521ec5b96ee2bfa69effbc38f1f35c53552
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.7 MB (323681588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b58060dddba748160f27e9036737add43a27c5c5418917972e799c9a591627cb`
-	Default Command: `["dotnet","fsi"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 18:16:03 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Fri, 15 May 2020 18:16:03 GMT
ENV MONO_THREADS_PER_CPU=50
# Fri, 15 May 2020 18:25:33 GMT
RUN MONO_VERSION=6.8.0.105 &&     FSHARP_VERSION=10.2.3 &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     apt-get update && apt-get --no-install-recommends install -y gnupg dirmngr ca-certificates apt-transport-https &&     apt-key adv --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" | tee /etc/apt/sources.list.d/mono-official-stable.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y pkg-config make nuget mono-devel msbuild ca-certificates-mono locales &&     rm -rf /var/lib/apt/lists/* &&     echo 'en_US.UTF-8 UTF-8' > /etc/locale.gen && /usr/sbin/locale-gen &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local "$GNUPGHOME" &&     apt-get purge -y make gnupg dirmngr &&     apt-get clean
# Fri, 15 May 2020 18:25:33 GMT
WORKDIR /root
# Fri, 15 May 2020 18:25:33 GMT
CMD ["fsharpi"]
# Fri, 15 May 2020 18:41:41 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Fri, 15 May 2020 18:41:42 GMT
ENV FrameworkPathOverride=/usr/lib/mono/4.7.2-api/
# Fri, 15 May 2020 18:41:42 GMT
ENV NUGET_XMLDOC_MODE=skip DOTNET_RUNNING_IN_CONTAINER=true DOTNET_USE_POLLING_FILE_WATCHER=true
# Fri, 15 May 2020 18:41:50 GMT
RUN apt-get update &&     apt-get --no-install-recommends install -y     curl     libunwind8     gettext     apt-transport-https     libc6     libcurl4     libgcc1     libgssapi-krb5-2     libicu63     liblttng-ust0     libssl1.1     libstdc++6     libunwind8     libuuid1     zlib1g &&     rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 18:42:09 GMT
RUN DOTNET_SDK_VERSION=3.1.102 &&     DOTNET_SDK_DOWNLOAD_URL=https://dotnetcli.blob.core.windows.net/dotnet/Sdk/$DOTNET_SDK_VERSION/dotnet-sdk-$DOTNET_SDK_VERSION-linux-x64.tar.gz &&     DOTNET_SDK_DOWNLOAD_SHA=9cacdc9700468a915e6fa51a3e5539b3519dd35b13e7f9d6c4dd0077e298baac0e50ad1880181df6781ef1dc64a232e9f78ad8e4494022987d12812c4ca15f29 &&     curl -SL $DOTNET_SDK_DOWNLOAD_URL --output dotnet.tar.gz &&     echo "$DOTNET_SDK_DOWNLOAD_SHA dotnet.tar.gz" | sha512sum -c - &&     mkdir -p /usr/share/dotnet &&     tar -zxf dotnet.tar.gz -C /usr/share/dotnet &&     rm dotnet.tar.gz &&     ln -s /usr/share/dotnet/dotnet /usr/bin/dotnet
# Fri, 15 May 2020 18:42:12 GMT
RUN mkdir warmup &&     cd warmup &&     dotnet new &&     cd - &&     rm -rf warmup /tmp/NuGetScratch
# Fri, 15 May 2020 18:42:12 GMT
WORKDIR /root
# Fri, 15 May 2020 18:42:13 GMT
CMD ["dotnet" "fsi"]
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74fe1ed6bb8e743af51a92cb071b53473eb49ba5abc8b134ee57da16c97a8c3e`  
		Last Modified: Fri, 15 May 2020 18:43:24 GMT  
		Size: 159.5 MB (159519960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16e515bde9e6a2dc65dd91aff7df88f3211f60f6530ed06a675d142e2e1a8b7`  
		Last Modified: Fri, 15 May 2020 18:44:24 GMT  
		Size: 17.2 MB (17202106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0cad3a34065b68dcf2be73336e175f225380b3e30303a6814646985b15d246f`  
		Last Modified: Fri, 15 May 2020 18:44:49 GMT  
		Size: 115.9 MB (115919150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ccdf5bc4037ddb48d0201a5d94402d5ae2b1145cb01a43a426e49f36aed4b7`  
		Last Modified: Fri, 15 May 2020 18:44:19 GMT  
		Size: 3.9 MB (3941616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fsharp:4`

```console
$ docker pull fsharp@sha256:052f2292f0955135402c6a2cff2fa51eb8079daecab0d113310282c6ce2bb6a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `fsharp:4` - linux; amd64

```console
$ docker pull fsharp@sha256:c9c0722cb4bbc3860f9135399cf646a6d5179f3b47368aff4dcc01c9062251fa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.3 MB (176299198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dc4e789a44c1847cb4443bbb013fc988520a4fd99b4f6d2b3e905f5f7c9e3e3`
-	Default Command: `["fsharpi"]`

```dockerfile
# Fri, 15 May 2020 06:29:39 GMT
ADD file:faa01786a6e5d5cc8855c0af88b1d49ddee288ddd39f479eff4da038a8e88065 in / 
# Fri, 15 May 2020 06:29:39 GMT
CMD ["bash"]
# Fri, 15 May 2020 18:25:41 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Fri, 15 May 2020 18:25:42 GMT
ENV MONO_THREADS_PER_CPU=50
# Fri, 15 May 2020 18:41:29 GMT
RUN MONO_VERSION=5.8.0.108 &&     FSHARP_VERSION=4.1.34 &&     FSHARP_PREFIX=/usr &&     FSHARP_GACDIR=/usr/lib/mono/gac &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     apt-key adv --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y autoconf libtool pkg-config make automake nuget mono-devel msbuild ca-certificates-mono &&     rm -rf /var/lib/apt/lists/* &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     ./autogen.sh --prefix=$FSHARP_PREFIX --with-gacdir=$FSHARP_GACDIR &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local &&     apt-get purge -y autoconf libtool make automake &&     apt-get clean
# Fri, 15 May 2020 18:41:30 GMT
WORKDIR /root
# Fri, 15 May 2020 18:41:30 GMT
CMD ["fsharpi"]
```

-	Layers:
	-	`sha256:a4834f3e07e2bd6b73cd4027a9549e06e42312f401d6307015085f7c0c2f112d`  
		Last Modified: Fri, 15 May 2020 06:38:13 GMT  
		Size: 30.2 MB (30159415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a0ab39aafbe5055f54281c31ddb1032b3e3340d7553f11f319ef69bfcce916`  
		Last Modified: Fri, 15 May 2020 18:44:11 GMT  
		Size: 146.1 MB (146139783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fsharp:4.1`

```console
$ docker pull fsharp@sha256:052f2292f0955135402c6a2cff2fa51eb8079daecab0d113310282c6ce2bb6a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `fsharp:4.1` - linux; amd64

```console
$ docker pull fsharp@sha256:c9c0722cb4bbc3860f9135399cf646a6d5179f3b47368aff4dcc01c9062251fa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.3 MB (176299198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dc4e789a44c1847cb4443bbb013fc988520a4fd99b4f6d2b3e905f5f7c9e3e3`
-	Default Command: `["fsharpi"]`

```dockerfile
# Fri, 15 May 2020 06:29:39 GMT
ADD file:faa01786a6e5d5cc8855c0af88b1d49ddee288ddd39f479eff4da038a8e88065 in / 
# Fri, 15 May 2020 06:29:39 GMT
CMD ["bash"]
# Fri, 15 May 2020 18:25:41 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Fri, 15 May 2020 18:25:42 GMT
ENV MONO_THREADS_PER_CPU=50
# Fri, 15 May 2020 18:41:29 GMT
RUN MONO_VERSION=5.8.0.108 &&     FSHARP_VERSION=4.1.34 &&     FSHARP_PREFIX=/usr &&     FSHARP_GACDIR=/usr/lib/mono/gac &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     apt-key adv --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y autoconf libtool pkg-config make automake nuget mono-devel msbuild ca-certificates-mono &&     rm -rf /var/lib/apt/lists/* &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     ./autogen.sh --prefix=$FSHARP_PREFIX --with-gacdir=$FSHARP_GACDIR &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local &&     apt-get purge -y autoconf libtool make automake &&     apt-get clean
# Fri, 15 May 2020 18:41:30 GMT
WORKDIR /root
# Fri, 15 May 2020 18:41:30 GMT
CMD ["fsharpi"]
```

-	Layers:
	-	`sha256:a4834f3e07e2bd6b73cd4027a9549e06e42312f401d6307015085f7c0c2f112d`  
		Last Modified: Fri, 15 May 2020 06:38:13 GMT  
		Size: 30.2 MB (30159415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a0ab39aafbe5055f54281c31ddb1032b3e3340d7553f11f319ef69bfcce916`  
		Last Modified: Fri, 15 May 2020 18:44:11 GMT  
		Size: 146.1 MB (146139783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fsharp:4.1.34`

```console
$ docker pull fsharp@sha256:052f2292f0955135402c6a2cff2fa51eb8079daecab0d113310282c6ce2bb6a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `fsharp:4.1.34` - linux; amd64

```console
$ docker pull fsharp@sha256:c9c0722cb4bbc3860f9135399cf646a6d5179f3b47368aff4dcc01c9062251fa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.3 MB (176299198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dc4e789a44c1847cb4443bbb013fc988520a4fd99b4f6d2b3e905f5f7c9e3e3`
-	Default Command: `["fsharpi"]`

```dockerfile
# Fri, 15 May 2020 06:29:39 GMT
ADD file:faa01786a6e5d5cc8855c0af88b1d49ddee288ddd39f479eff4da038a8e88065 in / 
# Fri, 15 May 2020 06:29:39 GMT
CMD ["bash"]
# Fri, 15 May 2020 18:25:41 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Fri, 15 May 2020 18:25:42 GMT
ENV MONO_THREADS_PER_CPU=50
# Fri, 15 May 2020 18:41:29 GMT
RUN MONO_VERSION=5.8.0.108 &&     FSHARP_VERSION=4.1.34 &&     FSHARP_PREFIX=/usr &&     FSHARP_GACDIR=/usr/lib/mono/gac &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     apt-key adv --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y autoconf libtool pkg-config make automake nuget mono-devel msbuild ca-certificates-mono &&     rm -rf /var/lib/apt/lists/* &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     ./autogen.sh --prefix=$FSHARP_PREFIX --with-gacdir=$FSHARP_GACDIR &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local &&     apt-get purge -y autoconf libtool make automake &&     apt-get clean
# Fri, 15 May 2020 18:41:30 GMT
WORKDIR /root
# Fri, 15 May 2020 18:41:30 GMT
CMD ["fsharpi"]
```

-	Layers:
	-	`sha256:a4834f3e07e2bd6b73cd4027a9549e06e42312f401d6307015085f7c0c2f112d`  
		Last Modified: Fri, 15 May 2020 06:38:13 GMT  
		Size: 30.2 MB (30159415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a0ab39aafbe5055f54281c31ddb1032b3e3340d7553f11f319ef69bfcce916`  
		Last Modified: Fri, 15 May 2020 18:44:11 GMT  
		Size: 146.1 MB (146139783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fsharp:latest`

```console
$ docker pull fsharp@sha256:d74735abb48ce5e5830569b3cc12fe2b8a0e40a8c02b5c48b2db0ced6faec0aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `fsharp:latest` - linux; amd64

```console
$ docker pull fsharp@sha256:76053ebd0f47351e7d2fd8647da6fb4f704c9b4f1d90cd1d76de4e6a2501d902
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.6 MB (186618716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07f1afa4082ad795eab7950031c098175b84369e3242e8ae984126f4e3acc441`
-	Default Command: `["fsharpi"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 18:16:03 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Fri, 15 May 2020 18:16:03 GMT
ENV MONO_THREADS_PER_CPU=50
# Fri, 15 May 2020 18:25:33 GMT
RUN MONO_VERSION=6.8.0.105 &&     FSHARP_VERSION=10.2.3 &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     apt-get update && apt-get --no-install-recommends install -y gnupg dirmngr ca-certificates apt-transport-https &&     apt-key adv --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" | tee /etc/apt/sources.list.d/mono-official-stable.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y pkg-config make nuget mono-devel msbuild ca-certificates-mono locales &&     rm -rf /var/lib/apt/lists/* &&     echo 'en_US.UTF-8 UTF-8' > /etc/locale.gen && /usr/sbin/locale-gen &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local "$GNUPGHOME" &&     apt-get purge -y make gnupg dirmngr &&     apt-get clean
# Fri, 15 May 2020 18:25:33 GMT
WORKDIR /root
# Fri, 15 May 2020 18:25:33 GMT
CMD ["fsharpi"]
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74fe1ed6bb8e743af51a92cb071b53473eb49ba5abc8b134ee57da16c97a8c3e`  
		Last Modified: Fri, 15 May 2020 18:43:24 GMT  
		Size: 159.5 MB (159519960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fsharp:latest` - linux; arm64 variant v8

```console
$ docker pull fsharp@sha256:703500113022afbd42119ea3e95d85404c2e61a3872cc43851f6ff872ffb1835
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.6 MB (183637080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc2dd8a49dfc0d4b3f98f61c4c3cf7d37d97e65433fb28c53e45cf5272e02f1c`
-	Default Command: `["fsharpi"]`

```dockerfile
# Wed, 13 May 2020 21:43:44 GMT
ADD file:37b141a882e9c33a09f7554ab39e3ba9c7f2b12e916c721436bd85817951eb4c in / 
# Wed, 13 May 2020 21:43:47 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:52:12 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Thu, 14 May 2020 00:52:13 GMT
ENV MONO_THREADS_PER_CPU=50
# Thu, 14 May 2020 01:10:21 GMT
RUN MONO_VERSION=6.8.0.105 &&     FSHARP_VERSION=10.2.3 &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     apt-get update && apt-get --no-install-recommends install -y gnupg dirmngr ca-certificates apt-transport-https &&     apt-key adv --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" | tee /etc/apt/sources.list.d/mono-official-stable.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y pkg-config make nuget mono-devel msbuild ca-certificates-mono locales &&     rm -rf /var/lib/apt/lists/* &&     echo 'en_US.UTF-8 UTF-8' > /etc/locale.gen && /usr/sbin/locale-gen &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local "$GNUPGHOME" &&     apt-get purge -y make gnupg dirmngr &&     apt-get clean
# Thu, 14 May 2020 01:10:36 GMT
WORKDIR /root
# Thu, 14 May 2020 01:10:38 GMT
CMD ["fsharpi"]
```

-	Layers:
	-	`sha256:b24dc5b5f4f0ffe0f8a33241aa35f3d74ee4213bc2b87eb3ec4b72a6e70ba7bc`  
		Last Modified: Wed, 13 May 2020 21:53:15 GMT  
		Size: 25.9 MB (25851785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4c3526a3ff4107662914bbca00c466fa6c0bd17772c578e1b14e0a456da8710`  
		Last Modified: Thu, 14 May 2020 01:11:52 GMT  
		Size: 157.8 MB (157785295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fsharp:netcore`

```console
$ docker pull fsharp@sha256:fac2fb64dd348a9b553d9744f37e5cbdc815a71308c7c5424df69fa7f3c3dc37
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `fsharp:netcore` - linux; amd64

```console
$ docker pull fsharp@sha256:6e1a36d58bf3ae7d6290967c2dd89521ec5b96ee2bfa69effbc38f1f35c53552
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.7 MB (323681588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b58060dddba748160f27e9036737add43a27c5c5418917972e799c9a591627cb`
-	Default Command: `["dotnet","fsi"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 18:16:03 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Fri, 15 May 2020 18:16:03 GMT
ENV MONO_THREADS_PER_CPU=50
# Fri, 15 May 2020 18:25:33 GMT
RUN MONO_VERSION=6.8.0.105 &&     FSHARP_VERSION=10.2.3 &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     apt-get update && apt-get --no-install-recommends install -y gnupg dirmngr ca-certificates apt-transport-https &&     apt-key adv --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" | tee /etc/apt/sources.list.d/mono-official-stable.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y pkg-config make nuget mono-devel msbuild ca-certificates-mono locales &&     rm -rf /var/lib/apt/lists/* &&     echo 'en_US.UTF-8 UTF-8' > /etc/locale.gen && /usr/sbin/locale-gen &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local "$GNUPGHOME" &&     apt-get purge -y make gnupg dirmngr &&     apt-get clean
# Fri, 15 May 2020 18:25:33 GMT
WORKDIR /root
# Fri, 15 May 2020 18:25:33 GMT
CMD ["fsharpi"]
# Fri, 15 May 2020 18:41:41 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Fri, 15 May 2020 18:41:42 GMT
ENV FrameworkPathOverride=/usr/lib/mono/4.7.2-api/
# Fri, 15 May 2020 18:41:42 GMT
ENV NUGET_XMLDOC_MODE=skip DOTNET_RUNNING_IN_CONTAINER=true DOTNET_USE_POLLING_FILE_WATCHER=true
# Fri, 15 May 2020 18:41:50 GMT
RUN apt-get update &&     apt-get --no-install-recommends install -y     curl     libunwind8     gettext     apt-transport-https     libc6     libcurl4     libgcc1     libgssapi-krb5-2     libicu63     liblttng-ust0     libssl1.1     libstdc++6     libunwind8     libuuid1     zlib1g &&     rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 18:42:09 GMT
RUN DOTNET_SDK_VERSION=3.1.102 &&     DOTNET_SDK_DOWNLOAD_URL=https://dotnetcli.blob.core.windows.net/dotnet/Sdk/$DOTNET_SDK_VERSION/dotnet-sdk-$DOTNET_SDK_VERSION-linux-x64.tar.gz &&     DOTNET_SDK_DOWNLOAD_SHA=9cacdc9700468a915e6fa51a3e5539b3519dd35b13e7f9d6c4dd0077e298baac0e50ad1880181df6781ef1dc64a232e9f78ad8e4494022987d12812c4ca15f29 &&     curl -SL $DOTNET_SDK_DOWNLOAD_URL --output dotnet.tar.gz &&     echo "$DOTNET_SDK_DOWNLOAD_SHA dotnet.tar.gz" | sha512sum -c - &&     mkdir -p /usr/share/dotnet &&     tar -zxf dotnet.tar.gz -C /usr/share/dotnet &&     rm dotnet.tar.gz &&     ln -s /usr/share/dotnet/dotnet /usr/bin/dotnet
# Fri, 15 May 2020 18:42:12 GMT
RUN mkdir warmup &&     cd warmup &&     dotnet new &&     cd - &&     rm -rf warmup /tmp/NuGetScratch
# Fri, 15 May 2020 18:42:12 GMT
WORKDIR /root
# Fri, 15 May 2020 18:42:13 GMT
CMD ["dotnet" "fsi"]
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74fe1ed6bb8e743af51a92cb071b53473eb49ba5abc8b134ee57da16c97a8c3e`  
		Last Modified: Fri, 15 May 2020 18:43:24 GMT  
		Size: 159.5 MB (159519960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16e515bde9e6a2dc65dd91aff7df88f3211f60f6530ed06a675d142e2e1a8b7`  
		Last Modified: Fri, 15 May 2020 18:44:24 GMT  
		Size: 17.2 MB (17202106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0cad3a34065b68dcf2be73336e175f225380b3e30303a6814646985b15d246f`  
		Last Modified: Fri, 15 May 2020 18:44:49 GMT  
		Size: 115.9 MB (115919150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ccdf5bc4037ddb48d0201a5d94402d5ae2b1145cb01a43a426e49f36aed4b7`  
		Last Modified: Fri, 15 May 2020 18:44:19 GMT  
		Size: 3.9 MB (3941616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
