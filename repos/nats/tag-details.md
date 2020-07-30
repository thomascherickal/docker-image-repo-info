<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats`

-	[`nats:2`](#nats2)
-	[`nats:2.1`](#nats21)
-	[`nats:2.1.7`](#nats217)
-	[`nats:2.1.7-alpine`](#nats217-alpine)
-	[`nats:2.1.7-alpine3.11`](#nats217-alpine311)
-	[`nats:2.1.7-linux`](#nats217-linux)
-	[`nats:2.1.7-nanoserver`](#nats217-nanoserver)
-	[`nats:2.1.7-nanoserver-1809`](#nats217-nanoserver-1809)
-	[`nats:2.1.7-scratch`](#nats217-scratch)
-	[`nats:2.1.7-windowsservercore`](#nats217-windowsservercore)
-	[`nats:2.1.7-windowsservercore-1809`](#nats217-windowsservercore-1809)
-	[`nats:2.1.7-windowsservercore-ltsc2016`](#nats217-windowsservercore-ltsc2016)
-	[`nats:2.1-alpine`](#nats21-alpine)
-	[`nats:2.1-alpine3.11`](#nats21-alpine311)
-	[`nats:2.1-linux`](#nats21-linux)
-	[`nats:2.1-nanoserver`](#nats21-nanoserver)
-	[`nats:2.1-nanoserver-1809`](#nats21-nanoserver-1809)
-	[`nats:2.1-scratch`](#nats21-scratch)
-	[`nats:2.1-windowsservercore`](#nats21-windowsservercore)
-	[`nats:2.1-windowsservercore-1809`](#nats21-windowsservercore-1809)
-	[`nats:2.1-windowsservercore-ltsc2016`](#nats21-windowsservercore-ltsc2016)
-	[`nats:2-alpine`](#nats2-alpine)
-	[`nats:2-alpine3.11`](#nats2-alpine311)
-	[`nats:2-linux`](#nats2-linux)
-	[`nats:2-nanoserver`](#nats2-nanoserver)
-	[`nats:2-nanoserver-1809`](#nats2-nanoserver-1809)
-	[`nats:2-scratch`](#nats2-scratch)
-	[`nats:2-windowsservercore`](#nats2-windowsservercore)
-	[`nats:2-windowsservercore-1809`](#nats2-windowsservercore-1809)
-	[`nats:2-windowsservercore-ltsc2016`](#nats2-windowsservercore-ltsc2016)
-	[`nats:alpine`](#natsalpine)
-	[`nats:alpine3.11`](#natsalpine311)
-	[`nats:latest`](#natslatest)
-	[`nats:linux`](#natslinux)
-	[`nats:nanoserver`](#natsnanoserver)
-	[`nats:nanoserver-1809`](#natsnanoserver-1809)
-	[`nats:scratch`](#natsscratch)
-	[`nats:windowsservercore`](#natswindowsservercore)
-	[`nats:windowsservercore-1809`](#natswindowsservercore-1809)
-	[`nats:windowsservercore-ltsc2016`](#natswindowsservercore-ltsc2016)

## `nats:2`

```console
$ docker pull nats@sha256:35d212a94eb9c1d6568d91f450637a8a597ecb703b5d32425df06a31945bbf32
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1339; amd64

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:6aace730d886f9719841c60ec11f826e494b8fcc631378b32f5e01ca32d87ab9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4087969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e93a56bc1852bb18d91f1741edde016c59b49c92f7ad91960d583ee0486ebf3`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 16 May 2020 09:47:58 GMT
COPY file:27ab63fb5115ca3cb7456a256d6d6dab7ba864d8806821652fbe569f4f845df5 in /nats-server 
# Sat, 16 May 2020 09:47:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 16 May 2020 09:47:59 GMT
EXPOSE 4222 6222 8222
# Sat, 16 May 2020 09:47:59 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 16 May 2020 09:47:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b509577c042697add820579de13ceed535b1c02ec7fa460b892d6c63941390a7`  
		Last Modified: Sat, 16 May 2020 09:48:21 GMT  
		Size: 4.1 MB (4087491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ce65065eb7bc6684476be5937b3d0d4046e7cc7241bc5017d70488d0edbfe3`  
		Last Modified: Sat, 16 May 2020 09:48:20 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:e8b59aabb2b6838ced59a3125ba4216cc8a4d0622f8b8c1e9e40fb30cd63a135
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3796375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8116ee7998ff454ed4eaa153438504925828993f56f26fb96fd11b31c9dc2128`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 15 May 2020 19:53:42 GMT
COPY file:9951c1b4ae20021f4d6efd6c039d0f0d0044470572e81beae625f15ffa13d2f1 in /nats-server 
# Fri, 15 May 2020 19:53:43 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 15 May 2020 19:53:44 GMT
EXPOSE 4222 6222 8222
# Fri, 15 May 2020 19:53:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 15 May 2020 19:53:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7976dc3d59fddf78c4ca25d0692135431e63b9fb744ae2c3d02b7a8214b5bfd9`  
		Last Modified: Fri, 15 May 2020 19:54:21 GMT  
		Size: 3.8 MB (3795898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b520f7415a5fab1b4a83eb7a8259e321475f75f5b06bfe95493b598c9ee9f4`  
		Last Modified: Fri, 15 May 2020 19:54:20 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:707f02b7c81a3f071abba9ce0a74b1cf0bf7a664e0220ab6cae112f2721a24bf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3792273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d2f2220669ef3621c45d5e4fd8460e7378e258044eb57003584ce55db5bdd9b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 16 May 2020 04:26:09 GMT
COPY file:3320edcd8f0db9551469809c752244493d1c6cf3be0287714c8a507e339283b2 in /nats-server 
# Sat, 16 May 2020 04:26:09 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 16 May 2020 04:26:11 GMT
EXPOSE 4222 6222 8222
# Sat, 16 May 2020 04:26:12 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 16 May 2020 04:26:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7ceefb66163b74f9719728ecace35bd406e85998a252d90c9e07a02582c7b6f1`  
		Last Modified: Sat, 16 May 2020 04:26:55 GMT  
		Size: 3.8 MB (3791795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db182fe235e1ef3b80de633e39d8ab9040cef44127adee97dbc4513df27dacfe`  
		Last Modified: Sat, 16 May 2020 04:26:53 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8cb2b90d45f90f3bdfb841b4a1399ff3a1b0a835e54664ee375ef309ff4c4398
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3776968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fffbb615827376dda1ad45bce22763d7cdc858675e4eafc55deb2d134f813338`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 29 Jul 2020 22:41:42 GMT
COPY file:67a03d7df05756de9c16c4cd22dfaf6ed9cc9a43b78a90ebfaa81ee7ebbc7abf in /nats-server 
# Wed, 29 Jul 2020 22:41:43 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 29 Jul 2020 22:41:44 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 22:41:44 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 29 Jul 2020 22:41:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:39a183ba93759b5fab08b0cb81f1f1a4c9f5a95c3746b031082c6bc3a57441b3`  
		Last Modified: Wed, 29 Jul 2020 22:42:18 GMT  
		Size: 3.8 MB (3776492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a510a0d87b5b915212ee2a5e5d877dced1c30164c0e82d6e60951d00374fe7`  
		Last Modified: Wed, 29 Jul 2020 22:42:17 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats@sha256:00f69dcad2cdf6b3da43ef4701091ca04d3f35b2ec80c666554d49e5684258d8
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (104957159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edebc41e62feb1ccc604f2e015421dd2e938344719a06d92981822566271a91b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Jul 2020 13:50:07 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jul 2020 15:05:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 15:05:16 GMT
RUN cmd /S /C #(nop) COPY file:18561b827240029ad80d0e3d25142efae62905c30cc520fc37cfc68e7d889848 in C:\nats-server.exe 
# Wed, 15 Jul 2020 15:05:18 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jul 2020 15:05:18 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Jul 2020 15:05:19 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jul 2020 15:05:20 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:dc95608099543221ef539391bfece5c1ce37b97af9da457f5990349cab028a12`  
		Size: 100.9 MB (100895619 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5f0c27d781c53928c03429d5b34e0f49fc26b7e7c996c1d9a2a8474162eade60`  
		Last Modified: Wed, 15 Jul 2020 15:09:50 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10a270f5d0666930958ddfeac073712f678d77b5a05a08210012ada454204077`  
		Last Modified: Wed, 15 Jul 2020 15:10:00 GMT  
		Size: 4.1 MB (4056451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b5e48167a563124481e83cd3f3e3ca1bd3ea8f52b9e52dc9b4982e98a21d7d`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 1.5 KB (1470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64aecdf43c40f563833e5ad1c027bb2e67c1b0c51bb2ab795b99df1f4c2f26f`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 930.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:accd609b6f7304740da44e2a7331717a73ec3f94a35c25198a189b81bd84e204`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 928.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84a11ddf5d09a44b078d904b91df1cd82bf2a0cefb6ec9f52761f36fcf23f54`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1`

```console
$ docker pull nats@sha256:35d212a94eb9c1d6568d91f450637a8a597ecb703b5d32425df06a31945bbf32
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1339; amd64

### `nats:2.1` - linux; amd64

```console
$ docker pull nats@sha256:6aace730d886f9719841c60ec11f826e494b8fcc631378b32f5e01ca32d87ab9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4087969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e93a56bc1852bb18d91f1741edde016c59b49c92f7ad91960d583ee0486ebf3`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 16 May 2020 09:47:58 GMT
COPY file:27ab63fb5115ca3cb7456a256d6d6dab7ba864d8806821652fbe569f4f845df5 in /nats-server 
# Sat, 16 May 2020 09:47:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 16 May 2020 09:47:59 GMT
EXPOSE 4222 6222 8222
# Sat, 16 May 2020 09:47:59 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 16 May 2020 09:47:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b509577c042697add820579de13ceed535b1c02ec7fa460b892d6c63941390a7`  
		Last Modified: Sat, 16 May 2020 09:48:21 GMT  
		Size: 4.1 MB (4087491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ce65065eb7bc6684476be5937b3d0d4046e7cc7241bc5017d70488d0edbfe3`  
		Last Modified: Sat, 16 May 2020 09:48:20 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1` - linux; arm variant v6

```console
$ docker pull nats@sha256:e8b59aabb2b6838ced59a3125ba4216cc8a4d0622f8b8c1e9e40fb30cd63a135
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3796375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8116ee7998ff454ed4eaa153438504925828993f56f26fb96fd11b31c9dc2128`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 15 May 2020 19:53:42 GMT
COPY file:9951c1b4ae20021f4d6efd6c039d0f0d0044470572e81beae625f15ffa13d2f1 in /nats-server 
# Fri, 15 May 2020 19:53:43 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 15 May 2020 19:53:44 GMT
EXPOSE 4222 6222 8222
# Fri, 15 May 2020 19:53:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 15 May 2020 19:53:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7976dc3d59fddf78c4ca25d0692135431e63b9fb744ae2c3d02b7a8214b5bfd9`  
		Last Modified: Fri, 15 May 2020 19:54:21 GMT  
		Size: 3.8 MB (3795898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b520f7415a5fab1b4a83eb7a8259e321475f75f5b06bfe95493b598c9ee9f4`  
		Last Modified: Fri, 15 May 2020 19:54:20 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1` - linux; arm variant v7

```console
$ docker pull nats@sha256:707f02b7c81a3f071abba9ce0a74b1cf0bf7a664e0220ab6cae112f2721a24bf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3792273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d2f2220669ef3621c45d5e4fd8460e7378e258044eb57003584ce55db5bdd9b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 16 May 2020 04:26:09 GMT
COPY file:3320edcd8f0db9551469809c752244493d1c6cf3be0287714c8a507e339283b2 in /nats-server 
# Sat, 16 May 2020 04:26:09 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 16 May 2020 04:26:11 GMT
EXPOSE 4222 6222 8222
# Sat, 16 May 2020 04:26:12 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 16 May 2020 04:26:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7ceefb66163b74f9719728ecace35bd406e85998a252d90c9e07a02582c7b6f1`  
		Last Modified: Sat, 16 May 2020 04:26:55 GMT  
		Size: 3.8 MB (3791795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db182fe235e1ef3b80de633e39d8ab9040cef44127adee97dbc4513df27dacfe`  
		Last Modified: Sat, 16 May 2020 04:26:53 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8cb2b90d45f90f3bdfb841b4a1399ff3a1b0a835e54664ee375ef309ff4c4398
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3776968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fffbb615827376dda1ad45bce22763d7cdc858675e4eafc55deb2d134f813338`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 29 Jul 2020 22:41:42 GMT
COPY file:67a03d7df05756de9c16c4cd22dfaf6ed9cc9a43b78a90ebfaa81ee7ebbc7abf in /nats-server 
# Wed, 29 Jul 2020 22:41:43 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 29 Jul 2020 22:41:44 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 22:41:44 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 29 Jul 2020 22:41:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:39a183ba93759b5fab08b0cb81f1f1a4c9f5a95c3746b031082c6bc3a57441b3`  
		Last Modified: Wed, 29 Jul 2020 22:42:18 GMT  
		Size: 3.8 MB (3776492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a510a0d87b5b915212ee2a5e5d877dced1c30164c0e82d6e60951d00374fe7`  
		Last Modified: Wed, 29 Jul 2020 22:42:17 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats@sha256:00f69dcad2cdf6b3da43ef4701091ca04d3f35b2ec80c666554d49e5684258d8
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (104957159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edebc41e62feb1ccc604f2e015421dd2e938344719a06d92981822566271a91b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Jul 2020 13:50:07 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jul 2020 15:05:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 15:05:16 GMT
RUN cmd /S /C #(nop) COPY file:18561b827240029ad80d0e3d25142efae62905c30cc520fc37cfc68e7d889848 in C:\nats-server.exe 
# Wed, 15 Jul 2020 15:05:18 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jul 2020 15:05:18 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Jul 2020 15:05:19 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jul 2020 15:05:20 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:dc95608099543221ef539391bfece5c1ce37b97af9da457f5990349cab028a12`  
		Size: 100.9 MB (100895619 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5f0c27d781c53928c03429d5b34e0f49fc26b7e7c996c1d9a2a8474162eade60`  
		Last Modified: Wed, 15 Jul 2020 15:09:50 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10a270f5d0666930958ddfeac073712f678d77b5a05a08210012ada454204077`  
		Last Modified: Wed, 15 Jul 2020 15:10:00 GMT  
		Size: 4.1 MB (4056451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b5e48167a563124481e83cd3f3e3ca1bd3ea8f52b9e52dc9b4982e98a21d7d`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 1.5 KB (1470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64aecdf43c40f563833e5ad1c027bb2e67c1b0c51bb2ab795b99df1f4c2f26f`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 930.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:accd609b6f7304740da44e2a7331717a73ec3f94a35c25198a189b81bd84e204`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 928.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84a11ddf5d09a44b078d904b91df1cd82bf2a0cefb6ec9f52761f36fcf23f54`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.7`

```console
$ docker pull nats@sha256:35d212a94eb9c1d6568d91f450637a8a597ecb703b5d32425df06a31945bbf32
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1339; amd64

### `nats:2.1.7` - linux; amd64

```console
$ docker pull nats@sha256:6aace730d886f9719841c60ec11f826e494b8fcc631378b32f5e01ca32d87ab9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4087969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e93a56bc1852bb18d91f1741edde016c59b49c92f7ad91960d583ee0486ebf3`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 16 May 2020 09:47:58 GMT
COPY file:27ab63fb5115ca3cb7456a256d6d6dab7ba864d8806821652fbe569f4f845df5 in /nats-server 
# Sat, 16 May 2020 09:47:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 16 May 2020 09:47:59 GMT
EXPOSE 4222 6222 8222
# Sat, 16 May 2020 09:47:59 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 16 May 2020 09:47:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b509577c042697add820579de13ceed535b1c02ec7fa460b892d6c63941390a7`  
		Last Modified: Sat, 16 May 2020 09:48:21 GMT  
		Size: 4.1 MB (4087491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ce65065eb7bc6684476be5937b3d0d4046e7cc7241bc5017d70488d0edbfe3`  
		Last Modified: Sat, 16 May 2020 09:48:20 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.7` - linux; arm variant v6

```console
$ docker pull nats@sha256:e8b59aabb2b6838ced59a3125ba4216cc8a4d0622f8b8c1e9e40fb30cd63a135
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3796375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8116ee7998ff454ed4eaa153438504925828993f56f26fb96fd11b31c9dc2128`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 15 May 2020 19:53:42 GMT
COPY file:9951c1b4ae20021f4d6efd6c039d0f0d0044470572e81beae625f15ffa13d2f1 in /nats-server 
# Fri, 15 May 2020 19:53:43 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 15 May 2020 19:53:44 GMT
EXPOSE 4222 6222 8222
# Fri, 15 May 2020 19:53:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 15 May 2020 19:53:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7976dc3d59fddf78c4ca25d0692135431e63b9fb744ae2c3d02b7a8214b5bfd9`  
		Last Modified: Fri, 15 May 2020 19:54:21 GMT  
		Size: 3.8 MB (3795898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b520f7415a5fab1b4a83eb7a8259e321475f75f5b06bfe95493b598c9ee9f4`  
		Last Modified: Fri, 15 May 2020 19:54:20 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.7` - linux; arm variant v7

```console
$ docker pull nats@sha256:707f02b7c81a3f071abba9ce0a74b1cf0bf7a664e0220ab6cae112f2721a24bf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3792273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d2f2220669ef3621c45d5e4fd8460e7378e258044eb57003584ce55db5bdd9b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 16 May 2020 04:26:09 GMT
COPY file:3320edcd8f0db9551469809c752244493d1c6cf3be0287714c8a507e339283b2 in /nats-server 
# Sat, 16 May 2020 04:26:09 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 16 May 2020 04:26:11 GMT
EXPOSE 4222 6222 8222
# Sat, 16 May 2020 04:26:12 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 16 May 2020 04:26:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7ceefb66163b74f9719728ecace35bd406e85998a252d90c9e07a02582c7b6f1`  
		Last Modified: Sat, 16 May 2020 04:26:55 GMT  
		Size: 3.8 MB (3791795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db182fe235e1ef3b80de633e39d8ab9040cef44127adee97dbc4513df27dacfe`  
		Last Modified: Sat, 16 May 2020 04:26:53 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.7` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8cb2b90d45f90f3bdfb841b4a1399ff3a1b0a835e54664ee375ef309ff4c4398
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3776968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fffbb615827376dda1ad45bce22763d7cdc858675e4eafc55deb2d134f813338`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 29 Jul 2020 22:41:42 GMT
COPY file:67a03d7df05756de9c16c4cd22dfaf6ed9cc9a43b78a90ebfaa81ee7ebbc7abf in /nats-server 
# Wed, 29 Jul 2020 22:41:43 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 29 Jul 2020 22:41:44 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 22:41:44 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 29 Jul 2020 22:41:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:39a183ba93759b5fab08b0cb81f1f1a4c9f5a95c3746b031082c6bc3a57441b3`  
		Last Modified: Wed, 29 Jul 2020 22:42:18 GMT  
		Size: 3.8 MB (3776492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a510a0d87b5b915212ee2a5e5d877dced1c30164c0e82d6e60951d00374fe7`  
		Last Modified: Wed, 29 Jul 2020 22:42:17 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.7` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats@sha256:00f69dcad2cdf6b3da43ef4701091ca04d3f35b2ec80c666554d49e5684258d8
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (104957159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edebc41e62feb1ccc604f2e015421dd2e938344719a06d92981822566271a91b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Jul 2020 13:50:07 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jul 2020 15:05:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 15:05:16 GMT
RUN cmd /S /C #(nop) COPY file:18561b827240029ad80d0e3d25142efae62905c30cc520fc37cfc68e7d889848 in C:\nats-server.exe 
# Wed, 15 Jul 2020 15:05:18 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jul 2020 15:05:18 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Jul 2020 15:05:19 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jul 2020 15:05:20 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:dc95608099543221ef539391bfece5c1ce37b97af9da457f5990349cab028a12`  
		Size: 100.9 MB (100895619 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5f0c27d781c53928c03429d5b34e0f49fc26b7e7c996c1d9a2a8474162eade60`  
		Last Modified: Wed, 15 Jul 2020 15:09:50 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10a270f5d0666930958ddfeac073712f678d77b5a05a08210012ada454204077`  
		Last Modified: Wed, 15 Jul 2020 15:10:00 GMT  
		Size: 4.1 MB (4056451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b5e48167a563124481e83cd3f3e3ca1bd3ea8f52b9e52dc9b4982e98a21d7d`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 1.5 KB (1470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64aecdf43c40f563833e5ad1c027bb2e67c1b0c51bb2ab795b99df1f4c2f26f`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 930.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:accd609b6f7304740da44e2a7331717a73ec3f94a35c25198a189b81bd84e204`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 928.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84a11ddf5d09a44b078d904b91df1cd82bf2a0cefb6ec9f52761f36fcf23f54`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.7-alpine`

```console
$ docker pull nats@sha256:2ca671f95f6f5c4d9144a701d8b7be77a1830041d86766e2e193fb58b00af449
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.1.7-alpine` - linux; amd64

```console
$ docker pull nats@sha256:c1c1159e76d03431b2c612d378a62fc914f0817df3f9a8092adddb589ac74e53
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7203227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54acd9cf4794435761c0462aba37d41e69e9581a77daeef4d16255b6a579f2c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Sat, 16 May 2020 09:47:11 GMT
ENV NATS_SERVER=2.1.7
# Wed, 29 Jul 2020 23:25:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a08d7ce0399df8701d3e3cd4c36744180c3a566cdb38efeccc12a364f0083705' ;; 		armhf) natsArch='arm6'; sha256='987c23f758842fb09c0d4500f632c5302aedc61d218f03998444b94074aabddb' ;; 		armv7) natsArch='arm7'; sha256='077fd1647aa25865ade5acc3d6ee5f542d2c62feb2fb41ec6d1dd83294bea05e' ;; 		x86_64) natsArch='amd64'; sha256='23cce53fe7f628f203dbbeadf434c3480d094690aba6ff0b1d374b8f2f9ffd8c' ;; 		x86) natsArch='386'; sha256='64e271690782af823930c95574db0f701d06a36ff42b9272c04841d4611bcd15' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:25:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 29 Jul 2020 23:25:41 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Jul 2020 23:25:42 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 23:25:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:25:42 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09eebfe9509bcbfcefadbc17c68fa103be7b7cf978f08ea01527a6aba38c5554`  
		Last Modified: Wed, 29 Jul 2020 23:26:16 GMT  
		Size: 4.4 MB (4388967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab62a5d69bc21353fa665e0b7fbf8e6a4a5d3fda0e87d58c02073999f76ff43f`  
		Last Modified: Wed, 29 Jul 2020 23:26:15 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a297d716cd17565b8a6331222fe5c2bcf967f50c6e424f62a5051e864941e2`  
		Last Modified: Wed, 29 Jul 2020 23:26:15 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.7-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:fee67afb8a9c6c38c60a5b90f51b6a6dfdb607b13d04240cf4faae9f8235d69d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6717777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb5af24d85d20ca2ddf1a257d6667c94e32ad6c1f381964f6ea48833ebc6eb39`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Fri, 15 May 2020 19:50:13 GMT
ENV NATS_SERVER=2.1.7
# Wed, 29 Jul 2020 23:02:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a08d7ce0399df8701d3e3cd4c36744180c3a566cdb38efeccc12a364f0083705' ;; 		armhf) natsArch='arm6'; sha256='987c23f758842fb09c0d4500f632c5302aedc61d218f03998444b94074aabddb' ;; 		armv7) natsArch='arm7'; sha256='077fd1647aa25865ade5acc3d6ee5f542d2c62feb2fb41ec6d1dd83294bea05e' ;; 		x86_64) natsArch='amd64'; sha256='23cce53fe7f628f203dbbeadf434c3480d094690aba6ff0b1d374b8f2f9ffd8c' ;; 		x86) natsArch='386'; sha256='64e271690782af823930c95574db0f701d06a36ff42b9272c04841d4611bcd15' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:02:35 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 29 Jul 2020 23:02:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Jul 2020 23:02:36 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 23:02:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:02:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0546a69fc010fc7d9fdae3cd6ff1eb8d7d7471a3561d782f6bb2bebcb079ad`  
		Last Modified: Wed, 29 Jul 2020 23:03:02 GMT  
		Size: 4.1 MB (4096870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02dc6927e9f4f4d185c4420481f8b1e06d55f058ad32ac4c0a9fc2ca3c2e0e64`  
		Last Modified: Wed, 29 Jul 2020 23:03:01 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6963e293037e1e7ddf702b89cf5a9441918b610e877f1710001b055560f92901`  
		Last Modified: Wed, 29 Jul 2020 23:03:01 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.7-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:197a92e111811ad767369a9bd75175ecb906fa57009400e78fa5d07ff8b0b47d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6515331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4546538a81c298be13378de43d24f5778e46917a8c2e6feca95287f8695e7d82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Sat, 16 May 2020 04:17:01 GMT
ENV NATS_SERVER=2.1.7
# Wed, 29 Jul 2020 23:11:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a08d7ce0399df8701d3e3cd4c36744180c3a566cdb38efeccc12a364f0083705' ;; 		armhf) natsArch='arm6'; sha256='987c23f758842fb09c0d4500f632c5302aedc61d218f03998444b94074aabddb' ;; 		armv7) natsArch='arm7'; sha256='077fd1647aa25865ade5acc3d6ee5f542d2c62feb2fb41ec6d1dd83294bea05e' ;; 		x86_64) natsArch='amd64'; sha256='23cce53fe7f628f203dbbeadf434c3480d094690aba6ff0b1d374b8f2f9ffd8c' ;; 		x86) natsArch='386'; sha256='64e271690782af823930c95574db0f701d06a36ff42b9272c04841d4611bcd15' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:11:46 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 29 Jul 2020 23:11:46 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Jul 2020 23:11:47 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 23:11:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:11:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4572ecf34c0bc5aa1ca0925f8f3c17e07cdf857ae8e31be72e5360711b24016`  
		Last Modified: Wed, 29 Jul 2020 23:15:57 GMT  
		Size: 4.1 MB (4092296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67632d2c07c7d161703500f1b0fa040775c8cb0c4474b8749a8ea961b5964f7e`  
		Last Modified: Wed, 29 Jul 2020 23:15:56 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5f50a8c5ae0937cd72ab745aacf65d53e62fed9a22d0de4fb3fe2f3d88a9b6`  
		Last Modified: Wed, 29 Jul 2020 23:15:56 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:e3338a58db906f99cb91860cf607e3670e8b6676026d2eb70d26100b26bfcd5f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6803458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e79bcc07d57e06d12e6ae92a95f16c0dfe72401e9efdc3a3869273d02110feda`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Jul 2020 16:28:21 GMT
ENV NATS_SERVER=2.1.7
# Wed, 29 Jul 2020 22:41:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a08d7ce0399df8701d3e3cd4c36744180c3a566cdb38efeccc12a364f0083705' ;; 		armhf) natsArch='arm6'; sha256='987c23f758842fb09c0d4500f632c5302aedc61d218f03998444b94074aabddb' ;; 		armv7) natsArch='arm7'; sha256='077fd1647aa25865ade5acc3d6ee5f542d2c62feb2fb41ec6d1dd83294bea05e' ;; 		x86_64) natsArch='amd64'; sha256='23cce53fe7f628f203dbbeadf434c3480d094690aba6ff0b1d374b8f2f9ffd8c' ;; 		x86) natsArch='386'; sha256='64e271690782af823930c95574db0f701d06a36ff42b9272c04841d4611bcd15' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 22:41:30 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 29 Jul 2020 22:41:30 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Jul 2020 22:41:31 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 22:41:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 22:41:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e23520311eff0ccb9b4116bad00040e13d45013d01d87ee89bba20b01b5e536`  
		Last Modified: Wed, 29 Jul 2020 22:42:03 GMT  
		Size: 4.1 MB (4078060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5bd55073b3a781fd6af08f7e29facaf7e8d37e977fc7b8a7bcb57098c1dc49b`  
		Last Modified: Wed, 29 Jul 2020 22:42:02 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2eb0d8170b7670bd8ae9406d3cc6298a0cc3b8f3ec7434dd09ec858f8701183`  
		Last Modified: Wed, 29 Jul 2020 22:42:02 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.7-alpine3.11`

```console
$ docker pull nats@sha256:2ca671f95f6f5c4d9144a701d8b7be77a1830041d86766e2e193fb58b00af449
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.1.7-alpine3.11` - linux; amd64

```console
$ docker pull nats@sha256:c1c1159e76d03431b2c612d378a62fc914f0817df3f9a8092adddb589ac74e53
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7203227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54acd9cf4794435761c0462aba37d41e69e9581a77daeef4d16255b6a579f2c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Sat, 16 May 2020 09:47:11 GMT
ENV NATS_SERVER=2.1.7
# Wed, 29 Jul 2020 23:25:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a08d7ce0399df8701d3e3cd4c36744180c3a566cdb38efeccc12a364f0083705' ;; 		armhf) natsArch='arm6'; sha256='987c23f758842fb09c0d4500f632c5302aedc61d218f03998444b94074aabddb' ;; 		armv7) natsArch='arm7'; sha256='077fd1647aa25865ade5acc3d6ee5f542d2c62feb2fb41ec6d1dd83294bea05e' ;; 		x86_64) natsArch='amd64'; sha256='23cce53fe7f628f203dbbeadf434c3480d094690aba6ff0b1d374b8f2f9ffd8c' ;; 		x86) natsArch='386'; sha256='64e271690782af823930c95574db0f701d06a36ff42b9272c04841d4611bcd15' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:25:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 29 Jul 2020 23:25:41 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Jul 2020 23:25:42 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 23:25:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:25:42 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09eebfe9509bcbfcefadbc17c68fa103be7b7cf978f08ea01527a6aba38c5554`  
		Last Modified: Wed, 29 Jul 2020 23:26:16 GMT  
		Size: 4.4 MB (4388967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab62a5d69bc21353fa665e0b7fbf8e6a4a5d3fda0e87d58c02073999f76ff43f`  
		Last Modified: Wed, 29 Jul 2020 23:26:15 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a297d716cd17565b8a6331222fe5c2bcf967f50c6e424f62a5051e864941e2`  
		Last Modified: Wed, 29 Jul 2020 23:26:15 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.7-alpine3.11` - linux; arm variant v6

```console
$ docker pull nats@sha256:fee67afb8a9c6c38c60a5b90f51b6a6dfdb607b13d04240cf4faae9f8235d69d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6717777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb5af24d85d20ca2ddf1a257d6667c94e32ad6c1f381964f6ea48833ebc6eb39`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Fri, 15 May 2020 19:50:13 GMT
ENV NATS_SERVER=2.1.7
# Wed, 29 Jul 2020 23:02:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a08d7ce0399df8701d3e3cd4c36744180c3a566cdb38efeccc12a364f0083705' ;; 		armhf) natsArch='arm6'; sha256='987c23f758842fb09c0d4500f632c5302aedc61d218f03998444b94074aabddb' ;; 		armv7) natsArch='arm7'; sha256='077fd1647aa25865ade5acc3d6ee5f542d2c62feb2fb41ec6d1dd83294bea05e' ;; 		x86_64) natsArch='amd64'; sha256='23cce53fe7f628f203dbbeadf434c3480d094690aba6ff0b1d374b8f2f9ffd8c' ;; 		x86) natsArch='386'; sha256='64e271690782af823930c95574db0f701d06a36ff42b9272c04841d4611bcd15' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:02:35 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 29 Jul 2020 23:02:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Jul 2020 23:02:36 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 23:02:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:02:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0546a69fc010fc7d9fdae3cd6ff1eb8d7d7471a3561d782f6bb2bebcb079ad`  
		Last Modified: Wed, 29 Jul 2020 23:03:02 GMT  
		Size: 4.1 MB (4096870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02dc6927e9f4f4d185c4420481f8b1e06d55f058ad32ac4c0a9fc2ca3c2e0e64`  
		Last Modified: Wed, 29 Jul 2020 23:03:01 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6963e293037e1e7ddf702b89cf5a9441918b610e877f1710001b055560f92901`  
		Last Modified: Wed, 29 Jul 2020 23:03:01 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.7-alpine3.11` - linux; arm variant v7

```console
$ docker pull nats@sha256:197a92e111811ad767369a9bd75175ecb906fa57009400e78fa5d07ff8b0b47d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6515331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4546538a81c298be13378de43d24f5778e46917a8c2e6feca95287f8695e7d82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Sat, 16 May 2020 04:17:01 GMT
ENV NATS_SERVER=2.1.7
# Wed, 29 Jul 2020 23:11:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a08d7ce0399df8701d3e3cd4c36744180c3a566cdb38efeccc12a364f0083705' ;; 		armhf) natsArch='arm6'; sha256='987c23f758842fb09c0d4500f632c5302aedc61d218f03998444b94074aabddb' ;; 		armv7) natsArch='arm7'; sha256='077fd1647aa25865ade5acc3d6ee5f542d2c62feb2fb41ec6d1dd83294bea05e' ;; 		x86_64) natsArch='amd64'; sha256='23cce53fe7f628f203dbbeadf434c3480d094690aba6ff0b1d374b8f2f9ffd8c' ;; 		x86) natsArch='386'; sha256='64e271690782af823930c95574db0f701d06a36ff42b9272c04841d4611bcd15' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:11:46 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 29 Jul 2020 23:11:46 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Jul 2020 23:11:47 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 23:11:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:11:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4572ecf34c0bc5aa1ca0925f8f3c17e07cdf857ae8e31be72e5360711b24016`  
		Last Modified: Wed, 29 Jul 2020 23:15:57 GMT  
		Size: 4.1 MB (4092296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67632d2c07c7d161703500f1b0fa040775c8cb0c4474b8749a8ea961b5964f7e`  
		Last Modified: Wed, 29 Jul 2020 23:15:56 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5f50a8c5ae0937cd72ab745aacf65d53e62fed9a22d0de4fb3fe2f3d88a9b6`  
		Last Modified: Wed, 29 Jul 2020 23:15:56 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.7-alpine3.11` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:e3338a58db906f99cb91860cf607e3670e8b6676026d2eb70d26100b26bfcd5f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6803458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e79bcc07d57e06d12e6ae92a95f16c0dfe72401e9efdc3a3869273d02110feda`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Jul 2020 16:28:21 GMT
ENV NATS_SERVER=2.1.7
# Wed, 29 Jul 2020 22:41:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a08d7ce0399df8701d3e3cd4c36744180c3a566cdb38efeccc12a364f0083705' ;; 		armhf) natsArch='arm6'; sha256='987c23f758842fb09c0d4500f632c5302aedc61d218f03998444b94074aabddb' ;; 		armv7) natsArch='arm7'; sha256='077fd1647aa25865ade5acc3d6ee5f542d2c62feb2fb41ec6d1dd83294bea05e' ;; 		x86_64) natsArch='amd64'; sha256='23cce53fe7f628f203dbbeadf434c3480d094690aba6ff0b1d374b8f2f9ffd8c' ;; 		x86) natsArch='386'; sha256='64e271690782af823930c95574db0f701d06a36ff42b9272c04841d4611bcd15' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 22:41:30 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 29 Jul 2020 22:41:30 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Jul 2020 22:41:31 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 22:41:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 22:41:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e23520311eff0ccb9b4116bad00040e13d45013d01d87ee89bba20b01b5e536`  
		Last Modified: Wed, 29 Jul 2020 22:42:03 GMT  
		Size: 4.1 MB (4078060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5bd55073b3a781fd6af08f7e29facaf7e8d37e977fc7b8a7bcb57098c1dc49b`  
		Last Modified: Wed, 29 Jul 2020 22:42:02 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2eb0d8170b7670bd8ae9406d3cc6298a0cc3b8f3ec7434dd09ec858f8701183`  
		Last Modified: Wed, 29 Jul 2020 22:42:02 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.7-linux`

```console
$ docker pull nats@sha256:7a3219e049b4d8b10a7ff389fa689c8d08d5732fe37dcf9c5a72fda463d6c6ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.1.7-linux` - linux; amd64

```console
$ docker pull nats@sha256:6aace730d886f9719841c60ec11f826e494b8fcc631378b32f5e01ca32d87ab9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4087969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e93a56bc1852bb18d91f1741edde016c59b49c92f7ad91960d583ee0486ebf3`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 16 May 2020 09:47:58 GMT
COPY file:27ab63fb5115ca3cb7456a256d6d6dab7ba864d8806821652fbe569f4f845df5 in /nats-server 
# Sat, 16 May 2020 09:47:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 16 May 2020 09:47:59 GMT
EXPOSE 4222 6222 8222
# Sat, 16 May 2020 09:47:59 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 16 May 2020 09:47:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b509577c042697add820579de13ceed535b1c02ec7fa460b892d6c63941390a7`  
		Last Modified: Sat, 16 May 2020 09:48:21 GMT  
		Size: 4.1 MB (4087491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ce65065eb7bc6684476be5937b3d0d4046e7cc7241bc5017d70488d0edbfe3`  
		Last Modified: Sat, 16 May 2020 09:48:20 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.7-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:e8b59aabb2b6838ced59a3125ba4216cc8a4d0622f8b8c1e9e40fb30cd63a135
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3796375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8116ee7998ff454ed4eaa153438504925828993f56f26fb96fd11b31c9dc2128`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 15 May 2020 19:53:42 GMT
COPY file:9951c1b4ae20021f4d6efd6c039d0f0d0044470572e81beae625f15ffa13d2f1 in /nats-server 
# Fri, 15 May 2020 19:53:43 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 15 May 2020 19:53:44 GMT
EXPOSE 4222 6222 8222
# Fri, 15 May 2020 19:53:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 15 May 2020 19:53:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7976dc3d59fddf78c4ca25d0692135431e63b9fb744ae2c3d02b7a8214b5bfd9`  
		Last Modified: Fri, 15 May 2020 19:54:21 GMT  
		Size: 3.8 MB (3795898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b520f7415a5fab1b4a83eb7a8259e321475f75f5b06bfe95493b598c9ee9f4`  
		Last Modified: Fri, 15 May 2020 19:54:20 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.7-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:707f02b7c81a3f071abba9ce0a74b1cf0bf7a664e0220ab6cae112f2721a24bf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3792273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d2f2220669ef3621c45d5e4fd8460e7378e258044eb57003584ce55db5bdd9b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 16 May 2020 04:26:09 GMT
COPY file:3320edcd8f0db9551469809c752244493d1c6cf3be0287714c8a507e339283b2 in /nats-server 
# Sat, 16 May 2020 04:26:09 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 16 May 2020 04:26:11 GMT
EXPOSE 4222 6222 8222
# Sat, 16 May 2020 04:26:12 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 16 May 2020 04:26:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7ceefb66163b74f9719728ecace35bd406e85998a252d90c9e07a02582c7b6f1`  
		Last Modified: Sat, 16 May 2020 04:26:55 GMT  
		Size: 3.8 MB (3791795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db182fe235e1ef3b80de633e39d8ab9040cef44127adee97dbc4513df27dacfe`  
		Last Modified: Sat, 16 May 2020 04:26:53 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.7-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8cb2b90d45f90f3bdfb841b4a1399ff3a1b0a835e54664ee375ef309ff4c4398
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3776968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fffbb615827376dda1ad45bce22763d7cdc858675e4eafc55deb2d134f813338`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 29 Jul 2020 22:41:42 GMT
COPY file:67a03d7df05756de9c16c4cd22dfaf6ed9cc9a43b78a90ebfaa81ee7ebbc7abf in /nats-server 
# Wed, 29 Jul 2020 22:41:43 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 29 Jul 2020 22:41:44 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 22:41:44 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 29 Jul 2020 22:41:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:39a183ba93759b5fab08b0cb81f1f1a4c9f5a95c3746b031082c6bc3a57441b3`  
		Last Modified: Wed, 29 Jul 2020 22:42:18 GMT  
		Size: 3.8 MB (3776492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a510a0d87b5b915212ee2a5e5d877dced1c30164c0e82d6e60951d00374fe7`  
		Last Modified: Wed, 29 Jul 2020 22:42:17 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.7-nanoserver`

```console
$ docker pull nats@sha256:d3e9d8a5a0ad31f0845175c1071e35cea4ac4ebb849c16526e0664a3c0918608
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `nats:2.1.7-nanoserver` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats@sha256:00f69dcad2cdf6b3da43ef4701091ca04d3f35b2ec80c666554d49e5684258d8
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (104957159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edebc41e62feb1ccc604f2e015421dd2e938344719a06d92981822566271a91b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Jul 2020 13:50:07 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jul 2020 15:05:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 15:05:16 GMT
RUN cmd /S /C #(nop) COPY file:18561b827240029ad80d0e3d25142efae62905c30cc520fc37cfc68e7d889848 in C:\nats-server.exe 
# Wed, 15 Jul 2020 15:05:18 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jul 2020 15:05:18 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Jul 2020 15:05:19 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jul 2020 15:05:20 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:dc95608099543221ef539391bfece5c1ce37b97af9da457f5990349cab028a12`  
		Size: 100.9 MB (100895619 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5f0c27d781c53928c03429d5b34e0f49fc26b7e7c996c1d9a2a8474162eade60`  
		Last Modified: Wed, 15 Jul 2020 15:09:50 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10a270f5d0666930958ddfeac073712f678d77b5a05a08210012ada454204077`  
		Last Modified: Wed, 15 Jul 2020 15:10:00 GMT  
		Size: 4.1 MB (4056451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b5e48167a563124481e83cd3f3e3ca1bd3ea8f52b9e52dc9b4982e98a21d7d`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 1.5 KB (1470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64aecdf43c40f563833e5ad1c027bb2e67c1b0c51bb2ab795b99df1f4c2f26f`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 930.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:accd609b6f7304740da44e2a7331717a73ec3f94a35c25198a189b81bd84e204`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 928.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84a11ddf5d09a44b078d904b91df1cd82bf2a0cefb6ec9f52761f36fcf23f54`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.7-nanoserver-1809`

```console
$ docker pull nats@sha256:d3e9d8a5a0ad31f0845175c1071e35cea4ac4ebb849c16526e0664a3c0918608
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `nats:2.1.7-nanoserver-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats@sha256:00f69dcad2cdf6b3da43ef4701091ca04d3f35b2ec80c666554d49e5684258d8
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (104957159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edebc41e62feb1ccc604f2e015421dd2e938344719a06d92981822566271a91b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Jul 2020 13:50:07 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jul 2020 15:05:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 15:05:16 GMT
RUN cmd /S /C #(nop) COPY file:18561b827240029ad80d0e3d25142efae62905c30cc520fc37cfc68e7d889848 in C:\nats-server.exe 
# Wed, 15 Jul 2020 15:05:18 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jul 2020 15:05:18 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Jul 2020 15:05:19 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jul 2020 15:05:20 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:dc95608099543221ef539391bfece5c1ce37b97af9da457f5990349cab028a12`  
		Size: 100.9 MB (100895619 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5f0c27d781c53928c03429d5b34e0f49fc26b7e7c996c1d9a2a8474162eade60`  
		Last Modified: Wed, 15 Jul 2020 15:09:50 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10a270f5d0666930958ddfeac073712f678d77b5a05a08210012ada454204077`  
		Last Modified: Wed, 15 Jul 2020 15:10:00 GMT  
		Size: 4.1 MB (4056451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b5e48167a563124481e83cd3f3e3ca1bd3ea8f52b9e52dc9b4982e98a21d7d`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 1.5 KB (1470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64aecdf43c40f563833e5ad1c027bb2e67c1b0c51bb2ab795b99df1f4c2f26f`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 930.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:accd609b6f7304740da44e2a7331717a73ec3f94a35c25198a189b81bd84e204`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 928.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84a11ddf5d09a44b078d904b91df1cd82bf2a0cefb6ec9f52761f36fcf23f54`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.7-scratch`

```console
$ docker pull nats@sha256:7a3219e049b4d8b10a7ff389fa689c8d08d5732fe37dcf9c5a72fda463d6c6ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.1.7-scratch` - linux; amd64

```console
$ docker pull nats@sha256:6aace730d886f9719841c60ec11f826e494b8fcc631378b32f5e01ca32d87ab9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4087969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e93a56bc1852bb18d91f1741edde016c59b49c92f7ad91960d583ee0486ebf3`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 16 May 2020 09:47:58 GMT
COPY file:27ab63fb5115ca3cb7456a256d6d6dab7ba864d8806821652fbe569f4f845df5 in /nats-server 
# Sat, 16 May 2020 09:47:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 16 May 2020 09:47:59 GMT
EXPOSE 4222 6222 8222
# Sat, 16 May 2020 09:47:59 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 16 May 2020 09:47:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b509577c042697add820579de13ceed535b1c02ec7fa460b892d6c63941390a7`  
		Last Modified: Sat, 16 May 2020 09:48:21 GMT  
		Size: 4.1 MB (4087491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ce65065eb7bc6684476be5937b3d0d4046e7cc7241bc5017d70488d0edbfe3`  
		Last Modified: Sat, 16 May 2020 09:48:20 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.7-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:e8b59aabb2b6838ced59a3125ba4216cc8a4d0622f8b8c1e9e40fb30cd63a135
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3796375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8116ee7998ff454ed4eaa153438504925828993f56f26fb96fd11b31c9dc2128`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 15 May 2020 19:53:42 GMT
COPY file:9951c1b4ae20021f4d6efd6c039d0f0d0044470572e81beae625f15ffa13d2f1 in /nats-server 
# Fri, 15 May 2020 19:53:43 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 15 May 2020 19:53:44 GMT
EXPOSE 4222 6222 8222
# Fri, 15 May 2020 19:53:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 15 May 2020 19:53:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7976dc3d59fddf78c4ca25d0692135431e63b9fb744ae2c3d02b7a8214b5bfd9`  
		Last Modified: Fri, 15 May 2020 19:54:21 GMT  
		Size: 3.8 MB (3795898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b520f7415a5fab1b4a83eb7a8259e321475f75f5b06bfe95493b598c9ee9f4`  
		Last Modified: Fri, 15 May 2020 19:54:20 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.7-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:707f02b7c81a3f071abba9ce0a74b1cf0bf7a664e0220ab6cae112f2721a24bf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3792273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d2f2220669ef3621c45d5e4fd8460e7378e258044eb57003584ce55db5bdd9b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 16 May 2020 04:26:09 GMT
COPY file:3320edcd8f0db9551469809c752244493d1c6cf3be0287714c8a507e339283b2 in /nats-server 
# Sat, 16 May 2020 04:26:09 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 16 May 2020 04:26:11 GMT
EXPOSE 4222 6222 8222
# Sat, 16 May 2020 04:26:12 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 16 May 2020 04:26:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7ceefb66163b74f9719728ecace35bd406e85998a252d90c9e07a02582c7b6f1`  
		Last Modified: Sat, 16 May 2020 04:26:55 GMT  
		Size: 3.8 MB (3791795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db182fe235e1ef3b80de633e39d8ab9040cef44127adee97dbc4513df27dacfe`  
		Last Modified: Sat, 16 May 2020 04:26:53 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.7-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8cb2b90d45f90f3bdfb841b4a1399ff3a1b0a835e54664ee375ef309ff4c4398
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3776968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fffbb615827376dda1ad45bce22763d7cdc858675e4eafc55deb2d134f813338`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 29 Jul 2020 22:41:42 GMT
COPY file:67a03d7df05756de9c16c4cd22dfaf6ed9cc9a43b78a90ebfaa81ee7ebbc7abf in /nats-server 
# Wed, 29 Jul 2020 22:41:43 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 29 Jul 2020 22:41:44 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 22:41:44 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 29 Jul 2020 22:41:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:39a183ba93759b5fab08b0cb81f1f1a4c9f5a95c3746b031082c6bc3a57441b3`  
		Last Modified: Wed, 29 Jul 2020 22:42:18 GMT  
		Size: 3.8 MB (3776492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a510a0d87b5b915212ee2a5e5d877dced1c30164c0e82d6e60951d00374fe7`  
		Last Modified: Wed, 29 Jul 2020 22:42:17 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.7-windowsservercore`

```console
$ docker pull nats@sha256:59a9a5745643d652dd6d49be5d422a2270a2539f6dfa398ba219d78c00c701e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64
	-	windows version 10.0.14393.3808; amd64

### `nats:2.1.7-windowsservercore` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats@sha256:84ed3b1eb1e35102dff57509d666e9ae99f4fd0a492b9410b473bedda4aeebdf
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2328185203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8d69d5e23b4cff9ad8df708d4059e6525b91686ad490775e104e6c06b863457`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Wed, 15 Jul 2020 12:15:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jul 2020 15:03:03 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 15:03:03 GMT
ENV NATS_SERVER=2.1.7
# Wed, 15 Jul 2020 15:03:04 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.7/nats-server-v2.1.7-windows-amd64.zip
# Wed, 29 Jul 2020 23:14:26 GMT
ENV GIT_DOWNLOAD_SHA256=1e1ad5c00929cc145341fd65f8b0a41a38e942b9b9fd9fdb0216c47654afdc8f
# Wed, 29 Jul 2020 23:15:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 29 Jul 2020 23:16:49 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 29 Jul 2020 23:16:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 29 Jul 2020 23:16:54 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 23:16:55 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 29 Jul 2020 23:16:56 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1cc883a0e3509a474bb32f3c40411bf86219325ae9710e25a5dcce6b44eef357`  
		Last Modified: Wed, 15 Jul 2020 14:32:06 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dd35c9a62007b6ded1ca968562be97de62ea3e2b3c7db85f4a50baaa9efecb`  
		Last Modified: Wed, 15 Jul 2020 15:09:33 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5789d32300712f2fa8b6564efe911f5f523cf150f1fde2bf8d6deedbb56feb4`  
		Last Modified: Wed, 15 Jul 2020 15:09:32 GMT  
		Size: 1.1 KB (1105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b62b1740ff37517c10b8b8bfae73367d0c5538cf934392846eea648031c1857`  
		Last Modified: Wed, 15 Jul 2020 15:09:31 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c765e0c4aba82f5140dd325bb9fc2dc97095f673b4d88039867aecc92e331f5e`  
		Last Modified: Wed, 29 Jul 2020 23:21:23 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9dfd44060c9c9e79fca23ba4227434b55a5a3353c7a32ba8140fa252af2631f`  
		Last Modified: Wed, 29 Jul 2020 23:21:24 GMT  
		Size: 4.8 MB (4803853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011be3335c53769b99af80accd8e25f40172d44bc0e20780c88f1ab787bbf09e`  
		Last Modified: Wed, 29 Jul 2020 23:21:24 GMT  
		Size: 13.2 MB (13178319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f913f5767f1c088f27134bdefc531acacd106610ce085ef7ca5470fdeda55e80`  
		Last Modified: Wed, 29 Jul 2020 23:21:20 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8436f3f54d22f495452cdb61489bf5833c2cda6a2e6012c732b2c8ffbc72262f`  
		Last Modified: Wed, 29 Jul 2020 23:21:20 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12724c1ab2196db2d2cd8bff6069b1ea932e514cd5473240dd515f50361e4fa`  
		Last Modified: Wed, 29 Jul 2020 23:21:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419a5e47094ff5e8a8cb733bf81fcd97e46b00a5b62b9cbcd5993a66942a7e7e`  
		Last Modified: Wed, 29 Jul 2020 23:21:20 GMT  
		Size: 1.1 KB (1100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.7-windowsservercore` - windows version 10.0.14393.3808; amd64

```console
$ docker pull nats@sha256:9145e80ebf209b601e34e199defd755bf43a5b09f674ece13c4c6299b21d4870
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5756757168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a3c13889118f6f6c65e859be772b7b0cb7e0497de0a2326a3b54c097daa6670`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Jul 2020 21:05:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Jul 2020 12:24:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jul 2020 15:05:26 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 15:05:27 GMT
ENV NATS_SERVER=2.1.7
# Wed, 15 Jul 2020 15:05:28 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.7/nats-server-v2.1.7-windows-amd64.zip
# Wed, 29 Jul 2020 23:17:15 GMT
ENV GIT_DOWNLOAD_SHA256=1e1ad5c00929cc145341fd65f8b0a41a38e942b9b9fd9fdb0216c47654afdc8f
# Wed, 29 Jul 2020 23:18:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 29 Jul 2020 23:20:43 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 29 Jul 2020 23:20:45 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 29 Jul 2020 23:20:46 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 23:20:47 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 29 Jul 2020 23:20:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:802c4beb8b091968ccf1bb4a853ded7955ddb79e6f8775a5155cb5ed07dcbcab`  
		Size: 1.7 GB (1667476199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3393eecaf56a66035ab178b379bacf81d30373b630b34b2973501f259aadb0f6`  
		Last Modified: Wed, 15 Jul 2020 14:32:38 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1430ee68db5fe3026683f1b7c74f31ae748da71bf8ad611efede726e9e036b1`  
		Last Modified: Wed, 15 Jul 2020 15:10:21 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae29b1720308eb8710d921cefbc8979061e4535b6276b35b3d471e08a09e7af`  
		Last Modified: Wed, 15 Jul 2020 15:10:19 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a76213345cac0ca18badbc3c8262b6973e3457484fdcb9af380fa4de2c64ea`  
		Last Modified: Wed, 15 Jul 2020 15:10:19 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2713fe8ba40241bc8ef85e6795703e42f101f0ab81d143357c549a03c4b00c`  
		Last Modified: Wed, 29 Jul 2020 23:21:44 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b8f23b09829f938cc622501d4059590b050bc95a7fb4c5d2e337e423af1e23`  
		Last Modified: Wed, 29 Jul 2020 23:21:46 GMT  
		Size: 5.4 MB (5391705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0857d1594c42a8ff34ec0fc99b717f343d2e6dcdcb980e3b54621a8127ecf4a`  
		Last Modified: Wed, 29 Jul 2020 23:21:57 GMT  
		Size: 13.9 MB (13892511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7afe295ad113f1145078cde44f86ce197d64aa5ceb92784bf4c60ff710b95256`  
		Last Modified: Wed, 29 Jul 2020 23:21:41 GMT  
		Size: 1.7 KB (1683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9b54006dba8cc76bc2325f78d0377969e727070a8f9069e26090b7a4e18f36`  
		Last Modified: Wed, 29 Jul 2020 23:21:41 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97bb5b91db82c40b2b26f5fcc7a1e07fce677242cd70722fbe2d3256e4548dfc`  
		Last Modified: Wed, 29 Jul 2020 23:21:42 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58919d245b3713c0a29f1039075f368c82d09514f57a595cade8fae1010c7847`  
		Last Modified: Wed, 29 Jul 2020 23:21:42 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.7-windowsservercore-1809`

```console
$ docker pull nats@sha256:f9351e549406b5be23d79a960a8188aae30b521a25b98855bcf4ad382d0446e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `nats:2.1.7-windowsservercore-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats@sha256:84ed3b1eb1e35102dff57509d666e9ae99f4fd0a492b9410b473bedda4aeebdf
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2328185203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8d69d5e23b4cff9ad8df708d4059e6525b91686ad490775e104e6c06b863457`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Wed, 15 Jul 2020 12:15:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jul 2020 15:03:03 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 15:03:03 GMT
ENV NATS_SERVER=2.1.7
# Wed, 15 Jul 2020 15:03:04 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.7/nats-server-v2.1.7-windows-amd64.zip
# Wed, 29 Jul 2020 23:14:26 GMT
ENV GIT_DOWNLOAD_SHA256=1e1ad5c00929cc145341fd65f8b0a41a38e942b9b9fd9fdb0216c47654afdc8f
# Wed, 29 Jul 2020 23:15:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 29 Jul 2020 23:16:49 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 29 Jul 2020 23:16:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 29 Jul 2020 23:16:54 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 23:16:55 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 29 Jul 2020 23:16:56 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1cc883a0e3509a474bb32f3c40411bf86219325ae9710e25a5dcce6b44eef357`  
		Last Modified: Wed, 15 Jul 2020 14:32:06 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dd35c9a62007b6ded1ca968562be97de62ea3e2b3c7db85f4a50baaa9efecb`  
		Last Modified: Wed, 15 Jul 2020 15:09:33 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5789d32300712f2fa8b6564efe911f5f523cf150f1fde2bf8d6deedbb56feb4`  
		Last Modified: Wed, 15 Jul 2020 15:09:32 GMT  
		Size: 1.1 KB (1105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b62b1740ff37517c10b8b8bfae73367d0c5538cf934392846eea648031c1857`  
		Last Modified: Wed, 15 Jul 2020 15:09:31 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c765e0c4aba82f5140dd325bb9fc2dc97095f673b4d88039867aecc92e331f5e`  
		Last Modified: Wed, 29 Jul 2020 23:21:23 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9dfd44060c9c9e79fca23ba4227434b55a5a3353c7a32ba8140fa252af2631f`  
		Last Modified: Wed, 29 Jul 2020 23:21:24 GMT  
		Size: 4.8 MB (4803853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011be3335c53769b99af80accd8e25f40172d44bc0e20780c88f1ab787bbf09e`  
		Last Modified: Wed, 29 Jul 2020 23:21:24 GMT  
		Size: 13.2 MB (13178319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f913f5767f1c088f27134bdefc531acacd106610ce085ef7ca5470fdeda55e80`  
		Last Modified: Wed, 29 Jul 2020 23:21:20 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8436f3f54d22f495452cdb61489bf5833c2cda6a2e6012c732b2c8ffbc72262f`  
		Last Modified: Wed, 29 Jul 2020 23:21:20 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12724c1ab2196db2d2cd8bff6069b1ea932e514cd5473240dd515f50361e4fa`  
		Last Modified: Wed, 29 Jul 2020 23:21:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419a5e47094ff5e8a8cb733bf81fcd97e46b00a5b62b9cbcd5993a66942a7e7e`  
		Last Modified: Wed, 29 Jul 2020 23:21:20 GMT  
		Size: 1.1 KB (1100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.7-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:f405d1c17c29cd33ba2762684ab3ee983dbaafd8df62ef7b12fa78b3ad6b7d3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3808; amd64

### `nats:2.1.7-windowsservercore-ltsc2016` - windows version 10.0.14393.3808; amd64

```console
$ docker pull nats@sha256:9145e80ebf209b601e34e199defd755bf43a5b09f674ece13c4c6299b21d4870
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5756757168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a3c13889118f6f6c65e859be772b7b0cb7e0497de0a2326a3b54c097daa6670`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Jul 2020 21:05:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Jul 2020 12:24:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jul 2020 15:05:26 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 15:05:27 GMT
ENV NATS_SERVER=2.1.7
# Wed, 15 Jul 2020 15:05:28 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.7/nats-server-v2.1.7-windows-amd64.zip
# Wed, 29 Jul 2020 23:17:15 GMT
ENV GIT_DOWNLOAD_SHA256=1e1ad5c00929cc145341fd65f8b0a41a38e942b9b9fd9fdb0216c47654afdc8f
# Wed, 29 Jul 2020 23:18:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 29 Jul 2020 23:20:43 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 29 Jul 2020 23:20:45 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 29 Jul 2020 23:20:46 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 23:20:47 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 29 Jul 2020 23:20:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:802c4beb8b091968ccf1bb4a853ded7955ddb79e6f8775a5155cb5ed07dcbcab`  
		Size: 1.7 GB (1667476199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3393eecaf56a66035ab178b379bacf81d30373b630b34b2973501f259aadb0f6`  
		Last Modified: Wed, 15 Jul 2020 14:32:38 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1430ee68db5fe3026683f1b7c74f31ae748da71bf8ad611efede726e9e036b1`  
		Last Modified: Wed, 15 Jul 2020 15:10:21 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae29b1720308eb8710d921cefbc8979061e4535b6276b35b3d471e08a09e7af`  
		Last Modified: Wed, 15 Jul 2020 15:10:19 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a76213345cac0ca18badbc3c8262b6973e3457484fdcb9af380fa4de2c64ea`  
		Last Modified: Wed, 15 Jul 2020 15:10:19 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2713fe8ba40241bc8ef85e6795703e42f101f0ab81d143357c549a03c4b00c`  
		Last Modified: Wed, 29 Jul 2020 23:21:44 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b8f23b09829f938cc622501d4059590b050bc95a7fb4c5d2e337e423af1e23`  
		Last Modified: Wed, 29 Jul 2020 23:21:46 GMT  
		Size: 5.4 MB (5391705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0857d1594c42a8ff34ec0fc99b717f343d2e6dcdcb980e3b54621a8127ecf4a`  
		Last Modified: Wed, 29 Jul 2020 23:21:57 GMT  
		Size: 13.9 MB (13892511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7afe295ad113f1145078cde44f86ce197d64aa5ceb92784bf4c60ff710b95256`  
		Last Modified: Wed, 29 Jul 2020 23:21:41 GMT  
		Size: 1.7 KB (1683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9b54006dba8cc76bc2325f78d0377969e727070a8f9069e26090b7a4e18f36`  
		Last Modified: Wed, 29 Jul 2020 23:21:41 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97bb5b91db82c40b2b26f5fcc7a1e07fce677242cd70722fbe2d3256e4548dfc`  
		Last Modified: Wed, 29 Jul 2020 23:21:42 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58919d245b3713c0a29f1039075f368c82d09514f57a595cade8fae1010c7847`  
		Last Modified: Wed, 29 Jul 2020 23:21:42 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-alpine`

```console
$ docker pull nats@sha256:2ca671f95f6f5c4d9144a701d8b7be77a1830041d86766e2e193fb58b00af449
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.1-alpine` - linux; amd64

```console
$ docker pull nats@sha256:c1c1159e76d03431b2c612d378a62fc914f0817df3f9a8092adddb589ac74e53
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7203227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54acd9cf4794435761c0462aba37d41e69e9581a77daeef4d16255b6a579f2c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Sat, 16 May 2020 09:47:11 GMT
ENV NATS_SERVER=2.1.7
# Wed, 29 Jul 2020 23:25:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a08d7ce0399df8701d3e3cd4c36744180c3a566cdb38efeccc12a364f0083705' ;; 		armhf) natsArch='arm6'; sha256='987c23f758842fb09c0d4500f632c5302aedc61d218f03998444b94074aabddb' ;; 		armv7) natsArch='arm7'; sha256='077fd1647aa25865ade5acc3d6ee5f542d2c62feb2fb41ec6d1dd83294bea05e' ;; 		x86_64) natsArch='amd64'; sha256='23cce53fe7f628f203dbbeadf434c3480d094690aba6ff0b1d374b8f2f9ffd8c' ;; 		x86) natsArch='386'; sha256='64e271690782af823930c95574db0f701d06a36ff42b9272c04841d4611bcd15' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:25:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 29 Jul 2020 23:25:41 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Jul 2020 23:25:42 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 23:25:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:25:42 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09eebfe9509bcbfcefadbc17c68fa103be7b7cf978f08ea01527a6aba38c5554`  
		Last Modified: Wed, 29 Jul 2020 23:26:16 GMT  
		Size: 4.4 MB (4388967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab62a5d69bc21353fa665e0b7fbf8e6a4a5d3fda0e87d58c02073999f76ff43f`  
		Last Modified: Wed, 29 Jul 2020 23:26:15 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a297d716cd17565b8a6331222fe5c2bcf967f50c6e424f62a5051e864941e2`  
		Last Modified: Wed, 29 Jul 2020 23:26:15 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:fee67afb8a9c6c38c60a5b90f51b6a6dfdb607b13d04240cf4faae9f8235d69d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6717777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb5af24d85d20ca2ddf1a257d6667c94e32ad6c1f381964f6ea48833ebc6eb39`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Fri, 15 May 2020 19:50:13 GMT
ENV NATS_SERVER=2.1.7
# Wed, 29 Jul 2020 23:02:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a08d7ce0399df8701d3e3cd4c36744180c3a566cdb38efeccc12a364f0083705' ;; 		armhf) natsArch='arm6'; sha256='987c23f758842fb09c0d4500f632c5302aedc61d218f03998444b94074aabddb' ;; 		armv7) natsArch='arm7'; sha256='077fd1647aa25865ade5acc3d6ee5f542d2c62feb2fb41ec6d1dd83294bea05e' ;; 		x86_64) natsArch='amd64'; sha256='23cce53fe7f628f203dbbeadf434c3480d094690aba6ff0b1d374b8f2f9ffd8c' ;; 		x86) natsArch='386'; sha256='64e271690782af823930c95574db0f701d06a36ff42b9272c04841d4611bcd15' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:02:35 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 29 Jul 2020 23:02:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Jul 2020 23:02:36 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 23:02:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:02:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0546a69fc010fc7d9fdae3cd6ff1eb8d7d7471a3561d782f6bb2bebcb079ad`  
		Last Modified: Wed, 29 Jul 2020 23:03:02 GMT  
		Size: 4.1 MB (4096870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02dc6927e9f4f4d185c4420481f8b1e06d55f058ad32ac4c0a9fc2ca3c2e0e64`  
		Last Modified: Wed, 29 Jul 2020 23:03:01 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6963e293037e1e7ddf702b89cf5a9441918b610e877f1710001b055560f92901`  
		Last Modified: Wed, 29 Jul 2020 23:03:01 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:197a92e111811ad767369a9bd75175ecb906fa57009400e78fa5d07ff8b0b47d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6515331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4546538a81c298be13378de43d24f5778e46917a8c2e6feca95287f8695e7d82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Sat, 16 May 2020 04:17:01 GMT
ENV NATS_SERVER=2.1.7
# Wed, 29 Jul 2020 23:11:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a08d7ce0399df8701d3e3cd4c36744180c3a566cdb38efeccc12a364f0083705' ;; 		armhf) natsArch='arm6'; sha256='987c23f758842fb09c0d4500f632c5302aedc61d218f03998444b94074aabddb' ;; 		armv7) natsArch='arm7'; sha256='077fd1647aa25865ade5acc3d6ee5f542d2c62feb2fb41ec6d1dd83294bea05e' ;; 		x86_64) natsArch='amd64'; sha256='23cce53fe7f628f203dbbeadf434c3480d094690aba6ff0b1d374b8f2f9ffd8c' ;; 		x86) natsArch='386'; sha256='64e271690782af823930c95574db0f701d06a36ff42b9272c04841d4611bcd15' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:11:46 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 29 Jul 2020 23:11:46 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Jul 2020 23:11:47 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 23:11:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:11:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4572ecf34c0bc5aa1ca0925f8f3c17e07cdf857ae8e31be72e5360711b24016`  
		Last Modified: Wed, 29 Jul 2020 23:15:57 GMT  
		Size: 4.1 MB (4092296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67632d2c07c7d161703500f1b0fa040775c8cb0c4474b8749a8ea961b5964f7e`  
		Last Modified: Wed, 29 Jul 2020 23:15:56 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5f50a8c5ae0937cd72ab745aacf65d53e62fed9a22d0de4fb3fe2f3d88a9b6`  
		Last Modified: Wed, 29 Jul 2020 23:15:56 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:e3338a58db906f99cb91860cf607e3670e8b6676026d2eb70d26100b26bfcd5f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6803458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e79bcc07d57e06d12e6ae92a95f16c0dfe72401e9efdc3a3869273d02110feda`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Jul 2020 16:28:21 GMT
ENV NATS_SERVER=2.1.7
# Wed, 29 Jul 2020 22:41:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a08d7ce0399df8701d3e3cd4c36744180c3a566cdb38efeccc12a364f0083705' ;; 		armhf) natsArch='arm6'; sha256='987c23f758842fb09c0d4500f632c5302aedc61d218f03998444b94074aabddb' ;; 		armv7) natsArch='arm7'; sha256='077fd1647aa25865ade5acc3d6ee5f542d2c62feb2fb41ec6d1dd83294bea05e' ;; 		x86_64) natsArch='amd64'; sha256='23cce53fe7f628f203dbbeadf434c3480d094690aba6ff0b1d374b8f2f9ffd8c' ;; 		x86) natsArch='386'; sha256='64e271690782af823930c95574db0f701d06a36ff42b9272c04841d4611bcd15' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 22:41:30 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 29 Jul 2020 22:41:30 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Jul 2020 22:41:31 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 22:41:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 22:41:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e23520311eff0ccb9b4116bad00040e13d45013d01d87ee89bba20b01b5e536`  
		Last Modified: Wed, 29 Jul 2020 22:42:03 GMT  
		Size: 4.1 MB (4078060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5bd55073b3a781fd6af08f7e29facaf7e8d37e977fc7b8a7bcb57098c1dc49b`  
		Last Modified: Wed, 29 Jul 2020 22:42:02 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2eb0d8170b7670bd8ae9406d3cc6298a0cc3b8f3ec7434dd09ec858f8701183`  
		Last Modified: Wed, 29 Jul 2020 22:42:02 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-alpine3.11`

```console
$ docker pull nats@sha256:2ca671f95f6f5c4d9144a701d8b7be77a1830041d86766e2e193fb58b00af449
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.1-alpine3.11` - linux; amd64

```console
$ docker pull nats@sha256:c1c1159e76d03431b2c612d378a62fc914f0817df3f9a8092adddb589ac74e53
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7203227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54acd9cf4794435761c0462aba37d41e69e9581a77daeef4d16255b6a579f2c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Sat, 16 May 2020 09:47:11 GMT
ENV NATS_SERVER=2.1.7
# Wed, 29 Jul 2020 23:25:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a08d7ce0399df8701d3e3cd4c36744180c3a566cdb38efeccc12a364f0083705' ;; 		armhf) natsArch='arm6'; sha256='987c23f758842fb09c0d4500f632c5302aedc61d218f03998444b94074aabddb' ;; 		armv7) natsArch='arm7'; sha256='077fd1647aa25865ade5acc3d6ee5f542d2c62feb2fb41ec6d1dd83294bea05e' ;; 		x86_64) natsArch='amd64'; sha256='23cce53fe7f628f203dbbeadf434c3480d094690aba6ff0b1d374b8f2f9ffd8c' ;; 		x86) natsArch='386'; sha256='64e271690782af823930c95574db0f701d06a36ff42b9272c04841d4611bcd15' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:25:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 29 Jul 2020 23:25:41 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Jul 2020 23:25:42 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 23:25:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:25:42 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09eebfe9509bcbfcefadbc17c68fa103be7b7cf978f08ea01527a6aba38c5554`  
		Last Modified: Wed, 29 Jul 2020 23:26:16 GMT  
		Size: 4.4 MB (4388967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab62a5d69bc21353fa665e0b7fbf8e6a4a5d3fda0e87d58c02073999f76ff43f`  
		Last Modified: Wed, 29 Jul 2020 23:26:15 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a297d716cd17565b8a6331222fe5c2bcf967f50c6e424f62a5051e864941e2`  
		Last Modified: Wed, 29 Jul 2020 23:26:15 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-alpine3.11` - linux; arm variant v6

```console
$ docker pull nats@sha256:fee67afb8a9c6c38c60a5b90f51b6a6dfdb607b13d04240cf4faae9f8235d69d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6717777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb5af24d85d20ca2ddf1a257d6667c94e32ad6c1f381964f6ea48833ebc6eb39`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Fri, 15 May 2020 19:50:13 GMT
ENV NATS_SERVER=2.1.7
# Wed, 29 Jul 2020 23:02:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a08d7ce0399df8701d3e3cd4c36744180c3a566cdb38efeccc12a364f0083705' ;; 		armhf) natsArch='arm6'; sha256='987c23f758842fb09c0d4500f632c5302aedc61d218f03998444b94074aabddb' ;; 		armv7) natsArch='arm7'; sha256='077fd1647aa25865ade5acc3d6ee5f542d2c62feb2fb41ec6d1dd83294bea05e' ;; 		x86_64) natsArch='amd64'; sha256='23cce53fe7f628f203dbbeadf434c3480d094690aba6ff0b1d374b8f2f9ffd8c' ;; 		x86) natsArch='386'; sha256='64e271690782af823930c95574db0f701d06a36ff42b9272c04841d4611bcd15' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:02:35 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 29 Jul 2020 23:02:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Jul 2020 23:02:36 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 23:02:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:02:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0546a69fc010fc7d9fdae3cd6ff1eb8d7d7471a3561d782f6bb2bebcb079ad`  
		Last Modified: Wed, 29 Jul 2020 23:03:02 GMT  
		Size: 4.1 MB (4096870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02dc6927e9f4f4d185c4420481f8b1e06d55f058ad32ac4c0a9fc2ca3c2e0e64`  
		Last Modified: Wed, 29 Jul 2020 23:03:01 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6963e293037e1e7ddf702b89cf5a9441918b610e877f1710001b055560f92901`  
		Last Modified: Wed, 29 Jul 2020 23:03:01 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-alpine3.11` - linux; arm variant v7

```console
$ docker pull nats@sha256:197a92e111811ad767369a9bd75175ecb906fa57009400e78fa5d07ff8b0b47d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6515331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4546538a81c298be13378de43d24f5778e46917a8c2e6feca95287f8695e7d82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Sat, 16 May 2020 04:17:01 GMT
ENV NATS_SERVER=2.1.7
# Wed, 29 Jul 2020 23:11:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a08d7ce0399df8701d3e3cd4c36744180c3a566cdb38efeccc12a364f0083705' ;; 		armhf) natsArch='arm6'; sha256='987c23f758842fb09c0d4500f632c5302aedc61d218f03998444b94074aabddb' ;; 		armv7) natsArch='arm7'; sha256='077fd1647aa25865ade5acc3d6ee5f542d2c62feb2fb41ec6d1dd83294bea05e' ;; 		x86_64) natsArch='amd64'; sha256='23cce53fe7f628f203dbbeadf434c3480d094690aba6ff0b1d374b8f2f9ffd8c' ;; 		x86) natsArch='386'; sha256='64e271690782af823930c95574db0f701d06a36ff42b9272c04841d4611bcd15' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:11:46 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 29 Jul 2020 23:11:46 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Jul 2020 23:11:47 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 23:11:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:11:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4572ecf34c0bc5aa1ca0925f8f3c17e07cdf857ae8e31be72e5360711b24016`  
		Last Modified: Wed, 29 Jul 2020 23:15:57 GMT  
		Size: 4.1 MB (4092296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67632d2c07c7d161703500f1b0fa040775c8cb0c4474b8749a8ea961b5964f7e`  
		Last Modified: Wed, 29 Jul 2020 23:15:56 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5f50a8c5ae0937cd72ab745aacf65d53e62fed9a22d0de4fb3fe2f3d88a9b6`  
		Last Modified: Wed, 29 Jul 2020 23:15:56 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-alpine3.11` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:e3338a58db906f99cb91860cf607e3670e8b6676026d2eb70d26100b26bfcd5f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6803458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e79bcc07d57e06d12e6ae92a95f16c0dfe72401e9efdc3a3869273d02110feda`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Jul 2020 16:28:21 GMT
ENV NATS_SERVER=2.1.7
# Wed, 29 Jul 2020 22:41:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a08d7ce0399df8701d3e3cd4c36744180c3a566cdb38efeccc12a364f0083705' ;; 		armhf) natsArch='arm6'; sha256='987c23f758842fb09c0d4500f632c5302aedc61d218f03998444b94074aabddb' ;; 		armv7) natsArch='arm7'; sha256='077fd1647aa25865ade5acc3d6ee5f542d2c62feb2fb41ec6d1dd83294bea05e' ;; 		x86_64) natsArch='amd64'; sha256='23cce53fe7f628f203dbbeadf434c3480d094690aba6ff0b1d374b8f2f9ffd8c' ;; 		x86) natsArch='386'; sha256='64e271690782af823930c95574db0f701d06a36ff42b9272c04841d4611bcd15' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 22:41:30 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 29 Jul 2020 22:41:30 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Jul 2020 22:41:31 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 22:41:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 22:41:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e23520311eff0ccb9b4116bad00040e13d45013d01d87ee89bba20b01b5e536`  
		Last Modified: Wed, 29 Jul 2020 22:42:03 GMT  
		Size: 4.1 MB (4078060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5bd55073b3a781fd6af08f7e29facaf7e8d37e977fc7b8a7bcb57098c1dc49b`  
		Last Modified: Wed, 29 Jul 2020 22:42:02 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2eb0d8170b7670bd8ae9406d3cc6298a0cc3b8f3ec7434dd09ec858f8701183`  
		Last Modified: Wed, 29 Jul 2020 22:42:02 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-linux`

```console
$ docker pull nats@sha256:7a3219e049b4d8b10a7ff389fa689c8d08d5732fe37dcf9c5a72fda463d6c6ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.1-linux` - linux; amd64

```console
$ docker pull nats@sha256:6aace730d886f9719841c60ec11f826e494b8fcc631378b32f5e01ca32d87ab9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4087969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e93a56bc1852bb18d91f1741edde016c59b49c92f7ad91960d583ee0486ebf3`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 16 May 2020 09:47:58 GMT
COPY file:27ab63fb5115ca3cb7456a256d6d6dab7ba864d8806821652fbe569f4f845df5 in /nats-server 
# Sat, 16 May 2020 09:47:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 16 May 2020 09:47:59 GMT
EXPOSE 4222 6222 8222
# Sat, 16 May 2020 09:47:59 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 16 May 2020 09:47:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b509577c042697add820579de13ceed535b1c02ec7fa460b892d6c63941390a7`  
		Last Modified: Sat, 16 May 2020 09:48:21 GMT  
		Size: 4.1 MB (4087491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ce65065eb7bc6684476be5937b3d0d4046e7cc7241bc5017d70488d0edbfe3`  
		Last Modified: Sat, 16 May 2020 09:48:20 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:e8b59aabb2b6838ced59a3125ba4216cc8a4d0622f8b8c1e9e40fb30cd63a135
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3796375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8116ee7998ff454ed4eaa153438504925828993f56f26fb96fd11b31c9dc2128`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 15 May 2020 19:53:42 GMT
COPY file:9951c1b4ae20021f4d6efd6c039d0f0d0044470572e81beae625f15ffa13d2f1 in /nats-server 
# Fri, 15 May 2020 19:53:43 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 15 May 2020 19:53:44 GMT
EXPOSE 4222 6222 8222
# Fri, 15 May 2020 19:53:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 15 May 2020 19:53:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7976dc3d59fddf78c4ca25d0692135431e63b9fb744ae2c3d02b7a8214b5bfd9`  
		Last Modified: Fri, 15 May 2020 19:54:21 GMT  
		Size: 3.8 MB (3795898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b520f7415a5fab1b4a83eb7a8259e321475f75f5b06bfe95493b598c9ee9f4`  
		Last Modified: Fri, 15 May 2020 19:54:20 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:707f02b7c81a3f071abba9ce0a74b1cf0bf7a664e0220ab6cae112f2721a24bf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3792273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d2f2220669ef3621c45d5e4fd8460e7378e258044eb57003584ce55db5bdd9b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 16 May 2020 04:26:09 GMT
COPY file:3320edcd8f0db9551469809c752244493d1c6cf3be0287714c8a507e339283b2 in /nats-server 
# Sat, 16 May 2020 04:26:09 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 16 May 2020 04:26:11 GMT
EXPOSE 4222 6222 8222
# Sat, 16 May 2020 04:26:12 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 16 May 2020 04:26:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7ceefb66163b74f9719728ecace35bd406e85998a252d90c9e07a02582c7b6f1`  
		Last Modified: Sat, 16 May 2020 04:26:55 GMT  
		Size: 3.8 MB (3791795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db182fe235e1ef3b80de633e39d8ab9040cef44127adee97dbc4513df27dacfe`  
		Last Modified: Sat, 16 May 2020 04:26:53 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8cb2b90d45f90f3bdfb841b4a1399ff3a1b0a835e54664ee375ef309ff4c4398
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3776968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fffbb615827376dda1ad45bce22763d7cdc858675e4eafc55deb2d134f813338`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 29 Jul 2020 22:41:42 GMT
COPY file:67a03d7df05756de9c16c4cd22dfaf6ed9cc9a43b78a90ebfaa81ee7ebbc7abf in /nats-server 
# Wed, 29 Jul 2020 22:41:43 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 29 Jul 2020 22:41:44 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 22:41:44 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 29 Jul 2020 22:41:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:39a183ba93759b5fab08b0cb81f1f1a4c9f5a95c3746b031082c6bc3a57441b3`  
		Last Modified: Wed, 29 Jul 2020 22:42:18 GMT  
		Size: 3.8 MB (3776492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a510a0d87b5b915212ee2a5e5d877dced1c30164c0e82d6e60951d00374fe7`  
		Last Modified: Wed, 29 Jul 2020 22:42:17 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-nanoserver`

```console
$ docker pull nats@sha256:d3e9d8a5a0ad31f0845175c1071e35cea4ac4ebb849c16526e0664a3c0918608
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `nats:2.1-nanoserver` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats@sha256:00f69dcad2cdf6b3da43ef4701091ca04d3f35b2ec80c666554d49e5684258d8
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (104957159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edebc41e62feb1ccc604f2e015421dd2e938344719a06d92981822566271a91b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Jul 2020 13:50:07 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jul 2020 15:05:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 15:05:16 GMT
RUN cmd /S /C #(nop) COPY file:18561b827240029ad80d0e3d25142efae62905c30cc520fc37cfc68e7d889848 in C:\nats-server.exe 
# Wed, 15 Jul 2020 15:05:18 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jul 2020 15:05:18 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Jul 2020 15:05:19 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jul 2020 15:05:20 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:dc95608099543221ef539391bfece5c1ce37b97af9da457f5990349cab028a12`  
		Size: 100.9 MB (100895619 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5f0c27d781c53928c03429d5b34e0f49fc26b7e7c996c1d9a2a8474162eade60`  
		Last Modified: Wed, 15 Jul 2020 15:09:50 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10a270f5d0666930958ddfeac073712f678d77b5a05a08210012ada454204077`  
		Last Modified: Wed, 15 Jul 2020 15:10:00 GMT  
		Size: 4.1 MB (4056451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b5e48167a563124481e83cd3f3e3ca1bd3ea8f52b9e52dc9b4982e98a21d7d`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 1.5 KB (1470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64aecdf43c40f563833e5ad1c027bb2e67c1b0c51bb2ab795b99df1f4c2f26f`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 930.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:accd609b6f7304740da44e2a7331717a73ec3f94a35c25198a189b81bd84e204`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 928.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84a11ddf5d09a44b078d904b91df1cd82bf2a0cefb6ec9f52761f36fcf23f54`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-nanoserver-1809`

```console
$ docker pull nats@sha256:d3e9d8a5a0ad31f0845175c1071e35cea4ac4ebb849c16526e0664a3c0918608
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `nats:2.1-nanoserver-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats@sha256:00f69dcad2cdf6b3da43ef4701091ca04d3f35b2ec80c666554d49e5684258d8
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (104957159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edebc41e62feb1ccc604f2e015421dd2e938344719a06d92981822566271a91b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Jul 2020 13:50:07 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jul 2020 15:05:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 15:05:16 GMT
RUN cmd /S /C #(nop) COPY file:18561b827240029ad80d0e3d25142efae62905c30cc520fc37cfc68e7d889848 in C:\nats-server.exe 
# Wed, 15 Jul 2020 15:05:18 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jul 2020 15:05:18 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Jul 2020 15:05:19 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jul 2020 15:05:20 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:dc95608099543221ef539391bfece5c1ce37b97af9da457f5990349cab028a12`  
		Size: 100.9 MB (100895619 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5f0c27d781c53928c03429d5b34e0f49fc26b7e7c996c1d9a2a8474162eade60`  
		Last Modified: Wed, 15 Jul 2020 15:09:50 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10a270f5d0666930958ddfeac073712f678d77b5a05a08210012ada454204077`  
		Last Modified: Wed, 15 Jul 2020 15:10:00 GMT  
		Size: 4.1 MB (4056451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b5e48167a563124481e83cd3f3e3ca1bd3ea8f52b9e52dc9b4982e98a21d7d`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 1.5 KB (1470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64aecdf43c40f563833e5ad1c027bb2e67c1b0c51bb2ab795b99df1f4c2f26f`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 930.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:accd609b6f7304740da44e2a7331717a73ec3f94a35c25198a189b81bd84e204`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 928.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84a11ddf5d09a44b078d904b91df1cd82bf2a0cefb6ec9f52761f36fcf23f54`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-scratch`

```console
$ docker pull nats@sha256:7a3219e049b4d8b10a7ff389fa689c8d08d5732fe37dcf9c5a72fda463d6c6ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.1-scratch` - linux; amd64

```console
$ docker pull nats@sha256:6aace730d886f9719841c60ec11f826e494b8fcc631378b32f5e01ca32d87ab9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4087969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e93a56bc1852bb18d91f1741edde016c59b49c92f7ad91960d583ee0486ebf3`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 16 May 2020 09:47:58 GMT
COPY file:27ab63fb5115ca3cb7456a256d6d6dab7ba864d8806821652fbe569f4f845df5 in /nats-server 
# Sat, 16 May 2020 09:47:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 16 May 2020 09:47:59 GMT
EXPOSE 4222 6222 8222
# Sat, 16 May 2020 09:47:59 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 16 May 2020 09:47:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b509577c042697add820579de13ceed535b1c02ec7fa460b892d6c63941390a7`  
		Last Modified: Sat, 16 May 2020 09:48:21 GMT  
		Size: 4.1 MB (4087491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ce65065eb7bc6684476be5937b3d0d4046e7cc7241bc5017d70488d0edbfe3`  
		Last Modified: Sat, 16 May 2020 09:48:20 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:e8b59aabb2b6838ced59a3125ba4216cc8a4d0622f8b8c1e9e40fb30cd63a135
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3796375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8116ee7998ff454ed4eaa153438504925828993f56f26fb96fd11b31c9dc2128`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 15 May 2020 19:53:42 GMT
COPY file:9951c1b4ae20021f4d6efd6c039d0f0d0044470572e81beae625f15ffa13d2f1 in /nats-server 
# Fri, 15 May 2020 19:53:43 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 15 May 2020 19:53:44 GMT
EXPOSE 4222 6222 8222
# Fri, 15 May 2020 19:53:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 15 May 2020 19:53:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7976dc3d59fddf78c4ca25d0692135431e63b9fb744ae2c3d02b7a8214b5bfd9`  
		Last Modified: Fri, 15 May 2020 19:54:21 GMT  
		Size: 3.8 MB (3795898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b520f7415a5fab1b4a83eb7a8259e321475f75f5b06bfe95493b598c9ee9f4`  
		Last Modified: Fri, 15 May 2020 19:54:20 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:707f02b7c81a3f071abba9ce0a74b1cf0bf7a664e0220ab6cae112f2721a24bf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3792273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d2f2220669ef3621c45d5e4fd8460e7378e258044eb57003584ce55db5bdd9b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 16 May 2020 04:26:09 GMT
COPY file:3320edcd8f0db9551469809c752244493d1c6cf3be0287714c8a507e339283b2 in /nats-server 
# Sat, 16 May 2020 04:26:09 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 16 May 2020 04:26:11 GMT
EXPOSE 4222 6222 8222
# Sat, 16 May 2020 04:26:12 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 16 May 2020 04:26:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7ceefb66163b74f9719728ecace35bd406e85998a252d90c9e07a02582c7b6f1`  
		Last Modified: Sat, 16 May 2020 04:26:55 GMT  
		Size: 3.8 MB (3791795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db182fe235e1ef3b80de633e39d8ab9040cef44127adee97dbc4513df27dacfe`  
		Last Modified: Sat, 16 May 2020 04:26:53 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8cb2b90d45f90f3bdfb841b4a1399ff3a1b0a835e54664ee375ef309ff4c4398
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3776968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fffbb615827376dda1ad45bce22763d7cdc858675e4eafc55deb2d134f813338`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 29 Jul 2020 22:41:42 GMT
COPY file:67a03d7df05756de9c16c4cd22dfaf6ed9cc9a43b78a90ebfaa81ee7ebbc7abf in /nats-server 
# Wed, 29 Jul 2020 22:41:43 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 29 Jul 2020 22:41:44 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 22:41:44 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 29 Jul 2020 22:41:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:39a183ba93759b5fab08b0cb81f1f1a4c9f5a95c3746b031082c6bc3a57441b3`  
		Last Modified: Wed, 29 Jul 2020 22:42:18 GMT  
		Size: 3.8 MB (3776492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a510a0d87b5b915212ee2a5e5d877dced1c30164c0e82d6e60951d00374fe7`  
		Last Modified: Wed, 29 Jul 2020 22:42:17 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-windowsservercore`

```console
$ docker pull nats@sha256:59a9a5745643d652dd6d49be5d422a2270a2539f6dfa398ba219d78c00c701e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64
	-	windows version 10.0.14393.3808; amd64

### `nats:2.1-windowsservercore` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats@sha256:84ed3b1eb1e35102dff57509d666e9ae99f4fd0a492b9410b473bedda4aeebdf
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2328185203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8d69d5e23b4cff9ad8df708d4059e6525b91686ad490775e104e6c06b863457`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Wed, 15 Jul 2020 12:15:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jul 2020 15:03:03 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 15:03:03 GMT
ENV NATS_SERVER=2.1.7
# Wed, 15 Jul 2020 15:03:04 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.7/nats-server-v2.1.7-windows-amd64.zip
# Wed, 29 Jul 2020 23:14:26 GMT
ENV GIT_DOWNLOAD_SHA256=1e1ad5c00929cc145341fd65f8b0a41a38e942b9b9fd9fdb0216c47654afdc8f
# Wed, 29 Jul 2020 23:15:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 29 Jul 2020 23:16:49 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 29 Jul 2020 23:16:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 29 Jul 2020 23:16:54 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 23:16:55 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 29 Jul 2020 23:16:56 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1cc883a0e3509a474bb32f3c40411bf86219325ae9710e25a5dcce6b44eef357`  
		Last Modified: Wed, 15 Jul 2020 14:32:06 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dd35c9a62007b6ded1ca968562be97de62ea3e2b3c7db85f4a50baaa9efecb`  
		Last Modified: Wed, 15 Jul 2020 15:09:33 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5789d32300712f2fa8b6564efe911f5f523cf150f1fde2bf8d6deedbb56feb4`  
		Last Modified: Wed, 15 Jul 2020 15:09:32 GMT  
		Size: 1.1 KB (1105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b62b1740ff37517c10b8b8bfae73367d0c5538cf934392846eea648031c1857`  
		Last Modified: Wed, 15 Jul 2020 15:09:31 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c765e0c4aba82f5140dd325bb9fc2dc97095f673b4d88039867aecc92e331f5e`  
		Last Modified: Wed, 29 Jul 2020 23:21:23 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9dfd44060c9c9e79fca23ba4227434b55a5a3353c7a32ba8140fa252af2631f`  
		Last Modified: Wed, 29 Jul 2020 23:21:24 GMT  
		Size: 4.8 MB (4803853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011be3335c53769b99af80accd8e25f40172d44bc0e20780c88f1ab787bbf09e`  
		Last Modified: Wed, 29 Jul 2020 23:21:24 GMT  
		Size: 13.2 MB (13178319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f913f5767f1c088f27134bdefc531acacd106610ce085ef7ca5470fdeda55e80`  
		Last Modified: Wed, 29 Jul 2020 23:21:20 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8436f3f54d22f495452cdb61489bf5833c2cda6a2e6012c732b2c8ffbc72262f`  
		Last Modified: Wed, 29 Jul 2020 23:21:20 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12724c1ab2196db2d2cd8bff6069b1ea932e514cd5473240dd515f50361e4fa`  
		Last Modified: Wed, 29 Jul 2020 23:21:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419a5e47094ff5e8a8cb733bf81fcd97e46b00a5b62b9cbcd5993a66942a7e7e`  
		Last Modified: Wed, 29 Jul 2020 23:21:20 GMT  
		Size: 1.1 KB (1100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-windowsservercore` - windows version 10.0.14393.3808; amd64

```console
$ docker pull nats@sha256:9145e80ebf209b601e34e199defd755bf43a5b09f674ece13c4c6299b21d4870
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5756757168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a3c13889118f6f6c65e859be772b7b0cb7e0497de0a2326a3b54c097daa6670`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Jul 2020 21:05:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Jul 2020 12:24:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jul 2020 15:05:26 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 15:05:27 GMT
ENV NATS_SERVER=2.1.7
# Wed, 15 Jul 2020 15:05:28 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.7/nats-server-v2.1.7-windows-amd64.zip
# Wed, 29 Jul 2020 23:17:15 GMT
ENV GIT_DOWNLOAD_SHA256=1e1ad5c00929cc145341fd65f8b0a41a38e942b9b9fd9fdb0216c47654afdc8f
# Wed, 29 Jul 2020 23:18:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 29 Jul 2020 23:20:43 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 29 Jul 2020 23:20:45 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 29 Jul 2020 23:20:46 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 23:20:47 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 29 Jul 2020 23:20:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:802c4beb8b091968ccf1bb4a853ded7955ddb79e6f8775a5155cb5ed07dcbcab`  
		Size: 1.7 GB (1667476199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3393eecaf56a66035ab178b379bacf81d30373b630b34b2973501f259aadb0f6`  
		Last Modified: Wed, 15 Jul 2020 14:32:38 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1430ee68db5fe3026683f1b7c74f31ae748da71bf8ad611efede726e9e036b1`  
		Last Modified: Wed, 15 Jul 2020 15:10:21 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae29b1720308eb8710d921cefbc8979061e4535b6276b35b3d471e08a09e7af`  
		Last Modified: Wed, 15 Jul 2020 15:10:19 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a76213345cac0ca18badbc3c8262b6973e3457484fdcb9af380fa4de2c64ea`  
		Last Modified: Wed, 15 Jul 2020 15:10:19 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2713fe8ba40241bc8ef85e6795703e42f101f0ab81d143357c549a03c4b00c`  
		Last Modified: Wed, 29 Jul 2020 23:21:44 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b8f23b09829f938cc622501d4059590b050bc95a7fb4c5d2e337e423af1e23`  
		Last Modified: Wed, 29 Jul 2020 23:21:46 GMT  
		Size: 5.4 MB (5391705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0857d1594c42a8ff34ec0fc99b717f343d2e6dcdcb980e3b54621a8127ecf4a`  
		Last Modified: Wed, 29 Jul 2020 23:21:57 GMT  
		Size: 13.9 MB (13892511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7afe295ad113f1145078cde44f86ce197d64aa5ceb92784bf4c60ff710b95256`  
		Last Modified: Wed, 29 Jul 2020 23:21:41 GMT  
		Size: 1.7 KB (1683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9b54006dba8cc76bc2325f78d0377969e727070a8f9069e26090b7a4e18f36`  
		Last Modified: Wed, 29 Jul 2020 23:21:41 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97bb5b91db82c40b2b26f5fcc7a1e07fce677242cd70722fbe2d3256e4548dfc`  
		Last Modified: Wed, 29 Jul 2020 23:21:42 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58919d245b3713c0a29f1039075f368c82d09514f57a595cade8fae1010c7847`  
		Last Modified: Wed, 29 Jul 2020 23:21:42 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-windowsservercore-1809`

```console
$ docker pull nats@sha256:f9351e549406b5be23d79a960a8188aae30b521a25b98855bcf4ad382d0446e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `nats:2.1-windowsservercore-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats@sha256:84ed3b1eb1e35102dff57509d666e9ae99f4fd0a492b9410b473bedda4aeebdf
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2328185203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8d69d5e23b4cff9ad8df708d4059e6525b91686ad490775e104e6c06b863457`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Wed, 15 Jul 2020 12:15:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jul 2020 15:03:03 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 15:03:03 GMT
ENV NATS_SERVER=2.1.7
# Wed, 15 Jul 2020 15:03:04 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.7/nats-server-v2.1.7-windows-amd64.zip
# Wed, 29 Jul 2020 23:14:26 GMT
ENV GIT_DOWNLOAD_SHA256=1e1ad5c00929cc145341fd65f8b0a41a38e942b9b9fd9fdb0216c47654afdc8f
# Wed, 29 Jul 2020 23:15:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 29 Jul 2020 23:16:49 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 29 Jul 2020 23:16:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 29 Jul 2020 23:16:54 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 23:16:55 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 29 Jul 2020 23:16:56 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1cc883a0e3509a474bb32f3c40411bf86219325ae9710e25a5dcce6b44eef357`  
		Last Modified: Wed, 15 Jul 2020 14:32:06 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dd35c9a62007b6ded1ca968562be97de62ea3e2b3c7db85f4a50baaa9efecb`  
		Last Modified: Wed, 15 Jul 2020 15:09:33 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5789d32300712f2fa8b6564efe911f5f523cf150f1fde2bf8d6deedbb56feb4`  
		Last Modified: Wed, 15 Jul 2020 15:09:32 GMT  
		Size: 1.1 KB (1105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b62b1740ff37517c10b8b8bfae73367d0c5538cf934392846eea648031c1857`  
		Last Modified: Wed, 15 Jul 2020 15:09:31 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c765e0c4aba82f5140dd325bb9fc2dc97095f673b4d88039867aecc92e331f5e`  
		Last Modified: Wed, 29 Jul 2020 23:21:23 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9dfd44060c9c9e79fca23ba4227434b55a5a3353c7a32ba8140fa252af2631f`  
		Last Modified: Wed, 29 Jul 2020 23:21:24 GMT  
		Size: 4.8 MB (4803853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011be3335c53769b99af80accd8e25f40172d44bc0e20780c88f1ab787bbf09e`  
		Last Modified: Wed, 29 Jul 2020 23:21:24 GMT  
		Size: 13.2 MB (13178319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f913f5767f1c088f27134bdefc531acacd106610ce085ef7ca5470fdeda55e80`  
		Last Modified: Wed, 29 Jul 2020 23:21:20 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8436f3f54d22f495452cdb61489bf5833c2cda6a2e6012c732b2c8ffbc72262f`  
		Last Modified: Wed, 29 Jul 2020 23:21:20 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12724c1ab2196db2d2cd8bff6069b1ea932e514cd5473240dd515f50361e4fa`  
		Last Modified: Wed, 29 Jul 2020 23:21:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419a5e47094ff5e8a8cb733bf81fcd97e46b00a5b62b9cbcd5993a66942a7e7e`  
		Last Modified: Wed, 29 Jul 2020 23:21:20 GMT  
		Size: 1.1 KB (1100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:f405d1c17c29cd33ba2762684ab3ee983dbaafd8df62ef7b12fa78b3ad6b7d3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3808; amd64

### `nats:2.1-windowsservercore-ltsc2016` - windows version 10.0.14393.3808; amd64

```console
$ docker pull nats@sha256:9145e80ebf209b601e34e199defd755bf43a5b09f674ece13c4c6299b21d4870
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5756757168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a3c13889118f6f6c65e859be772b7b0cb7e0497de0a2326a3b54c097daa6670`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Jul 2020 21:05:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Jul 2020 12:24:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jul 2020 15:05:26 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 15:05:27 GMT
ENV NATS_SERVER=2.1.7
# Wed, 15 Jul 2020 15:05:28 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.7/nats-server-v2.1.7-windows-amd64.zip
# Wed, 29 Jul 2020 23:17:15 GMT
ENV GIT_DOWNLOAD_SHA256=1e1ad5c00929cc145341fd65f8b0a41a38e942b9b9fd9fdb0216c47654afdc8f
# Wed, 29 Jul 2020 23:18:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 29 Jul 2020 23:20:43 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 29 Jul 2020 23:20:45 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 29 Jul 2020 23:20:46 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 23:20:47 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 29 Jul 2020 23:20:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:802c4beb8b091968ccf1bb4a853ded7955ddb79e6f8775a5155cb5ed07dcbcab`  
		Size: 1.7 GB (1667476199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3393eecaf56a66035ab178b379bacf81d30373b630b34b2973501f259aadb0f6`  
		Last Modified: Wed, 15 Jul 2020 14:32:38 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1430ee68db5fe3026683f1b7c74f31ae748da71bf8ad611efede726e9e036b1`  
		Last Modified: Wed, 15 Jul 2020 15:10:21 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae29b1720308eb8710d921cefbc8979061e4535b6276b35b3d471e08a09e7af`  
		Last Modified: Wed, 15 Jul 2020 15:10:19 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a76213345cac0ca18badbc3c8262b6973e3457484fdcb9af380fa4de2c64ea`  
		Last Modified: Wed, 15 Jul 2020 15:10:19 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2713fe8ba40241bc8ef85e6795703e42f101f0ab81d143357c549a03c4b00c`  
		Last Modified: Wed, 29 Jul 2020 23:21:44 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b8f23b09829f938cc622501d4059590b050bc95a7fb4c5d2e337e423af1e23`  
		Last Modified: Wed, 29 Jul 2020 23:21:46 GMT  
		Size: 5.4 MB (5391705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0857d1594c42a8ff34ec0fc99b717f343d2e6dcdcb980e3b54621a8127ecf4a`  
		Last Modified: Wed, 29 Jul 2020 23:21:57 GMT  
		Size: 13.9 MB (13892511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7afe295ad113f1145078cde44f86ce197d64aa5ceb92784bf4c60ff710b95256`  
		Last Modified: Wed, 29 Jul 2020 23:21:41 GMT  
		Size: 1.7 KB (1683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9b54006dba8cc76bc2325f78d0377969e727070a8f9069e26090b7a4e18f36`  
		Last Modified: Wed, 29 Jul 2020 23:21:41 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97bb5b91db82c40b2b26f5fcc7a1e07fce677242cd70722fbe2d3256e4548dfc`  
		Last Modified: Wed, 29 Jul 2020 23:21:42 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58919d245b3713c0a29f1039075f368c82d09514f57a595cade8fae1010c7847`  
		Last Modified: Wed, 29 Jul 2020 23:21:42 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:2ca671f95f6f5c4d9144a701d8b7be77a1830041d86766e2e193fb58b00af449
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:c1c1159e76d03431b2c612d378a62fc914f0817df3f9a8092adddb589ac74e53
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7203227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54acd9cf4794435761c0462aba37d41e69e9581a77daeef4d16255b6a579f2c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Sat, 16 May 2020 09:47:11 GMT
ENV NATS_SERVER=2.1.7
# Wed, 29 Jul 2020 23:25:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a08d7ce0399df8701d3e3cd4c36744180c3a566cdb38efeccc12a364f0083705' ;; 		armhf) natsArch='arm6'; sha256='987c23f758842fb09c0d4500f632c5302aedc61d218f03998444b94074aabddb' ;; 		armv7) natsArch='arm7'; sha256='077fd1647aa25865ade5acc3d6ee5f542d2c62feb2fb41ec6d1dd83294bea05e' ;; 		x86_64) natsArch='amd64'; sha256='23cce53fe7f628f203dbbeadf434c3480d094690aba6ff0b1d374b8f2f9ffd8c' ;; 		x86) natsArch='386'; sha256='64e271690782af823930c95574db0f701d06a36ff42b9272c04841d4611bcd15' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:25:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 29 Jul 2020 23:25:41 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Jul 2020 23:25:42 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 23:25:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:25:42 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09eebfe9509bcbfcefadbc17c68fa103be7b7cf978f08ea01527a6aba38c5554`  
		Last Modified: Wed, 29 Jul 2020 23:26:16 GMT  
		Size: 4.4 MB (4388967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab62a5d69bc21353fa665e0b7fbf8e6a4a5d3fda0e87d58c02073999f76ff43f`  
		Last Modified: Wed, 29 Jul 2020 23:26:15 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a297d716cd17565b8a6331222fe5c2bcf967f50c6e424f62a5051e864941e2`  
		Last Modified: Wed, 29 Jul 2020 23:26:15 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:fee67afb8a9c6c38c60a5b90f51b6a6dfdb607b13d04240cf4faae9f8235d69d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6717777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb5af24d85d20ca2ddf1a257d6667c94e32ad6c1f381964f6ea48833ebc6eb39`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Fri, 15 May 2020 19:50:13 GMT
ENV NATS_SERVER=2.1.7
# Wed, 29 Jul 2020 23:02:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a08d7ce0399df8701d3e3cd4c36744180c3a566cdb38efeccc12a364f0083705' ;; 		armhf) natsArch='arm6'; sha256='987c23f758842fb09c0d4500f632c5302aedc61d218f03998444b94074aabddb' ;; 		armv7) natsArch='arm7'; sha256='077fd1647aa25865ade5acc3d6ee5f542d2c62feb2fb41ec6d1dd83294bea05e' ;; 		x86_64) natsArch='amd64'; sha256='23cce53fe7f628f203dbbeadf434c3480d094690aba6ff0b1d374b8f2f9ffd8c' ;; 		x86) natsArch='386'; sha256='64e271690782af823930c95574db0f701d06a36ff42b9272c04841d4611bcd15' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:02:35 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 29 Jul 2020 23:02:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Jul 2020 23:02:36 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 23:02:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:02:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0546a69fc010fc7d9fdae3cd6ff1eb8d7d7471a3561d782f6bb2bebcb079ad`  
		Last Modified: Wed, 29 Jul 2020 23:03:02 GMT  
		Size: 4.1 MB (4096870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02dc6927e9f4f4d185c4420481f8b1e06d55f058ad32ac4c0a9fc2ca3c2e0e64`  
		Last Modified: Wed, 29 Jul 2020 23:03:01 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6963e293037e1e7ddf702b89cf5a9441918b610e877f1710001b055560f92901`  
		Last Modified: Wed, 29 Jul 2020 23:03:01 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:197a92e111811ad767369a9bd75175ecb906fa57009400e78fa5d07ff8b0b47d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6515331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4546538a81c298be13378de43d24f5778e46917a8c2e6feca95287f8695e7d82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Sat, 16 May 2020 04:17:01 GMT
ENV NATS_SERVER=2.1.7
# Wed, 29 Jul 2020 23:11:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a08d7ce0399df8701d3e3cd4c36744180c3a566cdb38efeccc12a364f0083705' ;; 		armhf) natsArch='arm6'; sha256='987c23f758842fb09c0d4500f632c5302aedc61d218f03998444b94074aabddb' ;; 		armv7) natsArch='arm7'; sha256='077fd1647aa25865ade5acc3d6ee5f542d2c62feb2fb41ec6d1dd83294bea05e' ;; 		x86_64) natsArch='amd64'; sha256='23cce53fe7f628f203dbbeadf434c3480d094690aba6ff0b1d374b8f2f9ffd8c' ;; 		x86) natsArch='386'; sha256='64e271690782af823930c95574db0f701d06a36ff42b9272c04841d4611bcd15' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:11:46 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 29 Jul 2020 23:11:46 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Jul 2020 23:11:47 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 23:11:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:11:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4572ecf34c0bc5aa1ca0925f8f3c17e07cdf857ae8e31be72e5360711b24016`  
		Last Modified: Wed, 29 Jul 2020 23:15:57 GMT  
		Size: 4.1 MB (4092296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67632d2c07c7d161703500f1b0fa040775c8cb0c4474b8749a8ea961b5964f7e`  
		Last Modified: Wed, 29 Jul 2020 23:15:56 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5f50a8c5ae0937cd72ab745aacf65d53e62fed9a22d0de4fb3fe2f3d88a9b6`  
		Last Modified: Wed, 29 Jul 2020 23:15:56 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:e3338a58db906f99cb91860cf607e3670e8b6676026d2eb70d26100b26bfcd5f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6803458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e79bcc07d57e06d12e6ae92a95f16c0dfe72401e9efdc3a3869273d02110feda`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Jul 2020 16:28:21 GMT
ENV NATS_SERVER=2.1.7
# Wed, 29 Jul 2020 22:41:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a08d7ce0399df8701d3e3cd4c36744180c3a566cdb38efeccc12a364f0083705' ;; 		armhf) natsArch='arm6'; sha256='987c23f758842fb09c0d4500f632c5302aedc61d218f03998444b94074aabddb' ;; 		armv7) natsArch='arm7'; sha256='077fd1647aa25865ade5acc3d6ee5f542d2c62feb2fb41ec6d1dd83294bea05e' ;; 		x86_64) natsArch='amd64'; sha256='23cce53fe7f628f203dbbeadf434c3480d094690aba6ff0b1d374b8f2f9ffd8c' ;; 		x86) natsArch='386'; sha256='64e271690782af823930c95574db0f701d06a36ff42b9272c04841d4611bcd15' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 22:41:30 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 29 Jul 2020 22:41:30 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Jul 2020 22:41:31 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 22:41:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 22:41:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e23520311eff0ccb9b4116bad00040e13d45013d01d87ee89bba20b01b5e536`  
		Last Modified: Wed, 29 Jul 2020 22:42:03 GMT  
		Size: 4.1 MB (4078060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5bd55073b3a781fd6af08f7e29facaf7e8d37e977fc7b8a7bcb57098c1dc49b`  
		Last Modified: Wed, 29 Jul 2020 22:42:02 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2eb0d8170b7670bd8ae9406d3cc6298a0cc3b8f3ec7434dd09ec858f8701183`  
		Last Modified: Wed, 29 Jul 2020 22:42:02 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.11`

```console
$ docker pull nats@sha256:2ca671f95f6f5c4d9144a701d8b7be77a1830041d86766e2e193fb58b00af449
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.11` - linux; amd64

```console
$ docker pull nats@sha256:c1c1159e76d03431b2c612d378a62fc914f0817df3f9a8092adddb589ac74e53
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7203227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54acd9cf4794435761c0462aba37d41e69e9581a77daeef4d16255b6a579f2c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Sat, 16 May 2020 09:47:11 GMT
ENV NATS_SERVER=2.1.7
# Wed, 29 Jul 2020 23:25:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a08d7ce0399df8701d3e3cd4c36744180c3a566cdb38efeccc12a364f0083705' ;; 		armhf) natsArch='arm6'; sha256='987c23f758842fb09c0d4500f632c5302aedc61d218f03998444b94074aabddb' ;; 		armv7) natsArch='arm7'; sha256='077fd1647aa25865ade5acc3d6ee5f542d2c62feb2fb41ec6d1dd83294bea05e' ;; 		x86_64) natsArch='amd64'; sha256='23cce53fe7f628f203dbbeadf434c3480d094690aba6ff0b1d374b8f2f9ffd8c' ;; 		x86) natsArch='386'; sha256='64e271690782af823930c95574db0f701d06a36ff42b9272c04841d4611bcd15' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:25:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 29 Jul 2020 23:25:41 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Jul 2020 23:25:42 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 23:25:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:25:42 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09eebfe9509bcbfcefadbc17c68fa103be7b7cf978f08ea01527a6aba38c5554`  
		Last Modified: Wed, 29 Jul 2020 23:26:16 GMT  
		Size: 4.4 MB (4388967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab62a5d69bc21353fa665e0b7fbf8e6a4a5d3fda0e87d58c02073999f76ff43f`  
		Last Modified: Wed, 29 Jul 2020 23:26:15 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a297d716cd17565b8a6331222fe5c2bcf967f50c6e424f62a5051e864941e2`  
		Last Modified: Wed, 29 Jul 2020 23:26:15 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.11` - linux; arm variant v6

```console
$ docker pull nats@sha256:fee67afb8a9c6c38c60a5b90f51b6a6dfdb607b13d04240cf4faae9f8235d69d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6717777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb5af24d85d20ca2ddf1a257d6667c94e32ad6c1f381964f6ea48833ebc6eb39`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Fri, 15 May 2020 19:50:13 GMT
ENV NATS_SERVER=2.1.7
# Wed, 29 Jul 2020 23:02:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a08d7ce0399df8701d3e3cd4c36744180c3a566cdb38efeccc12a364f0083705' ;; 		armhf) natsArch='arm6'; sha256='987c23f758842fb09c0d4500f632c5302aedc61d218f03998444b94074aabddb' ;; 		armv7) natsArch='arm7'; sha256='077fd1647aa25865ade5acc3d6ee5f542d2c62feb2fb41ec6d1dd83294bea05e' ;; 		x86_64) natsArch='amd64'; sha256='23cce53fe7f628f203dbbeadf434c3480d094690aba6ff0b1d374b8f2f9ffd8c' ;; 		x86) natsArch='386'; sha256='64e271690782af823930c95574db0f701d06a36ff42b9272c04841d4611bcd15' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:02:35 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 29 Jul 2020 23:02:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Jul 2020 23:02:36 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 23:02:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:02:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0546a69fc010fc7d9fdae3cd6ff1eb8d7d7471a3561d782f6bb2bebcb079ad`  
		Last Modified: Wed, 29 Jul 2020 23:03:02 GMT  
		Size: 4.1 MB (4096870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02dc6927e9f4f4d185c4420481f8b1e06d55f058ad32ac4c0a9fc2ca3c2e0e64`  
		Last Modified: Wed, 29 Jul 2020 23:03:01 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6963e293037e1e7ddf702b89cf5a9441918b610e877f1710001b055560f92901`  
		Last Modified: Wed, 29 Jul 2020 23:03:01 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.11` - linux; arm variant v7

```console
$ docker pull nats@sha256:197a92e111811ad767369a9bd75175ecb906fa57009400e78fa5d07ff8b0b47d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6515331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4546538a81c298be13378de43d24f5778e46917a8c2e6feca95287f8695e7d82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Sat, 16 May 2020 04:17:01 GMT
ENV NATS_SERVER=2.1.7
# Wed, 29 Jul 2020 23:11:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a08d7ce0399df8701d3e3cd4c36744180c3a566cdb38efeccc12a364f0083705' ;; 		armhf) natsArch='arm6'; sha256='987c23f758842fb09c0d4500f632c5302aedc61d218f03998444b94074aabddb' ;; 		armv7) natsArch='arm7'; sha256='077fd1647aa25865ade5acc3d6ee5f542d2c62feb2fb41ec6d1dd83294bea05e' ;; 		x86_64) natsArch='amd64'; sha256='23cce53fe7f628f203dbbeadf434c3480d094690aba6ff0b1d374b8f2f9ffd8c' ;; 		x86) natsArch='386'; sha256='64e271690782af823930c95574db0f701d06a36ff42b9272c04841d4611bcd15' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:11:46 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 29 Jul 2020 23:11:46 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Jul 2020 23:11:47 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 23:11:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:11:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4572ecf34c0bc5aa1ca0925f8f3c17e07cdf857ae8e31be72e5360711b24016`  
		Last Modified: Wed, 29 Jul 2020 23:15:57 GMT  
		Size: 4.1 MB (4092296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67632d2c07c7d161703500f1b0fa040775c8cb0c4474b8749a8ea961b5964f7e`  
		Last Modified: Wed, 29 Jul 2020 23:15:56 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5f50a8c5ae0937cd72ab745aacf65d53e62fed9a22d0de4fb3fe2f3d88a9b6`  
		Last Modified: Wed, 29 Jul 2020 23:15:56 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.11` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:e3338a58db906f99cb91860cf607e3670e8b6676026d2eb70d26100b26bfcd5f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6803458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e79bcc07d57e06d12e6ae92a95f16c0dfe72401e9efdc3a3869273d02110feda`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Jul 2020 16:28:21 GMT
ENV NATS_SERVER=2.1.7
# Wed, 29 Jul 2020 22:41:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a08d7ce0399df8701d3e3cd4c36744180c3a566cdb38efeccc12a364f0083705' ;; 		armhf) natsArch='arm6'; sha256='987c23f758842fb09c0d4500f632c5302aedc61d218f03998444b94074aabddb' ;; 		armv7) natsArch='arm7'; sha256='077fd1647aa25865ade5acc3d6ee5f542d2c62feb2fb41ec6d1dd83294bea05e' ;; 		x86_64) natsArch='amd64'; sha256='23cce53fe7f628f203dbbeadf434c3480d094690aba6ff0b1d374b8f2f9ffd8c' ;; 		x86) natsArch='386'; sha256='64e271690782af823930c95574db0f701d06a36ff42b9272c04841d4611bcd15' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 22:41:30 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 29 Jul 2020 22:41:30 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Jul 2020 22:41:31 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 22:41:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 22:41:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e23520311eff0ccb9b4116bad00040e13d45013d01d87ee89bba20b01b5e536`  
		Last Modified: Wed, 29 Jul 2020 22:42:03 GMT  
		Size: 4.1 MB (4078060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5bd55073b3a781fd6af08f7e29facaf7e8d37e977fc7b8a7bcb57098c1dc49b`  
		Last Modified: Wed, 29 Jul 2020 22:42:02 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2eb0d8170b7670bd8ae9406d3cc6298a0cc3b8f3ec7434dd09ec858f8701183`  
		Last Modified: Wed, 29 Jul 2020 22:42:02 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:7a3219e049b4d8b10a7ff389fa689c8d08d5732fe37dcf9c5a72fda463d6c6ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:6aace730d886f9719841c60ec11f826e494b8fcc631378b32f5e01ca32d87ab9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4087969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e93a56bc1852bb18d91f1741edde016c59b49c92f7ad91960d583ee0486ebf3`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 16 May 2020 09:47:58 GMT
COPY file:27ab63fb5115ca3cb7456a256d6d6dab7ba864d8806821652fbe569f4f845df5 in /nats-server 
# Sat, 16 May 2020 09:47:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 16 May 2020 09:47:59 GMT
EXPOSE 4222 6222 8222
# Sat, 16 May 2020 09:47:59 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 16 May 2020 09:47:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b509577c042697add820579de13ceed535b1c02ec7fa460b892d6c63941390a7`  
		Last Modified: Sat, 16 May 2020 09:48:21 GMT  
		Size: 4.1 MB (4087491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ce65065eb7bc6684476be5937b3d0d4046e7cc7241bc5017d70488d0edbfe3`  
		Last Modified: Sat, 16 May 2020 09:48:20 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:e8b59aabb2b6838ced59a3125ba4216cc8a4d0622f8b8c1e9e40fb30cd63a135
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3796375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8116ee7998ff454ed4eaa153438504925828993f56f26fb96fd11b31c9dc2128`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 15 May 2020 19:53:42 GMT
COPY file:9951c1b4ae20021f4d6efd6c039d0f0d0044470572e81beae625f15ffa13d2f1 in /nats-server 
# Fri, 15 May 2020 19:53:43 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 15 May 2020 19:53:44 GMT
EXPOSE 4222 6222 8222
# Fri, 15 May 2020 19:53:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 15 May 2020 19:53:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7976dc3d59fddf78c4ca25d0692135431e63b9fb744ae2c3d02b7a8214b5bfd9`  
		Last Modified: Fri, 15 May 2020 19:54:21 GMT  
		Size: 3.8 MB (3795898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b520f7415a5fab1b4a83eb7a8259e321475f75f5b06bfe95493b598c9ee9f4`  
		Last Modified: Fri, 15 May 2020 19:54:20 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:707f02b7c81a3f071abba9ce0a74b1cf0bf7a664e0220ab6cae112f2721a24bf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3792273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d2f2220669ef3621c45d5e4fd8460e7378e258044eb57003584ce55db5bdd9b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 16 May 2020 04:26:09 GMT
COPY file:3320edcd8f0db9551469809c752244493d1c6cf3be0287714c8a507e339283b2 in /nats-server 
# Sat, 16 May 2020 04:26:09 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 16 May 2020 04:26:11 GMT
EXPOSE 4222 6222 8222
# Sat, 16 May 2020 04:26:12 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 16 May 2020 04:26:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7ceefb66163b74f9719728ecace35bd406e85998a252d90c9e07a02582c7b6f1`  
		Last Modified: Sat, 16 May 2020 04:26:55 GMT  
		Size: 3.8 MB (3791795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db182fe235e1ef3b80de633e39d8ab9040cef44127adee97dbc4513df27dacfe`  
		Last Modified: Sat, 16 May 2020 04:26:53 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8cb2b90d45f90f3bdfb841b4a1399ff3a1b0a835e54664ee375ef309ff4c4398
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3776968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fffbb615827376dda1ad45bce22763d7cdc858675e4eafc55deb2d134f813338`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 29 Jul 2020 22:41:42 GMT
COPY file:67a03d7df05756de9c16c4cd22dfaf6ed9cc9a43b78a90ebfaa81ee7ebbc7abf in /nats-server 
# Wed, 29 Jul 2020 22:41:43 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 29 Jul 2020 22:41:44 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 22:41:44 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 29 Jul 2020 22:41:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:39a183ba93759b5fab08b0cb81f1f1a4c9f5a95c3746b031082c6bc3a57441b3`  
		Last Modified: Wed, 29 Jul 2020 22:42:18 GMT  
		Size: 3.8 MB (3776492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a510a0d87b5b915212ee2a5e5d877dced1c30164c0e82d6e60951d00374fe7`  
		Last Modified: Wed, 29 Jul 2020 22:42:17 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:d3e9d8a5a0ad31f0845175c1071e35cea4ac4ebb849c16526e0664a3c0918608
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats@sha256:00f69dcad2cdf6b3da43ef4701091ca04d3f35b2ec80c666554d49e5684258d8
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (104957159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edebc41e62feb1ccc604f2e015421dd2e938344719a06d92981822566271a91b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Jul 2020 13:50:07 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jul 2020 15:05:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 15:05:16 GMT
RUN cmd /S /C #(nop) COPY file:18561b827240029ad80d0e3d25142efae62905c30cc520fc37cfc68e7d889848 in C:\nats-server.exe 
# Wed, 15 Jul 2020 15:05:18 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jul 2020 15:05:18 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Jul 2020 15:05:19 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jul 2020 15:05:20 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:dc95608099543221ef539391bfece5c1ce37b97af9da457f5990349cab028a12`  
		Size: 100.9 MB (100895619 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5f0c27d781c53928c03429d5b34e0f49fc26b7e7c996c1d9a2a8474162eade60`  
		Last Modified: Wed, 15 Jul 2020 15:09:50 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10a270f5d0666930958ddfeac073712f678d77b5a05a08210012ada454204077`  
		Last Modified: Wed, 15 Jul 2020 15:10:00 GMT  
		Size: 4.1 MB (4056451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b5e48167a563124481e83cd3f3e3ca1bd3ea8f52b9e52dc9b4982e98a21d7d`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 1.5 KB (1470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64aecdf43c40f563833e5ad1c027bb2e67c1b0c51bb2ab795b99df1f4c2f26f`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 930.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:accd609b6f7304740da44e2a7331717a73ec3f94a35c25198a189b81bd84e204`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 928.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84a11ddf5d09a44b078d904b91df1cd82bf2a0cefb6ec9f52761f36fcf23f54`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:d3e9d8a5a0ad31f0845175c1071e35cea4ac4ebb849c16526e0664a3c0918608
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats@sha256:00f69dcad2cdf6b3da43ef4701091ca04d3f35b2ec80c666554d49e5684258d8
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (104957159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edebc41e62feb1ccc604f2e015421dd2e938344719a06d92981822566271a91b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Jul 2020 13:50:07 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jul 2020 15:05:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 15:05:16 GMT
RUN cmd /S /C #(nop) COPY file:18561b827240029ad80d0e3d25142efae62905c30cc520fc37cfc68e7d889848 in C:\nats-server.exe 
# Wed, 15 Jul 2020 15:05:18 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jul 2020 15:05:18 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Jul 2020 15:05:19 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jul 2020 15:05:20 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:dc95608099543221ef539391bfece5c1ce37b97af9da457f5990349cab028a12`  
		Size: 100.9 MB (100895619 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5f0c27d781c53928c03429d5b34e0f49fc26b7e7c996c1d9a2a8474162eade60`  
		Last Modified: Wed, 15 Jul 2020 15:09:50 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10a270f5d0666930958ddfeac073712f678d77b5a05a08210012ada454204077`  
		Last Modified: Wed, 15 Jul 2020 15:10:00 GMT  
		Size: 4.1 MB (4056451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b5e48167a563124481e83cd3f3e3ca1bd3ea8f52b9e52dc9b4982e98a21d7d`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 1.5 KB (1470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64aecdf43c40f563833e5ad1c027bb2e67c1b0c51bb2ab795b99df1f4c2f26f`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 930.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:accd609b6f7304740da44e2a7331717a73ec3f94a35c25198a189b81bd84e204`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 928.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84a11ddf5d09a44b078d904b91df1cd82bf2a0cefb6ec9f52761f36fcf23f54`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:7a3219e049b4d8b10a7ff389fa689c8d08d5732fe37dcf9c5a72fda463d6c6ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:6aace730d886f9719841c60ec11f826e494b8fcc631378b32f5e01ca32d87ab9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4087969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e93a56bc1852bb18d91f1741edde016c59b49c92f7ad91960d583ee0486ebf3`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 16 May 2020 09:47:58 GMT
COPY file:27ab63fb5115ca3cb7456a256d6d6dab7ba864d8806821652fbe569f4f845df5 in /nats-server 
# Sat, 16 May 2020 09:47:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 16 May 2020 09:47:59 GMT
EXPOSE 4222 6222 8222
# Sat, 16 May 2020 09:47:59 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 16 May 2020 09:47:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b509577c042697add820579de13ceed535b1c02ec7fa460b892d6c63941390a7`  
		Last Modified: Sat, 16 May 2020 09:48:21 GMT  
		Size: 4.1 MB (4087491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ce65065eb7bc6684476be5937b3d0d4046e7cc7241bc5017d70488d0edbfe3`  
		Last Modified: Sat, 16 May 2020 09:48:20 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:e8b59aabb2b6838ced59a3125ba4216cc8a4d0622f8b8c1e9e40fb30cd63a135
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3796375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8116ee7998ff454ed4eaa153438504925828993f56f26fb96fd11b31c9dc2128`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 15 May 2020 19:53:42 GMT
COPY file:9951c1b4ae20021f4d6efd6c039d0f0d0044470572e81beae625f15ffa13d2f1 in /nats-server 
# Fri, 15 May 2020 19:53:43 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 15 May 2020 19:53:44 GMT
EXPOSE 4222 6222 8222
# Fri, 15 May 2020 19:53:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 15 May 2020 19:53:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7976dc3d59fddf78c4ca25d0692135431e63b9fb744ae2c3d02b7a8214b5bfd9`  
		Last Modified: Fri, 15 May 2020 19:54:21 GMT  
		Size: 3.8 MB (3795898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b520f7415a5fab1b4a83eb7a8259e321475f75f5b06bfe95493b598c9ee9f4`  
		Last Modified: Fri, 15 May 2020 19:54:20 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:707f02b7c81a3f071abba9ce0a74b1cf0bf7a664e0220ab6cae112f2721a24bf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3792273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d2f2220669ef3621c45d5e4fd8460e7378e258044eb57003584ce55db5bdd9b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 16 May 2020 04:26:09 GMT
COPY file:3320edcd8f0db9551469809c752244493d1c6cf3be0287714c8a507e339283b2 in /nats-server 
# Sat, 16 May 2020 04:26:09 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 16 May 2020 04:26:11 GMT
EXPOSE 4222 6222 8222
# Sat, 16 May 2020 04:26:12 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 16 May 2020 04:26:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7ceefb66163b74f9719728ecace35bd406e85998a252d90c9e07a02582c7b6f1`  
		Last Modified: Sat, 16 May 2020 04:26:55 GMT  
		Size: 3.8 MB (3791795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db182fe235e1ef3b80de633e39d8ab9040cef44127adee97dbc4513df27dacfe`  
		Last Modified: Sat, 16 May 2020 04:26:53 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8cb2b90d45f90f3bdfb841b4a1399ff3a1b0a835e54664ee375ef309ff4c4398
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3776968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fffbb615827376dda1ad45bce22763d7cdc858675e4eafc55deb2d134f813338`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 29 Jul 2020 22:41:42 GMT
COPY file:67a03d7df05756de9c16c4cd22dfaf6ed9cc9a43b78a90ebfaa81ee7ebbc7abf in /nats-server 
# Wed, 29 Jul 2020 22:41:43 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 29 Jul 2020 22:41:44 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 22:41:44 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 29 Jul 2020 22:41:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:39a183ba93759b5fab08b0cb81f1f1a4c9f5a95c3746b031082c6bc3a57441b3`  
		Last Modified: Wed, 29 Jul 2020 22:42:18 GMT  
		Size: 3.8 MB (3776492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a510a0d87b5b915212ee2a5e5d877dced1c30164c0e82d6e60951d00374fe7`  
		Last Modified: Wed, 29 Jul 2020 22:42:17 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:59a9a5745643d652dd6d49be5d422a2270a2539f6dfa398ba219d78c00c701e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64
	-	windows version 10.0.14393.3808; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats@sha256:84ed3b1eb1e35102dff57509d666e9ae99f4fd0a492b9410b473bedda4aeebdf
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2328185203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8d69d5e23b4cff9ad8df708d4059e6525b91686ad490775e104e6c06b863457`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Wed, 15 Jul 2020 12:15:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jul 2020 15:03:03 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 15:03:03 GMT
ENV NATS_SERVER=2.1.7
# Wed, 15 Jul 2020 15:03:04 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.7/nats-server-v2.1.7-windows-amd64.zip
# Wed, 29 Jul 2020 23:14:26 GMT
ENV GIT_DOWNLOAD_SHA256=1e1ad5c00929cc145341fd65f8b0a41a38e942b9b9fd9fdb0216c47654afdc8f
# Wed, 29 Jul 2020 23:15:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 29 Jul 2020 23:16:49 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 29 Jul 2020 23:16:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 29 Jul 2020 23:16:54 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 23:16:55 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 29 Jul 2020 23:16:56 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1cc883a0e3509a474bb32f3c40411bf86219325ae9710e25a5dcce6b44eef357`  
		Last Modified: Wed, 15 Jul 2020 14:32:06 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dd35c9a62007b6ded1ca968562be97de62ea3e2b3c7db85f4a50baaa9efecb`  
		Last Modified: Wed, 15 Jul 2020 15:09:33 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5789d32300712f2fa8b6564efe911f5f523cf150f1fde2bf8d6deedbb56feb4`  
		Last Modified: Wed, 15 Jul 2020 15:09:32 GMT  
		Size: 1.1 KB (1105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b62b1740ff37517c10b8b8bfae73367d0c5538cf934392846eea648031c1857`  
		Last Modified: Wed, 15 Jul 2020 15:09:31 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c765e0c4aba82f5140dd325bb9fc2dc97095f673b4d88039867aecc92e331f5e`  
		Last Modified: Wed, 29 Jul 2020 23:21:23 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9dfd44060c9c9e79fca23ba4227434b55a5a3353c7a32ba8140fa252af2631f`  
		Last Modified: Wed, 29 Jul 2020 23:21:24 GMT  
		Size: 4.8 MB (4803853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011be3335c53769b99af80accd8e25f40172d44bc0e20780c88f1ab787bbf09e`  
		Last Modified: Wed, 29 Jul 2020 23:21:24 GMT  
		Size: 13.2 MB (13178319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f913f5767f1c088f27134bdefc531acacd106610ce085ef7ca5470fdeda55e80`  
		Last Modified: Wed, 29 Jul 2020 23:21:20 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8436f3f54d22f495452cdb61489bf5833c2cda6a2e6012c732b2c8ffbc72262f`  
		Last Modified: Wed, 29 Jul 2020 23:21:20 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12724c1ab2196db2d2cd8bff6069b1ea932e514cd5473240dd515f50361e4fa`  
		Last Modified: Wed, 29 Jul 2020 23:21:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419a5e47094ff5e8a8cb733bf81fcd97e46b00a5b62b9cbcd5993a66942a7e7e`  
		Last Modified: Wed, 29 Jul 2020 23:21:20 GMT  
		Size: 1.1 KB (1100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-windowsservercore` - windows version 10.0.14393.3808; amd64

```console
$ docker pull nats@sha256:9145e80ebf209b601e34e199defd755bf43a5b09f674ece13c4c6299b21d4870
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5756757168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a3c13889118f6f6c65e859be772b7b0cb7e0497de0a2326a3b54c097daa6670`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Jul 2020 21:05:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Jul 2020 12:24:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jul 2020 15:05:26 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 15:05:27 GMT
ENV NATS_SERVER=2.1.7
# Wed, 15 Jul 2020 15:05:28 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.7/nats-server-v2.1.7-windows-amd64.zip
# Wed, 29 Jul 2020 23:17:15 GMT
ENV GIT_DOWNLOAD_SHA256=1e1ad5c00929cc145341fd65f8b0a41a38e942b9b9fd9fdb0216c47654afdc8f
# Wed, 29 Jul 2020 23:18:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 29 Jul 2020 23:20:43 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 29 Jul 2020 23:20:45 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 29 Jul 2020 23:20:46 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 23:20:47 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 29 Jul 2020 23:20:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:802c4beb8b091968ccf1bb4a853ded7955ddb79e6f8775a5155cb5ed07dcbcab`  
		Size: 1.7 GB (1667476199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3393eecaf56a66035ab178b379bacf81d30373b630b34b2973501f259aadb0f6`  
		Last Modified: Wed, 15 Jul 2020 14:32:38 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1430ee68db5fe3026683f1b7c74f31ae748da71bf8ad611efede726e9e036b1`  
		Last Modified: Wed, 15 Jul 2020 15:10:21 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae29b1720308eb8710d921cefbc8979061e4535b6276b35b3d471e08a09e7af`  
		Last Modified: Wed, 15 Jul 2020 15:10:19 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a76213345cac0ca18badbc3c8262b6973e3457484fdcb9af380fa4de2c64ea`  
		Last Modified: Wed, 15 Jul 2020 15:10:19 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2713fe8ba40241bc8ef85e6795703e42f101f0ab81d143357c549a03c4b00c`  
		Last Modified: Wed, 29 Jul 2020 23:21:44 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b8f23b09829f938cc622501d4059590b050bc95a7fb4c5d2e337e423af1e23`  
		Last Modified: Wed, 29 Jul 2020 23:21:46 GMT  
		Size: 5.4 MB (5391705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0857d1594c42a8ff34ec0fc99b717f343d2e6dcdcb980e3b54621a8127ecf4a`  
		Last Modified: Wed, 29 Jul 2020 23:21:57 GMT  
		Size: 13.9 MB (13892511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7afe295ad113f1145078cde44f86ce197d64aa5ceb92784bf4c60ff710b95256`  
		Last Modified: Wed, 29 Jul 2020 23:21:41 GMT  
		Size: 1.7 KB (1683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9b54006dba8cc76bc2325f78d0377969e727070a8f9069e26090b7a4e18f36`  
		Last Modified: Wed, 29 Jul 2020 23:21:41 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97bb5b91db82c40b2b26f5fcc7a1e07fce677242cd70722fbe2d3256e4548dfc`  
		Last Modified: Wed, 29 Jul 2020 23:21:42 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58919d245b3713c0a29f1039075f368c82d09514f57a595cade8fae1010c7847`  
		Last Modified: Wed, 29 Jul 2020 23:21:42 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:f9351e549406b5be23d79a960a8188aae30b521a25b98855bcf4ad382d0446e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats@sha256:84ed3b1eb1e35102dff57509d666e9ae99f4fd0a492b9410b473bedda4aeebdf
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2328185203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8d69d5e23b4cff9ad8df708d4059e6525b91686ad490775e104e6c06b863457`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Wed, 15 Jul 2020 12:15:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jul 2020 15:03:03 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 15:03:03 GMT
ENV NATS_SERVER=2.1.7
# Wed, 15 Jul 2020 15:03:04 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.7/nats-server-v2.1.7-windows-amd64.zip
# Wed, 29 Jul 2020 23:14:26 GMT
ENV GIT_DOWNLOAD_SHA256=1e1ad5c00929cc145341fd65f8b0a41a38e942b9b9fd9fdb0216c47654afdc8f
# Wed, 29 Jul 2020 23:15:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 29 Jul 2020 23:16:49 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 29 Jul 2020 23:16:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 29 Jul 2020 23:16:54 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 23:16:55 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 29 Jul 2020 23:16:56 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1cc883a0e3509a474bb32f3c40411bf86219325ae9710e25a5dcce6b44eef357`  
		Last Modified: Wed, 15 Jul 2020 14:32:06 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dd35c9a62007b6ded1ca968562be97de62ea3e2b3c7db85f4a50baaa9efecb`  
		Last Modified: Wed, 15 Jul 2020 15:09:33 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5789d32300712f2fa8b6564efe911f5f523cf150f1fde2bf8d6deedbb56feb4`  
		Last Modified: Wed, 15 Jul 2020 15:09:32 GMT  
		Size: 1.1 KB (1105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b62b1740ff37517c10b8b8bfae73367d0c5538cf934392846eea648031c1857`  
		Last Modified: Wed, 15 Jul 2020 15:09:31 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c765e0c4aba82f5140dd325bb9fc2dc97095f673b4d88039867aecc92e331f5e`  
		Last Modified: Wed, 29 Jul 2020 23:21:23 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9dfd44060c9c9e79fca23ba4227434b55a5a3353c7a32ba8140fa252af2631f`  
		Last Modified: Wed, 29 Jul 2020 23:21:24 GMT  
		Size: 4.8 MB (4803853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011be3335c53769b99af80accd8e25f40172d44bc0e20780c88f1ab787bbf09e`  
		Last Modified: Wed, 29 Jul 2020 23:21:24 GMT  
		Size: 13.2 MB (13178319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f913f5767f1c088f27134bdefc531acacd106610ce085ef7ca5470fdeda55e80`  
		Last Modified: Wed, 29 Jul 2020 23:21:20 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8436f3f54d22f495452cdb61489bf5833c2cda6a2e6012c732b2c8ffbc72262f`  
		Last Modified: Wed, 29 Jul 2020 23:21:20 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12724c1ab2196db2d2cd8bff6069b1ea932e514cd5473240dd515f50361e4fa`  
		Last Modified: Wed, 29 Jul 2020 23:21:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419a5e47094ff5e8a8cb733bf81fcd97e46b00a5b62b9cbcd5993a66942a7e7e`  
		Last Modified: Wed, 29 Jul 2020 23:21:20 GMT  
		Size: 1.1 KB (1100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:f405d1c17c29cd33ba2762684ab3ee983dbaafd8df62ef7b12fa78b3ad6b7d3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3808; amd64

### `nats:2-windowsservercore-ltsc2016` - windows version 10.0.14393.3808; amd64

```console
$ docker pull nats@sha256:9145e80ebf209b601e34e199defd755bf43a5b09f674ece13c4c6299b21d4870
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5756757168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a3c13889118f6f6c65e859be772b7b0cb7e0497de0a2326a3b54c097daa6670`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Jul 2020 21:05:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Jul 2020 12:24:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jul 2020 15:05:26 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 15:05:27 GMT
ENV NATS_SERVER=2.1.7
# Wed, 15 Jul 2020 15:05:28 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.7/nats-server-v2.1.7-windows-amd64.zip
# Wed, 29 Jul 2020 23:17:15 GMT
ENV GIT_DOWNLOAD_SHA256=1e1ad5c00929cc145341fd65f8b0a41a38e942b9b9fd9fdb0216c47654afdc8f
# Wed, 29 Jul 2020 23:18:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 29 Jul 2020 23:20:43 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 29 Jul 2020 23:20:45 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 29 Jul 2020 23:20:46 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 23:20:47 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 29 Jul 2020 23:20:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:802c4beb8b091968ccf1bb4a853ded7955ddb79e6f8775a5155cb5ed07dcbcab`  
		Size: 1.7 GB (1667476199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3393eecaf56a66035ab178b379bacf81d30373b630b34b2973501f259aadb0f6`  
		Last Modified: Wed, 15 Jul 2020 14:32:38 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1430ee68db5fe3026683f1b7c74f31ae748da71bf8ad611efede726e9e036b1`  
		Last Modified: Wed, 15 Jul 2020 15:10:21 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae29b1720308eb8710d921cefbc8979061e4535b6276b35b3d471e08a09e7af`  
		Last Modified: Wed, 15 Jul 2020 15:10:19 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a76213345cac0ca18badbc3c8262b6973e3457484fdcb9af380fa4de2c64ea`  
		Last Modified: Wed, 15 Jul 2020 15:10:19 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2713fe8ba40241bc8ef85e6795703e42f101f0ab81d143357c549a03c4b00c`  
		Last Modified: Wed, 29 Jul 2020 23:21:44 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b8f23b09829f938cc622501d4059590b050bc95a7fb4c5d2e337e423af1e23`  
		Last Modified: Wed, 29 Jul 2020 23:21:46 GMT  
		Size: 5.4 MB (5391705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0857d1594c42a8ff34ec0fc99b717f343d2e6dcdcb980e3b54621a8127ecf4a`  
		Last Modified: Wed, 29 Jul 2020 23:21:57 GMT  
		Size: 13.9 MB (13892511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7afe295ad113f1145078cde44f86ce197d64aa5ceb92784bf4c60ff710b95256`  
		Last Modified: Wed, 29 Jul 2020 23:21:41 GMT  
		Size: 1.7 KB (1683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9b54006dba8cc76bc2325f78d0377969e727070a8f9069e26090b7a4e18f36`  
		Last Modified: Wed, 29 Jul 2020 23:21:41 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97bb5b91db82c40b2b26f5fcc7a1e07fce677242cd70722fbe2d3256e4548dfc`  
		Last Modified: Wed, 29 Jul 2020 23:21:42 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58919d245b3713c0a29f1039075f368c82d09514f57a595cade8fae1010c7847`  
		Last Modified: Wed, 29 Jul 2020 23:21:42 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:2ca671f95f6f5c4d9144a701d8b7be77a1830041d86766e2e193fb58b00af449
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:c1c1159e76d03431b2c612d378a62fc914f0817df3f9a8092adddb589ac74e53
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7203227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54acd9cf4794435761c0462aba37d41e69e9581a77daeef4d16255b6a579f2c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Sat, 16 May 2020 09:47:11 GMT
ENV NATS_SERVER=2.1.7
# Wed, 29 Jul 2020 23:25:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a08d7ce0399df8701d3e3cd4c36744180c3a566cdb38efeccc12a364f0083705' ;; 		armhf) natsArch='arm6'; sha256='987c23f758842fb09c0d4500f632c5302aedc61d218f03998444b94074aabddb' ;; 		armv7) natsArch='arm7'; sha256='077fd1647aa25865ade5acc3d6ee5f542d2c62feb2fb41ec6d1dd83294bea05e' ;; 		x86_64) natsArch='amd64'; sha256='23cce53fe7f628f203dbbeadf434c3480d094690aba6ff0b1d374b8f2f9ffd8c' ;; 		x86) natsArch='386'; sha256='64e271690782af823930c95574db0f701d06a36ff42b9272c04841d4611bcd15' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:25:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 29 Jul 2020 23:25:41 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Jul 2020 23:25:42 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 23:25:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:25:42 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09eebfe9509bcbfcefadbc17c68fa103be7b7cf978f08ea01527a6aba38c5554`  
		Last Modified: Wed, 29 Jul 2020 23:26:16 GMT  
		Size: 4.4 MB (4388967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab62a5d69bc21353fa665e0b7fbf8e6a4a5d3fda0e87d58c02073999f76ff43f`  
		Last Modified: Wed, 29 Jul 2020 23:26:15 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a297d716cd17565b8a6331222fe5c2bcf967f50c6e424f62a5051e864941e2`  
		Last Modified: Wed, 29 Jul 2020 23:26:15 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:fee67afb8a9c6c38c60a5b90f51b6a6dfdb607b13d04240cf4faae9f8235d69d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6717777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb5af24d85d20ca2ddf1a257d6667c94e32ad6c1f381964f6ea48833ebc6eb39`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Fri, 15 May 2020 19:50:13 GMT
ENV NATS_SERVER=2.1.7
# Wed, 29 Jul 2020 23:02:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a08d7ce0399df8701d3e3cd4c36744180c3a566cdb38efeccc12a364f0083705' ;; 		armhf) natsArch='arm6'; sha256='987c23f758842fb09c0d4500f632c5302aedc61d218f03998444b94074aabddb' ;; 		armv7) natsArch='arm7'; sha256='077fd1647aa25865ade5acc3d6ee5f542d2c62feb2fb41ec6d1dd83294bea05e' ;; 		x86_64) natsArch='amd64'; sha256='23cce53fe7f628f203dbbeadf434c3480d094690aba6ff0b1d374b8f2f9ffd8c' ;; 		x86) natsArch='386'; sha256='64e271690782af823930c95574db0f701d06a36ff42b9272c04841d4611bcd15' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:02:35 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 29 Jul 2020 23:02:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Jul 2020 23:02:36 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 23:02:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:02:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0546a69fc010fc7d9fdae3cd6ff1eb8d7d7471a3561d782f6bb2bebcb079ad`  
		Last Modified: Wed, 29 Jul 2020 23:03:02 GMT  
		Size: 4.1 MB (4096870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02dc6927e9f4f4d185c4420481f8b1e06d55f058ad32ac4c0a9fc2ca3c2e0e64`  
		Last Modified: Wed, 29 Jul 2020 23:03:01 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6963e293037e1e7ddf702b89cf5a9441918b610e877f1710001b055560f92901`  
		Last Modified: Wed, 29 Jul 2020 23:03:01 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:197a92e111811ad767369a9bd75175ecb906fa57009400e78fa5d07ff8b0b47d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6515331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4546538a81c298be13378de43d24f5778e46917a8c2e6feca95287f8695e7d82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Sat, 16 May 2020 04:17:01 GMT
ENV NATS_SERVER=2.1.7
# Wed, 29 Jul 2020 23:11:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a08d7ce0399df8701d3e3cd4c36744180c3a566cdb38efeccc12a364f0083705' ;; 		armhf) natsArch='arm6'; sha256='987c23f758842fb09c0d4500f632c5302aedc61d218f03998444b94074aabddb' ;; 		armv7) natsArch='arm7'; sha256='077fd1647aa25865ade5acc3d6ee5f542d2c62feb2fb41ec6d1dd83294bea05e' ;; 		x86_64) natsArch='amd64'; sha256='23cce53fe7f628f203dbbeadf434c3480d094690aba6ff0b1d374b8f2f9ffd8c' ;; 		x86) natsArch='386'; sha256='64e271690782af823930c95574db0f701d06a36ff42b9272c04841d4611bcd15' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:11:46 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 29 Jul 2020 23:11:46 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Jul 2020 23:11:47 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 23:11:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:11:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4572ecf34c0bc5aa1ca0925f8f3c17e07cdf857ae8e31be72e5360711b24016`  
		Last Modified: Wed, 29 Jul 2020 23:15:57 GMT  
		Size: 4.1 MB (4092296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67632d2c07c7d161703500f1b0fa040775c8cb0c4474b8749a8ea961b5964f7e`  
		Last Modified: Wed, 29 Jul 2020 23:15:56 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5f50a8c5ae0937cd72ab745aacf65d53e62fed9a22d0de4fb3fe2f3d88a9b6`  
		Last Modified: Wed, 29 Jul 2020 23:15:56 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:e3338a58db906f99cb91860cf607e3670e8b6676026d2eb70d26100b26bfcd5f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6803458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e79bcc07d57e06d12e6ae92a95f16c0dfe72401e9efdc3a3869273d02110feda`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Jul 2020 16:28:21 GMT
ENV NATS_SERVER=2.1.7
# Wed, 29 Jul 2020 22:41:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a08d7ce0399df8701d3e3cd4c36744180c3a566cdb38efeccc12a364f0083705' ;; 		armhf) natsArch='arm6'; sha256='987c23f758842fb09c0d4500f632c5302aedc61d218f03998444b94074aabddb' ;; 		armv7) natsArch='arm7'; sha256='077fd1647aa25865ade5acc3d6ee5f542d2c62feb2fb41ec6d1dd83294bea05e' ;; 		x86_64) natsArch='amd64'; sha256='23cce53fe7f628f203dbbeadf434c3480d094690aba6ff0b1d374b8f2f9ffd8c' ;; 		x86) natsArch='386'; sha256='64e271690782af823930c95574db0f701d06a36ff42b9272c04841d4611bcd15' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 22:41:30 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 29 Jul 2020 22:41:30 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Jul 2020 22:41:31 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 22:41:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 22:41:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e23520311eff0ccb9b4116bad00040e13d45013d01d87ee89bba20b01b5e536`  
		Last Modified: Wed, 29 Jul 2020 22:42:03 GMT  
		Size: 4.1 MB (4078060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5bd55073b3a781fd6af08f7e29facaf7e8d37e977fc7b8a7bcb57098c1dc49b`  
		Last Modified: Wed, 29 Jul 2020 22:42:02 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2eb0d8170b7670bd8ae9406d3cc6298a0cc3b8f3ec7434dd09ec858f8701183`  
		Last Modified: Wed, 29 Jul 2020 22:42:02 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.11`

```console
$ docker pull nats@sha256:2ca671f95f6f5c4d9144a701d8b7be77a1830041d86766e2e193fb58b00af449
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.11` - linux; amd64

```console
$ docker pull nats@sha256:c1c1159e76d03431b2c612d378a62fc914f0817df3f9a8092adddb589ac74e53
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7203227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54acd9cf4794435761c0462aba37d41e69e9581a77daeef4d16255b6a579f2c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Sat, 16 May 2020 09:47:11 GMT
ENV NATS_SERVER=2.1.7
# Wed, 29 Jul 2020 23:25:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a08d7ce0399df8701d3e3cd4c36744180c3a566cdb38efeccc12a364f0083705' ;; 		armhf) natsArch='arm6'; sha256='987c23f758842fb09c0d4500f632c5302aedc61d218f03998444b94074aabddb' ;; 		armv7) natsArch='arm7'; sha256='077fd1647aa25865ade5acc3d6ee5f542d2c62feb2fb41ec6d1dd83294bea05e' ;; 		x86_64) natsArch='amd64'; sha256='23cce53fe7f628f203dbbeadf434c3480d094690aba6ff0b1d374b8f2f9ffd8c' ;; 		x86) natsArch='386'; sha256='64e271690782af823930c95574db0f701d06a36ff42b9272c04841d4611bcd15' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:25:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 29 Jul 2020 23:25:41 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Jul 2020 23:25:42 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 23:25:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:25:42 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09eebfe9509bcbfcefadbc17c68fa103be7b7cf978f08ea01527a6aba38c5554`  
		Last Modified: Wed, 29 Jul 2020 23:26:16 GMT  
		Size: 4.4 MB (4388967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab62a5d69bc21353fa665e0b7fbf8e6a4a5d3fda0e87d58c02073999f76ff43f`  
		Last Modified: Wed, 29 Jul 2020 23:26:15 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a297d716cd17565b8a6331222fe5c2bcf967f50c6e424f62a5051e864941e2`  
		Last Modified: Wed, 29 Jul 2020 23:26:15 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.11` - linux; arm variant v6

```console
$ docker pull nats@sha256:fee67afb8a9c6c38c60a5b90f51b6a6dfdb607b13d04240cf4faae9f8235d69d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6717777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb5af24d85d20ca2ddf1a257d6667c94e32ad6c1f381964f6ea48833ebc6eb39`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Fri, 15 May 2020 19:50:13 GMT
ENV NATS_SERVER=2.1.7
# Wed, 29 Jul 2020 23:02:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a08d7ce0399df8701d3e3cd4c36744180c3a566cdb38efeccc12a364f0083705' ;; 		armhf) natsArch='arm6'; sha256='987c23f758842fb09c0d4500f632c5302aedc61d218f03998444b94074aabddb' ;; 		armv7) natsArch='arm7'; sha256='077fd1647aa25865ade5acc3d6ee5f542d2c62feb2fb41ec6d1dd83294bea05e' ;; 		x86_64) natsArch='amd64'; sha256='23cce53fe7f628f203dbbeadf434c3480d094690aba6ff0b1d374b8f2f9ffd8c' ;; 		x86) natsArch='386'; sha256='64e271690782af823930c95574db0f701d06a36ff42b9272c04841d4611bcd15' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:02:35 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 29 Jul 2020 23:02:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Jul 2020 23:02:36 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 23:02:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:02:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0546a69fc010fc7d9fdae3cd6ff1eb8d7d7471a3561d782f6bb2bebcb079ad`  
		Last Modified: Wed, 29 Jul 2020 23:03:02 GMT  
		Size: 4.1 MB (4096870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02dc6927e9f4f4d185c4420481f8b1e06d55f058ad32ac4c0a9fc2ca3c2e0e64`  
		Last Modified: Wed, 29 Jul 2020 23:03:01 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6963e293037e1e7ddf702b89cf5a9441918b610e877f1710001b055560f92901`  
		Last Modified: Wed, 29 Jul 2020 23:03:01 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.11` - linux; arm variant v7

```console
$ docker pull nats@sha256:197a92e111811ad767369a9bd75175ecb906fa57009400e78fa5d07ff8b0b47d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6515331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4546538a81c298be13378de43d24f5778e46917a8c2e6feca95287f8695e7d82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Sat, 16 May 2020 04:17:01 GMT
ENV NATS_SERVER=2.1.7
# Wed, 29 Jul 2020 23:11:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a08d7ce0399df8701d3e3cd4c36744180c3a566cdb38efeccc12a364f0083705' ;; 		armhf) natsArch='arm6'; sha256='987c23f758842fb09c0d4500f632c5302aedc61d218f03998444b94074aabddb' ;; 		armv7) natsArch='arm7'; sha256='077fd1647aa25865ade5acc3d6ee5f542d2c62feb2fb41ec6d1dd83294bea05e' ;; 		x86_64) natsArch='amd64'; sha256='23cce53fe7f628f203dbbeadf434c3480d094690aba6ff0b1d374b8f2f9ffd8c' ;; 		x86) natsArch='386'; sha256='64e271690782af823930c95574db0f701d06a36ff42b9272c04841d4611bcd15' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:11:46 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 29 Jul 2020 23:11:46 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Jul 2020 23:11:47 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 23:11:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:11:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4572ecf34c0bc5aa1ca0925f8f3c17e07cdf857ae8e31be72e5360711b24016`  
		Last Modified: Wed, 29 Jul 2020 23:15:57 GMT  
		Size: 4.1 MB (4092296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67632d2c07c7d161703500f1b0fa040775c8cb0c4474b8749a8ea961b5964f7e`  
		Last Modified: Wed, 29 Jul 2020 23:15:56 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5f50a8c5ae0937cd72ab745aacf65d53e62fed9a22d0de4fb3fe2f3d88a9b6`  
		Last Modified: Wed, 29 Jul 2020 23:15:56 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.11` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:e3338a58db906f99cb91860cf607e3670e8b6676026d2eb70d26100b26bfcd5f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6803458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e79bcc07d57e06d12e6ae92a95f16c0dfe72401e9efdc3a3869273d02110feda`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Jul 2020 16:28:21 GMT
ENV NATS_SERVER=2.1.7
# Wed, 29 Jul 2020 22:41:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a08d7ce0399df8701d3e3cd4c36744180c3a566cdb38efeccc12a364f0083705' ;; 		armhf) natsArch='arm6'; sha256='987c23f758842fb09c0d4500f632c5302aedc61d218f03998444b94074aabddb' ;; 		armv7) natsArch='arm7'; sha256='077fd1647aa25865ade5acc3d6ee5f542d2c62feb2fb41ec6d1dd83294bea05e' ;; 		x86_64) natsArch='amd64'; sha256='23cce53fe7f628f203dbbeadf434c3480d094690aba6ff0b1d374b8f2f9ffd8c' ;; 		x86) natsArch='386'; sha256='64e271690782af823930c95574db0f701d06a36ff42b9272c04841d4611bcd15' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 22:41:30 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 29 Jul 2020 22:41:30 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Jul 2020 22:41:31 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 22:41:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 22:41:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e23520311eff0ccb9b4116bad00040e13d45013d01d87ee89bba20b01b5e536`  
		Last Modified: Wed, 29 Jul 2020 22:42:03 GMT  
		Size: 4.1 MB (4078060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5bd55073b3a781fd6af08f7e29facaf7e8d37e977fc7b8a7bcb57098c1dc49b`  
		Last Modified: Wed, 29 Jul 2020 22:42:02 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2eb0d8170b7670bd8ae9406d3cc6298a0cc3b8f3ec7434dd09ec858f8701183`  
		Last Modified: Wed, 29 Jul 2020 22:42:02 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:35d212a94eb9c1d6568d91f450637a8a597ecb703b5d32425df06a31945bbf32
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1339; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:6aace730d886f9719841c60ec11f826e494b8fcc631378b32f5e01ca32d87ab9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4087969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e93a56bc1852bb18d91f1741edde016c59b49c92f7ad91960d583ee0486ebf3`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 16 May 2020 09:47:58 GMT
COPY file:27ab63fb5115ca3cb7456a256d6d6dab7ba864d8806821652fbe569f4f845df5 in /nats-server 
# Sat, 16 May 2020 09:47:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 16 May 2020 09:47:59 GMT
EXPOSE 4222 6222 8222
# Sat, 16 May 2020 09:47:59 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 16 May 2020 09:47:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b509577c042697add820579de13ceed535b1c02ec7fa460b892d6c63941390a7`  
		Last Modified: Sat, 16 May 2020 09:48:21 GMT  
		Size: 4.1 MB (4087491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ce65065eb7bc6684476be5937b3d0d4046e7cc7241bc5017d70488d0edbfe3`  
		Last Modified: Sat, 16 May 2020 09:48:20 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:e8b59aabb2b6838ced59a3125ba4216cc8a4d0622f8b8c1e9e40fb30cd63a135
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3796375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8116ee7998ff454ed4eaa153438504925828993f56f26fb96fd11b31c9dc2128`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 15 May 2020 19:53:42 GMT
COPY file:9951c1b4ae20021f4d6efd6c039d0f0d0044470572e81beae625f15ffa13d2f1 in /nats-server 
# Fri, 15 May 2020 19:53:43 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 15 May 2020 19:53:44 GMT
EXPOSE 4222 6222 8222
# Fri, 15 May 2020 19:53:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 15 May 2020 19:53:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7976dc3d59fddf78c4ca25d0692135431e63b9fb744ae2c3d02b7a8214b5bfd9`  
		Last Modified: Fri, 15 May 2020 19:54:21 GMT  
		Size: 3.8 MB (3795898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b520f7415a5fab1b4a83eb7a8259e321475f75f5b06bfe95493b598c9ee9f4`  
		Last Modified: Fri, 15 May 2020 19:54:20 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:707f02b7c81a3f071abba9ce0a74b1cf0bf7a664e0220ab6cae112f2721a24bf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3792273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d2f2220669ef3621c45d5e4fd8460e7378e258044eb57003584ce55db5bdd9b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 16 May 2020 04:26:09 GMT
COPY file:3320edcd8f0db9551469809c752244493d1c6cf3be0287714c8a507e339283b2 in /nats-server 
# Sat, 16 May 2020 04:26:09 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 16 May 2020 04:26:11 GMT
EXPOSE 4222 6222 8222
# Sat, 16 May 2020 04:26:12 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 16 May 2020 04:26:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7ceefb66163b74f9719728ecace35bd406e85998a252d90c9e07a02582c7b6f1`  
		Last Modified: Sat, 16 May 2020 04:26:55 GMT  
		Size: 3.8 MB (3791795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db182fe235e1ef3b80de633e39d8ab9040cef44127adee97dbc4513df27dacfe`  
		Last Modified: Sat, 16 May 2020 04:26:53 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8cb2b90d45f90f3bdfb841b4a1399ff3a1b0a835e54664ee375ef309ff4c4398
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3776968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fffbb615827376dda1ad45bce22763d7cdc858675e4eafc55deb2d134f813338`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 29 Jul 2020 22:41:42 GMT
COPY file:67a03d7df05756de9c16c4cd22dfaf6ed9cc9a43b78a90ebfaa81ee7ebbc7abf in /nats-server 
# Wed, 29 Jul 2020 22:41:43 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 29 Jul 2020 22:41:44 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 22:41:44 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 29 Jul 2020 22:41:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:39a183ba93759b5fab08b0cb81f1f1a4c9f5a95c3746b031082c6bc3a57441b3`  
		Last Modified: Wed, 29 Jul 2020 22:42:18 GMT  
		Size: 3.8 MB (3776492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a510a0d87b5b915212ee2a5e5d877dced1c30164c0e82d6e60951d00374fe7`  
		Last Modified: Wed, 29 Jul 2020 22:42:17 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats@sha256:00f69dcad2cdf6b3da43ef4701091ca04d3f35b2ec80c666554d49e5684258d8
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (104957159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edebc41e62feb1ccc604f2e015421dd2e938344719a06d92981822566271a91b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Jul 2020 13:50:07 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jul 2020 15:05:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 15:05:16 GMT
RUN cmd /S /C #(nop) COPY file:18561b827240029ad80d0e3d25142efae62905c30cc520fc37cfc68e7d889848 in C:\nats-server.exe 
# Wed, 15 Jul 2020 15:05:18 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jul 2020 15:05:18 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Jul 2020 15:05:19 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jul 2020 15:05:20 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:dc95608099543221ef539391bfece5c1ce37b97af9da457f5990349cab028a12`  
		Size: 100.9 MB (100895619 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5f0c27d781c53928c03429d5b34e0f49fc26b7e7c996c1d9a2a8474162eade60`  
		Last Modified: Wed, 15 Jul 2020 15:09:50 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10a270f5d0666930958ddfeac073712f678d77b5a05a08210012ada454204077`  
		Last Modified: Wed, 15 Jul 2020 15:10:00 GMT  
		Size: 4.1 MB (4056451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b5e48167a563124481e83cd3f3e3ca1bd3ea8f52b9e52dc9b4982e98a21d7d`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 1.5 KB (1470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64aecdf43c40f563833e5ad1c027bb2e67c1b0c51bb2ab795b99df1f4c2f26f`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 930.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:accd609b6f7304740da44e2a7331717a73ec3f94a35c25198a189b81bd84e204`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 928.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84a11ddf5d09a44b078d904b91df1cd82bf2a0cefb6ec9f52761f36fcf23f54`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:7a3219e049b4d8b10a7ff389fa689c8d08d5732fe37dcf9c5a72fda463d6c6ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:6aace730d886f9719841c60ec11f826e494b8fcc631378b32f5e01ca32d87ab9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4087969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e93a56bc1852bb18d91f1741edde016c59b49c92f7ad91960d583ee0486ebf3`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 16 May 2020 09:47:58 GMT
COPY file:27ab63fb5115ca3cb7456a256d6d6dab7ba864d8806821652fbe569f4f845df5 in /nats-server 
# Sat, 16 May 2020 09:47:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 16 May 2020 09:47:59 GMT
EXPOSE 4222 6222 8222
# Sat, 16 May 2020 09:47:59 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 16 May 2020 09:47:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b509577c042697add820579de13ceed535b1c02ec7fa460b892d6c63941390a7`  
		Last Modified: Sat, 16 May 2020 09:48:21 GMT  
		Size: 4.1 MB (4087491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ce65065eb7bc6684476be5937b3d0d4046e7cc7241bc5017d70488d0edbfe3`  
		Last Modified: Sat, 16 May 2020 09:48:20 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:e8b59aabb2b6838ced59a3125ba4216cc8a4d0622f8b8c1e9e40fb30cd63a135
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3796375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8116ee7998ff454ed4eaa153438504925828993f56f26fb96fd11b31c9dc2128`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 15 May 2020 19:53:42 GMT
COPY file:9951c1b4ae20021f4d6efd6c039d0f0d0044470572e81beae625f15ffa13d2f1 in /nats-server 
# Fri, 15 May 2020 19:53:43 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 15 May 2020 19:53:44 GMT
EXPOSE 4222 6222 8222
# Fri, 15 May 2020 19:53:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 15 May 2020 19:53:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7976dc3d59fddf78c4ca25d0692135431e63b9fb744ae2c3d02b7a8214b5bfd9`  
		Last Modified: Fri, 15 May 2020 19:54:21 GMT  
		Size: 3.8 MB (3795898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b520f7415a5fab1b4a83eb7a8259e321475f75f5b06bfe95493b598c9ee9f4`  
		Last Modified: Fri, 15 May 2020 19:54:20 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:707f02b7c81a3f071abba9ce0a74b1cf0bf7a664e0220ab6cae112f2721a24bf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3792273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d2f2220669ef3621c45d5e4fd8460e7378e258044eb57003584ce55db5bdd9b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 16 May 2020 04:26:09 GMT
COPY file:3320edcd8f0db9551469809c752244493d1c6cf3be0287714c8a507e339283b2 in /nats-server 
# Sat, 16 May 2020 04:26:09 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 16 May 2020 04:26:11 GMT
EXPOSE 4222 6222 8222
# Sat, 16 May 2020 04:26:12 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 16 May 2020 04:26:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7ceefb66163b74f9719728ecace35bd406e85998a252d90c9e07a02582c7b6f1`  
		Last Modified: Sat, 16 May 2020 04:26:55 GMT  
		Size: 3.8 MB (3791795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db182fe235e1ef3b80de633e39d8ab9040cef44127adee97dbc4513df27dacfe`  
		Last Modified: Sat, 16 May 2020 04:26:53 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8cb2b90d45f90f3bdfb841b4a1399ff3a1b0a835e54664ee375ef309ff4c4398
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3776968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fffbb615827376dda1ad45bce22763d7cdc858675e4eafc55deb2d134f813338`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 29 Jul 2020 22:41:42 GMT
COPY file:67a03d7df05756de9c16c4cd22dfaf6ed9cc9a43b78a90ebfaa81ee7ebbc7abf in /nats-server 
# Wed, 29 Jul 2020 22:41:43 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 29 Jul 2020 22:41:44 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 22:41:44 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 29 Jul 2020 22:41:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:39a183ba93759b5fab08b0cb81f1f1a4c9f5a95c3746b031082c6bc3a57441b3`  
		Last Modified: Wed, 29 Jul 2020 22:42:18 GMT  
		Size: 3.8 MB (3776492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a510a0d87b5b915212ee2a5e5d877dced1c30164c0e82d6e60951d00374fe7`  
		Last Modified: Wed, 29 Jul 2020 22:42:17 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:d3e9d8a5a0ad31f0845175c1071e35cea4ac4ebb849c16526e0664a3c0918608
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `nats:nanoserver` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats@sha256:00f69dcad2cdf6b3da43ef4701091ca04d3f35b2ec80c666554d49e5684258d8
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (104957159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edebc41e62feb1ccc604f2e015421dd2e938344719a06d92981822566271a91b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Jul 2020 13:50:07 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jul 2020 15:05:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 15:05:16 GMT
RUN cmd /S /C #(nop) COPY file:18561b827240029ad80d0e3d25142efae62905c30cc520fc37cfc68e7d889848 in C:\nats-server.exe 
# Wed, 15 Jul 2020 15:05:18 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jul 2020 15:05:18 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Jul 2020 15:05:19 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jul 2020 15:05:20 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:dc95608099543221ef539391bfece5c1ce37b97af9da457f5990349cab028a12`  
		Size: 100.9 MB (100895619 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5f0c27d781c53928c03429d5b34e0f49fc26b7e7c996c1d9a2a8474162eade60`  
		Last Modified: Wed, 15 Jul 2020 15:09:50 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10a270f5d0666930958ddfeac073712f678d77b5a05a08210012ada454204077`  
		Last Modified: Wed, 15 Jul 2020 15:10:00 GMT  
		Size: 4.1 MB (4056451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b5e48167a563124481e83cd3f3e3ca1bd3ea8f52b9e52dc9b4982e98a21d7d`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 1.5 KB (1470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64aecdf43c40f563833e5ad1c027bb2e67c1b0c51bb2ab795b99df1f4c2f26f`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 930.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:accd609b6f7304740da44e2a7331717a73ec3f94a35c25198a189b81bd84e204`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 928.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84a11ddf5d09a44b078d904b91df1cd82bf2a0cefb6ec9f52761f36fcf23f54`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:d3e9d8a5a0ad31f0845175c1071e35cea4ac4ebb849c16526e0664a3c0918608
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats@sha256:00f69dcad2cdf6b3da43ef4701091ca04d3f35b2ec80c666554d49e5684258d8
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (104957159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edebc41e62feb1ccc604f2e015421dd2e938344719a06d92981822566271a91b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Jul 2020 13:50:07 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jul 2020 15:05:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 15:05:16 GMT
RUN cmd /S /C #(nop) COPY file:18561b827240029ad80d0e3d25142efae62905c30cc520fc37cfc68e7d889848 in C:\nats-server.exe 
# Wed, 15 Jul 2020 15:05:18 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jul 2020 15:05:18 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Jul 2020 15:05:19 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jul 2020 15:05:20 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:dc95608099543221ef539391bfece5c1ce37b97af9da457f5990349cab028a12`  
		Size: 100.9 MB (100895619 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5f0c27d781c53928c03429d5b34e0f49fc26b7e7c996c1d9a2a8474162eade60`  
		Last Modified: Wed, 15 Jul 2020 15:09:50 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10a270f5d0666930958ddfeac073712f678d77b5a05a08210012ada454204077`  
		Last Modified: Wed, 15 Jul 2020 15:10:00 GMT  
		Size: 4.1 MB (4056451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b5e48167a563124481e83cd3f3e3ca1bd3ea8f52b9e52dc9b4982e98a21d7d`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 1.5 KB (1470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64aecdf43c40f563833e5ad1c027bb2e67c1b0c51bb2ab795b99df1f4c2f26f`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 930.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:accd609b6f7304740da44e2a7331717a73ec3f94a35c25198a189b81bd84e204`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 928.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84a11ddf5d09a44b078d904b91df1cd82bf2a0cefb6ec9f52761f36fcf23f54`  
		Last Modified: Wed, 15 Jul 2020 15:09:47 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:7a3219e049b4d8b10a7ff389fa689c8d08d5732fe37dcf9c5a72fda463d6c6ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:6aace730d886f9719841c60ec11f826e494b8fcc631378b32f5e01ca32d87ab9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4087969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e93a56bc1852bb18d91f1741edde016c59b49c92f7ad91960d583ee0486ebf3`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 16 May 2020 09:47:58 GMT
COPY file:27ab63fb5115ca3cb7456a256d6d6dab7ba864d8806821652fbe569f4f845df5 in /nats-server 
# Sat, 16 May 2020 09:47:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 16 May 2020 09:47:59 GMT
EXPOSE 4222 6222 8222
# Sat, 16 May 2020 09:47:59 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 16 May 2020 09:47:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b509577c042697add820579de13ceed535b1c02ec7fa460b892d6c63941390a7`  
		Last Modified: Sat, 16 May 2020 09:48:21 GMT  
		Size: 4.1 MB (4087491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ce65065eb7bc6684476be5937b3d0d4046e7cc7241bc5017d70488d0edbfe3`  
		Last Modified: Sat, 16 May 2020 09:48:20 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:e8b59aabb2b6838ced59a3125ba4216cc8a4d0622f8b8c1e9e40fb30cd63a135
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3796375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8116ee7998ff454ed4eaa153438504925828993f56f26fb96fd11b31c9dc2128`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 15 May 2020 19:53:42 GMT
COPY file:9951c1b4ae20021f4d6efd6c039d0f0d0044470572e81beae625f15ffa13d2f1 in /nats-server 
# Fri, 15 May 2020 19:53:43 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 15 May 2020 19:53:44 GMT
EXPOSE 4222 6222 8222
# Fri, 15 May 2020 19:53:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 15 May 2020 19:53:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7976dc3d59fddf78c4ca25d0692135431e63b9fb744ae2c3d02b7a8214b5bfd9`  
		Last Modified: Fri, 15 May 2020 19:54:21 GMT  
		Size: 3.8 MB (3795898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b520f7415a5fab1b4a83eb7a8259e321475f75f5b06bfe95493b598c9ee9f4`  
		Last Modified: Fri, 15 May 2020 19:54:20 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:707f02b7c81a3f071abba9ce0a74b1cf0bf7a664e0220ab6cae112f2721a24bf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3792273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d2f2220669ef3621c45d5e4fd8460e7378e258044eb57003584ce55db5bdd9b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 16 May 2020 04:26:09 GMT
COPY file:3320edcd8f0db9551469809c752244493d1c6cf3be0287714c8a507e339283b2 in /nats-server 
# Sat, 16 May 2020 04:26:09 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 16 May 2020 04:26:11 GMT
EXPOSE 4222 6222 8222
# Sat, 16 May 2020 04:26:12 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 16 May 2020 04:26:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7ceefb66163b74f9719728ecace35bd406e85998a252d90c9e07a02582c7b6f1`  
		Last Modified: Sat, 16 May 2020 04:26:55 GMT  
		Size: 3.8 MB (3791795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db182fe235e1ef3b80de633e39d8ab9040cef44127adee97dbc4513df27dacfe`  
		Last Modified: Sat, 16 May 2020 04:26:53 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8cb2b90d45f90f3bdfb841b4a1399ff3a1b0a835e54664ee375ef309ff4c4398
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3776968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fffbb615827376dda1ad45bce22763d7cdc858675e4eafc55deb2d134f813338`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 29 Jul 2020 22:41:42 GMT
COPY file:67a03d7df05756de9c16c4cd22dfaf6ed9cc9a43b78a90ebfaa81ee7ebbc7abf in /nats-server 
# Wed, 29 Jul 2020 22:41:43 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 29 Jul 2020 22:41:44 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 22:41:44 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 29 Jul 2020 22:41:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:39a183ba93759b5fab08b0cb81f1f1a4c9f5a95c3746b031082c6bc3a57441b3`  
		Last Modified: Wed, 29 Jul 2020 22:42:18 GMT  
		Size: 3.8 MB (3776492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a510a0d87b5b915212ee2a5e5d877dced1c30164c0e82d6e60951d00374fe7`  
		Last Modified: Wed, 29 Jul 2020 22:42:17 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:59a9a5745643d652dd6d49be5d422a2270a2539f6dfa398ba219d78c00c701e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64
	-	windows version 10.0.14393.3808; amd64

### `nats:windowsservercore` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats@sha256:84ed3b1eb1e35102dff57509d666e9ae99f4fd0a492b9410b473bedda4aeebdf
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2328185203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8d69d5e23b4cff9ad8df708d4059e6525b91686ad490775e104e6c06b863457`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Wed, 15 Jul 2020 12:15:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jul 2020 15:03:03 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 15:03:03 GMT
ENV NATS_SERVER=2.1.7
# Wed, 15 Jul 2020 15:03:04 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.7/nats-server-v2.1.7-windows-amd64.zip
# Wed, 29 Jul 2020 23:14:26 GMT
ENV GIT_DOWNLOAD_SHA256=1e1ad5c00929cc145341fd65f8b0a41a38e942b9b9fd9fdb0216c47654afdc8f
# Wed, 29 Jul 2020 23:15:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 29 Jul 2020 23:16:49 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 29 Jul 2020 23:16:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 29 Jul 2020 23:16:54 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 23:16:55 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 29 Jul 2020 23:16:56 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1cc883a0e3509a474bb32f3c40411bf86219325ae9710e25a5dcce6b44eef357`  
		Last Modified: Wed, 15 Jul 2020 14:32:06 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dd35c9a62007b6ded1ca968562be97de62ea3e2b3c7db85f4a50baaa9efecb`  
		Last Modified: Wed, 15 Jul 2020 15:09:33 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5789d32300712f2fa8b6564efe911f5f523cf150f1fde2bf8d6deedbb56feb4`  
		Last Modified: Wed, 15 Jul 2020 15:09:32 GMT  
		Size: 1.1 KB (1105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b62b1740ff37517c10b8b8bfae73367d0c5538cf934392846eea648031c1857`  
		Last Modified: Wed, 15 Jul 2020 15:09:31 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c765e0c4aba82f5140dd325bb9fc2dc97095f673b4d88039867aecc92e331f5e`  
		Last Modified: Wed, 29 Jul 2020 23:21:23 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9dfd44060c9c9e79fca23ba4227434b55a5a3353c7a32ba8140fa252af2631f`  
		Last Modified: Wed, 29 Jul 2020 23:21:24 GMT  
		Size: 4.8 MB (4803853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011be3335c53769b99af80accd8e25f40172d44bc0e20780c88f1ab787bbf09e`  
		Last Modified: Wed, 29 Jul 2020 23:21:24 GMT  
		Size: 13.2 MB (13178319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f913f5767f1c088f27134bdefc531acacd106610ce085ef7ca5470fdeda55e80`  
		Last Modified: Wed, 29 Jul 2020 23:21:20 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8436f3f54d22f495452cdb61489bf5833c2cda6a2e6012c732b2c8ffbc72262f`  
		Last Modified: Wed, 29 Jul 2020 23:21:20 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12724c1ab2196db2d2cd8bff6069b1ea932e514cd5473240dd515f50361e4fa`  
		Last Modified: Wed, 29 Jul 2020 23:21:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419a5e47094ff5e8a8cb733bf81fcd97e46b00a5b62b9cbcd5993a66942a7e7e`  
		Last Modified: Wed, 29 Jul 2020 23:21:20 GMT  
		Size: 1.1 KB (1100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:windowsservercore` - windows version 10.0.14393.3808; amd64

```console
$ docker pull nats@sha256:9145e80ebf209b601e34e199defd755bf43a5b09f674ece13c4c6299b21d4870
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5756757168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a3c13889118f6f6c65e859be772b7b0cb7e0497de0a2326a3b54c097daa6670`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Jul 2020 21:05:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Jul 2020 12:24:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jul 2020 15:05:26 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 15:05:27 GMT
ENV NATS_SERVER=2.1.7
# Wed, 15 Jul 2020 15:05:28 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.7/nats-server-v2.1.7-windows-amd64.zip
# Wed, 29 Jul 2020 23:17:15 GMT
ENV GIT_DOWNLOAD_SHA256=1e1ad5c00929cc145341fd65f8b0a41a38e942b9b9fd9fdb0216c47654afdc8f
# Wed, 29 Jul 2020 23:18:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 29 Jul 2020 23:20:43 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 29 Jul 2020 23:20:45 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 29 Jul 2020 23:20:46 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 23:20:47 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 29 Jul 2020 23:20:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:802c4beb8b091968ccf1bb4a853ded7955ddb79e6f8775a5155cb5ed07dcbcab`  
		Size: 1.7 GB (1667476199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3393eecaf56a66035ab178b379bacf81d30373b630b34b2973501f259aadb0f6`  
		Last Modified: Wed, 15 Jul 2020 14:32:38 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1430ee68db5fe3026683f1b7c74f31ae748da71bf8ad611efede726e9e036b1`  
		Last Modified: Wed, 15 Jul 2020 15:10:21 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae29b1720308eb8710d921cefbc8979061e4535b6276b35b3d471e08a09e7af`  
		Last Modified: Wed, 15 Jul 2020 15:10:19 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a76213345cac0ca18badbc3c8262b6973e3457484fdcb9af380fa4de2c64ea`  
		Last Modified: Wed, 15 Jul 2020 15:10:19 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2713fe8ba40241bc8ef85e6795703e42f101f0ab81d143357c549a03c4b00c`  
		Last Modified: Wed, 29 Jul 2020 23:21:44 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b8f23b09829f938cc622501d4059590b050bc95a7fb4c5d2e337e423af1e23`  
		Last Modified: Wed, 29 Jul 2020 23:21:46 GMT  
		Size: 5.4 MB (5391705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0857d1594c42a8ff34ec0fc99b717f343d2e6dcdcb980e3b54621a8127ecf4a`  
		Last Modified: Wed, 29 Jul 2020 23:21:57 GMT  
		Size: 13.9 MB (13892511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7afe295ad113f1145078cde44f86ce197d64aa5ceb92784bf4c60ff710b95256`  
		Last Modified: Wed, 29 Jul 2020 23:21:41 GMT  
		Size: 1.7 KB (1683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9b54006dba8cc76bc2325f78d0377969e727070a8f9069e26090b7a4e18f36`  
		Last Modified: Wed, 29 Jul 2020 23:21:41 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97bb5b91db82c40b2b26f5fcc7a1e07fce677242cd70722fbe2d3256e4548dfc`  
		Last Modified: Wed, 29 Jul 2020 23:21:42 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58919d245b3713c0a29f1039075f368c82d09514f57a595cade8fae1010c7847`  
		Last Modified: Wed, 29 Jul 2020 23:21:42 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:f9351e549406b5be23d79a960a8188aae30b521a25b98855bcf4ad382d0446e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats@sha256:84ed3b1eb1e35102dff57509d666e9ae99f4fd0a492b9410b473bedda4aeebdf
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2328185203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8d69d5e23b4cff9ad8df708d4059e6525b91686ad490775e104e6c06b863457`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Wed, 15 Jul 2020 12:15:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jul 2020 15:03:03 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 15:03:03 GMT
ENV NATS_SERVER=2.1.7
# Wed, 15 Jul 2020 15:03:04 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.7/nats-server-v2.1.7-windows-amd64.zip
# Wed, 29 Jul 2020 23:14:26 GMT
ENV GIT_DOWNLOAD_SHA256=1e1ad5c00929cc145341fd65f8b0a41a38e942b9b9fd9fdb0216c47654afdc8f
# Wed, 29 Jul 2020 23:15:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 29 Jul 2020 23:16:49 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 29 Jul 2020 23:16:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 29 Jul 2020 23:16:54 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 23:16:55 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 29 Jul 2020 23:16:56 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1cc883a0e3509a474bb32f3c40411bf86219325ae9710e25a5dcce6b44eef357`  
		Last Modified: Wed, 15 Jul 2020 14:32:06 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dd35c9a62007b6ded1ca968562be97de62ea3e2b3c7db85f4a50baaa9efecb`  
		Last Modified: Wed, 15 Jul 2020 15:09:33 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5789d32300712f2fa8b6564efe911f5f523cf150f1fde2bf8d6deedbb56feb4`  
		Last Modified: Wed, 15 Jul 2020 15:09:32 GMT  
		Size: 1.1 KB (1105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b62b1740ff37517c10b8b8bfae73367d0c5538cf934392846eea648031c1857`  
		Last Modified: Wed, 15 Jul 2020 15:09:31 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c765e0c4aba82f5140dd325bb9fc2dc97095f673b4d88039867aecc92e331f5e`  
		Last Modified: Wed, 29 Jul 2020 23:21:23 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9dfd44060c9c9e79fca23ba4227434b55a5a3353c7a32ba8140fa252af2631f`  
		Last Modified: Wed, 29 Jul 2020 23:21:24 GMT  
		Size: 4.8 MB (4803853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011be3335c53769b99af80accd8e25f40172d44bc0e20780c88f1ab787bbf09e`  
		Last Modified: Wed, 29 Jul 2020 23:21:24 GMT  
		Size: 13.2 MB (13178319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f913f5767f1c088f27134bdefc531acacd106610ce085ef7ca5470fdeda55e80`  
		Last Modified: Wed, 29 Jul 2020 23:21:20 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8436f3f54d22f495452cdb61489bf5833c2cda6a2e6012c732b2c8ffbc72262f`  
		Last Modified: Wed, 29 Jul 2020 23:21:20 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12724c1ab2196db2d2cd8bff6069b1ea932e514cd5473240dd515f50361e4fa`  
		Last Modified: Wed, 29 Jul 2020 23:21:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419a5e47094ff5e8a8cb733bf81fcd97e46b00a5b62b9cbcd5993a66942a7e7e`  
		Last Modified: Wed, 29 Jul 2020 23:21:20 GMT  
		Size: 1.1 KB (1100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:f405d1c17c29cd33ba2762684ab3ee983dbaafd8df62ef7b12fa78b3ad6b7d3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3808; amd64

### `nats:windowsservercore-ltsc2016` - windows version 10.0.14393.3808; amd64

```console
$ docker pull nats@sha256:9145e80ebf209b601e34e199defd755bf43a5b09f674ece13c4c6299b21d4870
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5756757168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a3c13889118f6f6c65e859be772b7b0cb7e0497de0a2326a3b54c097daa6670`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Jul 2020 21:05:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Jul 2020 12:24:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jul 2020 15:05:26 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 15:05:27 GMT
ENV NATS_SERVER=2.1.7
# Wed, 15 Jul 2020 15:05:28 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.7/nats-server-v2.1.7-windows-amd64.zip
# Wed, 29 Jul 2020 23:17:15 GMT
ENV GIT_DOWNLOAD_SHA256=1e1ad5c00929cc145341fd65f8b0a41a38e942b9b9fd9fdb0216c47654afdc8f
# Wed, 29 Jul 2020 23:18:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 29 Jul 2020 23:20:43 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 29 Jul 2020 23:20:45 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 29 Jul 2020 23:20:46 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Jul 2020 23:20:47 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 29 Jul 2020 23:20:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:802c4beb8b091968ccf1bb4a853ded7955ddb79e6f8775a5155cb5ed07dcbcab`  
		Size: 1.7 GB (1667476199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3393eecaf56a66035ab178b379bacf81d30373b630b34b2973501f259aadb0f6`  
		Last Modified: Wed, 15 Jul 2020 14:32:38 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1430ee68db5fe3026683f1b7c74f31ae748da71bf8ad611efede726e9e036b1`  
		Last Modified: Wed, 15 Jul 2020 15:10:21 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae29b1720308eb8710d921cefbc8979061e4535b6276b35b3d471e08a09e7af`  
		Last Modified: Wed, 15 Jul 2020 15:10:19 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a76213345cac0ca18badbc3c8262b6973e3457484fdcb9af380fa4de2c64ea`  
		Last Modified: Wed, 15 Jul 2020 15:10:19 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2713fe8ba40241bc8ef85e6795703e42f101f0ab81d143357c549a03c4b00c`  
		Last Modified: Wed, 29 Jul 2020 23:21:44 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b8f23b09829f938cc622501d4059590b050bc95a7fb4c5d2e337e423af1e23`  
		Last Modified: Wed, 29 Jul 2020 23:21:46 GMT  
		Size: 5.4 MB (5391705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0857d1594c42a8ff34ec0fc99b717f343d2e6dcdcb980e3b54621a8127ecf4a`  
		Last Modified: Wed, 29 Jul 2020 23:21:57 GMT  
		Size: 13.9 MB (13892511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7afe295ad113f1145078cde44f86ce197d64aa5ceb92784bf4c60ff710b95256`  
		Last Modified: Wed, 29 Jul 2020 23:21:41 GMT  
		Size: 1.7 KB (1683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9b54006dba8cc76bc2325f78d0377969e727070a8f9069e26090b7a4e18f36`  
		Last Modified: Wed, 29 Jul 2020 23:21:41 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97bb5b91db82c40b2b26f5fcc7a1e07fce677242cd70722fbe2d3256e4548dfc`  
		Last Modified: Wed, 29 Jul 2020 23:21:42 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58919d245b3713c0a29f1039075f368c82d09514f57a595cade8fae1010c7847`  
		Last Modified: Wed, 29 Jul 2020 23:21:42 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
