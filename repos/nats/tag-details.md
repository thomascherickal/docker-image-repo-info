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
$ docker pull nats@sha256:85589e53092232c686097acfdc3828ac0e20a562d63c5d0f0e7dfceade6fad49
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
$ docker pull nats@sha256:85589e53092232c686097acfdc3828ac0e20a562d63c5d0f0e7dfceade6fad49
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
$ docker pull nats@sha256:3817ae87ac429a46599e90372c0d61fc47524881af5c8060e659bf43bd0b9b95
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
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
$ docker pull nats@sha256:966bafc8fed140348df882cdfce8c6ec0ae84246af19ba2dc4c44192a330c18b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats:2.1.7-alpine` - linux; amd64

```console
$ docker pull nats@sha256:afc307dec8317bf0bee1c448f05a0e928635b5115f7e21890b9b6885de27e3e9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7204657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d55057d2200ae8b71e69d563361a7c078b9959e2df3b828c14c5c852d7ee85e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Sat, 16 May 2020 09:47:11 GMT
ENV NATS_SERVER=2.1.7
# Sat, 16 May 2020 09:47:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 16 May 2020 09:47:13 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 06 Jun 2020 02:20:01 GMT
COPY file:e90698d1d7a93a6e661321ceff0cc34f74523d472fad403fb682bb5d43b6a785 in /usr/local/bin 
# Sat, 06 Jun 2020 02:20:01 GMT
EXPOSE 4222 6222 8222
# Sat, 06 Jun 2020 02:20:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Jun 2020 02:20:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eaf9939fdcf9c33e5b47fb1d09e4994e32b77b1ae5f3e396ad0bd90449b3e99`  
		Last Modified: Sat, 16 May 2020 09:48:12 GMT  
		Size: 4.4 MB (4390368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd216f8fa68b80c5b89b67bdf4aeedbe6d445ea495e9af5b07ff07c932d3478e`  
		Last Modified: Sat, 16 May 2020 09:48:12 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f04bcbae80555bc5a339111607737c8a22387e1ef9bdde9cd8cf59f7a7d2edd9`  
		Last Modified: Sat, 06 Jun 2020 02:20:38 GMT  
		Size: 444.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.7-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:92881cbdb3078b8a4456e1a45a34d9272357c7ab82ece5a9f96a517176aaaf9d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6720097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c294dd603de46043cfee2c1d0d9c7bb5783559f5d94b3e7e370d07d9ed3c0b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Fri, 15 May 2020 19:50:13 GMT
ENV NATS_SERVER=2.1.7
# Fri, 15 May 2020 19:50:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 15 May 2020 19:50:25 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 06 Jun 2020 02:50:21 GMT
COPY file:e90698d1d7a93a6e661321ceff0cc34f74523d472fad403fb682bb5d43b6a785 in /usr/local/bin 
# Sat, 06 Jun 2020 02:50:23 GMT
EXPOSE 4222 6222 8222
# Sat, 06 Jun 2020 02:50:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Jun 2020 02:50:27 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2da3e9f49b6c3ee3b36761ca52b69d8d5eef0937cb74cd8fddbb46850e21eea`  
		Last Modified: Fri, 15 May 2020 19:54:08 GMT  
		Size: 4.1 MB (4099154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf99cc6797b449693d5c09898c063ff989f060f8aec84ee465a356d2a45323c`  
		Last Modified: Fri, 15 May 2020 19:54:06 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c5786c0476f10cbaaed737392af53825da728437020325ccbd384cdf53b100`  
		Last Modified: Sat, 06 Jun 2020 02:57:26 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.7-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:2ce1841a96e019cbad94dc856fc41df447c6bfa53cda82adb93e431dc4bcc652
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6516346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:353d1047af5e64a22156c535460a8883c63c3bb196aa977c1a8a96c09f716163`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Sat, 16 May 2020 04:17:01 GMT
ENV NATS_SERVER=2.1.7
# Sat, 16 May 2020 04:17:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 16 May 2020 04:17:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 06 Jun 2020 02:59:06 GMT
COPY file:e90698d1d7a93a6e661321ceff0cc34f74523d472fad403fb682bb5d43b6a785 in /usr/local/bin 
# Sat, 06 Jun 2020 02:59:06 GMT
EXPOSE 4222 6222 8222
# Sat, 06 Jun 2020 02:59:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Jun 2020 02:59:08 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2111cd33403a7683737ec41dba39b7fd69d4d4c770b66eff350253601018f65`  
		Last Modified: Sat, 16 May 2020 04:26:40 GMT  
		Size: 4.1 MB (4093275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab45b7c0f143ec333947ad8048d647c2b8bc669596d874e502e79ee4e74e0f3`  
		Last Modified: Sat, 16 May 2020 04:26:40 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967546c6e8edd236036de77257c69742e6740d1e64cd55cd2905478fcfde9552`  
		Last Modified: Sat, 06 Jun 2020 03:09:08 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.7-alpine3.11`

```console
$ docker pull nats@sha256:966bafc8fed140348df882cdfce8c6ec0ae84246af19ba2dc4c44192a330c18b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats:2.1.7-alpine3.11` - linux; amd64

```console
$ docker pull nats@sha256:afc307dec8317bf0bee1c448f05a0e928635b5115f7e21890b9b6885de27e3e9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7204657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d55057d2200ae8b71e69d563361a7c078b9959e2df3b828c14c5c852d7ee85e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Sat, 16 May 2020 09:47:11 GMT
ENV NATS_SERVER=2.1.7
# Sat, 16 May 2020 09:47:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 16 May 2020 09:47:13 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 06 Jun 2020 02:20:01 GMT
COPY file:e90698d1d7a93a6e661321ceff0cc34f74523d472fad403fb682bb5d43b6a785 in /usr/local/bin 
# Sat, 06 Jun 2020 02:20:01 GMT
EXPOSE 4222 6222 8222
# Sat, 06 Jun 2020 02:20:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Jun 2020 02:20:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eaf9939fdcf9c33e5b47fb1d09e4994e32b77b1ae5f3e396ad0bd90449b3e99`  
		Last Modified: Sat, 16 May 2020 09:48:12 GMT  
		Size: 4.4 MB (4390368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd216f8fa68b80c5b89b67bdf4aeedbe6d445ea495e9af5b07ff07c932d3478e`  
		Last Modified: Sat, 16 May 2020 09:48:12 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f04bcbae80555bc5a339111607737c8a22387e1ef9bdde9cd8cf59f7a7d2edd9`  
		Last Modified: Sat, 06 Jun 2020 02:20:38 GMT  
		Size: 444.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.7-alpine3.11` - linux; arm variant v6

```console
$ docker pull nats@sha256:92881cbdb3078b8a4456e1a45a34d9272357c7ab82ece5a9f96a517176aaaf9d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6720097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c294dd603de46043cfee2c1d0d9c7bb5783559f5d94b3e7e370d07d9ed3c0b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Fri, 15 May 2020 19:50:13 GMT
ENV NATS_SERVER=2.1.7
# Fri, 15 May 2020 19:50:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 15 May 2020 19:50:25 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 06 Jun 2020 02:50:21 GMT
COPY file:e90698d1d7a93a6e661321ceff0cc34f74523d472fad403fb682bb5d43b6a785 in /usr/local/bin 
# Sat, 06 Jun 2020 02:50:23 GMT
EXPOSE 4222 6222 8222
# Sat, 06 Jun 2020 02:50:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Jun 2020 02:50:27 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2da3e9f49b6c3ee3b36761ca52b69d8d5eef0937cb74cd8fddbb46850e21eea`  
		Last Modified: Fri, 15 May 2020 19:54:08 GMT  
		Size: 4.1 MB (4099154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf99cc6797b449693d5c09898c063ff989f060f8aec84ee465a356d2a45323c`  
		Last Modified: Fri, 15 May 2020 19:54:06 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c5786c0476f10cbaaed737392af53825da728437020325ccbd384cdf53b100`  
		Last Modified: Sat, 06 Jun 2020 02:57:26 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.7-alpine3.11` - linux; arm variant v7

```console
$ docker pull nats@sha256:2ce1841a96e019cbad94dc856fc41df447c6bfa53cda82adb93e431dc4bcc652
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6516346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:353d1047af5e64a22156c535460a8883c63c3bb196aa977c1a8a96c09f716163`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Sat, 16 May 2020 04:17:01 GMT
ENV NATS_SERVER=2.1.7
# Sat, 16 May 2020 04:17:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 16 May 2020 04:17:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 06 Jun 2020 02:59:06 GMT
COPY file:e90698d1d7a93a6e661321ceff0cc34f74523d472fad403fb682bb5d43b6a785 in /usr/local/bin 
# Sat, 06 Jun 2020 02:59:06 GMT
EXPOSE 4222 6222 8222
# Sat, 06 Jun 2020 02:59:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Jun 2020 02:59:08 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2111cd33403a7683737ec41dba39b7fd69d4d4c770b66eff350253601018f65`  
		Last Modified: Sat, 16 May 2020 04:26:40 GMT  
		Size: 4.1 MB (4093275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab45b7c0f143ec333947ad8048d647c2b8bc669596d874e502e79ee4e74e0f3`  
		Last Modified: Sat, 16 May 2020 04:26:40 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967546c6e8edd236036de77257c69742e6740d1e64cd55cd2905478fcfde9552`  
		Last Modified: Sat, 06 Jun 2020 03:09:08 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.7-linux`

```console
$ docker pull nats@sha256:4579aa17c12c15c7e6db8e0f9f02260683d7e5efe20a2501f5d569c9ed98d672
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

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
$ docker pull nats@sha256:4579aa17c12c15c7e6db8e0f9f02260683d7e5efe20a2501f5d569c9ed98d672
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

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

## `nats:2.1.7-windowsservercore`

```console
$ docker pull nats@sha256:d8b4027afa12bde158081e46da01e775d11b8281d7bfdd6dc418fab46607afc2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64
	-	windows version 10.0.14393.3808; amd64

### `nats:2.1.7-windowsservercore` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats@sha256:853c70bfa92057d5ff5cce9d40f23822b02351d1f196dc2aeee6f8b1d6b4e01e
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2328178778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de952a8a6f9f77294e1eb06c5e736386fc96f24575bd3d472aa6ed634683e147`
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
# Wed, 15 Jul 2020 15:03:42 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jul 2020 15:04:57 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Jul 2020 15:04:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jul 2020 15:05:00 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Jul 2020 15:05:01 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jul 2020 15:05:02 GMT
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
	-	`sha256:3cc0292f299542ec593d4cf8b4cae1422da5920a655cc145378a1f343bb4b82a`  
		Last Modified: Wed, 15 Jul 2020 15:09:33 GMT  
		Size: 4.8 MB (4800276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377ab72fb858121eb624585d89868fd66349f054e41a7feb0d6a8f9dcce7621f`  
		Last Modified: Wed, 15 Jul 2020 15:09:32 GMT  
		Size: 13.2 MB (13176530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b414836d9ec08b0beeed7d90882777bb3872b65a528d27eff46d11224367eb4`  
		Last Modified: Wed, 15 Jul 2020 15:09:29 GMT  
		Size: 1.7 KB (1699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218276e4e5be6f495bd072ca818cc3126a8e1de83e81cf3aac0e434a7cf998d3`  
		Last Modified: Wed, 15 Jul 2020 15:09:29 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554b66195d7e4135f672a2c5c88017b81cb523a28b19b3b01d7dc0cd0ac08b29`  
		Last Modified: Wed, 15 Jul 2020 15:09:29 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f992754834fc067d9ef4edb88b29e743cfb3feda4ebc33340af1fa7117fc762`  
		Last Modified: Wed, 15 Jul 2020 15:09:29 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.7-windowsservercore` - windows version 10.0.14393.3808; amd64

```console
$ docker pull nats@sha256:43b41d3085f47eee811b28506b54ff7c29da295345d214565a6d4f6e301bf396
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5756765076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9ff7196afcabade265df8afe613aa8fc6dcc055ed374eb60e92aa93e4978b7f`
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
# Wed, 15 Jul 2020 15:06:44 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jul 2020 15:08:49 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Jul 2020 15:08:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jul 2020 15:08:52 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Jul 2020 15:08:53 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jul 2020 15:08:54 GMT
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
	-	`sha256:0584eb6b5415d012501558a2dcc9f68bf8d1c0d96ab16abc0658534ca083763f`  
		Last Modified: Wed, 15 Jul 2020 15:10:20 GMT  
		Size: 5.4 MB (5361288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52eab21ed3b97aead8a8bafd9d07b9ac114cc1ccd2e5cfa6c2afac7401e38442`  
		Last Modified: Wed, 15 Jul 2020 15:10:22 GMT  
		Size: 13.9 MB (13931973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c1e79456e304bb7e24066e10b332b7da148fd981c19c151146e0498e09dbff`  
		Last Modified: Wed, 15 Jul 2020 15:10:16 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead3b72b2add53883aa3e0b7be3eb60a9f37fe43c4457e036da44a70e8b9cb23`  
		Last Modified: Wed, 15 Jul 2020 15:10:16 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3014d80ec0460dda49e4bf323f74bdf7b51b76cf368b453d59eb96443d61d1d8`  
		Last Modified: Wed, 15 Jul 2020 15:10:17 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aca79d7cfc3c47963f81e8c6f692cb6ffada2b4dc42fed607734a1446029e5f`  
		Last Modified: Wed, 15 Jul 2020 15:10:16 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.7-windowsservercore-1809`

```console
$ docker pull nats@sha256:666bfe8f181744c240647e0af2fc10ac2dfa90a7dfdf3e0cfe368f8d7d44087c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `nats:2.1.7-windowsservercore-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats@sha256:853c70bfa92057d5ff5cce9d40f23822b02351d1f196dc2aeee6f8b1d6b4e01e
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2328178778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de952a8a6f9f77294e1eb06c5e736386fc96f24575bd3d472aa6ed634683e147`
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
# Wed, 15 Jul 2020 15:03:42 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jul 2020 15:04:57 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Jul 2020 15:04:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jul 2020 15:05:00 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Jul 2020 15:05:01 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jul 2020 15:05:02 GMT
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
	-	`sha256:3cc0292f299542ec593d4cf8b4cae1422da5920a655cc145378a1f343bb4b82a`  
		Last Modified: Wed, 15 Jul 2020 15:09:33 GMT  
		Size: 4.8 MB (4800276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377ab72fb858121eb624585d89868fd66349f054e41a7feb0d6a8f9dcce7621f`  
		Last Modified: Wed, 15 Jul 2020 15:09:32 GMT  
		Size: 13.2 MB (13176530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b414836d9ec08b0beeed7d90882777bb3872b65a528d27eff46d11224367eb4`  
		Last Modified: Wed, 15 Jul 2020 15:09:29 GMT  
		Size: 1.7 KB (1699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218276e4e5be6f495bd072ca818cc3126a8e1de83e81cf3aac0e434a7cf998d3`  
		Last Modified: Wed, 15 Jul 2020 15:09:29 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554b66195d7e4135f672a2c5c88017b81cb523a28b19b3b01d7dc0cd0ac08b29`  
		Last Modified: Wed, 15 Jul 2020 15:09:29 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f992754834fc067d9ef4edb88b29e743cfb3feda4ebc33340af1fa7117fc762`  
		Last Modified: Wed, 15 Jul 2020 15:09:29 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.7-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:ce555ef8cbfebaaa0aa85b82cbccc3c230a067d2bddb3ab8a82e2ff094dc3bd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3808; amd64

### `nats:2.1.7-windowsservercore-ltsc2016` - windows version 10.0.14393.3808; amd64

```console
$ docker pull nats@sha256:43b41d3085f47eee811b28506b54ff7c29da295345d214565a6d4f6e301bf396
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5756765076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9ff7196afcabade265df8afe613aa8fc6dcc055ed374eb60e92aa93e4978b7f`
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
# Wed, 15 Jul 2020 15:06:44 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jul 2020 15:08:49 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Jul 2020 15:08:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jul 2020 15:08:52 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Jul 2020 15:08:53 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jul 2020 15:08:54 GMT
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
	-	`sha256:0584eb6b5415d012501558a2dcc9f68bf8d1c0d96ab16abc0658534ca083763f`  
		Last Modified: Wed, 15 Jul 2020 15:10:20 GMT  
		Size: 5.4 MB (5361288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52eab21ed3b97aead8a8bafd9d07b9ac114cc1ccd2e5cfa6c2afac7401e38442`  
		Last Modified: Wed, 15 Jul 2020 15:10:22 GMT  
		Size: 13.9 MB (13931973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c1e79456e304bb7e24066e10b332b7da148fd981c19c151146e0498e09dbff`  
		Last Modified: Wed, 15 Jul 2020 15:10:16 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead3b72b2add53883aa3e0b7be3eb60a9f37fe43c4457e036da44a70e8b9cb23`  
		Last Modified: Wed, 15 Jul 2020 15:10:16 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3014d80ec0460dda49e4bf323f74bdf7b51b76cf368b453d59eb96443d61d1d8`  
		Last Modified: Wed, 15 Jul 2020 15:10:17 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aca79d7cfc3c47963f81e8c6f692cb6ffada2b4dc42fed607734a1446029e5f`  
		Last Modified: Wed, 15 Jul 2020 15:10:16 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-alpine`

```console
$ docker pull nats@sha256:966bafc8fed140348df882cdfce8c6ec0ae84246af19ba2dc4c44192a330c18b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats:2.1-alpine` - linux; amd64

```console
$ docker pull nats@sha256:afc307dec8317bf0bee1c448f05a0e928635b5115f7e21890b9b6885de27e3e9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7204657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d55057d2200ae8b71e69d563361a7c078b9959e2df3b828c14c5c852d7ee85e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Sat, 16 May 2020 09:47:11 GMT
ENV NATS_SERVER=2.1.7
# Sat, 16 May 2020 09:47:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 16 May 2020 09:47:13 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 06 Jun 2020 02:20:01 GMT
COPY file:e90698d1d7a93a6e661321ceff0cc34f74523d472fad403fb682bb5d43b6a785 in /usr/local/bin 
# Sat, 06 Jun 2020 02:20:01 GMT
EXPOSE 4222 6222 8222
# Sat, 06 Jun 2020 02:20:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Jun 2020 02:20:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eaf9939fdcf9c33e5b47fb1d09e4994e32b77b1ae5f3e396ad0bd90449b3e99`  
		Last Modified: Sat, 16 May 2020 09:48:12 GMT  
		Size: 4.4 MB (4390368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd216f8fa68b80c5b89b67bdf4aeedbe6d445ea495e9af5b07ff07c932d3478e`  
		Last Modified: Sat, 16 May 2020 09:48:12 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f04bcbae80555bc5a339111607737c8a22387e1ef9bdde9cd8cf59f7a7d2edd9`  
		Last Modified: Sat, 06 Jun 2020 02:20:38 GMT  
		Size: 444.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:92881cbdb3078b8a4456e1a45a34d9272357c7ab82ece5a9f96a517176aaaf9d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6720097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c294dd603de46043cfee2c1d0d9c7bb5783559f5d94b3e7e370d07d9ed3c0b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Fri, 15 May 2020 19:50:13 GMT
ENV NATS_SERVER=2.1.7
# Fri, 15 May 2020 19:50:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 15 May 2020 19:50:25 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 06 Jun 2020 02:50:21 GMT
COPY file:e90698d1d7a93a6e661321ceff0cc34f74523d472fad403fb682bb5d43b6a785 in /usr/local/bin 
# Sat, 06 Jun 2020 02:50:23 GMT
EXPOSE 4222 6222 8222
# Sat, 06 Jun 2020 02:50:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Jun 2020 02:50:27 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2da3e9f49b6c3ee3b36761ca52b69d8d5eef0937cb74cd8fddbb46850e21eea`  
		Last Modified: Fri, 15 May 2020 19:54:08 GMT  
		Size: 4.1 MB (4099154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf99cc6797b449693d5c09898c063ff989f060f8aec84ee465a356d2a45323c`  
		Last Modified: Fri, 15 May 2020 19:54:06 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c5786c0476f10cbaaed737392af53825da728437020325ccbd384cdf53b100`  
		Last Modified: Sat, 06 Jun 2020 02:57:26 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:2ce1841a96e019cbad94dc856fc41df447c6bfa53cda82adb93e431dc4bcc652
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6516346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:353d1047af5e64a22156c535460a8883c63c3bb196aa977c1a8a96c09f716163`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Sat, 16 May 2020 04:17:01 GMT
ENV NATS_SERVER=2.1.7
# Sat, 16 May 2020 04:17:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 16 May 2020 04:17:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 06 Jun 2020 02:59:06 GMT
COPY file:e90698d1d7a93a6e661321ceff0cc34f74523d472fad403fb682bb5d43b6a785 in /usr/local/bin 
# Sat, 06 Jun 2020 02:59:06 GMT
EXPOSE 4222 6222 8222
# Sat, 06 Jun 2020 02:59:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Jun 2020 02:59:08 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2111cd33403a7683737ec41dba39b7fd69d4d4c770b66eff350253601018f65`  
		Last Modified: Sat, 16 May 2020 04:26:40 GMT  
		Size: 4.1 MB (4093275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab45b7c0f143ec333947ad8048d647c2b8bc669596d874e502e79ee4e74e0f3`  
		Last Modified: Sat, 16 May 2020 04:26:40 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967546c6e8edd236036de77257c69742e6740d1e64cd55cd2905478fcfde9552`  
		Last Modified: Sat, 06 Jun 2020 03:09:08 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-alpine3.11`

```console
$ docker pull nats@sha256:966bafc8fed140348df882cdfce8c6ec0ae84246af19ba2dc4c44192a330c18b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats:2.1-alpine3.11` - linux; amd64

```console
$ docker pull nats@sha256:afc307dec8317bf0bee1c448f05a0e928635b5115f7e21890b9b6885de27e3e9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7204657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d55057d2200ae8b71e69d563361a7c078b9959e2df3b828c14c5c852d7ee85e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Sat, 16 May 2020 09:47:11 GMT
ENV NATS_SERVER=2.1.7
# Sat, 16 May 2020 09:47:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 16 May 2020 09:47:13 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 06 Jun 2020 02:20:01 GMT
COPY file:e90698d1d7a93a6e661321ceff0cc34f74523d472fad403fb682bb5d43b6a785 in /usr/local/bin 
# Sat, 06 Jun 2020 02:20:01 GMT
EXPOSE 4222 6222 8222
# Sat, 06 Jun 2020 02:20:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Jun 2020 02:20:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eaf9939fdcf9c33e5b47fb1d09e4994e32b77b1ae5f3e396ad0bd90449b3e99`  
		Last Modified: Sat, 16 May 2020 09:48:12 GMT  
		Size: 4.4 MB (4390368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd216f8fa68b80c5b89b67bdf4aeedbe6d445ea495e9af5b07ff07c932d3478e`  
		Last Modified: Sat, 16 May 2020 09:48:12 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f04bcbae80555bc5a339111607737c8a22387e1ef9bdde9cd8cf59f7a7d2edd9`  
		Last Modified: Sat, 06 Jun 2020 02:20:38 GMT  
		Size: 444.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-alpine3.11` - linux; arm variant v6

```console
$ docker pull nats@sha256:92881cbdb3078b8a4456e1a45a34d9272357c7ab82ece5a9f96a517176aaaf9d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6720097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c294dd603de46043cfee2c1d0d9c7bb5783559f5d94b3e7e370d07d9ed3c0b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Fri, 15 May 2020 19:50:13 GMT
ENV NATS_SERVER=2.1.7
# Fri, 15 May 2020 19:50:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 15 May 2020 19:50:25 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 06 Jun 2020 02:50:21 GMT
COPY file:e90698d1d7a93a6e661321ceff0cc34f74523d472fad403fb682bb5d43b6a785 in /usr/local/bin 
# Sat, 06 Jun 2020 02:50:23 GMT
EXPOSE 4222 6222 8222
# Sat, 06 Jun 2020 02:50:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Jun 2020 02:50:27 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2da3e9f49b6c3ee3b36761ca52b69d8d5eef0937cb74cd8fddbb46850e21eea`  
		Last Modified: Fri, 15 May 2020 19:54:08 GMT  
		Size: 4.1 MB (4099154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf99cc6797b449693d5c09898c063ff989f060f8aec84ee465a356d2a45323c`  
		Last Modified: Fri, 15 May 2020 19:54:06 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c5786c0476f10cbaaed737392af53825da728437020325ccbd384cdf53b100`  
		Last Modified: Sat, 06 Jun 2020 02:57:26 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-alpine3.11` - linux; arm variant v7

```console
$ docker pull nats@sha256:2ce1841a96e019cbad94dc856fc41df447c6bfa53cda82adb93e431dc4bcc652
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6516346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:353d1047af5e64a22156c535460a8883c63c3bb196aa977c1a8a96c09f716163`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Sat, 16 May 2020 04:17:01 GMT
ENV NATS_SERVER=2.1.7
# Sat, 16 May 2020 04:17:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 16 May 2020 04:17:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 06 Jun 2020 02:59:06 GMT
COPY file:e90698d1d7a93a6e661321ceff0cc34f74523d472fad403fb682bb5d43b6a785 in /usr/local/bin 
# Sat, 06 Jun 2020 02:59:06 GMT
EXPOSE 4222 6222 8222
# Sat, 06 Jun 2020 02:59:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Jun 2020 02:59:08 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2111cd33403a7683737ec41dba39b7fd69d4d4c770b66eff350253601018f65`  
		Last Modified: Sat, 16 May 2020 04:26:40 GMT  
		Size: 4.1 MB (4093275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab45b7c0f143ec333947ad8048d647c2b8bc669596d874e502e79ee4e74e0f3`  
		Last Modified: Sat, 16 May 2020 04:26:40 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967546c6e8edd236036de77257c69742e6740d1e64cd55cd2905478fcfde9552`  
		Last Modified: Sat, 06 Jun 2020 03:09:08 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-linux`

```console
$ docker pull nats@sha256:b26e71094f7c4af203bdc62cd789f1ad78003d15c2889a02dafe21ef7cd8c035
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
$ docker pull nats@sha256:b26e71094f7c4af203bdc62cd789f1ad78003d15c2889a02dafe21ef7cd8c035
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
$ docker pull nats@sha256:d8b4027afa12bde158081e46da01e775d11b8281d7bfdd6dc418fab46607afc2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64
	-	windows version 10.0.14393.3808; amd64

### `nats:2.1-windowsservercore` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats@sha256:853c70bfa92057d5ff5cce9d40f23822b02351d1f196dc2aeee6f8b1d6b4e01e
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2328178778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de952a8a6f9f77294e1eb06c5e736386fc96f24575bd3d472aa6ed634683e147`
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
# Wed, 15 Jul 2020 15:03:42 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jul 2020 15:04:57 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Jul 2020 15:04:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jul 2020 15:05:00 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Jul 2020 15:05:01 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jul 2020 15:05:02 GMT
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
	-	`sha256:3cc0292f299542ec593d4cf8b4cae1422da5920a655cc145378a1f343bb4b82a`  
		Last Modified: Wed, 15 Jul 2020 15:09:33 GMT  
		Size: 4.8 MB (4800276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377ab72fb858121eb624585d89868fd66349f054e41a7feb0d6a8f9dcce7621f`  
		Last Modified: Wed, 15 Jul 2020 15:09:32 GMT  
		Size: 13.2 MB (13176530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b414836d9ec08b0beeed7d90882777bb3872b65a528d27eff46d11224367eb4`  
		Last Modified: Wed, 15 Jul 2020 15:09:29 GMT  
		Size: 1.7 KB (1699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218276e4e5be6f495bd072ca818cc3126a8e1de83e81cf3aac0e434a7cf998d3`  
		Last Modified: Wed, 15 Jul 2020 15:09:29 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554b66195d7e4135f672a2c5c88017b81cb523a28b19b3b01d7dc0cd0ac08b29`  
		Last Modified: Wed, 15 Jul 2020 15:09:29 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f992754834fc067d9ef4edb88b29e743cfb3feda4ebc33340af1fa7117fc762`  
		Last Modified: Wed, 15 Jul 2020 15:09:29 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-windowsservercore` - windows version 10.0.14393.3808; amd64

```console
$ docker pull nats@sha256:43b41d3085f47eee811b28506b54ff7c29da295345d214565a6d4f6e301bf396
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5756765076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9ff7196afcabade265df8afe613aa8fc6dcc055ed374eb60e92aa93e4978b7f`
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
# Wed, 15 Jul 2020 15:06:44 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jul 2020 15:08:49 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Jul 2020 15:08:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jul 2020 15:08:52 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Jul 2020 15:08:53 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jul 2020 15:08:54 GMT
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
	-	`sha256:0584eb6b5415d012501558a2dcc9f68bf8d1c0d96ab16abc0658534ca083763f`  
		Last Modified: Wed, 15 Jul 2020 15:10:20 GMT  
		Size: 5.4 MB (5361288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52eab21ed3b97aead8a8bafd9d07b9ac114cc1ccd2e5cfa6c2afac7401e38442`  
		Last Modified: Wed, 15 Jul 2020 15:10:22 GMT  
		Size: 13.9 MB (13931973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c1e79456e304bb7e24066e10b332b7da148fd981c19c151146e0498e09dbff`  
		Last Modified: Wed, 15 Jul 2020 15:10:16 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead3b72b2add53883aa3e0b7be3eb60a9f37fe43c4457e036da44a70e8b9cb23`  
		Last Modified: Wed, 15 Jul 2020 15:10:16 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3014d80ec0460dda49e4bf323f74bdf7b51b76cf368b453d59eb96443d61d1d8`  
		Last Modified: Wed, 15 Jul 2020 15:10:17 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aca79d7cfc3c47963f81e8c6f692cb6ffada2b4dc42fed607734a1446029e5f`  
		Last Modified: Wed, 15 Jul 2020 15:10:16 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-windowsservercore-1809`

```console
$ docker pull nats@sha256:666bfe8f181744c240647e0af2fc10ac2dfa90a7dfdf3e0cfe368f8d7d44087c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `nats:2.1-windowsservercore-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats@sha256:853c70bfa92057d5ff5cce9d40f23822b02351d1f196dc2aeee6f8b1d6b4e01e
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2328178778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de952a8a6f9f77294e1eb06c5e736386fc96f24575bd3d472aa6ed634683e147`
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
# Wed, 15 Jul 2020 15:03:42 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jul 2020 15:04:57 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Jul 2020 15:04:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jul 2020 15:05:00 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Jul 2020 15:05:01 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jul 2020 15:05:02 GMT
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
	-	`sha256:3cc0292f299542ec593d4cf8b4cae1422da5920a655cc145378a1f343bb4b82a`  
		Last Modified: Wed, 15 Jul 2020 15:09:33 GMT  
		Size: 4.8 MB (4800276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377ab72fb858121eb624585d89868fd66349f054e41a7feb0d6a8f9dcce7621f`  
		Last Modified: Wed, 15 Jul 2020 15:09:32 GMT  
		Size: 13.2 MB (13176530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b414836d9ec08b0beeed7d90882777bb3872b65a528d27eff46d11224367eb4`  
		Last Modified: Wed, 15 Jul 2020 15:09:29 GMT  
		Size: 1.7 KB (1699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218276e4e5be6f495bd072ca818cc3126a8e1de83e81cf3aac0e434a7cf998d3`  
		Last Modified: Wed, 15 Jul 2020 15:09:29 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554b66195d7e4135f672a2c5c88017b81cb523a28b19b3b01d7dc0cd0ac08b29`  
		Last Modified: Wed, 15 Jul 2020 15:09:29 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f992754834fc067d9ef4edb88b29e743cfb3feda4ebc33340af1fa7117fc762`  
		Last Modified: Wed, 15 Jul 2020 15:09:29 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:ce555ef8cbfebaaa0aa85b82cbccc3c230a067d2bddb3ab8a82e2ff094dc3bd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3808; amd64

### `nats:2.1-windowsservercore-ltsc2016` - windows version 10.0.14393.3808; amd64

```console
$ docker pull nats@sha256:43b41d3085f47eee811b28506b54ff7c29da295345d214565a6d4f6e301bf396
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5756765076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9ff7196afcabade265df8afe613aa8fc6dcc055ed374eb60e92aa93e4978b7f`
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
# Wed, 15 Jul 2020 15:06:44 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jul 2020 15:08:49 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Jul 2020 15:08:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jul 2020 15:08:52 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Jul 2020 15:08:53 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jul 2020 15:08:54 GMT
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
	-	`sha256:0584eb6b5415d012501558a2dcc9f68bf8d1c0d96ab16abc0658534ca083763f`  
		Last Modified: Wed, 15 Jul 2020 15:10:20 GMT  
		Size: 5.4 MB (5361288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52eab21ed3b97aead8a8bafd9d07b9ac114cc1ccd2e5cfa6c2afac7401e38442`  
		Last Modified: Wed, 15 Jul 2020 15:10:22 GMT  
		Size: 13.9 MB (13931973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c1e79456e304bb7e24066e10b332b7da148fd981c19c151146e0498e09dbff`  
		Last Modified: Wed, 15 Jul 2020 15:10:16 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead3b72b2add53883aa3e0b7be3eb60a9f37fe43c4457e036da44a70e8b9cb23`  
		Last Modified: Wed, 15 Jul 2020 15:10:16 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3014d80ec0460dda49e4bf323f74bdf7b51b76cf368b453d59eb96443d61d1d8`  
		Last Modified: Wed, 15 Jul 2020 15:10:17 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aca79d7cfc3c47963f81e8c6f692cb6ffada2b4dc42fed607734a1446029e5f`  
		Last Modified: Wed, 15 Jul 2020 15:10:16 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:966bafc8fed140348df882cdfce8c6ec0ae84246af19ba2dc4c44192a330c18b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:afc307dec8317bf0bee1c448f05a0e928635b5115f7e21890b9b6885de27e3e9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7204657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d55057d2200ae8b71e69d563361a7c078b9959e2df3b828c14c5c852d7ee85e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Sat, 16 May 2020 09:47:11 GMT
ENV NATS_SERVER=2.1.7
# Sat, 16 May 2020 09:47:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 16 May 2020 09:47:13 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 06 Jun 2020 02:20:01 GMT
COPY file:e90698d1d7a93a6e661321ceff0cc34f74523d472fad403fb682bb5d43b6a785 in /usr/local/bin 
# Sat, 06 Jun 2020 02:20:01 GMT
EXPOSE 4222 6222 8222
# Sat, 06 Jun 2020 02:20:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Jun 2020 02:20:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eaf9939fdcf9c33e5b47fb1d09e4994e32b77b1ae5f3e396ad0bd90449b3e99`  
		Last Modified: Sat, 16 May 2020 09:48:12 GMT  
		Size: 4.4 MB (4390368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd216f8fa68b80c5b89b67bdf4aeedbe6d445ea495e9af5b07ff07c932d3478e`  
		Last Modified: Sat, 16 May 2020 09:48:12 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f04bcbae80555bc5a339111607737c8a22387e1ef9bdde9cd8cf59f7a7d2edd9`  
		Last Modified: Sat, 06 Jun 2020 02:20:38 GMT  
		Size: 444.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:92881cbdb3078b8a4456e1a45a34d9272357c7ab82ece5a9f96a517176aaaf9d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6720097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c294dd603de46043cfee2c1d0d9c7bb5783559f5d94b3e7e370d07d9ed3c0b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Fri, 15 May 2020 19:50:13 GMT
ENV NATS_SERVER=2.1.7
# Fri, 15 May 2020 19:50:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 15 May 2020 19:50:25 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 06 Jun 2020 02:50:21 GMT
COPY file:e90698d1d7a93a6e661321ceff0cc34f74523d472fad403fb682bb5d43b6a785 in /usr/local/bin 
# Sat, 06 Jun 2020 02:50:23 GMT
EXPOSE 4222 6222 8222
# Sat, 06 Jun 2020 02:50:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Jun 2020 02:50:27 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2da3e9f49b6c3ee3b36761ca52b69d8d5eef0937cb74cd8fddbb46850e21eea`  
		Last Modified: Fri, 15 May 2020 19:54:08 GMT  
		Size: 4.1 MB (4099154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf99cc6797b449693d5c09898c063ff989f060f8aec84ee465a356d2a45323c`  
		Last Modified: Fri, 15 May 2020 19:54:06 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c5786c0476f10cbaaed737392af53825da728437020325ccbd384cdf53b100`  
		Last Modified: Sat, 06 Jun 2020 02:57:26 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:2ce1841a96e019cbad94dc856fc41df447c6bfa53cda82adb93e431dc4bcc652
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6516346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:353d1047af5e64a22156c535460a8883c63c3bb196aa977c1a8a96c09f716163`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Sat, 16 May 2020 04:17:01 GMT
ENV NATS_SERVER=2.1.7
# Sat, 16 May 2020 04:17:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 16 May 2020 04:17:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 06 Jun 2020 02:59:06 GMT
COPY file:e90698d1d7a93a6e661321ceff0cc34f74523d472fad403fb682bb5d43b6a785 in /usr/local/bin 
# Sat, 06 Jun 2020 02:59:06 GMT
EXPOSE 4222 6222 8222
# Sat, 06 Jun 2020 02:59:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Jun 2020 02:59:08 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2111cd33403a7683737ec41dba39b7fd69d4d4c770b66eff350253601018f65`  
		Last Modified: Sat, 16 May 2020 04:26:40 GMT  
		Size: 4.1 MB (4093275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab45b7c0f143ec333947ad8048d647c2b8bc669596d874e502e79ee4e74e0f3`  
		Last Modified: Sat, 16 May 2020 04:26:40 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967546c6e8edd236036de77257c69742e6740d1e64cd55cd2905478fcfde9552`  
		Last Modified: Sat, 06 Jun 2020 03:09:08 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.11`

```console
$ docker pull nats@sha256:966bafc8fed140348df882cdfce8c6ec0ae84246af19ba2dc4c44192a330c18b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats:2-alpine3.11` - linux; amd64

```console
$ docker pull nats@sha256:afc307dec8317bf0bee1c448f05a0e928635b5115f7e21890b9b6885de27e3e9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7204657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d55057d2200ae8b71e69d563361a7c078b9959e2df3b828c14c5c852d7ee85e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Sat, 16 May 2020 09:47:11 GMT
ENV NATS_SERVER=2.1.7
# Sat, 16 May 2020 09:47:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 16 May 2020 09:47:13 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 06 Jun 2020 02:20:01 GMT
COPY file:e90698d1d7a93a6e661321ceff0cc34f74523d472fad403fb682bb5d43b6a785 in /usr/local/bin 
# Sat, 06 Jun 2020 02:20:01 GMT
EXPOSE 4222 6222 8222
# Sat, 06 Jun 2020 02:20:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Jun 2020 02:20:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eaf9939fdcf9c33e5b47fb1d09e4994e32b77b1ae5f3e396ad0bd90449b3e99`  
		Last Modified: Sat, 16 May 2020 09:48:12 GMT  
		Size: 4.4 MB (4390368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd216f8fa68b80c5b89b67bdf4aeedbe6d445ea495e9af5b07ff07c932d3478e`  
		Last Modified: Sat, 16 May 2020 09:48:12 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f04bcbae80555bc5a339111607737c8a22387e1ef9bdde9cd8cf59f7a7d2edd9`  
		Last Modified: Sat, 06 Jun 2020 02:20:38 GMT  
		Size: 444.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.11` - linux; arm variant v6

```console
$ docker pull nats@sha256:92881cbdb3078b8a4456e1a45a34d9272357c7ab82ece5a9f96a517176aaaf9d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6720097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c294dd603de46043cfee2c1d0d9c7bb5783559f5d94b3e7e370d07d9ed3c0b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Fri, 15 May 2020 19:50:13 GMT
ENV NATS_SERVER=2.1.7
# Fri, 15 May 2020 19:50:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 15 May 2020 19:50:25 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 06 Jun 2020 02:50:21 GMT
COPY file:e90698d1d7a93a6e661321ceff0cc34f74523d472fad403fb682bb5d43b6a785 in /usr/local/bin 
# Sat, 06 Jun 2020 02:50:23 GMT
EXPOSE 4222 6222 8222
# Sat, 06 Jun 2020 02:50:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Jun 2020 02:50:27 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2da3e9f49b6c3ee3b36761ca52b69d8d5eef0937cb74cd8fddbb46850e21eea`  
		Last Modified: Fri, 15 May 2020 19:54:08 GMT  
		Size: 4.1 MB (4099154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf99cc6797b449693d5c09898c063ff989f060f8aec84ee465a356d2a45323c`  
		Last Modified: Fri, 15 May 2020 19:54:06 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c5786c0476f10cbaaed737392af53825da728437020325ccbd384cdf53b100`  
		Last Modified: Sat, 06 Jun 2020 02:57:26 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.11` - linux; arm variant v7

```console
$ docker pull nats@sha256:2ce1841a96e019cbad94dc856fc41df447c6bfa53cda82adb93e431dc4bcc652
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6516346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:353d1047af5e64a22156c535460a8883c63c3bb196aa977c1a8a96c09f716163`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Sat, 16 May 2020 04:17:01 GMT
ENV NATS_SERVER=2.1.7
# Sat, 16 May 2020 04:17:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 16 May 2020 04:17:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 06 Jun 2020 02:59:06 GMT
COPY file:e90698d1d7a93a6e661321ceff0cc34f74523d472fad403fb682bb5d43b6a785 in /usr/local/bin 
# Sat, 06 Jun 2020 02:59:06 GMT
EXPOSE 4222 6222 8222
# Sat, 06 Jun 2020 02:59:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Jun 2020 02:59:08 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2111cd33403a7683737ec41dba39b7fd69d4d4c770b66eff350253601018f65`  
		Last Modified: Sat, 16 May 2020 04:26:40 GMT  
		Size: 4.1 MB (4093275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab45b7c0f143ec333947ad8048d647c2b8bc669596d874e502e79ee4e74e0f3`  
		Last Modified: Sat, 16 May 2020 04:26:40 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967546c6e8edd236036de77257c69742e6740d1e64cd55cd2905478fcfde9552`  
		Last Modified: Sat, 06 Jun 2020 03:09:08 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:b26e71094f7c4af203bdc62cd789f1ad78003d15c2889a02dafe21ef7cd8c035
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
$ docker pull nats@sha256:b26e71094f7c4af203bdc62cd789f1ad78003d15c2889a02dafe21ef7cd8c035
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
$ docker pull nats@sha256:d8b4027afa12bde158081e46da01e775d11b8281d7bfdd6dc418fab46607afc2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64
	-	windows version 10.0.14393.3808; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats@sha256:853c70bfa92057d5ff5cce9d40f23822b02351d1f196dc2aeee6f8b1d6b4e01e
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2328178778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de952a8a6f9f77294e1eb06c5e736386fc96f24575bd3d472aa6ed634683e147`
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
# Wed, 15 Jul 2020 15:03:42 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jul 2020 15:04:57 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Jul 2020 15:04:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jul 2020 15:05:00 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Jul 2020 15:05:01 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jul 2020 15:05:02 GMT
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
	-	`sha256:3cc0292f299542ec593d4cf8b4cae1422da5920a655cc145378a1f343bb4b82a`  
		Last Modified: Wed, 15 Jul 2020 15:09:33 GMT  
		Size: 4.8 MB (4800276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377ab72fb858121eb624585d89868fd66349f054e41a7feb0d6a8f9dcce7621f`  
		Last Modified: Wed, 15 Jul 2020 15:09:32 GMT  
		Size: 13.2 MB (13176530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b414836d9ec08b0beeed7d90882777bb3872b65a528d27eff46d11224367eb4`  
		Last Modified: Wed, 15 Jul 2020 15:09:29 GMT  
		Size: 1.7 KB (1699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218276e4e5be6f495bd072ca818cc3126a8e1de83e81cf3aac0e434a7cf998d3`  
		Last Modified: Wed, 15 Jul 2020 15:09:29 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554b66195d7e4135f672a2c5c88017b81cb523a28b19b3b01d7dc0cd0ac08b29`  
		Last Modified: Wed, 15 Jul 2020 15:09:29 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f992754834fc067d9ef4edb88b29e743cfb3feda4ebc33340af1fa7117fc762`  
		Last Modified: Wed, 15 Jul 2020 15:09:29 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-windowsservercore` - windows version 10.0.14393.3808; amd64

```console
$ docker pull nats@sha256:43b41d3085f47eee811b28506b54ff7c29da295345d214565a6d4f6e301bf396
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5756765076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9ff7196afcabade265df8afe613aa8fc6dcc055ed374eb60e92aa93e4978b7f`
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
# Wed, 15 Jul 2020 15:06:44 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jul 2020 15:08:49 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Jul 2020 15:08:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jul 2020 15:08:52 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Jul 2020 15:08:53 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jul 2020 15:08:54 GMT
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
	-	`sha256:0584eb6b5415d012501558a2dcc9f68bf8d1c0d96ab16abc0658534ca083763f`  
		Last Modified: Wed, 15 Jul 2020 15:10:20 GMT  
		Size: 5.4 MB (5361288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52eab21ed3b97aead8a8bafd9d07b9ac114cc1ccd2e5cfa6c2afac7401e38442`  
		Last Modified: Wed, 15 Jul 2020 15:10:22 GMT  
		Size: 13.9 MB (13931973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c1e79456e304bb7e24066e10b332b7da148fd981c19c151146e0498e09dbff`  
		Last Modified: Wed, 15 Jul 2020 15:10:16 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead3b72b2add53883aa3e0b7be3eb60a9f37fe43c4457e036da44a70e8b9cb23`  
		Last Modified: Wed, 15 Jul 2020 15:10:16 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3014d80ec0460dda49e4bf323f74bdf7b51b76cf368b453d59eb96443d61d1d8`  
		Last Modified: Wed, 15 Jul 2020 15:10:17 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aca79d7cfc3c47963f81e8c6f692cb6ffada2b4dc42fed607734a1446029e5f`  
		Last Modified: Wed, 15 Jul 2020 15:10:16 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:666bfe8f181744c240647e0af2fc10ac2dfa90a7dfdf3e0cfe368f8d7d44087c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats@sha256:853c70bfa92057d5ff5cce9d40f23822b02351d1f196dc2aeee6f8b1d6b4e01e
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2328178778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de952a8a6f9f77294e1eb06c5e736386fc96f24575bd3d472aa6ed634683e147`
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
# Wed, 15 Jul 2020 15:03:42 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jul 2020 15:04:57 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Jul 2020 15:04:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jul 2020 15:05:00 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Jul 2020 15:05:01 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jul 2020 15:05:02 GMT
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
	-	`sha256:3cc0292f299542ec593d4cf8b4cae1422da5920a655cc145378a1f343bb4b82a`  
		Last Modified: Wed, 15 Jul 2020 15:09:33 GMT  
		Size: 4.8 MB (4800276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377ab72fb858121eb624585d89868fd66349f054e41a7feb0d6a8f9dcce7621f`  
		Last Modified: Wed, 15 Jul 2020 15:09:32 GMT  
		Size: 13.2 MB (13176530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b414836d9ec08b0beeed7d90882777bb3872b65a528d27eff46d11224367eb4`  
		Last Modified: Wed, 15 Jul 2020 15:09:29 GMT  
		Size: 1.7 KB (1699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218276e4e5be6f495bd072ca818cc3126a8e1de83e81cf3aac0e434a7cf998d3`  
		Last Modified: Wed, 15 Jul 2020 15:09:29 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554b66195d7e4135f672a2c5c88017b81cb523a28b19b3b01d7dc0cd0ac08b29`  
		Last Modified: Wed, 15 Jul 2020 15:09:29 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f992754834fc067d9ef4edb88b29e743cfb3feda4ebc33340af1fa7117fc762`  
		Last Modified: Wed, 15 Jul 2020 15:09:29 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:ce555ef8cbfebaaa0aa85b82cbccc3c230a067d2bddb3ab8a82e2ff094dc3bd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3808; amd64

### `nats:2-windowsservercore-ltsc2016` - windows version 10.0.14393.3808; amd64

```console
$ docker pull nats@sha256:43b41d3085f47eee811b28506b54ff7c29da295345d214565a6d4f6e301bf396
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5756765076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9ff7196afcabade265df8afe613aa8fc6dcc055ed374eb60e92aa93e4978b7f`
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
# Wed, 15 Jul 2020 15:06:44 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jul 2020 15:08:49 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Jul 2020 15:08:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jul 2020 15:08:52 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Jul 2020 15:08:53 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jul 2020 15:08:54 GMT
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
	-	`sha256:0584eb6b5415d012501558a2dcc9f68bf8d1c0d96ab16abc0658534ca083763f`  
		Last Modified: Wed, 15 Jul 2020 15:10:20 GMT  
		Size: 5.4 MB (5361288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52eab21ed3b97aead8a8bafd9d07b9ac114cc1ccd2e5cfa6c2afac7401e38442`  
		Last Modified: Wed, 15 Jul 2020 15:10:22 GMT  
		Size: 13.9 MB (13931973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c1e79456e304bb7e24066e10b332b7da148fd981c19c151146e0498e09dbff`  
		Last Modified: Wed, 15 Jul 2020 15:10:16 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead3b72b2add53883aa3e0b7be3eb60a9f37fe43c4457e036da44a70e8b9cb23`  
		Last Modified: Wed, 15 Jul 2020 15:10:16 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3014d80ec0460dda49e4bf323f74bdf7b51b76cf368b453d59eb96443d61d1d8`  
		Last Modified: Wed, 15 Jul 2020 15:10:17 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aca79d7cfc3c47963f81e8c6f692cb6ffada2b4dc42fed607734a1446029e5f`  
		Last Modified: Wed, 15 Jul 2020 15:10:16 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:966bafc8fed140348df882cdfce8c6ec0ae84246af19ba2dc4c44192a330c18b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:afc307dec8317bf0bee1c448f05a0e928635b5115f7e21890b9b6885de27e3e9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7204657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d55057d2200ae8b71e69d563361a7c078b9959e2df3b828c14c5c852d7ee85e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Sat, 16 May 2020 09:47:11 GMT
ENV NATS_SERVER=2.1.7
# Sat, 16 May 2020 09:47:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 16 May 2020 09:47:13 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 06 Jun 2020 02:20:01 GMT
COPY file:e90698d1d7a93a6e661321ceff0cc34f74523d472fad403fb682bb5d43b6a785 in /usr/local/bin 
# Sat, 06 Jun 2020 02:20:01 GMT
EXPOSE 4222 6222 8222
# Sat, 06 Jun 2020 02:20:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Jun 2020 02:20:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eaf9939fdcf9c33e5b47fb1d09e4994e32b77b1ae5f3e396ad0bd90449b3e99`  
		Last Modified: Sat, 16 May 2020 09:48:12 GMT  
		Size: 4.4 MB (4390368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd216f8fa68b80c5b89b67bdf4aeedbe6d445ea495e9af5b07ff07c932d3478e`  
		Last Modified: Sat, 16 May 2020 09:48:12 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f04bcbae80555bc5a339111607737c8a22387e1ef9bdde9cd8cf59f7a7d2edd9`  
		Last Modified: Sat, 06 Jun 2020 02:20:38 GMT  
		Size: 444.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:92881cbdb3078b8a4456e1a45a34d9272357c7ab82ece5a9f96a517176aaaf9d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6720097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c294dd603de46043cfee2c1d0d9c7bb5783559f5d94b3e7e370d07d9ed3c0b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Fri, 15 May 2020 19:50:13 GMT
ENV NATS_SERVER=2.1.7
# Fri, 15 May 2020 19:50:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 15 May 2020 19:50:25 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 06 Jun 2020 02:50:21 GMT
COPY file:e90698d1d7a93a6e661321ceff0cc34f74523d472fad403fb682bb5d43b6a785 in /usr/local/bin 
# Sat, 06 Jun 2020 02:50:23 GMT
EXPOSE 4222 6222 8222
# Sat, 06 Jun 2020 02:50:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Jun 2020 02:50:27 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2da3e9f49b6c3ee3b36761ca52b69d8d5eef0937cb74cd8fddbb46850e21eea`  
		Last Modified: Fri, 15 May 2020 19:54:08 GMT  
		Size: 4.1 MB (4099154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf99cc6797b449693d5c09898c063ff989f060f8aec84ee465a356d2a45323c`  
		Last Modified: Fri, 15 May 2020 19:54:06 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c5786c0476f10cbaaed737392af53825da728437020325ccbd384cdf53b100`  
		Last Modified: Sat, 06 Jun 2020 02:57:26 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:2ce1841a96e019cbad94dc856fc41df447c6bfa53cda82adb93e431dc4bcc652
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6516346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:353d1047af5e64a22156c535460a8883c63c3bb196aa977c1a8a96c09f716163`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Sat, 16 May 2020 04:17:01 GMT
ENV NATS_SERVER=2.1.7
# Sat, 16 May 2020 04:17:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 16 May 2020 04:17:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 06 Jun 2020 02:59:06 GMT
COPY file:e90698d1d7a93a6e661321ceff0cc34f74523d472fad403fb682bb5d43b6a785 in /usr/local/bin 
# Sat, 06 Jun 2020 02:59:06 GMT
EXPOSE 4222 6222 8222
# Sat, 06 Jun 2020 02:59:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Jun 2020 02:59:08 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2111cd33403a7683737ec41dba39b7fd69d4d4c770b66eff350253601018f65`  
		Last Modified: Sat, 16 May 2020 04:26:40 GMT  
		Size: 4.1 MB (4093275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab45b7c0f143ec333947ad8048d647c2b8bc669596d874e502e79ee4e74e0f3`  
		Last Modified: Sat, 16 May 2020 04:26:40 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967546c6e8edd236036de77257c69742e6740d1e64cd55cd2905478fcfde9552`  
		Last Modified: Sat, 06 Jun 2020 03:09:08 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.11`

```console
$ docker pull nats@sha256:966bafc8fed140348df882cdfce8c6ec0ae84246af19ba2dc4c44192a330c18b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats:alpine3.11` - linux; amd64

```console
$ docker pull nats@sha256:afc307dec8317bf0bee1c448f05a0e928635b5115f7e21890b9b6885de27e3e9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7204657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d55057d2200ae8b71e69d563361a7c078b9959e2df3b828c14c5c852d7ee85e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Sat, 16 May 2020 09:47:11 GMT
ENV NATS_SERVER=2.1.7
# Sat, 16 May 2020 09:47:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 16 May 2020 09:47:13 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 06 Jun 2020 02:20:01 GMT
COPY file:e90698d1d7a93a6e661321ceff0cc34f74523d472fad403fb682bb5d43b6a785 in /usr/local/bin 
# Sat, 06 Jun 2020 02:20:01 GMT
EXPOSE 4222 6222 8222
# Sat, 06 Jun 2020 02:20:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Jun 2020 02:20:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eaf9939fdcf9c33e5b47fb1d09e4994e32b77b1ae5f3e396ad0bd90449b3e99`  
		Last Modified: Sat, 16 May 2020 09:48:12 GMT  
		Size: 4.4 MB (4390368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd216f8fa68b80c5b89b67bdf4aeedbe6d445ea495e9af5b07ff07c932d3478e`  
		Last Modified: Sat, 16 May 2020 09:48:12 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f04bcbae80555bc5a339111607737c8a22387e1ef9bdde9cd8cf59f7a7d2edd9`  
		Last Modified: Sat, 06 Jun 2020 02:20:38 GMT  
		Size: 444.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.11` - linux; arm variant v6

```console
$ docker pull nats@sha256:92881cbdb3078b8a4456e1a45a34d9272357c7ab82ece5a9f96a517176aaaf9d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6720097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c294dd603de46043cfee2c1d0d9c7bb5783559f5d94b3e7e370d07d9ed3c0b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Fri, 15 May 2020 19:50:13 GMT
ENV NATS_SERVER=2.1.7
# Fri, 15 May 2020 19:50:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 15 May 2020 19:50:25 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 06 Jun 2020 02:50:21 GMT
COPY file:e90698d1d7a93a6e661321ceff0cc34f74523d472fad403fb682bb5d43b6a785 in /usr/local/bin 
# Sat, 06 Jun 2020 02:50:23 GMT
EXPOSE 4222 6222 8222
# Sat, 06 Jun 2020 02:50:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Jun 2020 02:50:27 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2da3e9f49b6c3ee3b36761ca52b69d8d5eef0937cb74cd8fddbb46850e21eea`  
		Last Modified: Fri, 15 May 2020 19:54:08 GMT  
		Size: 4.1 MB (4099154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf99cc6797b449693d5c09898c063ff989f060f8aec84ee465a356d2a45323c`  
		Last Modified: Fri, 15 May 2020 19:54:06 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c5786c0476f10cbaaed737392af53825da728437020325ccbd384cdf53b100`  
		Last Modified: Sat, 06 Jun 2020 02:57:26 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.11` - linux; arm variant v7

```console
$ docker pull nats@sha256:2ce1841a96e019cbad94dc856fc41df447c6bfa53cda82adb93e431dc4bcc652
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6516346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:353d1047af5e64a22156c535460a8883c63c3bb196aa977c1a8a96c09f716163`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Sat, 16 May 2020 04:17:01 GMT
ENV NATS_SERVER=2.1.7
# Sat, 16 May 2020 04:17:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 16 May 2020 04:17:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 06 Jun 2020 02:59:06 GMT
COPY file:e90698d1d7a93a6e661321ceff0cc34f74523d472fad403fb682bb5d43b6a785 in /usr/local/bin 
# Sat, 06 Jun 2020 02:59:06 GMT
EXPOSE 4222 6222 8222
# Sat, 06 Jun 2020 02:59:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Jun 2020 02:59:08 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2111cd33403a7683737ec41dba39b7fd69d4d4c770b66eff350253601018f65`  
		Last Modified: Sat, 16 May 2020 04:26:40 GMT  
		Size: 4.1 MB (4093275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab45b7c0f143ec333947ad8048d647c2b8bc669596d874e502e79ee4e74e0f3`  
		Last Modified: Sat, 16 May 2020 04:26:40 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967546c6e8edd236036de77257c69742e6740d1e64cd55cd2905478fcfde9552`  
		Last Modified: Sat, 06 Jun 2020 03:09:08 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:85589e53092232c686097acfdc3828ac0e20a562d63c5d0f0e7dfceade6fad49
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
$ docker pull nats@sha256:b26e71094f7c4af203bdc62cd789f1ad78003d15c2889a02dafe21ef7cd8c035
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
$ docker pull nats@sha256:b26e71094f7c4af203bdc62cd789f1ad78003d15c2889a02dafe21ef7cd8c035
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
$ docker pull nats@sha256:d8b4027afa12bde158081e46da01e775d11b8281d7bfdd6dc418fab46607afc2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64
	-	windows version 10.0.14393.3808; amd64

### `nats:windowsservercore` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats@sha256:853c70bfa92057d5ff5cce9d40f23822b02351d1f196dc2aeee6f8b1d6b4e01e
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2328178778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de952a8a6f9f77294e1eb06c5e736386fc96f24575bd3d472aa6ed634683e147`
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
# Wed, 15 Jul 2020 15:03:42 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jul 2020 15:04:57 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Jul 2020 15:04:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jul 2020 15:05:00 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Jul 2020 15:05:01 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jul 2020 15:05:02 GMT
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
	-	`sha256:3cc0292f299542ec593d4cf8b4cae1422da5920a655cc145378a1f343bb4b82a`  
		Last Modified: Wed, 15 Jul 2020 15:09:33 GMT  
		Size: 4.8 MB (4800276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377ab72fb858121eb624585d89868fd66349f054e41a7feb0d6a8f9dcce7621f`  
		Last Modified: Wed, 15 Jul 2020 15:09:32 GMT  
		Size: 13.2 MB (13176530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b414836d9ec08b0beeed7d90882777bb3872b65a528d27eff46d11224367eb4`  
		Last Modified: Wed, 15 Jul 2020 15:09:29 GMT  
		Size: 1.7 KB (1699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218276e4e5be6f495bd072ca818cc3126a8e1de83e81cf3aac0e434a7cf998d3`  
		Last Modified: Wed, 15 Jul 2020 15:09:29 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554b66195d7e4135f672a2c5c88017b81cb523a28b19b3b01d7dc0cd0ac08b29`  
		Last Modified: Wed, 15 Jul 2020 15:09:29 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f992754834fc067d9ef4edb88b29e743cfb3feda4ebc33340af1fa7117fc762`  
		Last Modified: Wed, 15 Jul 2020 15:09:29 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:windowsservercore` - windows version 10.0.14393.3808; amd64

```console
$ docker pull nats@sha256:43b41d3085f47eee811b28506b54ff7c29da295345d214565a6d4f6e301bf396
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5756765076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9ff7196afcabade265df8afe613aa8fc6dcc055ed374eb60e92aa93e4978b7f`
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
# Wed, 15 Jul 2020 15:06:44 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jul 2020 15:08:49 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Jul 2020 15:08:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jul 2020 15:08:52 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Jul 2020 15:08:53 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jul 2020 15:08:54 GMT
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
	-	`sha256:0584eb6b5415d012501558a2dcc9f68bf8d1c0d96ab16abc0658534ca083763f`  
		Last Modified: Wed, 15 Jul 2020 15:10:20 GMT  
		Size: 5.4 MB (5361288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52eab21ed3b97aead8a8bafd9d07b9ac114cc1ccd2e5cfa6c2afac7401e38442`  
		Last Modified: Wed, 15 Jul 2020 15:10:22 GMT  
		Size: 13.9 MB (13931973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c1e79456e304bb7e24066e10b332b7da148fd981c19c151146e0498e09dbff`  
		Last Modified: Wed, 15 Jul 2020 15:10:16 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead3b72b2add53883aa3e0b7be3eb60a9f37fe43c4457e036da44a70e8b9cb23`  
		Last Modified: Wed, 15 Jul 2020 15:10:16 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3014d80ec0460dda49e4bf323f74bdf7b51b76cf368b453d59eb96443d61d1d8`  
		Last Modified: Wed, 15 Jul 2020 15:10:17 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aca79d7cfc3c47963f81e8c6f692cb6ffada2b4dc42fed607734a1446029e5f`  
		Last Modified: Wed, 15 Jul 2020 15:10:16 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:666bfe8f181744c240647e0af2fc10ac2dfa90a7dfdf3e0cfe368f8d7d44087c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats@sha256:853c70bfa92057d5ff5cce9d40f23822b02351d1f196dc2aeee6f8b1d6b4e01e
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2328178778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de952a8a6f9f77294e1eb06c5e736386fc96f24575bd3d472aa6ed634683e147`
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
# Wed, 15 Jul 2020 15:03:42 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jul 2020 15:04:57 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Jul 2020 15:04:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jul 2020 15:05:00 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Jul 2020 15:05:01 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jul 2020 15:05:02 GMT
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
	-	`sha256:3cc0292f299542ec593d4cf8b4cae1422da5920a655cc145378a1f343bb4b82a`  
		Last Modified: Wed, 15 Jul 2020 15:09:33 GMT  
		Size: 4.8 MB (4800276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377ab72fb858121eb624585d89868fd66349f054e41a7feb0d6a8f9dcce7621f`  
		Last Modified: Wed, 15 Jul 2020 15:09:32 GMT  
		Size: 13.2 MB (13176530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b414836d9ec08b0beeed7d90882777bb3872b65a528d27eff46d11224367eb4`  
		Last Modified: Wed, 15 Jul 2020 15:09:29 GMT  
		Size: 1.7 KB (1699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218276e4e5be6f495bd072ca818cc3126a8e1de83e81cf3aac0e434a7cf998d3`  
		Last Modified: Wed, 15 Jul 2020 15:09:29 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554b66195d7e4135f672a2c5c88017b81cb523a28b19b3b01d7dc0cd0ac08b29`  
		Last Modified: Wed, 15 Jul 2020 15:09:29 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f992754834fc067d9ef4edb88b29e743cfb3feda4ebc33340af1fa7117fc762`  
		Last Modified: Wed, 15 Jul 2020 15:09:29 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:ce555ef8cbfebaaa0aa85b82cbccc3c230a067d2bddb3ab8a82e2ff094dc3bd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3808; amd64

### `nats:windowsservercore-ltsc2016` - windows version 10.0.14393.3808; amd64

```console
$ docker pull nats@sha256:43b41d3085f47eee811b28506b54ff7c29da295345d214565a6d4f6e301bf396
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5756765076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9ff7196afcabade265df8afe613aa8fc6dcc055ed374eb60e92aa93e4978b7f`
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
# Wed, 15 Jul 2020 15:06:44 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jul 2020 15:08:49 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Jul 2020 15:08:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Jul 2020 15:08:52 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Jul 2020 15:08:53 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jul 2020 15:08:54 GMT
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
	-	`sha256:0584eb6b5415d012501558a2dcc9f68bf8d1c0d96ab16abc0658534ca083763f`  
		Last Modified: Wed, 15 Jul 2020 15:10:20 GMT  
		Size: 5.4 MB (5361288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52eab21ed3b97aead8a8bafd9d07b9ac114cc1ccd2e5cfa6c2afac7401e38442`  
		Last Modified: Wed, 15 Jul 2020 15:10:22 GMT  
		Size: 13.9 MB (13931973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c1e79456e304bb7e24066e10b332b7da148fd981c19c151146e0498e09dbff`  
		Last Modified: Wed, 15 Jul 2020 15:10:16 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead3b72b2add53883aa3e0b7be3eb60a9f37fe43c4457e036da44a70e8b9cb23`  
		Last Modified: Wed, 15 Jul 2020 15:10:16 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3014d80ec0460dda49e4bf323f74bdf7b51b76cf368b453d59eb96443d61d1d8`  
		Last Modified: Wed, 15 Jul 2020 15:10:17 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aca79d7cfc3c47963f81e8c6f692cb6ffada2b4dc42fed607734a1446029e5f`  
		Last Modified: Wed, 15 Jul 2020 15:10:16 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
