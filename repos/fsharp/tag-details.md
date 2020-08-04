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
$ docker pull fsharp@sha256:cb1d330d127542284525eec04ee59cdaf17f8bad4e0dfbbb8627b164e637ef79
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `fsharp:10` - linux; amd64

```console
$ docker pull fsharp@sha256:d5a7b8a26183d8a310a1123889187e145b5af52597fc44e37f5ed61da7507cb1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.6 MB (186614877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:939477056606d5bbb89d1c99d4ac8179f4697f57bb0ae86dfb80275b2dcd0c59`
-	Default Command: `["fsharpi"]`

```dockerfile
# Wed, 22 Jul 2020 02:03:37 GMT
ADD file:6ccb3bbcc69b0d44c48a8ef1bfa08d835444ea13b8a93701bd37d86b81b13ac2 in / 
# Wed, 22 Jul 2020 02:03:37 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 18:20:55 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Wed, 22 Jul 2020 18:20:55 GMT
ENV MONO_THREADS_PER_CPU=50
# Wed, 22 Jul 2020 18:33:41 GMT
RUN MONO_VERSION=6.8.0.105 &&     FSHARP_VERSION=10.2.3 &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     apt-get update && apt-get --no-install-recommends install -y gnupg dirmngr ca-certificates apt-transport-https &&     apt-key adv --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" | tee /etc/apt/sources.list.d/mono-official-stable.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y pkg-config make nuget mono-devel msbuild ca-certificates-mono locales &&     rm -rf /var/lib/apt/lists/* &&     echo 'en_US.UTF-8 UTF-8' > /etc/locale.gen && /usr/sbin/locale-gen &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local "$GNUPGHOME" &&     apt-get purge -y make gnupg dirmngr &&     apt-get clean
# Wed, 22 Jul 2020 18:33:42 GMT
WORKDIR /root
# Wed, 22 Jul 2020 18:33:42 GMT
CMD ["fsharpi"]
```

