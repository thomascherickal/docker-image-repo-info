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
$ docker pull fsharp@sha256:0c0863dc4614b54441d44d046d50711428b2b0c9b693ebf2cd356df365a3f307
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `fsharp:10` - linux; amd64

```console
$ docker pull fsharp@sha256:e85186e8f5f07033b8506d54857fc8e623dd6b4f82e06848f55adb606d148228
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.6 MB (186621139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eea53ecdc52826f4405ef6450e50216cfdc7774a1ba2a41d318a3c1d75d865a1`
-	Default Command: `["fsharpi"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 22:14:06 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Tue, 04 Aug 2020 22:14:06 GMT
ENV MONO_THREADS_PER_CPU=50
# Tue, 04 Aug 2020 22:23:10 GMT
RUN MONO_VERSION=6.8.0.105 &&     FSHARP_VERSION=10.2.3 &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     apt-get update && apt-get --no-install-recommends install -y gnupg dirmngr ca-certificates apt-transport-https &&     apt-key adv --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" | tee /etc/apt/sources.list.d/mono-official-stable.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y pkg-config make nuget mono-devel msbuild ca-certificates-mono locales &&     rm -rf /var/lib/apt/lists/* &&     echo 'en_US.UTF-8 UTF-8' > /etc/locale.gen && /usr/sbin/locale-gen &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local "$GNUPGHOME" &&     apt-get purge -y make gnupg dirmngr &&     apt-get clean
# Tue, 04 Aug 2020 22:23:11 GMT
WORKDIR /root
# Tue, 04 Aug 2020 22:23:11 GMT
CMD ["fsharpi"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad071f039e224d782f72efb004400d9a41f2296d99b6be15dffeef86552641f7`  
		Last Modified: Tue, 04 Aug 2020 22:38:06 GMT  
		Size: 159.5 MB (159529018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fsharp:10` - linux; arm64 variant v8

```console
$ docker pull fsharp@sha256:84e54fc81a1a270267d92a0f4693a083b3fffef5971c0606267df4c65d269335
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.6 MB (183616233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09bed1ae438a3866ac8dd13a22626ec69c861a4b18334cbfc93bde4e1918a0e9`
-	Default Command: `["fsharpi"]`

```dockerfile
# Wed, 09 Sep 2020 23:50:54 GMT
ADD file:d870fb0484ea283840d9cc923c9c3fe36d1bb6b3b5ecfefcce06aa26a22c9414 in / 
# Wed, 09 Sep 2020 23:50:57 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 03:01:12 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Thu, 10 Sep 2020 03:01:13 GMT
ENV MONO_THREADS_PER_CPU=50
# Thu, 10 Sep 2020 03:19:05 GMT
RUN MONO_VERSION=6.8.0.105 &&     FSHARP_VERSION=10.2.3 &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     apt-get update && apt-get --no-install-recommends install -y gnupg dirmngr ca-certificates apt-transport-https &&     apt-key adv --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" | tee /etc/apt/sources.list.d/mono-official-stable.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y pkg-config make nuget mono-devel msbuild ca-certificates-mono locales &&     rm -rf /var/lib/apt/lists/* &&     echo 'en_US.UTF-8 UTF-8' > /etc/locale.gen && /usr/sbin/locale-gen &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local "$GNUPGHOME" &&     apt-get purge -y make gnupg dirmngr &&     apt-get clean
# Thu, 10 Sep 2020 03:19:11 GMT
WORKDIR /root
# Thu, 10 Sep 2020 03:19:12 GMT
CMD ["fsharpi"]
```

-	Layers:
	-	`sha256:a6d76de28f58f3470aff71c934c0fec4e5d0fad788f8b8bcc50601266fc1b34d`  
		Last Modified: Wed, 09 Sep 2020 23:59:09 GMT  
		Size: 25.8 MB (25849325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ac8dd03e8ff2dde050544eb443da735f1fcbab184cabf5533ccd96fdab3f6f6`  
		Last Modified: Thu, 10 Sep 2020 03:20:16 GMT  
		Size: 157.8 MB (157766908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fsharp:10.7`

```console
$ docker pull fsharp@sha256:0c0863dc4614b54441d44d046d50711428b2b0c9b693ebf2cd356df365a3f307
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `fsharp:10.7` - linux; amd64

```console
$ docker pull fsharp@sha256:e85186e8f5f07033b8506d54857fc8e623dd6b4f82e06848f55adb606d148228
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.6 MB (186621139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eea53ecdc52826f4405ef6450e50216cfdc7774a1ba2a41d318a3c1d75d865a1`
-	Default Command: `["fsharpi"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 22:14:06 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Tue, 04 Aug 2020 22:14:06 GMT
ENV MONO_THREADS_PER_CPU=50
# Tue, 04 Aug 2020 22:23:10 GMT
RUN MONO_VERSION=6.8.0.105 &&     FSHARP_VERSION=10.2.3 &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     apt-get update && apt-get --no-install-recommends install -y gnupg dirmngr ca-certificates apt-transport-https &&     apt-key adv --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" | tee /etc/apt/sources.list.d/mono-official-stable.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y pkg-config make nuget mono-devel msbuild ca-certificates-mono locales &&     rm -rf /var/lib/apt/lists/* &&     echo 'en_US.UTF-8 UTF-8' > /etc/locale.gen && /usr/sbin/locale-gen &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local "$GNUPGHOME" &&     apt-get purge -y make gnupg dirmngr &&     apt-get clean
# Tue, 04 Aug 2020 22:23:11 GMT
WORKDIR /root
# Tue, 04 Aug 2020 22:23:11 GMT
CMD ["fsharpi"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad071f039e224d782f72efb004400d9a41f2296d99b6be15dffeef86552641f7`  
		Last Modified: Tue, 04 Aug 2020 22:38:06 GMT  
		Size: 159.5 MB (159529018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fsharp:10.7` - linux; arm64 variant v8

```console
$ docker pull fsharp@sha256:84e54fc81a1a270267d92a0f4693a083b3fffef5971c0606267df4c65d269335
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.6 MB (183616233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09bed1ae438a3866ac8dd13a22626ec69c861a4b18334cbfc93bde4e1918a0e9`
-	Default Command: `["fsharpi"]`

```dockerfile
# Wed, 09 Sep 2020 23:50:54 GMT
ADD file:d870fb0484ea283840d9cc923c9c3fe36d1bb6b3b5ecfefcce06aa26a22c9414 in / 
# Wed, 09 Sep 2020 23:50:57 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 03:01:12 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Thu, 10 Sep 2020 03:01:13 GMT
ENV MONO_THREADS_PER_CPU=50
# Thu, 10 Sep 2020 03:19:05 GMT
RUN MONO_VERSION=6.8.0.105 &&     FSHARP_VERSION=10.2.3 &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     apt-get update && apt-get --no-install-recommends install -y gnupg dirmngr ca-certificates apt-transport-https &&     apt-key adv --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" | tee /etc/apt/sources.list.d/mono-official-stable.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y pkg-config make nuget mono-devel msbuild ca-certificates-mono locales &&     rm -rf /var/lib/apt/lists/* &&     echo 'en_US.UTF-8 UTF-8' > /etc/locale.gen && /usr/sbin/locale-gen &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local "$GNUPGHOME" &&     apt-get purge -y make gnupg dirmngr &&     apt-get clean
# Thu, 10 Sep 2020 03:19:11 GMT
WORKDIR /root
# Thu, 10 Sep 2020 03:19:12 GMT
CMD ["fsharpi"]
```

-	Layers:
	-	`sha256:a6d76de28f58f3470aff71c934c0fec4e5d0fad788f8b8bcc50601266fc1b34d`  
		Last Modified: Wed, 09 Sep 2020 23:59:09 GMT  
		Size: 25.8 MB (25849325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ac8dd03e8ff2dde050544eb443da735f1fcbab184cabf5533ccd96fdab3f6f6`  
		Last Modified: Thu, 10 Sep 2020 03:20:16 GMT  
		Size: 157.8 MB (157766908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fsharp:10.7.0`

```console
$ docker pull fsharp@sha256:0c0863dc4614b54441d44d046d50711428b2b0c9b693ebf2cd356df365a3f307
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `fsharp:10.7.0` - linux; amd64

```console
$ docker pull fsharp@sha256:e85186e8f5f07033b8506d54857fc8e623dd6b4f82e06848f55adb606d148228
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.6 MB (186621139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eea53ecdc52826f4405ef6450e50216cfdc7774a1ba2a41d318a3c1d75d865a1`
-	Default Command: `["fsharpi"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 22:14:06 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Tue, 04 Aug 2020 22:14:06 GMT
ENV MONO_THREADS_PER_CPU=50
# Tue, 04 Aug 2020 22:23:10 GMT
RUN MONO_VERSION=6.8.0.105 &&     FSHARP_VERSION=10.2.3 &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     apt-get update && apt-get --no-install-recommends install -y gnupg dirmngr ca-certificates apt-transport-https &&     apt-key adv --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" | tee /etc/apt/sources.list.d/mono-official-stable.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y pkg-config make nuget mono-devel msbuild ca-certificates-mono locales &&     rm -rf /var/lib/apt/lists/* &&     echo 'en_US.UTF-8 UTF-8' > /etc/locale.gen && /usr/sbin/locale-gen &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local "$GNUPGHOME" &&     apt-get purge -y make gnupg dirmngr &&     apt-get clean
# Tue, 04 Aug 2020 22:23:11 GMT
WORKDIR /root
# Tue, 04 Aug 2020 22:23:11 GMT
CMD ["fsharpi"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad071f039e224d782f72efb004400d9a41f2296d99b6be15dffeef86552641f7`  
		Last Modified: Tue, 04 Aug 2020 22:38:06 GMT  
		Size: 159.5 MB (159529018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fsharp:10.7.0` - linux; arm64 variant v8

```console
$ docker pull fsharp@sha256:84e54fc81a1a270267d92a0f4693a083b3fffef5971c0606267df4c65d269335
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.6 MB (183616233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09bed1ae438a3866ac8dd13a22626ec69c861a4b18334cbfc93bde4e1918a0e9`
-	Default Command: `["fsharpi"]`

```dockerfile
# Wed, 09 Sep 2020 23:50:54 GMT
ADD file:d870fb0484ea283840d9cc923c9c3fe36d1bb6b3b5ecfefcce06aa26a22c9414 in / 
# Wed, 09 Sep 2020 23:50:57 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 03:01:12 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Thu, 10 Sep 2020 03:01:13 GMT
ENV MONO_THREADS_PER_CPU=50
# Thu, 10 Sep 2020 03:19:05 GMT
RUN MONO_VERSION=6.8.0.105 &&     FSHARP_VERSION=10.2.3 &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     apt-get update && apt-get --no-install-recommends install -y gnupg dirmngr ca-certificates apt-transport-https &&     apt-key adv --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" | tee /etc/apt/sources.list.d/mono-official-stable.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y pkg-config make nuget mono-devel msbuild ca-certificates-mono locales &&     rm -rf /var/lib/apt/lists/* &&     echo 'en_US.UTF-8 UTF-8' > /etc/locale.gen && /usr/sbin/locale-gen &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local "$GNUPGHOME" &&     apt-get purge -y make gnupg dirmngr &&     apt-get clean
# Thu, 10 Sep 2020 03:19:11 GMT
WORKDIR /root
# Thu, 10 Sep 2020 03:19:12 GMT
CMD ["fsharpi"]
```

-	Layers:
	-	`sha256:a6d76de28f58f3470aff71c934c0fec4e5d0fad788f8b8bcc50601266fc1b34d`  
		Last Modified: Wed, 09 Sep 2020 23:59:09 GMT  
		Size: 25.8 MB (25849325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ac8dd03e8ff2dde050544eb443da735f1fcbab184cabf5533ccd96fdab3f6f6`  
		Last Modified: Thu, 10 Sep 2020 03:20:16 GMT  
		Size: 157.8 MB (157766908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fsharp:10.7.0-netcore`

```console
$ docker pull fsharp@sha256:5f5721f5a5468f57315317e577944a883bed9a84a909a351962f2f226623bcd8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `fsharp:10.7.0-netcore` - linux; amd64

```console
$ docker pull fsharp@sha256:8512a1784a97fc052d9008b3870f3b8b136adfc455487818a70f477f86e80774
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.7 MB (323684044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c618c56837120d0f20a31472f1a9c29332f0c76b531799a39d22a2350395a79`
-	Default Command: `["dotnet","fsi"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 22:14:06 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Tue, 04 Aug 2020 22:14:06 GMT
ENV MONO_THREADS_PER_CPU=50
# Tue, 04 Aug 2020 22:23:10 GMT
RUN MONO_VERSION=6.8.0.105 &&     FSHARP_VERSION=10.2.3 &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     apt-get update && apt-get --no-install-recommends install -y gnupg dirmngr ca-certificates apt-transport-https &&     apt-key adv --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" | tee /etc/apt/sources.list.d/mono-official-stable.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y pkg-config make nuget mono-devel msbuild ca-certificates-mono locales &&     rm -rf /var/lib/apt/lists/* &&     echo 'en_US.UTF-8 UTF-8' > /etc/locale.gen && /usr/sbin/locale-gen &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local "$GNUPGHOME" &&     apt-get purge -y make gnupg dirmngr &&     apt-get clean
# Tue, 04 Aug 2020 22:23:11 GMT
WORKDIR /root
# Tue, 04 Aug 2020 22:23:11 GMT
CMD ["fsharpi"]
# Tue, 04 Aug 2020 22:36:27 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Tue, 04 Aug 2020 22:36:28 GMT
ENV FrameworkPathOverride=/usr/lib/mono/4.7.2-api/
# Tue, 04 Aug 2020 22:36:28 GMT
ENV NUGET_XMLDOC_MODE=skip DOTNET_RUNNING_IN_CONTAINER=true DOTNET_USE_POLLING_FILE_WATCHER=true
# Tue, 04 Aug 2020 22:36:35 GMT
RUN apt-get update &&     apt-get --no-install-recommends install -y     curl     libunwind8     gettext     apt-transport-https     libc6     libcurl4     libgcc1     libgssapi-krb5-2     libicu63     liblttng-ust0     libssl1.1     libstdc++6     libunwind8     libuuid1     zlib1g &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 22:36:50 GMT
RUN DOTNET_SDK_VERSION=3.1.102 &&     DOTNET_SDK_DOWNLOAD_URL=https://dotnetcli.blob.core.windows.net/dotnet/Sdk/$DOTNET_SDK_VERSION/dotnet-sdk-$DOTNET_SDK_VERSION-linux-x64.tar.gz &&     DOTNET_SDK_DOWNLOAD_SHA=9cacdc9700468a915e6fa51a3e5539b3519dd35b13e7f9d6c4dd0077e298baac0e50ad1880181df6781ef1dc64a232e9f78ad8e4494022987d12812c4ca15f29 &&     curl -SL $DOTNET_SDK_DOWNLOAD_URL --output dotnet.tar.gz &&     echo "$DOTNET_SDK_DOWNLOAD_SHA dotnet.tar.gz" | sha512sum -c - &&     mkdir -p /usr/share/dotnet &&     tar -zxf dotnet.tar.gz -C /usr/share/dotnet &&     rm dotnet.tar.gz &&     ln -s /usr/share/dotnet/dotnet /usr/bin/dotnet
# Tue, 04 Aug 2020 22:36:52 GMT
RUN mkdir warmup &&     cd warmup &&     dotnet new &&     cd - &&     rm -rf warmup /tmp/NuGetScratch
# Tue, 04 Aug 2020 22:36:52 GMT
WORKDIR /root
# Tue, 04 Aug 2020 22:36:52 GMT
CMD ["dotnet" "fsi"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad071f039e224d782f72efb004400d9a41f2296d99b6be15dffeef86552641f7`  
		Last Modified: Tue, 04 Aug 2020 22:38:06 GMT  
		Size: 159.5 MB (159529018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae93fda9e26eaab1c47295d50f5d9d5e65f85eeeb63a4f4ccc4197e682df1a1`  
		Last Modified: Tue, 04 Aug 2020 22:38:48 GMT  
		Size: 17.2 MB (17202142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:379d586ed6618f91f7df8947d9e1f3405d57bd7e846b625c72de01bf6e07ff1c`  
		Last Modified: Tue, 04 Aug 2020 22:39:09 GMT  
		Size: 115.9 MB (115919163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87b7a1205fd827465854791ff9fe1088317f288e978d7e487496b3f840d10df`  
		Last Modified: Tue, 04 Aug 2020 22:38:44 GMT  
		Size: 3.9 MB (3941600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fsharp:10.7-netcore`

```console
$ docker pull fsharp@sha256:5f5721f5a5468f57315317e577944a883bed9a84a909a351962f2f226623bcd8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `fsharp:10.7-netcore` - linux; amd64

```console
$ docker pull fsharp@sha256:8512a1784a97fc052d9008b3870f3b8b136adfc455487818a70f477f86e80774
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.7 MB (323684044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c618c56837120d0f20a31472f1a9c29332f0c76b531799a39d22a2350395a79`
-	Default Command: `["dotnet","fsi"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 22:14:06 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Tue, 04 Aug 2020 22:14:06 GMT
ENV MONO_THREADS_PER_CPU=50
# Tue, 04 Aug 2020 22:23:10 GMT
RUN MONO_VERSION=6.8.0.105 &&     FSHARP_VERSION=10.2.3 &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     apt-get update && apt-get --no-install-recommends install -y gnupg dirmngr ca-certificates apt-transport-https &&     apt-key adv --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" | tee /etc/apt/sources.list.d/mono-official-stable.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y pkg-config make nuget mono-devel msbuild ca-certificates-mono locales &&     rm -rf /var/lib/apt/lists/* &&     echo 'en_US.UTF-8 UTF-8' > /etc/locale.gen && /usr/sbin/locale-gen &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local "$GNUPGHOME" &&     apt-get purge -y make gnupg dirmngr &&     apt-get clean
# Tue, 04 Aug 2020 22:23:11 GMT
WORKDIR /root
# Tue, 04 Aug 2020 22:23:11 GMT
CMD ["fsharpi"]
# Tue, 04 Aug 2020 22:36:27 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Tue, 04 Aug 2020 22:36:28 GMT
ENV FrameworkPathOverride=/usr/lib/mono/4.7.2-api/
# Tue, 04 Aug 2020 22:36:28 GMT
ENV NUGET_XMLDOC_MODE=skip DOTNET_RUNNING_IN_CONTAINER=true DOTNET_USE_POLLING_FILE_WATCHER=true
# Tue, 04 Aug 2020 22:36:35 GMT
RUN apt-get update &&     apt-get --no-install-recommends install -y     curl     libunwind8     gettext     apt-transport-https     libc6     libcurl4     libgcc1     libgssapi-krb5-2     libicu63     liblttng-ust0     libssl1.1     libstdc++6     libunwind8     libuuid1     zlib1g &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 22:36:50 GMT
RUN DOTNET_SDK_VERSION=3.1.102 &&     DOTNET_SDK_DOWNLOAD_URL=https://dotnetcli.blob.core.windows.net/dotnet/Sdk/$DOTNET_SDK_VERSION/dotnet-sdk-$DOTNET_SDK_VERSION-linux-x64.tar.gz &&     DOTNET_SDK_DOWNLOAD_SHA=9cacdc9700468a915e6fa51a3e5539b3519dd35b13e7f9d6c4dd0077e298baac0e50ad1880181df6781ef1dc64a232e9f78ad8e4494022987d12812c4ca15f29 &&     curl -SL $DOTNET_SDK_DOWNLOAD_URL --output dotnet.tar.gz &&     echo "$DOTNET_SDK_DOWNLOAD_SHA dotnet.tar.gz" | sha512sum -c - &&     mkdir -p /usr/share/dotnet &&     tar -zxf dotnet.tar.gz -C /usr/share/dotnet &&     rm dotnet.tar.gz &&     ln -s /usr/share/dotnet/dotnet /usr/bin/dotnet
# Tue, 04 Aug 2020 22:36:52 GMT
RUN mkdir warmup &&     cd warmup &&     dotnet new &&     cd - &&     rm -rf warmup /tmp/NuGetScratch
# Tue, 04 Aug 2020 22:36:52 GMT
WORKDIR /root
# Tue, 04 Aug 2020 22:36:52 GMT
CMD ["dotnet" "fsi"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad071f039e224d782f72efb004400d9a41f2296d99b6be15dffeef86552641f7`  
		Last Modified: Tue, 04 Aug 2020 22:38:06 GMT  
		Size: 159.5 MB (159529018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae93fda9e26eaab1c47295d50f5d9d5e65f85eeeb63a4f4ccc4197e682df1a1`  
		Last Modified: Tue, 04 Aug 2020 22:38:48 GMT  
		Size: 17.2 MB (17202142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:379d586ed6618f91f7df8947d9e1f3405d57bd7e846b625c72de01bf6e07ff1c`  
		Last Modified: Tue, 04 Aug 2020 22:39:09 GMT  
		Size: 115.9 MB (115919163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87b7a1205fd827465854791ff9fe1088317f288e978d7e487496b3f840d10df`  
		Last Modified: Tue, 04 Aug 2020 22:38:44 GMT  
		Size: 3.9 MB (3941600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fsharp:10-netcore`

```console
$ docker pull fsharp@sha256:5f5721f5a5468f57315317e577944a883bed9a84a909a351962f2f226623bcd8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `fsharp:10-netcore` - linux; amd64

```console
$ docker pull fsharp@sha256:8512a1784a97fc052d9008b3870f3b8b136adfc455487818a70f477f86e80774
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.7 MB (323684044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c618c56837120d0f20a31472f1a9c29332f0c76b531799a39d22a2350395a79`
-	Default Command: `["dotnet","fsi"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 22:14:06 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Tue, 04 Aug 2020 22:14:06 GMT
ENV MONO_THREADS_PER_CPU=50
# Tue, 04 Aug 2020 22:23:10 GMT
RUN MONO_VERSION=6.8.0.105 &&     FSHARP_VERSION=10.2.3 &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     apt-get update && apt-get --no-install-recommends install -y gnupg dirmngr ca-certificates apt-transport-https &&     apt-key adv --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" | tee /etc/apt/sources.list.d/mono-official-stable.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y pkg-config make nuget mono-devel msbuild ca-certificates-mono locales &&     rm -rf /var/lib/apt/lists/* &&     echo 'en_US.UTF-8 UTF-8' > /etc/locale.gen && /usr/sbin/locale-gen &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local "$GNUPGHOME" &&     apt-get purge -y make gnupg dirmngr &&     apt-get clean
# Tue, 04 Aug 2020 22:23:11 GMT
WORKDIR /root
# Tue, 04 Aug 2020 22:23:11 GMT
CMD ["fsharpi"]
# Tue, 04 Aug 2020 22:36:27 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Tue, 04 Aug 2020 22:36:28 GMT
ENV FrameworkPathOverride=/usr/lib/mono/4.7.2-api/
# Tue, 04 Aug 2020 22:36:28 GMT
ENV NUGET_XMLDOC_MODE=skip DOTNET_RUNNING_IN_CONTAINER=true DOTNET_USE_POLLING_FILE_WATCHER=true
# Tue, 04 Aug 2020 22:36:35 GMT
RUN apt-get update &&     apt-get --no-install-recommends install -y     curl     libunwind8     gettext     apt-transport-https     libc6     libcurl4     libgcc1     libgssapi-krb5-2     libicu63     liblttng-ust0     libssl1.1     libstdc++6     libunwind8     libuuid1     zlib1g &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 22:36:50 GMT
RUN DOTNET_SDK_VERSION=3.1.102 &&     DOTNET_SDK_DOWNLOAD_URL=https://dotnetcli.blob.core.windows.net/dotnet/Sdk/$DOTNET_SDK_VERSION/dotnet-sdk-$DOTNET_SDK_VERSION-linux-x64.tar.gz &&     DOTNET_SDK_DOWNLOAD_SHA=9cacdc9700468a915e6fa51a3e5539b3519dd35b13e7f9d6c4dd0077e298baac0e50ad1880181df6781ef1dc64a232e9f78ad8e4494022987d12812c4ca15f29 &&     curl -SL $DOTNET_SDK_DOWNLOAD_URL --output dotnet.tar.gz &&     echo "$DOTNET_SDK_DOWNLOAD_SHA dotnet.tar.gz" | sha512sum -c - &&     mkdir -p /usr/share/dotnet &&     tar -zxf dotnet.tar.gz -C /usr/share/dotnet &&     rm dotnet.tar.gz &&     ln -s /usr/share/dotnet/dotnet /usr/bin/dotnet
# Tue, 04 Aug 2020 22:36:52 GMT
RUN mkdir warmup &&     cd warmup &&     dotnet new &&     cd - &&     rm -rf warmup /tmp/NuGetScratch
# Tue, 04 Aug 2020 22:36:52 GMT
WORKDIR /root
# Tue, 04 Aug 2020 22:36:52 GMT
CMD ["dotnet" "fsi"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad071f039e224d782f72efb004400d9a41f2296d99b6be15dffeef86552641f7`  
		Last Modified: Tue, 04 Aug 2020 22:38:06 GMT  
		Size: 159.5 MB (159529018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae93fda9e26eaab1c47295d50f5d9d5e65f85eeeb63a4f4ccc4197e682df1a1`  
		Last Modified: Tue, 04 Aug 2020 22:38:48 GMT  
		Size: 17.2 MB (17202142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:379d586ed6618f91f7df8947d9e1f3405d57bd7e846b625c72de01bf6e07ff1c`  
		Last Modified: Tue, 04 Aug 2020 22:39:09 GMT  
		Size: 115.9 MB (115919163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87b7a1205fd827465854791ff9fe1088317f288e978d7e487496b3f840d10df`  
		Last Modified: Tue, 04 Aug 2020 22:38:44 GMT  
		Size: 3.9 MB (3941600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fsharp:4`

```console
$ docker pull fsharp@sha256:7d58267ddf234c1eba51c4fd3b0656378894de9c0f9343c22e52fca840a8188c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `fsharp:4` - linux; amd64

```console
$ docker pull fsharp@sha256:2ac236e9259876a85be6b6dd1ab4e1d76b55ff46ce01d883f387ae6a942ecde9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.3 MB (176300544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac533703cb198727efbbc8d1e778f3beb6fdd44714ff94219ec7c11f32487614`
-	Default Command: `["fsharpi"]`

```dockerfile
# Tue, 04 Aug 2020 15:43:20 GMT
ADD file:f2ded135aabfb02dcfeb9df41447c58b6e156ed3889e7b97bc6c416b8f869e9b in / 
# Tue, 04 Aug 2020 15:43:21 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 22:23:30 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Tue, 04 Aug 2020 22:23:30 GMT
ENV MONO_THREADS_PER_CPU=50
# Tue, 04 Aug 2020 22:36:12 GMT
RUN MONO_VERSION=5.8.0.108 &&     FSHARP_VERSION=4.1.34 &&     FSHARP_PREFIX=/usr &&     FSHARP_GACDIR=/usr/lib/mono/gac &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     apt-key adv --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y autoconf libtool pkg-config make automake nuget mono-devel msbuild ca-certificates-mono &&     rm -rf /var/lib/apt/lists/* &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     ./autogen.sh --prefix=$FSHARP_PREFIX --with-gacdir=$FSHARP_GACDIR &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local &&     apt-get purge -y autoconf libtool make automake &&     apt-get clean
# Tue, 04 Aug 2020 22:36:13 GMT
WORKDIR /root
# Tue, 04 Aug 2020 22:36:13 GMT
CMD ["fsharpi"]
```

-	Layers:
	-	`sha256:358f5eb397669a96c573eeeece7fe974d14ea7264298456555494ad58a697022`  
		Last Modified: Tue, 04 Aug 2020 15:49:56 GMT  
		Size: 30.2 MB (30159619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b84da34f6a1dcf0fa65cf2f67158ec6b6a8eaf850379d74f66d42b2356b3c6d`  
		Last Modified: Tue, 04 Aug 2020 22:38:39 GMT  
		Size: 146.1 MB (146140925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fsharp:4.1`

```console
$ docker pull fsharp@sha256:7d58267ddf234c1eba51c4fd3b0656378894de9c0f9343c22e52fca840a8188c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `fsharp:4.1` - linux; amd64

```console
$ docker pull fsharp@sha256:2ac236e9259876a85be6b6dd1ab4e1d76b55ff46ce01d883f387ae6a942ecde9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.3 MB (176300544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac533703cb198727efbbc8d1e778f3beb6fdd44714ff94219ec7c11f32487614`
-	Default Command: `["fsharpi"]`

```dockerfile
# Tue, 04 Aug 2020 15:43:20 GMT
ADD file:f2ded135aabfb02dcfeb9df41447c58b6e156ed3889e7b97bc6c416b8f869e9b in / 
# Tue, 04 Aug 2020 15:43:21 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 22:23:30 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Tue, 04 Aug 2020 22:23:30 GMT
ENV MONO_THREADS_PER_CPU=50
# Tue, 04 Aug 2020 22:36:12 GMT
RUN MONO_VERSION=5.8.0.108 &&     FSHARP_VERSION=4.1.34 &&     FSHARP_PREFIX=/usr &&     FSHARP_GACDIR=/usr/lib/mono/gac &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     apt-key adv --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y autoconf libtool pkg-config make automake nuget mono-devel msbuild ca-certificates-mono &&     rm -rf /var/lib/apt/lists/* &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     ./autogen.sh --prefix=$FSHARP_PREFIX --with-gacdir=$FSHARP_GACDIR &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local &&     apt-get purge -y autoconf libtool make automake &&     apt-get clean
# Tue, 04 Aug 2020 22:36:13 GMT
WORKDIR /root
# Tue, 04 Aug 2020 22:36:13 GMT
CMD ["fsharpi"]
```

-	Layers:
	-	`sha256:358f5eb397669a96c573eeeece7fe974d14ea7264298456555494ad58a697022`  
		Last Modified: Tue, 04 Aug 2020 15:49:56 GMT  
		Size: 30.2 MB (30159619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b84da34f6a1dcf0fa65cf2f67158ec6b6a8eaf850379d74f66d42b2356b3c6d`  
		Last Modified: Tue, 04 Aug 2020 22:38:39 GMT  
		Size: 146.1 MB (146140925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fsharp:4.1.34`

```console
$ docker pull fsharp@sha256:7d58267ddf234c1eba51c4fd3b0656378894de9c0f9343c22e52fca840a8188c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `fsharp:4.1.34` - linux; amd64

```console
$ docker pull fsharp@sha256:2ac236e9259876a85be6b6dd1ab4e1d76b55ff46ce01d883f387ae6a942ecde9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.3 MB (176300544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac533703cb198727efbbc8d1e778f3beb6fdd44714ff94219ec7c11f32487614`
-	Default Command: `["fsharpi"]`

```dockerfile
# Tue, 04 Aug 2020 15:43:20 GMT
ADD file:f2ded135aabfb02dcfeb9df41447c58b6e156ed3889e7b97bc6c416b8f869e9b in / 
# Tue, 04 Aug 2020 15:43:21 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 22:23:30 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Tue, 04 Aug 2020 22:23:30 GMT
ENV MONO_THREADS_PER_CPU=50
# Tue, 04 Aug 2020 22:36:12 GMT
RUN MONO_VERSION=5.8.0.108 &&     FSHARP_VERSION=4.1.34 &&     FSHARP_PREFIX=/usr &&     FSHARP_GACDIR=/usr/lib/mono/gac &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     apt-key adv --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y autoconf libtool pkg-config make automake nuget mono-devel msbuild ca-certificates-mono &&     rm -rf /var/lib/apt/lists/* &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     ./autogen.sh --prefix=$FSHARP_PREFIX --with-gacdir=$FSHARP_GACDIR &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local &&     apt-get purge -y autoconf libtool make automake &&     apt-get clean
# Tue, 04 Aug 2020 22:36:13 GMT
WORKDIR /root
# Tue, 04 Aug 2020 22:36:13 GMT
CMD ["fsharpi"]
```

-	Layers:
	-	`sha256:358f5eb397669a96c573eeeece7fe974d14ea7264298456555494ad58a697022`  
		Last Modified: Tue, 04 Aug 2020 15:49:56 GMT  
		Size: 30.2 MB (30159619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b84da34f6a1dcf0fa65cf2f67158ec6b6a8eaf850379d74f66d42b2356b3c6d`  
		Last Modified: Tue, 04 Aug 2020 22:38:39 GMT  
		Size: 146.1 MB (146140925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fsharp:latest`

```console
$ docker pull fsharp@sha256:0c0863dc4614b54441d44d046d50711428b2b0c9b693ebf2cd356df365a3f307
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `fsharp:latest` - linux; amd64

```console
$ docker pull fsharp@sha256:e85186e8f5f07033b8506d54857fc8e623dd6b4f82e06848f55adb606d148228
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.6 MB (186621139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eea53ecdc52826f4405ef6450e50216cfdc7774a1ba2a41d318a3c1d75d865a1`
-	Default Command: `["fsharpi"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 22:14:06 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Tue, 04 Aug 2020 22:14:06 GMT
ENV MONO_THREADS_PER_CPU=50
# Tue, 04 Aug 2020 22:23:10 GMT
RUN MONO_VERSION=6.8.0.105 &&     FSHARP_VERSION=10.2.3 &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     apt-get update && apt-get --no-install-recommends install -y gnupg dirmngr ca-certificates apt-transport-https &&     apt-key adv --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" | tee /etc/apt/sources.list.d/mono-official-stable.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y pkg-config make nuget mono-devel msbuild ca-certificates-mono locales &&     rm -rf /var/lib/apt/lists/* &&     echo 'en_US.UTF-8 UTF-8' > /etc/locale.gen && /usr/sbin/locale-gen &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local "$GNUPGHOME" &&     apt-get purge -y make gnupg dirmngr &&     apt-get clean
# Tue, 04 Aug 2020 22:23:11 GMT
WORKDIR /root
# Tue, 04 Aug 2020 22:23:11 GMT
CMD ["fsharpi"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad071f039e224d782f72efb004400d9a41f2296d99b6be15dffeef86552641f7`  
		Last Modified: Tue, 04 Aug 2020 22:38:06 GMT  
		Size: 159.5 MB (159529018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fsharp:latest` - linux; arm64 variant v8

```console
$ docker pull fsharp@sha256:84e54fc81a1a270267d92a0f4693a083b3fffef5971c0606267df4c65d269335
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.6 MB (183616233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09bed1ae438a3866ac8dd13a22626ec69c861a4b18334cbfc93bde4e1918a0e9`
-	Default Command: `["fsharpi"]`

```dockerfile
# Wed, 09 Sep 2020 23:50:54 GMT
ADD file:d870fb0484ea283840d9cc923c9c3fe36d1bb6b3b5ecfefcce06aa26a22c9414 in / 
# Wed, 09 Sep 2020 23:50:57 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 03:01:12 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Thu, 10 Sep 2020 03:01:13 GMT
ENV MONO_THREADS_PER_CPU=50
# Thu, 10 Sep 2020 03:19:05 GMT
RUN MONO_VERSION=6.8.0.105 &&     FSHARP_VERSION=10.2.3 &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     apt-get update && apt-get --no-install-recommends install -y gnupg dirmngr ca-certificates apt-transport-https &&     apt-key adv --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" | tee /etc/apt/sources.list.d/mono-official-stable.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y pkg-config make nuget mono-devel msbuild ca-certificates-mono locales &&     rm -rf /var/lib/apt/lists/* &&     echo 'en_US.UTF-8 UTF-8' > /etc/locale.gen && /usr/sbin/locale-gen &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local "$GNUPGHOME" &&     apt-get purge -y make gnupg dirmngr &&     apt-get clean
# Thu, 10 Sep 2020 03:19:11 GMT
WORKDIR /root
# Thu, 10 Sep 2020 03:19:12 GMT
CMD ["fsharpi"]
```

-	Layers:
	-	`sha256:a6d76de28f58f3470aff71c934c0fec4e5d0fad788f8b8bcc50601266fc1b34d`  
		Last Modified: Wed, 09 Sep 2020 23:59:09 GMT  
		Size: 25.8 MB (25849325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ac8dd03e8ff2dde050544eb443da735f1fcbab184cabf5533ccd96fdab3f6f6`  
		Last Modified: Thu, 10 Sep 2020 03:20:16 GMT  
		Size: 157.8 MB (157766908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fsharp:netcore`

```console
$ docker pull fsharp@sha256:5f5721f5a5468f57315317e577944a883bed9a84a909a351962f2f226623bcd8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `fsharp:netcore` - linux; amd64

```console
$ docker pull fsharp@sha256:8512a1784a97fc052d9008b3870f3b8b136adfc455487818a70f477f86e80774
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.7 MB (323684044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c618c56837120d0f20a31472f1a9c29332f0c76b531799a39d22a2350395a79`
-	Default Command: `["dotnet","fsi"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 22:14:06 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Tue, 04 Aug 2020 22:14:06 GMT
ENV MONO_THREADS_PER_CPU=50
# Tue, 04 Aug 2020 22:23:10 GMT
RUN MONO_VERSION=6.8.0.105 &&     FSHARP_VERSION=10.2.3 &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     apt-get update && apt-get --no-install-recommends install -y gnupg dirmngr ca-certificates apt-transport-https &&     apt-key adv --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" | tee /etc/apt/sources.list.d/mono-official-stable.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y pkg-config make nuget mono-devel msbuild ca-certificates-mono locales &&     rm -rf /var/lib/apt/lists/* &&     echo 'en_US.UTF-8 UTF-8' > /etc/locale.gen && /usr/sbin/locale-gen &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local "$GNUPGHOME" &&     apt-get purge -y make gnupg dirmngr &&     apt-get clean
# Tue, 04 Aug 2020 22:23:11 GMT
WORKDIR /root
# Tue, 04 Aug 2020 22:23:11 GMT
CMD ["fsharpi"]
# Tue, 04 Aug 2020 22:36:27 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Tue, 04 Aug 2020 22:36:28 GMT
ENV FrameworkPathOverride=/usr/lib/mono/4.7.2-api/
# Tue, 04 Aug 2020 22:36:28 GMT
ENV NUGET_XMLDOC_MODE=skip DOTNET_RUNNING_IN_CONTAINER=true DOTNET_USE_POLLING_FILE_WATCHER=true
# Tue, 04 Aug 2020 22:36:35 GMT
RUN apt-get update &&     apt-get --no-install-recommends install -y     curl     libunwind8     gettext     apt-transport-https     libc6     libcurl4     libgcc1     libgssapi-krb5-2     libicu63     liblttng-ust0     libssl1.1     libstdc++6     libunwind8     libuuid1     zlib1g &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 22:36:50 GMT
RUN DOTNET_SDK_VERSION=3.1.102 &&     DOTNET_SDK_DOWNLOAD_URL=https://dotnetcli.blob.core.windows.net/dotnet/Sdk/$DOTNET_SDK_VERSION/dotnet-sdk-$DOTNET_SDK_VERSION-linux-x64.tar.gz &&     DOTNET_SDK_DOWNLOAD_SHA=9cacdc9700468a915e6fa51a3e5539b3519dd35b13e7f9d6c4dd0077e298baac0e50ad1880181df6781ef1dc64a232e9f78ad8e4494022987d12812c4ca15f29 &&     curl -SL $DOTNET_SDK_DOWNLOAD_URL --output dotnet.tar.gz &&     echo "$DOTNET_SDK_DOWNLOAD_SHA dotnet.tar.gz" | sha512sum -c - &&     mkdir -p /usr/share/dotnet &&     tar -zxf dotnet.tar.gz -C /usr/share/dotnet &&     rm dotnet.tar.gz &&     ln -s /usr/share/dotnet/dotnet /usr/bin/dotnet
# Tue, 04 Aug 2020 22:36:52 GMT
RUN mkdir warmup &&     cd warmup &&     dotnet new &&     cd - &&     rm -rf warmup /tmp/NuGetScratch
# Tue, 04 Aug 2020 22:36:52 GMT
WORKDIR /root
# Tue, 04 Aug 2020 22:36:52 GMT
CMD ["dotnet" "fsi"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad071f039e224d782f72efb004400d9a41f2296d99b6be15dffeef86552641f7`  
		Last Modified: Tue, 04 Aug 2020 22:38:06 GMT  
		Size: 159.5 MB (159529018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae93fda9e26eaab1c47295d50f5d9d5e65f85eeeb63a4f4ccc4197e682df1a1`  
		Last Modified: Tue, 04 Aug 2020 22:38:48 GMT  
		Size: 17.2 MB (17202142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:379d586ed6618f91f7df8947d9e1f3405d57bd7e846b625c72de01bf6e07ff1c`  
		Last Modified: Tue, 04 Aug 2020 22:39:09 GMT  
		Size: 115.9 MB (115919163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87b7a1205fd827465854791ff9fe1088317f288e978d7e487496b3f840d10df`  
		Last Modified: Tue, 04 Aug 2020 22:38:44 GMT  
		Size: 3.9 MB (3941600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
