<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats`

-	[`nats:2`](#nats2)
-	[`nats:2.1`](#nats21)
-	[`nats:2.1.2`](#nats212)
-	[`nats:2.1.2-alpine`](#nats212-alpine)
-	[`nats:2.1.2-alpine3.10`](#nats212-alpine310)
-	[`nats:2.1.2-linux`](#nats212-linux)
-	[`nats:2.1.2-nanoserver`](#nats212-nanoserver)
-	[`nats:2.1.2-nanoserver-1803`](#nats212-nanoserver-1803)
-	[`nats:2.1.2-nanoserver-1809`](#nats212-nanoserver-1809)
-	[`nats:2.1.2-scratch`](#nats212-scratch)
-	[`nats:2.1.2-windowsservercore`](#nats212-windowsservercore)
-	[`nats:2.1.2-windowsservercore-1803`](#nats212-windowsservercore-1803)
-	[`nats:2.1.2-windowsservercore-1809`](#nats212-windowsservercore-1809)
-	[`nats:2.1.2-windowsservercore-ltsc2016`](#nats212-windowsservercore-ltsc2016)
-	[`nats:2.1-alpine`](#nats21-alpine)
-	[`nats:2.1-alpine3.10`](#nats21-alpine310)
-	[`nats:2.1-linux`](#nats21-linux)
-	[`nats:2.1-nanoserver`](#nats21-nanoserver)
-	[`nats:2.1-nanoserver-1803`](#nats21-nanoserver-1803)
-	[`nats:2.1-nanoserver-1809`](#nats21-nanoserver-1809)
-	[`nats:2.1-scratch`](#nats21-scratch)
-	[`nats:2.1-windowsservercore`](#nats21-windowsservercore)
-	[`nats:2.1-windowsservercore-1803`](#nats21-windowsservercore-1803)
-	[`nats:2.1-windowsservercore-1809`](#nats21-windowsservercore-1809)
-	[`nats:2.1-windowsservercore-ltsc2016`](#nats21-windowsservercore-ltsc2016)
-	[`nats:2-alpine`](#nats2-alpine)
-	[`nats:2-alpine3.10`](#nats2-alpine310)
-	[`nats:2-linux`](#nats2-linux)
-	[`nats:2-nanoserver`](#nats2-nanoserver)
-	[`nats:2-nanoserver-1803`](#nats2-nanoserver-1803)
-	[`nats:2-nanoserver-1809`](#nats2-nanoserver-1809)
-	[`nats:2-scratch`](#nats2-scratch)
-	[`nats:2-windowsservercore`](#nats2-windowsservercore)
-	[`nats:2-windowsservercore-1803`](#nats2-windowsservercore-1803)
-	[`nats:2-windowsservercore-1809`](#nats2-windowsservercore-1809)
-	[`nats:2-windowsservercore-ltsc2016`](#nats2-windowsservercore-ltsc2016)
-	[`nats:alpine`](#natsalpine)
-	[`nats:alpine3.10`](#natsalpine310)
-	[`nats:latest`](#natslatest)
-	[`nats:linux`](#natslinux)
-	[`nats:nanoserver`](#natsnanoserver)
-	[`nats:nanoserver-1803`](#natsnanoserver-1803)
-	[`nats:nanoserver-1809`](#natsnanoserver-1809)
-	[`nats:scratch`](#natsscratch)
-	[`nats:windowsservercore`](#natswindowsservercore)
-	[`nats:windowsservercore-1803`](#natswindowsservercore-1803)
-	[`nats:windowsservercore-1809`](#natswindowsservercore-1809)
-	[`nats:windowsservercore-ltsc2016`](#natswindowsservercore-ltsc2016)

## `nats:2`

```console
$ docker pull nats@sha256:53bb39638aa9d14460f6532db6863cd9ded675219b3b9dce3b63ce61276a6d05
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.973; amd64
	-	windows version 10.0.17134.1246; amd64

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:8139c5bf4df6e8635cb3420d2dfab08ecdf75b8d16cd82c40a67bd4417b2e71c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (4002673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49014ccb53efc06dc1ce6656aea0abf000881d9db3ac5b31c6f8aef934452b30`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Nov 2019 01:14:07 GMT
COPY file:f7ba6139c8151888be538812698c1aab4311e97fcfac3b5af13138cd7d7e1405 in /nats-server 
# Wed, 20 Nov 2019 01:14:07 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 20 Nov 2019 01:14:08 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Nov 2019 01:14:08 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Nov 2019 01:14:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f3c8f35bd9bcd03ff8eba7551a59aa4fb56c5eabac4758b0b6cb12709785f25c`  
		Last Modified: Wed, 20 Nov 2019 01:14:44 GMT  
		Size: 4.0 MB (4002195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba25f2430b4efc5a2c8e36c142c7aca0b9a14a6caf16fe09d29f97f77f4efce`  
		Last Modified: Wed, 20 Nov 2019 01:14:43 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:234935205b93b7c99b67d82fe35226290aa302e2b35b32f7f9516aa770bf6003
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3790304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66f838f1a59cd8673948823057d50b486bb443ce5318e5a24502ded16334feda`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Nov 2019 00:04:38 GMT
COPY file:1c509c11a9e5697ac3184dd6c0dca46386d2a5d22fabbd0f4898bad8342884d8 in /nats-server 
# Wed, 20 Nov 2019 00:04:39 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 20 Nov 2019 00:04:39 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Nov 2019 00:04:40 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Nov 2019 00:04:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ab4822bfc4bb3725c051563099752bf9f3cc14db9a698a66f64c906201e88b2d`  
		Last Modified: Wed, 20 Nov 2019 00:05:19 GMT  
		Size: 3.8 MB (3789828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd9cf11d4796d35bb8140733b85f1398c199c592ad417cb6d22eac97b0ac377`  
		Last Modified: Wed, 20 Nov 2019 00:05:18 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:92ea09078a55fc56a807ede1630a862d4b6acc12633391a5a42b41483c6b66fa
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3786713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df9b97d154301cbefd42558306e1ece9667269fb9bda4c0ff2c2f601b578c2c8`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Nov 2019 00:53:13 GMT
COPY file:f7bd56432332a04229b22e2b4ed52b31e5ba863bb47a2aacf6d808bd4a8397d1 in /nats-server 
# Wed, 20 Nov 2019 00:53:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 20 Nov 2019 00:53:15 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Nov 2019 00:53:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Nov 2019 00:53:19 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:27216bfb43f9e231372de919d3bbc108e604422a1019a0b0407001997c0575fe`  
		Last Modified: Wed, 20 Nov 2019 00:54:09 GMT  
		Size: 3.8 MB (3786237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3750c7c4312b8b2af995298314a15791a97ce1ef156b81c0477e579fb42b7f2e`  
		Last Modified: Wed, 20 Nov 2019 00:54:09 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:284c4850adc39c33100ab1324dbe23ddde7450c6e5bd15da874d459e68e0ea3e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3665772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeda44c76561e9490c8a19cffd362e26a5552c3aafd41c98b9562a6ae8a01874`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 20 Sep 2019 23:29:17 GMT
COPY file:f0dce6fb207b92a78774313458c6030a8ac0653785d2a2d54e8b5c8935d9b6b8 in /nats-server 
# Fri, 18 Oct 2019 18:04:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 18 Oct 2019 18:04:47 GMT
EXPOSE 4222 6222 8222
# Fri, 18 Oct 2019 18:04:48 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 18 Oct 2019 18:04:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:98fcb931241702ef0a04aa16bb1e4bab6b8afd06f792790462dff69dee05835c`  
		Last Modified: Fri, 20 Sep 2019 23:29:32 GMT  
		Size: 3.7 MB (3665294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e761cba9328047725686c1ed6eecd9eeef33879d348aea70fb3d219b546165`  
		Last Modified: Fri, 18 Oct 2019 18:05:08 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.973; amd64

```console
$ docker pull nats@sha256:fe1ec52862c24ed520cc33ba713ca2a1ab61132fe67f8e4271dd3d54739175bf
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105047963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d2592fd645781c520143281ac28e8f8eba6f4184b893dd1f41c47f4cfea6e22`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 04 Jan 2020 07:17:17 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jan 2020 17:50:29 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:50:31 GMT
RUN cmd /S /C #(nop) COPY file:a9e3f6c9790c912d513d2134dc1f68e02a9edf34862dd584010eae5ab8418108 in C:\nats-server.exe 
# Wed, 15 Jan 2020 17:50:33 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:50:34 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:50:36 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:50:37 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ee446884f7bef76f8275c2f16add1c4fb598bea2ba861e72bce8fb4aac9b55ef`  
		Size: 101.1 MB (101054324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95d31e7189792498b758db35ae56b1ca97128d8063404cbe62a32205d08d1d4a`  
		Last Modified: Wed, 15 Jan 2020 17:54:30 GMT  
		Size: 940.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06dd0cb87c9a67456f9c940ed213536b3e08acb7279b65835e3c65a7654d86f3`  
		Last Modified: Wed, 15 Jan 2020 17:54:30 GMT  
		Size: 4.0 MB (3988335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a3fd5110f7e9b5b9bdf1dcaa1d44324372e6327142443cd9886d09870d8897e`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 1.6 KB (1560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc491f53dd9a291eef7348c3086782cb45ddb7d249aa3fcd080d0dcc05dc8000`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 939.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8053efdd66e716af07b38c62c28b0878f99af0173a9360e403074367593dcc1`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 942.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3215e4233ac1a2ec100e0e6d20af8633eebf5fce1e5813077fdbab6deb27fbb`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17134.1246; amd64

```console
$ docker pull nats@sha256:5f107d9f832b82ff068741b598503279a5c98f7239c376ba43f9e9e63eb46e9a
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.9 MB (157902423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b01104ee474980123a7757c086644468acfb2f4883fb483597c3db674d4181a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 11 Apr 2018 22:12:30 GMT
RUN Apply image 1803-RTM-amd64
# Wed, 08 Jan 2020 15:12:42 GMT
RUN Install update 1803-amd64
# Wed, 15 Jan 2020 17:46:46 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:46:49 GMT
RUN cmd /S /C #(nop) COPY file:a9e3f6c9790c912d513d2134dc1f68e02a9edf34862dd584010eae5ab8418108 in C:\nats-server.exe 
# Wed, 15 Jan 2020 17:46:50 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:46:52 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:46:53 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:46:54 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e46172273a4e4384e1eec7fb01091c828a256ea0f87b30f61381fba9bc511371`  
		Last Modified: Mon, 17 Sep 2018 20:23:30 GMT  
		Size: 92.8 MB (92818888 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c0783c3b88b74a9de609bda64fc01cd5e23fb65d57e750a9c584e8a9ed842fa9`  
		Size: 61.1 MB (61089912 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:24f456fbaddb9e6d59a1ebc9e9244a4b7b003b467f4379a121463c469fe5ac34`  
		Last Modified: Wed, 15 Jan 2020 17:53:01 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2280cf6b56b3522c9f82db3208ab840d8e3292ec7d042eb1d7d4c00319b640`  
		Last Modified: Wed, 15 Jan 2020 17:53:01 GMT  
		Size: 4.0 MB (3988299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c0024dc7e88bada373f0f9593d8ca873d955ddef73363bd42f421f37a339598`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 1.6 KB (1555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d6c860f0094966bd95e3a9b933773c4aa19466f9b337f383aa138b5b41ab22`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15569096640ccf86ed6b731f1e8ecac13947a7bfe4fdaa0b9800f7484bb266c4`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 951.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c849d8e8a6767e0308da9ac7027ca2eecb68424c8d4d748989768b7f920283`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1`

```console
$ docker pull nats@sha256:53bb39638aa9d14460f6532db6863cd9ded675219b3b9dce3b63ce61276a6d05
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.973; amd64
	-	windows version 10.0.17134.1246; amd64

### `nats:2.1` - linux; amd64

```console
$ docker pull nats@sha256:8139c5bf4df6e8635cb3420d2dfab08ecdf75b8d16cd82c40a67bd4417b2e71c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (4002673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49014ccb53efc06dc1ce6656aea0abf000881d9db3ac5b31c6f8aef934452b30`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Nov 2019 01:14:07 GMT
COPY file:f7ba6139c8151888be538812698c1aab4311e97fcfac3b5af13138cd7d7e1405 in /nats-server 
# Wed, 20 Nov 2019 01:14:07 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 20 Nov 2019 01:14:08 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Nov 2019 01:14:08 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Nov 2019 01:14:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f3c8f35bd9bcd03ff8eba7551a59aa4fb56c5eabac4758b0b6cb12709785f25c`  
		Last Modified: Wed, 20 Nov 2019 01:14:44 GMT  
		Size: 4.0 MB (4002195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba25f2430b4efc5a2c8e36c142c7aca0b9a14a6caf16fe09d29f97f77f4efce`  
		Last Modified: Wed, 20 Nov 2019 01:14:43 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1` - linux; arm variant v6

```console
$ docker pull nats@sha256:234935205b93b7c99b67d82fe35226290aa302e2b35b32f7f9516aa770bf6003
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3790304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66f838f1a59cd8673948823057d50b486bb443ce5318e5a24502ded16334feda`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Nov 2019 00:04:38 GMT
COPY file:1c509c11a9e5697ac3184dd6c0dca46386d2a5d22fabbd0f4898bad8342884d8 in /nats-server 
# Wed, 20 Nov 2019 00:04:39 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 20 Nov 2019 00:04:39 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Nov 2019 00:04:40 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Nov 2019 00:04:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ab4822bfc4bb3725c051563099752bf9f3cc14db9a698a66f64c906201e88b2d`  
		Last Modified: Wed, 20 Nov 2019 00:05:19 GMT  
		Size: 3.8 MB (3789828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd9cf11d4796d35bb8140733b85f1398c199c592ad417cb6d22eac97b0ac377`  
		Last Modified: Wed, 20 Nov 2019 00:05:18 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1` - linux; arm variant v7

```console
$ docker pull nats@sha256:92ea09078a55fc56a807ede1630a862d4b6acc12633391a5a42b41483c6b66fa
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3786713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df9b97d154301cbefd42558306e1ece9667269fb9bda4c0ff2c2f601b578c2c8`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Nov 2019 00:53:13 GMT
COPY file:f7bd56432332a04229b22e2b4ed52b31e5ba863bb47a2aacf6d808bd4a8397d1 in /nats-server 
# Wed, 20 Nov 2019 00:53:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 20 Nov 2019 00:53:15 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Nov 2019 00:53:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Nov 2019 00:53:19 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:27216bfb43f9e231372de919d3bbc108e604422a1019a0b0407001997c0575fe`  
		Last Modified: Wed, 20 Nov 2019 00:54:09 GMT  
		Size: 3.8 MB (3786237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3750c7c4312b8b2af995298314a15791a97ce1ef156b81c0477e579fb42b7f2e`  
		Last Modified: Wed, 20 Nov 2019 00:54:09 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:284c4850adc39c33100ab1324dbe23ddde7450c6e5bd15da874d459e68e0ea3e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3665772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeda44c76561e9490c8a19cffd362e26a5552c3aafd41c98b9562a6ae8a01874`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 20 Sep 2019 23:29:17 GMT
COPY file:f0dce6fb207b92a78774313458c6030a8ac0653785d2a2d54e8b5c8935d9b6b8 in /nats-server 
# Fri, 18 Oct 2019 18:04:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 18 Oct 2019 18:04:47 GMT
EXPOSE 4222 6222 8222
# Fri, 18 Oct 2019 18:04:48 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 18 Oct 2019 18:04:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:98fcb931241702ef0a04aa16bb1e4bab6b8afd06f792790462dff69dee05835c`  
		Last Modified: Fri, 20 Sep 2019 23:29:32 GMT  
		Size: 3.7 MB (3665294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e761cba9328047725686c1ed6eecd9eeef33879d348aea70fb3d219b546165`  
		Last Modified: Fri, 18 Oct 2019 18:05:08 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1` - windows version 10.0.17763.973; amd64

```console
$ docker pull nats@sha256:fe1ec52862c24ed520cc33ba713ca2a1ab61132fe67f8e4271dd3d54739175bf
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105047963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d2592fd645781c520143281ac28e8f8eba6f4184b893dd1f41c47f4cfea6e22`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 04 Jan 2020 07:17:17 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jan 2020 17:50:29 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:50:31 GMT
RUN cmd /S /C #(nop) COPY file:a9e3f6c9790c912d513d2134dc1f68e02a9edf34862dd584010eae5ab8418108 in C:\nats-server.exe 
# Wed, 15 Jan 2020 17:50:33 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:50:34 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:50:36 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:50:37 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ee446884f7bef76f8275c2f16add1c4fb598bea2ba861e72bce8fb4aac9b55ef`  
		Size: 101.1 MB (101054324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95d31e7189792498b758db35ae56b1ca97128d8063404cbe62a32205d08d1d4a`  
		Last Modified: Wed, 15 Jan 2020 17:54:30 GMT  
		Size: 940.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06dd0cb87c9a67456f9c940ed213536b3e08acb7279b65835e3c65a7654d86f3`  
		Last Modified: Wed, 15 Jan 2020 17:54:30 GMT  
		Size: 4.0 MB (3988335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a3fd5110f7e9b5b9bdf1dcaa1d44324372e6327142443cd9886d09870d8897e`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 1.6 KB (1560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc491f53dd9a291eef7348c3086782cb45ddb7d249aa3fcd080d0dcc05dc8000`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 939.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8053efdd66e716af07b38c62c28b0878f99af0173a9360e403074367593dcc1`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 942.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3215e4233ac1a2ec100e0e6d20af8633eebf5fce1e5813077fdbab6deb27fbb`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1` - windows version 10.0.17134.1246; amd64

```console
$ docker pull nats@sha256:5f107d9f832b82ff068741b598503279a5c98f7239c376ba43f9e9e63eb46e9a
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.9 MB (157902423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b01104ee474980123a7757c086644468acfb2f4883fb483597c3db674d4181a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 11 Apr 2018 22:12:30 GMT
RUN Apply image 1803-RTM-amd64
# Wed, 08 Jan 2020 15:12:42 GMT
RUN Install update 1803-amd64
# Wed, 15 Jan 2020 17:46:46 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:46:49 GMT
RUN cmd /S /C #(nop) COPY file:a9e3f6c9790c912d513d2134dc1f68e02a9edf34862dd584010eae5ab8418108 in C:\nats-server.exe 
# Wed, 15 Jan 2020 17:46:50 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:46:52 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:46:53 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:46:54 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e46172273a4e4384e1eec7fb01091c828a256ea0f87b30f61381fba9bc511371`  
		Last Modified: Mon, 17 Sep 2018 20:23:30 GMT  
		Size: 92.8 MB (92818888 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c0783c3b88b74a9de609bda64fc01cd5e23fb65d57e750a9c584e8a9ed842fa9`  
		Size: 61.1 MB (61089912 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:24f456fbaddb9e6d59a1ebc9e9244a4b7b003b467f4379a121463c469fe5ac34`  
		Last Modified: Wed, 15 Jan 2020 17:53:01 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2280cf6b56b3522c9f82db3208ab840d8e3292ec7d042eb1d7d4c00319b640`  
		Last Modified: Wed, 15 Jan 2020 17:53:01 GMT  
		Size: 4.0 MB (3988299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c0024dc7e88bada373f0f9593d8ca873d955ddef73363bd42f421f37a339598`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 1.6 KB (1555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d6c860f0094966bd95e3a9b933773c4aa19466f9b337f383aa138b5b41ab22`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15569096640ccf86ed6b731f1e8ecac13947a7bfe4fdaa0b9800f7484bb266c4`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 951.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c849d8e8a6767e0308da9ac7027ca2eecb68424c8d4d748989768b7f920283`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.2`

```console
$ docker pull nats@sha256:22c95dc23b2e59c92666f3288ea367745f0225e0e029efc334ee15daa33815fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	windows version 10.0.17763.973; amd64
	-	windows version 10.0.17134.1246; amd64

### `nats:2.1.2` - linux; amd64

```console
$ docker pull nats@sha256:8139c5bf4df6e8635cb3420d2dfab08ecdf75b8d16cd82c40a67bd4417b2e71c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (4002673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49014ccb53efc06dc1ce6656aea0abf000881d9db3ac5b31c6f8aef934452b30`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Nov 2019 01:14:07 GMT
COPY file:f7ba6139c8151888be538812698c1aab4311e97fcfac3b5af13138cd7d7e1405 in /nats-server 
# Wed, 20 Nov 2019 01:14:07 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 20 Nov 2019 01:14:08 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Nov 2019 01:14:08 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Nov 2019 01:14:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f3c8f35bd9bcd03ff8eba7551a59aa4fb56c5eabac4758b0b6cb12709785f25c`  
		Last Modified: Wed, 20 Nov 2019 01:14:44 GMT  
		Size: 4.0 MB (4002195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba25f2430b4efc5a2c8e36c142c7aca0b9a14a6caf16fe09d29f97f77f4efce`  
		Last Modified: Wed, 20 Nov 2019 01:14:43 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.2` - linux; arm variant v6

```console
$ docker pull nats@sha256:234935205b93b7c99b67d82fe35226290aa302e2b35b32f7f9516aa770bf6003
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3790304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66f838f1a59cd8673948823057d50b486bb443ce5318e5a24502ded16334feda`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Nov 2019 00:04:38 GMT
COPY file:1c509c11a9e5697ac3184dd6c0dca46386d2a5d22fabbd0f4898bad8342884d8 in /nats-server 
# Wed, 20 Nov 2019 00:04:39 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 20 Nov 2019 00:04:39 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Nov 2019 00:04:40 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Nov 2019 00:04:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ab4822bfc4bb3725c051563099752bf9f3cc14db9a698a66f64c906201e88b2d`  
		Last Modified: Wed, 20 Nov 2019 00:05:19 GMT  
		Size: 3.8 MB (3789828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd9cf11d4796d35bb8140733b85f1398c199c592ad417cb6d22eac97b0ac377`  
		Last Modified: Wed, 20 Nov 2019 00:05:18 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.2` - linux; arm variant v7

```console
$ docker pull nats@sha256:92ea09078a55fc56a807ede1630a862d4b6acc12633391a5a42b41483c6b66fa
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3786713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df9b97d154301cbefd42558306e1ece9667269fb9bda4c0ff2c2f601b578c2c8`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Nov 2019 00:53:13 GMT
COPY file:f7bd56432332a04229b22e2b4ed52b31e5ba863bb47a2aacf6d808bd4a8397d1 in /nats-server 
# Wed, 20 Nov 2019 00:53:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 20 Nov 2019 00:53:15 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Nov 2019 00:53:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Nov 2019 00:53:19 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:27216bfb43f9e231372de919d3bbc108e604422a1019a0b0407001997c0575fe`  
		Last Modified: Wed, 20 Nov 2019 00:54:09 GMT  
		Size: 3.8 MB (3786237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3750c7c4312b8b2af995298314a15791a97ce1ef156b81c0477e579fb42b7f2e`  
		Last Modified: Wed, 20 Nov 2019 00:54:09 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.2` - windows version 10.0.17763.973; amd64

```console
$ docker pull nats@sha256:fe1ec52862c24ed520cc33ba713ca2a1ab61132fe67f8e4271dd3d54739175bf
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105047963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d2592fd645781c520143281ac28e8f8eba6f4184b893dd1f41c47f4cfea6e22`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 04 Jan 2020 07:17:17 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jan 2020 17:50:29 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:50:31 GMT
RUN cmd /S /C #(nop) COPY file:a9e3f6c9790c912d513d2134dc1f68e02a9edf34862dd584010eae5ab8418108 in C:\nats-server.exe 
# Wed, 15 Jan 2020 17:50:33 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:50:34 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:50:36 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:50:37 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ee446884f7bef76f8275c2f16add1c4fb598bea2ba861e72bce8fb4aac9b55ef`  
		Size: 101.1 MB (101054324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95d31e7189792498b758db35ae56b1ca97128d8063404cbe62a32205d08d1d4a`  
		Last Modified: Wed, 15 Jan 2020 17:54:30 GMT  
		Size: 940.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06dd0cb87c9a67456f9c940ed213536b3e08acb7279b65835e3c65a7654d86f3`  
		Last Modified: Wed, 15 Jan 2020 17:54:30 GMT  
		Size: 4.0 MB (3988335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a3fd5110f7e9b5b9bdf1dcaa1d44324372e6327142443cd9886d09870d8897e`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 1.6 KB (1560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc491f53dd9a291eef7348c3086782cb45ddb7d249aa3fcd080d0dcc05dc8000`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 939.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8053efdd66e716af07b38c62c28b0878f99af0173a9360e403074367593dcc1`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 942.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3215e4233ac1a2ec100e0e6d20af8633eebf5fce1e5813077fdbab6deb27fbb`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.2` - windows version 10.0.17134.1246; amd64

```console
$ docker pull nats@sha256:5f107d9f832b82ff068741b598503279a5c98f7239c376ba43f9e9e63eb46e9a
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.9 MB (157902423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b01104ee474980123a7757c086644468acfb2f4883fb483597c3db674d4181a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 11 Apr 2018 22:12:30 GMT
RUN Apply image 1803-RTM-amd64
# Wed, 08 Jan 2020 15:12:42 GMT
RUN Install update 1803-amd64
# Wed, 15 Jan 2020 17:46:46 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:46:49 GMT
RUN cmd /S /C #(nop) COPY file:a9e3f6c9790c912d513d2134dc1f68e02a9edf34862dd584010eae5ab8418108 in C:\nats-server.exe 
# Wed, 15 Jan 2020 17:46:50 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:46:52 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:46:53 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:46:54 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e46172273a4e4384e1eec7fb01091c828a256ea0f87b30f61381fba9bc511371`  
		Last Modified: Mon, 17 Sep 2018 20:23:30 GMT  
		Size: 92.8 MB (92818888 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c0783c3b88b74a9de609bda64fc01cd5e23fb65d57e750a9c584e8a9ed842fa9`  
		Size: 61.1 MB (61089912 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:24f456fbaddb9e6d59a1ebc9e9244a4b7b003b467f4379a121463c469fe5ac34`  
		Last Modified: Wed, 15 Jan 2020 17:53:01 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2280cf6b56b3522c9f82db3208ab840d8e3292ec7d042eb1d7d4c00319b640`  
		Last Modified: Wed, 15 Jan 2020 17:53:01 GMT  
		Size: 4.0 MB (3988299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c0024dc7e88bada373f0f9593d8ca873d955ddef73363bd42f421f37a339598`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 1.6 KB (1555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d6c860f0094966bd95e3a9b933773c4aa19466f9b337f383aa138b5b41ab22`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15569096640ccf86ed6b731f1e8ecac13947a7bfe4fdaa0b9800f7484bb266c4`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 951.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c849d8e8a6767e0308da9ac7027ca2eecb68424c8d4d748989768b7f920283`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.2-alpine`

```console
$ docker pull nats@sha256:71e945d4d94bfc25dfdb242bad666f2979caef77f1bff75728f1cc72b4804081
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats:2.1.2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:f507195794f36c37413ca058f5c3442ad24a80facf94cf4779297e4ab0971f99
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7092803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffa6d536d932527718344a90a884bb621e3480d21893e4bf8e4b7e46b05ad957`
-	Default Command: `["nats-server"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 19:19:25 GMT
ENV NATS_SERVER=2.1.2
# Thu, 23 Jan 2020 19:19:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 23 Jan 2020 19:19:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 23 Jan 2020 19:19:29 GMT
EXPOSE 4222 6222 8222
# Thu, 23 Jan 2020 19:19:29 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581b0b35a07f0a300a55e836a3ba0cb3d18061455a6367a15fbd6f127b57351c`  
		Last Modified: Thu, 23 Jan 2020 19:20:29 GMT  
		Size: 4.3 MB (4305310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82a66d5edde56b04466489c0c46457358c6737789e7e4cde197d7b0befe4fa3`  
		Last Modified: Thu, 23 Jan 2020 19:20:28 GMT  
		Size: 531.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:6380d8b1fc432a021689908f6501d49747edf3b3c2bc54134e433c10e77efb1c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6664521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a20dd366129d9b5428c44f6c6853a8297f7b86b3e6b8f20a1600da467f76599`
-	Default Command: `["nats-server"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:27 GMT
ADD file:2aa80d52585a6b34b2cc5811d46965a084e50cfb8cd183f1a88b2b1bc6556e1f in / 
# Thu, 23 Jan 2020 16:53:28 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:44:32 GMT
ENV NATS_SERVER=2.1.2
# Thu, 23 Jan 2020 17:44:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 23 Jan 2020 17:44:39 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 23 Jan 2020 17:44:40 GMT
EXPOSE 4222 6222 8222
# Thu, 23 Jan 2020 17:44:41 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:896868b7b9168cabb308702db96dc9769d10c23e20fc66f5f4abedf4c75d7642`  
		Last Modified: Thu, 23 Jan 2020 16:54:07 GMT  
		Size: 2.6 MB (2571407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f146c76b464f3790626809adda3914591425f7cd06759a183ccd5da25e26bb82`  
		Last Modified: Thu, 23 Jan 2020 17:45:13 GMT  
		Size: 4.1 MB (4092555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162410de1cd5b2c2ce2cd44dc7973ff2511dc755faeca556ea9e69b1aa55fae3`  
		Last Modified: Thu, 23 Jan 2020 17:45:12 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:d60f1b23e6d2ce2e8edac172e464de946fa830452af16b709c8d3c8234a3c045
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6466632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d154ea04a5c19abf9bcf38dacc8b82bee649c6c507024227c5cd298ed1ac75c6`
-	Default Command: `["nats-server"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:31 GMT
ADD file:d05c9f9143d11d12045d4faef882e5985e6b38fabe52237dd8d8c0627a9620ab in / 
# Thu, 23 Jan 2020 16:53:32 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:55:25 GMT
ENV NATS_SERVER=2.1.2
# Thu, 23 Jan 2020 17:55:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 23 Jan 2020 17:55:30 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 23 Jan 2020 17:55:31 GMT
EXPOSE 4222 6222 8222
# Thu, 23 Jan 2020 17:55:32 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:4e972d957a606327b0b6c2e8aa4a6045c263b7496a536298aaebf690e9d85f1d`  
		Last Modified: Thu, 23 Jan 2020 16:53:59 GMT  
		Size: 2.4 MB (2378408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c375dc9edf38cadcfdc6537707cdea65e2b45d840940712d2f88d19cc967edc6`  
		Last Modified: Thu, 23 Jan 2020 17:56:08 GMT  
		Size: 4.1 MB (4087666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bfcd4ad511455617c2f402e3d5ebd12e714c0d9a0d280f7399735754fab756e`  
		Last Modified: Thu, 23 Jan 2020 17:56:08 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.2-alpine3.10`

```console
$ docker pull nats@sha256:71e945d4d94bfc25dfdb242bad666f2979caef77f1bff75728f1cc72b4804081
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats:2.1.2-alpine3.10` - linux; amd64

```console
$ docker pull nats@sha256:f507195794f36c37413ca058f5c3442ad24a80facf94cf4779297e4ab0971f99
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7092803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffa6d536d932527718344a90a884bb621e3480d21893e4bf8e4b7e46b05ad957`
-	Default Command: `["nats-server"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 19:19:25 GMT
ENV NATS_SERVER=2.1.2
# Thu, 23 Jan 2020 19:19:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 23 Jan 2020 19:19:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 23 Jan 2020 19:19:29 GMT
EXPOSE 4222 6222 8222
# Thu, 23 Jan 2020 19:19:29 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581b0b35a07f0a300a55e836a3ba0cb3d18061455a6367a15fbd6f127b57351c`  
		Last Modified: Thu, 23 Jan 2020 19:20:29 GMT  
		Size: 4.3 MB (4305310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82a66d5edde56b04466489c0c46457358c6737789e7e4cde197d7b0befe4fa3`  
		Last Modified: Thu, 23 Jan 2020 19:20:28 GMT  
		Size: 531.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.2-alpine3.10` - linux; arm variant v6

```console
$ docker pull nats@sha256:6380d8b1fc432a021689908f6501d49747edf3b3c2bc54134e433c10e77efb1c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6664521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a20dd366129d9b5428c44f6c6853a8297f7b86b3e6b8f20a1600da467f76599`
-	Default Command: `["nats-server"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:27 GMT
ADD file:2aa80d52585a6b34b2cc5811d46965a084e50cfb8cd183f1a88b2b1bc6556e1f in / 
# Thu, 23 Jan 2020 16:53:28 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:44:32 GMT
ENV NATS_SERVER=2.1.2
# Thu, 23 Jan 2020 17:44:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 23 Jan 2020 17:44:39 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 23 Jan 2020 17:44:40 GMT
EXPOSE 4222 6222 8222
# Thu, 23 Jan 2020 17:44:41 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:896868b7b9168cabb308702db96dc9769d10c23e20fc66f5f4abedf4c75d7642`  
		Last Modified: Thu, 23 Jan 2020 16:54:07 GMT  
		Size: 2.6 MB (2571407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f146c76b464f3790626809adda3914591425f7cd06759a183ccd5da25e26bb82`  
		Last Modified: Thu, 23 Jan 2020 17:45:13 GMT  
		Size: 4.1 MB (4092555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162410de1cd5b2c2ce2cd44dc7973ff2511dc755faeca556ea9e69b1aa55fae3`  
		Last Modified: Thu, 23 Jan 2020 17:45:12 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.2-alpine3.10` - linux; arm variant v7

```console
$ docker pull nats@sha256:d60f1b23e6d2ce2e8edac172e464de946fa830452af16b709c8d3c8234a3c045
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6466632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d154ea04a5c19abf9bcf38dacc8b82bee649c6c507024227c5cd298ed1ac75c6`
-	Default Command: `["nats-server"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:31 GMT
ADD file:d05c9f9143d11d12045d4faef882e5985e6b38fabe52237dd8d8c0627a9620ab in / 
# Thu, 23 Jan 2020 16:53:32 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:55:25 GMT
ENV NATS_SERVER=2.1.2
# Thu, 23 Jan 2020 17:55:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 23 Jan 2020 17:55:30 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 23 Jan 2020 17:55:31 GMT
EXPOSE 4222 6222 8222
# Thu, 23 Jan 2020 17:55:32 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:4e972d957a606327b0b6c2e8aa4a6045c263b7496a536298aaebf690e9d85f1d`  
		Last Modified: Thu, 23 Jan 2020 16:53:59 GMT  
		Size: 2.4 MB (2378408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c375dc9edf38cadcfdc6537707cdea65e2b45d840940712d2f88d19cc967edc6`  
		Last Modified: Thu, 23 Jan 2020 17:56:08 GMT  
		Size: 4.1 MB (4087666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bfcd4ad511455617c2f402e3d5ebd12e714c0d9a0d280f7399735754fab756e`  
		Last Modified: Thu, 23 Jan 2020 17:56:08 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.2-linux`

```console
$ docker pull nats@sha256:5d778a5f18cfeef52e2e6676b2c6447fb21723e25ed25c65668d00f118b7c2c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats:2.1.2-linux` - linux; amd64

```console
$ docker pull nats@sha256:8139c5bf4df6e8635cb3420d2dfab08ecdf75b8d16cd82c40a67bd4417b2e71c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (4002673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49014ccb53efc06dc1ce6656aea0abf000881d9db3ac5b31c6f8aef934452b30`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Nov 2019 01:14:07 GMT
COPY file:f7ba6139c8151888be538812698c1aab4311e97fcfac3b5af13138cd7d7e1405 in /nats-server 
# Wed, 20 Nov 2019 01:14:07 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 20 Nov 2019 01:14:08 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Nov 2019 01:14:08 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Nov 2019 01:14:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f3c8f35bd9bcd03ff8eba7551a59aa4fb56c5eabac4758b0b6cb12709785f25c`  
		Last Modified: Wed, 20 Nov 2019 01:14:44 GMT  
		Size: 4.0 MB (4002195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba25f2430b4efc5a2c8e36c142c7aca0b9a14a6caf16fe09d29f97f77f4efce`  
		Last Modified: Wed, 20 Nov 2019 01:14:43 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:234935205b93b7c99b67d82fe35226290aa302e2b35b32f7f9516aa770bf6003
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3790304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66f838f1a59cd8673948823057d50b486bb443ce5318e5a24502ded16334feda`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Nov 2019 00:04:38 GMT
COPY file:1c509c11a9e5697ac3184dd6c0dca46386d2a5d22fabbd0f4898bad8342884d8 in /nats-server 
# Wed, 20 Nov 2019 00:04:39 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 20 Nov 2019 00:04:39 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Nov 2019 00:04:40 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Nov 2019 00:04:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ab4822bfc4bb3725c051563099752bf9f3cc14db9a698a66f64c906201e88b2d`  
		Last Modified: Wed, 20 Nov 2019 00:05:19 GMT  
		Size: 3.8 MB (3789828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd9cf11d4796d35bb8140733b85f1398c199c592ad417cb6d22eac97b0ac377`  
		Last Modified: Wed, 20 Nov 2019 00:05:18 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:92ea09078a55fc56a807ede1630a862d4b6acc12633391a5a42b41483c6b66fa
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3786713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df9b97d154301cbefd42558306e1ece9667269fb9bda4c0ff2c2f601b578c2c8`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Nov 2019 00:53:13 GMT
COPY file:f7bd56432332a04229b22e2b4ed52b31e5ba863bb47a2aacf6d808bd4a8397d1 in /nats-server 
# Wed, 20 Nov 2019 00:53:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 20 Nov 2019 00:53:15 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Nov 2019 00:53:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Nov 2019 00:53:19 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:27216bfb43f9e231372de919d3bbc108e604422a1019a0b0407001997c0575fe`  
		Last Modified: Wed, 20 Nov 2019 00:54:09 GMT  
		Size: 3.8 MB (3786237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3750c7c4312b8b2af995298314a15791a97ce1ef156b81c0477e579fb42b7f2e`  
		Last Modified: Wed, 20 Nov 2019 00:54:09 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.2-nanoserver`

```console
$ docker pull nats@sha256:d028e8a1c50120304d4111bb1214475e11f3684b7176df24a5ec7b00f650decb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64
	-	windows version 10.0.17134.1246; amd64

### `nats:2.1.2-nanoserver` - windows version 10.0.17763.973; amd64

```console
$ docker pull nats@sha256:fe1ec52862c24ed520cc33ba713ca2a1ab61132fe67f8e4271dd3d54739175bf
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105047963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d2592fd645781c520143281ac28e8f8eba6f4184b893dd1f41c47f4cfea6e22`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 04 Jan 2020 07:17:17 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jan 2020 17:50:29 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:50:31 GMT
RUN cmd /S /C #(nop) COPY file:a9e3f6c9790c912d513d2134dc1f68e02a9edf34862dd584010eae5ab8418108 in C:\nats-server.exe 
# Wed, 15 Jan 2020 17:50:33 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:50:34 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:50:36 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:50:37 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ee446884f7bef76f8275c2f16add1c4fb598bea2ba861e72bce8fb4aac9b55ef`  
		Size: 101.1 MB (101054324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95d31e7189792498b758db35ae56b1ca97128d8063404cbe62a32205d08d1d4a`  
		Last Modified: Wed, 15 Jan 2020 17:54:30 GMT  
		Size: 940.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06dd0cb87c9a67456f9c940ed213536b3e08acb7279b65835e3c65a7654d86f3`  
		Last Modified: Wed, 15 Jan 2020 17:54:30 GMT  
		Size: 4.0 MB (3988335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a3fd5110f7e9b5b9bdf1dcaa1d44324372e6327142443cd9886d09870d8897e`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 1.6 KB (1560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc491f53dd9a291eef7348c3086782cb45ddb7d249aa3fcd080d0dcc05dc8000`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 939.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8053efdd66e716af07b38c62c28b0878f99af0173a9360e403074367593dcc1`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 942.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3215e4233ac1a2ec100e0e6d20af8633eebf5fce1e5813077fdbab6deb27fbb`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.2-nanoserver` - windows version 10.0.17134.1246; amd64

```console
$ docker pull nats@sha256:5f107d9f832b82ff068741b598503279a5c98f7239c376ba43f9e9e63eb46e9a
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.9 MB (157902423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b01104ee474980123a7757c086644468acfb2f4883fb483597c3db674d4181a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 11 Apr 2018 22:12:30 GMT
RUN Apply image 1803-RTM-amd64
# Wed, 08 Jan 2020 15:12:42 GMT
RUN Install update 1803-amd64
# Wed, 15 Jan 2020 17:46:46 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:46:49 GMT
RUN cmd /S /C #(nop) COPY file:a9e3f6c9790c912d513d2134dc1f68e02a9edf34862dd584010eae5ab8418108 in C:\nats-server.exe 
# Wed, 15 Jan 2020 17:46:50 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:46:52 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:46:53 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:46:54 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e46172273a4e4384e1eec7fb01091c828a256ea0f87b30f61381fba9bc511371`  
		Last Modified: Mon, 17 Sep 2018 20:23:30 GMT  
		Size: 92.8 MB (92818888 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c0783c3b88b74a9de609bda64fc01cd5e23fb65d57e750a9c584e8a9ed842fa9`  
		Size: 61.1 MB (61089912 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:24f456fbaddb9e6d59a1ebc9e9244a4b7b003b467f4379a121463c469fe5ac34`  
		Last Modified: Wed, 15 Jan 2020 17:53:01 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2280cf6b56b3522c9f82db3208ab840d8e3292ec7d042eb1d7d4c00319b640`  
		Last Modified: Wed, 15 Jan 2020 17:53:01 GMT  
		Size: 4.0 MB (3988299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c0024dc7e88bada373f0f9593d8ca873d955ddef73363bd42f421f37a339598`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 1.6 KB (1555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d6c860f0094966bd95e3a9b933773c4aa19466f9b337f383aa138b5b41ab22`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15569096640ccf86ed6b731f1e8ecac13947a7bfe4fdaa0b9800f7484bb266c4`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 951.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c849d8e8a6767e0308da9ac7027ca2eecb68424c8d4d748989768b7f920283`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.2-nanoserver-1803`

```console
$ docker pull nats@sha256:9c4a8412f1acfb6279840bdb68e678c0e848b259196fecef0d4ea62c120654c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17134.1246; amd64

### `nats:2.1.2-nanoserver-1803` - windows version 10.0.17134.1246; amd64

```console
$ docker pull nats@sha256:5f107d9f832b82ff068741b598503279a5c98f7239c376ba43f9e9e63eb46e9a
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.9 MB (157902423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b01104ee474980123a7757c086644468acfb2f4883fb483597c3db674d4181a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 11 Apr 2018 22:12:30 GMT
RUN Apply image 1803-RTM-amd64
# Wed, 08 Jan 2020 15:12:42 GMT
RUN Install update 1803-amd64
# Wed, 15 Jan 2020 17:46:46 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:46:49 GMT
RUN cmd /S /C #(nop) COPY file:a9e3f6c9790c912d513d2134dc1f68e02a9edf34862dd584010eae5ab8418108 in C:\nats-server.exe 
# Wed, 15 Jan 2020 17:46:50 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:46:52 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:46:53 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:46:54 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e46172273a4e4384e1eec7fb01091c828a256ea0f87b30f61381fba9bc511371`  
		Last Modified: Mon, 17 Sep 2018 20:23:30 GMT  
		Size: 92.8 MB (92818888 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c0783c3b88b74a9de609bda64fc01cd5e23fb65d57e750a9c584e8a9ed842fa9`  
		Size: 61.1 MB (61089912 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:24f456fbaddb9e6d59a1ebc9e9244a4b7b003b467f4379a121463c469fe5ac34`  
		Last Modified: Wed, 15 Jan 2020 17:53:01 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2280cf6b56b3522c9f82db3208ab840d8e3292ec7d042eb1d7d4c00319b640`  
		Last Modified: Wed, 15 Jan 2020 17:53:01 GMT  
		Size: 4.0 MB (3988299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c0024dc7e88bada373f0f9593d8ca873d955ddef73363bd42f421f37a339598`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 1.6 KB (1555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d6c860f0094966bd95e3a9b933773c4aa19466f9b337f383aa138b5b41ab22`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15569096640ccf86ed6b731f1e8ecac13947a7bfe4fdaa0b9800f7484bb266c4`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 951.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c849d8e8a6767e0308da9ac7027ca2eecb68424c8d4d748989768b7f920283`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.2-nanoserver-1809`

```console
$ docker pull nats@sha256:35356d98d96477f83eab4060656843a014506567dc5ad5c2acea557bd05c69b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64

### `nats:2.1.2-nanoserver-1809` - windows version 10.0.17763.973; amd64

```console
$ docker pull nats@sha256:fe1ec52862c24ed520cc33ba713ca2a1ab61132fe67f8e4271dd3d54739175bf
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105047963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d2592fd645781c520143281ac28e8f8eba6f4184b893dd1f41c47f4cfea6e22`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 04 Jan 2020 07:17:17 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jan 2020 17:50:29 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:50:31 GMT
RUN cmd /S /C #(nop) COPY file:a9e3f6c9790c912d513d2134dc1f68e02a9edf34862dd584010eae5ab8418108 in C:\nats-server.exe 
# Wed, 15 Jan 2020 17:50:33 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:50:34 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:50:36 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:50:37 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ee446884f7bef76f8275c2f16add1c4fb598bea2ba861e72bce8fb4aac9b55ef`  
		Size: 101.1 MB (101054324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95d31e7189792498b758db35ae56b1ca97128d8063404cbe62a32205d08d1d4a`  
		Last Modified: Wed, 15 Jan 2020 17:54:30 GMT  
		Size: 940.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06dd0cb87c9a67456f9c940ed213536b3e08acb7279b65835e3c65a7654d86f3`  
		Last Modified: Wed, 15 Jan 2020 17:54:30 GMT  
		Size: 4.0 MB (3988335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a3fd5110f7e9b5b9bdf1dcaa1d44324372e6327142443cd9886d09870d8897e`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 1.6 KB (1560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc491f53dd9a291eef7348c3086782cb45ddb7d249aa3fcd080d0dcc05dc8000`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 939.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8053efdd66e716af07b38c62c28b0878f99af0173a9360e403074367593dcc1`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 942.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3215e4233ac1a2ec100e0e6d20af8633eebf5fce1e5813077fdbab6deb27fbb`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.2-scratch`

```console
$ docker pull nats@sha256:5d778a5f18cfeef52e2e6676b2c6447fb21723e25ed25c65668d00f118b7c2c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats:2.1.2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:8139c5bf4df6e8635cb3420d2dfab08ecdf75b8d16cd82c40a67bd4417b2e71c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (4002673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49014ccb53efc06dc1ce6656aea0abf000881d9db3ac5b31c6f8aef934452b30`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Nov 2019 01:14:07 GMT
COPY file:f7ba6139c8151888be538812698c1aab4311e97fcfac3b5af13138cd7d7e1405 in /nats-server 
# Wed, 20 Nov 2019 01:14:07 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 20 Nov 2019 01:14:08 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Nov 2019 01:14:08 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Nov 2019 01:14:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f3c8f35bd9bcd03ff8eba7551a59aa4fb56c5eabac4758b0b6cb12709785f25c`  
		Last Modified: Wed, 20 Nov 2019 01:14:44 GMT  
		Size: 4.0 MB (4002195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba25f2430b4efc5a2c8e36c142c7aca0b9a14a6caf16fe09d29f97f77f4efce`  
		Last Modified: Wed, 20 Nov 2019 01:14:43 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:234935205b93b7c99b67d82fe35226290aa302e2b35b32f7f9516aa770bf6003
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3790304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66f838f1a59cd8673948823057d50b486bb443ce5318e5a24502ded16334feda`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Nov 2019 00:04:38 GMT
COPY file:1c509c11a9e5697ac3184dd6c0dca46386d2a5d22fabbd0f4898bad8342884d8 in /nats-server 
# Wed, 20 Nov 2019 00:04:39 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 20 Nov 2019 00:04:39 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Nov 2019 00:04:40 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Nov 2019 00:04:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ab4822bfc4bb3725c051563099752bf9f3cc14db9a698a66f64c906201e88b2d`  
		Last Modified: Wed, 20 Nov 2019 00:05:19 GMT  
		Size: 3.8 MB (3789828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd9cf11d4796d35bb8140733b85f1398c199c592ad417cb6d22eac97b0ac377`  
		Last Modified: Wed, 20 Nov 2019 00:05:18 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:92ea09078a55fc56a807ede1630a862d4b6acc12633391a5a42b41483c6b66fa
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3786713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df9b97d154301cbefd42558306e1ece9667269fb9bda4c0ff2c2f601b578c2c8`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Nov 2019 00:53:13 GMT
COPY file:f7bd56432332a04229b22e2b4ed52b31e5ba863bb47a2aacf6d808bd4a8397d1 in /nats-server 
# Wed, 20 Nov 2019 00:53:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 20 Nov 2019 00:53:15 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Nov 2019 00:53:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Nov 2019 00:53:19 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:27216bfb43f9e231372de919d3bbc108e604422a1019a0b0407001997c0575fe`  
		Last Modified: Wed, 20 Nov 2019 00:54:09 GMT  
		Size: 3.8 MB (3786237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3750c7c4312b8b2af995298314a15791a97ce1ef156b81c0477e579fb42b7f2e`  
		Last Modified: Wed, 20 Nov 2019 00:54:09 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.2-windowsservercore`

```console
$ docker pull nats@sha256:a42f0c67634d642f56a78fcc79c12b8d5d4da81b34b93f1ccb103ba2743f6e23
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64
	-	windows version 10.0.17134.1246; amd64
	-	windows version 10.0.14393.3443; amd64

### `nats:2.1.2-windowsservercore` - windows version 10.0.17763.973; amd64

```console
$ docker pull nats@sha256:f5ac96a023326f836cf1c02a5f5b30abd128056d648cac3a4643c8125532ec4f
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2230470888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66ed94808574b78075af126587ee0e95fd33c3b8964fbec51c76c08c20bba3d6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Wed, 15 Jan 2020 14:40:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jan 2020 17:41:54 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:41:55 GMT
ENV NATS_SERVER=2.1.2
# Wed, 15 Jan 2020 17:41:56 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.2/nats-server-v2.1.2-windows-amd64.zip
# Wed, 15 Jan 2020 17:42:38 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jan 2020 17:43:46 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Jan 2020 17:43:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:43:49 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:43:50 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:43:52 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2397868e5c7aa285f662aaa9309fa4756277739e11d589a663a204df80595f2c`  
		Last Modified: Wed, 15 Jan 2020 17:10:53 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b23c268ec0520ea9af1e83b69008728041b2a5f234937b9a6272d2a739fd92e`  
		Last Modified: Wed, 15 Jan 2020 17:51:25 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8bf81f9ddd524bd8d7611b92b362a8f558a338e038fb1a81f81872f58a76f7`  
		Last Modified: Wed, 15 Jan 2020 17:51:25 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb3c94fff5bd229bc976399c1904de65b246152cd41d0147af159fd09877822a`  
		Last Modified: Wed, 15 Jan 2020 17:51:24 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e70dcd5f51d264f2ff2ba291ee37e474f5637d236d01c2d5cd8a4ab039dc60`  
		Last Modified: Wed, 15 Jan 2020 17:51:26 GMT  
		Size: 4.5 MB (4548759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b87189fe10fd6d476acc4c0869463fe1f0d813aa1fc2ff3d95efa65f86d7f34`  
		Last Modified: Wed, 15 Jan 2020 17:51:31 GMT  
		Size: 8.5 MB (8500806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a611e13685ceef48268051590fc9cc976fdec2ec0968e3a12fb9b7ef72b6f2`  
		Last Modified: Wed, 15 Jan 2020 17:51:22 GMT  
		Size: 1.8 KB (1763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ebd020bd73cd69b61c2325da491f4c057f7fdeac1f37db60365aef9d9f56e6`  
		Last Modified: Wed, 15 Jan 2020 17:51:22 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2ef97f255816c764614a7a10afa9fa89f6b8fa9c107f24458eab08ad8aee6d`  
		Last Modified: Wed, 15 Jan 2020 17:51:22 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d555934698e4f3eaa1e7fef777b3692d4a519ec978ec5f191be9ea1a772ad6`  
		Last Modified: Wed, 15 Jan 2020 17:51:22 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.2-windowsservercore` - windows version 10.0.17134.1246; amd64

```console
$ docker pull nats@sha256:68c9dff50987d82ca20958b1a5ca7cb816509b6d6b024ecc0a5f83cfe26f5f59
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2368141200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20f6b32275bca4375a3ca4b65ab024126e7ae1c30725dcd7ab47d638bc9c5dbc`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 12 Apr 2018 09:20:54 GMT
RUN Apply image 1803-RTM-amd64
# Wed, 08 Jan 2020 15:30:02 GMT
RUN Install update 1803-amd64
# Wed, 15 Jan 2020 17:44:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jan 2020 17:44:14 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:44:15 GMT
ENV NATS_SERVER=2.1.2
# Wed, 15 Jan 2020 17:44:16 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.2/nats-server-v2.1.2-windows-amd64.zip
# Wed, 15 Jan 2020 17:45:13 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jan 2020 17:46:20 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Jan 2020 17:46:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:46:22 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:46:24 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:46:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d9e8b01179bfc94a5bdb1810fbd76b999aa52016001ace2d3a4c4bc7065a9601`  
		Last Modified: Tue, 18 Sep 2018 22:43:55 GMT  
		Size: 1.7 GB (1659688273 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:270ec3ad3fc7d52c0dd086b32f7751131c799e25cdcd4686cc33cbf2b607c34e`  
		Size: 699.2 MB (699246147 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dbec356e813f8f1863318efd5cd62c261f7de4ac49fc093c648020e26d0520fb`  
		Last Modified: Wed, 15 Jan 2020 17:52:17 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c748a716adbca27bf760bc535221171b42c3dcfd044a49e011295928c66c39`  
		Last Modified: Wed, 15 Jan 2020 17:52:17 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7efb3710bacce94103ccc92d28b0a0af30a9bb7a29f1d7f45fc18a75e959ee2d`  
		Last Modified: Wed, 15 Jan 2020 17:52:16 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883bd0fc138e4a17c679bf7d23bb5f0186ccae58fbacdfda29c147e85e2d9383`  
		Last Modified: Wed, 15 Jan 2020 17:52:15 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967451731bebacb830dc7e26892242d8d5c55f6576f5476820313ac2f35d2550`  
		Last Modified: Wed, 15 Jan 2020 17:52:17 GMT  
		Size: 4.9 MB (4880651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35062fb2b37da05d5d753b6519295e3b14da0bf8fecf57ba90fb507aaf498b7`  
		Last Modified: Wed, 15 Jan 2020 17:52:15 GMT  
		Size: 4.3 MB (4316097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bcb4b1ca97cf159a8a5030f29505c9c52626907a92244c92d25df16333f84bf`  
		Last Modified: Wed, 15 Jan 2020 17:52:13 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a380672454ff5ba95dd36413220fa3f00b7998578a8f32ee0b85cfd6d6f9666`  
		Last Modified: Wed, 15 Jan 2020 17:52:13 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f545bb1274ec20783b4966e6592ba3ca21b327f02552a0480c57eae7bd6a77`  
		Last Modified: Wed, 15 Jan 2020 17:52:13 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29eea8dff9fd0ad0a6c1d9943b993b4519c8d7c48140eeb20de7f46fe018e764`  
		Last Modified: Wed, 15 Jan 2020 17:52:13 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.2-windowsservercore` - windows version 10.0.14393.3443; amd64

```console
$ docker pull nats@sha256:f3b8aa519f1e9981b369d238e46b3e336b2df7654f7cf784b5601d5342a49137
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 GB (5739369423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56ca53177d88b1126a979fb5530e66d83974e1838cecce90ade826949f5ea259`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 02 Jan 2020 15:48:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Jan 2020 15:20:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jan 2020 17:47:08 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:47:10 GMT
ENV NATS_SERVER=2.1.2
# Wed, 15 Jan 2020 17:47:11 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.2/nats-server-v2.1.2-windows-amd64.zip
# Wed, 15 Jan 2020 17:48:21 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jan 2020 17:50:09 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Jan 2020 17:50:10 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:50:12 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:50:14 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:50:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31f9df80631e7b5d379647ee7701ff50e009bd2c03b30a67a0a8e7bba4a26f94`  
		Size: 1.7 GB (1654613376 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:43da502775fb34b738d9f908cb549c2825c04f1451d1039ec99749be127e47ef`  
		Last Modified: Wed, 15 Jan 2020 17:12:02 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6771e606bb5340710c7ec7fa3294903a0a1f901e5c1e79211ee54fc1f074179a`  
		Last Modified: Wed, 15 Jan 2020 17:53:47 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8885516d0bc2df9c7e82fe0aeb847bc83415084fe85a9aed26a03b3b56ae7c`  
		Last Modified: Wed, 15 Jan 2020 17:53:46 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68459b3a704ec7e5908e23d0d52576c68eef20a4b3ede7bf88ec4e3b2321d170`  
		Last Modified: Wed, 15 Jan 2020 17:53:46 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196e19f93e85979cb0240edd67162a54a2e716e7b139c9c7a99882b3dc42fc2a`  
		Last Modified: Wed, 15 Jan 2020 17:53:47 GMT  
		Size: 5.4 MB (5383420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2ec8ad5670f9274bd1b0dbc71a9ac551d4b18d3f6254bf51bbd80049d7d9c2`  
		Last Modified: Wed, 15 Jan 2020 17:53:46 GMT  
		Size: 9.4 MB (9376638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4abd28582063a6691f03037049db18ea066600d7023aa3d2975eb66ea3cafd`  
		Last Modified: Wed, 15 Jan 2020 17:53:43 GMT  
		Size: 1.8 KB (1762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe6eef99ce520e46eef3031fa6ebd7aeba735253cef9dd2b4e7e07255a9efd8`  
		Last Modified: Wed, 15 Jan 2020 17:53:43 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb11317f8d70c8d41b0ec7372f568029527c0809262db66d162a67d82e2ddc4d`  
		Last Modified: Wed, 15 Jan 2020 17:53:42 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3993164e2c009ccf7891a7fb2956b069daf095ac7a081307e8494e594e98fa`  
		Last Modified: Wed, 15 Jan 2020 17:53:43 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.2-windowsservercore-1803`

```console
$ docker pull nats@sha256:d06f971a89319c413118f67b67dab4e52914ad2540fcd2844f831c2a237c35d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17134.1246; amd64

### `nats:2.1.2-windowsservercore-1803` - windows version 10.0.17134.1246; amd64

```console
$ docker pull nats@sha256:68c9dff50987d82ca20958b1a5ca7cb816509b6d6b024ecc0a5f83cfe26f5f59
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2368141200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20f6b32275bca4375a3ca4b65ab024126e7ae1c30725dcd7ab47d638bc9c5dbc`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 12 Apr 2018 09:20:54 GMT
RUN Apply image 1803-RTM-amd64
# Wed, 08 Jan 2020 15:30:02 GMT
RUN Install update 1803-amd64
# Wed, 15 Jan 2020 17:44:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jan 2020 17:44:14 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:44:15 GMT
ENV NATS_SERVER=2.1.2
# Wed, 15 Jan 2020 17:44:16 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.2/nats-server-v2.1.2-windows-amd64.zip
# Wed, 15 Jan 2020 17:45:13 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jan 2020 17:46:20 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Jan 2020 17:46:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:46:22 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:46:24 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:46:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d9e8b01179bfc94a5bdb1810fbd76b999aa52016001ace2d3a4c4bc7065a9601`  
		Last Modified: Tue, 18 Sep 2018 22:43:55 GMT  
		Size: 1.7 GB (1659688273 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:270ec3ad3fc7d52c0dd086b32f7751131c799e25cdcd4686cc33cbf2b607c34e`  
		Size: 699.2 MB (699246147 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dbec356e813f8f1863318efd5cd62c261f7de4ac49fc093c648020e26d0520fb`  
		Last Modified: Wed, 15 Jan 2020 17:52:17 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c748a716adbca27bf760bc535221171b42c3dcfd044a49e011295928c66c39`  
		Last Modified: Wed, 15 Jan 2020 17:52:17 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7efb3710bacce94103ccc92d28b0a0af30a9bb7a29f1d7f45fc18a75e959ee2d`  
		Last Modified: Wed, 15 Jan 2020 17:52:16 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883bd0fc138e4a17c679bf7d23bb5f0186ccae58fbacdfda29c147e85e2d9383`  
		Last Modified: Wed, 15 Jan 2020 17:52:15 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967451731bebacb830dc7e26892242d8d5c55f6576f5476820313ac2f35d2550`  
		Last Modified: Wed, 15 Jan 2020 17:52:17 GMT  
		Size: 4.9 MB (4880651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35062fb2b37da05d5d753b6519295e3b14da0bf8fecf57ba90fb507aaf498b7`  
		Last Modified: Wed, 15 Jan 2020 17:52:15 GMT  
		Size: 4.3 MB (4316097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bcb4b1ca97cf159a8a5030f29505c9c52626907a92244c92d25df16333f84bf`  
		Last Modified: Wed, 15 Jan 2020 17:52:13 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a380672454ff5ba95dd36413220fa3f00b7998578a8f32ee0b85cfd6d6f9666`  
		Last Modified: Wed, 15 Jan 2020 17:52:13 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f545bb1274ec20783b4966e6592ba3ca21b327f02552a0480c57eae7bd6a77`  
		Last Modified: Wed, 15 Jan 2020 17:52:13 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29eea8dff9fd0ad0a6c1d9943b993b4519c8d7c48140eeb20de7f46fe018e764`  
		Last Modified: Wed, 15 Jan 2020 17:52:13 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.2-windowsservercore-1809`

```console
$ docker pull nats@sha256:655dcc67ed8905581e9ef5bbc18c06dbd66da9bea9b4dbfc5baf5e575525438e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64

### `nats:2.1.2-windowsservercore-1809` - windows version 10.0.17763.973; amd64

```console
$ docker pull nats@sha256:f5ac96a023326f836cf1c02a5f5b30abd128056d648cac3a4643c8125532ec4f
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2230470888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66ed94808574b78075af126587ee0e95fd33c3b8964fbec51c76c08c20bba3d6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Wed, 15 Jan 2020 14:40:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jan 2020 17:41:54 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:41:55 GMT
ENV NATS_SERVER=2.1.2
# Wed, 15 Jan 2020 17:41:56 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.2/nats-server-v2.1.2-windows-amd64.zip
# Wed, 15 Jan 2020 17:42:38 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jan 2020 17:43:46 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Jan 2020 17:43:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:43:49 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:43:50 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:43:52 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2397868e5c7aa285f662aaa9309fa4756277739e11d589a663a204df80595f2c`  
		Last Modified: Wed, 15 Jan 2020 17:10:53 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b23c268ec0520ea9af1e83b69008728041b2a5f234937b9a6272d2a739fd92e`  
		Last Modified: Wed, 15 Jan 2020 17:51:25 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8bf81f9ddd524bd8d7611b92b362a8f558a338e038fb1a81f81872f58a76f7`  
		Last Modified: Wed, 15 Jan 2020 17:51:25 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb3c94fff5bd229bc976399c1904de65b246152cd41d0147af159fd09877822a`  
		Last Modified: Wed, 15 Jan 2020 17:51:24 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e70dcd5f51d264f2ff2ba291ee37e474f5637d236d01c2d5cd8a4ab039dc60`  
		Last Modified: Wed, 15 Jan 2020 17:51:26 GMT  
		Size: 4.5 MB (4548759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b87189fe10fd6d476acc4c0869463fe1f0d813aa1fc2ff3d95efa65f86d7f34`  
		Last Modified: Wed, 15 Jan 2020 17:51:31 GMT  
		Size: 8.5 MB (8500806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a611e13685ceef48268051590fc9cc976fdec2ec0968e3a12fb9b7ef72b6f2`  
		Last Modified: Wed, 15 Jan 2020 17:51:22 GMT  
		Size: 1.8 KB (1763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ebd020bd73cd69b61c2325da491f4c057f7fdeac1f37db60365aef9d9f56e6`  
		Last Modified: Wed, 15 Jan 2020 17:51:22 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2ef97f255816c764614a7a10afa9fa89f6b8fa9c107f24458eab08ad8aee6d`  
		Last Modified: Wed, 15 Jan 2020 17:51:22 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d555934698e4f3eaa1e7fef777b3692d4a519ec978ec5f191be9ea1a772ad6`  
		Last Modified: Wed, 15 Jan 2020 17:51:22 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:b0bab523ef87fed76cbcc206909058cdceace4206e8797b3dc3bb074f8148c9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3443; amd64

### `nats:2.1.2-windowsservercore-ltsc2016` - windows version 10.0.14393.3443; amd64

```console
$ docker pull nats@sha256:f3b8aa519f1e9981b369d238e46b3e336b2df7654f7cf784b5601d5342a49137
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 GB (5739369423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56ca53177d88b1126a979fb5530e66d83974e1838cecce90ade826949f5ea259`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 02 Jan 2020 15:48:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Jan 2020 15:20:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jan 2020 17:47:08 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:47:10 GMT
ENV NATS_SERVER=2.1.2
# Wed, 15 Jan 2020 17:47:11 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.2/nats-server-v2.1.2-windows-amd64.zip
# Wed, 15 Jan 2020 17:48:21 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jan 2020 17:50:09 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Jan 2020 17:50:10 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:50:12 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:50:14 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:50:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31f9df80631e7b5d379647ee7701ff50e009bd2c03b30a67a0a8e7bba4a26f94`  
		Size: 1.7 GB (1654613376 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:43da502775fb34b738d9f908cb549c2825c04f1451d1039ec99749be127e47ef`  
		Last Modified: Wed, 15 Jan 2020 17:12:02 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6771e606bb5340710c7ec7fa3294903a0a1f901e5c1e79211ee54fc1f074179a`  
		Last Modified: Wed, 15 Jan 2020 17:53:47 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8885516d0bc2df9c7e82fe0aeb847bc83415084fe85a9aed26a03b3b56ae7c`  
		Last Modified: Wed, 15 Jan 2020 17:53:46 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68459b3a704ec7e5908e23d0d52576c68eef20a4b3ede7bf88ec4e3b2321d170`  
		Last Modified: Wed, 15 Jan 2020 17:53:46 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196e19f93e85979cb0240edd67162a54a2e716e7b139c9c7a99882b3dc42fc2a`  
		Last Modified: Wed, 15 Jan 2020 17:53:47 GMT  
		Size: 5.4 MB (5383420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2ec8ad5670f9274bd1b0dbc71a9ac551d4b18d3f6254bf51bbd80049d7d9c2`  
		Last Modified: Wed, 15 Jan 2020 17:53:46 GMT  
		Size: 9.4 MB (9376638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4abd28582063a6691f03037049db18ea066600d7023aa3d2975eb66ea3cafd`  
		Last Modified: Wed, 15 Jan 2020 17:53:43 GMT  
		Size: 1.8 KB (1762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe6eef99ce520e46eef3031fa6ebd7aeba735253cef9dd2b4e7e07255a9efd8`  
		Last Modified: Wed, 15 Jan 2020 17:53:43 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb11317f8d70c8d41b0ec7372f568029527c0809262db66d162a67d82e2ddc4d`  
		Last Modified: Wed, 15 Jan 2020 17:53:42 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3993164e2c009ccf7891a7fb2956b069daf095ac7a081307e8494e594e98fa`  
		Last Modified: Wed, 15 Jan 2020 17:53:43 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-alpine`

```console
$ docker pull nats@sha256:71e945d4d94bfc25dfdb242bad666f2979caef77f1bff75728f1cc72b4804081
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats:2.1-alpine` - linux; amd64

```console
$ docker pull nats@sha256:f507195794f36c37413ca058f5c3442ad24a80facf94cf4779297e4ab0971f99
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7092803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffa6d536d932527718344a90a884bb621e3480d21893e4bf8e4b7e46b05ad957`
-	Default Command: `["nats-server"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 19:19:25 GMT
ENV NATS_SERVER=2.1.2
# Thu, 23 Jan 2020 19:19:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 23 Jan 2020 19:19:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 23 Jan 2020 19:19:29 GMT
EXPOSE 4222 6222 8222
# Thu, 23 Jan 2020 19:19:29 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581b0b35a07f0a300a55e836a3ba0cb3d18061455a6367a15fbd6f127b57351c`  
		Last Modified: Thu, 23 Jan 2020 19:20:29 GMT  
		Size: 4.3 MB (4305310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82a66d5edde56b04466489c0c46457358c6737789e7e4cde197d7b0befe4fa3`  
		Last Modified: Thu, 23 Jan 2020 19:20:28 GMT  
		Size: 531.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:6380d8b1fc432a021689908f6501d49747edf3b3c2bc54134e433c10e77efb1c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6664521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a20dd366129d9b5428c44f6c6853a8297f7b86b3e6b8f20a1600da467f76599`
-	Default Command: `["nats-server"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:27 GMT
ADD file:2aa80d52585a6b34b2cc5811d46965a084e50cfb8cd183f1a88b2b1bc6556e1f in / 
# Thu, 23 Jan 2020 16:53:28 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:44:32 GMT
ENV NATS_SERVER=2.1.2
# Thu, 23 Jan 2020 17:44:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 23 Jan 2020 17:44:39 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 23 Jan 2020 17:44:40 GMT
EXPOSE 4222 6222 8222
# Thu, 23 Jan 2020 17:44:41 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:896868b7b9168cabb308702db96dc9769d10c23e20fc66f5f4abedf4c75d7642`  
		Last Modified: Thu, 23 Jan 2020 16:54:07 GMT  
		Size: 2.6 MB (2571407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f146c76b464f3790626809adda3914591425f7cd06759a183ccd5da25e26bb82`  
		Last Modified: Thu, 23 Jan 2020 17:45:13 GMT  
		Size: 4.1 MB (4092555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162410de1cd5b2c2ce2cd44dc7973ff2511dc755faeca556ea9e69b1aa55fae3`  
		Last Modified: Thu, 23 Jan 2020 17:45:12 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:d60f1b23e6d2ce2e8edac172e464de946fa830452af16b709c8d3c8234a3c045
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6466632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d154ea04a5c19abf9bcf38dacc8b82bee649c6c507024227c5cd298ed1ac75c6`
-	Default Command: `["nats-server"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:31 GMT
ADD file:d05c9f9143d11d12045d4faef882e5985e6b38fabe52237dd8d8c0627a9620ab in / 
# Thu, 23 Jan 2020 16:53:32 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:55:25 GMT
ENV NATS_SERVER=2.1.2
# Thu, 23 Jan 2020 17:55:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 23 Jan 2020 17:55:30 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 23 Jan 2020 17:55:31 GMT
EXPOSE 4222 6222 8222
# Thu, 23 Jan 2020 17:55:32 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:4e972d957a606327b0b6c2e8aa4a6045c263b7496a536298aaebf690e9d85f1d`  
		Last Modified: Thu, 23 Jan 2020 16:53:59 GMT  
		Size: 2.4 MB (2378408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c375dc9edf38cadcfdc6537707cdea65e2b45d840940712d2f88d19cc967edc6`  
		Last Modified: Thu, 23 Jan 2020 17:56:08 GMT  
		Size: 4.1 MB (4087666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bfcd4ad511455617c2f402e3d5ebd12e714c0d9a0d280f7399735754fab756e`  
		Last Modified: Thu, 23 Jan 2020 17:56:08 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-alpine3.10`

```console
$ docker pull nats@sha256:71e945d4d94bfc25dfdb242bad666f2979caef77f1bff75728f1cc72b4804081
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats:2.1-alpine3.10` - linux; amd64

```console
$ docker pull nats@sha256:f507195794f36c37413ca058f5c3442ad24a80facf94cf4779297e4ab0971f99
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7092803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffa6d536d932527718344a90a884bb621e3480d21893e4bf8e4b7e46b05ad957`
-	Default Command: `["nats-server"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 19:19:25 GMT
ENV NATS_SERVER=2.1.2
# Thu, 23 Jan 2020 19:19:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 23 Jan 2020 19:19:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 23 Jan 2020 19:19:29 GMT
EXPOSE 4222 6222 8222
# Thu, 23 Jan 2020 19:19:29 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581b0b35a07f0a300a55e836a3ba0cb3d18061455a6367a15fbd6f127b57351c`  
		Last Modified: Thu, 23 Jan 2020 19:20:29 GMT  
		Size: 4.3 MB (4305310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82a66d5edde56b04466489c0c46457358c6737789e7e4cde197d7b0befe4fa3`  
		Last Modified: Thu, 23 Jan 2020 19:20:28 GMT  
		Size: 531.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-alpine3.10` - linux; arm variant v6

```console
$ docker pull nats@sha256:6380d8b1fc432a021689908f6501d49747edf3b3c2bc54134e433c10e77efb1c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6664521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a20dd366129d9b5428c44f6c6853a8297f7b86b3e6b8f20a1600da467f76599`
-	Default Command: `["nats-server"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:27 GMT
ADD file:2aa80d52585a6b34b2cc5811d46965a084e50cfb8cd183f1a88b2b1bc6556e1f in / 
# Thu, 23 Jan 2020 16:53:28 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:44:32 GMT
ENV NATS_SERVER=2.1.2
# Thu, 23 Jan 2020 17:44:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 23 Jan 2020 17:44:39 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 23 Jan 2020 17:44:40 GMT
EXPOSE 4222 6222 8222
# Thu, 23 Jan 2020 17:44:41 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:896868b7b9168cabb308702db96dc9769d10c23e20fc66f5f4abedf4c75d7642`  
		Last Modified: Thu, 23 Jan 2020 16:54:07 GMT  
		Size: 2.6 MB (2571407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f146c76b464f3790626809adda3914591425f7cd06759a183ccd5da25e26bb82`  
		Last Modified: Thu, 23 Jan 2020 17:45:13 GMT  
		Size: 4.1 MB (4092555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162410de1cd5b2c2ce2cd44dc7973ff2511dc755faeca556ea9e69b1aa55fae3`  
		Last Modified: Thu, 23 Jan 2020 17:45:12 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-alpine3.10` - linux; arm variant v7

```console
$ docker pull nats@sha256:d60f1b23e6d2ce2e8edac172e464de946fa830452af16b709c8d3c8234a3c045
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6466632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d154ea04a5c19abf9bcf38dacc8b82bee649c6c507024227c5cd298ed1ac75c6`
-	Default Command: `["nats-server"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:31 GMT
ADD file:d05c9f9143d11d12045d4faef882e5985e6b38fabe52237dd8d8c0627a9620ab in / 
# Thu, 23 Jan 2020 16:53:32 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:55:25 GMT
ENV NATS_SERVER=2.1.2
# Thu, 23 Jan 2020 17:55:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 23 Jan 2020 17:55:30 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 23 Jan 2020 17:55:31 GMT
EXPOSE 4222 6222 8222
# Thu, 23 Jan 2020 17:55:32 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:4e972d957a606327b0b6c2e8aa4a6045c263b7496a536298aaebf690e9d85f1d`  
		Last Modified: Thu, 23 Jan 2020 16:53:59 GMT  
		Size: 2.4 MB (2378408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c375dc9edf38cadcfdc6537707cdea65e2b45d840940712d2f88d19cc967edc6`  
		Last Modified: Thu, 23 Jan 2020 17:56:08 GMT  
		Size: 4.1 MB (4087666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bfcd4ad511455617c2f402e3d5ebd12e714c0d9a0d280f7399735754fab756e`  
		Last Modified: Thu, 23 Jan 2020 17:56:08 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-linux`

```console
$ docker pull nats@sha256:59141670457fa112c6b1cf5cca3b159ad15bfb7e70fe0b1acbbb5616d922a3c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.1-linux` - linux; amd64

```console
$ docker pull nats@sha256:8139c5bf4df6e8635cb3420d2dfab08ecdf75b8d16cd82c40a67bd4417b2e71c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (4002673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49014ccb53efc06dc1ce6656aea0abf000881d9db3ac5b31c6f8aef934452b30`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Nov 2019 01:14:07 GMT
COPY file:f7ba6139c8151888be538812698c1aab4311e97fcfac3b5af13138cd7d7e1405 in /nats-server 
# Wed, 20 Nov 2019 01:14:07 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 20 Nov 2019 01:14:08 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Nov 2019 01:14:08 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Nov 2019 01:14:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f3c8f35bd9bcd03ff8eba7551a59aa4fb56c5eabac4758b0b6cb12709785f25c`  
		Last Modified: Wed, 20 Nov 2019 01:14:44 GMT  
		Size: 4.0 MB (4002195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba25f2430b4efc5a2c8e36c142c7aca0b9a14a6caf16fe09d29f97f77f4efce`  
		Last Modified: Wed, 20 Nov 2019 01:14:43 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:234935205b93b7c99b67d82fe35226290aa302e2b35b32f7f9516aa770bf6003
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3790304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66f838f1a59cd8673948823057d50b486bb443ce5318e5a24502ded16334feda`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Nov 2019 00:04:38 GMT
COPY file:1c509c11a9e5697ac3184dd6c0dca46386d2a5d22fabbd0f4898bad8342884d8 in /nats-server 
# Wed, 20 Nov 2019 00:04:39 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 20 Nov 2019 00:04:39 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Nov 2019 00:04:40 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Nov 2019 00:04:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ab4822bfc4bb3725c051563099752bf9f3cc14db9a698a66f64c906201e88b2d`  
		Last Modified: Wed, 20 Nov 2019 00:05:19 GMT  
		Size: 3.8 MB (3789828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd9cf11d4796d35bb8140733b85f1398c199c592ad417cb6d22eac97b0ac377`  
		Last Modified: Wed, 20 Nov 2019 00:05:18 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:92ea09078a55fc56a807ede1630a862d4b6acc12633391a5a42b41483c6b66fa
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3786713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df9b97d154301cbefd42558306e1ece9667269fb9bda4c0ff2c2f601b578c2c8`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Nov 2019 00:53:13 GMT
COPY file:f7bd56432332a04229b22e2b4ed52b31e5ba863bb47a2aacf6d808bd4a8397d1 in /nats-server 
# Wed, 20 Nov 2019 00:53:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 20 Nov 2019 00:53:15 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Nov 2019 00:53:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Nov 2019 00:53:19 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:27216bfb43f9e231372de919d3bbc108e604422a1019a0b0407001997c0575fe`  
		Last Modified: Wed, 20 Nov 2019 00:54:09 GMT  
		Size: 3.8 MB (3786237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3750c7c4312b8b2af995298314a15791a97ce1ef156b81c0477e579fb42b7f2e`  
		Last Modified: Wed, 20 Nov 2019 00:54:09 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:284c4850adc39c33100ab1324dbe23ddde7450c6e5bd15da874d459e68e0ea3e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3665772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeda44c76561e9490c8a19cffd362e26a5552c3aafd41c98b9562a6ae8a01874`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 20 Sep 2019 23:29:17 GMT
COPY file:f0dce6fb207b92a78774313458c6030a8ac0653785d2a2d54e8b5c8935d9b6b8 in /nats-server 
# Fri, 18 Oct 2019 18:04:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 18 Oct 2019 18:04:47 GMT
EXPOSE 4222 6222 8222
# Fri, 18 Oct 2019 18:04:48 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 18 Oct 2019 18:04:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:98fcb931241702ef0a04aa16bb1e4bab6b8afd06f792790462dff69dee05835c`  
		Last Modified: Fri, 20 Sep 2019 23:29:32 GMT  
		Size: 3.7 MB (3665294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e761cba9328047725686c1ed6eecd9eeef33879d348aea70fb3d219b546165`  
		Last Modified: Fri, 18 Oct 2019 18:05:08 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-nanoserver`

```console
$ docker pull nats@sha256:d028e8a1c50120304d4111bb1214475e11f3684b7176df24a5ec7b00f650decb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64
	-	windows version 10.0.17134.1246; amd64

### `nats:2.1-nanoserver` - windows version 10.0.17763.973; amd64

```console
$ docker pull nats@sha256:fe1ec52862c24ed520cc33ba713ca2a1ab61132fe67f8e4271dd3d54739175bf
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105047963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d2592fd645781c520143281ac28e8f8eba6f4184b893dd1f41c47f4cfea6e22`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 04 Jan 2020 07:17:17 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jan 2020 17:50:29 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:50:31 GMT
RUN cmd /S /C #(nop) COPY file:a9e3f6c9790c912d513d2134dc1f68e02a9edf34862dd584010eae5ab8418108 in C:\nats-server.exe 
# Wed, 15 Jan 2020 17:50:33 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:50:34 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:50:36 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:50:37 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ee446884f7bef76f8275c2f16add1c4fb598bea2ba861e72bce8fb4aac9b55ef`  
		Size: 101.1 MB (101054324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95d31e7189792498b758db35ae56b1ca97128d8063404cbe62a32205d08d1d4a`  
		Last Modified: Wed, 15 Jan 2020 17:54:30 GMT  
		Size: 940.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06dd0cb87c9a67456f9c940ed213536b3e08acb7279b65835e3c65a7654d86f3`  
		Last Modified: Wed, 15 Jan 2020 17:54:30 GMT  
		Size: 4.0 MB (3988335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a3fd5110f7e9b5b9bdf1dcaa1d44324372e6327142443cd9886d09870d8897e`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 1.6 KB (1560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc491f53dd9a291eef7348c3086782cb45ddb7d249aa3fcd080d0dcc05dc8000`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 939.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8053efdd66e716af07b38c62c28b0878f99af0173a9360e403074367593dcc1`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 942.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3215e4233ac1a2ec100e0e6d20af8633eebf5fce1e5813077fdbab6deb27fbb`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-nanoserver` - windows version 10.0.17134.1246; amd64

```console
$ docker pull nats@sha256:5f107d9f832b82ff068741b598503279a5c98f7239c376ba43f9e9e63eb46e9a
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.9 MB (157902423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b01104ee474980123a7757c086644468acfb2f4883fb483597c3db674d4181a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 11 Apr 2018 22:12:30 GMT
RUN Apply image 1803-RTM-amd64
# Wed, 08 Jan 2020 15:12:42 GMT
RUN Install update 1803-amd64
# Wed, 15 Jan 2020 17:46:46 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:46:49 GMT
RUN cmd /S /C #(nop) COPY file:a9e3f6c9790c912d513d2134dc1f68e02a9edf34862dd584010eae5ab8418108 in C:\nats-server.exe 
# Wed, 15 Jan 2020 17:46:50 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:46:52 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:46:53 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:46:54 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e46172273a4e4384e1eec7fb01091c828a256ea0f87b30f61381fba9bc511371`  
		Last Modified: Mon, 17 Sep 2018 20:23:30 GMT  
		Size: 92.8 MB (92818888 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c0783c3b88b74a9de609bda64fc01cd5e23fb65d57e750a9c584e8a9ed842fa9`  
		Size: 61.1 MB (61089912 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:24f456fbaddb9e6d59a1ebc9e9244a4b7b003b467f4379a121463c469fe5ac34`  
		Last Modified: Wed, 15 Jan 2020 17:53:01 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2280cf6b56b3522c9f82db3208ab840d8e3292ec7d042eb1d7d4c00319b640`  
		Last Modified: Wed, 15 Jan 2020 17:53:01 GMT  
		Size: 4.0 MB (3988299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c0024dc7e88bada373f0f9593d8ca873d955ddef73363bd42f421f37a339598`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 1.6 KB (1555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d6c860f0094966bd95e3a9b933773c4aa19466f9b337f383aa138b5b41ab22`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15569096640ccf86ed6b731f1e8ecac13947a7bfe4fdaa0b9800f7484bb266c4`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 951.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c849d8e8a6767e0308da9ac7027ca2eecb68424c8d4d748989768b7f920283`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-nanoserver-1803`

```console
$ docker pull nats@sha256:9c4a8412f1acfb6279840bdb68e678c0e848b259196fecef0d4ea62c120654c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17134.1246; amd64

### `nats:2.1-nanoserver-1803` - windows version 10.0.17134.1246; amd64

```console
$ docker pull nats@sha256:5f107d9f832b82ff068741b598503279a5c98f7239c376ba43f9e9e63eb46e9a
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.9 MB (157902423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b01104ee474980123a7757c086644468acfb2f4883fb483597c3db674d4181a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 11 Apr 2018 22:12:30 GMT
RUN Apply image 1803-RTM-amd64
# Wed, 08 Jan 2020 15:12:42 GMT
RUN Install update 1803-amd64
# Wed, 15 Jan 2020 17:46:46 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:46:49 GMT
RUN cmd /S /C #(nop) COPY file:a9e3f6c9790c912d513d2134dc1f68e02a9edf34862dd584010eae5ab8418108 in C:\nats-server.exe 
# Wed, 15 Jan 2020 17:46:50 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:46:52 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:46:53 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:46:54 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e46172273a4e4384e1eec7fb01091c828a256ea0f87b30f61381fba9bc511371`  
		Last Modified: Mon, 17 Sep 2018 20:23:30 GMT  
		Size: 92.8 MB (92818888 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c0783c3b88b74a9de609bda64fc01cd5e23fb65d57e750a9c584e8a9ed842fa9`  
		Size: 61.1 MB (61089912 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:24f456fbaddb9e6d59a1ebc9e9244a4b7b003b467f4379a121463c469fe5ac34`  
		Last Modified: Wed, 15 Jan 2020 17:53:01 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2280cf6b56b3522c9f82db3208ab840d8e3292ec7d042eb1d7d4c00319b640`  
		Last Modified: Wed, 15 Jan 2020 17:53:01 GMT  
		Size: 4.0 MB (3988299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c0024dc7e88bada373f0f9593d8ca873d955ddef73363bd42f421f37a339598`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 1.6 KB (1555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d6c860f0094966bd95e3a9b933773c4aa19466f9b337f383aa138b5b41ab22`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15569096640ccf86ed6b731f1e8ecac13947a7bfe4fdaa0b9800f7484bb266c4`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 951.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c849d8e8a6767e0308da9ac7027ca2eecb68424c8d4d748989768b7f920283`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-nanoserver-1809`

```console
$ docker pull nats@sha256:35356d98d96477f83eab4060656843a014506567dc5ad5c2acea557bd05c69b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64

### `nats:2.1-nanoserver-1809` - windows version 10.0.17763.973; amd64

```console
$ docker pull nats@sha256:fe1ec52862c24ed520cc33ba713ca2a1ab61132fe67f8e4271dd3d54739175bf
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105047963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d2592fd645781c520143281ac28e8f8eba6f4184b893dd1f41c47f4cfea6e22`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 04 Jan 2020 07:17:17 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jan 2020 17:50:29 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:50:31 GMT
RUN cmd /S /C #(nop) COPY file:a9e3f6c9790c912d513d2134dc1f68e02a9edf34862dd584010eae5ab8418108 in C:\nats-server.exe 
# Wed, 15 Jan 2020 17:50:33 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:50:34 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:50:36 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:50:37 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ee446884f7bef76f8275c2f16add1c4fb598bea2ba861e72bce8fb4aac9b55ef`  
		Size: 101.1 MB (101054324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95d31e7189792498b758db35ae56b1ca97128d8063404cbe62a32205d08d1d4a`  
		Last Modified: Wed, 15 Jan 2020 17:54:30 GMT  
		Size: 940.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06dd0cb87c9a67456f9c940ed213536b3e08acb7279b65835e3c65a7654d86f3`  
		Last Modified: Wed, 15 Jan 2020 17:54:30 GMT  
		Size: 4.0 MB (3988335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a3fd5110f7e9b5b9bdf1dcaa1d44324372e6327142443cd9886d09870d8897e`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 1.6 KB (1560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc491f53dd9a291eef7348c3086782cb45ddb7d249aa3fcd080d0dcc05dc8000`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 939.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8053efdd66e716af07b38c62c28b0878f99af0173a9360e403074367593dcc1`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 942.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3215e4233ac1a2ec100e0e6d20af8633eebf5fce1e5813077fdbab6deb27fbb`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-scratch`

```console
$ docker pull nats@sha256:59141670457fa112c6b1cf5cca3b159ad15bfb7e70fe0b1acbbb5616d922a3c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.1-scratch` - linux; amd64

```console
$ docker pull nats@sha256:8139c5bf4df6e8635cb3420d2dfab08ecdf75b8d16cd82c40a67bd4417b2e71c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (4002673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49014ccb53efc06dc1ce6656aea0abf000881d9db3ac5b31c6f8aef934452b30`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Nov 2019 01:14:07 GMT
COPY file:f7ba6139c8151888be538812698c1aab4311e97fcfac3b5af13138cd7d7e1405 in /nats-server 
# Wed, 20 Nov 2019 01:14:07 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 20 Nov 2019 01:14:08 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Nov 2019 01:14:08 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Nov 2019 01:14:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f3c8f35bd9bcd03ff8eba7551a59aa4fb56c5eabac4758b0b6cb12709785f25c`  
		Last Modified: Wed, 20 Nov 2019 01:14:44 GMT  
		Size: 4.0 MB (4002195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba25f2430b4efc5a2c8e36c142c7aca0b9a14a6caf16fe09d29f97f77f4efce`  
		Last Modified: Wed, 20 Nov 2019 01:14:43 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:234935205b93b7c99b67d82fe35226290aa302e2b35b32f7f9516aa770bf6003
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3790304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66f838f1a59cd8673948823057d50b486bb443ce5318e5a24502ded16334feda`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Nov 2019 00:04:38 GMT
COPY file:1c509c11a9e5697ac3184dd6c0dca46386d2a5d22fabbd0f4898bad8342884d8 in /nats-server 
# Wed, 20 Nov 2019 00:04:39 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 20 Nov 2019 00:04:39 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Nov 2019 00:04:40 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Nov 2019 00:04:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ab4822bfc4bb3725c051563099752bf9f3cc14db9a698a66f64c906201e88b2d`  
		Last Modified: Wed, 20 Nov 2019 00:05:19 GMT  
		Size: 3.8 MB (3789828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd9cf11d4796d35bb8140733b85f1398c199c592ad417cb6d22eac97b0ac377`  
		Last Modified: Wed, 20 Nov 2019 00:05:18 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:92ea09078a55fc56a807ede1630a862d4b6acc12633391a5a42b41483c6b66fa
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3786713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df9b97d154301cbefd42558306e1ece9667269fb9bda4c0ff2c2f601b578c2c8`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Nov 2019 00:53:13 GMT
COPY file:f7bd56432332a04229b22e2b4ed52b31e5ba863bb47a2aacf6d808bd4a8397d1 in /nats-server 
# Wed, 20 Nov 2019 00:53:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 20 Nov 2019 00:53:15 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Nov 2019 00:53:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Nov 2019 00:53:19 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:27216bfb43f9e231372de919d3bbc108e604422a1019a0b0407001997c0575fe`  
		Last Modified: Wed, 20 Nov 2019 00:54:09 GMT  
		Size: 3.8 MB (3786237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3750c7c4312b8b2af995298314a15791a97ce1ef156b81c0477e579fb42b7f2e`  
		Last Modified: Wed, 20 Nov 2019 00:54:09 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:284c4850adc39c33100ab1324dbe23ddde7450c6e5bd15da874d459e68e0ea3e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3665772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeda44c76561e9490c8a19cffd362e26a5552c3aafd41c98b9562a6ae8a01874`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 20 Sep 2019 23:29:17 GMT
COPY file:f0dce6fb207b92a78774313458c6030a8ac0653785d2a2d54e8b5c8935d9b6b8 in /nats-server 
# Fri, 18 Oct 2019 18:04:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 18 Oct 2019 18:04:47 GMT
EXPOSE 4222 6222 8222
# Fri, 18 Oct 2019 18:04:48 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 18 Oct 2019 18:04:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:98fcb931241702ef0a04aa16bb1e4bab6b8afd06f792790462dff69dee05835c`  
		Last Modified: Fri, 20 Sep 2019 23:29:32 GMT  
		Size: 3.7 MB (3665294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e761cba9328047725686c1ed6eecd9eeef33879d348aea70fb3d219b546165`  
		Last Modified: Fri, 18 Oct 2019 18:05:08 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-windowsservercore`

```console
$ docker pull nats@sha256:a42f0c67634d642f56a78fcc79c12b8d5d4da81b34b93f1ccb103ba2743f6e23
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64
	-	windows version 10.0.17134.1246; amd64
	-	windows version 10.0.14393.3443; amd64

### `nats:2.1-windowsservercore` - windows version 10.0.17763.973; amd64

```console
$ docker pull nats@sha256:f5ac96a023326f836cf1c02a5f5b30abd128056d648cac3a4643c8125532ec4f
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2230470888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66ed94808574b78075af126587ee0e95fd33c3b8964fbec51c76c08c20bba3d6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Wed, 15 Jan 2020 14:40:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jan 2020 17:41:54 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:41:55 GMT
ENV NATS_SERVER=2.1.2
# Wed, 15 Jan 2020 17:41:56 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.2/nats-server-v2.1.2-windows-amd64.zip
# Wed, 15 Jan 2020 17:42:38 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jan 2020 17:43:46 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Jan 2020 17:43:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:43:49 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:43:50 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:43:52 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2397868e5c7aa285f662aaa9309fa4756277739e11d589a663a204df80595f2c`  
		Last Modified: Wed, 15 Jan 2020 17:10:53 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b23c268ec0520ea9af1e83b69008728041b2a5f234937b9a6272d2a739fd92e`  
		Last Modified: Wed, 15 Jan 2020 17:51:25 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8bf81f9ddd524bd8d7611b92b362a8f558a338e038fb1a81f81872f58a76f7`  
		Last Modified: Wed, 15 Jan 2020 17:51:25 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb3c94fff5bd229bc976399c1904de65b246152cd41d0147af159fd09877822a`  
		Last Modified: Wed, 15 Jan 2020 17:51:24 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e70dcd5f51d264f2ff2ba291ee37e474f5637d236d01c2d5cd8a4ab039dc60`  
		Last Modified: Wed, 15 Jan 2020 17:51:26 GMT  
		Size: 4.5 MB (4548759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b87189fe10fd6d476acc4c0869463fe1f0d813aa1fc2ff3d95efa65f86d7f34`  
		Last Modified: Wed, 15 Jan 2020 17:51:31 GMT  
		Size: 8.5 MB (8500806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a611e13685ceef48268051590fc9cc976fdec2ec0968e3a12fb9b7ef72b6f2`  
		Last Modified: Wed, 15 Jan 2020 17:51:22 GMT  
		Size: 1.8 KB (1763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ebd020bd73cd69b61c2325da491f4c057f7fdeac1f37db60365aef9d9f56e6`  
		Last Modified: Wed, 15 Jan 2020 17:51:22 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2ef97f255816c764614a7a10afa9fa89f6b8fa9c107f24458eab08ad8aee6d`  
		Last Modified: Wed, 15 Jan 2020 17:51:22 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d555934698e4f3eaa1e7fef777b3692d4a519ec978ec5f191be9ea1a772ad6`  
		Last Modified: Wed, 15 Jan 2020 17:51:22 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-windowsservercore` - windows version 10.0.17134.1246; amd64

```console
$ docker pull nats@sha256:68c9dff50987d82ca20958b1a5ca7cb816509b6d6b024ecc0a5f83cfe26f5f59
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2368141200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20f6b32275bca4375a3ca4b65ab024126e7ae1c30725dcd7ab47d638bc9c5dbc`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 12 Apr 2018 09:20:54 GMT
RUN Apply image 1803-RTM-amd64
# Wed, 08 Jan 2020 15:30:02 GMT
RUN Install update 1803-amd64
# Wed, 15 Jan 2020 17:44:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jan 2020 17:44:14 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:44:15 GMT
ENV NATS_SERVER=2.1.2
# Wed, 15 Jan 2020 17:44:16 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.2/nats-server-v2.1.2-windows-amd64.zip
# Wed, 15 Jan 2020 17:45:13 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jan 2020 17:46:20 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Jan 2020 17:46:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:46:22 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:46:24 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:46:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d9e8b01179bfc94a5bdb1810fbd76b999aa52016001ace2d3a4c4bc7065a9601`  
		Last Modified: Tue, 18 Sep 2018 22:43:55 GMT  
		Size: 1.7 GB (1659688273 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:270ec3ad3fc7d52c0dd086b32f7751131c799e25cdcd4686cc33cbf2b607c34e`  
		Size: 699.2 MB (699246147 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dbec356e813f8f1863318efd5cd62c261f7de4ac49fc093c648020e26d0520fb`  
		Last Modified: Wed, 15 Jan 2020 17:52:17 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c748a716adbca27bf760bc535221171b42c3dcfd044a49e011295928c66c39`  
		Last Modified: Wed, 15 Jan 2020 17:52:17 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7efb3710bacce94103ccc92d28b0a0af30a9bb7a29f1d7f45fc18a75e959ee2d`  
		Last Modified: Wed, 15 Jan 2020 17:52:16 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883bd0fc138e4a17c679bf7d23bb5f0186ccae58fbacdfda29c147e85e2d9383`  
		Last Modified: Wed, 15 Jan 2020 17:52:15 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967451731bebacb830dc7e26892242d8d5c55f6576f5476820313ac2f35d2550`  
		Last Modified: Wed, 15 Jan 2020 17:52:17 GMT  
		Size: 4.9 MB (4880651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35062fb2b37da05d5d753b6519295e3b14da0bf8fecf57ba90fb507aaf498b7`  
		Last Modified: Wed, 15 Jan 2020 17:52:15 GMT  
		Size: 4.3 MB (4316097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bcb4b1ca97cf159a8a5030f29505c9c52626907a92244c92d25df16333f84bf`  
		Last Modified: Wed, 15 Jan 2020 17:52:13 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a380672454ff5ba95dd36413220fa3f00b7998578a8f32ee0b85cfd6d6f9666`  
		Last Modified: Wed, 15 Jan 2020 17:52:13 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f545bb1274ec20783b4966e6592ba3ca21b327f02552a0480c57eae7bd6a77`  
		Last Modified: Wed, 15 Jan 2020 17:52:13 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29eea8dff9fd0ad0a6c1d9943b993b4519c8d7c48140eeb20de7f46fe018e764`  
		Last Modified: Wed, 15 Jan 2020 17:52:13 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-windowsservercore` - windows version 10.0.14393.3443; amd64

```console
$ docker pull nats@sha256:f3b8aa519f1e9981b369d238e46b3e336b2df7654f7cf784b5601d5342a49137
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 GB (5739369423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56ca53177d88b1126a979fb5530e66d83974e1838cecce90ade826949f5ea259`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 02 Jan 2020 15:48:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Jan 2020 15:20:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jan 2020 17:47:08 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:47:10 GMT
ENV NATS_SERVER=2.1.2
# Wed, 15 Jan 2020 17:47:11 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.2/nats-server-v2.1.2-windows-amd64.zip
# Wed, 15 Jan 2020 17:48:21 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jan 2020 17:50:09 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Jan 2020 17:50:10 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:50:12 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:50:14 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:50:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31f9df80631e7b5d379647ee7701ff50e009bd2c03b30a67a0a8e7bba4a26f94`  
		Size: 1.7 GB (1654613376 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:43da502775fb34b738d9f908cb549c2825c04f1451d1039ec99749be127e47ef`  
		Last Modified: Wed, 15 Jan 2020 17:12:02 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6771e606bb5340710c7ec7fa3294903a0a1f901e5c1e79211ee54fc1f074179a`  
		Last Modified: Wed, 15 Jan 2020 17:53:47 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8885516d0bc2df9c7e82fe0aeb847bc83415084fe85a9aed26a03b3b56ae7c`  
		Last Modified: Wed, 15 Jan 2020 17:53:46 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68459b3a704ec7e5908e23d0d52576c68eef20a4b3ede7bf88ec4e3b2321d170`  
		Last Modified: Wed, 15 Jan 2020 17:53:46 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196e19f93e85979cb0240edd67162a54a2e716e7b139c9c7a99882b3dc42fc2a`  
		Last Modified: Wed, 15 Jan 2020 17:53:47 GMT  
		Size: 5.4 MB (5383420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2ec8ad5670f9274bd1b0dbc71a9ac551d4b18d3f6254bf51bbd80049d7d9c2`  
		Last Modified: Wed, 15 Jan 2020 17:53:46 GMT  
		Size: 9.4 MB (9376638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4abd28582063a6691f03037049db18ea066600d7023aa3d2975eb66ea3cafd`  
		Last Modified: Wed, 15 Jan 2020 17:53:43 GMT  
		Size: 1.8 KB (1762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe6eef99ce520e46eef3031fa6ebd7aeba735253cef9dd2b4e7e07255a9efd8`  
		Last Modified: Wed, 15 Jan 2020 17:53:43 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb11317f8d70c8d41b0ec7372f568029527c0809262db66d162a67d82e2ddc4d`  
		Last Modified: Wed, 15 Jan 2020 17:53:42 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3993164e2c009ccf7891a7fb2956b069daf095ac7a081307e8494e594e98fa`  
		Last Modified: Wed, 15 Jan 2020 17:53:43 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-windowsservercore-1803`

```console
$ docker pull nats@sha256:d06f971a89319c413118f67b67dab4e52914ad2540fcd2844f831c2a237c35d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17134.1246; amd64

### `nats:2.1-windowsservercore-1803` - windows version 10.0.17134.1246; amd64

```console
$ docker pull nats@sha256:68c9dff50987d82ca20958b1a5ca7cb816509b6d6b024ecc0a5f83cfe26f5f59
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2368141200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20f6b32275bca4375a3ca4b65ab024126e7ae1c30725dcd7ab47d638bc9c5dbc`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 12 Apr 2018 09:20:54 GMT
RUN Apply image 1803-RTM-amd64
# Wed, 08 Jan 2020 15:30:02 GMT
RUN Install update 1803-amd64
# Wed, 15 Jan 2020 17:44:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jan 2020 17:44:14 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:44:15 GMT
ENV NATS_SERVER=2.1.2
# Wed, 15 Jan 2020 17:44:16 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.2/nats-server-v2.1.2-windows-amd64.zip
# Wed, 15 Jan 2020 17:45:13 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jan 2020 17:46:20 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Jan 2020 17:46:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:46:22 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:46:24 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:46:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d9e8b01179bfc94a5bdb1810fbd76b999aa52016001ace2d3a4c4bc7065a9601`  
		Last Modified: Tue, 18 Sep 2018 22:43:55 GMT  
		Size: 1.7 GB (1659688273 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:270ec3ad3fc7d52c0dd086b32f7751131c799e25cdcd4686cc33cbf2b607c34e`  
		Size: 699.2 MB (699246147 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dbec356e813f8f1863318efd5cd62c261f7de4ac49fc093c648020e26d0520fb`  
		Last Modified: Wed, 15 Jan 2020 17:52:17 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c748a716adbca27bf760bc535221171b42c3dcfd044a49e011295928c66c39`  
		Last Modified: Wed, 15 Jan 2020 17:52:17 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7efb3710bacce94103ccc92d28b0a0af30a9bb7a29f1d7f45fc18a75e959ee2d`  
		Last Modified: Wed, 15 Jan 2020 17:52:16 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883bd0fc138e4a17c679bf7d23bb5f0186ccae58fbacdfda29c147e85e2d9383`  
		Last Modified: Wed, 15 Jan 2020 17:52:15 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967451731bebacb830dc7e26892242d8d5c55f6576f5476820313ac2f35d2550`  
		Last Modified: Wed, 15 Jan 2020 17:52:17 GMT  
		Size: 4.9 MB (4880651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35062fb2b37da05d5d753b6519295e3b14da0bf8fecf57ba90fb507aaf498b7`  
		Last Modified: Wed, 15 Jan 2020 17:52:15 GMT  
		Size: 4.3 MB (4316097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bcb4b1ca97cf159a8a5030f29505c9c52626907a92244c92d25df16333f84bf`  
		Last Modified: Wed, 15 Jan 2020 17:52:13 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a380672454ff5ba95dd36413220fa3f00b7998578a8f32ee0b85cfd6d6f9666`  
		Last Modified: Wed, 15 Jan 2020 17:52:13 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f545bb1274ec20783b4966e6592ba3ca21b327f02552a0480c57eae7bd6a77`  
		Last Modified: Wed, 15 Jan 2020 17:52:13 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29eea8dff9fd0ad0a6c1d9943b993b4519c8d7c48140eeb20de7f46fe018e764`  
		Last Modified: Wed, 15 Jan 2020 17:52:13 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-windowsservercore-1809`

```console
$ docker pull nats@sha256:655dcc67ed8905581e9ef5bbc18c06dbd66da9bea9b4dbfc5baf5e575525438e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64

### `nats:2.1-windowsservercore-1809` - windows version 10.0.17763.973; amd64

```console
$ docker pull nats@sha256:f5ac96a023326f836cf1c02a5f5b30abd128056d648cac3a4643c8125532ec4f
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2230470888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66ed94808574b78075af126587ee0e95fd33c3b8964fbec51c76c08c20bba3d6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Wed, 15 Jan 2020 14:40:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jan 2020 17:41:54 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:41:55 GMT
ENV NATS_SERVER=2.1.2
# Wed, 15 Jan 2020 17:41:56 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.2/nats-server-v2.1.2-windows-amd64.zip
# Wed, 15 Jan 2020 17:42:38 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jan 2020 17:43:46 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Jan 2020 17:43:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:43:49 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:43:50 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:43:52 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2397868e5c7aa285f662aaa9309fa4756277739e11d589a663a204df80595f2c`  
		Last Modified: Wed, 15 Jan 2020 17:10:53 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b23c268ec0520ea9af1e83b69008728041b2a5f234937b9a6272d2a739fd92e`  
		Last Modified: Wed, 15 Jan 2020 17:51:25 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8bf81f9ddd524bd8d7611b92b362a8f558a338e038fb1a81f81872f58a76f7`  
		Last Modified: Wed, 15 Jan 2020 17:51:25 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb3c94fff5bd229bc976399c1904de65b246152cd41d0147af159fd09877822a`  
		Last Modified: Wed, 15 Jan 2020 17:51:24 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e70dcd5f51d264f2ff2ba291ee37e474f5637d236d01c2d5cd8a4ab039dc60`  
		Last Modified: Wed, 15 Jan 2020 17:51:26 GMT  
		Size: 4.5 MB (4548759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b87189fe10fd6d476acc4c0869463fe1f0d813aa1fc2ff3d95efa65f86d7f34`  
		Last Modified: Wed, 15 Jan 2020 17:51:31 GMT  
		Size: 8.5 MB (8500806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a611e13685ceef48268051590fc9cc976fdec2ec0968e3a12fb9b7ef72b6f2`  
		Last Modified: Wed, 15 Jan 2020 17:51:22 GMT  
		Size: 1.8 KB (1763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ebd020bd73cd69b61c2325da491f4c057f7fdeac1f37db60365aef9d9f56e6`  
		Last Modified: Wed, 15 Jan 2020 17:51:22 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2ef97f255816c764614a7a10afa9fa89f6b8fa9c107f24458eab08ad8aee6d`  
		Last Modified: Wed, 15 Jan 2020 17:51:22 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d555934698e4f3eaa1e7fef777b3692d4a519ec978ec5f191be9ea1a772ad6`  
		Last Modified: Wed, 15 Jan 2020 17:51:22 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:b0bab523ef87fed76cbcc206909058cdceace4206e8797b3dc3bb074f8148c9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3443; amd64

### `nats:2.1-windowsservercore-ltsc2016` - windows version 10.0.14393.3443; amd64

```console
$ docker pull nats@sha256:f3b8aa519f1e9981b369d238e46b3e336b2df7654f7cf784b5601d5342a49137
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 GB (5739369423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56ca53177d88b1126a979fb5530e66d83974e1838cecce90ade826949f5ea259`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 02 Jan 2020 15:48:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Jan 2020 15:20:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jan 2020 17:47:08 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:47:10 GMT
ENV NATS_SERVER=2.1.2
# Wed, 15 Jan 2020 17:47:11 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.2/nats-server-v2.1.2-windows-amd64.zip
# Wed, 15 Jan 2020 17:48:21 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jan 2020 17:50:09 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Jan 2020 17:50:10 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:50:12 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:50:14 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:50:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31f9df80631e7b5d379647ee7701ff50e009bd2c03b30a67a0a8e7bba4a26f94`  
		Size: 1.7 GB (1654613376 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:43da502775fb34b738d9f908cb549c2825c04f1451d1039ec99749be127e47ef`  
		Last Modified: Wed, 15 Jan 2020 17:12:02 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6771e606bb5340710c7ec7fa3294903a0a1f901e5c1e79211ee54fc1f074179a`  
		Last Modified: Wed, 15 Jan 2020 17:53:47 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8885516d0bc2df9c7e82fe0aeb847bc83415084fe85a9aed26a03b3b56ae7c`  
		Last Modified: Wed, 15 Jan 2020 17:53:46 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68459b3a704ec7e5908e23d0d52576c68eef20a4b3ede7bf88ec4e3b2321d170`  
		Last Modified: Wed, 15 Jan 2020 17:53:46 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196e19f93e85979cb0240edd67162a54a2e716e7b139c9c7a99882b3dc42fc2a`  
		Last Modified: Wed, 15 Jan 2020 17:53:47 GMT  
		Size: 5.4 MB (5383420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2ec8ad5670f9274bd1b0dbc71a9ac551d4b18d3f6254bf51bbd80049d7d9c2`  
		Last Modified: Wed, 15 Jan 2020 17:53:46 GMT  
		Size: 9.4 MB (9376638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4abd28582063a6691f03037049db18ea066600d7023aa3d2975eb66ea3cafd`  
		Last Modified: Wed, 15 Jan 2020 17:53:43 GMT  
		Size: 1.8 KB (1762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe6eef99ce520e46eef3031fa6ebd7aeba735253cef9dd2b4e7e07255a9efd8`  
		Last Modified: Wed, 15 Jan 2020 17:53:43 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb11317f8d70c8d41b0ec7372f568029527c0809262db66d162a67d82e2ddc4d`  
		Last Modified: Wed, 15 Jan 2020 17:53:42 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3993164e2c009ccf7891a7fb2956b069daf095ac7a081307e8494e594e98fa`  
		Last Modified: Wed, 15 Jan 2020 17:53:43 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:71e945d4d94bfc25dfdb242bad666f2979caef77f1bff75728f1cc72b4804081
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:f507195794f36c37413ca058f5c3442ad24a80facf94cf4779297e4ab0971f99
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7092803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffa6d536d932527718344a90a884bb621e3480d21893e4bf8e4b7e46b05ad957`
-	Default Command: `["nats-server"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 19:19:25 GMT
ENV NATS_SERVER=2.1.2
# Thu, 23 Jan 2020 19:19:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 23 Jan 2020 19:19:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 23 Jan 2020 19:19:29 GMT
EXPOSE 4222 6222 8222
# Thu, 23 Jan 2020 19:19:29 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581b0b35a07f0a300a55e836a3ba0cb3d18061455a6367a15fbd6f127b57351c`  
		Last Modified: Thu, 23 Jan 2020 19:20:29 GMT  
		Size: 4.3 MB (4305310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82a66d5edde56b04466489c0c46457358c6737789e7e4cde197d7b0befe4fa3`  
		Last Modified: Thu, 23 Jan 2020 19:20:28 GMT  
		Size: 531.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:6380d8b1fc432a021689908f6501d49747edf3b3c2bc54134e433c10e77efb1c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6664521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a20dd366129d9b5428c44f6c6853a8297f7b86b3e6b8f20a1600da467f76599`
-	Default Command: `["nats-server"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:27 GMT
ADD file:2aa80d52585a6b34b2cc5811d46965a084e50cfb8cd183f1a88b2b1bc6556e1f in / 
# Thu, 23 Jan 2020 16:53:28 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:44:32 GMT
ENV NATS_SERVER=2.1.2
# Thu, 23 Jan 2020 17:44:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 23 Jan 2020 17:44:39 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 23 Jan 2020 17:44:40 GMT
EXPOSE 4222 6222 8222
# Thu, 23 Jan 2020 17:44:41 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:896868b7b9168cabb308702db96dc9769d10c23e20fc66f5f4abedf4c75d7642`  
		Last Modified: Thu, 23 Jan 2020 16:54:07 GMT  
		Size: 2.6 MB (2571407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f146c76b464f3790626809adda3914591425f7cd06759a183ccd5da25e26bb82`  
		Last Modified: Thu, 23 Jan 2020 17:45:13 GMT  
		Size: 4.1 MB (4092555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162410de1cd5b2c2ce2cd44dc7973ff2511dc755faeca556ea9e69b1aa55fae3`  
		Last Modified: Thu, 23 Jan 2020 17:45:12 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:d60f1b23e6d2ce2e8edac172e464de946fa830452af16b709c8d3c8234a3c045
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6466632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d154ea04a5c19abf9bcf38dacc8b82bee649c6c507024227c5cd298ed1ac75c6`
-	Default Command: `["nats-server"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:31 GMT
ADD file:d05c9f9143d11d12045d4faef882e5985e6b38fabe52237dd8d8c0627a9620ab in / 
# Thu, 23 Jan 2020 16:53:32 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:55:25 GMT
ENV NATS_SERVER=2.1.2
# Thu, 23 Jan 2020 17:55:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 23 Jan 2020 17:55:30 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 23 Jan 2020 17:55:31 GMT
EXPOSE 4222 6222 8222
# Thu, 23 Jan 2020 17:55:32 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:4e972d957a606327b0b6c2e8aa4a6045c263b7496a536298aaebf690e9d85f1d`  
		Last Modified: Thu, 23 Jan 2020 16:53:59 GMT  
		Size: 2.4 MB (2378408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c375dc9edf38cadcfdc6537707cdea65e2b45d840940712d2f88d19cc967edc6`  
		Last Modified: Thu, 23 Jan 2020 17:56:08 GMT  
		Size: 4.1 MB (4087666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bfcd4ad511455617c2f402e3d5ebd12e714c0d9a0d280f7399735754fab756e`  
		Last Modified: Thu, 23 Jan 2020 17:56:08 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.10`

```console
$ docker pull nats@sha256:71e945d4d94bfc25dfdb242bad666f2979caef77f1bff75728f1cc72b4804081
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats:2-alpine3.10` - linux; amd64

```console
$ docker pull nats@sha256:f507195794f36c37413ca058f5c3442ad24a80facf94cf4779297e4ab0971f99
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7092803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffa6d536d932527718344a90a884bb621e3480d21893e4bf8e4b7e46b05ad957`
-	Default Command: `["nats-server"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 19:19:25 GMT
ENV NATS_SERVER=2.1.2
# Thu, 23 Jan 2020 19:19:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 23 Jan 2020 19:19:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 23 Jan 2020 19:19:29 GMT
EXPOSE 4222 6222 8222
# Thu, 23 Jan 2020 19:19:29 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581b0b35a07f0a300a55e836a3ba0cb3d18061455a6367a15fbd6f127b57351c`  
		Last Modified: Thu, 23 Jan 2020 19:20:29 GMT  
		Size: 4.3 MB (4305310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82a66d5edde56b04466489c0c46457358c6737789e7e4cde197d7b0befe4fa3`  
		Last Modified: Thu, 23 Jan 2020 19:20:28 GMT  
		Size: 531.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.10` - linux; arm variant v6

```console
$ docker pull nats@sha256:6380d8b1fc432a021689908f6501d49747edf3b3c2bc54134e433c10e77efb1c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6664521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a20dd366129d9b5428c44f6c6853a8297f7b86b3e6b8f20a1600da467f76599`
-	Default Command: `["nats-server"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:27 GMT
ADD file:2aa80d52585a6b34b2cc5811d46965a084e50cfb8cd183f1a88b2b1bc6556e1f in / 
# Thu, 23 Jan 2020 16:53:28 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:44:32 GMT
ENV NATS_SERVER=2.1.2
# Thu, 23 Jan 2020 17:44:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 23 Jan 2020 17:44:39 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 23 Jan 2020 17:44:40 GMT
EXPOSE 4222 6222 8222
# Thu, 23 Jan 2020 17:44:41 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:896868b7b9168cabb308702db96dc9769d10c23e20fc66f5f4abedf4c75d7642`  
		Last Modified: Thu, 23 Jan 2020 16:54:07 GMT  
		Size: 2.6 MB (2571407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f146c76b464f3790626809adda3914591425f7cd06759a183ccd5da25e26bb82`  
		Last Modified: Thu, 23 Jan 2020 17:45:13 GMT  
		Size: 4.1 MB (4092555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162410de1cd5b2c2ce2cd44dc7973ff2511dc755faeca556ea9e69b1aa55fae3`  
		Last Modified: Thu, 23 Jan 2020 17:45:12 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.10` - linux; arm variant v7

```console
$ docker pull nats@sha256:d60f1b23e6d2ce2e8edac172e464de946fa830452af16b709c8d3c8234a3c045
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6466632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d154ea04a5c19abf9bcf38dacc8b82bee649c6c507024227c5cd298ed1ac75c6`
-	Default Command: `["nats-server"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:31 GMT
ADD file:d05c9f9143d11d12045d4faef882e5985e6b38fabe52237dd8d8c0627a9620ab in / 
# Thu, 23 Jan 2020 16:53:32 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:55:25 GMT
ENV NATS_SERVER=2.1.2
# Thu, 23 Jan 2020 17:55:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 23 Jan 2020 17:55:30 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 23 Jan 2020 17:55:31 GMT
EXPOSE 4222 6222 8222
# Thu, 23 Jan 2020 17:55:32 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:4e972d957a606327b0b6c2e8aa4a6045c263b7496a536298aaebf690e9d85f1d`  
		Last Modified: Thu, 23 Jan 2020 16:53:59 GMT  
		Size: 2.4 MB (2378408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c375dc9edf38cadcfdc6537707cdea65e2b45d840940712d2f88d19cc967edc6`  
		Last Modified: Thu, 23 Jan 2020 17:56:08 GMT  
		Size: 4.1 MB (4087666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bfcd4ad511455617c2f402e3d5ebd12e714c0d9a0d280f7399735754fab756e`  
		Last Modified: Thu, 23 Jan 2020 17:56:08 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:59141670457fa112c6b1cf5cca3b159ad15bfb7e70fe0b1acbbb5616d922a3c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:8139c5bf4df6e8635cb3420d2dfab08ecdf75b8d16cd82c40a67bd4417b2e71c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (4002673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49014ccb53efc06dc1ce6656aea0abf000881d9db3ac5b31c6f8aef934452b30`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Nov 2019 01:14:07 GMT
COPY file:f7ba6139c8151888be538812698c1aab4311e97fcfac3b5af13138cd7d7e1405 in /nats-server 
# Wed, 20 Nov 2019 01:14:07 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 20 Nov 2019 01:14:08 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Nov 2019 01:14:08 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Nov 2019 01:14:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f3c8f35bd9bcd03ff8eba7551a59aa4fb56c5eabac4758b0b6cb12709785f25c`  
		Last Modified: Wed, 20 Nov 2019 01:14:44 GMT  
		Size: 4.0 MB (4002195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba25f2430b4efc5a2c8e36c142c7aca0b9a14a6caf16fe09d29f97f77f4efce`  
		Last Modified: Wed, 20 Nov 2019 01:14:43 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:234935205b93b7c99b67d82fe35226290aa302e2b35b32f7f9516aa770bf6003
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3790304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66f838f1a59cd8673948823057d50b486bb443ce5318e5a24502ded16334feda`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Nov 2019 00:04:38 GMT
COPY file:1c509c11a9e5697ac3184dd6c0dca46386d2a5d22fabbd0f4898bad8342884d8 in /nats-server 
# Wed, 20 Nov 2019 00:04:39 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 20 Nov 2019 00:04:39 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Nov 2019 00:04:40 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Nov 2019 00:04:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ab4822bfc4bb3725c051563099752bf9f3cc14db9a698a66f64c906201e88b2d`  
		Last Modified: Wed, 20 Nov 2019 00:05:19 GMT  
		Size: 3.8 MB (3789828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd9cf11d4796d35bb8140733b85f1398c199c592ad417cb6d22eac97b0ac377`  
		Last Modified: Wed, 20 Nov 2019 00:05:18 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:92ea09078a55fc56a807ede1630a862d4b6acc12633391a5a42b41483c6b66fa
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3786713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df9b97d154301cbefd42558306e1ece9667269fb9bda4c0ff2c2f601b578c2c8`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Nov 2019 00:53:13 GMT
COPY file:f7bd56432332a04229b22e2b4ed52b31e5ba863bb47a2aacf6d808bd4a8397d1 in /nats-server 
# Wed, 20 Nov 2019 00:53:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 20 Nov 2019 00:53:15 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Nov 2019 00:53:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Nov 2019 00:53:19 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:27216bfb43f9e231372de919d3bbc108e604422a1019a0b0407001997c0575fe`  
		Last Modified: Wed, 20 Nov 2019 00:54:09 GMT  
		Size: 3.8 MB (3786237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3750c7c4312b8b2af995298314a15791a97ce1ef156b81c0477e579fb42b7f2e`  
		Last Modified: Wed, 20 Nov 2019 00:54:09 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:284c4850adc39c33100ab1324dbe23ddde7450c6e5bd15da874d459e68e0ea3e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3665772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeda44c76561e9490c8a19cffd362e26a5552c3aafd41c98b9562a6ae8a01874`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 20 Sep 2019 23:29:17 GMT
COPY file:f0dce6fb207b92a78774313458c6030a8ac0653785d2a2d54e8b5c8935d9b6b8 in /nats-server 
# Fri, 18 Oct 2019 18:04:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 18 Oct 2019 18:04:47 GMT
EXPOSE 4222 6222 8222
# Fri, 18 Oct 2019 18:04:48 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 18 Oct 2019 18:04:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:98fcb931241702ef0a04aa16bb1e4bab6b8afd06f792790462dff69dee05835c`  
		Last Modified: Fri, 20 Sep 2019 23:29:32 GMT  
		Size: 3.7 MB (3665294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e761cba9328047725686c1ed6eecd9eeef33879d348aea70fb3d219b546165`  
		Last Modified: Fri, 18 Oct 2019 18:05:08 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:d028e8a1c50120304d4111bb1214475e11f3684b7176df24a5ec7b00f650decb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64
	-	windows version 10.0.17134.1246; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.973; amd64

```console
$ docker pull nats@sha256:fe1ec52862c24ed520cc33ba713ca2a1ab61132fe67f8e4271dd3d54739175bf
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105047963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d2592fd645781c520143281ac28e8f8eba6f4184b893dd1f41c47f4cfea6e22`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 04 Jan 2020 07:17:17 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jan 2020 17:50:29 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:50:31 GMT
RUN cmd /S /C #(nop) COPY file:a9e3f6c9790c912d513d2134dc1f68e02a9edf34862dd584010eae5ab8418108 in C:\nats-server.exe 
# Wed, 15 Jan 2020 17:50:33 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:50:34 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:50:36 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:50:37 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ee446884f7bef76f8275c2f16add1c4fb598bea2ba861e72bce8fb4aac9b55ef`  
		Size: 101.1 MB (101054324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95d31e7189792498b758db35ae56b1ca97128d8063404cbe62a32205d08d1d4a`  
		Last Modified: Wed, 15 Jan 2020 17:54:30 GMT  
		Size: 940.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06dd0cb87c9a67456f9c940ed213536b3e08acb7279b65835e3c65a7654d86f3`  
		Last Modified: Wed, 15 Jan 2020 17:54:30 GMT  
		Size: 4.0 MB (3988335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a3fd5110f7e9b5b9bdf1dcaa1d44324372e6327142443cd9886d09870d8897e`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 1.6 KB (1560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc491f53dd9a291eef7348c3086782cb45ddb7d249aa3fcd080d0dcc05dc8000`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 939.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8053efdd66e716af07b38c62c28b0878f99af0173a9360e403074367593dcc1`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 942.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3215e4233ac1a2ec100e0e6d20af8633eebf5fce1e5813077fdbab6deb27fbb`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-nanoserver` - windows version 10.0.17134.1246; amd64

```console
$ docker pull nats@sha256:5f107d9f832b82ff068741b598503279a5c98f7239c376ba43f9e9e63eb46e9a
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.9 MB (157902423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b01104ee474980123a7757c086644468acfb2f4883fb483597c3db674d4181a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 11 Apr 2018 22:12:30 GMT
RUN Apply image 1803-RTM-amd64
# Wed, 08 Jan 2020 15:12:42 GMT
RUN Install update 1803-amd64
# Wed, 15 Jan 2020 17:46:46 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:46:49 GMT
RUN cmd /S /C #(nop) COPY file:a9e3f6c9790c912d513d2134dc1f68e02a9edf34862dd584010eae5ab8418108 in C:\nats-server.exe 
# Wed, 15 Jan 2020 17:46:50 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:46:52 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:46:53 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:46:54 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e46172273a4e4384e1eec7fb01091c828a256ea0f87b30f61381fba9bc511371`  
		Last Modified: Mon, 17 Sep 2018 20:23:30 GMT  
		Size: 92.8 MB (92818888 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c0783c3b88b74a9de609bda64fc01cd5e23fb65d57e750a9c584e8a9ed842fa9`  
		Size: 61.1 MB (61089912 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:24f456fbaddb9e6d59a1ebc9e9244a4b7b003b467f4379a121463c469fe5ac34`  
		Last Modified: Wed, 15 Jan 2020 17:53:01 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2280cf6b56b3522c9f82db3208ab840d8e3292ec7d042eb1d7d4c00319b640`  
		Last Modified: Wed, 15 Jan 2020 17:53:01 GMT  
		Size: 4.0 MB (3988299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c0024dc7e88bada373f0f9593d8ca873d955ddef73363bd42f421f37a339598`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 1.6 KB (1555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d6c860f0094966bd95e3a9b933773c4aa19466f9b337f383aa138b5b41ab22`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15569096640ccf86ed6b731f1e8ecac13947a7bfe4fdaa0b9800f7484bb266c4`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 951.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c849d8e8a6767e0308da9ac7027ca2eecb68424c8d4d748989768b7f920283`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1803`

```console
$ docker pull nats@sha256:9c4a8412f1acfb6279840bdb68e678c0e848b259196fecef0d4ea62c120654c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17134.1246; amd64

### `nats:2-nanoserver-1803` - windows version 10.0.17134.1246; amd64

```console
$ docker pull nats@sha256:5f107d9f832b82ff068741b598503279a5c98f7239c376ba43f9e9e63eb46e9a
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.9 MB (157902423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b01104ee474980123a7757c086644468acfb2f4883fb483597c3db674d4181a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 11 Apr 2018 22:12:30 GMT
RUN Apply image 1803-RTM-amd64
# Wed, 08 Jan 2020 15:12:42 GMT
RUN Install update 1803-amd64
# Wed, 15 Jan 2020 17:46:46 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:46:49 GMT
RUN cmd /S /C #(nop) COPY file:a9e3f6c9790c912d513d2134dc1f68e02a9edf34862dd584010eae5ab8418108 in C:\nats-server.exe 
# Wed, 15 Jan 2020 17:46:50 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:46:52 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:46:53 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:46:54 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e46172273a4e4384e1eec7fb01091c828a256ea0f87b30f61381fba9bc511371`  
		Last Modified: Mon, 17 Sep 2018 20:23:30 GMT  
		Size: 92.8 MB (92818888 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c0783c3b88b74a9de609bda64fc01cd5e23fb65d57e750a9c584e8a9ed842fa9`  
		Size: 61.1 MB (61089912 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:24f456fbaddb9e6d59a1ebc9e9244a4b7b003b467f4379a121463c469fe5ac34`  
		Last Modified: Wed, 15 Jan 2020 17:53:01 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2280cf6b56b3522c9f82db3208ab840d8e3292ec7d042eb1d7d4c00319b640`  
		Last Modified: Wed, 15 Jan 2020 17:53:01 GMT  
		Size: 4.0 MB (3988299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c0024dc7e88bada373f0f9593d8ca873d955ddef73363bd42f421f37a339598`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 1.6 KB (1555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d6c860f0094966bd95e3a9b933773c4aa19466f9b337f383aa138b5b41ab22`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15569096640ccf86ed6b731f1e8ecac13947a7bfe4fdaa0b9800f7484bb266c4`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 951.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c849d8e8a6767e0308da9ac7027ca2eecb68424c8d4d748989768b7f920283`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:35356d98d96477f83eab4060656843a014506567dc5ad5c2acea557bd05c69b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.973; amd64

```console
$ docker pull nats@sha256:fe1ec52862c24ed520cc33ba713ca2a1ab61132fe67f8e4271dd3d54739175bf
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105047963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d2592fd645781c520143281ac28e8f8eba6f4184b893dd1f41c47f4cfea6e22`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 04 Jan 2020 07:17:17 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jan 2020 17:50:29 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:50:31 GMT
RUN cmd /S /C #(nop) COPY file:a9e3f6c9790c912d513d2134dc1f68e02a9edf34862dd584010eae5ab8418108 in C:\nats-server.exe 
# Wed, 15 Jan 2020 17:50:33 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:50:34 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:50:36 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:50:37 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ee446884f7bef76f8275c2f16add1c4fb598bea2ba861e72bce8fb4aac9b55ef`  
		Size: 101.1 MB (101054324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95d31e7189792498b758db35ae56b1ca97128d8063404cbe62a32205d08d1d4a`  
		Last Modified: Wed, 15 Jan 2020 17:54:30 GMT  
		Size: 940.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06dd0cb87c9a67456f9c940ed213536b3e08acb7279b65835e3c65a7654d86f3`  
		Last Modified: Wed, 15 Jan 2020 17:54:30 GMT  
		Size: 4.0 MB (3988335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a3fd5110f7e9b5b9bdf1dcaa1d44324372e6327142443cd9886d09870d8897e`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 1.6 KB (1560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc491f53dd9a291eef7348c3086782cb45ddb7d249aa3fcd080d0dcc05dc8000`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 939.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8053efdd66e716af07b38c62c28b0878f99af0173a9360e403074367593dcc1`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 942.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3215e4233ac1a2ec100e0e6d20af8633eebf5fce1e5813077fdbab6deb27fbb`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:59141670457fa112c6b1cf5cca3b159ad15bfb7e70fe0b1acbbb5616d922a3c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:8139c5bf4df6e8635cb3420d2dfab08ecdf75b8d16cd82c40a67bd4417b2e71c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (4002673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49014ccb53efc06dc1ce6656aea0abf000881d9db3ac5b31c6f8aef934452b30`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Nov 2019 01:14:07 GMT
COPY file:f7ba6139c8151888be538812698c1aab4311e97fcfac3b5af13138cd7d7e1405 in /nats-server 
# Wed, 20 Nov 2019 01:14:07 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 20 Nov 2019 01:14:08 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Nov 2019 01:14:08 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Nov 2019 01:14:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f3c8f35bd9bcd03ff8eba7551a59aa4fb56c5eabac4758b0b6cb12709785f25c`  
		Last Modified: Wed, 20 Nov 2019 01:14:44 GMT  
		Size: 4.0 MB (4002195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba25f2430b4efc5a2c8e36c142c7aca0b9a14a6caf16fe09d29f97f77f4efce`  
		Last Modified: Wed, 20 Nov 2019 01:14:43 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:234935205b93b7c99b67d82fe35226290aa302e2b35b32f7f9516aa770bf6003
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3790304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66f838f1a59cd8673948823057d50b486bb443ce5318e5a24502ded16334feda`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Nov 2019 00:04:38 GMT
COPY file:1c509c11a9e5697ac3184dd6c0dca46386d2a5d22fabbd0f4898bad8342884d8 in /nats-server 
# Wed, 20 Nov 2019 00:04:39 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 20 Nov 2019 00:04:39 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Nov 2019 00:04:40 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Nov 2019 00:04:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ab4822bfc4bb3725c051563099752bf9f3cc14db9a698a66f64c906201e88b2d`  
		Last Modified: Wed, 20 Nov 2019 00:05:19 GMT  
		Size: 3.8 MB (3789828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd9cf11d4796d35bb8140733b85f1398c199c592ad417cb6d22eac97b0ac377`  
		Last Modified: Wed, 20 Nov 2019 00:05:18 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:92ea09078a55fc56a807ede1630a862d4b6acc12633391a5a42b41483c6b66fa
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3786713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df9b97d154301cbefd42558306e1ece9667269fb9bda4c0ff2c2f601b578c2c8`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Nov 2019 00:53:13 GMT
COPY file:f7bd56432332a04229b22e2b4ed52b31e5ba863bb47a2aacf6d808bd4a8397d1 in /nats-server 
# Wed, 20 Nov 2019 00:53:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 20 Nov 2019 00:53:15 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Nov 2019 00:53:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Nov 2019 00:53:19 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:27216bfb43f9e231372de919d3bbc108e604422a1019a0b0407001997c0575fe`  
		Last Modified: Wed, 20 Nov 2019 00:54:09 GMT  
		Size: 3.8 MB (3786237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3750c7c4312b8b2af995298314a15791a97ce1ef156b81c0477e579fb42b7f2e`  
		Last Modified: Wed, 20 Nov 2019 00:54:09 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:284c4850adc39c33100ab1324dbe23ddde7450c6e5bd15da874d459e68e0ea3e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3665772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeda44c76561e9490c8a19cffd362e26a5552c3aafd41c98b9562a6ae8a01874`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 20 Sep 2019 23:29:17 GMT
COPY file:f0dce6fb207b92a78774313458c6030a8ac0653785d2a2d54e8b5c8935d9b6b8 in /nats-server 
# Fri, 18 Oct 2019 18:04:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 18 Oct 2019 18:04:47 GMT
EXPOSE 4222 6222 8222
# Fri, 18 Oct 2019 18:04:48 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 18 Oct 2019 18:04:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:98fcb931241702ef0a04aa16bb1e4bab6b8afd06f792790462dff69dee05835c`  
		Last Modified: Fri, 20 Sep 2019 23:29:32 GMT  
		Size: 3.7 MB (3665294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e761cba9328047725686c1ed6eecd9eeef33879d348aea70fb3d219b546165`  
		Last Modified: Fri, 18 Oct 2019 18:05:08 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:a42f0c67634d642f56a78fcc79c12b8d5d4da81b34b93f1ccb103ba2743f6e23
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64
	-	windows version 10.0.17134.1246; amd64
	-	windows version 10.0.14393.3443; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.973; amd64

```console
$ docker pull nats@sha256:f5ac96a023326f836cf1c02a5f5b30abd128056d648cac3a4643c8125532ec4f
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2230470888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66ed94808574b78075af126587ee0e95fd33c3b8964fbec51c76c08c20bba3d6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Wed, 15 Jan 2020 14:40:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jan 2020 17:41:54 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:41:55 GMT
ENV NATS_SERVER=2.1.2
# Wed, 15 Jan 2020 17:41:56 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.2/nats-server-v2.1.2-windows-amd64.zip
# Wed, 15 Jan 2020 17:42:38 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jan 2020 17:43:46 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Jan 2020 17:43:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:43:49 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:43:50 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:43:52 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2397868e5c7aa285f662aaa9309fa4756277739e11d589a663a204df80595f2c`  
		Last Modified: Wed, 15 Jan 2020 17:10:53 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b23c268ec0520ea9af1e83b69008728041b2a5f234937b9a6272d2a739fd92e`  
		Last Modified: Wed, 15 Jan 2020 17:51:25 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8bf81f9ddd524bd8d7611b92b362a8f558a338e038fb1a81f81872f58a76f7`  
		Last Modified: Wed, 15 Jan 2020 17:51:25 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb3c94fff5bd229bc976399c1904de65b246152cd41d0147af159fd09877822a`  
		Last Modified: Wed, 15 Jan 2020 17:51:24 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e70dcd5f51d264f2ff2ba291ee37e474f5637d236d01c2d5cd8a4ab039dc60`  
		Last Modified: Wed, 15 Jan 2020 17:51:26 GMT  
		Size: 4.5 MB (4548759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b87189fe10fd6d476acc4c0869463fe1f0d813aa1fc2ff3d95efa65f86d7f34`  
		Last Modified: Wed, 15 Jan 2020 17:51:31 GMT  
		Size: 8.5 MB (8500806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a611e13685ceef48268051590fc9cc976fdec2ec0968e3a12fb9b7ef72b6f2`  
		Last Modified: Wed, 15 Jan 2020 17:51:22 GMT  
		Size: 1.8 KB (1763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ebd020bd73cd69b61c2325da491f4c057f7fdeac1f37db60365aef9d9f56e6`  
		Last Modified: Wed, 15 Jan 2020 17:51:22 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2ef97f255816c764614a7a10afa9fa89f6b8fa9c107f24458eab08ad8aee6d`  
		Last Modified: Wed, 15 Jan 2020 17:51:22 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d555934698e4f3eaa1e7fef777b3692d4a519ec978ec5f191be9ea1a772ad6`  
		Last Modified: Wed, 15 Jan 2020 17:51:22 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-windowsservercore` - windows version 10.0.17134.1246; amd64

```console
$ docker pull nats@sha256:68c9dff50987d82ca20958b1a5ca7cb816509b6d6b024ecc0a5f83cfe26f5f59
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2368141200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20f6b32275bca4375a3ca4b65ab024126e7ae1c30725dcd7ab47d638bc9c5dbc`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 12 Apr 2018 09:20:54 GMT
RUN Apply image 1803-RTM-amd64
# Wed, 08 Jan 2020 15:30:02 GMT
RUN Install update 1803-amd64
# Wed, 15 Jan 2020 17:44:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jan 2020 17:44:14 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:44:15 GMT
ENV NATS_SERVER=2.1.2
# Wed, 15 Jan 2020 17:44:16 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.2/nats-server-v2.1.2-windows-amd64.zip
# Wed, 15 Jan 2020 17:45:13 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jan 2020 17:46:20 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Jan 2020 17:46:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:46:22 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:46:24 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:46:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d9e8b01179bfc94a5bdb1810fbd76b999aa52016001ace2d3a4c4bc7065a9601`  
		Last Modified: Tue, 18 Sep 2018 22:43:55 GMT  
		Size: 1.7 GB (1659688273 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:270ec3ad3fc7d52c0dd086b32f7751131c799e25cdcd4686cc33cbf2b607c34e`  
		Size: 699.2 MB (699246147 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dbec356e813f8f1863318efd5cd62c261f7de4ac49fc093c648020e26d0520fb`  
		Last Modified: Wed, 15 Jan 2020 17:52:17 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c748a716adbca27bf760bc535221171b42c3dcfd044a49e011295928c66c39`  
		Last Modified: Wed, 15 Jan 2020 17:52:17 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7efb3710bacce94103ccc92d28b0a0af30a9bb7a29f1d7f45fc18a75e959ee2d`  
		Last Modified: Wed, 15 Jan 2020 17:52:16 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883bd0fc138e4a17c679bf7d23bb5f0186ccae58fbacdfda29c147e85e2d9383`  
		Last Modified: Wed, 15 Jan 2020 17:52:15 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967451731bebacb830dc7e26892242d8d5c55f6576f5476820313ac2f35d2550`  
		Last Modified: Wed, 15 Jan 2020 17:52:17 GMT  
		Size: 4.9 MB (4880651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35062fb2b37da05d5d753b6519295e3b14da0bf8fecf57ba90fb507aaf498b7`  
		Last Modified: Wed, 15 Jan 2020 17:52:15 GMT  
		Size: 4.3 MB (4316097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bcb4b1ca97cf159a8a5030f29505c9c52626907a92244c92d25df16333f84bf`  
		Last Modified: Wed, 15 Jan 2020 17:52:13 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a380672454ff5ba95dd36413220fa3f00b7998578a8f32ee0b85cfd6d6f9666`  
		Last Modified: Wed, 15 Jan 2020 17:52:13 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f545bb1274ec20783b4966e6592ba3ca21b327f02552a0480c57eae7bd6a77`  
		Last Modified: Wed, 15 Jan 2020 17:52:13 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29eea8dff9fd0ad0a6c1d9943b993b4519c8d7c48140eeb20de7f46fe018e764`  
		Last Modified: Wed, 15 Jan 2020 17:52:13 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-windowsservercore` - windows version 10.0.14393.3443; amd64

```console
$ docker pull nats@sha256:f3b8aa519f1e9981b369d238e46b3e336b2df7654f7cf784b5601d5342a49137
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 GB (5739369423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56ca53177d88b1126a979fb5530e66d83974e1838cecce90ade826949f5ea259`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 02 Jan 2020 15:48:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Jan 2020 15:20:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jan 2020 17:47:08 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:47:10 GMT
ENV NATS_SERVER=2.1.2
# Wed, 15 Jan 2020 17:47:11 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.2/nats-server-v2.1.2-windows-amd64.zip
# Wed, 15 Jan 2020 17:48:21 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jan 2020 17:50:09 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Jan 2020 17:50:10 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:50:12 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:50:14 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:50:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31f9df80631e7b5d379647ee7701ff50e009bd2c03b30a67a0a8e7bba4a26f94`  
		Size: 1.7 GB (1654613376 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:43da502775fb34b738d9f908cb549c2825c04f1451d1039ec99749be127e47ef`  
		Last Modified: Wed, 15 Jan 2020 17:12:02 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6771e606bb5340710c7ec7fa3294903a0a1f901e5c1e79211ee54fc1f074179a`  
		Last Modified: Wed, 15 Jan 2020 17:53:47 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8885516d0bc2df9c7e82fe0aeb847bc83415084fe85a9aed26a03b3b56ae7c`  
		Last Modified: Wed, 15 Jan 2020 17:53:46 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68459b3a704ec7e5908e23d0d52576c68eef20a4b3ede7bf88ec4e3b2321d170`  
		Last Modified: Wed, 15 Jan 2020 17:53:46 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196e19f93e85979cb0240edd67162a54a2e716e7b139c9c7a99882b3dc42fc2a`  
		Last Modified: Wed, 15 Jan 2020 17:53:47 GMT  
		Size: 5.4 MB (5383420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2ec8ad5670f9274bd1b0dbc71a9ac551d4b18d3f6254bf51bbd80049d7d9c2`  
		Last Modified: Wed, 15 Jan 2020 17:53:46 GMT  
		Size: 9.4 MB (9376638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4abd28582063a6691f03037049db18ea066600d7023aa3d2975eb66ea3cafd`  
		Last Modified: Wed, 15 Jan 2020 17:53:43 GMT  
		Size: 1.8 KB (1762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe6eef99ce520e46eef3031fa6ebd7aeba735253cef9dd2b4e7e07255a9efd8`  
		Last Modified: Wed, 15 Jan 2020 17:53:43 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb11317f8d70c8d41b0ec7372f568029527c0809262db66d162a67d82e2ddc4d`  
		Last Modified: Wed, 15 Jan 2020 17:53:42 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3993164e2c009ccf7891a7fb2956b069daf095ac7a081307e8494e594e98fa`  
		Last Modified: Wed, 15 Jan 2020 17:53:43 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1803`

```console
$ docker pull nats@sha256:d06f971a89319c413118f67b67dab4e52914ad2540fcd2844f831c2a237c35d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17134.1246; amd64

### `nats:2-windowsservercore-1803` - windows version 10.0.17134.1246; amd64

```console
$ docker pull nats@sha256:68c9dff50987d82ca20958b1a5ca7cb816509b6d6b024ecc0a5f83cfe26f5f59
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2368141200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20f6b32275bca4375a3ca4b65ab024126e7ae1c30725dcd7ab47d638bc9c5dbc`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 12 Apr 2018 09:20:54 GMT
RUN Apply image 1803-RTM-amd64
# Wed, 08 Jan 2020 15:30:02 GMT
RUN Install update 1803-amd64
# Wed, 15 Jan 2020 17:44:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jan 2020 17:44:14 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:44:15 GMT
ENV NATS_SERVER=2.1.2
# Wed, 15 Jan 2020 17:44:16 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.2/nats-server-v2.1.2-windows-amd64.zip
# Wed, 15 Jan 2020 17:45:13 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jan 2020 17:46:20 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Jan 2020 17:46:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:46:22 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:46:24 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:46:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d9e8b01179bfc94a5bdb1810fbd76b999aa52016001ace2d3a4c4bc7065a9601`  
		Last Modified: Tue, 18 Sep 2018 22:43:55 GMT  
		Size: 1.7 GB (1659688273 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:270ec3ad3fc7d52c0dd086b32f7751131c799e25cdcd4686cc33cbf2b607c34e`  
		Size: 699.2 MB (699246147 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dbec356e813f8f1863318efd5cd62c261f7de4ac49fc093c648020e26d0520fb`  
		Last Modified: Wed, 15 Jan 2020 17:52:17 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c748a716adbca27bf760bc535221171b42c3dcfd044a49e011295928c66c39`  
		Last Modified: Wed, 15 Jan 2020 17:52:17 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7efb3710bacce94103ccc92d28b0a0af30a9bb7a29f1d7f45fc18a75e959ee2d`  
		Last Modified: Wed, 15 Jan 2020 17:52:16 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883bd0fc138e4a17c679bf7d23bb5f0186ccae58fbacdfda29c147e85e2d9383`  
		Last Modified: Wed, 15 Jan 2020 17:52:15 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967451731bebacb830dc7e26892242d8d5c55f6576f5476820313ac2f35d2550`  
		Last Modified: Wed, 15 Jan 2020 17:52:17 GMT  
		Size: 4.9 MB (4880651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35062fb2b37da05d5d753b6519295e3b14da0bf8fecf57ba90fb507aaf498b7`  
		Last Modified: Wed, 15 Jan 2020 17:52:15 GMT  
		Size: 4.3 MB (4316097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bcb4b1ca97cf159a8a5030f29505c9c52626907a92244c92d25df16333f84bf`  
		Last Modified: Wed, 15 Jan 2020 17:52:13 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a380672454ff5ba95dd36413220fa3f00b7998578a8f32ee0b85cfd6d6f9666`  
		Last Modified: Wed, 15 Jan 2020 17:52:13 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f545bb1274ec20783b4966e6592ba3ca21b327f02552a0480c57eae7bd6a77`  
		Last Modified: Wed, 15 Jan 2020 17:52:13 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29eea8dff9fd0ad0a6c1d9943b993b4519c8d7c48140eeb20de7f46fe018e764`  
		Last Modified: Wed, 15 Jan 2020 17:52:13 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:655dcc67ed8905581e9ef5bbc18c06dbd66da9bea9b4dbfc5baf5e575525438e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.973; amd64

```console
$ docker pull nats@sha256:f5ac96a023326f836cf1c02a5f5b30abd128056d648cac3a4643c8125532ec4f
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2230470888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66ed94808574b78075af126587ee0e95fd33c3b8964fbec51c76c08c20bba3d6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Wed, 15 Jan 2020 14:40:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jan 2020 17:41:54 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:41:55 GMT
ENV NATS_SERVER=2.1.2
# Wed, 15 Jan 2020 17:41:56 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.2/nats-server-v2.1.2-windows-amd64.zip
# Wed, 15 Jan 2020 17:42:38 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jan 2020 17:43:46 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Jan 2020 17:43:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:43:49 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:43:50 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:43:52 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2397868e5c7aa285f662aaa9309fa4756277739e11d589a663a204df80595f2c`  
		Last Modified: Wed, 15 Jan 2020 17:10:53 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b23c268ec0520ea9af1e83b69008728041b2a5f234937b9a6272d2a739fd92e`  
		Last Modified: Wed, 15 Jan 2020 17:51:25 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8bf81f9ddd524bd8d7611b92b362a8f558a338e038fb1a81f81872f58a76f7`  
		Last Modified: Wed, 15 Jan 2020 17:51:25 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb3c94fff5bd229bc976399c1904de65b246152cd41d0147af159fd09877822a`  
		Last Modified: Wed, 15 Jan 2020 17:51:24 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e70dcd5f51d264f2ff2ba291ee37e474f5637d236d01c2d5cd8a4ab039dc60`  
		Last Modified: Wed, 15 Jan 2020 17:51:26 GMT  
		Size: 4.5 MB (4548759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b87189fe10fd6d476acc4c0869463fe1f0d813aa1fc2ff3d95efa65f86d7f34`  
		Last Modified: Wed, 15 Jan 2020 17:51:31 GMT  
		Size: 8.5 MB (8500806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a611e13685ceef48268051590fc9cc976fdec2ec0968e3a12fb9b7ef72b6f2`  
		Last Modified: Wed, 15 Jan 2020 17:51:22 GMT  
		Size: 1.8 KB (1763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ebd020bd73cd69b61c2325da491f4c057f7fdeac1f37db60365aef9d9f56e6`  
		Last Modified: Wed, 15 Jan 2020 17:51:22 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2ef97f255816c764614a7a10afa9fa89f6b8fa9c107f24458eab08ad8aee6d`  
		Last Modified: Wed, 15 Jan 2020 17:51:22 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d555934698e4f3eaa1e7fef777b3692d4a519ec978ec5f191be9ea1a772ad6`  
		Last Modified: Wed, 15 Jan 2020 17:51:22 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:b0bab523ef87fed76cbcc206909058cdceace4206e8797b3dc3bb074f8148c9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3443; amd64

### `nats:2-windowsservercore-ltsc2016` - windows version 10.0.14393.3443; amd64

```console
$ docker pull nats@sha256:f3b8aa519f1e9981b369d238e46b3e336b2df7654f7cf784b5601d5342a49137
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 GB (5739369423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56ca53177d88b1126a979fb5530e66d83974e1838cecce90ade826949f5ea259`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 02 Jan 2020 15:48:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Jan 2020 15:20:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jan 2020 17:47:08 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:47:10 GMT
ENV NATS_SERVER=2.1.2
# Wed, 15 Jan 2020 17:47:11 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.2/nats-server-v2.1.2-windows-amd64.zip
# Wed, 15 Jan 2020 17:48:21 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jan 2020 17:50:09 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Jan 2020 17:50:10 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:50:12 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:50:14 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:50:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31f9df80631e7b5d379647ee7701ff50e009bd2c03b30a67a0a8e7bba4a26f94`  
		Size: 1.7 GB (1654613376 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:43da502775fb34b738d9f908cb549c2825c04f1451d1039ec99749be127e47ef`  
		Last Modified: Wed, 15 Jan 2020 17:12:02 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6771e606bb5340710c7ec7fa3294903a0a1f901e5c1e79211ee54fc1f074179a`  
		Last Modified: Wed, 15 Jan 2020 17:53:47 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8885516d0bc2df9c7e82fe0aeb847bc83415084fe85a9aed26a03b3b56ae7c`  
		Last Modified: Wed, 15 Jan 2020 17:53:46 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68459b3a704ec7e5908e23d0d52576c68eef20a4b3ede7bf88ec4e3b2321d170`  
		Last Modified: Wed, 15 Jan 2020 17:53:46 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196e19f93e85979cb0240edd67162a54a2e716e7b139c9c7a99882b3dc42fc2a`  
		Last Modified: Wed, 15 Jan 2020 17:53:47 GMT  
		Size: 5.4 MB (5383420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2ec8ad5670f9274bd1b0dbc71a9ac551d4b18d3f6254bf51bbd80049d7d9c2`  
		Last Modified: Wed, 15 Jan 2020 17:53:46 GMT  
		Size: 9.4 MB (9376638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4abd28582063a6691f03037049db18ea066600d7023aa3d2975eb66ea3cafd`  
		Last Modified: Wed, 15 Jan 2020 17:53:43 GMT  
		Size: 1.8 KB (1762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe6eef99ce520e46eef3031fa6ebd7aeba735253cef9dd2b4e7e07255a9efd8`  
		Last Modified: Wed, 15 Jan 2020 17:53:43 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb11317f8d70c8d41b0ec7372f568029527c0809262db66d162a67d82e2ddc4d`  
		Last Modified: Wed, 15 Jan 2020 17:53:42 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3993164e2c009ccf7891a7fb2956b069daf095ac7a081307e8494e594e98fa`  
		Last Modified: Wed, 15 Jan 2020 17:53:43 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:71e945d4d94bfc25dfdb242bad666f2979caef77f1bff75728f1cc72b4804081
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:f507195794f36c37413ca058f5c3442ad24a80facf94cf4779297e4ab0971f99
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7092803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffa6d536d932527718344a90a884bb621e3480d21893e4bf8e4b7e46b05ad957`
-	Default Command: `["nats-server"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 19:19:25 GMT
ENV NATS_SERVER=2.1.2
# Thu, 23 Jan 2020 19:19:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 23 Jan 2020 19:19:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 23 Jan 2020 19:19:29 GMT
EXPOSE 4222 6222 8222
# Thu, 23 Jan 2020 19:19:29 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581b0b35a07f0a300a55e836a3ba0cb3d18061455a6367a15fbd6f127b57351c`  
		Last Modified: Thu, 23 Jan 2020 19:20:29 GMT  
		Size: 4.3 MB (4305310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82a66d5edde56b04466489c0c46457358c6737789e7e4cde197d7b0befe4fa3`  
		Last Modified: Thu, 23 Jan 2020 19:20:28 GMT  
		Size: 531.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:6380d8b1fc432a021689908f6501d49747edf3b3c2bc54134e433c10e77efb1c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6664521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a20dd366129d9b5428c44f6c6853a8297f7b86b3e6b8f20a1600da467f76599`
-	Default Command: `["nats-server"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:27 GMT
ADD file:2aa80d52585a6b34b2cc5811d46965a084e50cfb8cd183f1a88b2b1bc6556e1f in / 
# Thu, 23 Jan 2020 16:53:28 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:44:32 GMT
ENV NATS_SERVER=2.1.2
# Thu, 23 Jan 2020 17:44:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 23 Jan 2020 17:44:39 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 23 Jan 2020 17:44:40 GMT
EXPOSE 4222 6222 8222
# Thu, 23 Jan 2020 17:44:41 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:896868b7b9168cabb308702db96dc9769d10c23e20fc66f5f4abedf4c75d7642`  
		Last Modified: Thu, 23 Jan 2020 16:54:07 GMT  
		Size: 2.6 MB (2571407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f146c76b464f3790626809adda3914591425f7cd06759a183ccd5da25e26bb82`  
		Last Modified: Thu, 23 Jan 2020 17:45:13 GMT  
		Size: 4.1 MB (4092555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162410de1cd5b2c2ce2cd44dc7973ff2511dc755faeca556ea9e69b1aa55fae3`  
		Last Modified: Thu, 23 Jan 2020 17:45:12 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:d60f1b23e6d2ce2e8edac172e464de946fa830452af16b709c8d3c8234a3c045
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6466632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d154ea04a5c19abf9bcf38dacc8b82bee649c6c507024227c5cd298ed1ac75c6`
-	Default Command: `["nats-server"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:31 GMT
ADD file:d05c9f9143d11d12045d4faef882e5985e6b38fabe52237dd8d8c0627a9620ab in / 
# Thu, 23 Jan 2020 16:53:32 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:55:25 GMT
ENV NATS_SERVER=2.1.2
# Thu, 23 Jan 2020 17:55:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 23 Jan 2020 17:55:30 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 23 Jan 2020 17:55:31 GMT
EXPOSE 4222 6222 8222
# Thu, 23 Jan 2020 17:55:32 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:4e972d957a606327b0b6c2e8aa4a6045c263b7496a536298aaebf690e9d85f1d`  
		Last Modified: Thu, 23 Jan 2020 16:53:59 GMT  
		Size: 2.4 MB (2378408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c375dc9edf38cadcfdc6537707cdea65e2b45d840940712d2f88d19cc967edc6`  
		Last Modified: Thu, 23 Jan 2020 17:56:08 GMT  
		Size: 4.1 MB (4087666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bfcd4ad511455617c2f402e3d5ebd12e714c0d9a0d280f7399735754fab756e`  
		Last Modified: Thu, 23 Jan 2020 17:56:08 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.10`

```console
$ docker pull nats@sha256:71e945d4d94bfc25dfdb242bad666f2979caef77f1bff75728f1cc72b4804081
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats:alpine3.10` - linux; amd64

```console
$ docker pull nats@sha256:f507195794f36c37413ca058f5c3442ad24a80facf94cf4779297e4ab0971f99
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7092803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffa6d536d932527718344a90a884bb621e3480d21893e4bf8e4b7e46b05ad957`
-	Default Command: `["nats-server"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 19:19:25 GMT
ENV NATS_SERVER=2.1.2
# Thu, 23 Jan 2020 19:19:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 23 Jan 2020 19:19:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 23 Jan 2020 19:19:29 GMT
EXPOSE 4222 6222 8222
# Thu, 23 Jan 2020 19:19:29 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581b0b35a07f0a300a55e836a3ba0cb3d18061455a6367a15fbd6f127b57351c`  
		Last Modified: Thu, 23 Jan 2020 19:20:29 GMT  
		Size: 4.3 MB (4305310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82a66d5edde56b04466489c0c46457358c6737789e7e4cde197d7b0befe4fa3`  
		Last Modified: Thu, 23 Jan 2020 19:20:28 GMT  
		Size: 531.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.10` - linux; arm variant v6

```console
$ docker pull nats@sha256:6380d8b1fc432a021689908f6501d49747edf3b3c2bc54134e433c10e77efb1c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6664521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a20dd366129d9b5428c44f6c6853a8297f7b86b3e6b8f20a1600da467f76599`
-	Default Command: `["nats-server"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:27 GMT
ADD file:2aa80d52585a6b34b2cc5811d46965a084e50cfb8cd183f1a88b2b1bc6556e1f in / 
# Thu, 23 Jan 2020 16:53:28 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:44:32 GMT
ENV NATS_SERVER=2.1.2
# Thu, 23 Jan 2020 17:44:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 23 Jan 2020 17:44:39 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 23 Jan 2020 17:44:40 GMT
EXPOSE 4222 6222 8222
# Thu, 23 Jan 2020 17:44:41 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:896868b7b9168cabb308702db96dc9769d10c23e20fc66f5f4abedf4c75d7642`  
		Last Modified: Thu, 23 Jan 2020 16:54:07 GMT  
		Size: 2.6 MB (2571407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f146c76b464f3790626809adda3914591425f7cd06759a183ccd5da25e26bb82`  
		Last Modified: Thu, 23 Jan 2020 17:45:13 GMT  
		Size: 4.1 MB (4092555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162410de1cd5b2c2ce2cd44dc7973ff2511dc755faeca556ea9e69b1aa55fae3`  
		Last Modified: Thu, 23 Jan 2020 17:45:12 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.10` - linux; arm variant v7

```console
$ docker pull nats@sha256:d60f1b23e6d2ce2e8edac172e464de946fa830452af16b709c8d3c8234a3c045
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6466632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d154ea04a5c19abf9bcf38dacc8b82bee649c6c507024227c5cd298ed1ac75c6`
-	Default Command: `["nats-server"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:31 GMT
ADD file:d05c9f9143d11d12045d4faef882e5985e6b38fabe52237dd8d8c0627a9620ab in / 
# Thu, 23 Jan 2020 16:53:32 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:55:25 GMT
ENV NATS_SERVER=2.1.2
# Thu, 23 Jan 2020 17:55:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 23 Jan 2020 17:55:30 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 23 Jan 2020 17:55:31 GMT
EXPOSE 4222 6222 8222
# Thu, 23 Jan 2020 17:55:32 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:4e972d957a606327b0b6c2e8aa4a6045c263b7496a536298aaebf690e9d85f1d`  
		Last Modified: Thu, 23 Jan 2020 16:53:59 GMT  
		Size: 2.4 MB (2378408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c375dc9edf38cadcfdc6537707cdea65e2b45d840940712d2f88d19cc967edc6`  
		Last Modified: Thu, 23 Jan 2020 17:56:08 GMT  
		Size: 4.1 MB (4087666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bfcd4ad511455617c2f402e3d5ebd12e714c0d9a0d280f7399735754fab756e`  
		Last Modified: Thu, 23 Jan 2020 17:56:08 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:53bb39638aa9d14460f6532db6863cd9ded675219b3b9dce3b63ce61276a6d05
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.973; amd64
	-	windows version 10.0.17134.1246; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:8139c5bf4df6e8635cb3420d2dfab08ecdf75b8d16cd82c40a67bd4417b2e71c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (4002673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49014ccb53efc06dc1ce6656aea0abf000881d9db3ac5b31c6f8aef934452b30`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Nov 2019 01:14:07 GMT
COPY file:f7ba6139c8151888be538812698c1aab4311e97fcfac3b5af13138cd7d7e1405 in /nats-server 
# Wed, 20 Nov 2019 01:14:07 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 20 Nov 2019 01:14:08 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Nov 2019 01:14:08 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Nov 2019 01:14:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f3c8f35bd9bcd03ff8eba7551a59aa4fb56c5eabac4758b0b6cb12709785f25c`  
		Last Modified: Wed, 20 Nov 2019 01:14:44 GMT  
		Size: 4.0 MB (4002195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba25f2430b4efc5a2c8e36c142c7aca0b9a14a6caf16fe09d29f97f77f4efce`  
		Last Modified: Wed, 20 Nov 2019 01:14:43 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:234935205b93b7c99b67d82fe35226290aa302e2b35b32f7f9516aa770bf6003
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3790304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66f838f1a59cd8673948823057d50b486bb443ce5318e5a24502ded16334feda`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Nov 2019 00:04:38 GMT
COPY file:1c509c11a9e5697ac3184dd6c0dca46386d2a5d22fabbd0f4898bad8342884d8 in /nats-server 
# Wed, 20 Nov 2019 00:04:39 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 20 Nov 2019 00:04:39 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Nov 2019 00:04:40 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Nov 2019 00:04:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ab4822bfc4bb3725c051563099752bf9f3cc14db9a698a66f64c906201e88b2d`  
		Last Modified: Wed, 20 Nov 2019 00:05:19 GMT  
		Size: 3.8 MB (3789828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd9cf11d4796d35bb8140733b85f1398c199c592ad417cb6d22eac97b0ac377`  
		Last Modified: Wed, 20 Nov 2019 00:05:18 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:92ea09078a55fc56a807ede1630a862d4b6acc12633391a5a42b41483c6b66fa
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3786713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df9b97d154301cbefd42558306e1ece9667269fb9bda4c0ff2c2f601b578c2c8`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Nov 2019 00:53:13 GMT
COPY file:f7bd56432332a04229b22e2b4ed52b31e5ba863bb47a2aacf6d808bd4a8397d1 in /nats-server 
# Wed, 20 Nov 2019 00:53:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 20 Nov 2019 00:53:15 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Nov 2019 00:53:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Nov 2019 00:53:19 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:27216bfb43f9e231372de919d3bbc108e604422a1019a0b0407001997c0575fe`  
		Last Modified: Wed, 20 Nov 2019 00:54:09 GMT  
		Size: 3.8 MB (3786237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3750c7c4312b8b2af995298314a15791a97ce1ef156b81c0477e579fb42b7f2e`  
		Last Modified: Wed, 20 Nov 2019 00:54:09 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:284c4850adc39c33100ab1324dbe23ddde7450c6e5bd15da874d459e68e0ea3e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3665772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeda44c76561e9490c8a19cffd362e26a5552c3aafd41c98b9562a6ae8a01874`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 20 Sep 2019 23:29:17 GMT
COPY file:f0dce6fb207b92a78774313458c6030a8ac0653785d2a2d54e8b5c8935d9b6b8 in /nats-server 
# Fri, 18 Oct 2019 18:04:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 18 Oct 2019 18:04:47 GMT
EXPOSE 4222 6222 8222
# Fri, 18 Oct 2019 18:04:48 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 18 Oct 2019 18:04:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:98fcb931241702ef0a04aa16bb1e4bab6b8afd06f792790462dff69dee05835c`  
		Last Modified: Fri, 20 Sep 2019 23:29:32 GMT  
		Size: 3.7 MB (3665294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e761cba9328047725686c1ed6eecd9eeef33879d348aea70fb3d219b546165`  
		Last Modified: Fri, 18 Oct 2019 18:05:08 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.973; amd64

```console
$ docker pull nats@sha256:fe1ec52862c24ed520cc33ba713ca2a1ab61132fe67f8e4271dd3d54739175bf
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105047963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d2592fd645781c520143281ac28e8f8eba6f4184b893dd1f41c47f4cfea6e22`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 04 Jan 2020 07:17:17 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jan 2020 17:50:29 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:50:31 GMT
RUN cmd /S /C #(nop) COPY file:a9e3f6c9790c912d513d2134dc1f68e02a9edf34862dd584010eae5ab8418108 in C:\nats-server.exe 
# Wed, 15 Jan 2020 17:50:33 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:50:34 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:50:36 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:50:37 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ee446884f7bef76f8275c2f16add1c4fb598bea2ba861e72bce8fb4aac9b55ef`  
		Size: 101.1 MB (101054324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95d31e7189792498b758db35ae56b1ca97128d8063404cbe62a32205d08d1d4a`  
		Last Modified: Wed, 15 Jan 2020 17:54:30 GMT  
		Size: 940.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06dd0cb87c9a67456f9c940ed213536b3e08acb7279b65835e3c65a7654d86f3`  
		Last Modified: Wed, 15 Jan 2020 17:54:30 GMT  
		Size: 4.0 MB (3988335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a3fd5110f7e9b5b9bdf1dcaa1d44324372e6327142443cd9886d09870d8897e`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 1.6 KB (1560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc491f53dd9a291eef7348c3086782cb45ddb7d249aa3fcd080d0dcc05dc8000`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 939.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8053efdd66e716af07b38c62c28b0878f99af0173a9360e403074367593dcc1`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 942.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3215e4233ac1a2ec100e0e6d20af8633eebf5fce1e5813077fdbab6deb27fbb`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17134.1246; amd64

```console
$ docker pull nats@sha256:5f107d9f832b82ff068741b598503279a5c98f7239c376ba43f9e9e63eb46e9a
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.9 MB (157902423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b01104ee474980123a7757c086644468acfb2f4883fb483597c3db674d4181a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 11 Apr 2018 22:12:30 GMT
RUN Apply image 1803-RTM-amd64
# Wed, 08 Jan 2020 15:12:42 GMT
RUN Install update 1803-amd64
# Wed, 15 Jan 2020 17:46:46 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:46:49 GMT
RUN cmd /S /C #(nop) COPY file:a9e3f6c9790c912d513d2134dc1f68e02a9edf34862dd584010eae5ab8418108 in C:\nats-server.exe 
# Wed, 15 Jan 2020 17:46:50 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:46:52 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:46:53 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:46:54 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e46172273a4e4384e1eec7fb01091c828a256ea0f87b30f61381fba9bc511371`  
		Last Modified: Mon, 17 Sep 2018 20:23:30 GMT  
		Size: 92.8 MB (92818888 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c0783c3b88b74a9de609bda64fc01cd5e23fb65d57e750a9c584e8a9ed842fa9`  
		Size: 61.1 MB (61089912 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:24f456fbaddb9e6d59a1ebc9e9244a4b7b003b467f4379a121463c469fe5ac34`  
		Last Modified: Wed, 15 Jan 2020 17:53:01 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2280cf6b56b3522c9f82db3208ab840d8e3292ec7d042eb1d7d4c00319b640`  
		Last Modified: Wed, 15 Jan 2020 17:53:01 GMT  
		Size: 4.0 MB (3988299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c0024dc7e88bada373f0f9593d8ca873d955ddef73363bd42f421f37a339598`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 1.6 KB (1555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d6c860f0094966bd95e3a9b933773c4aa19466f9b337f383aa138b5b41ab22`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15569096640ccf86ed6b731f1e8ecac13947a7bfe4fdaa0b9800f7484bb266c4`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 951.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c849d8e8a6767e0308da9ac7027ca2eecb68424c8d4d748989768b7f920283`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:59141670457fa112c6b1cf5cca3b159ad15bfb7e70fe0b1acbbb5616d922a3c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:8139c5bf4df6e8635cb3420d2dfab08ecdf75b8d16cd82c40a67bd4417b2e71c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (4002673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49014ccb53efc06dc1ce6656aea0abf000881d9db3ac5b31c6f8aef934452b30`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Nov 2019 01:14:07 GMT
COPY file:f7ba6139c8151888be538812698c1aab4311e97fcfac3b5af13138cd7d7e1405 in /nats-server 
# Wed, 20 Nov 2019 01:14:07 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 20 Nov 2019 01:14:08 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Nov 2019 01:14:08 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Nov 2019 01:14:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f3c8f35bd9bcd03ff8eba7551a59aa4fb56c5eabac4758b0b6cb12709785f25c`  
		Last Modified: Wed, 20 Nov 2019 01:14:44 GMT  
		Size: 4.0 MB (4002195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba25f2430b4efc5a2c8e36c142c7aca0b9a14a6caf16fe09d29f97f77f4efce`  
		Last Modified: Wed, 20 Nov 2019 01:14:43 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:234935205b93b7c99b67d82fe35226290aa302e2b35b32f7f9516aa770bf6003
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3790304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66f838f1a59cd8673948823057d50b486bb443ce5318e5a24502ded16334feda`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Nov 2019 00:04:38 GMT
COPY file:1c509c11a9e5697ac3184dd6c0dca46386d2a5d22fabbd0f4898bad8342884d8 in /nats-server 
# Wed, 20 Nov 2019 00:04:39 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 20 Nov 2019 00:04:39 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Nov 2019 00:04:40 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Nov 2019 00:04:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ab4822bfc4bb3725c051563099752bf9f3cc14db9a698a66f64c906201e88b2d`  
		Last Modified: Wed, 20 Nov 2019 00:05:19 GMT  
		Size: 3.8 MB (3789828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd9cf11d4796d35bb8140733b85f1398c199c592ad417cb6d22eac97b0ac377`  
		Last Modified: Wed, 20 Nov 2019 00:05:18 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:92ea09078a55fc56a807ede1630a862d4b6acc12633391a5a42b41483c6b66fa
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3786713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df9b97d154301cbefd42558306e1ece9667269fb9bda4c0ff2c2f601b578c2c8`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Nov 2019 00:53:13 GMT
COPY file:f7bd56432332a04229b22e2b4ed52b31e5ba863bb47a2aacf6d808bd4a8397d1 in /nats-server 
# Wed, 20 Nov 2019 00:53:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 20 Nov 2019 00:53:15 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Nov 2019 00:53:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Nov 2019 00:53:19 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:27216bfb43f9e231372de919d3bbc108e604422a1019a0b0407001997c0575fe`  
		Last Modified: Wed, 20 Nov 2019 00:54:09 GMT  
		Size: 3.8 MB (3786237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3750c7c4312b8b2af995298314a15791a97ce1ef156b81c0477e579fb42b7f2e`  
		Last Modified: Wed, 20 Nov 2019 00:54:09 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:284c4850adc39c33100ab1324dbe23ddde7450c6e5bd15da874d459e68e0ea3e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3665772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeda44c76561e9490c8a19cffd362e26a5552c3aafd41c98b9562a6ae8a01874`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 20 Sep 2019 23:29:17 GMT
COPY file:f0dce6fb207b92a78774313458c6030a8ac0653785d2a2d54e8b5c8935d9b6b8 in /nats-server 
# Fri, 18 Oct 2019 18:04:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 18 Oct 2019 18:04:47 GMT
EXPOSE 4222 6222 8222
# Fri, 18 Oct 2019 18:04:48 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 18 Oct 2019 18:04:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:98fcb931241702ef0a04aa16bb1e4bab6b8afd06f792790462dff69dee05835c`  
		Last Modified: Fri, 20 Sep 2019 23:29:32 GMT  
		Size: 3.7 MB (3665294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e761cba9328047725686c1ed6eecd9eeef33879d348aea70fb3d219b546165`  
		Last Modified: Fri, 18 Oct 2019 18:05:08 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:d028e8a1c50120304d4111bb1214475e11f3684b7176df24a5ec7b00f650decb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64
	-	windows version 10.0.17134.1246; amd64

### `nats:nanoserver` - windows version 10.0.17763.973; amd64

```console
$ docker pull nats@sha256:fe1ec52862c24ed520cc33ba713ca2a1ab61132fe67f8e4271dd3d54739175bf
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105047963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d2592fd645781c520143281ac28e8f8eba6f4184b893dd1f41c47f4cfea6e22`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 04 Jan 2020 07:17:17 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jan 2020 17:50:29 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:50:31 GMT
RUN cmd /S /C #(nop) COPY file:a9e3f6c9790c912d513d2134dc1f68e02a9edf34862dd584010eae5ab8418108 in C:\nats-server.exe 
# Wed, 15 Jan 2020 17:50:33 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:50:34 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:50:36 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:50:37 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ee446884f7bef76f8275c2f16add1c4fb598bea2ba861e72bce8fb4aac9b55ef`  
		Size: 101.1 MB (101054324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95d31e7189792498b758db35ae56b1ca97128d8063404cbe62a32205d08d1d4a`  
		Last Modified: Wed, 15 Jan 2020 17:54:30 GMT  
		Size: 940.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06dd0cb87c9a67456f9c940ed213536b3e08acb7279b65835e3c65a7654d86f3`  
		Last Modified: Wed, 15 Jan 2020 17:54:30 GMT  
		Size: 4.0 MB (3988335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a3fd5110f7e9b5b9bdf1dcaa1d44324372e6327142443cd9886d09870d8897e`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 1.6 KB (1560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc491f53dd9a291eef7348c3086782cb45ddb7d249aa3fcd080d0dcc05dc8000`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 939.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8053efdd66e716af07b38c62c28b0878f99af0173a9360e403074367593dcc1`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 942.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3215e4233ac1a2ec100e0e6d20af8633eebf5fce1e5813077fdbab6deb27fbb`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:nanoserver` - windows version 10.0.17134.1246; amd64

```console
$ docker pull nats@sha256:5f107d9f832b82ff068741b598503279a5c98f7239c376ba43f9e9e63eb46e9a
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.9 MB (157902423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b01104ee474980123a7757c086644468acfb2f4883fb483597c3db674d4181a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 11 Apr 2018 22:12:30 GMT
RUN Apply image 1803-RTM-amd64
# Wed, 08 Jan 2020 15:12:42 GMT
RUN Install update 1803-amd64
# Wed, 15 Jan 2020 17:46:46 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:46:49 GMT
RUN cmd /S /C #(nop) COPY file:a9e3f6c9790c912d513d2134dc1f68e02a9edf34862dd584010eae5ab8418108 in C:\nats-server.exe 
# Wed, 15 Jan 2020 17:46:50 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:46:52 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:46:53 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:46:54 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e46172273a4e4384e1eec7fb01091c828a256ea0f87b30f61381fba9bc511371`  
		Last Modified: Mon, 17 Sep 2018 20:23:30 GMT  
		Size: 92.8 MB (92818888 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c0783c3b88b74a9de609bda64fc01cd5e23fb65d57e750a9c584e8a9ed842fa9`  
		Size: 61.1 MB (61089912 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:24f456fbaddb9e6d59a1ebc9e9244a4b7b003b467f4379a121463c469fe5ac34`  
		Last Modified: Wed, 15 Jan 2020 17:53:01 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2280cf6b56b3522c9f82db3208ab840d8e3292ec7d042eb1d7d4c00319b640`  
		Last Modified: Wed, 15 Jan 2020 17:53:01 GMT  
		Size: 4.0 MB (3988299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c0024dc7e88bada373f0f9593d8ca873d955ddef73363bd42f421f37a339598`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 1.6 KB (1555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d6c860f0094966bd95e3a9b933773c4aa19466f9b337f383aa138b5b41ab22`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15569096640ccf86ed6b731f1e8ecac13947a7bfe4fdaa0b9800f7484bb266c4`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 951.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c849d8e8a6767e0308da9ac7027ca2eecb68424c8d4d748989768b7f920283`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1803`

```console
$ docker pull nats@sha256:9c4a8412f1acfb6279840bdb68e678c0e848b259196fecef0d4ea62c120654c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17134.1246; amd64

### `nats:nanoserver-1803` - windows version 10.0.17134.1246; amd64

```console
$ docker pull nats@sha256:5f107d9f832b82ff068741b598503279a5c98f7239c376ba43f9e9e63eb46e9a
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.9 MB (157902423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b01104ee474980123a7757c086644468acfb2f4883fb483597c3db674d4181a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 11 Apr 2018 22:12:30 GMT
RUN Apply image 1803-RTM-amd64
# Wed, 08 Jan 2020 15:12:42 GMT
RUN Install update 1803-amd64
# Wed, 15 Jan 2020 17:46:46 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:46:49 GMT
RUN cmd /S /C #(nop) COPY file:a9e3f6c9790c912d513d2134dc1f68e02a9edf34862dd584010eae5ab8418108 in C:\nats-server.exe 
# Wed, 15 Jan 2020 17:46:50 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:46:52 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:46:53 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:46:54 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e46172273a4e4384e1eec7fb01091c828a256ea0f87b30f61381fba9bc511371`  
		Last Modified: Mon, 17 Sep 2018 20:23:30 GMT  
		Size: 92.8 MB (92818888 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c0783c3b88b74a9de609bda64fc01cd5e23fb65d57e750a9c584e8a9ed842fa9`  
		Size: 61.1 MB (61089912 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:24f456fbaddb9e6d59a1ebc9e9244a4b7b003b467f4379a121463c469fe5ac34`  
		Last Modified: Wed, 15 Jan 2020 17:53:01 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2280cf6b56b3522c9f82db3208ab840d8e3292ec7d042eb1d7d4c00319b640`  
		Last Modified: Wed, 15 Jan 2020 17:53:01 GMT  
		Size: 4.0 MB (3988299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c0024dc7e88bada373f0f9593d8ca873d955ddef73363bd42f421f37a339598`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 1.6 KB (1555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d6c860f0094966bd95e3a9b933773c4aa19466f9b337f383aa138b5b41ab22`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15569096640ccf86ed6b731f1e8ecac13947a7bfe4fdaa0b9800f7484bb266c4`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 951.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c849d8e8a6767e0308da9ac7027ca2eecb68424c8d4d748989768b7f920283`  
		Last Modified: Wed, 15 Jan 2020 17:52:59 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:35356d98d96477f83eab4060656843a014506567dc5ad5c2acea557bd05c69b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.973; amd64

```console
$ docker pull nats@sha256:fe1ec52862c24ed520cc33ba713ca2a1ab61132fe67f8e4271dd3d54739175bf
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105047963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d2592fd645781c520143281ac28e8f8eba6f4184b893dd1f41c47f4cfea6e22`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 04 Jan 2020 07:17:17 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jan 2020 17:50:29 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:50:31 GMT
RUN cmd /S /C #(nop) COPY file:a9e3f6c9790c912d513d2134dc1f68e02a9edf34862dd584010eae5ab8418108 in C:\nats-server.exe 
# Wed, 15 Jan 2020 17:50:33 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:50:34 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:50:36 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:50:37 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ee446884f7bef76f8275c2f16add1c4fb598bea2ba861e72bce8fb4aac9b55ef`  
		Size: 101.1 MB (101054324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95d31e7189792498b758db35ae56b1ca97128d8063404cbe62a32205d08d1d4a`  
		Last Modified: Wed, 15 Jan 2020 17:54:30 GMT  
		Size: 940.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06dd0cb87c9a67456f9c940ed213536b3e08acb7279b65835e3c65a7654d86f3`  
		Last Modified: Wed, 15 Jan 2020 17:54:30 GMT  
		Size: 4.0 MB (3988335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a3fd5110f7e9b5b9bdf1dcaa1d44324372e6327142443cd9886d09870d8897e`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 1.6 KB (1560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc491f53dd9a291eef7348c3086782cb45ddb7d249aa3fcd080d0dcc05dc8000`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 939.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8053efdd66e716af07b38c62c28b0878f99af0173a9360e403074367593dcc1`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 942.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3215e4233ac1a2ec100e0e6d20af8633eebf5fce1e5813077fdbab6deb27fbb`  
		Last Modified: Wed, 15 Jan 2020 17:54:28 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:59141670457fa112c6b1cf5cca3b159ad15bfb7e70fe0b1acbbb5616d922a3c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:8139c5bf4df6e8635cb3420d2dfab08ecdf75b8d16cd82c40a67bd4417b2e71c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (4002673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49014ccb53efc06dc1ce6656aea0abf000881d9db3ac5b31c6f8aef934452b30`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Nov 2019 01:14:07 GMT
COPY file:f7ba6139c8151888be538812698c1aab4311e97fcfac3b5af13138cd7d7e1405 in /nats-server 
# Wed, 20 Nov 2019 01:14:07 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 20 Nov 2019 01:14:08 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Nov 2019 01:14:08 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Nov 2019 01:14:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f3c8f35bd9bcd03ff8eba7551a59aa4fb56c5eabac4758b0b6cb12709785f25c`  
		Last Modified: Wed, 20 Nov 2019 01:14:44 GMT  
		Size: 4.0 MB (4002195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba25f2430b4efc5a2c8e36c142c7aca0b9a14a6caf16fe09d29f97f77f4efce`  
		Last Modified: Wed, 20 Nov 2019 01:14:43 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:234935205b93b7c99b67d82fe35226290aa302e2b35b32f7f9516aa770bf6003
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3790304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66f838f1a59cd8673948823057d50b486bb443ce5318e5a24502ded16334feda`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Nov 2019 00:04:38 GMT
COPY file:1c509c11a9e5697ac3184dd6c0dca46386d2a5d22fabbd0f4898bad8342884d8 in /nats-server 
# Wed, 20 Nov 2019 00:04:39 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 20 Nov 2019 00:04:39 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Nov 2019 00:04:40 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Nov 2019 00:04:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ab4822bfc4bb3725c051563099752bf9f3cc14db9a698a66f64c906201e88b2d`  
		Last Modified: Wed, 20 Nov 2019 00:05:19 GMT  
		Size: 3.8 MB (3789828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd9cf11d4796d35bb8140733b85f1398c199c592ad417cb6d22eac97b0ac377`  
		Last Modified: Wed, 20 Nov 2019 00:05:18 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:92ea09078a55fc56a807ede1630a862d4b6acc12633391a5a42b41483c6b66fa
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3786713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df9b97d154301cbefd42558306e1ece9667269fb9bda4c0ff2c2f601b578c2c8`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Nov 2019 00:53:13 GMT
COPY file:f7bd56432332a04229b22e2b4ed52b31e5ba863bb47a2aacf6d808bd4a8397d1 in /nats-server 
# Wed, 20 Nov 2019 00:53:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 20 Nov 2019 00:53:15 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Nov 2019 00:53:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Nov 2019 00:53:19 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:27216bfb43f9e231372de919d3bbc108e604422a1019a0b0407001997c0575fe`  
		Last Modified: Wed, 20 Nov 2019 00:54:09 GMT  
		Size: 3.8 MB (3786237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3750c7c4312b8b2af995298314a15791a97ce1ef156b81c0477e579fb42b7f2e`  
		Last Modified: Wed, 20 Nov 2019 00:54:09 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:284c4850adc39c33100ab1324dbe23ddde7450c6e5bd15da874d459e68e0ea3e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3665772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeda44c76561e9490c8a19cffd362e26a5552c3aafd41c98b9562a6ae8a01874`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 20 Sep 2019 23:29:17 GMT
COPY file:f0dce6fb207b92a78774313458c6030a8ac0653785d2a2d54e8b5c8935d9b6b8 in /nats-server 
# Fri, 18 Oct 2019 18:04:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 18 Oct 2019 18:04:47 GMT
EXPOSE 4222 6222 8222
# Fri, 18 Oct 2019 18:04:48 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 18 Oct 2019 18:04:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:98fcb931241702ef0a04aa16bb1e4bab6b8afd06f792790462dff69dee05835c`  
		Last Modified: Fri, 20 Sep 2019 23:29:32 GMT  
		Size: 3.7 MB (3665294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e761cba9328047725686c1ed6eecd9eeef33879d348aea70fb3d219b546165`  
		Last Modified: Fri, 18 Oct 2019 18:05:08 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:a42f0c67634d642f56a78fcc79c12b8d5d4da81b34b93f1ccb103ba2743f6e23
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64
	-	windows version 10.0.17134.1246; amd64
	-	windows version 10.0.14393.3443; amd64

### `nats:windowsservercore` - windows version 10.0.17763.973; amd64

```console
$ docker pull nats@sha256:f5ac96a023326f836cf1c02a5f5b30abd128056d648cac3a4643c8125532ec4f
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2230470888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66ed94808574b78075af126587ee0e95fd33c3b8964fbec51c76c08c20bba3d6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Wed, 15 Jan 2020 14:40:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jan 2020 17:41:54 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:41:55 GMT
ENV NATS_SERVER=2.1.2
# Wed, 15 Jan 2020 17:41:56 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.2/nats-server-v2.1.2-windows-amd64.zip
# Wed, 15 Jan 2020 17:42:38 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jan 2020 17:43:46 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Jan 2020 17:43:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:43:49 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:43:50 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:43:52 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2397868e5c7aa285f662aaa9309fa4756277739e11d589a663a204df80595f2c`  
		Last Modified: Wed, 15 Jan 2020 17:10:53 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b23c268ec0520ea9af1e83b69008728041b2a5f234937b9a6272d2a739fd92e`  
		Last Modified: Wed, 15 Jan 2020 17:51:25 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8bf81f9ddd524bd8d7611b92b362a8f558a338e038fb1a81f81872f58a76f7`  
		Last Modified: Wed, 15 Jan 2020 17:51:25 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb3c94fff5bd229bc976399c1904de65b246152cd41d0147af159fd09877822a`  
		Last Modified: Wed, 15 Jan 2020 17:51:24 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e70dcd5f51d264f2ff2ba291ee37e474f5637d236d01c2d5cd8a4ab039dc60`  
		Last Modified: Wed, 15 Jan 2020 17:51:26 GMT  
		Size: 4.5 MB (4548759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b87189fe10fd6d476acc4c0869463fe1f0d813aa1fc2ff3d95efa65f86d7f34`  
		Last Modified: Wed, 15 Jan 2020 17:51:31 GMT  
		Size: 8.5 MB (8500806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a611e13685ceef48268051590fc9cc976fdec2ec0968e3a12fb9b7ef72b6f2`  
		Last Modified: Wed, 15 Jan 2020 17:51:22 GMT  
		Size: 1.8 KB (1763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ebd020bd73cd69b61c2325da491f4c057f7fdeac1f37db60365aef9d9f56e6`  
		Last Modified: Wed, 15 Jan 2020 17:51:22 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2ef97f255816c764614a7a10afa9fa89f6b8fa9c107f24458eab08ad8aee6d`  
		Last Modified: Wed, 15 Jan 2020 17:51:22 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d555934698e4f3eaa1e7fef777b3692d4a519ec978ec5f191be9ea1a772ad6`  
		Last Modified: Wed, 15 Jan 2020 17:51:22 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:windowsservercore` - windows version 10.0.17134.1246; amd64

```console
$ docker pull nats@sha256:68c9dff50987d82ca20958b1a5ca7cb816509b6d6b024ecc0a5f83cfe26f5f59
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2368141200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20f6b32275bca4375a3ca4b65ab024126e7ae1c30725dcd7ab47d638bc9c5dbc`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 12 Apr 2018 09:20:54 GMT
RUN Apply image 1803-RTM-amd64
# Wed, 08 Jan 2020 15:30:02 GMT
RUN Install update 1803-amd64
# Wed, 15 Jan 2020 17:44:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jan 2020 17:44:14 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:44:15 GMT
ENV NATS_SERVER=2.1.2
# Wed, 15 Jan 2020 17:44:16 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.2/nats-server-v2.1.2-windows-amd64.zip
# Wed, 15 Jan 2020 17:45:13 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jan 2020 17:46:20 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Jan 2020 17:46:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:46:22 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:46:24 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:46:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d9e8b01179bfc94a5bdb1810fbd76b999aa52016001ace2d3a4c4bc7065a9601`  
		Last Modified: Tue, 18 Sep 2018 22:43:55 GMT  
		Size: 1.7 GB (1659688273 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:270ec3ad3fc7d52c0dd086b32f7751131c799e25cdcd4686cc33cbf2b607c34e`  
		Size: 699.2 MB (699246147 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dbec356e813f8f1863318efd5cd62c261f7de4ac49fc093c648020e26d0520fb`  
		Last Modified: Wed, 15 Jan 2020 17:52:17 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c748a716adbca27bf760bc535221171b42c3dcfd044a49e011295928c66c39`  
		Last Modified: Wed, 15 Jan 2020 17:52:17 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7efb3710bacce94103ccc92d28b0a0af30a9bb7a29f1d7f45fc18a75e959ee2d`  
		Last Modified: Wed, 15 Jan 2020 17:52:16 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883bd0fc138e4a17c679bf7d23bb5f0186ccae58fbacdfda29c147e85e2d9383`  
		Last Modified: Wed, 15 Jan 2020 17:52:15 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967451731bebacb830dc7e26892242d8d5c55f6576f5476820313ac2f35d2550`  
		Last Modified: Wed, 15 Jan 2020 17:52:17 GMT  
		Size: 4.9 MB (4880651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35062fb2b37da05d5d753b6519295e3b14da0bf8fecf57ba90fb507aaf498b7`  
		Last Modified: Wed, 15 Jan 2020 17:52:15 GMT  
		Size: 4.3 MB (4316097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bcb4b1ca97cf159a8a5030f29505c9c52626907a92244c92d25df16333f84bf`  
		Last Modified: Wed, 15 Jan 2020 17:52:13 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a380672454ff5ba95dd36413220fa3f00b7998578a8f32ee0b85cfd6d6f9666`  
		Last Modified: Wed, 15 Jan 2020 17:52:13 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f545bb1274ec20783b4966e6592ba3ca21b327f02552a0480c57eae7bd6a77`  
		Last Modified: Wed, 15 Jan 2020 17:52:13 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29eea8dff9fd0ad0a6c1d9943b993b4519c8d7c48140eeb20de7f46fe018e764`  
		Last Modified: Wed, 15 Jan 2020 17:52:13 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:windowsservercore` - windows version 10.0.14393.3443; amd64

```console
$ docker pull nats@sha256:f3b8aa519f1e9981b369d238e46b3e336b2df7654f7cf784b5601d5342a49137
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 GB (5739369423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56ca53177d88b1126a979fb5530e66d83974e1838cecce90ade826949f5ea259`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 02 Jan 2020 15:48:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Jan 2020 15:20:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jan 2020 17:47:08 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:47:10 GMT
ENV NATS_SERVER=2.1.2
# Wed, 15 Jan 2020 17:47:11 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.2/nats-server-v2.1.2-windows-amd64.zip
# Wed, 15 Jan 2020 17:48:21 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jan 2020 17:50:09 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Jan 2020 17:50:10 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:50:12 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:50:14 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:50:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31f9df80631e7b5d379647ee7701ff50e009bd2c03b30a67a0a8e7bba4a26f94`  
		Size: 1.7 GB (1654613376 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:43da502775fb34b738d9f908cb549c2825c04f1451d1039ec99749be127e47ef`  
		Last Modified: Wed, 15 Jan 2020 17:12:02 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6771e606bb5340710c7ec7fa3294903a0a1f901e5c1e79211ee54fc1f074179a`  
		Last Modified: Wed, 15 Jan 2020 17:53:47 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8885516d0bc2df9c7e82fe0aeb847bc83415084fe85a9aed26a03b3b56ae7c`  
		Last Modified: Wed, 15 Jan 2020 17:53:46 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68459b3a704ec7e5908e23d0d52576c68eef20a4b3ede7bf88ec4e3b2321d170`  
		Last Modified: Wed, 15 Jan 2020 17:53:46 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196e19f93e85979cb0240edd67162a54a2e716e7b139c9c7a99882b3dc42fc2a`  
		Last Modified: Wed, 15 Jan 2020 17:53:47 GMT  
		Size: 5.4 MB (5383420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2ec8ad5670f9274bd1b0dbc71a9ac551d4b18d3f6254bf51bbd80049d7d9c2`  
		Last Modified: Wed, 15 Jan 2020 17:53:46 GMT  
		Size: 9.4 MB (9376638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4abd28582063a6691f03037049db18ea066600d7023aa3d2975eb66ea3cafd`  
		Last Modified: Wed, 15 Jan 2020 17:53:43 GMT  
		Size: 1.8 KB (1762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe6eef99ce520e46eef3031fa6ebd7aeba735253cef9dd2b4e7e07255a9efd8`  
		Last Modified: Wed, 15 Jan 2020 17:53:43 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb11317f8d70c8d41b0ec7372f568029527c0809262db66d162a67d82e2ddc4d`  
		Last Modified: Wed, 15 Jan 2020 17:53:42 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3993164e2c009ccf7891a7fb2956b069daf095ac7a081307e8494e594e98fa`  
		Last Modified: Wed, 15 Jan 2020 17:53:43 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1803`

```console
$ docker pull nats@sha256:d06f971a89319c413118f67b67dab4e52914ad2540fcd2844f831c2a237c35d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17134.1246; amd64

### `nats:windowsservercore-1803` - windows version 10.0.17134.1246; amd64

```console
$ docker pull nats@sha256:68c9dff50987d82ca20958b1a5ca7cb816509b6d6b024ecc0a5f83cfe26f5f59
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2368141200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20f6b32275bca4375a3ca4b65ab024126e7ae1c30725dcd7ab47d638bc9c5dbc`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 12 Apr 2018 09:20:54 GMT
RUN Apply image 1803-RTM-amd64
# Wed, 08 Jan 2020 15:30:02 GMT
RUN Install update 1803-amd64
# Wed, 15 Jan 2020 17:44:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jan 2020 17:44:14 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:44:15 GMT
ENV NATS_SERVER=2.1.2
# Wed, 15 Jan 2020 17:44:16 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.2/nats-server-v2.1.2-windows-amd64.zip
# Wed, 15 Jan 2020 17:45:13 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jan 2020 17:46:20 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Jan 2020 17:46:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:46:22 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:46:24 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:46:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d9e8b01179bfc94a5bdb1810fbd76b999aa52016001ace2d3a4c4bc7065a9601`  
		Last Modified: Tue, 18 Sep 2018 22:43:55 GMT  
		Size: 1.7 GB (1659688273 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:270ec3ad3fc7d52c0dd086b32f7751131c799e25cdcd4686cc33cbf2b607c34e`  
		Size: 699.2 MB (699246147 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dbec356e813f8f1863318efd5cd62c261f7de4ac49fc093c648020e26d0520fb`  
		Last Modified: Wed, 15 Jan 2020 17:52:17 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c748a716adbca27bf760bc535221171b42c3dcfd044a49e011295928c66c39`  
		Last Modified: Wed, 15 Jan 2020 17:52:17 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7efb3710bacce94103ccc92d28b0a0af30a9bb7a29f1d7f45fc18a75e959ee2d`  
		Last Modified: Wed, 15 Jan 2020 17:52:16 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883bd0fc138e4a17c679bf7d23bb5f0186ccae58fbacdfda29c147e85e2d9383`  
		Last Modified: Wed, 15 Jan 2020 17:52:15 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967451731bebacb830dc7e26892242d8d5c55f6576f5476820313ac2f35d2550`  
		Last Modified: Wed, 15 Jan 2020 17:52:17 GMT  
		Size: 4.9 MB (4880651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35062fb2b37da05d5d753b6519295e3b14da0bf8fecf57ba90fb507aaf498b7`  
		Last Modified: Wed, 15 Jan 2020 17:52:15 GMT  
		Size: 4.3 MB (4316097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bcb4b1ca97cf159a8a5030f29505c9c52626907a92244c92d25df16333f84bf`  
		Last Modified: Wed, 15 Jan 2020 17:52:13 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a380672454ff5ba95dd36413220fa3f00b7998578a8f32ee0b85cfd6d6f9666`  
		Last Modified: Wed, 15 Jan 2020 17:52:13 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f545bb1274ec20783b4966e6592ba3ca21b327f02552a0480c57eae7bd6a77`  
		Last Modified: Wed, 15 Jan 2020 17:52:13 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29eea8dff9fd0ad0a6c1d9943b993b4519c8d7c48140eeb20de7f46fe018e764`  
		Last Modified: Wed, 15 Jan 2020 17:52:13 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:655dcc67ed8905581e9ef5bbc18c06dbd66da9bea9b4dbfc5baf5e575525438e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.973; amd64

```console
$ docker pull nats@sha256:f5ac96a023326f836cf1c02a5f5b30abd128056d648cac3a4643c8125532ec4f
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2230470888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66ed94808574b78075af126587ee0e95fd33c3b8964fbec51c76c08c20bba3d6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Wed, 15 Jan 2020 14:40:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jan 2020 17:41:54 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:41:55 GMT
ENV NATS_SERVER=2.1.2
# Wed, 15 Jan 2020 17:41:56 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.2/nats-server-v2.1.2-windows-amd64.zip
# Wed, 15 Jan 2020 17:42:38 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jan 2020 17:43:46 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Jan 2020 17:43:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:43:49 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:43:50 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:43:52 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2397868e5c7aa285f662aaa9309fa4756277739e11d589a663a204df80595f2c`  
		Last Modified: Wed, 15 Jan 2020 17:10:53 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b23c268ec0520ea9af1e83b69008728041b2a5f234937b9a6272d2a739fd92e`  
		Last Modified: Wed, 15 Jan 2020 17:51:25 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8bf81f9ddd524bd8d7611b92b362a8f558a338e038fb1a81f81872f58a76f7`  
		Last Modified: Wed, 15 Jan 2020 17:51:25 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb3c94fff5bd229bc976399c1904de65b246152cd41d0147af159fd09877822a`  
		Last Modified: Wed, 15 Jan 2020 17:51:24 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e70dcd5f51d264f2ff2ba291ee37e474f5637d236d01c2d5cd8a4ab039dc60`  
		Last Modified: Wed, 15 Jan 2020 17:51:26 GMT  
		Size: 4.5 MB (4548759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b87189fe10fd6d476acc4c0869463fe1f0d813aa1fc2ff3d95efa65f86d7f34`  
		Last Modified: Wed, 15 Jan 2020 17:51:31 GMT  
		Size: 8.5 MB (8500806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a611e13685ceef48268051590fc9cc976fdec2ec0968e3a12fb9b7ef72b6f2`  
		Last Modified: Wed, 15 Jan 2020 17:51:22 GMT  
		Size: 1.8 KB (1763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ebd020bd73cd69b61c2325da491f4c057f7fdeac1f37db60365aef9d9f56e6`  
		Last Modified: Wed, 15 Jan 2020 17:51:22 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2ef97f255816c764614a7a10afa9fa89f6b8fa9c107f24458eab08ad8aee6d`  
		Last Modified: Wed, 15 Jan 2020 17:51:22 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d555934698e4f3eaa1e7fef777b3692d4a519ec978ec5f191be9ea1a772ad6`  
		Last Modified: Wed, 15 Jan 2020 17:51:22 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:b0bab523ef87fed76cbcc206909058cdceace4206e8797b3dc3bb074f8148c9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3443; amd64

### `nats:windowsservercore-ltsc2016` - windows version 10.0.14393.3443; amd64

```console
$ docker pull nats@sha256:f3b8aa519f1e9981b369d238e46b3e336b2df7654f7cf784b5601d5342a49137
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 GB (5739369423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56ca53177d88b1126a979fb5530e66d83974e1838cecce90ade826949f5ea259`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 02 Jan 2020 15:48:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Jan 2020 15:20:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jan 2020 17:47:08 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 17:47:10 GMT
ENV NATS_SERVER=2.1.2
# Wed, 15 Jan 2020 17:47:11 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.2/nats-server-v2.1.2-windows-amd64.zip
# Wed, 15 Jan 2020 17:48:21 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jan 2020 17:50:09 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Jan 2020 17:50:10 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jan 2020 17:50:12 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Jan 2020 17:50:14 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jan 2020 17:50:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31f9df80631e7b5d379647ee7701ff50e009bd2c03b30a67a0a8e7bba4a26f94`  
		Size: 1.7 GB (1654613376 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:43da502775fb34b738d9f908cb549c2825c04f1451d1039ec99749be127e47ef`  
		Last Modified: Wed, 15 Jan 2020 17:12:02 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6771e606bb5340710c7ec7fa3294903a0a1f901e5c1e79211ee54fc1f074179a`  
		Last Modified: Wed, 15 Jan 2020 17:53:47 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8885516d0bc2df9c7e82fe0aeb847bc83415084fe85a9aed26a03b3b56ae7c`  
		Last Modified: Wed, 15 Jan 2020 17:53:46 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68459b3a704ec7e5908e23d0d52576c68eef20a4b3ede7bf88ec4e3b2321d170`  
		Last Modified: Wed, 15 Jan 2020 17:53:46 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196e19f93e85979cb0240edd67162a54a2e716e7b139c9c7a99882b3dc42fc2a`  
		Last Modified: Wed, 15 Jan 2020 17:53:47 GMT  
		Size: 5.4 MB (5383420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2ec8ad5670f9274bd1b0dbc71a9ac551d4b18d3f6254bf51bbd80049d7d9c2`  
		Last Modified: Wed, 15 Jan 2020 17:53:46 GMT  
		Size: 9.4 MB (9376638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4abd28582063a6691f03037049db18ea066600d7023aa3d2975eb66ea3cafd`  
		Last Modified: Wed, 15 Jan 2020 17:53:43 GMT  
		Size: 1.8 KB (1762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe6eef99ce520e46eef3031fa6ebd7aeba735253cef9dd2b4e7e07255a9efd8`  
		Last Modified: Wed, 15 Jan 2020 17:53:43 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb11317f8d70c8d41b0ec7372f568029527c0809262db66d162a67d82e2ddc4d`  
		Last Modified: Wed, 15 Jan 2020 17:53:42 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3993164e2c009ccf7891a7fb2956b069daf095ac7a081307e8494e594e98fa`  
		Last Modified: Wed, 15 Jan 2020 17:53:43 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