-	Layers:
	-	`sha256:6ec8c9369e08152361a01729f2c8a1e7aae898426c6e67267f41894bf9524827`  
		Last Modified: Wed, 22 Jul 2020 02:09:51 GMT  
		Size: 27.1 MB (27098544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc1a1f2ce3823522eb039c7c91b31af81a9e447d85e19590143dbe79e06a095`  
		Last Modified: Wed, 22 Jul 2020 18:51:16 GMT  
		Size: 159.5 MB (159516333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fsharp:10` - linux; arm64 variant v8

```console
$ docker pull fsharp@sha256:cc77bf6a597a9bae5cdf318dc2bb6aeab8181afc34af400f882056895b8c3ee6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.6 MB (183616374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f3348e155faea0d52b7e8281f83752bc9b42bdff4553a132da15cee0aeb79f0`
-	Default Command: `["fsharpi"]`

```dockerfile
# Tue, 04 Aug 2020 06:57:29 GMT
ADD file:90ba7821623ab55fc1073647cc611cc45f5e306ade734910e587021971483eec in / 
# Tue, 04 Aug 2020 06:57:31 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 12:10:25 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Tue, 04 Aug 2020 12:10:26 GMT
ENV MONO_THREADS_PER_CPU=50
# Tue, 04 Aug 2020 12:27:40 GMT
RUN MONO_VERSION=6.8.0.105 &&     FSHARP_VERSION=10.2.3 &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     apt-get update && apt-get --no-install-recommends install -y gnupg dirmngr ca-certificates apt-transport-https &&     apt-key adv --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" | tee /etc/apt/sources.list.d/mono-official-stable.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y pkg-config make nuget mono-devel msbuild ca-certificates-mono locales &&     rm -rf /var/lib/apt/lists/* &&     echo 'en_US.UTF-8 UTF-8' > /etc/locale.gen && /usr/sbin/locale-gen &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local "$GNUPGHOME" &&     apt-get purge -y make gnupg dirmngr &&     apt-get clean
# Tue, 04 Aug 2020 12:27:45 GMT
WORKDIR /root
# Tue, 04 Aug 2020 12:27:46 GMT
CMD ["fsharpi"]
```

-	Layers:
	-	`sha256:3742235f1882fee5cca1effc4ca0f0c7c180bbe169800a85daedcf3968b0d8f0`  
		Last Modified: Tue, 04 Aug 2020 07:04:03 GMT  
		Size: 25.8 MB (25849301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4190faf78aeba92e3dca92a54fc1b4cefaff4eee88c7af14b546a5a149900928`  
		Last Modified: Tue, 04 Aug 2020 12:29:03 GMT  
		Size: 157.8 MB (157767073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fsharp:10.7`

```console
$ docker pull fsharp@sha256:cb1d330d127542284525eec04ee59cdaf17f8bad4e0dfbbb8627b164e637ef79
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `fsharp:10.7` - linux; amd64

```console
$ docker pull fsharp@sha256:d5a7b8a26183d8a310a1123889187e145b5af52597fc44e37f5ed61da7507cb1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.6 MB (186614877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:939477056606d5bbb89d1c99d4ac8179f4697f57bb0ae86dfb80275b2dcd0c59`
-	Default Command: `["fsharpi"]`

```dockerfile
# Wed, 22 Jul 2020 02:03:37 GMT
ADD file:6ccb3bbcc69b0d44c48a8ef1bfa08d835444ea13b8a93701bd37d86b81b13ac2 in / 
# Wed, 22 Jul 2020 02:03:37 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 18:20:55 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Wed, 22 Jul 2020 18:20:55 GMT
ENV MONO_THREADS_PER_CPU=50
# Wed, 22 Jul 2020 18:33:41 GMT
RUN MONO_VERSION=6.8.0.105 &&     FSHARP_VERSION=10.2.3 &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     apt-get update && apt-get --no-install-recommends install -y gnupg dirmngr ca-certificates apt-transport-https &&     apt-key adv --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" | tee /etc/apt/sources.list.d/mono-official-stable.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y pkg-config make nuget mono-devel msbuild ca-certificates-mono locales &&     rm -rf /var/lib/apt/lists/* &&     echo 'en_US.UTF-8 UTF-8' > /etc/locale.gen && /usr/sbin/locale-gen &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local "$GNUPGHOME" &&     apt-get purge -y make gnupg dirmngr &&     apt-get clean
# Wed, 22 Jul 2020 18:33:42 GMT
WORKDIR /root
# Wed, 22 Jul 2020 18:33:42 GMT
CMD ["fsharpi"]
```

-	Layers:
	-	`sha256:6ec8c9369e08152361a01729f2c8a1e7aae898426c6e67267f41894bf9524827`  
		Last Modified: Wed, 22 Jul 2020 02:09:51 GMT  
		Size: 27.1 MB (27098544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc1a1f2ce3823522eb039c7c91b31af81a9e447d85e19590143dbe79e06a095`  
		Last Modified: Wed, 22 Jul 2020 18:51:16 GMT  
		Size: 159.5 MB (159516333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fsharp:10.7` - linux; arm64 variant v8

```console
$ docker pull fsharp@sha256:cc77bf6a597a9bae5cdf318dc2bb6aeab8181afc34af400f882056895b8c3ee6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.6 MB (183616374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f3348e155faea0d52b7e8281f83752bc9b42bdff4553a132da15cee0aeb79f0`
-	Default Command: `["fsharpi"]`

```dockerfile
# Tue, 04 Aug 2020 06:57:29 GMT
ADD file:90ba7821623ab55fc1073647cc611cc45f5e306ade734910e587021971483eec in / 
# Tue, 04 Aug 2020 06:57:31 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 12:10:25 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Tue, 04 Aug 2020 12:10:26 GMT
ENV MONO_THREADS_PER_CPU=50
# Tue, 04 Aug 2020 12:27:40 GMT
RUN MONO_VERSION=6.8.0.105 &&     FSHARP_VERSION=10.2.3 &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     apt-get update && apt-get --no-install-recommends install -y gnupg dirmngr ca-certificates apt-transport-https &&     apt-key adv --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" | tee /etc/apt/sources.list.d/mono-official-stable.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y pkg-config make nuget mono-devel msbuild ca-certificates-mono locales &&     rm -rf /var/lib/apt/lists/* &&     echo 'en_US.UTF-8 UTF-8' > /etc/locale.gen && /usr/sbin/locale-gen &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local "$GNUPGHOME" &&     apt-get purge -y make gnupg dirmngr &&     apt-get clean
# Tue, 04 Aug 2020 12:27:45 GMT
WORKDIR /root
# Tue, 04 Aug 2020 12:27:46 GMT
CMD ["fsharpi"]
```

-	Layers:
	-	`sha256:3742235f1882fee5cca1effc4ca0f0c7c180bbe169800a85daedcf3968b0d8f0`  
		Last Modified: Tue, 04 Aug 2020 07:04:03 GMT  
		Size: 25.8 MB (25849301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4190faf78aeba92e3dca92a54fc1b4cefaff4eee88c7af14b546a5a149900928`  
		Last Modified: Tue, 04 Aug 2020 12:29:03 GMT  
		Size: 157.8 MB (157767073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fsharp:10.7.0`

```console
$ docker pull fsharp@sha256:cb1d330d127542284525eec04ee59cdaf17f8bad4e0dfbbb8627b164e637ef79
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `fsharp:10.7.0` - linux; amd64

```console
$ docker pull fsharp@sha256:d5a7b8a26183d8a310a1123889187e145b5af52597fc44e37f5ed61da7507cb1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.6 MB (186614877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:939477056606d5bbb89d1c99d4ac8179f4697f57bb0ae86dfb80275b2dcd0c59`
-	Default Command: `["fsharpi"]`

```dockerfile
# Wed, 22 Jul 2020 02:03:37 GMT
ADD file:6ccb3bbcc69b0d44c48a8ef1bfa08d835444ea13b8a93701bd37d86b81b13ac2 in / 
# Wed, 22 Jul 2020 02:03:37 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 18:20:55 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Wed, 22 Jul 2020 18:20:55 GMT
ENV MONO_THREADS_PER_CPU=50
# Wed, 22 Jul 2020 18:33:41 GMT
RUN MONO_VERSION=6.8.0.105 &&     FSHARP_VERSION=10.2.3 &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     apt-get update && apt-get --no-install-recommends install -y gnupg dirmngr ca-certificates apt-transport-https &&     apt-key adv --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" | tee /etc/apt/sources.list.d/mono-official-stable.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y pkg-config make nuget mono-devel msbuild ca-certificates-mono locales &&     rm -rf /var/lib/apt/lists/* &&     echo 'en_US.UTF-8 UTF-8' > /etc/locale.gen && /usr/sbin/locale-gen &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local "$GNUPGHOME" &&     apt-get purge -y make gnupg dirmngr &&     apt-get clean
# Wed, 22 Jul 2020 18:33:42 GMT
WORKDIR /root
# Wed, 22 Jul 2020 18:33:42 GMT
CMD ["fsharpi"]
```

-	Layers:
	-	`sha256:6ec8c9369e08152361a01729f2c8a1e7aae898426c6e67267f41894bf9524827`  
		Last Modified: Wed, 22 Jul 2020 02:09:51 GMT  
		Size: 27.1 MB (27098544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc1a1f2ce3823522eb039c7c91b31af81a9e447d85e19590143dbe79e06a095`  
		Last Modified: Wed, 22 Jul 2020 18:51:16 GMT  
		Size: 159.5 MB (159516333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fsharp:10.7.0` - linux; arm64 variant v8

```console
$ docker pull fsharp@sha256:cc77bf6a597a9bae5cdf318dc2bb6aeab8181afc34af400f882056895b8c3ee6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.6 MB (183616374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f3348e155faea0d52b7e8281f83752bc9b42bdff4553a132da15cee0aeb79f0`
-	Default Command: `["fsharpi"]`

```dockerfile
# Tue, 04 Aug 2020 06:57:29 GMT
ADD file:90ba7821623ab55fc1073647cc611cc45f5e306ade734910e587021971483eec in / 
# Tue, 04 Aug 2020 06:57:31 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 12:10:25 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Tue, 04 Aug 2020 12:10:26 GMT
ENV MONO_THREADS_PER_CPU=50
# Tue, 04 Aug 2020 12:27:40 GMT
RUN MONO_VERSION=6.8.0.105 &&     FSHARP_VERSION=10.2.3 &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     apt-get update && apt-get --no-install-recommends install -y gnupg dirmngr ca-certificates apt-transport-https &&     apt-key adv --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" | tee /etc/apt/sources.list.d/mono-official-stable.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y pkg-config make nuget mono-devel msbuild ca-certificates-mono locales &&     rm -rf /var/lib/apt/lists/* &&     echo 'en_US.UTF-8 UTF-8' > /etc/locale.gen && /usr/sbin/locale-gen &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local "$GNUPGHOME" &&     apt-get purge -y make gnupg dirmngr &&     apt-get clean
# Tue, 04 Aug 2020 12:27:45 GMT
WORKDIR /root
# Tue, 04 Aug 2020 12:27:46 GMT
CMD ["fsharpi"]
```

-	Layers:
	-	`sha256:3742235f1882fee5cca1effc4ca0f0c7c180bbe169800a85daedcf3968b0d8f0`  
		Last Modified: Tue, 04 Aug 2020 07:04:03 GMT  
		Size: 25.8 MB (25849301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4190faf78aeba92e3dca92a54fc1b4cefaff4eee88c7af14b546a5a149900928`  
		Last Modified: Tue, 04 Aug 2020 12:29:03 GMT  
		Size: 157.8 MB (157767073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fsharp:10.7.0-netcore`

```console
$ docker pull fsharp@sha256:774cb89a4d59112fa4084c05d319c6a6280e3649a02731e333a5fb2fd8f4a199
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `fsharp:10.7.0-netcore` - linux; amd64

```console
$ docker pull fsharp@sha256:b23a7b3da30a78ad363c8d46a5f42013c68431db09f5f17a7add5bbf399d3a02
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.7 MB (323677738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b741b3b5b455c19b826d84e222ee3cfcc5c118695753b316614d8cbb3662b539`
-	Default Command: `["dotnet","fsi"]`

```dockerfile
# Wed, 22 Jul 2020 02:03:37 GMT
ADD file:6ccb3bbcc69b0d44c48a8ef1bfa08d835444ea13b8a93701bd37d86b81b13ac2 in / 
# Wed, 22 Jul 2020 02:03:37 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 18:20:55 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Wed, 22 Jul 2020 18:20:55 GMT
ENV MONO_THREADS_PER_CPU=50
# Wed, 22 Jul 2020 18:33:41 GMT
RUN MONO_VERSION=6.8.0.105 &&     FSHARP_VERSION=10.2.3 &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     apt-get update && apt-get --no-install-recommends install -y gnupg dirmngr ca-certificates apt-transport-https &&     apt-key adv --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" | tee /etc/apt/sources.list.d/mono-official-stable.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y pkg-config make nuget mono-devel msbuild ca-certificates-mono locales &&     rm -rf /var/lib/apt/lists/* &&     echo 'en_US.UTF-8 UTF-8' > /etc/locale.gen && /usr/sbin/locale-gen &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local "$GNUPGHOME" &&     apt-get purge -y make gnupg dirmngr &&     apt-get clean
# Wed, 22 Jul 2020 18:33:42 GMT
WORKDIR /root
# Wed, 22 Jul 2020 18:33:42 GMT
CMD ["fsharpi"]
# Wed, 22 Jul 2020 18:49:38 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Wed, 22 Jul 2020 18:49:38 GMT
ENV FrameworkPathOverride=/usr/lib/mono/4.7.2-api/
# Wed, 22 Jul 2020 18:49:39 GMT
ENV NUGET_XMLDOC_MODE=skip DOTNET_RUNNING_IN_CONTAINER=true DOTNET_USE_POLLING_FILE_WATCHER=true
# Wed, 22 Jul 2020 18:49:51 GMT
RUN apt-get update &&     apt-get --no-install-recommends install -y     curl     libunwind8     gettext     apt-transport-https     libc6     libcurl4     libgcc1     libgssapi-krb5-2     libicu63     liblttng-ust0     libssl1.1     libstdc++6     libunwind8     libuuid1     zlib1g &&     rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 18:50:16 GMT
RUN DOTNET_SDK_VERSION=3.1.102 &&     DOTNET_SDK_DOWNLOAD_URL=https://dotnetcli.blob.core.windows.net/dotnet/Sdk/$DOTNET_SDK_VERSION/dotnet-sdk-$DOTNET_SDK_VERSION-linux-x64.tar.gz &&     DOTNET_SDK_DOWNLOAD_SHA=9cacdc9700468a915e6fa51a3e5539b3519dd35b13e7f9d6c4dd0077e298baac0e50ad1880181df6781ef1dc64a232e9f78ad8e4494022987d12812c4ca15f29 &&     curl -SL $DOTNET_SDK_DOWNLOAD_URL --output dotnet.tar.gz &&     echo "$DOTNET_SDK_DOWNLOAD_SHA dotnet.tar.gz" | sha512sum -c - &&     mkdir -p /usr/share/dotnet &&     tar -zxf dotnet.tar.gz -C /usr/share/dotnet &&     rm dotnet.tar.gz &&     ln -s /usr/share/dotnet/dotnet /usr/bin/dotnet
# Wed, 22 Jul 2020 18:50:20 GMT
RUN mkdir warmup &&     cd warmup &&     dotnet new &&     cd - &&     rm -rf warmup /tmp/NuGetScratch
# Wed, 22 Jul 2020 18:50:20 GMT
WORKDIR /root
# Wed, 22 Jul 2020 18:50:20 GMT
CMD ["dotnet" "fsi"]
```

-	Layers:
	-	`sha256:6ec8c9369e08152361a01729f2c8a1e7aae898426c6e67267f41894bf9524827`  
		Last Modified: Wed, 22 Jul 2020 02:09:51 GMT  
		Size: 27.1 MB (27098544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc1a1f2ce3823522eb039c7c91b31af81a9e447d85e19590143dbe79e06a095`  
		Last Modified: Wed, 22 Jul 2020 18:51:16 GMT  
		Size: 159.5 MB (159516333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:282f28c472212d3d7c23a3091ea491c951112150aa8efcf31a49dbe0b3733272`  
		Last Modified: Wed, 22 Jul 2020 18:52:12 GMT  
		Size: 17.2 MB (17202129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22f0f195baaa00dc5780c98a9187f12c781e14575a1c717e0d5a315418c1067d`  
		Last Modified: Wed, 22 Jul 2020 18:52:33 GMT  
		Size: 115.9 MB (115919106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9843e3d655d3d75f96bcad739edcfd62e683c2c90ad611e71657738728b4512c`  
		Last Modified: Wed, 22 Jul 2020 18:52:09 GMT  
		Size: 3.9 MB (3941626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fsharp:10.7-netcore`

```console
$ docker pull fsharp@sha256:774cb89a4d59112fa4084c05d319c6a6280e3649a02731e333a5fb2fd8f4a199
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `fsharp:10.7-netcore` - linux; amd64

```console
$ docker pull fsharp@sha256:b23a7b3da30a78ad363c8d46a5f42013c68431db09f5f17a7add5bbf399d3a02
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.7 MB (323677738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b741b3b5b455c19b826d84e222ee3cfcc5c118695753b316614d8cbb3662b539`
-	Default Command: `["dotnet","fsi"]`

```dockerfile
# Wed, 22 Jul 2020 02:03:37 GMT
ADD file:6ccb3bbcc69b0d44c48a8ef1bfa08d835444ea13b8a93701bd37d86b81b13ac2 in / 
# Wed, 22 Jul 2020 02:03:37 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 18:20:55 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Wed, 22 Jul 2020 18:20:55 GMT
ENV MONO_THREADS_PER_CPU=50
# Wed, 22 Jul 2020 18:33:41 GMT
RUN MONO_VERSION=6.8.0.105 &&     FSHARP_VERSION=10.2.3 &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     apt-get update && apt-get --no-install-recommends install -y gnupg dirmngr ca-certificates apt-transport-https &&     apt-key adv --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" | tee /etc/apt/sources.list.d/mono-official-stable.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y pkg-config make nuget mono-devel msbuild ca-certificates-mono locales &&     rm -rf /var/lib/apt/lists/* &&     echo 'en_US.UTF-8 UTF-8' > /etc/locale.gen && /usr/sbin/locale-gen &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local "$GNUPGHOME" &&     apt-get purge -y make gnupg dirmngr &&     apt-get clean
# Wed, 22 Jul 2020 18:33:42 GMT
WORKDIR /root
# Wed, 22 Jul 2020 18:33:42 GMT
CMD ["fsharpi"]
# Wed, 22 Jul 2020 18:49:38 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Wed, 22 Jul 2020 18:49:38 GMT
ENV FrameworkPathOverride=/usr/lib/mono/4.7.2-api/
# Wed, 22 Jul 2020 18:49:39 GMT
ENV NUGET_XMLDOC_MODE=skip DOTNET_RUNNING_IN_CONTAINER=true DOTNET_USE_POLLING_FILE_WATCHER=true
# Wed, 22 Jul 2020 18:49:51 GMT
RUN apt-get update &&     apt-get --no-install-recommends install -y     curl     libunwind8     gettext     apt-transport-https     libc6     libcurl4     libgcc1     libgssapi-krb5-2     libicu63     liblttng-ust0     libssl1.1     libstdc++6     libunwind8     libuuid1     zlib1g &&     rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 18:50:16 GMT
RUN DOTNET_SDK_VERSION=3.1.102 &&     DOTNET_SDK_DOWNLOAD_URL=https://dotnetcli.blob.core.windows.net/dotnet/Sdk/$DOTNET_SDK_VERSION/dotnet-sdk-$DOTNET_SDK_VERSION-linux-x64.tar.gz &&     DOTNET_SDK_DOWNLOAD_SHA=9cacdc9700468a915e6fa51a3e5539b3519dd35b13e7f9d6c4dd0077e298baac0e50ad1880181df6781ef1dc64a232e9f78ad8e4494022987d12812c4ca15f29 &&     curl -SL $DOTNET_SDK_DOWNLOAD_URL --output dotnet.tar.gz &&     echo "$DOTNET_SDK_DOWNLOAD_SHA dotnet.tar.gz" | sha512sum -c - &&     mkdir -p /usr/share/dotnet &&     tar -zxf dotnet.tar.gz -C /usr/share/dotnet &&     rm dotnet.tar.gz &&     ln -s /usr/share/dotnet/dotnet /usr/bin/dotnet
# Wed, 22 Jul 2020 18:50:20 GMT
RUN mkdir warmup &&     cd warmup &&     dotnet new &&     cd - &&     rm -rf warmup /tmp/NuGetScratch
# Wed, 22 Jul 2020 18:50:20 GMT
WORKDIR /root
# Wed, 22 Jul 2020 18:50:20 GMT
CMD ["dotnet" "fsi"]
```

-	Layers:
	-	`sha256:6ec8c9369e08152361a01729f2c8a1e7aae898426c6e67267f41894bf9524827`  
		Last Modified: Wed, 22 Jul 2020 02:09:51 GMT  
		Size: 27.1 MB (27098544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc1a1f2ce3823522eb039c7c91b31af81a9e447d85e19590143dbe79e06a095`  
		Last Modified: Wed, 22 Jul 2020 18:51:16 GMT  
		Size: 159.5 MB (159516333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:282f28c472212d3d7c23a3091ea491c951112150aa8efcf31a49dbe0b3733272`  
		Last Modified: Wed, 22 Jul 2020 18:52:12 GMT  
		Size: 17.2 MB (17202129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22f0f195baaa00dc5780c98a9187f12c781e14575a1c717e0d5a315418c1067d`  
		Last Modified: Wed, 22 Jul 2020 18:52:33 GMT  
		Size: 115.9 MB (115919106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9843e3d655d3d75f96bcad739edcfd62e683c2c90ad611e71657738728b4512c`  
		Last Modified: Wed, 22 Jul 2020 18:52:09 GMT  
		Size: 3.9 MB (3941626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fsharp:10-netcore`

```console
$ docker pull fsharp@sha256:774cb89a4d59112fa4084c05d319c6a6280e3649a02731e333a5fb2fd8f4a199
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `fsharp:10-netcore` - linux; amd64

```console
$ docker pull fsharp@sha256:b23a7b3da30a78ad363c8d46a5f42013c68431db09f5f17a7add5bbf399d3a02
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.7 MB (323677738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b741b3b5b455c19b826d84e222ee3cfcc5c118695753b316614d8cbb3662b539`
-	Default Command: `["dotnet","fsi"]`

```dockerfile
# Wed, 22 Jul 2020 02:03:37 GMT
ADD file:6ccb3bbcc69b0d44c48a8ef1bfa08d835444ea13b8a93701bd37d86b81b13ac2 in / 
# Wed, 22 Jul 2020 02:03:37 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 18:20:55 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Wed, 22 Jul 2020 18:20:55 GMT
ENV MONO_THREADS_PER_CPU=50
# Wed, 22 Jul 2020 18:33:41 GMT
RUN MONO_VERSION=6.8.0.105 &&     FSHARP_VERSION=10.2.3 &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     apt-get update && apt-get --no-install-recommends install -y gnupg dirmngr ca-certificates apt-transport-https &&     apt-key adv --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" | tee /etc/apt/sources.list.d/mono-official-stable.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y pkg-config make nuget mono-devel msbuild ca-certificates-mono locales &&     rm -rf /var/lib/apt/lists/* &&     echo 'en_US.UTF-8 UTF-8' > /etc/locale.gen && /usr/sbin/locale-gen &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local "$GNUPGHOME" &&     apt-get purge -y make gnupg dirmngr &&     apt-get clean
# Wed, 22 Jul 2020 18:33:42 GMT
WORKDIR /root
# Wed, 22 Jul 2020 18:33:42 GMT
CMD ["fsharpi"]
# Wed, 22 Jul 2020 18:49:38 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Wed, 22 Jul 2020 18:49:38 GMT
ENV FrameworkPathOverride=/usr/lib/mono/4.7.2-api/
# Wed, 22 Jul 2020 18:49:39 GMT
ENV NUGET_XMLDOC_MODE=skip DOTNET_RUNNING_IN_CONTAINER=true DOTNET_USE_POLLING_FILE_WATCHER=true
# Wed, 22 Jul 2020 18:49:51 GMT
RUN apt-get update &&     apt-get --no-install-recommends install -y     curl     libunwind8     gettext     apt-transport-https     libc6     libcurl4     libgcc1     libgssapi-krb5-2     libicu63     liblttng-ust0     libssl1.1     libstdc++6     libunwind8     libuuid1     zlib1g &&     rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 18:50:16 GMT
RUN DOTNET_SDK_VERSION=3.1.102 &&     DOTNET_SDK_DOWNLOAD_URL=https://dotnetcli.blob.core.windows.net/dotnet/Sdk/$DOTNET_SDK_VERSION/dotnet-sdk-$DOTNET_SDK_VERSION-linux-x64.tar.gz &&     DOTNET_SDK_DOWNLOAD_SHA=9cacdc9700468a915e6fa51a3e5539b3519dd35b13e7f9d6c4dd0077e298baac0e50ad1880181df6781ef1dc64a232e9f78ad8e4494022987d12812c4ca15f29 &&     curl -SL $DOTNET_SDK_DOWNLOAD_URL --output dotnet.tar.gz &&     echo "$DOTNET_SDK_DOWNLOAD_SHA dotnet.tar.gz" | sha512sum -c - &&     mkdir -p /usr/share/dotnet &&     tar -zxf dotnet.tar.gz -C /usr/share/dotnet &&     rm dotnet.tar.gz &&     ln -s /usr/share/dotnet/dotnet /usr/bin/dotnet
# Wed, 22 Jul 2020 18:50:20 GMT
RUN mkdir warmup &&     cd warmup &&     dotnet new &&     cd - &&     rm -rf warmup /tmp/NuGetScratch
# Wed, 22 Jul 2020 18:50:20 GMT
WORKDIR /root
# Wed, 22 Jul 2020 18:50:20 GMT
CMD ["dotnet" "fsi"]
```

-	Layers:
	-	`sha256:6ec8c9369e08152361a01729f2c8a1e7aae898426c6e67267f41894bf9524827`  
		Last Modified: Wed, 22 Jul 2020 02:09:51 GMT  
		Size: 27.1 MB (27098544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc1a1f2ce3823522eb039c7c91b31af81a9e447d85e19590143dbe79e06a095`  
		Last Modified: Wed, 22 Jul 2020 18:51:16 GMT  
		Size: 159.5 MB (159516333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:282f28c472212d3d7c23a3091ea491c951112150aa8efcf31a49dbe0b3733272`  
		Last Modified: Wed, 22 Jul 2020 18:52:12 GMT  
		Size: 17.2 MB (17202129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22f0f195baaa00dc5780c98a9187f12c781e14575a1c717e0d5a315418c1067d`  
		Last Modified: Wed, 22 Jul 2020 18:52:33 GMT  
		Size: 115.9 MB (115919106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9843e3d655d3d75f96bcad739edcfd62e683c2c90ad611e71657738728b4512c`  
		Last Modified: Wed, 22 Jul 2020 18:52:09 GMT  
		Size: 3.9 MB (3941626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fsharp:4`

```console
$ docker pull fsharp@sha256:5ce571ec1d7713024e5848d31661a2a17d941589462021910ebc63ea68ea2658
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `fsharp:4` - linux; amd64

```console
$ docker pull fsharp@sha256:a7d09cca81b27412e6f693e2bf2a1ccde5b269a9418243de835d667690428006
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.3 MB (176300188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:120246c59ccd4862c86d476955348dfc1c1925e98a8090d4ef15917a4b47ed5c`
-	Default Command: `["fsharpi"]`

```dockerfile
# Wed, 22 Jul 2020 02:04:16 GMT
ADD file:1b140421e4dff0539ea6d9a00828eeacf9255e74a317a1c8978ccdb450bb3d7a in / 
# Wed, 22 Jul 2020 02:04:17 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 18:33:52 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Wed, 22 Jul 2020 18:33:52 GMT
ENV MONO_THREADS_PER_CPU=50
# Wed, 22 Jul 2020 18:49:30 GMT
RUN MONO_VERSION=5.8.0.108 &&     FSHARP_VERSION=4.1.34 &&     FSHARP_PREFIX=/usr &&     FSHARP_GACDIR=/usr/lib/mono/gac &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     apt-key adv --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y autoconf libtool pkg-config make automake nuget mono-devel msbuild ca-certificates-mono &&     rm -rf /var/lib/apt/lists/* &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     ./autogen.sh --prefix=$FSHARP_PREFIX --with-gacdir=$FSHARP_GACDIR &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local &&     apt-get purge -y autoconf libtool make automake &&     apt-get clean
# Wed, 22 Jul 2020 18:49:31 GMT
WORKDIR /root
# Wed, 22 Jul 2020 18:49:31 GMT
CMD ["fsharpi"]
```

-	Layers:
	-	`sha256:724849f5fd5b18ee489d5838f03b76cd94d52a249d1d4f52da0453c6eaba7e7e`  
		Last Modified: Wed, 22 Jul 2020 02:10:26 GMT  
		Size: 30.2 MB (30159717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59bed6d420fc584cdeb639292320e2c3848c8106019e4681a406df13608034ec`  
		Last Modified: Wed, 22 Jul 2020 18:52:03 GMT  
		Size: 146.1 MB (146140471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fsharp:4.1`

```console
$ docker pull fsharp@sha256:5ce571ec1d7713024e5848d31661a2a17d941589462021910ebc63ea68ea2658
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `fsharp:4.1` - linux; amd64

```console
$ docker pull fsharp@sha256:a7d09cca81b27412e6f693e2bf2a1ccde5b269a9418243de835d667690428006
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.3 MB (176300188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:120246c59ccd4862c86d476955348dfc1c1925e98a8090d4ef15917a4b47ed5c`
-	Default Command: `["fsharpi"]`

```dockerfile
# Wed, 22 Jul 2020 02:04:16 GMT
ADD file:1b140421e4dff0539ea6d9a00828eeacf9255e74a317a1c8978ccdb450bb3d7a in / 
# Wed, 22 Jul 2020 02:04:17 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 18:33:52 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Wed, 22 Jul 2020 18:33:52 GMT
ENV MONO_THREADS_PER_CPU=50
# Wed, 22 Jul 2020 18:49:30 GMT
RUN MONO_VERSION=5.8.0.108 &&     FSHARP_VERSION=4.1.34 &&     FSHARP_PREFIX=/usr &&     FSHARP_GACDIR=/usr/lib/mono/gac &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     apt-key adv --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y autoconf libtool pkg-config make automake nuget mono-devel msbuild ca-certificates-mono &&     rm -rf /var/lib/apt/lists/* &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     ./autogen.sh --prefix=$FSHARP_PREFIX --with-gacdir=$FSHARP_GACDIR &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local &&     apt-get purge -y autoconf libtool make automake &&     apt-get clean
# Wed, 22 Jul 2020 18:49:31 GMT
WORKDIR /root
# Wed, 22 Jul 2020 18:49:31 GMT
CMD ["fsharpi"]
```

-	Layers:
	-	`sha256:724849f5fd5b18ee489d5838f03b76cd94d52a249d1d4f52da0453c6eaba7e7e`  
		Last Modified: Wed, 22 Jul 2020 02:10:26 GMT  
		Size: 30.2 MB (30159717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59bed6d420fc584cdeb639292320e2c3848c8106019e4681a406df13608034ec`  
		Last Modified: Wed, 22 Jul 2020 18:52:03 GMT  
		Size: 146.1 MB (146140471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fsharp:4.1.34`

```console
$ docker pull fsharp@sha256:5ce571ec1d7713024e5848d31661a2a17d941589462021910ebc63ea68ea2658
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `fsharp:4.1.34` - linux; amd64

```console
$ docker pull fsharp@sha256:a7d09cca81b27412e6f693e2bf2a1ccde5b269a9418243de835d667690428006
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.3 MB (176300188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:120246c59ccd4862c86d476955348dfc1c1925e98a8090d4ef15917a4b47ed5c`
-	Default Command: `["fsharpi"]`

```dockerfile
# Wed, 22 Jul 2020 02:04:16 GMT
ADD file:1b140421e4dff0539ea6d9a00828eeacf9255e74a317a1c8978ccdb450bb3d7a in / 
# Wed, 22 Jul 2020 02:04:17 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 18:33:52 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Wed, 22 Jul 2020 18:33:52 GMT
ENV MONO_THREADS_PER_CPU=50
# Wed, 22 Jul 2020 18:49:30 GMT
RUN MONO_VERSION=5.8.0.108 &&     FSHARP_VERSION=4.1.34 &&     FSHARP_PREFIX=/usr &&     FSHARP_GACDIR=/usr/lib/mono/gac &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     apt-key adv --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb http://download.mono-project.com/repo/debian jessie/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y autoconf libtool pkg-config make automake nuget mono-devel msbuild ca-certificates-mono &&     rm -rf /var/lib/apt/lists/* &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     ./autogen.sh --prefix=$FSHARP_PREFIX --with-gacdir=$FSHARP_GACDIR &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local &&     apt-get purge -y autoconf libtool make automake &&     apt-get clean
# Wed, 22 Jul 2020 18:49:31 GMT
WORKDIR /root
# Wed, 22 Jul 2020 18:49:31 GMT
CMD ["fsharpi"]
```

-	Layers:
	-	`sha256:724849f5fd5b18ee489d5838f03b76cd94d52a249d1d4f52da0453c6eaba7e7e`  
		Last Modified: Wed, 22 Jul 2020 02:10:26 GMT  
		Size: 30.2 MB (30159717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59bed6d420fc584cdeb639292320e2c3848c8106019e4681a406df13608034ec`  
		Last Modified: Wed, 22 Jul 2020 18:52:03 GMT  
		Size: 146.1 MB (146140471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fsharp:latest`

```console
$ docker pull fsharp@sha256:cb1d330d127542284525eec04ee59cdaf17f8bad4e0dfbbb8627b164e637ef79
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `fsharp:latest` - linux; amd64

```console
$ docker pull fsharp@sha256:d5a7b8a26183d8a310a1123889187e145b5af52597fc44e37f5ed61da7507cb1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.6 MB (186614877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:939477056606d5bbb89d1c99d4ac8179f4697f57bb0ae86dfb80275b2dcd0c59`
-	Default Command: `["fsharpi"]`

```dockerfile
# Wed, 22 Jul 2020 02:03:37 GMT
ADD file:6ccb3bbcc69b0d44c48a8ef1bfa08d835444ea13b8a93701bd37d86b81b13ac2 in / 
# Wed, 22 Jul 2020 02:03:37 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 18:20:55 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Wed, 22 Jul 2020 18:20:55 GMT
ENV MONO_THREADS_PER_CPU=50
# Wed, 22 Jul 2020 18:33:41 GMT
RUN MONO_VERSION=6.8.0.105 &&     FSHARP_VERSION=10.2.3 &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     apt-get update && apt-get --no-install-recommends install -y gnupg dirmngr ca-certificates apt-transport-https &&     apt-key adv --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" | tee /etc/apt/sources.list.d/mono-official-stable.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y pkg-config make nuget mono-devel msbuild ca-certificates-mono locales &&     rm -rf /var/lib/apt/lists/* &&     echo 'en_US.UTF-8 UTF-8' > /etc/locale.gen && /usr/sbin/locale-gen &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local "$GNUPGHOME" &&     apt-get purge -y make gnupg dirmngr &&     apt-get clean
# Wed, 22 Jul 2020 18:33:42 GMT
WORKDIR /root
# Wed, 22 Jul 2020 18:33:42 GMT
CMD ["fsharpi"]
```

-	Layers:
	-	`sha256:6ec8c9369e08152361a01729f2c8a1e7aae898426c6e67267f41894bf9524827`  
		Last Modified: Wed, 22 Jul 2020 02:09:51 GMT  
		Size: 27.1 MB (27098544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc1a1f2ce3823522eb039c7c91b31af81a9e447d85e19590143dbe79e06a095`  
		Last Modified: Wed, 22 Jul 2020 18:51:16 GMT  
		Size: 159.5 MB (159516333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fsharp:latest` - linux; arm64 variant v8

```console
$ docker pull fsharp@sha256:cc77bf6a597a9bae5cdf318dc2bb6aeab8181afc34af400f882056895b8c3ee6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.6 MB (183616374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f3348e155faea0d52b7e8281f83752bc9b42bdff4553a132da15cee0aeb79f0`
-	Default Command: `["fsharpi"]`

```dockerfile
# Tue, 04 Aug 2020 06:57:29 GMT
ADD file:90ba7821623ab55fc1073647cc611cc45f5e306ade734910e587021971483eec in / 
# Tue, 04 Aug 2020 06:57:31 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 12:10:25 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Tue, 04 Aug 2020 12:10:26 GMT
ENV MONO_THREADS_PER_CPU=50
# Tue, 04 Aug 2020 12:27:40 GMT
RUN MONO_VERSION=6.8.0.105 &&     FSHARP_VERSION=10.2.3 &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     apt-get update && apt-get --no-install-recommends install -y gnupg dirmngr ca-certificates apt-transport-https &&     apt-key adv --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" | tee /etc/apt/sources.list.d/mono-official-stable.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y pkg-config make nuget mono-devel msbuild ca-certificates-mono locales &&     rm -rf /var/lib/apt/lists/* &&     echo 'en_US.UTF-8 UTF-8' > /etc/locale.gen && /usr/sbin/locale-gen &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local "$GNUPGHOME" &&     apt-get purge -y make gnupg dirmngr &&     apt-get clean
# Tue, 04 Aug 2020 12:27:45 GMT
WORKDIR /root
# Tue, 04 Aug 2020 12:27:46 GMT
CMD ["fsharpi"]
```

-	Layers:
	-	`sha256:3742235f1882fee5cca1effc4ca0f0c7c180bbe169800a85daedcf3968b0d8f0`  
		Last Modified: Tue, 04 Aug 2020 07:04:03 GMT  
		Size: 25.8 MB (25849301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4190faf78aeba92e3dca92a54fc1b4cefaff4eee88c7af14b546a5a149900928`  
		Last Modified: Tue, 04 Aug 2020 12:29:03 GMT  
		Size: 157.8 MB (157767073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fsharp:netcore`

```console
$ docker pull fsharp@sha256:774cb89a4d59112fa4084c05d319c6a6280e3649a02731e333a5fb2fd8f4a199
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `fsharp:netcore` - linux; amd64

```console
$ docker pull fsharp@sha256:b23a7b3da30a78ad363c8d46a5f42013c68431db09f5f17a7add5bbf399d3a02
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.7 MB (323677738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b741b3b5b455c19b826d84e222ee3cfcc5c118695753b316614d8cbb3662b539`
-	Default Command: `["dotnet","fsi"]`

```dockerfile
# Wed, 22 Jul 2020 02:03:37 GMT
ADD file:6ccb3bbcc69b0d44c48a8ef1bfa08d835444ea13b8a93701bd37d86b81b13ac2 in / 
# Wed, 22 Jul 2020 02:03:37 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 18:20:55 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Wed, 22 Jul 2020 18:20:55 GMT
ENV MONO_THREADS_PER_CPU=50
# Wed, 22 Jul 2020 18:33:41 GMT
RUN MONO_VERSION=6.8.0.105 &&     FSHARP_VERSION=10.2.3 &&     FSHARP_BASENAME=fsharp-$FSHARP_VERSION &&     FSHARP_ARCHIVE=$FSHARP_VERSION.tar.gz &&     FSHARP_ARCHIVE_URL=https://github.com/fsharp/fsharp/archive/$FSHARP_VERSION.tar.gz &&     export GNUPGHOME="$(mktemp -d)" &&     apt-get update && apt-get --no-install-recommends install -y gnupg dirmngr ca-certificates apt-transport-https &&     apt-key adv --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF &&     echo "deb https://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" | tee /etc/apt/sources.list.d/mono-official-stable.list &&     apt-get update -y &&     apt-get --no-install-recommends install -y pkg-config make nuget mono-devel msbuild ca-certificates-mono locales &&     rm -rf /var/lib/apt/lists/* &&     echo 'en_US.UTF-8 UTF-8' > /etc/locale.gen && /usr/sbin/locale-gen &&     mkdir -p /tmp/src &&     cd /tmp/src &&     printf "namespace a { class b { public static void Main(string[] args) { new System.Net.WebClient().DownloadFile(\"%s\", \"%s\");}}}" $FSHARP_ARCHIVE_URL $FSHARP_ARCHIVE > download-fsharp.cs &&     mcs download-fsharp.cs && mono download-fsharp.exe && rm download-fsharp.exe download-fsharp.cs &&     tar xf $FSHARP_ARCHIVE &&     cd $FSHARP_BASENAME &&     make &&     make install &&     cd ~ &&     rm -rf /tmp/src /tmp/NuGetScratch ~/.nuget ~/.config ~/.local "$GNUPGHOME" &&     apt-get purge -y make gnupg dirmngr &&     apt-get clean
# Wed, 22 Jul 2020 18:33:42 GMT
WORKDIR /root
# Wed, 22 Jul 2020 18:33:42 GMT
CMD ["fsharpi"]
# Wed, 22 Jul 2020 18:49:38 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Steve Desmond <steve@stevedesmond.ca>
# Wed, 22 Jul 2020 18:49:38 GMT
ENV FrameworkPathOverride=/usr/lib/mono/4.7.2-api/
# Wed, 22 Jul 2020 18:49:39 GMT
ENV NUGET_XMLDOC_MODE=skip DOTNET_RUNNING_IN_CONTAINER=true DOTNET_USE_POLLING_FILE_WATCHER=true
# Wed, 22 Jul 2020 18:49:51 GMT
RUN apt-get update &&     apt-get --no-install-recommends install -y     curl     libunwind8     gettext     apt-transport-https     libc6     libcurl4     libgcc1     libgssapi-krb5-2     libicu63     liblttng-ust0     libssl1.1     libstdc++6     libunwind8     libuuid1     zlib1g &&     rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 18:50:16 GMT
RUN DOTNET_SDK_VERSION=3.1.102 &&     DOTNET_SDK_DOWNLOAD_URL=https://dotnetcli.blob.core.windows.net/dotnet/Sdk/$DOTNET_SDK_VERSION/dotnet-sdk-$DOTNET_SDK_VERSION-linux-x64.tar.gz &&     DOTNET_SDK_DOWNLOAD_SHA=9cacdc9700468a915e6fa51a3e5539b3519dd35b13e7f9d6c4dd0077e298baac0e50ad1880181df6781ef1dc64a232e9f78ad8e4494022987d12812c4ca15f29 &&     curl -SL $DOTNET_SDK_DOWNLOAD_URL --output dotnet.tar.gz &&     echo "$DOTNET_SDK_DOWNLOAD_SHA dotnet.tar.gz" | sha512sum -c - &&     mkdir -p /usr/share/dotnet &&     tar -zxf dotnet.tar.gz -C /usr/share/dotnet &&     rm dotnet.tar.gz &&     ln -s /usr/share/dotnet/dotnet /usr/bin/dotnet
# Wed, 22 Jul 2020 18:50:20 GMT
RUN mkdir warmup &&     cd warmup &&     dotnet new &&     cd - &&     rm -rf warmup /tmp/NuGetScratch
# Wed, 22 Jul 2020 18:50:20 GMT
WORKDIR /root
# Wed, 22 Jul 2020 18:50:20 GMT
CMD ["dotnet" "fsi"]
```

-	Layers:
	-	`sha256:6ec8c9369e08152361a01729f2c8a1e7aae898426c6e67267f41894bf9524827`  
		Last Modified: Wed, 22 Jul 2020 02:09:51 GMT  
		Size: 27.1 MB (27098544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc1a1f2ce3823522eb039c7c91b31af81a9e447d85e19590143dbe79e06a095`  
		Last Modified: Wed, 22 Jul 2020 18:51:16 GMT  
		Size: 159.5 MB (159516333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:282f28c472212d3d7c23a3091ea491c951112150aa8efcf31a49dbe0b3733272`  
		Last Modified: Wed, 22 Jul 2020 18:52:12 GMT  
		Size: 17.2 MB (17202129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22f0f195baaa00dc5780c98a9187f12c781e14575a1c717e0d5a315418c1067d`  
		Last Modified: Wed, 22 Jul 2020 18:52:33 GMT  
		Size: 115.9 MB (115919106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9843e3d655d3d75f96bcad739edcfd62e683c2c90ad611e71657738728b4512c`  
		Last Modified: Wed, 22 Jul 2020 18:52:09 GMT  
		Size: 3.9 MB (3941626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
