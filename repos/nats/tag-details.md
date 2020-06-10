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
$ docker pull nats@sha256:1dcedfdb0d872fe1394759ac6eb3d1176dfd50bf8c2e2ef74349ea3bac1fe4d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1282; amd64

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

### `nats:2` - windows version 10.0.17763.1282; amd64

```console
$ docker pull nats@sha256:23c3043b7d852c7a960b62141f08843223754582d236eb2e9610b349c110ce30
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105104931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d94790e871ec07154936db07dcf840f87ed91dbe648823dd3ab3bfd35cee85d`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 03 Jun 2020 11:12:32 GMT
RUN Apply image 1809-amd64
# Wed, 10 Jun 2020 16:04:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Jun 2020 16:04:16 GMT
RUN cmd /S /C #(nop) COPY file:18561b827240029ad80d0e3d25142efae62905c30cc520fc37cfc68e7d889848 in C:\nats-server.exe 
# Wed, 10 Jun 2020 16:04:18 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Jun 2020 16:04:19 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 Jun 2020 16:04:19 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Jun 2020 16:04:20 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c7d6d47ff7dfb2aa4d4e819641b93ec971e8541978dff0ffc24c193babeb8c07`  
		Size: 101.0 MB (101043386 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fd97aa6008f57e8475bff231216617c39835f885adb6a9c73a3a1599e2d788b9`  
		Last Modified: Wed, 10 Jun 2020 16:08:53 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550b5fdbee6a185b325bc673ac4059474353d34cc82ee5722edc4dca721c3c5a`  
		Last Modified: Wed, 10 Jun 2020 16:08:52 GMT  
		Size: 4.1 MB (4056494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ee7df3dace6c97838bc1bdecdff255d7e67bbec225868420ce6f188538c17a`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db8b53011d85727f476a78b4ad3a21cad54684c2ce7dac2011db5f3be7a2312`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9cac1f94d61b8883bdd4f0af6741b02ba9bb5df9bc58fa289e792f40f25310`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 918.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1306722d16f58c9f328a577068e5aea75b105b9d09dc8ad19a48734418ee276b`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1`

```console
$ docker pull nats@sha256:1dcedfdb0d872fe1394759ac6eb3d1176dfd50bf8c2e2ef74349ea3bac1fe4d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1282; amd64

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

### `nats:2.1` - windows version 10.0.17763.1282; amd64

```console
$ docker pull nats@sha256:23c3043b7d852c7a960b62141f08843223754582d236eb2e9610b349c110ce30
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105104931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d94790e871ec07154936db07dcf840f87ed91dbe648823dd3ab3bfd35cee85d`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 03 Jun 2020 11:12:32 GMT
RUN Apply image 1809-amd64
# Wed, 10 Jun 2020 16:04:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Jun 2020 16:04:16 GMT
RUN cmd /S /C #(nop) COPY file:18561b827240029ad80d0e3d25142efae62905c30cc520fc37cfc68e7d889848 in C:\nats-server.exe 
# Wed, 10 Jun 2020 16:04:18 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Jun 2020 16:04:19 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 Jun 2020 16:04:19 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Jun 2020 16:04:20 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c7d6d47ff7dfb2aa4d4e819641b93ec971e8541978dff0ffc24c193babeb8c07`  
		Size: 101.0 MB (101043386 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fd97aa6008f57e8475bff231216617c39835f885adb6a9c73a3a1599e2d788b9`  
		Last Modified: Wed, 10 Jun 2020 16:08:53 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550b5fdbee6a185b325bc673ac4059474353d34cc82ee5722edc4dca721c3c5a`  
		Last Modified: Wed, 10 Jun 2020 16:08:52 GMT  
		Size: 4.1 MB (4056494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ee7df3dace6c97838bc1bdecdff255d7e67bbec225868420ce6f188538c17a`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db8b53011d85727f476a78b4ad3a21cad54684c2ce7dac2011db5f3be7a2312`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9cac1f94d61b8883bdd4f0af6741b02ba9bb5df9bc58fa289e792f40f25310`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 918.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1306722d16f58c9f328a577068e5aea75b105b9d09dc8ad19a48734418ee276b`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.7`

```console
$ docker pull nats@sha256:9af523981ad0f8fc510fd0c8ed3c995e1b8621918f9de9989b3d3b480c572172
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	windows version 10.0.17763.1282; amd64

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

### `nats:2.1.7` - windows version 10.0.17763.1282; amd64

```console
$ docker pull nats@sha256:23c3043b7d852c7a960b62141f08843223754582d236eb2e9610b349c110ce30
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105104931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d94790e871ec07154936db07dcf840f87ed91dbe648823dd3ab3bfd35cee85d`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 03 Jun 2020 11:12:32 GMT
RUN Apply image 1809-amd64
# Wed, 10 Jun 2020 16:04:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Jun 2020 16:04:16 GMT
RUN cmd /S /C #(nop) COPY file:18561b827240029ad80d0e3d25142efae62905c30cc520fc37cfc68e7d889848 in C:\nats-server.exe 
# Wed, 10 Jun 2020 16:04:18 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Jun 2020 16:04:19 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 Jun 2020 16:04:19 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Jun 2020 16:04:20 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c7d6d47ff7dfb2aa4d4e819641b93ec971e8541978dff0ffc24c193babeb8c07`  
		Size: 101.0 MB (101043386 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fd97aa6008f57e8475bff231216617c39835f885adb6a9c73a3a1599e2d788b9`  
		Last Modified: Wed, 10 Jun 2020 16:08:53 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550b5fdbee6a185b325bc673ac4059474353d34cc82ee5722edc4dca721c3c5a`  
		Last Modified: Wed, 10 Jun 2020 16:08:52 GMT  
		Size: 4.1 MB (4056494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ee7df3dace6c97838bc1bdecdff255d7e67bbec225868420ce6f188538c17a`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db8b53011d85727f476a78b4ad3a21cad54684c2ce7dac2011db5f3be7a2312`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9cac1f94d61b8883bdd4f0af6741b02ba9bb5df9bc58fa289e792f40f25310`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 918.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1306722d16f58c9f328a577068e5aea75b105b9d09dc8ad19a48734418ee276b`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 895.0 B  
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
$ docker pull nats@sha256:d2f7f2b6e7ef60042e06a03f94573e6aab5cd1f073f476f9efec62f527a59689
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `nats:2.1.7-nanoserver` - windows version 10.0.17763.1282; amd64

```console
$ docker pull nats@sha256:23c3043b7d852c7a960b62141f08843223754582d236eb2e9610b349c110ce30
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105104931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d94790e871ec07154936db07dcf840f87ed91dbe648823dd3ab3bfd35cee85d`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 03 Jun 2020 11:12:32 GMT
RUN Apply image 1809-amd64
# Wed, 10 Jun 2020 16:04:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Jun 2020 16:04:16 GMT
RUN cmd /S /C #(nop) COPY file:18561b827240029ad80d0e3d25142efae62905c30cc520fc37cfc68e7d889848 in C:\nats-server.exe 
# Wed, 10 Jun 2020 16:04:18 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Jun 2020 16:04:19 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 Jun 2020 16:04:19 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Jun 2020 16:04:20 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c7d6d47ff7dfb2aa4d4e819641b93ec971e8541978dff0ffc24c193babeb8c07`  
		Size: 101.0 MB (101043386 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fd97aa6008f57e8475bff231216617c39835f885adb6a9c73a3a1599e2d788b9`  
		Last Modified: Wed, 10 Jun 2020 16:08:53 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550b5fdbee6a185b325bc673ac4059474353d34cc82ee5722edc4dca721c3c5a`  
		Last Modified: Wed, 10 Jun 2020 16:08:52 GMT  
		Size: 4.1 MB (4056494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ee7df3dace6c97838bc1bdecdff255d7e67bbec225868420ce6f188538c17a`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db8b53011d85727f476a78b4ad3a21cad54684c2ce7dac2011db5f3be7a2312`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9cac1f94d61b8883bdd4f0af6741b02ba9bb5df9bc58fa289e792f40f25310`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 918.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1306722d16f58c9f328a577068e5aea75b105b9d09dc8ad19a48734418ee276b`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.7-nanoserver-1809`

```console
$ docker pull nats@sha256:d2f7f2b6e7ef60042e06a03f94573e6aab5cd1f073f476f9efec62f527a59689
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `nats:2.1.7-nanoserver-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull nats@sha256:23c3043b7d852c7a960b62141f08843223754582d236eb2e9610b349c110ce30
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105104931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d94790e871ec07154936db07dcf840f87ed91dbe648823dd3ab3bfd35cee85d`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 03 Jun 2020 11:12:32 GMT
RUN Apply image 1809-amd64
# Wed, 10 Jun 2020 16:04:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Jun 2020 16:04:16 GMT
RUN cmd /S /C #(nop) COPY file:18561b827240029ad80d0e3d25142efae62905c30cc520fc37cfc68e7d889848 in C:\nats-server.exe 
# Wed, 10 Jun 2020 16:04:18 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Jun 2020 16:04:19 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 Jun 2020 16:04:19 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Jun 2020 16:04:20 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c7d6d47ff7dfb2aa4d4e819641b93ec971e8541978dff0ffc24c193babeb8c07`  
		Size: 101.0 MB (101043386 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fd97aa6008f57e8475bff231216617c39835f885adb6a9c73a3a1599e2d788b9`  
		Last Modified: Wed, 10 Jun 2020 16:08:53 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550b5fdbee6a185b325bc673ac4059474353d34cc82ee5722edc4dca721c3c5a`  
		Last Modified: Wed, 10 Jun 2020 16:08:52 GMT  
		Size: 4.1 MB (4056494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ee7df3dace6c97838bc1bdecdff255d7e67bbec225868420ce6f188538c17a`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db8b53011d85727f476a78b4ad3a21cad54684c2ce7dac2011db5f3be7a2312`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9cac1f94d61b8883bdd4f0af6741b02ba9bb5df9bc58fa289e792f40f25310`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 918.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1306722d16f58c9f328a577068e5aea75b105b9d09dc8ad19a48734418ee276b`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 895.0 B  
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
$ docker pull nats@sha256:fa6675e4c8e617650d11e3f132ede6070c024a9157e1d7d0e895c6cf6a4e3940
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64
	-	windows version 10.0.14393.3750; amd64

### `nats:2.1.7-windowsservercore` - windows version 10.0.17763.1282; amd64

```console
$ docker pull nats@sha256:fbdcfbf0773b8c7e2671b579b3b52400d4e8eca9d180bff2e5727f0a3d8d0864
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2307473223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6740ad609d50656fff721f580457edd9f2d4eba332ff31941549b128b84715f9`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 16:02:03 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Jun 2020 16:02:04 GMT
ENV NATS_SERVER=2.1.7
# Wed, 10 Jun 2020 16:02:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.7/nats-server-v2.1.7-windows-amd64.zip
# Wed, 10 Jun 2020 16:02:43 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Jun 2020 16:03:56 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 10 Jun 2020 16:03:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Jun 2020 16:03:58 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Jun 2020 16:03:59 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Jun 2020 16:04:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2192add29c9167423d378daa499903c4488337cdc2cf961ebeb0e4c0b492f9`  
		Last Modified: Wed, 10 Jun 2020 16:08:35 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a9b4e5c1b0529d2d48245b55ee7598147e2e80e110c5869d3d8be61369c5eb`  
		Last Modified: Wed, 10 Jun 2020 16:08:35 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c2e6ac9c7e61a2754411cf19adff6716f1e9301e89e68dd1ea7eb2a3b8cf8d`  
		Last Modified: Wed, 10 Jun 2020 16:08:34 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d98700f3301fe8993c249b37c71191744756fc10e53a69ffd98ec065fe27e43f`  
		Last Modified: Wed, 10 Jun 2020 16:08:36 GMT  
		Size: 4.8 MB (4764734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3494a6c6401e0ad8aedfe8e3894f88e5429c8cfd769fc50a4772f8da266df8b7`  
		Last Modified: Wed, 10 Jun 2020 16:08:34 GMT  
		Size: 8.8 MB (8784508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f3b6d9839159b8fa9ce12839aecab1ad582bbf2608244ba649076f938b2848`  
		Last Modified: Wed, 10 Jun 2020 16:08:32 GMT  
		Size: 1.7 KB (1702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c2e2690d3427b399abec715252650057d6a2549eba4cb2acaae27be4ebd5e0`  
		Last Modified: Wed, 10 Jun 2020 16:08:32 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4501d667c20eece078538960df5d805e0150b66e576e8d3cf89dca5499785d4b`  
		Last Modified: Wed, 10 Jun 2020 16:08:31 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16339bfc95d775f95c321531252cd1313eadd0df74728cb872aa8e1fec49af42`  
		Last Modified: Wed, 10 Jun 2020 16:08:32 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.7-windowsservercore` - windows version 10.0.14393.3750; amd64

```console
$ docker pull nats@sha256:e32d961331b1efecafe08329ab9579dcd89035dbfc98ccd5ecd0124195c61b47
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5753367260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9e5cc77e49551b49ff66ed004535dff02071725ccf10441495e760de85b0aeb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 16:04:27 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Jun 2020 16:04:28 GMT
ENV NATS_SERVER=2.1.7
# Wed, 10 Jun 2020 16:04:29 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.7/nats-server-v2.1.7-windows-amd64.zip
# Wed, 10 Jun 2020 16:05:49 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Jun 2020 16:07:56 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 10 Jun 2020 16:07:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Jun 2020 16:08:00 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Jun 2020 16:08:01 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Jun 2020 16:08:02 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f945dc3cc7d024d3f86a74f177545b57d99c3209592a625bb655bf01921d2c`  
		Last Modified: Wed, 10 Jun 2020 16:09:12 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ae6d270564022284992180f4fd75553672266c2ac3ddfe37fcda523777d5d4`  
		Last Modified: Wed, 10 Jun 2020 16:09:12 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8835d3a93f1398493ed2485d211c2eaae6b2f63edaa2ad57b730e64ebe89d90a`  
		Last Modified: Wed, 10 Jun 2020 16:09:11 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b240ea1a26e00edd4b16bdbbe0af06d5cf97b87f869b97d75339b3db6bb5201d`  
		Last Modified: Wed, 10 Jun 2020 16:09:13 GMT  
		Size: 5.4 MB (5390325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dea13e836f486c4c268d4f38ad5227bfb7a088e2ce55dd1c1cdc37141d9a2c8`  
		Last Modified: Wed, 10 Jun 2020 16:09:26 GMT  
		Size: 14.0 MB (13969545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038f152d17356e6f5f3e4cddca5abe8c49f44535b31fddbbf6f92c71972dd08d`  
		Last Modified: Wed, 10 Jun 2020 16:09:09 GMT  
		Size: 1.7 KB (1675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b3323f04d21e510ede92022b9360017f11ac36acdb708ba7ccc23057653d07`  
		Last Modified: Wed, 10 Jun 2020 16:09:09 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce846dc61a45df9d993497543ac474d7e5fd8ac7fbebaa3fa8a7f81fc2516b68`  
		Last Modified: Wed, 10 Jun 2020 16:09:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c842d78fea670830598639f4e6b3ad36bc8109e8a0169a66647e71ebb1a5c037`  
		Last Modified: Wed, 10 Jun 2020 16:09:09 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.7-windowsservercore-1809`

```console
$ docker pull nats@sha256:99209f1bc0877c1ac614efdb7985f2e5e5e77bff2d36a896816727429dff0d88
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `nats:2.1.7-windowsservercore-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull nats@sha256:fbdcfbf0773b8c7e2671b579b3b52400d4e8eca9d180bff2e5727f0a3d8d0864
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2307473223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6740ad609d50656fff721f580457edd9f2d4eba332ff31941549b128b84715f9`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 16:02:03 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Jun 2020 16:02:04 GMT
ENV NATS_SERVER=2.1.7
# Wed, 10 Jun 2020 16:02:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.7/nats-server-v2.1.7-windows-amd64.zip
# Wed, 10 Jun 2020 16:02:43 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Jun 2020 16:03:56 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 10 Jun 2020 16:03:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Jun 2020 16:03:58 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Jun 2020 16:03:59 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Jun 2020 16:04:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2192add29c9167423d378daa499903c4488337cdc2cf961ebeb0e4c0b492f9`  
		Last Modified: Wed, 10 Jun 2020 16:08:35 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a9b4e5c1b0529d2d48245b55ee7598147e2e80e110c5869d3d8be61369c5eb`  
		Last Modified: Wed, 10 Jun 2020 16:08:35 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c2e6ac9c7e61a2754411cf19adff6716f1e9301e89e68dd1ea7eb2a3b8cf8d`  
		Last Modified: Wed, 10 Jun 2020 16:08:34 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d98700f3301fe8993c249b37c71191744756fc10e53a69ffd98ec065fe27e43f`  
		Last Modified: Wed, 10 Jun 2020 16:08:36 GMT  
		Size: 4.8 MB (4764734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3494a6c6401e0ad8aedfe8e3894f88e5429c8cfd769fc50a4772f8da266df8b7`  
		Last Modified: Wed, 10 Jun 2020 16:08:34 GMT  
		Size: 8.8 MB (8784508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f3b6d9839159b8fa9ce12839aecab1ad582bbf2608244ba649076f938b2848`  
		Last Modified: Wed, 10 Jun 2020 16:08:32 GMT  
		Size: 1.7 KB (1702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c2e2690d3427b399abec715252650057d6a2549eba4cb2acaae27be4ebd5e0`  
		Last Modified: Wed, 10 Jun 2020 16:08:32 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4501d667c20eece078538960df5d805e0150b66e576e8d3cf89dca5499785d4b`  
		Last Modified: Wed, 10 Jun 2020 16:08:31 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16339bfc95d775f95c321531252cd1313eadd0df74728cb872aa8e1fec49af42`  
		Last Modified: Wed, 10 Jun 2020 16:08:32 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.7-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:c2e62e318eac246768f23032a9426cda29b6b24e10e4b2ffb15fe955c4e1020c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64

### `nats:2.1.7-windowsservercore-ltsc2016` - windows version 10.0.14393.3750; amd64

```console
$ docker pull nats@sha256:e32d961331b1efecafe08329ab9579dcd89035dbfc98ccd5ecd0124195c61b47
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5753367260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9e5cc77e49551b49ff66ed004535dff02071725ccf10441495e760de85b0aeb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 16:04:27 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Jun 2020 16:04:28 GMT
ENV NATS_SERVER=2.1.7
# Wed, 10 Jun 2020 16:04:29 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.7/nats-server-v2.1.7-windows-amd64.zip
# Wed, 10 Jun 2020 16:05:49 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Jun 2020 16:07:56 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 10 Jun 2020 16:07:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Jun 2020 16:08:00 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Jun 2020 16:08:01 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Jun 2020 16:08:02 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f945dc3cc7d024d3f86a74f177545b57d99c3209592a625bb655bf01921d2c`  
		Last Modified: Wed, 10 Jun 2020 16:09:12 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ae6d270564022284992180f4fd75553672266c2ac3ddfe37fcda523777d5d4`  
		Last Modified: Wed, 10 Jun 2020 16:09:12 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8835d3a93f1398493ed2485d211c2eaae6b2f63edaa2ad57b730e64ebe89d90a`  
		Last Modified: Wed, 10 Jun 2020 16:09:11 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b240ea1a26e00edd4b16bdbbe0af06d5cf97b87f869b97d75339b3db6bb5201d`  
		Last Modified: Wed, 10 Jun 2020 16:09:13 GMT  
		Size: 5.4 MB (5390325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dea13e836f486c4c268d4f38ad5227bfb7a088e2ce55dd1c1cdc37141d9a2c8`  
		Last Modified: Wed, 10 Jun 2020 16:09:26 GMT  
		Size: 14.0 MB (13969545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038f152d17356e6f5f3e4cddca5abe8c49f44535b31fddbbf6f92c71972dd08d`  
		Last Modified: Wed, 10 Jun 2020 16:09:09 GMT  
		Size: 1.7 KB (1675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b3323f04d21e510ede92022b9360017f11ac36acdb708ba7ccc23057653d07`  
		Last Modified: Wed, 10 Jun 2020 16:09:09 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce846dc61a45df9d993497543ac474d7e5fd8ac7fbebaa3fa8a7f81fc2516b68`  
		Last Modified: Wed, 10 Jun 2020 16:09:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c842d78fea670830598639f4e6b3ad36bc8109e8a0169a66647e71ebb1a5c037`  
		Last Modified: Wed, 10 Jun 2020 16:09:09 GMT  
		Size: 1.1 KB (1149 bytes)  
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
$ docker pull nats@sha256:d2f7f2b6e7ef60042e06a03f94573e6aab5cd1f073f476f9efec62f527a59689
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `nats:2.1-nanoserver` - windows version 10.0.17763.1282; amd64

```console
$ docker pull nats@sha256:23c3043b7d852c7a960b62141f08843223754582d236eb2e9610b349c110ce30
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105104931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d94790e871ec07154936db07dcf840f87ed91dbe648823dd3ab3bfd35cee85d`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 03 Jun 2020 11:12:32 GMT
RUN Apply image 1809-amd64
# Wed, 10 Jun 2020 16:04:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Jun 2020 16:04:16 GMT
RUN cmd /S /C #(nop) COPY file:18561b827240029ad80d0e3d25142efae62905c30cc520fc37cfc68e7d889848 in C:\nats-server.exe 
# Wed, 10 Jun 2020 16:04:18 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Jun 2020 16:04:19 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 Jun 2020 16:04:19 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Jun 2020 16:04:20 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c7d6d47ff7dfb2aa4d4e819641b93ec971e8541978dff0ffc24c193babeb8c07`  
		Size: 101.0 MB (101043386 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fd97aa6008f57e8475bff231216617c39835f885adb6a9c73a3a1599e2d788b9`  
		Last Modified: Wed, 10 Jun 2020 16:08:53 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550b5fdbee6a185b325bc673ac4059474353d34cc82ee5722edc4dca721c3c5a`  
		Last Modified: Wed, 10 Jun 2020 16:08:52 GMT  
		Size: 4.1 MB (4056494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ee7df3dace6c97838bc1bdecdff255d7e67bbec225868420ce6f188538c17a`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db8b53011d85727f476a78b4ad3a21cad54684c2ce7dac2011db5f3be7a2312`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9cac1f94d61b8883bdd4f0af6741b02ba9bb5df9bc58fa289e792f40f25310`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 918.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1306722d16f58c9f328a577068e5aea75b105b9d09dc8ad19a48734418ee276b`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-nanoserver-1809`

```console
$ docker pull nats@sha256:d2f7f2b6e7ef60042e06a03f94573e6aab5cd1f073f476f9efec62f527a59689
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `nats:2.1-nanoserver-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull nats@sha256:23c3043b7d852c7a960b62141f08843223754582d236eb2e9610b349c110ce30
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105104931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d94790e871ec07154936db07dcf840f87ed91dbe648823dd3ab3bfd35cee85d`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 03 Jun 2020 11:12:32 GMT
RUN Apply image 1809-amd64
# Wed, 10 Jun 2020 16:04:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Jun 2020 16:04:16 GMT
RUN cmd /S /C #(nop) COPY file:18561b827240029ad80d0e3d25142efae62905c30cc520fc37cfc68e7d889848 in C:\nats-server.exe 
# Wed, 10 Jun 2020 16:04:18 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Jun 2020 16:04:19 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 Jun 2020 16:04:19 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Jun 2020 16:04:20 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c7d6d47ff7dfb2aa4d4e819641b93ec971e8541978dff0ffc24c193babeb8c07`  
		Size: 101.0 MB (101043386 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fd97aa6008f57e8475bff231216617c39835f885adb6a9c73a3a1599e2d788b9`  
		Last Modified: Wed, 10 Jun 2020 16:08:53 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550b5fdbee6a185b325bc673ac4059474353d34cc82ee5722edc4dca721c3c5a`  
		Last Modified: Wed, 10 Jun 2020 16:08:52 GMT  
		Size: 4.1 MB (4056494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ee7df3dace6c97838bc1bdecdff255d7e67bbec225868420ce6f188538c17a`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db8b53011d85727f476a78b4ad3a21cad54684c2ce7dac2011db5f3be7a2312`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9cac1f94d61b8883bdd4f0af6741b02ba9bb5df9bc58fa289e792f40f25310`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 918.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1306722d16f58c9f328a577068e5aea75b105b9d09dc8ad19a48734418ee276b`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 895.0 B  
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
$ docker pull nats@sha256:fa6675e4c8e617650d11e3f132ede6070c024a9157e1d7d0e895c6cf6a4e3940
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64
	-	windows version 10.0.14393.3750; amd64

### `nats:2.1-windowsservercore` - windows version 10.0.17763.1282; amd64

```console
$ docker pull nats@sha256:fbdcfbf0773b8c7e2671b579b3b52400d4e8eca9d180bff2e5727f0a3d8d0864
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2307473223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6740ad609d50656fff721f580457edd9f2d4eba332ff31941549b128b84715f9`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 16:02:03 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Jun 2020 16:02:04 GMT
ENV NATS_SERVER=2.1.7
# Wed, 10 Jun 2020 16:02:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.7/nats-server-v2.1.7-windows-amd64.zip
# Wed, 10 Jun 2020 16:02:43 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Jun 2020 16:03:56 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 10 Jun 2020 16:03:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Jun 2020 16:03:58 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Jun 2020 16:03:59 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Jun 2020 16:04:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2192add29c9167423d378daa499903c4488337cdc2cf961ebeb0e4c0b492f9`  
		Last Modified: Wed, 10 Jun 2020 16:08:35 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a9b4e5c1b0529d2d48245b55ee7598147e2e80e110c5869d3d8be61369c5eb`  
		Last Modified: Wed, 10 Jun 2020 16:08:35 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c2e6ac9c7e61a2754411cf19adff6716f1e9301e89e68dd1ea7eb2a3b8cf8d`  
		Last Modified: Wed, 10 Jun 2020 16:08:34 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d98700f3301fe8993c249b37c71191744756fc10e53a69ffd98ec065fe27e43f`  
		Last Modified: Wed, 10 Jun 2020 16:08:36 GMT  
		Size: 4.8 MB (4764734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3494a6c6401e0ad8aedfe8e3894f88e5429c8cfd769fc50a4772f8da266df8b7`  
		Last Modified: Wed, 10 Jun 2020 16:08:34 GMT  
		Size: 8.8 MB (8784508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f3b6d9839159b8fa9ce12839aecab1ad582bbf2608244ba649076f938b2848`  
		Last Modified: Wed, 10 Jun 2020 16:08:32 GMT  
		Size: 1.7 KB (1702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c2e2690d3427b399abec715252650057d6a2549eba4cb2acaae27be4ebd5e0`  
		Last Modified: Wed, 10 Jun 2020 16:08:32 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4501d667c20eece078538960df5d805e0150b66e576e8d3cf89dca5499785d4b`  
		Last Modified: Wed, 10 Jun 2020 16:08:31 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16339bfc95d775f95c321531252cd1313eadd0df74728cb872aa8e1fec49af42`  
		Last Modified: Wed, 10 Jun 2020 16:08:32 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-windowsservercore` - windows version 10.0.14393.3750; amd64

```console
$ docker pull nats@sha256:e32d961331b1efecafe08329ab9579dcd89035dbfc98ccd5ecd0124195c61b47
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5753367260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9e5cc77e49551b49ff66ed004535dff02071725ccf10441495e760de85b0aeb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 16:04:27 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Jun 2020 16:04:28 GMT
ENV NATS_SERVER=2.1.7
# Wed, 10 Jun 2020 16:04:29 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.7/nats-server-v2.1.7-windows-amd64.zip
# Wed, 10 Jun 2020 16:05:49 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Jun 2020 16:07:56 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 10 Jun 2020 16:07:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Jun 2020 16:08:00 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Jun 2020 16:08:01 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Jun 2020 16:08:02 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f945dc3cc7d024d3f86a74f177545b57d99c3209592a625bb655bf01921d2c`  
		Last Modified: Wed, 10 Jun 2020 16:09:12 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ae6d270564022284992180f4fd75553672266c2ac3ddfe37fcda523777d5d4`  
		Last Modified: Wed, 10 Jun 2020 16:09:12 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8835d3a93f1398493ed2485d211c2eaae6b2f63edaa2ad57b730e64ebe89d90a`  
		Last Modified: Wed, 10 Jun 2020 16:09:11 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b240ea1a26e00edd4b16bdbbe0af06d5cf97b87f869b97d75339b3db6bb5201d`  
		Last Modified: Wed, 10 Jun 2020 16:09:13 GMT  
		Size: 5.4 MB (5390325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dea13e836f486c4c268d4f38ad5227bfb7a088e2ce55dd1c1cdc37141d9a2c8`  
		Last Modified: Wed, 10 Jun 2020 16:09:26 GMT  
		Size: 14.0 MB (13969545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038f152d17356e6f5f3e4cddca5abe8c49f44535b31fddbbf6f92c71972dd08d`  
		Last Modified: Wed, 10 Jun 2020 16:09:09 GMT  
		Size: 1.7 KB (1675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b3323f04d21e510ede92022b9360017f11ac36acdb708ba7ccc23057653d07`  
		Last Modified: Wed, 10 Jun 2020 16:09:09 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce846dc61a45df9d993497543ac474d7e5fd8ac7fbebaa3fa8a7f81fc2516b68`  
		Last Modified: Wed, 10 Jun 2020 16:09:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c842d78fea670830598639f4e6b3ad36bc8109e8a0169a66647e71ebb1a5c037`  
		Last Modified: Wed, 10 Jun 2020 16:09:09 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-windowsservercore-1809`

```console
$ docker pull nats@sha256:99209f1bc0877c1ac614efdb7985f2e5e5e77bff2d36a896816727429dff0d88
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `nats:2.1-windowsservercore-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull nats@sha256:fbdcfbf0773b8c7e2671b579b3b52400d4e8eca9d180bff2e5727f0a3d8d0864
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2307473223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6740ad609d50656fff721f580457edd9f2d4eba332ff31941549b128b84715f9`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 16:02:03 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Jun 2020 16:02:04 GMT
ENV NATS_SERVER=2.1.7
# Wed, 10 Jun 2020 16:02:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.7/nats-server-v2.1.7-windows-amd64.zip
# Wed, 10 Jun 2020 16:02:43 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Jun 2020 16:03:56 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 10 Jun 2020 16:03:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Jun 2020 16:03:58 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Jun 2020 16:03:59 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Jun 2020 16:04:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2192add29c9167423d378daa499903c4488337cdc2cf961ebeb0e4c0b492f9`  
		Last Modified: Wed, 10 Jun 2020 16:08:35 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a9b4e5c1b0529d2d48245b55ee7598147e2e80e110c5869d3d8be61369c5eb`  
		Last Modified: Wed, 10 Jun 2020 16:08:35 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c2e6ac9c7e61a2754411cf19adff6716f1e9301e89e68dd1ea7eb2a3b8cf8d`  
		Last Modified: Wed, 10 Jun 2020 16:08:34 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d98700f3301fe8993c249b37c71191744756fc10e53a69ffd98ec065fe27e43f`  
		Last Modified: Wed, 10 Jun 2020 16:08:36 GMT  
		Size: 4.8 MB (4764734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3494a6c6401e0ad8aedfe8e3894f88e5429c8cfd769fc50a4772f8da266df8b7`  
		Last Modified: Wed, 10 Jun 2020 16:08:34 GMT  
		Size: 8.8 MB (8784508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f3b6d9839159b8fa9ce12839aecab1ad582bbf2608244ba649076f938b2848`  
		Last Modified: Wed, 10 Jun 2020 16:08:32 GMT  
		Size: 1.7 KB (1702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c2e2690d3427b399abec715252650057d6a2549eba4cb2acaae27be4ebd5e0`  
		Last Modified: Wed, 10 Jun 2020 16:08:32 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4501d667c20eece078538960df5d805e0150b66e576e8d3cf89dca5499785d4b`  
		Last Modified: Wed, 10 Jun 2020 16:08:31 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16339bfc95d775f95c321531252cd1313eadd0df74728cb872aa8e1fec49af42`  
		Last Modified: Wed, 10 Jun 2020 16:08:32 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:c2e62e318eac246768f23032a9426cda29b6b24e10e4b2ffb15fe955c4e1020c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64

### `nats:2.1-windowsservercore-ltsc2016` - windows version 10.0.14393.3750; amd64

```console
$ docker pull nats@sha256:e32d961331b1efecafe08329ab9579dcd89035dbfc98ccd5ecd0124195c61b47
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5753367260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9e5cc77e49551b49ff66ed004535dff02071725ccf10441495e760de85b0aeb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 16:04:27 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Jun 2020 16:04:28 GMT
ENV NATS_SERVER=2.1.7
# Wed, 10 Jun 2020 16:04:29 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.7/nats-server-v2.1.7-windows-amd64.zip
# Wed, 10 Jun 2020 16:05:49 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Jun 2020 16:07:56 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 10 Jun 2020 16:07:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Jun 2020 16:08:00 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Jun 2020 16:08:01 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Jun 2020 16:08:02 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f945dc3cc7d024d3f86a74f177545b57d99c3209592a625bb655bf01921d2c`  
		Last Modified: Wed, 10 Jun 2020 16:09:12 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ae6d270564022284992180f4fd75553672266c2ac3ddfe37fcda523777d5d4`  
		Last Modified: Wed, 10 Jun 2020 16:09:12 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8835d3a93f1398493ed2485d211c2eaae6b2f63edaa2ad57b730e64ebe89d90a`  
		Last Modified: Wed, 10 Jun 2020 16:09:11 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b240ea1a26e00edd4b16bdbbe0af06d5cf97b87f869b97d75339b3db6bb5201d`  
		Last Modified: Wed, 10 Jun 2020 16:09:13 GMT  
		Size: 5.4 MB (5390325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dea13e836f486c4c268d4f38ad5227bfb7a088e2ce55dd1c1cdc37141d9a2c8`  
		Last Modified: Wed, 10 Jun 2020 16:09:26 GMT  
		Size: 14.0 MB (13969545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038f152d17356e6f5f3e4cddca5abe8c49f44535b31fddbbf6f92c71972dd08d`  
		Last Modified: Wed, 10 Jun 2020 16:09:09 GMT  
		Size: 1.7 KB (1675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b3323f04d21e510ede92022b9360017f11ac36acdb708ba7ccc23057653d07`  
		Last Modified: Wed, 10 Jun 2020 16:09:09 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce846dc61a45df9d993497543ac474d7e5fd8ac7fbebaa3fa8a7f81fc2516b68`  
		Last Modified: Wed, 10 Jun 2020 16:09:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c842d78fea670830598639f4e6b3ad36bc8109e8a0169a66647e71ebb1a5c037`  
		Last Modified: Wed, 10 Jun 2020 16:09:09 GMT  
		Size: 1.1 KB (1149 bytes)  
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
$ docker pull nats@sha256:d2f7f2b6e7ef60042e06a03f94573e6aab5cd1f073f476f9efec62f527a59689
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.1282; amd64

```console
$ docker pull nats@sha256:23c3043b7d852c7a960b62141f08843223754582d236eb2e9610b349c110ce30
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105104931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d94790e871ec07154936db07dcf840f87ed91dbe648823dd3ab3bfd35cee85d`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 03 Jun 2020 11:12:32 GMT
RUN Apply image 1809-amd64
# Wed, 10 Jun 2020 16:04:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Jun 2020 16:04:16 GMT
RUN cmd /S /C #(nop) COPY file:18561b827240029ad80d0e3d25142efae62905c30cc520fc37cfc68e7d889848 in C:\nats-server.exe 
# Wed, 10 Jun 2020 16:04:18 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Jun 2020 16:04:19 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 Jun 2020 16:04:19 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Jun 2020 16:04:20 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c7d6d47ff7dfb2aa4d4e819641b93ec971e8541978dff0ffc24c193babeb8c07`  
		Size: 101.0 MB (101043386 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fd97aa6008f57e8475bff231216617c39835f885adb6a9c73a3a1599e2d788b9`  
		Last Modified: Wed, 10 Jun 2020 16:08:53 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550b5fdbee6a185b325bc673ac4059474353d34cc82ee5722edc4dca721c3c5a`  
		Last Modified: Wed, 10 Jun 2020 16:08:52 GMT  
		Size: 4.1 MB (4056494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ee7df3dace6c97838bc1bdecdff255d7e67bbec225868420ce6f188538c17a`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db8b53011d85727f476a78b4ad3a21cad54684c2ce7dac2011db5f3be7a2312`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9cac1f94d61b8883bdd4f0af6741b02ba9bb5df9bc58fa289e792f40f25310`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 918.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1306722d16f58c9f328a577068e5aea75b105b9d09dc8ad19a48734418ee276b`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:d2f7f2b6e7ef60042e06a03f94573e6aab5cd1f073f476f9efec62f527a59689
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull nats@sha256:23c3043b7d852c7a960b62141f08843223754582d236eb2e9610b349c110ce30
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105104931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d94790e871ec07154936db07dcf840f87ed91dbe648823dd3ab3bfd35cee85d`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 03 Jun 2020 11:12:32 GMT
RUN Apply image 1809-amd64
# Wed, 10 Jun 2020 16:04:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Jun 2020 16:04:16 GMT
RUN cmd /S /C #(nop) COPY file:18561b827240029ad80d0e3d25142efae62905c30cc520fc37cfc68e7d889848 in C:\nats-server.exe 
# Wed, 10 Jun 2020 16:04:18 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Jun 2020 16:04:19 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 Jun 2020 16:04:19 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Jun 2020 16:04:20 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c7d6d47ff7dfb2aa4d4e819641b93ec971e8541978dff0ffc24c193babeb8c07`  
		Size: 101.0 MB (101043386 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fd97aa6008f57e8475bff231216617c39835f885adb6a9c73a3a1599e2d788b9`  
		Last Modified: Wed, 10 Jun 2020 16:08:53 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550b5fdbee6a185b325bc673ac4059474353d34cc82ee5722edc4dca721c3c5a`  
		Last Modified: Wed, 10 Jun 2020 16:08:52 GMT  
		Size: 4.1 MB (4056494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ee7df3dace6c97838bc1bdecdff255d7e67bbec225868420ce6f188538c17a`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db8b53011d85727f476a78b4ad3a21cad54684c2ce7dac2011db5f3be7a2312`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9cac1f94d61b8883bdd4f0af6741b02ba9bb5df9bc58fa289e792f40f25310`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 918.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1306722d16f58c9f328a577068e5aea75b105b9d09dc8ad19a48734418ee276b`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 895.0 B  
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
$ docker pull nats@sha256:fa6675e4c8e617650d11e3f132ede6070c024a9157e1d7d0e895c6cf6a4e3940
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64
	-	windows version 10.0.14393.3750; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.1282; amd64

```console
$ docker pull nats@sha256:fbdcfbf0773b8c7e2671b579b3b52400d4e8eca9d180bff2e5727f0a3d8d0864
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2307473223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6740ad609d50656fff721f580457edd9f2d4eba332ff31941549b128b84715f9`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 16:02:03 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Jun 2020 16:02:04 GMT
ENV NATS_SERVER=2.1.7
# Wed, 10 Jun 2020 16:02:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.7/nats-server-v2.1.7-windows-amd64.zip
# Wed, 10 Jun 2020 16:02:43 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Jun 2020 16:03:56 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 10 Jun 2020 16:03:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Jun 2020 16:03:58 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Jun 2020 16:03:59 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Jun 2020 16:04:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2192add29c9167423d378daa499903c4488337cdc2cf961ebeb0e4c0b492f9`  
		Last Modified: Wed, 10 Jun 2020 16:08:35 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a9b4e5c1b0529d2d48245b55ee7598147e2e80e110c5869d3d8be61369c5eb`  
		Last Modified: Wed, 10 Jun 2020 16:08:35 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c2e6ac9c7e61a2754411cf19adff6716f1e9301e89e68dd1ea7eb2a3b8cf8d`  
		Last Modified: Wed, 10 Jun 2020 16:08:34 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d98700f3301fe8993c249b37c71191744756fc10e53a69ffd98ec065fe27e43f`  
		Last Modified: Wed, 10 Jun 2020 16:08:36 GMT  
		Size: 4.8 MB (4764734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3494a6c6401e0ad8aedfe8e3894f88e5429c8cfd769fc50a4772f8da266df8b7`  
		Last Modified: Wed, 10 Jun 2020 16:08:34 GMT  
		Size: 8.8 MB (8784508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f3b6d9839159b8fa9ce12839aecab1ad582bbf2608244ba649076f938b2848`  
		Last Modified: Wed, 10 Jun 2020 16:08:32 GMT  
		Size: 1.7 KB (1702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c2e2690d3427b399abec715252650057d6a2549eba4cb2acaae27be4ebd5e0`  
		Last Modified: Wed, 10 Jun 2020 16:08:32 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4501d667c20eece078538960df5d805e0150b66e576e8d3cf89dca5499785d4b`  
		Last Modified: Wed, 10 Jun 2020 16:08:31 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16339bfc95d775f95c321531252cd1313eadd0df74728cb872aa8e1fec49af42`  
		Last Modified: Wed, 10 Jun 2020 16:08:32 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-windowsservercore` - windows version 10.0.14393.3750; amd64

```console
$ docker pull nats@sha256:e32d961331b1efecafe08329ab9579dcd89035dbfc98ccd5ecd0124195c61b47
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5753367260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9e5cc77e49551b49ff66ed004535dff02071725ccf10441495e760de85b0aeb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 16:04:27 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Jun 2020 16:04:28 GMT
ENV NATS_SERVER=2.1.7
# Wed, 10 Jun 2020 16:04:29 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.7/nats-server-v2.1.7-windows-amd64.zip
# Wed, 10 Jun 2020 16:05:49 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Jun 2020 16:07:56 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 10 Jun 2020 16:07:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Jun 2020 16:08:00 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Jun 2020 16:08:01 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Jun 2020 16:08:02 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f945dc3cc7d024d3f86a74f177545b57d99c3209592a625bb655bf01921d2c`  
		Last Modified: Wed, 10 Jun 2020 16:09:12 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ae6d270564022284992180f4fd75553672266c2ac3ddfe37fcda523777d5d4`  
		Last Modified: Wed, 10 Jun 2020 16:09:12 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8835d3a93f1398493ed2485d211c2eaae6b2f63edaa2ad57b730e64ebe89d90a`  
		Last Modified: Wed, 10 Jun 2020 16:09:11 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b240ea1a26e00edd4b16bdbbe0af06d5cf97b87f869b97d75339b3db6bb5201d`  
		Last Modified: Wed, 10 Jun 2020 16:09:13 GMT  
		Size: 5.4 MB (5390325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dea13e836f486c4c268d4f38ad5227bfb7a088e2ce55dd1c1cdc37141d9a2c8`  
		Last Modified: Wed, 10 Jun 2020 16:09:26 GMT  
		Size: 14.0 MB (13969545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038f152d17356e6f5f3e4cddca5abe8c49f44535b31fddbbf6f92c71972dd08d`  
		Last Modified: Wed, 10 Jun 2020 16:09:09 GMT  
		Size: 1.7 KB (1675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b3323f04d21e510ede92022b9360017f11ac36acdb708ba7ccc23057653d07`  
		Last Modified: Wed, 10 Jun 2020 16:09:09 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce846dc61a45df9d993497543ac474d7e5fd8ac7fbebaa3fa8a7f81fc2516b68`  
		Last Modified: Wed, 10 Jun 2020 16:09:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c842d78fea670830598639f4e6b3ad36bc8109e8a0169a66647e71ebb1a5c037`  
		Last Modified: Wed, 10 Jun 2020 16:09:09 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:99209f1bc0877c1ac614efdb7985f2e5e5e77bff2d36a896816727429dff0d88
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull nats@sha256:fbdcfbf0773b8c7e2671b579b3b52400d4e8eca9d180bff2e5727f0a3d8d0864
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2307473223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6740ad609d50656fff721f580457edd9f2d4eba332ff31941549b128b84715f9`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 16:02:03 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Jun 2020 16:02:04 GMT
ENV NATS_SERVER=2.1.7
# Wed, 10 Jun 2020 16:02:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.7/nats-server-v2.1.7-windows-amd64.zip
# Wed, 10 Jun 2020 16:02:43 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Jun 2020 16:03:56 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 10 Jun 2020 16:03:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Jun 2020 16:03:58 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Jun 2020 16:03:59 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Jun 2020 16:04:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2192add29c9167423d378daa499903c4488337cdc2cf961ebeb0e4c0b492f9`  
		Last Modified: Wed, 10 Jun 2020 16:08:35 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a9b4e5c1b0529d2d48245b55ee7598147e2e80e110c5869d3d8be61369c5eb`  
		Last Modified: Wed, 10 Jun 2020 16:08:35 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c2e6ac9c7e61a2754411cf19adff6716f1e9301e89e68dd1ea7eb2a3b8cf8d`  
		Last Modified: Wed, 10 Jun 2020 16:08:34 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d98700f3301fe8993c249b37c71191744756fc10e53a69ffd98ec065fe27e43f`  
		Last Modified: Wed, 10 Jun 2020 16:08:36 GMT  
		Size: 4.8 MB (4764734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3494a6c6401e0ad8aedfe8e3894f88e5429c8cfd769fc50a4772f8da266df8b7`  
		Last Modified: Wed, 10 Jun 2020 16:08:34 GMT  
		Size: 8.8 MB (8784508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f3b6d9839159b8fa9ce12839aecab1ad582bbf2608244ba649076f938b2848`  
		Last Modified: Wed, 10 Jun 2020 16:08:32 GMT  
		Size: 1.7 KB (1702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c2e2690d3427b399abec715252650057d6a2549eba4cb2acaae27be4ebd5e0`  
		Last Modified: Wed, 10 Jun 2020 16:08:32 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4501d667c20eece078538960df5d805e0150b66e576e8d3cf89dca5499785d4b`  
		Last Modified: Wed, 10 Jun 2020 16:08:31 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16339bfc95d775f95c321531252cd1313eadd0df74728cb872aa8e1fec49af42`  
		Last Modified: Wed, 10 Jun 2020 16:08:32 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:c2e62e318eac246768f23032a9426cda29b6b24e10e4b2ffb15fe955c4e1020c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64

### `nats:2-windowsservercore-ltsc2016` - windows version 10.0.14393.3750; amd64

```console
$ docker pull nats@sha256:e32d961331b1efecafe08329ab9579dcd89035dbfc98ccd5ecd0124195c61b47
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5753367260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9e5cc77e49551b49ff66ed004535dff02071725ccf10441495e760de85b0aeb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 16:04:27 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Jun 2020 16:04:28 GMT
ENV NATS_SERVER=2.1.7
# Wed, 10 Jun 2020 16:04:29 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.7/nats-server-v2.1.7-windows-amd64.zip
# Wed, 10 Jun 2020 16:05:49 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Jun 2020 16:07:56 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 10 Jun 2020 16:07:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Jun 2020 16:08:00 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Jun 2020 16:08:01 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Jun 2020 16:08:02 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f945dc3cc7d024d3f86a74f177545b57d99c3209592a625bb655bf01921d2c`  
		Last Modified: Wed, 10 Jun 2020 16:09:12 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ae6d270564022284992180f4fd75553672266c2ac3ddfe37fcda523777d5d4`  
		Last Modified: Wed, 10 Jun 2020 16:09:12 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8835d3a93f1398493ed2485d211c2eaae6b2f63edaa2ad57b730e64ebe89d90a`  
		Last Modified: Wed, 10 Jun 2020 16:09:11 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b240ea1a26e00edd4b16bdbbe0af06d5cf97b87f869b97d75339b3db6bb5201d`  
		Last Modified: Wed, 10 Jun 2020 16:09:13 GMT  
		Size: 5.4 MB (5390325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dea13e836f486c4c268d4f38ad5227bfb7a088e2ce55dd1c1cdc37141d9a2c8`  
		Last Modified: Wed, 10 Jun 2020 16:09:26 GMT  
		Size: 14.0 MB (13969545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038f152d17356e6f5f3e4cddca5abe8c49f44535b31fddbbf6f92c71972dd08d`  
		Last Modified: Wed, 10 Jun 2020 16:09:09 GMT  
		Size: 1.7 KB (1675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b3323f04d21e510ede92022b9360017f11ac36acdb708ba7ccc23057653d07`  
		Last Modified: Wed, 10 Jun 2020 16:09:09 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce846dc61a45df9d993497543ac474d7e5fd8ac7fbebaa3fa8a7f81fc2516b68`  
		Last Modified: Wed, 10 Jun 2020 16:09:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c842d78fea670830598639f4e6b3ad36bc8109e8a0169a66647e71ebb1a5c037`  
		Last Modified: Wed, 10 Jun 2020 16:09:09 GMT  
		Size: 1.1 KB (1149 bytes)  
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
$ docker pull nats@sha256:1dcedfdb0d872fe1394759ac6eb3d1176dfd50bf8c2e2ef74349ea3bac1fe4d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1282; amd64

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

### `nats:latest` - windows version 10.0.17763.1282; amd64

```console
$ docker pull nats@sha256:23c3043b7d852c7a960b62141f08843223754582d236eb2e9610b349c110ce30
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105104931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d94790e871ec07154936db07dcf840f87ed91dbe648823dd3ab3bfd35cee85d`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 03 Jun 2020 11:12:32 GMT
RUN Apply image 1809-amd64
# Wed, 10 Jun 2020 16:04:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Jun 2020 16:04:16 GMT
RUN cmd /S /C #(nop) COPY file:18561b827240029ad80d0e3d25142efae62905c30cc520fc37cfc68e7d889848 in C:\nats-server.exe 
# Wed, 10 Jun 2020 16:04:18 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Jun 2020 16:04:19 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 Jun 2020 16:04:19 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Jun 2020 16:04:20 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c7d6d47ff7dfb2aa4d4e819641b93ec971e8541978dff0ffc24c193babeb8c07`  
		Size: 101.0 MB (101043386 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fd97aa6008f57e8475bff231216617c39835f885adb6a9c73a3a1599e2d788b9`  
		Last Modified: Wed, 10 Jun 2020 16:08:53 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550b5fdbee6a185b325bc673ac4059474353d34cc82ee5722edc4dca721c3c5a`  
		Last Modified: Wed, 10 Jun 2020 16:08:52 GMT  
		Size: 4.1 MB (4056494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ee7df3dace6c97838bc1bdecdff255d7e67bbec225868420ce6f188538c17a`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db8b53011d85727f476a78b4ad3a21cad54684c2ce7dac2011db5f3be7a2312`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9cac1f94d61b8883bdd4f0af6741b02ba9bb5df9bc58fa289e792f40f25310`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 918.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1306722d16f58c9f328a577068e5aea75b105b9d09dc8ad19a48734418ee276b`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 895.0 B  
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
$ docker pull nats@sha256:d2f7f2b6e7ef60042e06a03f94573e6aab5cd1f073f476f9efec62f527a59689
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `nats:nanoserver` - windows version 10.0.17763.1282; amd64

```console
$ docker pull nats@sha256:23c3043b7d852c7a960b62141f08843223754582d236eb2e9610b349c110ce30
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105104931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d94790e871ec07154936db07dcf840f87ed91dbe648823dd3ab3bfd35cee85d`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 03 Jun 2020 11:12:32 GMT
RUN Apply image 1809-amd64
# Wed, 10 Jun 2020 16:04:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Jun 2020 16:04:16 GMT
RUN cmd /S /C #(nop) COPY file:18561b827240029ad80d0e3d25142efae62905c30cc520fc37cfc68e7d889848 in C:\nats-server.exe 
# Wed, 10 Jun 2020 16:04:18 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Jun 2020 16:04:19 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 Jun 2020 16:04:19 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Jun 2020 16:04:20 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c7d6d47ff7dfb2aa4d4e819641b93ec971e8541978dff0ffc24c193babeb8c07`  
		Size: 101.0 MB (101043386 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fd97aa6008f57e8475bff231216617c39835f885adb6a9c73a3a1599e2d788b9`  
		Last Modified: Wed, 10 Jun 2020 16:08:53 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550b5fdbee6a185b325bc673ac4059474353d34cc82ee5722edc4dca721c3c5a`  
		Last Modified: Wed, 10 Jun 2020 16:08:52 GMT  
		Size: 4.1 MB (4056494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ee7df3dace6c97838bc1bdecdff255d7e67bbec225868420ce6f188538c17a`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db8b53011d85727f476a78b4ad3a21cad54684c2ce7dac2011db5f3be7a2312`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9cac1f94d61b8883bdd4f0af6741b02ba9bb5df9bc58fa289e792f40f25310`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 918.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1306722d16f58c9f328a577068e5aea75b105b9d09dc8ad19a48734418ee276b`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:d2f7f2b6e7ef60042e06a03f94573e6aab5cd1f073f476f9efec62f527a59689
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull nats@sha256:23c3043b7d852c7a960b62141f08843223754582d236eb2e9610b349c110ce30
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105104931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d94790e871ec07154936db07dcf840f87ed91dbe648823dd3ab3bfd35cee85d`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 03 Jun 2020 11:12:32 GMT
RUN Apply image 1809-amd64
# Wed, 10 Jun 2020 16:04:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Jun 2020 16:04:16 GMT
RUN cmd /S /C #(nop) COPY file:18561b827240029ad80d0e3d25142efae62905c30cc520fc37cfc68e7d889848 in C:\nats-server.exe 
# Wed, 10 Jun 2020 16:04:18 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Jun 2020 16:04:19 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 Jun 2020 16:04:19 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Jun 2020 16:04:20 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c7d6d47ff7dfb2aa4d4e819641b93ec971e8541978dff0ffc24c193babeb8c07`  
		Size: 101.0 MB (101043386 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fd97aa6008f57e8475bff231216617c39835f885adb6a9c73a3a1599e2d788b9`  
		Last Modified: Wed, 10 Jun 2020 16:08:53 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550b5fdbee6a185b325bc673ac4059474353d34cc82ee5722edc4dca721c3c5a`  
		Last Modified: Wed, 10 Jun 2020 16:08:52 GMT  
		Size: 4.1 MB (4056494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ee7df3dace6c97838bc1bdecdff255d7e67bbec225868420ce6f188538c17a`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db8b53011d85727f476a78b4ad3a21cad54684c2ce7dac2011db5f3be7a2312`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9cac1f94d61b8883bdd4f0af6741b02ba9bb5df9bc58fa289e792f40f25310`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 918.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1306722d16f58c9f328a577068e5aea75b105b9d09dc8ad19a48734418ee276b`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 895.0 B  
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
$ docker pull nats@sha256:fa6675e4c8e617650d11e3f132ede6070c024a9157e1d7d0e895c6cf6a4e3940
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64
	-	windows version 10.0.14393.3750; amd64

### `nats:windowsservercore` - windows version 10.0.17763.1282; amd64

```console
$ docker pull nats@sha256:fbdcfbf0773b8c7e2671b579b3b52400d4e8eca9d180bff2e5727f0a3d8d0864
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2307473223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6740ad609d50656fff721f580457edd9f2d4eba332ff31941549b128b84715f9`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 16:02:03 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Jun 2020 16:02:04 GMT
ENV NATS_SERVER=2.1.7
# Wed, 10 Jun 2020 16:02:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.7/nats-server-v2.1.7-windows-amd64.zip
# Wed, 10 Jun 2020 16:02:43 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Jun 2020 16:03:56 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 10 Jun 2020 16:03:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Jun 2020 16:03:58 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Jun 2020 16:03:59 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Jun 2020 16:04:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2192add29c9167423d378daa499903c4488337cdc2cf961ebeb0e4c0b492f9`  
		Last Modified: Wed, 10 Jun 2020 16:08:35 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a9b4e5c1b0529d2d48245b55ee7598147e2e80e110c5869d3d8be61369c5eb`  
		Last Modified: Wed, 10 Jun 2020 16:08:35 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c2e6ac9c7e61a2754411cf19adff6716f1e9301e89e68dd1ea7eb2a3b8cf8d`  
		Last Modified: Wed, 10 Jun 2020 16:08:34 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d98700f3301fe8993c249b37c71191744756fc10e53a69ffd98ec065fe27e43f`  
		Last Modified: Wed, 10 Jun 2020 16:08:36 GMT  
		Size: 4.8 MB (4764734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3494a6c6401e0ad8aedfe8e3894f88e5429c8cfd769fc50a4772f8da266df8b7`  
		Last Modified: Wed, 10 Jun 2020 16:08:34 GMT  
		Size: 8.8 MB (8784508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f3b6d9839159b8fa9ce12839aecab1ad582bbf2608244ba649076f938b2848`  
		Last Modified: Wed, 10 Jun 2020 16:08:32 GMT  
		Size: 1.7 KB (1702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c2e2690d3427b399abec715252650057d6a2549eba4cb2acaae27be4ebd5e0`  
		Last Modified: Wed, 10 Jun 2020 16:08:32 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4501d667c20eece078538960df5d805e0150b66e576e8d3cf89dca5499785d4b`  
		Last Modified: Wed, 10 Jun 2020 16:08:31 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16339bfc95d775f95c321531252cd1313eadd0df74728cb872aa8e1fec49af42`  
		Last Modified: Wed, 10 Jun 2020 16:08:32 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:windowsservercore` - windows version 10.0.14393.3750; amd64

```console
$ docker pull nats@sha256:e32d961331b1efecafe08329ab9579dcd89035dbfc98ccd5ecd0124195c61b47
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5753367260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9e5cc77e49551b49ff66ed004535dff02071725ccf10441495e760de85b0aeb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 16:04:27 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Jun 2020 16:04:28 GMT
ENV NATS_SERVER=2.1.7
# Wed, 10 Jun 2020 16:04:29 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.7/nats-server-v2.1.7-windows-amd64.zip
# Wed, 10 Jun 2020 16:05:49 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Jun 2020 16:07:56 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 10 Jun 2020 16:07:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Jun 2020 16:08:00 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Jun 2020 16:08:01 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Jun 2020 16:08:02 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f945dc3cc7d024d3f86a74f177545b57d99c3209592a625bb655bf01921d2c`  
		Last Modified: Wed, 10 Jun 2020 16:09:12 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ae6d270564022284992180f4fd75553672266c2ac3ddfe37fcda523777d5d4`  
		Last Modified: Wed, 10 Jun 2020 16:09:12 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8835d3a93f1398493ed2485d211c2eaae6b2f63edaa2ad57b730e64ebe89d90a`  
		Last Modified: Wed, 10 Jun 2020 16:09:11 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b240ea1a26e00edd4b16bdbbe0af06d5cf97b87f869b97d75339b3db6bb5201d`  
		Last Modified: Wed, 10 Jun 2020 16:09:13 GMT  
		Size: 5.4 MB (5390325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dea13e836f486c4c268d4f38ad5227bfb7a088e2ce55dd1c1cdc37141d9a2c8`  
		Last Modified: Wed, 10 Jun 2020 16:09:26 GMT  
		Size: 14.0 MB (13969545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038f152d17356e6f5f3e4cddca5abe8c49f44535b31fddbbf6f92c71972dd08d`  
		Last Modified: Wed, 10 Jun 2020 16:09:09 GMT  
		Size: 1.7 KB (1675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b3323f04d21e510ede92022b9360017f11ac36acdb708ba7ccc23057653d07`  
		Last Modified: Wed, 10 Jun 2020 16:09:09 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce846dc61a45df9d993497543ac474d7e5fd8ac7fbebaa3fa8a7f81fc2516b68`  
		Last Modified: Wed, 10 Jun 2020 16:09:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c842d78fea670830598639f4e6b3ad36bc8109e8a0169a66647e71ebb1a5c037`  
		Last Modified: Wed, 10 Jun 2020 16:09:09 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:99209f1bc0877c1ac614efdb7985f2e5e5e77bff2d36a896816727429dff0d88
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull nats@sha256:fbdcfbf0773b8c7e2671b579b3b52400d4e8eca9d180bff2e5727f0a3d8d0864
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2307473223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6740ad609d50656fff721f580457edd9f2d4eba332ff31941549b128b84715f9`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 16:02:03 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Jun 2020 16:02:04 GMT
ENV NATS_SERVER=2.1.7
# Wed, 10 Jun 2020 16:02:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.7/nats-server-v2.1.7-windows-amd64.zip
# Wed, 10 Jun 2020 16:02:43 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Jun 2020 16:03:56 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 10 Jun 2020 16:03:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Jun 2020 16:03:58 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Jun 2020 16:03:59 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Jun 2020 16:04:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2192add29c9167423d378daa499903c4488337cdc2cf961ebeb0e4c0b492f9`  
		Last Modified: Wed, 10 Jun 2020 16:08:35 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a9b4e5c1b0529d2d48245b55ee7598147e2e80e110c5869d3d8be61369c5eb`  
		Last Modified: Wed, 10 Jun 2020 16:08:35 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c2e6ac9c7e61a2754411cf19adff6716f1e9301e89e68dd1ea7eb2a3b8cf8d`  
		Last Modified: Wed, 10 Jun 2020 16:08:34 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d98700f3301fe8993c249b37c71191744756fc10e53a69ffd98ec065fe27e43f`  
		Last Modified: Wed, 10 Jun 2020 16:08:36 GMT  
		Size: 4.8 MB (4764734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3494a6c6401e0ad8aedfe8e3894f88e5429c8cfd769fc50a4772f8da266df8b7`  
		Last Modified: Wed, 10 Jun 2020 16:08:34 GMT  
		Size: 8.8 MB (8784508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f3b6d9839159b8fa9ce12839aecab1ad582bbf2608244ba649076f938b2848`  
		Last Modified: Wed, 10 Jun 2020 16:08:32 GMT  
		Size: 1.7 KB (1702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c2e2690d3427b399abec715252650057d6a2549eba4cb2acaae27be4ebd5e0`  
		Last Modified: Wed, 10 Jun 2020 16:08:32 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4501d667c20eece078538960df5d805e0150b66e576e8d3cf89dca5499785d4b`  
		Last Modified: Wed, 10 Jun 2020 16:08:31 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16339bfc95d775f95c321531252cd1313eadd0df74728cb872aa8e1fec49af42`  
		Last Modified: Wed, 10 Jun 2020 16:08:32 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:c2e62e318eac246768f23032a9426cda29b6b24e10e4b2ffb15fe955c4e1020c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64

### `nats:windowsservercore-ltsc2016` - windows version 10.0.14393.3750; amd64

```console
$ docker pull nats@sha256:e32d961331b1efecafe08329ab9579dcd89035dbfc98ccd5ecd0124195c61b47
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5753367260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9e5cc77e49551b49ff66ed004535dff02071725ccf10441495e760de85b0aeb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 16:04:27 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Jun 2020 16:04:28 GMT
ENV NATS_SERVER=2.1.7
# Wed, 10 Jun 2020 16:04:29 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.7/nats-server-v2.1.7-windows-amd64.zip
# Wed, 10 Jun 2020 16:05:49 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Jun 2020 16:07:56 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 10 Jun 2020 16:07:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Jun 2020 16:08:00 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Jun 2020 16:08:01 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Jun 2020 16:08:02 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f945dc3cc7d024d3f86a74f177545b57d99c3209592a625bb655bf01921d2c`  
		Last Modified: Wed, 10 Jun 2020 16:09:12 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ae6d270564022284992180f4fd75553672266c2ac3ddfe37fcda523777d5d4`  
		Last Modified: Wed, 10 Jun 2020 16:09:12 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8835d3a93f1398493ed2485d211c2eaae6b2f63edaa2ad57b730e64ebe89d90a`  
		Last Modified: Wed, 10 Jun 2020 16:09:11 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b240ea1a26e00edd4b16bdbbe0af06d5cf97b87f869b97d75339b3db6bb5201d`  
		Last Modified: Wed, 10 Jun 2020 16:09:13 GMT  
		Size: 5.4 MB (5390325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dea13e836f486c4c268d4f38ad5227bfb7a088e2ce55dd1c1cdc37141d9a2c8`  
		Last Modified: Wed, 10 Jun 2020 16:09:26 GMT  
		Size: 14.0 MB (13969545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038f152d17356e6f5f3e4cddca5abe8c49f44535b31fddbbf6f92c71972dd08d`  
		Last Modified: Wed, 10 Jun 2020 16:09:09 GMT  
		Size: 1.7 KB (1675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b3323f04d21e510ede92022b9360017f11ac36acdb708ba7ccc23057653d07`  
		Last Modified: Wed, 10 Jun 2020 16:09:09 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce846dc61a45df9d993497543ac474d7e5fd8ac7fbebaa3fa8a7f81fc2516b68`  
		Last Modified: Wed, 10 Jun 2020 16:09:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c842d78fea670830598639f4e6b3ad36bc8109e8a0169a66647e71ebb1a5c037`  
		Last Modified: Wed, 10 Jun 2020 16:09:09 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
