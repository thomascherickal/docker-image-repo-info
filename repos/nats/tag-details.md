<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats`

-	[`nats:2`](#nats2)
-	[`nats:2.1`](#nats21)
-	[`nats:2.1.6`](#nats216)
-	[`nats:2.1.6-alpine`](#nats216-alpine)
-	[`nats:2.1.6-alpine3.11`](#nats216-alpine311)
-	[`nats:2.1.6-linux`](#nats216-linux)
-	[`nats:2.1.6-nanoserver`](#nats216-nanoserver)
-	[`nats:2.1.6-nanoserver-1809`](#nats216-nanoserver-1809)
-	[`nats:2.1.6-scratch`](#nats216-scratch)
-	[`nats:2.1.6-windowsservercore`](#nats216-windowsservercore)
-	[`nats:2.1.6-windowsservercore-1809`](#nats216-windowsservercore-1809)
-	[`nats:2.1.6-windowsservercore-ltsc2016`](#nats216-windowsservercore-ltsc2016)
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
$ docker pull nats@sha256:88d190b588ffccc3b646c6d0aabd194cb1e859a052a8f8af014db9a1002a9499
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1217; amd64

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:03f7a9538ca823f3e342254f0e0bd62fce56410fd037d70f11e208a64b9be51b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4068777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61d7629fb1351a52582452f08d569ef8aa395377751df3706474cb5769e8400d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 01 Apr 2020 06:49:28 GMT
COPY file:b5fc4f9d62c474e25c56f62242c0cbb4f21e732408978c639846820bd9b440a3 in /nats-server 
# Wed, 01 Apr 2020 06:49:28 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 01 Apr 2020 06:49:28 GMT
EXPOSE 4222 6222 8222
# Wed, 01 Apr 2020 06:49:29 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 01 Apr 2020 06:49:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9bafc186f2720cd817d9a0dca0d2d85b62db3667b346e18ad3cedee711853463`  
		Last Modified: Wed, 01 Apr 2020 06:49:48 GMT  
		Size: 4.1 MB (4068300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc99d87cfb673f46f50d4862e4486d00a26509752daa87beb60702054d53a2f8`  
		Last Modified: Wed, 01 Apr 2020 06:49:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:eff9f3146f76a2f78e896166707efdecae7f4aa7510d78cb4e986a578119bfb5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3781960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f158c883c70044a613a0b0a5bb6096487ac305e3f6f1b3e57a17a9f98bdaf09e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 31 Mar 2020 20:53:55 GMT
COPY file:5131c35b89e2bccdb55c8f10be46601f1fb947279308495595024bc0e2b29d5b in /nats-server 
# Tue, 31 Mar 2020 20:53:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 31 Mar 2020 20:53:57 GMT
EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 20:53:58 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 31 Mar 2020 20:53:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:705a3cd49f0567c17013b0eddbe53e6cffedd428744250d7076a8396babbe655`  
		Last Modified: Tue, 31 Mar 2020 20:54:42 GMT  
		Size: 3.8 MB (3781482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efabc067a958db0c40714b9365000273b61d5d19c9ce96c291b023d4ef2933f2`  
		Last Modified: Tue, 31 Mar 2020 20:54:41 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:bdda6b6ae6c62c1e78f902992214eca27cf00de2fc7d8d47235a663b3b35940a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3774917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7120ba5b06cdd64603f112b86a27c044b9e157fbfc6bdfad548f92351f75bbfe`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 01 Apr 2020 06:07:20 GMT
COPY file:846a74a5cdf1833ec24475ab97e1c375ea237825039dd6ad1d133be2c007faaf in /nats-server 
# Wed, 01 Apr 2020 06:07:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 01 Apr 2020 06:07:23 GMT
EXPOSE 4222 6222 8222
# Wed, 01 Apr 2020 06:07:24 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 01 Apr 2020 06:07:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3779a152c2262214f75fbef66a9ffa608a8a92efab5ce35515692282ae11c664`  
		Last Modified: Wed, 01 Apr 2020 06:08:10 GMT  
		Size: 3.8 MB (3774441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54270160df8d1b1d48a5e855464e3400a606022608035ba66e6914d03dd235f1`  
		Last Modified: Wed, 01 Apr 2020 06:08:08 GMT  
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

### `nats:2` - windows version 10.0.17763.1217; amd64

```console
$ docker pull nats@sha256:87d7512bdc9d1226af1b312aa729660e09e95389183c3d488ce15b0f8bf09fe5
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105061846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8852e70f71f58a4bc75aed961cd7cc5ddec1fc483e7fd17f20bfe4e8e89b1e70`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 May 2020 12:39:06 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 14:50:51 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 May 2020 14:50:52 GMT
RUN cmd /S /C #(nop) COPY file:5493aca6ccb800df74d7e7b98176527689b02c807794603a1f7dde376217279b in C:\nats-server.exe 
# Wed, 13 May 2020 14:50:54 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 May 2020 14:50:55 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 May 2020 14:50:56 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 May 2020 14:50:57 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b9e6fec25718aef5ed18d499b27e43adb524f9ee4f2eb3f0fffaea018e7e86b0`  
		Size: 101.0 MB (101019852 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eafb3f3d63d93b402dfcc428e091787a4242326bc71283a6e3ad40046a60cba0`  
		Last Modified: Wed, 13 May 2020 14:55:00 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be222cbce7c5fdc837c8334dba94184d6668f565b5330de1d5979c73aeeee084`  
		Last Modified: Wed, 13 May 2020 14:54:59 GMT  
		Size: 4.0 MB (4036982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ec160b0022b6d17fb0f35f3c82d9a64610e13d8f82f37adb2d94a41ebc82d2`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 1.5 KB (1498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e6543f6d7c7f56c892ddae258ff87ccf91344dc58fd3781de1949aed35cb431`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a063fcb9d7392f7823b459c27227c671814eef764a3a30a824eb40e0acb5a9`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540bee75308cb6ecf746719faa19454db1d8eedc79dc5ee409528aae0e9a4c87`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1`

```console
$ docker pull nats@sha256:88d190b588ffccc3b646c6d0aabd194cb1e859a052a8f8af014db9a1002a9499
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1217; amd64

### `nats:2.1` - linux; amd64

```console
$ docker pull nats@sha256:03f7a9538ca823f3e342254f0e0bd62fce56410fd037d70f11e208a64b9be51b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4068777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61d7629fb1351a52582452f08d569ef8aa395377751df3706474cb5769e8400d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 01 Apr 2020 06:49:28 GMT
COPY file:b5fc4f9d62c474e25c56f62242c0cbb4f21e732408978c639846820bd9b440a3 in /nats-server 
# Wed, 01 Apr 2020 06:49:28 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 01 Apr 2020 06:49:28 GMT
EXPOSE 4222 6222 8222
# Wed, 01 Apr 2020 06:49:29 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 01 Apr 2020 06:49:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9bafc186f2720cd817d9a0dca0d2d85b62db3667b346e18ad3cedee711853463`  
		Last Modified: Wed, 01 Apr 2020 06:49:48 GMT  
		Size: 4.1 MB (4068300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc99d87cfb673f46f50d4862e4486d00a26509752daa87beb60702054d53a2f8`  
		Last Modified: Wed, 01 Apr 2020 06:49:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1` - linux; arm variant v6

```console
$ docker pull nats@sha256:eff9f3146f76a2f78e896166707efdecae7f4aa7510d78cb4e986a578119bfb5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3781960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f158c883c70044a613a0b0a5bb6096487ac305e3f6f1b3e57a17a9f98bdaf09e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 31 Mar 2020 20:53:55 GMT
COPY file:5131c35b89e2bccdb55c8f10be46601f1fb947279308495595024bc0e2b29d5b in /nats-server 
# Tue, 31 Mar 2020 20:53:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 31 Mar 2020 20:53:57 GMT
EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 20:53:58 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 31 Mar 2020 20:53:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:705a3cd49f0567c17013b0eddbe53e6cffedd428744250d7076a8396babbe655`  
		Last Modified: Tue, 31 Mar 2020 20:54:42 GMT  
		Size: 3.8 MB (3781482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efabc067a958db0c40714b9365000273b61d5d19c9ce96c291b023d4ef2933f2`  
		Last Modified: Tue, 31 Mar 2020 20:54:41 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1` - linux; arm variant v7

```console
$ docker pull nats@sha256:bdda6b6ae6c62c1e78f902992214eca27cf00de2fc7d8d47235a663b3b35940a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3774917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7120ba5b06cdd64603f112b86a27c044b9e157fbfc6bdfad548f92351f75bbfe`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 01 Apr 2020 06:07:20 GMT
COPY file:846a74a5cdf1833ec24475ab97e1c375ea237825039dd6ad1d133be2c007faaf in /nats-server 
# Wed, 01 Apr 2020 06:07:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 01 Apr 2020 06:07:23 GMT
EXPOSE 4222 6222 8222
# Wed, 01 Apr 2020 06:07:24 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 01 Apr 2020 06:07:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3779a152c2262214f75fbef66a9ffa608a8a92efab5ce35515692282ae11c664`  
		Last Modified: Wed, 01 Apr 2020 06:08:10 GMT  
		Size: 3.8 MB (3774441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54270160df8d1b1d48a5e855464e3400a606022608035ba66e6914d03dd235f1`  
		Last Modified: Wed, 01 Apr 2020 06:08:08 GMT  
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

### `nats:2.1` - windows version 10.0.17763.1217; amd64

```console
$ docker pull nats@sha256:87d7512bdc9d1226af1b312aa729660e09e95389183c3d488ce15b0f8bf09fe5
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105061846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8852e70f71f58a4bc75aed961cd7cc5ddec1fc483e7fd17f20bfe4e8e89b1e70`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 May 2020 12:39:06 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 14:50:51 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 May 2020 14:50:52 GMT
RUN cmd /S /C #(nop) COPY file:5493aca6ccb800df74d7e7b98176527689b02c807794603a1f7dde376217279b in C:\nats-server.exe 
# Wed, 13 May 2020 14:50:54 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 May 2020 14:50:55 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 May 2020 14:50:56 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 May 2020 14:50:57 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b9e6fec25718aef5ed18d499b27e43adb524f9ee4f2eb3f0fffaea018e7e86b0`  
		Size: 101.0 MB (101019852 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eafb3f3d63d93b402dfcc428e091787a4242326bc71283a6e3ad40046a60cba0`  
		Last Modified: Wed, 13 May 2020 14:55:00 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be222cbce7c5fdc837c8334dba94184d6668f565b5330de1d5979c73aeeee084`  
		Last Modified: Wed, 13 May 2020 14:54:59 GMT  
		Size: 4.0 MB (4036982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ec160b0022b6d17fb0f35f3c82d9a64610e13d8f82f37adb2d94a41ebc82d2`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 1.5 KB (1498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e6543f6d7c7f56c892ddae258ff87ccf91344dc58fd3781de1949aed35cb431`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a063fcb9d7392f7823b459c27227c671814eef764a3a30a824eb40e0acb5a9`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540bee75308cb6ecf746719faa19454db1d8eedc79dc5ee409528aae0e9a4c87`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.6`

```console
$ docker pull nats@sha256:2ef842f90107e7bcadaf749a440bb07cde61768170110bda95646754b54854ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	windows version 10.0.17763.1217; amd64

### `nats:2.1.6` - linux; amd64

```console
$ docker pull nats@sha256:03f7a9538ca823f3e342254f0e0bd62fce56410fd037d70f11e208a64b9be51b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4068777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61d7629fb1351a52582452f08d569ef8aa395377751df3706474cb5769e8400d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 01 Apr 2020 06:49:28 GMT
COPY file:b5fc4f9d62c474e25c56f62242c0cbb4f21e732408978c639846820bd9b440a3 in /nats-server 
# Wed, 01 Apr 2020 06:49:28 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 01 Apr 2020 06:49:28 GMT
EXPOSE 4222 6222 8222
# Wed, 01 Apr 2020 06:49:29 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 01 Apr 2020 06:49:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9bafc186f2720cd817d9a0dca0d2d85b62db3667b346e18ad3cedee711853463`  
		Last Modified: Wed, 01 Apr 2020 06:49:48 GMT  
		Size: 4.1 MB (4068300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc99d87cfb673f46f50d4862e4486d00a26509752daa87beb60702054d53a2f8`  
		Last Modified: Wed, 01 Apr 2020 06:49:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.6` - linux; arm variant v6

```console
$ docker pull nats@sha256:eff9f3146f76a2f78e896166707efdecae7f4aa7510d78cb4e986a578119bfb5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3781960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f158c883c70044a613a0b0a5bb6096487ac305e3f6f1b3e57a17a9f98bdaf09e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 31 Mar 2020 20:53:55 GMT
COPY file:5131c35b89e2bccdb55c8f10be46601f1fb947279308495595024bc0e2b29d5b in /nats-server 
# Tue, 31 Mar 2020 20:53:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 31 Mar 2020 20:53:57 GMT
EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 20:53:58 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 31 Mar 2020 20:53:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:705a3cd49f0567c17013b0eddbe53e6cffedd428744250d7076a8396babbe655`  
		Last Modified: Tue, 31 Mar 2020 20:54:42 GMT  
		Size: 3.8 MB (3781482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efabc067a958db0c40714b9365000273b61d5d19c9ce96c291b023d4ef2933f2`  
		Last Modified: Tue, 31 Mar 2020 20:54:41 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.6` - linux; arm variant v7

```console
$ docker pull nats@sha256:bdda6b6ae6c62c1e78f902992214eca27cf00de2fc7d8d47235a663b3b35940a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3774917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7120ba5b06cdd64603f112b86a27c044b9e157fbfc6bdfad548f92351f75bbfe`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 01 Apr 2020 06:07:20 GMT
COPY file:846a74a5cdf1833ec24475ab97e1c375ea237825039dd6ad1d133be2c007faaf in /nats-server 
# Wed, 01 Apr 2020 06:07:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 01 Apr 2020 06:07:23 GMT
EXPOSE 4222 6222 8222
# Wed, 01 Apr 2020 06:07:24 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 01 Apr 2020 06:07:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3779a152c2262214f75fbef66a9ffa608a8a92efab5ce35515692282ae11c664`  
		Last Modified: Wed, 01 Apr 2020 06:08:10 GMT  
		Size: 3.8 MB (3774441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54270160df8d1b1d48a5e855464e3400a606022608035ba66e6914d03dd235f1`  
		Last Modified: Wed, 01 Apr 2020 06:08:08 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.6` - windows version 10.0.17763.1217; amd64

```console
$ docker pull nats@sha256:87d7512bdc9d1226af1b312aa729660e09e95389183c3d488ce15b0f8bf09fe5
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105061846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8852e70f71f58a4bc75aed961cd7cc5ddec1fc483e7fd17f20bfe4e8e89b1e70`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 May 2020 12:39:06 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 14:50:51 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 May 2020 14:50:52 GMT
RUN cmd /S /C #(nop) COPY file:5493aca6ccb800df74d7e7b98176527689b02c807794603a1f7dde376217279b in C:\nats-server.exe 
# Wed, 13 May 2020 14:50:54 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 May 2020 14:50:55 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 May 2020 14:50:56 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 May 2020 14:50:57 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b9e6fec25718aef5ed18d499b27e43adb524f9ee4f2eb3f0fffaea018e7e86b0`  
		Size: 101.0 MB (101019852 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eafb3f3d63d93b402dfcc428e091787a4242326bc71283a6e3ad40046a60cba0`  
		Last Modified: Wed, 13 May 2020 14:55:00 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be222cbce7c5fdc837c8334dba94184d6668f565b5330de1d5979c73aeeee084`  
		Last Modified: Wed, 13 May 2020 14:54:59 GMT  
		Size: 4.0 MB (4036982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ec160b0022b6d17fb0f35f3c82d9a64610e13d8f82f37adb2d94a41ebc82d2`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 1.5 KB (1498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e6543f6d7c7f56c892ddae258ff87ccf91344dc58fd3781de1949aed35cb431`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a063fcb9d7392f7823b459c27227c671814eef764a3a30a824eb40e0acb5a9`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540bee75308cb6ecf746719faa19454db1d8eedc79dc5ee409528aae0e9a4c87`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.6-alpine`

```console
$ docker pull nats@sha256:4d298a0f1ede8290e2c141b40a14a8f71026fb944aa373e66859f524939db2b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats:2.1.6-alpine` - linux; amd64

```console
$ docker pull nats@sha256:b970847a4d2c22f011fa8e238804d5ddca1e5fe149b1ce98b5b89264e94fa14a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7185423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5826bdbbffbca20fb421446c8380c24d0fe9eaa58c2d3926b5b69cdfe179afa0`
-	Default Command: `["nats-server"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 19:23:38 GMT
ENV NATS_SERVER=2.1.6
# Fri, 24 Apr 2020 19:23:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 24 Apr 2020 19:23:40 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 24 Apr 2020 19:23:41 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Apr 2020 19:23:41 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483d71d24eb24c812955e03b49a7aefe6addd1e9a27eed62d1063ccacb1daa35`  
		Last Modified: Fri, 24 Apr 2020 19:24:18 GMT  
		Size: 4.4 MB (4371577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28ddeb70b7c98a0c730372dfa9384e654535103ec63fd67de5c666ad1ed10b8`  
		Last Modified: Fri, 24 Apr 2020 19:24:18 GMT  
		Size: 530.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.6-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:bb4f4704888ba763d595a6f5b2ebc63fab245123aba0c49a4acd367fde8a85d0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6704214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6924374f96832a30c0999815ee9cf5d4b03b63a7cbce184a4f7cb463040e62cc`
-	Default Command: `["nats-server"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 18:27:15 GMT
ENV NATS_SERVER=2.1.6
# Thu, 23 Apr 2020 18:27:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 23 Apr 2020 18:27:20 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 23 Apr 2020 18:27:21 GMT
EXPOSE 4222 6222 8222
# Thu, 23 Apr 2020 18:27:22 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161abd33789448be6956b7a14750143115b738946a90dba01c171654b595db50`  
		Last Modified: Thu, 23 Apr 2020 18:27:57 GMT  
		Size: 4.1 MB (4083720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf87d86a5b745cab46e6723122e5108a56f20c54a8a908f98e64c84891dbd1f`  
		Last Modified: Thu, 23 Apr 2020 18:27:56 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.6-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:deebc7d7dc1b0429405f75d02ea6b57083cdd895d86b614a651d7623ec14a01e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6499411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66f80067dd868fea84d26f61d15ffaa2122d56c7788a50d5cc07243e534c1dff`
-	Default Command: `["nats-server"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 02:02:16 GMT
ENV NATS_SERVER=2.1.6
# Fri, 24 Apr 2020 02:02:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 24 Apr 2020 02:02:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 24 Apr 2020 02:02:25 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Apr 2020 02:02:27 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6fe91083b82217baefe1a9f0ed7d83e845198f22641b4d2b3f4b3c309cbac3`  
		Last Modified: Fri, 24 Apr 2020 02:03:03 GMT  
		Size: 4.1 MB (4076790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c4bd5409f67062e55b33a74e24037fc0aed5ad5d8e37095e02415d9ea93b84`  
		Last Modified: Fri, 24 Apr 2020 02:03:03 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.6-alpine3.11`

```console
$ docker pull nats@sha256:4d298a0f1ede8290e2c141b40a14a8f71026fb944aa373e66859f524939db2b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats:2.1.6-alpine3.11` - linux; amd64

```console
$ docker pull nats@sha256:b970847a4d2c22f011fa8e238804d5ddca1e5fe149b1ce98b5b89264e94fa14a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7185423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5826bdbbffbca20fb421446c8380c24d0fe9eaa58c2d3926b5b69cdfe179afa0`
-	Default Command: `["nats-server"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 19:23:38 GMT
ENV NATS_SERVER=2.1.6
# Fri, 24 Apr 2020 19:23:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 24 Apr 2020 19:23:40 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 24 Apr 2020 19:23:41 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Apr 2020 19:23:41 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483d71d24eb24c812955e03b49a7aefe6addd1e9a27eed62d1063ccacb1daa35`  
		Last Modified: Fri, 24 Apr 2020 19:24:18 GMT  
		Size: 4.4 MB (4371577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28ddeb70b7c98a0c730372dfa9384e654535103ec63fd67de5c666ad1ed10b8`  
		Last Modified: Fri, 24 Apr 2020 19:24:18 GMT  
		Size: 530.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.6-alpine3.11` - linux; arm variant v6

```console
$ docker pull nats@sha256:bb4f4704888ba763d595a6f5b2ebc63fab245123aba0c49a4acd367fde8a85d0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6704214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6924374f96832a30c0999815ee9cf5d4b03b63a7cbce184a4f7cb463040e62cc`
-	Default Command: `["nats-server"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 18:27:15 GMT
ENV NATS_SERVER=2.1.6
# Thu, 23 Apr 2020 18:27:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 23 Apr 2020 18:27:20 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 23 Apr 2020 18:27:21 GMT
EXPOSE 4222 6222 8222
# Thu, 23 Apr 2020 18:27:22 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161abd33789448be6956b7a14750143115b738946a90dba01c171654b595db50`  
		Last Modified: Thu, 23 Apr 2020 18:27:57 GMT  
		Size: 4.1 MB (4083720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf87d86a5b745cab46e6723122e5108a56f20c54a8a908f98e64c84891dbd1f`  
		Last Modified: Thu, 23 Apr 2020 18:27:56 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.6-alpine3.11` - linux; arm variant v7

```console
$ docker pull nats@sha256:deebc7d7dc1b0429405f75d02ea6b57083cdd895d86b614a651d7623ec14a01e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6499411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66f80067dd868fea84d26f61d15ffaa2122d56c7788a50d5cc07243e534c1dff`
-	Default Command: `["nats-server"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 02:02:16 GMT
ENV NATS_SERVER=2.1.6
# Fri, 24 Apr 2020 02:02:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 24 Apr 2020 02:02:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 24 Apr 2020 02:02:25 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Apr 2020 02:02:27 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6fe91083b82217baefe1a9f0ed7d83e845198f22641b4d2b3f4b3c309cbac3`  
		Last Modified: Fri, 24 Apr 2020 02:03:03 GMT  
		Size: 4.1 MB (4076790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c4bd5409f67062e55b33a74e24037fc0aed5ad5d8e37095e02415d9ea93b84`  
		Last Modified: Fri, 24 Apr 2020 02:03:03 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.6-linux`

```console
$ docker pull nats@sha256:0c3efd041e13dd1fb32f6d1607fffb296379fc6508650b2169bcb4342d1db08b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats:2.1.6-linux` - linux; amd64

```console
$ docker pull nats@sha256:03f7a9538ca823f3e342254f0e0bd62fce56410fd037d70f11e208a64b9be51b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4068777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61d7629fb1351a52582452f08d569ef8aa395377751df3706474cb5769e8400d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 01 Apr 2020 06:49:28 GMT
COPY file:b5fc4f9d62c474e25c56f62242c0cbb4f21e732408978c639846820bd9b440a3 in /nats-server 
# Wed, 01 Apr 2020 06:49:28 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 01 Apr 2020 06:49:28 GMT
EXPOSE 4222 6222 8222
# Wed, 01 Apr 2020 06:49:29 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 01 Apr 2020 06:49:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9bafc186f2720cd817d9a0dca0d2d85b62db3667b346e18ad3cedee711853463`  
		Last Modified: Wed, 01 Apr 2020 06:49:48 GMT  
		Size: 4.1 MB (4068300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc99d87cfb673f46f50d4862e4486d00a26509752daa87beb60702054d53a2f8`  
		Last Modified: Wed, 01 Apr 2020 06:49:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.6-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:eff9f3146f76a2f78e896166707efdecae7f4aa7510d78cb4e986a578119bfb5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3781960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f158c883c70044a613a0b0a5bb6096487ac305e3f6f1b3e57a17a9f98bdaf09e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 31 Mar 2020 20:53:55 GMT
COPY file:5131c35b89e2bccdb55c8f10be46601f1fb947279308495595024bc0e2b29d5b in /nats-server 
# Tue, 31 Mar 2020 20:53:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 31 Mar 2020 20:53:57 GMT
EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 20:53:58 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 31 Mar 2020 20:53:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:705a3cd49f0567c17013b0eddbe53e6cffedd428744250d7076a8396babbe655`  
		Last Modified: Tue, 31 Mar 2020 20:54:42 GMT  
		Size: 3.8 MB (3781482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efabc067a958db0c40714b9365000273b61d5d19c9ce96c291b023d4ef2933f2`  
		Last Modified: Tue, 31 Mar 2020 20:54:41 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.6-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:bdda6b6ae6c62c1e78f902992214eca27cf00de2fc7d8d47235a663b3b35940a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3774917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7120ba5b06cdd64603f112b86a27c044b9e157fbfc6bdfad548f92351f75bbfe`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 01 Apr 2020 06:07:20 GMT
COPY file:846a74a5cdf1833ec24475ab97e1c375ea237825039dd6ad1d133be2c007faaf in /nats-server 
# Wed, 01 Apr 2020 06:07:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 01 Apr 2020 06:07:23 GMT
EXPOSE 4222 6222 8222
# Wed, 01 Apr 2020 06:07:24 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 01 Apr 2020 06:07:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3779a152c2262214f75fbef66a9ffa608a8a92efab5ce35515692282ae11c664`  
		Last Modified: Wed, 01 Apr 2020 06:08:10 GMT  
		Size: 3.8 MB (3774441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54270160df8d1b1d48a5e855464e3400a606022608035ba66e6914d03dd235f1`  
		Last Modified: Wed, 01 Apr 2020 06:08:08 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.6-nanoserver`

```console
$ docker pull nats@sha256:749649b3ae8a91032076aaa300a79c0fb4497ca8106c3952af344ab8474ceb94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64

### `nats:2.1.6-nanoserver` - windows version 10.0.17763.1217; amd64

```console
$ docker pull nats@sha256:87d7512bdc9d1226af1b312aa729660e09e95389183c3d488ce15b0f8bf09fe5
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105061846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8852e70f71f58a4bc75aed961cd7cc5ddec1fc483e7fd17f20bfe4e8e89b1e70`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 May 2020 12:39:06 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 14:50:51 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 May 2020 14:50:52 GMT
RUN cmd /S /C #(nop) COPY file:5493aca6ccb800df74d7e7b98176527689b02c807794603a1f7dde376217279b in C:\nats-server.exe 
# Wed, 13 May 2020 14:50:54 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 May 2020 14:50:55 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 May 2020 14:50:56 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 May 2020 14:50:57 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b9e6fec25718aef5ed18d499b27e43adb524f9ee4f2eb3f0fffaea018e7e86b0`  
		Size: 101.0 MB (101019852 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eafb3f3d63d93b402dfcc428e091787a4242326bc71283a6e3ad40046a60cba0`  
		Last Modified: Wed, 13 May 2020 14:55:00 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be222cbce7c5fdc837c8334dba94184d6668f565b5330de1d5979c73aeeee084`  
		Last Modified: Wed, 13 May 2020 14:54:59 GMT  
		Size: 4.0 MB (4036982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ec160b0022b6d17fb0f35f3c82d9a64610e13d8f82f37adb2d94a41ebc82d2`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 1.5 KB (1498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e6543f6d7c7f56c892ddae258ff87ccf91344dc58fd3781de1949aed35cb431`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a063fcb9d7392f7823b459c27227c671814eef764a3a30a824eb40e0acb5a9`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540bee75308cb6ecf746719faa19454db1d8eedc79dc5ee409528aae0e9a4c87`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.6-nanoserver-1809`

```console
$ docker pull nats@sha256:749649b3ae8a91032076aaa300a79c0fb4497ca8106c3952af344ab8474ceb94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64

### `nats:2.1.6-nanoserver-1809` - windows version 10.0.17763.1217; amd64

```console
$ docker pull nats@sha256:87d7512bdc9d1226af1b312aa729660e09e95389183c3d488ce15b0f8bf09fe5
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105061846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8852e70f71f58a4bc75aed961cd7cc5ddec1fc483e7fd17f20bfe4e8e89b1e70`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 May 2020 12:39:06 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 14:50:51 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 May 2020 14:50:52 GMT
RUN cmd /S /C #(nop) COPY file:5493aca6ccb800df74d7e7b98176527689b02c807794603a1f7dde376217279b in C:\nats-server.exe 
# Wed, 13 May 2020 14:50:54 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 May 2020 14:50:55 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 May 2020 14:50:56 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 May 2020 14:50:57 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b9e6fec25718aef5ed18d499b27e43adb524f9ee4f2eb3f0fffaea018e7e86b0`  
		Size: 101.0 MB (101019852 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eafb3f3d63d93b402dfcc428e091787a4242326bc71283a6e3ad40046a60cba0`  
		Last Modified: Wed, 13 May 2020 14:55:00 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be222cbce7c5fdc837c8334dba94184d6668f565b5330de1d5979c73aeeee084`  
		Last Modified: Wed, 13 May 2020 14:54:59 GMT  
		Size: 4.0 MB (4036982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ec160b0022b6d17fb0f35f3c82d9a64610e13d8f82f37adb2d94a41ebc82d2`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 1.5 KB (1498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e6543f6d7c7f56c892ddae258ff87ccf91344dc58fd3781de1949aed35cb431`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a063fcb9d7392f7823b459c27227c671814eef764a3a30a824eb40e0acb5a9`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540bee75308cb6ecf746719faa19454db1d8eedc79dc5ee409528aae0e9a4c87`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.6-scratch`

```console
$ docker pull nats@sha256:0c3efd041e13dd1fb32f6d1607fffb296379fc6508650b2169bcb4342d1db08b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats:2.1.6-scratch` - linux; amd64

```console
$ docker pull nats@sha256:03f7a9538ca823f3e342254f0e0bd62fce56410fd037d70f11e208a64b9be51b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4068777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61d7629fb1351a52582452f08d569ef8aa395377751df3706474cb5769e8400d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 01 Apr 2020 06:49:28 GMT
COPY file:b5fc4f9d62c474e25c56f62242c0cbb4f21e732408978c639846820bd9b440a3 in /nats-server 
# Wed, 01 Apr 2020 06:49:28 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 01 Apr 2020 06:49:28 GMT
EXPOSE 4222 6222 8222
# Wed, 01 Apr 2020 06:49:29 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 01 Apr 2020 06:49:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9bafc186f2720cd817d9a0dca0d2d85b62db3667b346e18ad3cedee711853463`  
		Last Modified: Wed, 01 Apr 2020 06:49:48 GMT  
		Size: 4.1 MB (4068300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc99d87cfb673f46f50d4862e4486d00a26509752daa87beb60702054d53a2f8`  
		Last Modified: Wed, 01 Apr 2020 06:49:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.6-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:eff9f3146f76a2f78e896166707efdecae7f4aa7510d78cb4e986a578119bfb5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3781960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f158c883c70044a613a0b0a5bb6096487ac305e3f6f1b3e57a17a9f98bdaf09e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 31 Mar 2020 20:53:55 GMT
COPY file:5131c35b89e2bccdb55c8f10be46601f1fb947279308495595024bc0e2b29d5b in /nats-server 
# Tue, 31 Mar 2020 20:53:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 31 Mar 2020 20:53:57 GMT
EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 20:53:58 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 31 Mar 2020 20:53:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:705a3cd49f0567c17013b0eddbe53e6cffedd428744250d7076a8396babbe655`  
		Last Modified: Tue, 31 Mar 2020 20:54:42 GMT  
		Size: 3.8 MB (3781482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efabc067a958db0c40714b9365000273b61d5d19c9ce96c291b023d4ef2933f2`  
		Last Modified: Tue, 31 Mar 2020 20:54:41 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.6-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:bdda6b6ae6c62c1e78f902992214eca27cf00de2fc7d8d47235a663b3b35940a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3774917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7120ba5b06cdd64603f112b86a27c044b9e157fbfc6bdfad548f92351f75bbfe`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 01 Apr 2020 06:07:20 GMT
COPY file:846a74a5cdf1833ec24475ab97e1c375ea237825039dd6ad1d133be2c007faaf in /nats-server 
# Wed, 01 Apr 2020 06:07:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 01 Apr 2020 06:07:23 GMT
EXPOSE 4222 6222 8222
# Wed, 01 Apr 2020 06:07:24 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 01 Apr 2020 06:07:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3779a152c2262214f75fbef66a9ffa608a8a92efab5ce35515692282ae11c664`  
		Last Modified: Wed, 01 Apr 2020 06:08:10 GMT  
		Size: 3.8 MB (3774441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54270160df8d1b1d48a5e855464e3400a606022608035ba66e6914d03dd235f1`  
		Last Modified: Wed, 01 Apr 2020 06:08:08 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.6-windowsservercore`

```console
$ docker pull nats@sha256:49929c7e96cbd4d94b770c933fcdaa37523959b204770bcb8c6c64f39fd4d947
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64
	-	windows version 10.0.14393.3686; amd64

### `nats:2.1.6-windowsservercore` - windows version 10.0.17763.1217; amd64

```console
$ docker pull nats@sha256:38026bfd66cb1fe200a770ca74212b1855c9d6e853fb85ee00a3e18d58fee528
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1723030054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b410b6db1876f6835ba24bf47a165f529096991afa5e4d33092e7a9ea98682f6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 14:49:24 GMT
ENV NATS_DOCKERIZED=1
# Wed, 13 May 2020 14:49:25 GMT
ENV NATS_SERVER=2.1.6
# Wed, 13 May 2020 14:49:26 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Wed, 13 May 2020 14:49:46 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 May 2020 14:50:36 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 13 May 2020 14:50:37 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 May 2020 14:50:38 GMT
EXPOSE 4222 6222 8222
# Wed, 13 May 2020 14:50:39 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 May 2020 14:50:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6e220442d94ba050201e82fee90c58b5e714748e7906735032367404c473c91c`  
		Last Modified: Wed, 13 May 2020 14:27:38 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef78e6a0bb5c035fff387c2c5470bd8420babb53d74f1856b9e3ed900cd9af2`  
		Last Modified: Wed, 13 May 2020 14:54:40 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dcd0914a5c43759060ab8392ec986ac4a069accb2f9ce3fca4679b0a87d7c85`  
		Last Modified: Wed, 13 May 2020 14:54:40 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba2a9d9207a00a2aba1b3b0de0b4db3934394753808436964a988e33ee50f16`  
		Last Modified: Wed, 13 May 2020 14:54:40 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09721620d75a2711884513342bc0a1b80426f003a3fdd249f0449ae4e1d9ce5f`  
		Last Modified: Wed, 13 May 2020 14:54:40 GMT  
		Size: 340.9 KB (340876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfcdaddc68d3cecea8ab4b0121b52da7095d99088355df82ac59018d7dba025b`  
		Last Modified: Wed, 13 May 2020 14:54:43 GMT  
		Size: 4.3 MB (4346515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16f585abe2b7c6d8415117f4384304b4da7c7fa6bbde520ed7bc18e91d14d9e`  
		Last Modified: Wed, 13 May 2020 14:54:37 GMT  
		Size: 1.7 KB (1668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346112a5bf4cdc128a1a3469d52d43260ad562186d42e62b893e7850c660fa92`  
		Last Modified: Wed, 13 May 2020 14:54:37 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed443118936053d562d611d97fc3e38c75cd300f041dbd01171aa05ffd93bd10`  
		Last Modified: Wed, 13 May 2020 14:54:37 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9c7dfc60965547df88e7309ea367bb10050126f47110a7030f1ca563a9ce15`  
		Last Modified: Wed, 13 May 2020 14:54:37 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.6-windowsservercore` - windows version 10.0.14393.3686; amd64

```console
$ docker pull nats@sha256:9ac0a1a8b7c1d86e67b07c27da69c167bc06e4dd3d83235376b9441c2c7254dd
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5751199562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccc507bd9c022cd0ed7dbbd09cfa5913d866c520bcb826bfb6132ea62ea27549`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 14:51:03 GMT
ENV NATS_DOCKERIZED=1
# Wed, 13 May 2020 14:51:04 GMT
ENV NATS_SERVER=2.1.6
# Wed, 13 May 2020 14:51:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Wed, 13 May 2020 14:52:07 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 May 2020 14:54:02 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 13 May 2020 14:54:04 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 May 2020 14:54:06 GMT
EXPOSE 4222 6222 8222
# Wed, 13 May 2020 14:54:07 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 May 2020 14:54:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:78d9ecf24b3b7ef3e61c8b38d40e28e57a80552d6c97884f4cc142af2110ddff`  
		Last Modified: Wed, 13 May 2020 14:28:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5356fa8d07c48624dd3553b12cafae53b1e6818e2e77c7b4ad7c5e37a6edf5f5`  
		Last Modified: Wed, 13 May 2020 14:55:20 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:812d925d5330efdd0e3691f27be756f2d4bd21271b3d92a1fdbd7d0015ca751b`  
		Last Modified: Wed, 13 May 2020 14:55:21 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa02c160a78fb2c0432fda99964268c0d0be0c92dd4faad28abdc2aa3e9f2f3f`  
		Last Modified: Wed, 13 May 2020 14:55:20 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58a8e2f37803c472c8d10d3693e28446f643f41b20e716c97bb2cf561471f3c`  
		Last Modified: Wed, 13 May 2020 14:55:22 GMT  
		Size: 5.4 MB (5380611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a364666bd4bf347aa0241e06563fe518267439e92df88dd4c943475a6be316`  
		Last Modified: Wed, 13 May 2020 14:55:33 GMT  
		Size: 13.9 MB (13919327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07365ad87d191e5cdc05d203b8f0491d7c408b9cdbb94a131c53b05807f67f40`  
		Last Modified: Wed, 13 May 2020 14:55:17 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635bf5adfaf150aa00c8b9fe7bbfe96bfe97dbfee94544af1ad694e38cd7446c`  
		Last Modified: Wed, 13 May 2020 14:55:18 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84243df3097f51931f380c65fdf517d4a61a9a052a35d3fc8847695ca727781c`  
		Last Modified: Wed, 13 May 2020 14:55:17 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51aec177c2f2c1b498277b9130ad9ff47c26a7cb4057adf463705fc2fc671029`  
		Last Modified: Wed, 13 May 2020 14:55:18 GMT  
		Size: 1.1 KB (1104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.6-windowsservercore-1809`

```console
$ docker pull nats@sha256:a122adcc06b520dba3748d187fe8cec27a8b4a57cd15624d669b616cbd0b53e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64

### `nats:2.1.6-windowsservercore-1809` - windows version 10.0.17763.1217; amd64

```console
$ docker pull nats@sha256:38026bfd66cb1fe200a770ca74212b1855c9d6e853fb85ee00a3e18d58fee528
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1723030054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b410b6db1876f6835ba24bf47a165f529096991afa5e4d33092e7a9ea98682f6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 14:49:24 GMT
ENV NATS_DOCKERIZED=1
# Wed, 13 May 2020 14:49:25 GMT
ENV NATS_SERVER=2.1.6
# Wed, 13 May 2020 14:49:26 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Wed, 13 May 2020 14:49:46 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 May 2020 14:50:36 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 13 May 2020 14:50:37 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 May 2020 14:50:38 GMT
EXPOSE 4222 6222 8222
# Wed, 13 May 2020 14:50:39 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 May 2020 14:50:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6e220442d94ba050201e82fee90c58b5e714748e7906735032367404c473c91c`  
		Last Modified: Wed, 13 May 2020 14:27:38 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef78e6a0bb5c035fff387c2c5470bd8420babb53d74f1856b9e3ed900cd9af2`  
		Last Modified: Wed, 13 May 2020 14:54:40 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dcd0914a5c43759060ab8392ec986ac4a069accb2f9ce3fca4679b0a87d7c85`  
		Last Modified: Wed, 13 May 2020 14:54:40 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba2a9d9207a00a2aba1b3b0de0b4db3934394753808436964a988e33ee50f16`  
		Last Modified: Wed, 13 May 2020 14:54:40 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09721620d75a2711884513342bc0a1b80426f003a3fdd249f0449ae4e1d9ce5f`  
		Last Modified: Wed, 13 May 2020 14:54:40 GMT  
		Size: 340.9 KB (340876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfcdaddc68d3cecea8ab4b0121b52da7095d99088355df82ac59018d7dba025b`  
		Last Modified: Wed, 13 May 2020 14:54:43 GMT  
		Size: 4.3 MB (4346515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16f585abe2b7c6d8415117f4384304b4da7c7fa6bbde520ed7bc18e91d14d9e`  
		Last Modified: Wed, 13 May 2020 14:54:37 GMT  
		Size: 1.7 KB (1668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346112a5bf4cdc128a1a3469d52d43260ad562186d42e62b893e7850c660fa92`  
		Last Modified: Wed, 13 May 2020 14:54:37 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed443118936053d562d611d97fc3e38c75cd300f041dbd01171aa05ffd93bd10`  
		Last Modified: Wed, 13 May 2020 14:54:37 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9c7dfc60965547df88e7309ea367bb10050126f47110a7030f1ca563a9ce15`  
		Last Modified: Wed, 13 May 2020 14:54:37 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.6-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:08c9781136f212ba6156cc3bb7d0371eb17053726b1ce2a851b01ba0fd721895
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3686; amd64

### `nats:2.1.6-windowsservercore-ltsc2016` - windows version 10.0.14393.3686; amd64

```console
$ docker pull nats@sha256:9ac0a1a8b7c1d86e67b07c27da69c167bc06e4dd3d83235376b9441c2c7254dd
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5751199562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccc507bd9c022cd0ed7dbbd09cfa5913d866c520bcb826bfb6132ea62ea27549`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 14:51:03 GMT
ENV NATS_DOCKERIZED=1
# Wed, 13 May 2020 14:51:04 GMT
ENV NATS_SERVER=2.1.6
# Wed, 13 May 2020 14:51:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Wed, 13 May 2020 14:52:07 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 May 2020 14:54:02 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 13 May 2020 14:54:04 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 May 2020 14:54:06 GMT
EXPOSE 4222 6222 8222
# Wed, 13 May 2020 14:54:07 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 May 2020 14:54:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:78d9ecf24b3b7ef3e61c8b38d40e28e57a80552d6c97884f4cc142af2110ddff`  
		Last Modified: Wed, 13 May 2020 14:28:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5356fa8d07c48624dd3553b12cafae53b1e6818e2e77c7b4ad7c5e37a6edf5f5`  
		Last Modified: Wed, 13 May 2020 14:55:20 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:812d925d5330efdd0e3691f27be756f2d4bd21271b3d92a1fdbd7d0015ca751b`  
		Last Modified: Wed, 13 May 2020 14:55:21 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa02c160a78fb2c0432fda99964268c0d0be0c92dd4faad28abdc2aa3e9f2f3f`  
		Last Modified: Wed, 13 May 2020 14:55:20 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58a8e2f37803c472c8d10d3693e28446f643f41b20e716c97bb2cf561471f3c`  
		Last Modified: Wed, 13 May 2020 14:55:22 GMT  
		Size: 5.4 MB (5380611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a364666bd4bf347aa0241e06563fe518267439e92df88dd4c943475a6be316`  
		Last Modified: Wed, 13 May 2020 14:55:33 GMT  
		Size: 13.9 MB (13919327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07365ad87d191e5cdc05d203b8f0491d7c408b9cdbb94a131c53b05807f67f40`  
		Last Modified: Wed, 13 May 2020 14:55:17 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635bf5adfaf150aa00c8b9fe7bbfe96bfe97dbfee94544af1ad694e38cd7446c`  
		Last Modified: Wed, 13 May 2020 14:55:18 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84243df3097f51931f380c65fdf517d4a61a9a052a35d3fc8847695ca727781c`  
		Last Modified: Wed, 13 May 2020 14:55:17 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51aec177c2f2c1b498277b9130ad9ff47c26a7cb4057adf463705fc2fc671029`  
		Last Modified: Wed, 13 May 2020 14:55:18 GMT  
		Size: 1.1 KB (1104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-alpine`

```console
$ docker pull nats@sha256:4d298a0f1ede8290e2c141b40a14a8f71026fb944aa373e66859f524939db2b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats:2.1-alpine` - linux; amd64

```console
$ docker pull nats@sha256:b970847a4d2c22f011fa8e238804d5ddca1e5fe149b1ce98b5b89264e94fa14a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7185423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5826bdbbffbca20fb421446c8380c24d0fe9eaa58c2d3926b5b69cdfe179afa0`
-	Default Command: `["nats-server"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 19:23:38 GMT
ENV NATS_SERVER=2.1.6
# Fri, 24 Apr 2020 19:23:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 24 Apr 2020 19:23:40 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 24 Apr 2020 19:23:41 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Apr 2020 19:23:41 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483d71d24eb24c812955e03b49a7aefe6addd1e9a27eed62d1063ccacb1daa35`  
		Last Modified: Fri, 24 Apr 2020 19:24:18 GMT  
		Size: 4.4 MB (4371577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28ddeb70b7c98a0c730372dfa9384e654535103ec63fd67de5c666ad1ed10b8`  
		Last Modified: Fri, 24 Apr 2020 19:24:18 GMT  
		Size: 530.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:bb4f4704888ba763d595a6f5b2ebc63fab245123aba0c49a4acd367fde8a85d0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6704214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6924374f96832a30c0999815ee9cf5d4b03b63a7cbce184a4f7cb463040e62cc`
-	Default Command: `["nats-server"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 18:27:15 GMT
ENV NATS_SERVER=2.1.6
# Thu, 23 Apr 2020 18:27:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 23 Apr 2020 18:27:20 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 23 Apr 2020 18:27:21 GMT
EXPOSE 4222 6222 8222
# Thu, 23 Apr 2020 18:27:22 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161abd33789448be6956b7a14750143115b738946a90dba01c171654b595db50`  
		Last Modified: Thu, 23 Apr 2020 18:27:57 GMT  
		Size: 4.1 MB (4083720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf87d86a5b745cab46e6723122e5108a56f20c54a8a908f98e64c84891dbd1f`  
		Last Modified: Thu, 23 Apr 2020 18:27:56 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:deebc7d7dc1b0429405f75d02ea6b57083cdd895d86b614a651d7623ec14a01e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6499411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66f80067dd868fea84d26f61d15ffaa2122d56c7788a50d5cc07243e534c1dff`
-	Default Command: `["nats-server"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 02:02:16 GMT
ENV NATS_SERVER=2.1.6
# Fri, 24 Apr 2020 02:02:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 24 Apr 2020 02:02:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 24 Apr 2020 02:02:25 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Apr 2020 02:02:27 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6fe91083b82217baefe1a9f0ed7d83e845198f22641b4d2b3f4b3c309cbac3`  
		Last Modified: Fri, 24 Apr 2020 02:03:03 GMT  
		Size: 4.1 MB (4076790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c4bd5409f67062e55b33a74e24037fc0aed5ad5d8e37095e02415d9ea93b84`  
		Last Modified: Fri, 24 Apr 2020 02:03:03 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-alpine3.11`

```console
$ docker pull nats@sha256:4d298a0f1ede8290e2c141b40a14a8f71026fb944aa373e66859f524939db2b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats:2.1-alpine3.11` - linux; amd64

```console
$ docker pull nats@sha256:b970847a4d2c22f011fa8e238804d5ddca1e5fe149b1ce98b5b89264e94fa14a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7185423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5826bdbbffbca20fb421446c8380c24d0fe9eaa58c2d3926b5b69cdfe179afa0`
-	Default Command: `["nats-server"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 19:23:38 GMT
ENV NATS_SERVER=2.1.6
# Fri, 24 Apr 2020 19:23:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 24 Apr 2020 19:23:40 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 24 Apr 2020 19:23:41 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Apr 2020 19:23:41 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483d71d24eb24c812955e03b49a7aefe6addd1e9a27eed62d1063ccacb1daa35`  
		Last Modified: Fri, 24 Apr 2020 19:24:18 GMT  
		Size: 4.4 MB (4371577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28ddeb70b7c98a0c730372dfa9384e654535103ec63fd67de5c666ad1ed10b8`  
		Last Modified: Fri, 24 Apr 2020 19:24:18 GMT  
		Size: 530.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-alpine3.11` - linux; arm variant v6

```console
$ docker pull nats@sha256:bb4f4704888ba763d595a6f5b2ebc63fab245123aba0c49a4acd367fde8a85d0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6704214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6924374f96832a30c0999815ee9cf5d4b03b63a7cbce184a4f7cb463040e62cc`
-	Default Command: `["nats-server"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 18:27:15 GMT
ENV NATS_SERVER=2.1.6
# Thu, 23 Apr 2020 18:27:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 23 Apr 2020 18:27:20 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 23 Apr 2020 18:27:21 GMT
EXPOSE 4222 6222 8222
# Thu, 23 Apr 2020 18:27:22 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161abd33789448be6956b7a14750143115b738946a90dba01c171654b595db50`  
		Last Modified: Thu, 23 Apr 2020 18:27:57 GMT  
		Size: 4.1 MB (4083720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf87d86a5b745cab46e6723122e5108a56f20c54a8a908f98e64c84891dbd1f`  
		Last Modified: Thu, 23 Apr 2020 18:27:56 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-alpine3.11` - linux; arm variant v7

```console
$ docker pull nats@sha256:deebc7d7dc1b0429405f75d02ea6b57083cdd895d86b614a651d7623ec14a01e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6499411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66f80067dd868fea84d26f61d15ffaa2122d56c7788a50d5cc07243e534c1dff`
-	Default Command: `["nats-server"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 02:02:16 GMT
ENV NATS_SERVER=2.1.6
# Fri, 24 Apr 2020 02:02:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 24 Apr 2020 02:02:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 24 Apr 2020 02:02:25 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Apr 2020 02:02:27 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6fe91083b82217baefe1a9f0ed7d83e845198f22641b4d2b3f4b3c309cbac3`  
		Last Modified: Fri, 24 Apr 2020 02:03:03 GMT  
		Size: 4.1 MB (4076790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c4bd5409f67062e55b33a74e24037fc0aed5ad5d8e37095e02415d9ea93b84`  
		Last Modified: Fri, 24 Apr 2020 02:03:03 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-linux`

```console
$ docker pull nats@sha256:4dd85d386b2572917793b417e434162febf14a527e6d0fb9482d98ecdf72b4f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.1-linux` - linux; amd64

```console
$ docker pull nats@sha256:03f7a9538ca823f3e342254f0e0bd62fce56410fd037d70f11e208a64b9be51b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4068777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61d7629fb1351a52582452f08d569ef8aa395377751df3706474cb5769e8400d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 01 Apr 2020 06:49:28 GMT
COPY file:b5fc4f9d62c474e25c56f62242c0cbb4f21e732408978c639846820bd9b440a3 in /nats-server 
# Wed, 01 Apr 2020 06:49:28 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 01 Apr 2020 06:49:28 GMT
EXPOSE 4222 6222 8222
# Wed, 01 Apr 2020 06:49:29 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 01 Apr 2020 06:49:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9bafc186f2720cd817d9a0dca0d2d85b62db3667b346e18ad3cedee711853463`  
		Last Modified: Wed, 01 Apr 2020 06:49:48 GMT  
		Size: 4.1 MB (4068300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc99d87cfb673f46f50d4862e4486d00a26509752daa87beb60702054d53a2f8`  
		Last Modified: Wed, 01 Apr 2020 06:49:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:eff9f3146f76a2f78e896166707efdecae7f4aa7510d78cb4e986a578119bfb5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3781960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f158c883c70044a613a0b0a5bb6096487ac305e3f6f1b3e57a17a9f98bdaf09e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 31 Mar 2020 20:53:55 GMT
COPY file:5131c35b89e2bccdb55c8f10be46601f1fb947279308495595024bc0e2b29d5b in /nats-server 
# Tue, 31 Mar 2020 20:53:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 31 Mar 2020 20:53:57 GMT
EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 20:53:58 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 31 Mar 2020 20:53:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:705a3cd49f0567c17013b0eddbe53e6cffedd428744250d7076a8396babbe655`  
		Last Modified: Tue, 31 Mar 2020 20:54:42 GMT  
		Size: 3.8 MB (3781482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efabc067a958db0c40714b9365000273b61d5d19c9ce96c291b023d4ef2933f2`  
		Last Modified: Tue, 31 Mar 2020 20:54:41 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:bdda6b6ae6c62c1e78f902992214eca27cf00de2fc7d8d47235a663b3b35940a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3774917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7120ba5b06cdd64603f112b86a27c044b9e157fbfc6bdfad548f92351f75bbfe`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 01 Apr 2020 06:07:20 GMT
COPY file:846a74a5cdf1833ec24475ab97e1c375ea237825039dd6ad1d133be2c007faaf in /nats-server 
# Wed, 01 Apr 2020 06:07:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 01 Apr 2020 06:07:23 GMT
EXPOSE 4222 6222 8222
# Wed, 01 Apr 2020 06:07:24 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 01 Apr 2020 06:07:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3779a152c2262214f75fbef66a9ffa608a8a92efab5ce35515692282ae11c664`  
		Last Modified: Wed, 01 Apr 2020 06:08:10 GMT  
		Size: 3.8 MB (3774441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54270160df8d1b1d48a5e855464e3400a606022608035ba66e6914d03dd235f1`  
		Last Modified: Wed, 01 Apr 2020 06:08:08 GMT  
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
$ docker pull nats@sha256:749649b3ae8a91032076aaa300a79c0fb4497ca8106c3952af344ab8474ceb94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64

### `nats:2.1-nanoserver` - windows version 10.0.17763.1217; amd64

```console
$ docker pull nats@sha256:87d7512bdc9d1226af1b312aa729660e09e95389183c3d488ce15b0f8bf09fe5
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105061846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8852e70f71f58a4bc75aed961cd7cc5ddec1fc483e7fd17f20bfe4e8e89b1e70`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 May 2020 12:39:06 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 14:50:51 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 May 2020 14:50:52 GMT
RUN cmd /S /C #(nop) COPY file:5493aca6ccb800df74d7e7b98176527689b02c807794603a1f7dde376217279b in C:\nats-server.exe 
# Wed, 13 May 2020 14:50:54 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 May 2020 14:50:55 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 May 2020 14:50:56 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 May 2020 14:50:57 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b9e6fec25718aef5ed18d499b27e43adb524f9ee4f2eb3f0fffaea018e7e86b0`  
		Size: 101.0 MB (101019852 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eafb3f3d63d93b402dfcc428e091787a4242326bc71283a6e3ad40046a60cba0`  
		Last Modified: Wed, 13 May 2020 14:55:00 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be222cbce7c5fdc837c8334dba94184d6668f565b5330de1d5979c73aeeee084`  
		Last Modified: Wed, 13 May 2020 14:54:59 GMT  
		Size: 4.0 MB (4036982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ec160b0022b6d17fb0f35f3c82d9a64610e13d8f82f37adb2d94a41ebc82d2`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 1.5 KB (1498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e6543f6d7c7f56c892ddae258ff87ccf91344dc58fd3781de1949aed35cb431`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a063fcb9d7392f7823b459c27227c671814eef764a3a30a824eb40e0acb5a9`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540bee75308cb6ecf746719faa19454db1d8eedc79dc5ee409528aae0e9a4c87`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-nanoserver-1809`

```console
$ docker pull nats@sha256:749649b3ae8a91032076aaa300a79c0fb4497ca8106c3952af344ab8474ceb94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64

### `nats:2.1-nanoserver-1809` - windows version 10.0.17763.1217; amd64

```console
$ docker pull nats@sha256:87d7512bdc9d1226af1b312aa729660e09e95389183c3d488ce15b0f8bf09fe5
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105061846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8852e70f71f58a4bc75aed961cd7cc5ddec1fc483e7fd17f20bfe4e8e89b1e70`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 May 2020 12:39:06 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 14:50:51 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 May 2020 14:50:52 GMT
RUN cmd /S /C #(nop) COPY file:5493aca6ccb800df74d7e7b98176527689b02c807794603a1f7dde376217279b in C:\nats-server.exe 
# Wed, 13 May 2020 14:50:54 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 May 2020 14:50:55 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 May 2020 14:50:56 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 May 2020 14:50:57 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b9e6fec25718aef5ed18d499b27e43adb524f9ee4f2eb3f0fffaea018e7e86b0`  
		Size: 101.0 MB (101019852 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eafb3f3d63d93b402dfcc428e091787a4242326bc71283a6e3ad40046a60cba0`  
		Last Modified: Wed, 13 May 2020 14:55:00 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be222cbce7c5fdc837c8334dba94184d6668f565b5330de1d5979c73aeeee084`  
		Last Modified: Wed, 13 May 2020 14:54:59 GMT  
		Size: 4.0 MB (4036982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ec160b0022b6d17fb0f35f3c82d9a64610e13d8f82f37adb2d94a41ebc82d2`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 1.5 KB (1498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e6543f6d7c7f56c892ddae258ff87ccf91344dc58fd3781de1949aed35cb431`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a063fcb9d7392f7823b459c27227c671814eef764a3a30a824eb40e0acb5a9`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540bee75308cb6ecf746719faa19454db1d8eedc79dc5ee409528aae0e9a4c87`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-scratch`

```console
$ docker pull nats@sha256:4dd85d386b2572917793b417e434162febf14a527e6d0fb9482d98ecdf72b4f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.1-scratch` - linux; amd64

```console
$ docker pull nats@sha256:03f7a9538ca823f3e342254f0e0bd62fce56410fd037d70f11e208a64b9be51b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4068777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61d7629fb1351a52582452f08d569ef8aa395377751df3706474cb5769e8400d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 01 Apr 2020 06:49:28 GMT
COPY file:b5fc4f9d62c474e25c56f62242c0cbb4f21e732408978c639846820bd9b440a3 in /nats-server 
# Wed, 01 Apr 2020 06:49:28 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 01 Apr 2020 06:49:28 GMT
EXPOSE 4222 6222 8222
# Wed, 01 Apr 2020 06:49:29 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 01 Apr 2020 06:49:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9bafc186f2720cd817d9a0dca0d2d85b62db3667b346e18ad3cedee711853463`  
		Last Modified: Wed, 01 Apr 2020 06:49:48 GMT  
		Size: 4.1 MB (4068300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc99d87cfb673f46f50d4862e4486d00a26509752daa87beb60702054d53a2f8`  
		Last Modified: Wed, 01 Apr 2020 06:49:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:eff9f3146f76a2f78e896166707efdecae7f4aa7510d78cb4e986a578119bfb5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3781960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f158c883c70044a613a0b0a5bb6096487ac305e3f6f1b3e57a17a9f98bdaf09e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 31 Mar 2020 20:53:55 GMT
COPY file:5131c35b89e2bccdb55c8f10be46601f1fb947279308495595024bc0e2b29d5b in /nats-server 
# Tue, 31 Mar 2020 20:53:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 31 Mar 2020 20:53:57 GMT
EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 20:53:58 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 31 Mar 2020 20:53:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:705a3cd49f0567c17013b0eddbe53e6cffedd428744250d7076a8396babbe655`  
		Last Modified: Tue, 31 Mar 2020 20:54:42 GMT  
		Size: 3.8 MB (3781482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efabc067a958db0c40714b9365000273b61d5d19c9ce96c291b023d4ef2933f2`  
		Last Modified: Tue, 31 Mar 2020 20:54:41 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:bdda6b6ae6c62c1e78f902992214eca27cf00de2fc7d8d47235a663b3b35940a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3774917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7120ba5b06cdd64603f112b86a27c044b9e157fbfc6bdfad548f92351f75bbfe`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 01 Apr 2020 06:07:20 GMT
COPY file:846a74a5cdf1833ec24475ab97e1c375ea237825039dd6ad1d133be2c007faaf in /nats-server 
# Wed, 01 Apr 2020 06:07:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 01 Apr 2020 06:07:23 GMT
EXPOSE 4222 6222 8222
# Wed, 01 Apr 2020 06:07:24 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 01 Apr 2020 06:07:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3779a152c2262214f75fbef66a9ffa608a8a92efab5ce35515692282ae11c664`  
		Last Modified: Wed, 01 Apr 2020 06:08:10 GMT  
		Size: 3.8 MB (3774441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54270160df8d1b1d48a5e855464e3400a606022608035ba66e6914d03dd235f1`  
		Last Modified: Wed, 01 Apr 2020 06:08:08 GMT  
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
$ docker pull nats@sha256:49929c7e96cbd4d94b770c933fcdaa37523959b204770bcb8c6c64f39fd4d947
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64
	-	windows version 10.0.14393.3686; amd64

### `nats:2.1-windowsservercore` - windows version 10.0.17763.1217; amd64

```console
$ docker pull nats@sha256:38026bfd66cb1fe200a770ca74212b1855c9d6e853fb85ee00a3e18d58fee528
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1723030054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b410b6db1876f6835ba24bf47a165f529096991afa5e4d33092e7a9ea98682f6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 14:49:24 GMT
ENV NATS_DOCKERIZED=1
# Wed, 13 May 2020 14:49:25 GMT
ENV NATS_SERVER=2.1.6
# Wed, 13 May 2020 14:49:26 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Wed, 13 May 2020 14:49:46 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 May 2020 14:50:36 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 13 May 2020 14:50:37 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 May 2020 14:50:38 GMT
EXPOSE 4222 6222 8222
# Wed, 13 May 2020 14:50:39 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 May 2020 14:50:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6e220442d94ba050201e82fee90c58b5e714748e7906735032367404c473c91c`  
		Last Modified: Wed, 13 May 2020 14:27:38 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef78e6a0bb5c035fff387c2c5470bd8420babb53d74f1856b9e3ed900cd9af2`  
		Last Modified: Wed, 13 May 2020 14:54:40 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dcd0914a5c43759060ab8392ec986ac4a069accb2f9ce3fca4679b0a87d7c85`  
		Last Modified: Wed, 13 May 2020 14:54:40 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba2a9d9207a00a2aba1b3b0de0b4db3934394753808436964a988e33ee50f16`  
		Last Modified: Wed, 13 May 2020 14:54:40 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09721620d75a2711884513342bc0a1b80426f003a3fdd249f0449ae4e1d9ce5f`  
		Last Modified: Wed, 13 May 2020 14:54:40 GMT  
		Size: 340.9 KB (340876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfcdaddc68d3cecea8ab4b0121b52da7095d99088355df82ac59018d7dba025b`  
		Last Modified: Wed, 13 May 2020 14:54:43 GMT  
		Size: 4.3 MB (4346515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16f585abe2b7c6d8415117f4384304b4da7c7fa6bbde520ed7bc18e91d14d9e`  
		Last Modified: Wed, 13 May 2020 14:54:37 GMT  
		Size: 1.7 KB (1668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346112a5bf4cdc128a1a3469d52d43260ad562186d42e62b893e7850c660fa92`  
		Last Modified: Wed, 13 May 2020 14:54:37 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed443118936053d562d611d97fc3e38c75cd300f041dbd01171aa05ffd93bd10`  
		Last Modified: Wed, 13 May 2020 14:54:37 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9c7dfc60965547df88e7309ea367bb10050126f47110a7030f1ca563a9ce15`  
		Last Modified: Wed, 13 May 2020 14:54:37 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-windowsservercore` - windows version 10.0.14393.3686; amd64

```console
$ docker pull nats@sha256:9ac0a1a8b7c1d86e67b07c27da69c167bc06e4dd3d83235376b9441c2c7254dd
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5751199562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccc507bd9c022cd0ed7dbbd09cfa5913d866c520bcb826bfb6132ea62ea27549`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 14:51:03 GMT
ENV NATS_DOCKERIZED=1
# Wed, 13 May 2020 14:51:04 GMT
ENV NATS_SERVER=2.1.6
# Wed, 13 May 2020 14:51:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Wed, 13 May 2020 14:52:07 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 May 2020 14:54:02 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 13 May 2020 14:54:04 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 May 2020 14:54:06 GMT
EXPOSE 4222 6222 8222
# Wed, 13 May 2020 14:54:07 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 May 2020 14:54:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:78d9ecf24b3b7ef3e61c8b38d40e28e57a80552d6c97884f4cc142af2110ddff`  
		Last Modified: Wed, 13 May 2020 14:28:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5356fa8d07c48624dd3553b12cafae53b1e6818e2e77c7b4ad7c5e37a6edf5f5`  
		Last Modified: Wed, 13 May 2020 14:55:20 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:812d925d5330efdd0e3691f27be756f2d4bd21271b3d92a1fdbd7d0015ca751b`  
		Last Modified: Wed, 13 May 2020 14:55:21 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa02c160a78fb2c0432fda99964268c0d0be0c92dd4faad28abdc2aa3e9f2f3f`  
		Last Modified: Wed, 13 May 2020 14:55:20 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58a8e2f37803c472c8d10d3693e28446f643f41b20e716c97bb2cf561471f3c`  
		Last Modified: Wed, 13 May 2020 14:55:22 GMT  
		Size: 5.4 MB (5380611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a364666bd4bf347aa0241e06563fe518267439e92df88dd4c943475a6be316`  
		Last Modified: Wed, 13 May 2020 14:55:33 GMT  
		Size: 13.9 MB (13919327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07365ad87d191e5cdc05d203b8f0491d7c408b9cdbb94a131c53b05807f67f40`  
		Last Modified: Wed, 13 May 2020 14:55:17 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635bf5adfaf150aa00c8b9fe7bbfe96bfe97dbfee94544af1ad694e38cd7446c`  
		Last Modified: Wed, 13 May 2020 14:55:18 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84243df3097f51931f380c65fdf517d4a61a9a052a35d3fc8847695ca727781c`  
		Last Modified: Wed, 13 May 2020 14:55:17 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51aec177c2f2c1b498277b9130ad9ff47c26a7cb4057adf463705fc2fc671029`  
		Last Modified: Wed, 13 May 2020 14:55:18 GMT  
		Size: 1.1 KB (1104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-windowsservercore-1809`

```console
$ docker pull nats@sha256:a122adcc06b520dba3748d187fe8cec27a8b4a57cd15624d669b616cbd0b53e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64

### `nats:2.1-windowsservercore-1809` - windows version 10.0.17763.1217; amd64

```console
$ docker pull nats@sha256:38026bfd66cb1fe200a770ca74212b1855c9d6e853fb85ee00a3e18d58fee528
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1723030054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b410b6db1876f6835ba24bf47a165f529096991afa5e4d33092e7a9ea98682f6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 14:49:24 GMT
ENV NATS_DOCKERIZED=1
# Wed, 13 May 2020 14:49:25 GMT
ENV NATS_SERVER=2.1.6
# Wed, 13 May 2020 14:49:26 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Wed, 13 May 2020 14:49:46 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 May 2020 14:50:36 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 13 May 2020 14:50:37 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 May 2020 14:50:38 GMT
EXPOSE 4222 6222 8222
# Wed, 13 May 2020 14:50:39 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 May 2020 14:50:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6e220442d94ba050201e82fee90c58b5e714748e7906735032367404c473c91c`  
		Last Modified: Wed, 13 May 2020 14:27:38 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef78e6a0bb5c035fff387c2c5470bd8420babb53d74f1856b9e3ed900cd9af2`  
		Last Modified: Wed, 13 May 2020 14:54:40 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dcd0914a5c43759060ab8392ec986ac4a069accb2f9ce3fca4679b0a87d7c85`  
		Last Modified: Wed, 13 May 2020 14:54:40 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba2a9d9207a00a2aba1b3b0de0b4db3934394753808436964a988e33ee50f16`  
		Last Modified: Wed, 13 May 2020 14:54:40 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09721620d75a2711884513342bc0a1b80426f003a3fdd249f0449ae4e1d9ce5f`  
		Last Modified: Wed, 13 May 2020 14:54:40 GMT  
		Size: 340.9 KB (340876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfcdaddc68d3cecea8ab4b0121b52da7095d99088355df82ac59018d7dba025b`  
		Last Modified: Wed, 13 May 2020 14:54:43 GMT  
		Size: 4.3 MB (4346515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16f585abe2b7c6d8415117f4384304b4da7c7fa6bbde520ed7bc18e91d14d9e`  
		Last Modified: Wed, 13 May 2020 14:54:37 GMT  
		Size: 1.7 KB (1668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346112a5bf4cdc128a1a3469d52d43260ad562186d42e62b893e7850c660fa92`  
		Last Modified: Wed, 13 May 2020 14:54:37 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed443118936053d562d611d97fc3e38c75cd300f041dbd01171aa05ffd93bd10`  
		Last Modified: Wed, 13 May 2020 14:54:37 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9c7dfc60965547df88e7309ea367bb10050126f47110a7030f1ca563a9ce15`  
		Last Modified: Wed, 13 May 2020 14:54:37 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:08c9781136f212ba6156cc3bb7d0371eb17053726b1ce2a851b01ba0fd721895
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3686; amd64

### `nats:2.1-windowsservercore-ltsc2016` - windows version 10.0.14393.3686; amd64

```console
$ docker pull nats@sha256:9ac0a1a8b7c1d86e67b07c27da69c167bc06e4dd3d83235376b9441c2c7254dd
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5751199562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccc507bd9c022cd0ed7dbbd09cfa5913d866c520bcb826bfb6132ea62ea27549`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 14:51:03 GMT
ENV NATS_DOCKERIZED=1
# Wed, 13 May 2020 14:51:04 GMT
ENV NATS_SERVER=2.1.6
# Wed, 13 May 2020 14:51:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Wed, 13 May 2020 14:52:07 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 May 2020 14:54:02 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 13 May 2020 14:54:04 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 May 2020 14:54:06 GMT
EXPOSE 4222 6222 8222
# Wed, 13 May 2020 14:54:07 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 May 2020 14:54:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:78d9ecf24b3b7ef3e61c8b38d40e28e57a80552d6c97884f4cc142af2110ddff`  
		Last Modified: Wed, 13 May 2020 14:28:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5356fa8d07c48624dd3553b12cafae53b1e6818e2e77c7b4ad7c5e37a6edf5f5`  
		Last Modified: Wed, 13 May 2020 14:55:20 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:812d925d5330efdd0e3691f27be756f2d4bd21271b3d92a1fdbd7d0015ca751b`  
		Last Modified: Wed, 13 May 2020 14:55:21 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa02c160a78fb2c0432fda99964268c0d0be0c92dd4faad28abdc2aa3e9f2f3f`  
		Last Modified: Wed, 13 May 2020 14:55:20 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58a8e2f37803c472c8d10d3693e28446f643f41b20e716c97bb2cf561471f3c`  
		Last Modified: Wed, 13 May 2020 14:55:22 GMT  
		Size: 5.4 MB (5380611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a364666bd4bf347aa0241e06563fe518267439e92df88dd4c943475a6be316`  
		Last Modified: Wed, 13 May 2020 14:55:33 GMT  
		Size: 13.9 MB (13919327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07365ad87d191e5cdc05d203b8f0491d7c408b9cdbb94a131c53b05807f67f40`  
		Last Modified: Wed, 13 May 2020 14:55:17 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635bf5adfaf150aa00c8b9fe7bbfe96bfe97dbfee94544af1ad694e38cd7446c`  
		Last Modified: Wed, 13 May 2020 14:55:18 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84243df3097f51931f380c65fdf517d4a61a9a052a35d3fc8847695ca727781c`  
		Last Modified: Wed, 13 May 2020 14:55:17 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51aec177c2f2c1b498277b9130ad9ff47c26a7cb4057adf463705fc2fc671029`  
		Last Modified: Wed, 13 May 2020 14:55:18 GMT  
		Size: 1.1 KB (1104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:4d298a0f1ede8290e2c141b40a14a8f71026fb944aa373e66859f524939db2b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:b970847a4d2c22f011fa8e238804d5ddca1e5fe149b1ce98b5b89264e94fa14a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7185423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5826bdbbffbca20fb421446c8380c24d0fe9eaa58c2d3926b5b69cdfe179afa0`
-	Default Command: `["nats-server"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 19:23:38 GMT
ENV NATS_SERVER=2.1.6
# Fri, 24 Apr 2020 19:23:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 24 Apr 2020 19:23:40 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 24 Apr 2020 19:23:41 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Apr 2020 19:23:41 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483d71d24eb24c812955e03b49a7aefe6addd1e9a27eed62d1063ccacb1daa35`  
		Last Modified: Fri, 24 Apr 2020 19:24:18 GMT  
		Size: 4.4 MB (4371577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28ddeb70b7c98a0c730372dfa9384e654535103ec63fd67de5c666ad1ed10b8`  
		Last Modified: Fri, 24 Apr 2020 19:24:18 GMT  
		Size: 530.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:bb4f4704888ba763d595a6f5b2ebc63fab245123aba0c49a4acd367fde8a85d0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6704214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6924374f96832a30c0999815ee9cf5d4b03b63a7cbce184a4f7cb463040e62cc`
-	Default Command: `["nats-server"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 18:27:15 GMT
ENV NATS_SERVER=2.1.6
# Thu, 23 Apr 2020 18:27:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 23 Apr 2020 18:27:20 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 23 Apr 2020 18:27:21 GMT
EXPOSE 4222 6222 8222
# Thu, 23 Apr 2020 18:27:22 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161abd33789448be6956b7a14750143115b738946a90dba01c171654b595db50`  
		Last Modified: Thu, 23 Apr 2020 18:27:57 GMT  
		Size: 4.1 MB (4083720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf87d86a5b745cab46e6723122e5108a56f20c54a8a908f98e64c84891dbd1f`  
		Last Modified: Thu, 23 Apr 2020 18:27:56 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:deebc7d7dc1b0429405f75d02ea6b57083cdd895d86b614a651d7623ec14a01e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6499411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66f80067dd868fea84d26f61d15ffaa2122d56c7788a50d5cc07243e534c1dff`
-	Default Command: `["nats-server"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 02:02:16 GMT
ENV NATS_SERVER=2.1.6
# Fri, 24 Apr 2020 02:02:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 24 Apr 2020 02:02:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 24 Apr 2020 02:02:25 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Apr 2020 02:02:27 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6fe91083b82217baefe1a9f0ed7d83e845198f22641b4d2b3f4b3c309cbac3`  
		Last Modified: Fri, 24 Apr 2020 02:03:03 GMT  
		Size: 4.1 MB (4076790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c4bd5409f67062e55b33a74e24037fc0aed5ad5d8e37095e02415d9ea93b84`  
		Last Modified: Fri, 24 Apr 2020 02:03:03 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.11`

```console
$ docker pull nats@sha256:4d298a0f1ede8290e2c141b40a14a8f71026fb944aa373e66859f524939db2b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats:2-alpine3.11` - linux; amd64

```console
$ docker pull nats@sha256:b970847a4d2c22f011fa8e238804d5ddca1e5fe149b1ce98b5b89264e94fa14a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7185423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5826bdbbffbca20fb421446c8380c24d0fe9eaa58c2d3926b5b69cdfe179afa0`
-	Default Command: `["nats-server"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 19:23:38 GMT
ENV NATS_SERVER=2.1.6
# Fri, 24 Apr 2020 19:23:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 24 Apr 2020 19:23:40 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 24 Apr 2020 19:23:41 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Apr 2020 19:23:41 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483d71d24eb24c812955e03b49a7aefe6addd1e9a27eed62d1063ccacb1daa35`  
		Last Modified: Fri, 24 Apr 2020 19:24:18 GMT  
		Size: 4.4 MB (4371577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28ddeb70b7c98a0c730372dfa9384e654535103ec63fd67de5c666ad1ed10b8`  
		Last Modified: Fri, 24 Apr 2020 19:24:18 GMT  
		Size: 530.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.11` - linux; arm variant v6

```console
$ docker pull nats@sha256:bb4f4704888ba763d595a6f5b2ebc63fab245123aba0c49a4acd367fde8a85d0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6704214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6924374f96832a30c0999815ee9cf5d4b03b63a7cbce184a4f7cb463040e62cc`
-	Default Command: `["nats-server"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 18:27:15 GMT
ENV NATS_SERVER=2.1.6
# Thu, 23 Apr 2020 18:27:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 23 Apr 2020 18:27:20 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 23 Apr 2020 18:27:21 GMT
EXPOSE 4222 6222 8222
# Thu, 23 Apr 2020 18:27:22 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161abd33789448be6956b7a14750143115b738946a90dba01c171654b595db50`  
		Last Modified: Thu, 23 Apr 2020 18:27:57 GMT  
		Size: 4.1 MB (4083720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf87d86a5b745cab46e6723122e5108a56f20c54a8a908f98e64c84891dbd1f`  
		Last Modified: Thu, 23 Apr 2020 18:27:56 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.11` - linux; arm variant v7

```console
$ docker pull nats@sha256:deebc7d7dc1b0429405f75d02ea6b57083cdd895d86b614a651d7623ec14a01e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6499411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66f80067dd868fea84d26f61d15ffaa2122d56c7788a50d5cc07243e534c1dff`
-	Default Command: `["nats-server"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 02:02:16 GMT
ENV NATS_SERVER=2.1.6
# Fri, 24 Apr 2020 02:02:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 24 Apr 2020 02:02:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 24 Apr 2020 02:02:25 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Apr 2020 02:02:27 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6fe91083b82217baefe1a9f0ed7d83e845198f22641b4d2b3f4b3c309cbac3`  
		Last Modified: Fri, 24 Apr 2020 02:03:03 GMT  
		Size: 4.1 MB (4076790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c4bd5409f67062e55b33a74e24037fc0aed5ad5d8e37095e02415d9ea93b84`  
		Last Modified: Fri, 24 Apr 2020 02:03:03 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:4dd85d386b2572917793b417e434162febf14a527e6d0fb9482d98ecdf72b4f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:03f7a9538ca823f3e342254f0e0bd62fce56410fd037d70f11e208a64b9be51b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4068777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61d7629fb1351a52582452f08d569ef8aa395377751df3706474cb5769e8400d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 01 Apr 2020 06:49:28 GMT
COPY file:b5fc4f9d62c474e25c56f62242c0cbb4f21e732408978c639846820bd9b440a3 in /nats-server 
# Wed, 01 Apr 2020 06:49:28 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 01 Apr 2020 06:49:28 GMT
EXPOSE 4222 6222 8222
# Wed, 01 Apr 2020 06:49:29 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 01 Apr 2020 06:49:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9bafc186f2720cd817d9a0dca0d2d85b62db3667b346e18ad3cedee711853463`  
		Last Modified: Wed, 01 Apr 2020 06:49:48 GMT  
		Size: 4.1 MB (4068300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc99d87cfb673f46f50d4862e4486d00a26509752daa87beb60702054d53a2f8`  
		Last Modified: Wed, 01 Apr 2020 06:49:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:eff9f3146f76a2f78e896166707efdecae7f4aa7510d78cb4e986a578119bfb5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3781960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f158c883c70044a613a0b0a5bb6096487ac305e3f6f1b3e57a17a9f98bdaf09e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 31 Mar 2020 20:53:55 GMT
COPY file:5131c35b89e2bccdb55c8f10be46601f1fb947279308495595024bc0e2b29d5b in /nats-server 
# Tue, 31 Mar 2020 20:53:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 31 Mar 2020 20:53:57 GMT
EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 20:53:58 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 31 Mar 2020 20:53:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:705a3cd49f0567c17013b0eddbe53e6cffedd428744250d7076a8396babbe655`  
		Last Modified: Tue, 31 Mar 2020 20:54:42 GMT  
		Size: 3.8 MB (3781482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efabc067a958db0c40714b9365000273b61d5d19c9ce96c291b023d4ef2933f2`  
		Last Modified: Tue, 31 Mar 2020 20:54:41 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:bdda6b6ae6c62c1e78f902992214eca27cf00de2fc7d8d47235a663b3b35940a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3774917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7120ba5b06cdd64603f112b86a27c044b9e157fbfc6bdfad548f92351f75bbfe`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 01 Apr 2020 06:07:20 GMT
COPY file:846a74a5cdf1833ec24475ab97e1c375ea237825039dd6ad1d133be2c007faaf in /nats-server 
# Wed, 01 Apr 2020 06:07:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 01 Apr 2020 06:07:23 GMT
EXPOSE 4222 6222 8222
# Wed, 01 Apr 2020 06:07:24 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 01 Apr 2020 06:07:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3779a152c2262214f75fbef66a9ffa608a8a92efab5ce35515692282ae11c664`  
		Last Modified: Wed, 01 Apr 2020 06:08:10 GMT  
		Size: 3.8 MB (3774441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54270160df8d1b1d48a5e855464e3400a606022608035ba66e6914d03dd235f1`  
		Last Modified: Wed, 01 Apr 2020 06:08:08 GMT  
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
$ docker pull nats@sha256:749649b3ae8a91032076aaa300a79c0fb4497ca8106c3952af344ab8474ceb94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.1217; amd64

```console
$ docker pull nats@sha256:87d7512bdc9d1226af1b312aa729660e09e95389183c3d488ce15b0f8bf09fe5
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105061846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8852e70f71f58a4bc75aed961cd7cc5ddec1fc483e7fd17f20bfe4e8e89b1e70`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 May 2020 12:39:06 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 14:50:51 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 May 2020 14:50:52 GMT
RUN cmd /S /C #(nop) COPY file:5493aca6ccb800df74d7e7b98176527689b02c807794603a1f7dde376217279b in C:\nats-server.exe 
# Wed, 13 May 2020 14:50:54 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 May 2020 14:50:55 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 May 2020 14:50:56 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 May 2020 14:50:57 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b9e6fec25718aef5ed18d499b27e43adb524f9ee4f2eb3f0fffaea018e7e86b0`  
		Size: 101.0 MB (101019852 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eafb3f3d63d93b402dfcc428e091787a4242326bc71283a6e3ad40046a60cba0`  
		Last Modified: Wed, 13 May 2020 14:55:00 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be222cbce7c5fdc837c8334dba94184d6668f565b5330de1d5979c73aeeee084`  
		Last Modified: Wed, 13 May 2020 14:54:59 GMT  
		Size: 4.0 MB (4036982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ec160b0022b6d17fb0f35f3c82d9a64610e13d8f82f37adb2d94a41ebc82d2`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 1.5 KB (1498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e6543f6d7c7f56c892ddae258ff87ccf91344dc58fd3781de1949aed35cb431`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a063fcb9d7392f7823b459c27227c671814eef764a3a30a824eb40e0acb5a9`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540bee75308cb6ecf746719faa19454db1d8eedc79dc5ee409528aae0e9a4c87`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:749649b3ae8a91032076aaa300a79c0fb4497ca8106c3952af344ab8474ceb94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.1217; amd64

```console
$ docker pull nats@sha256:87d7512bdc9d1226af1b312aa729660e09e95389183c3d488ce15b0f8bf09fe5
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105061846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8852e70f71f58a4bc75aed961cd7cc5ddec1fc483e7fd17f20bfe4e8e89b1e70`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 May 2020 12:39:06 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 14:50:51 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 May 2020 14:50:52 GMT
RUN cmd /S /C #(nop) COPY file:5493aca6ccb800df74d7e7b98176527689b02c807794603a1f7dde376217279b in C:\nats-server.exe 
# Wed, 13 May 2020 14:50:54 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 May 2020 14:50:55 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 May 2020 14:50:56 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 May 2020 14:50:57 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b9e6fec25718aef5ed18d499b27e43adb524f9ee4f2eb3f0fffaea018e7e86b0`  
		Size: 101.0 MB (101019852 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eafb3f3d63d93b402dfcc428e091787a4242326bc71283a6e3ad40046a60cba0`  
		Last Modified: Wed, 13 May 2020 14:55:00 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be222cbce7c5fdc837c8334dba94184d6668f565b5330de1d5979c73aeeee084`  
		Last Modified: Wed, 13 May 2020 14:54:59 GMT  
		Size: 4.0 MB (4036982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ec160b0022b6d17fb0f35f3c82d9a64610e13d8f82f37adb2d94a41ebc82d2`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 1.5 KB (1498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e6543f6d7c7f56c892ddae258ff87ccf91344dc58fd3781de1949aed35cb431`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a063fcb9d7392f7823b459c27227c671814eef764a3a30a824eb40e0acb5a9`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540bee75308cb6ecf746719faa19454db1d8eedc79dc5ee409528aae0e9a4c87`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:4dd85d386b2572917793b417e434162febf14a527e6d0fb9482d98ecdf72b4f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:03f7a9538ca823f3e342254f0e0bd62fce56410fd037d70f11e208a64b9be51b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4068777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61d7629fb1351a52582452f08d569ef8aa395377751df3706474cb5769e8400d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 01 Apr 2020 06:49:28 GMT
COPY file:b5fc4f9d62c474e25c56f62242c0cbb4f21e732408978c639846820bd9b440a3 in /nats-server 
# Wed, 01 Apr 2020 06:49:28 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 01 Apr 2020 06:49:28 GMT
EXPOSE 4222 6222 8222
# Wed, 01 Apr 2020 06:49:29 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 01 Apr 2020 06:49:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9bafc186f2720cd817d9a0dca0d2d85b62db3667b346e18ad3cedee711853463`  
		Last Modified: Wed, 01 Apr 2020 06:49:48 GMT  
		Size: 4.1 MB (4068300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc99d87cfb673f46f50d4862e4486d00a26509752daa87beb60702054d53a2f8`  
		Last Modified: Wed, 01 Apr 2020 06:49:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:eff9f3146f76a2f78e896166707efdecae7f4aa7510d78cb4e986a578119bfb5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3781960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f158c883c70044a613a0b0a5bb6096487ac305e3f6f1b3e57a17a9f98bdaf09e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 31 Mar 2020 20:53:55 GMT
COPY file:5131c35b89e2bccdb55c8f10be46601f1fb947279308495595024bc0e2b29d5b in /nats-server 
# Tue, 31 Mar 2020 20:53:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 31 Mar 2020 20:53:57 GMT
EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 20:53:58 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 31 Mar 2020 20:53:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:705a3cd49f0567c17013b0eddbe53e6cffedd428744250d7076a8396babbe655`  
		Last Modified: Tue, 31 Mar 2020 20:54:42 GMT  
		Size: 3.8 MB (3781482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efabc067a958db0c40714b9365000273b61d5d19c9ce96c291b023d4ef2933f2`  
		Last Modified: Tue, 31 Mar 2020 20:54:41 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:bdda6b6ae6c62c1e78f902992214eca27cf00de2fc7d8d47235a663b3b35940a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3774917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7120ba5b06cdd64603f112b86a27c044b9e157fbfc6bdfad548f92351f75bbfe`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 01 Apr 2020 06:07:20 GMT
COPY file:846a74a5cdf1833ec24475ab97e1c375ea237825039dd6ad1d133be2c007faaf in /nats-server 
# Wed, 01 Apr 2020 06:07:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 01 Apr 2020 06:07:23 GMT
EXPOSE 4222 6222 8222
# Wed, 01 Apr 2020 06:07:24 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 01 Apr 2020 06:07:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3779a152c2262214f75fbef66a9ffa608a8a92efab5ce35515692282ae11c664`  
		Last Modified: Wed, 01 Apr 2020 06:08:10 GMT  
		Size: 3.8 MB (3774441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54270160df8d1b1d48a5e855464e3400a606022608035ba66e6914d03dd235f1`  
		Last Modified: Wed, 01 Apr 2020 06:08:08 GMT  
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
$ docker pull nats@sha256:49929c7e96cbd4d94b770c933fcdaa37523959b204770bcb8c6c64f39fd4d947
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64
	-	windows version 10.0.14393.3686; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.1217; amd64

```console
$ docker pull nats@sha256:38026bfd66cb1fe200a770ca74212b1855c9d6e853fb85ee00a3e18d58fee528
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1723030054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b410b6db1876f6835ba24bf47a165f529096991afa5e4d33092e7a9ea98682f6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 14:49:24 GMT
ENV NATS_DOCKERIZED=1
# Wed, 13 May 2020 14:49:25 GMT
ENV NATS_SERVER=2.1.6
# Wed, 13 May 2020 14:49:26 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Wed, 13 May 2020 14:49:46 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 May 2020 14:50:36 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 13 May 2020 14:50:37 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 May 2020 14:50:38 GMT
EXPOSE 4222 6222 8222
# Wed, 13 May 2020 14:50:39 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 May 2020 14:50:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6e220442d94ba050201e82fee90c58b5e714748e7906735032367404c473c91c`  
		Last Modified: Wed, 13 May 2020 14:27:38 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef78e6a0bb5c035fff387c2c5470bd8420babb53d74f1856b9e3ed900cd9af2`  
		Last Modified: Wed, 13 May 2020 14:54:40 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dcd0914a5c43759060ab8392ec986ac4a069accb2f9ce3fca4679b0a87d7c85`  
		Last Modified: Wed, 13 May 2020 14:54:40 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba2a9d9207a00a2aba1b3b0de0b4db3934394753808436964a988e33ee50f16`  
		Last Modified: Wed, 13 May 2020 14:54:40 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09721620d75a2711884513342bc0a1b80426f003a3fdd249f0449ae4e1d9ce5f`  
		Last Modified: Wed, 13 May 2020 14:54:40 GMT  
		Size: 340.9 KB (340876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfcdaddc68d3cecea8ab4b0121b52da7095d99088355df82ac59018d7dba025b`  
		Last Modified: Wed, 13 May 2020 14:54:43 GMT  
		Size: 4.3 MB (4346515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16f585abe2b7c6d8415117f4384304b4da7c7fa6bbde520ed7bc18e91d14d9e`  
		Last Modified: Wed, 13 May 2020 14:54:37 GMT  
		Size: 1.7 KB (1668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346112a5bf4cdc128a1a3469d52d43260ad562186d42e62b893e7850c660fa92`  
		Last Modified: Wed, 13 May 2020 14:54:37 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed443118936053d562d611d97fc3e38c75cd300f041dbd01171aa05ffd93bd10`  
		Last Modified: Wed, 13 May 2020 14:54:37 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9c7dfc60965547df88e7309ea367bb10050126f47110a7030f1ca563a9ce15`  
		Last Modified: Wed, 13 May 2020 14:54:37 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-windowsservercore` - windows version 10.0.14393.3686; amd64

```console
$ docker pull nats@sha256:9ac0a1a8b7c1d86e67b07c27da69c167bc06e4dd3d83235376b9441c2c7254dd
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5751199562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccc507bd9c022cd0ed7dbbd09cfa5913d866c520bcb826bfb6132ea62ea27549`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 14:51:03 GMT
ENV NATS_DOCKERIZED=1
# Wed, 13 May 2020 14:51:04 GMT
ENV NATS_SERVER=2.1.6
# Wed, 13 May 2020 14:51:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Wed, 13 May 2020 14:52:07 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 May 2020 14:54:02 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 13 May 2020 14:54:04 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 May 2020 14:54:06 GMT
EXPOSE 4222 6222 8222
# Wed, 13 May 2020 14:54:07 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 May 2020 14:54:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:78d9ecf24b3b7ef3e61c8b38d40e28e57a80552d6c97884f4cc142af2110ddff`  
		Last Modified: Wed, 13 May 2020 14:28:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5356fa8d07c48624dd3553b12cafae53b1e6818e2e77c7b4ad7c5e37a6edf5f5`  
		Last Modified: Wed, 13 May 2020 14:55:20 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:812d925d5330efdd0e3691f27be756f2d4bd21271b3d92a1fdbd7d0015ca751b`  
		Last Modified: Wed, 13 May 2020 14:55:21 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa02c160a78fb2c0432fda99964268c0d0be0c92dd4faad28abdc2aa3e9f2f3f`  
		Last Modified: Wed, 13 May 2020 14:55:20 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58a8e2f37803c472c8d10d3693e28446f643f41b20e716c97bb2cf561471f3c`  
		Last Modified: Wed, 13 May 2020 14:55:22 GMT  
		Size: 5.4 MB (5380611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a364666bd4bf347aa0241e06563fe518267439e92df88dd4c943475a6be316`  
		Last Modified: Wed, 13 May 2020 14:55:33 GMT  
		Size: 13.9 MB (13919327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07365ad87d191e5cdc05d203b8f0491d7c408b9cdbb94a131c53b05807f67f40`  
		Last Modified: Wed, 13 May 2020 14:55:17 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635bf5adfaf150aa00c8b9fe7bbfe96bfe97dbfee94544af1ad694e38cd7446c`  
		Last Modified: Wed, 13 May 2020 14:55:18 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84243df3097f51931f380c65fdf517d4a61a9a052a35d3fc8847695ca727781c`  
		Last Modified: Wed, 13 May 2020 14:55:17 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51aec177c2f2c1b498277b9130ad9ff47c26a7cb4057adf463705fc2fc671029`  
		Last Modified: Wed, 13 May 2020 14:55:18 GMT  
		Size: 1.1 KB (1104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:a122adcc06b520dba3748d187fe8cec27a8b4a57cd15624d669b616cbd0b53e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.1217; amd64

```console
$ docker pull nats@sha256:38026bfd66cb1fe200a770ca74212b1855c9d6e853fb85ee00a3e18d58fee528
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1723030054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b410b6db1876f6835ba24bf47a165f529096991afa5e4d33092e7a9ea98682f6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 14:49:24 GMT
ENV NATS_DOCKERIZED=1
# Wed, 13 May 2020 14:49:25 GMT
ENV NATS_SERVER=2.1.6
# Wed, 13 May 2020 14:49:26 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Wed, 13 May 2020 14:49:46 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 May 2020 14:50:36 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 13 May 2020 14:50:37 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 May 2020 14:50:38 GMT
EXPOSE 4222 6222 8222
# Wed, 13 May 2020 14:50:39 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 May 2020 14:50:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6e220442d94ba050201e82fee90c58b5e714748e7906735032367404c473c91c`  
		Last Modified: Wed, 13 May 2020 14:27:38 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef78e6a0bb5c035fff387c2c5470bd8420babb53d74f1856b9e3ed900cd9af2`  
		Last Modified: Wed, 13 May 2020 14:54:40 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dcd0914a5c43759060ab8392ec986ac4a069accb2f9ce3fca4679b0a87d7c85`  
		Last Modified: Wed, 13 May 2020 14:54:40 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba2a9d9207a00a2aba1b3b0de0b4db3934394753808436964a988e33ee50f16`  
		Last Modified: Wed, 13 May 2020 14:54:40 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09721620d75a2711884513342bc0a1b80426f003a3fdd249f0449ae4e1d9ce5f`  
		Last Modified: Wed, 13 May 2020 14:54:40 GMT  
		Size: 340.9 KB (340876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfcdaddc68d3cecea8ab4b0121b52da7095d99088355df82ac59018d7dba025b`  
		Last Modified: Wed, 13 May 2020 14:54:43 GMT  
		Size: 4.3 MB (4346515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16f585abe2b7c6d8415117f4384304b4da7c7fa6bbde520ed7bc18e91d14d9e`  
		Last Modified: Wed, 13 May 2020 14:54:37 GMT  
		Size: 1.7 KB (1668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346112a5bf4cdc128a1a3469d52d43260ad562186d42e62b893e7850c660fa92`  
		Last Modified: Wed, 13 May 2020 14:54:37 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed443118936053d562d611d97fc3e38c75cd300f041dbd01171aa05ffd93bd10`  
		Last Modified: Wed, 13 May 2020 14:54:37 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9c7dfc60965547df88e7309ea367bb10050126f47110a7030f1ca563a9ce15`  
		Last Modified: Wed, 13 May 2020 14:54:37 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:08c9781136f212ba6156cc3bb7d0371eb17053726b1ce2a851b01ba0fd721895
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3686; amd64

### `nats:2-windowsservercore-ltsc2016` - windows version 10.0.14393.3686; amd64

```console
$ docker pull nats@sha256:9ac0a1a8b7c1d86e67b07c27da69c167bc06e4dd3d83235376b9441c2c7254dd
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5751199562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccc507bd9c022cd0ed7dbbd09cfa5913d866c520bcb826bfb6132ea62ea27549`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 14:51:03 GMT
ENV NATS_DOCKERIZED=1
# Wed, 13 May 2020 14:51:04 GMT
ENV NATS_SERVER=2.1.6
# Wed, 13 May 2020 14:51:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Wed, 13 May 2020 14:52:07 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 May 2020 14:54:02 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 13 May 2020 14:54:04 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 May 2020 14:54:06 GMT
EXPOSE 4222 6222 8222
# Wed, 13 May 2020 14:54:07 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 May 2020 14:54:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:78d9ecf24b3b7ef3e61c8b38d40e28e57a80552d6c97884f4cc142af2110ddff`  
		Last Modified: Wed, 13 May 2020 14:28:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5356fa8d07c48624dd3553b12cafae53b1e6818e2e77c7b4ad7c5e37a6edf5f5`  
		Last Modified: Wed, 13 May 2020 14:55:20 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:812d925d5330efdd0e3691f27be756f2d4bd21271b3d92a1fdbd7d0015ca751b`  
		Last Modified: Wed, 13 May 2020 14:55:21 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa02c160a78fb2c0432fda99964268c0d0be0c92dd4faad28abdc2aa3e9f2f3f`  
		Last Modified: Wed, 13 May 2020 14:55:20 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58a8e2f37803c472c8d10d3693e28446f643f41b20e716c97bb2cf561471f3c`  
		Last Modified: Wed, 13 May 2020 14:55:22 GMT  
		Size: 5.4 MB (5380611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a364666bd4bf347aa0241e06563fe518267439e92df88dd4c943475a6be316`  
		Last Modified: Wed, 13 May 2020 14:55:33 GMT  
		Size: 13.9 MB (13919327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07365ad87d191e5cdc05d203b8f0491d7c408b9cdbb94a131c53b05807f67f40`  
		Last Modified: Wed, 13 May 2020 14:55:17 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635bf5adfaf150aa00c8b9fe7bbfe96bfe97dbfee94544af1ad694e38cd7446c`  
		Last Modified: Wed, 13 May 2020 14:55:18 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84243df3097f51931f380c65fdf517d4a61a9a052a35d3fc8847695ca727781c`  
		Last Modified: Wed, 13 May 2020 14:55:17 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51aec177c2f2c1b498277b9130ad9ff47c26a7cb4057adf463705fc2fc671029`  
		Last Modified: Wed, 13 May 2020 14:55:18 GMT  
		Size: 1.1 KB (1104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:4d298a0f1ede8290e2c141b40a14a8f71026fb944aa373e66859f524939db2b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:b970847a4d2c22f011fa8e238804d5ddca1e5fe149b1ce98b5b89264e94fa14a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7185423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5826bdbbffbca20fb421446c8380c24d0fe9eaa58c2d3926b5b69cdfe179afa0`
-	Default Command: `["nats-server"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 19:23:38 GMT
ENV NATS_SERVER=2.1.6
# Fri, 24 Apr 2020 19:23:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 24 Apr 2020 19:23:40 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 24 Apr 2020 19:23:41 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Apr 2020 19:23:41 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483d71d24eb24c812955e03b49a7aefe6addd1e9a27eed62d1063ccacb1daa35`  
		Last Modified: Fri, 24 Apr 2020 19:24:18 GMT  
		Size: 4.4 MB (4371577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28ddeb70b7c98a0c730372dfa9384e654535103ec63fd67de5c666ad1ed10b8`  
		Last Modified: Fri, 24 Apr 2020 19:24:18 GMT  
		Size: 530.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:bb4f4704888ba763d595a6f5b2ebc63fab245123aba0c49a4acd367fde8a85d0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6704214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6924374f96832a30c0999815ee9cf5d4b03b63a7cbce184a4f7cb463040e62cc`
-	Default Command: `["nats-server"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 18:27:15 GMT
ENV NATS_SERVER=2.1.6
# Thu, 23 Apr 2020 18:27:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 23 Apr 2020 18:27:20 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 23 Apr 2020 18:27:21 GMT
EXPOSE 4222 6222 8222
# Thu, 23 Apr 2020 18:27:22 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161abd33789448be6956b7a14750143115b738946a90dba01c171654b595db50`  
		Last Modified: Thu, 23 Apr 2020 18:27:57 GMT  
		Size: 4.1 MB (4083720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf87d86a5b745cab46e6723122e5108a56f20c54a8a908f98e64c84891dbd1f`  
		Last Modified: Thu, 23 Apr 2020 18:27:56 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:deebc7d7dc1b0429405f75d02ea6b57083cdd895d86b614a651d7623ec14a01e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6499411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66f80067dd868fea84d26f61d15ffaa2122d56c7788a50d5cc07243e534c1dff`
-	Default Command: `["nats-server"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 02:02:16 GMT
ENV NATS_SERVER=2.1.6
# Fri, 24 Apr 2020 02:02:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 24 Apr 2020 02:02:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 24 Apr 2020 02:02:25 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Apr 2020 02:02:27 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6fe91083b82217baefe1a9f0ed7d83e845198f22641b4d2b3f4b3c309cbac3`  
		Last Modified: Fri, 24 Apr 2020 02:03:03 GMT  
		Size: 4.1 MB (4076790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c4bd5409f67062e55b33a74e24037fc0aed5ad5d8e37095e02415d9ea93b84`  
		Last Modified: Fri, 24 Apr 2020 02:03:03 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.11`

```console
$ docker pull nats@sha256:4d298a0f1ede8290e2c141b40a14a8f71026fb944aa373e66859f524939db2b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats:alpine3.11` - linux; amd64

```console
$ docker pull nats@sha256:b970847a4d2c22f011fa8e238804d5ddca1e5fe149b1ce98b5b89264e94fa14a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7185423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5826bdbbffbca20fb421446c8380c24d0fe9eaa58c2d3926b5b69cdfe179afa0`
-	Default Command: `["nats-server"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 19:23:38 GMT
ENV NATS_SERVER=2.1.6
# Fri, 24 Apr 2020 19:23:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 24 Apr 2020 19:23:40 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 24 Apr 2020 19:23:41 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Apr 2020 19:23:41 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483d71d24eb24c812955e03b49a7aefe6addd1e9a27eed62d1063ccacb1daa35`  
		Last Modified: Fri, 24 Apr 2020 19:24:18 GMT  
		Size: 4.4 MB (4371577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28ddeb70b7c98a0c730372dfa9384e654535103ec63fd67de5c666ad1ed10b8`  
		Last Modified: Fri, 24 Apr 2020 19:24:18 GMT  
		Size: 530.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.11` - linux; arm variant v6

```console
$ docker pull nats@sha256:bb4f4704888ba763d595a6f5b2ebc63fab245123aba0c49a4acd367fde8a85d0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6704214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6924374f96832a30c0999815ee9cf5d4b03b63a7cbce184a4f7cb463040e62cc`
-	Default Command: `["nats-server"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 18:27:15 GMT
ENV NATS_SERVER=2.1.6
# Thu, 23 Apr 2020 18:27:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 23 Apr 2020 18:27:20 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 23 Apr 2020 18:27:21 GMT
EXPOSE 4222 6222 8222
# Thu, 23 Apr 2020 18:27:22 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161abd33789448be6956b7a14750143115b738946a90dba01c171654b595db50`  
		Last Modified: Thu, 23 Apr 2020 18:27:57 GMT  
		Size: 4.1 MB (4083720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf87d86a5b745cab46e6723122e5108a56f20c54a8a908f98e64c84891dbd1f`  
		Last Modified: Thu, 23 Apr 2020 18:27:56 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.11` - linux; arm variant v7

```console
$ docker pull nats@sha256:deebc7d7dc1b0429405f75d02ea6b57083cdd895d86b614a651d7623ec14a01e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6499411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66f80067dd868fea84d26f61d15ffaa2122d56c7788a50d5cc07243e534c1dff`
-	Default Command: `["nats-server"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 02:02:16 GMT
ENV NATS_SERVER=2.1.6
# Fri, 24 Apr 2020 02:02:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 24 Apr 2020 02:02:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 24 Apr 2020 02:02:25 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Apr 2020 02:02:27 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6fe91083b82217baefe1a9f0ed7d83e845198f22641b4d2b3f4b3c309cbac3`  
		Last Modified: Fri, 24 Apr 2020 02:03:03 GMT  
		Size: 4.1 MB (4076790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c4bd5409f67062e55b33a74e24037fc0aed5ad5d8e37095e02415d9ea93b84`  
		Last Modified: Fri, 24 Apr 2020 02:03:03 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:88d190b588ffccc3b646c6d0aabd194cb1e859a052a8f8af014db9a1002a9499
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1217; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:03f7a9538ca823f3e342254f0e0bd62fce56410fd037d70f11e208a64b9be51b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4068777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61d7629fb1351a52582452f08d569ef8aa395377751df3706474cb5769e8400d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 01 Apr 2020 06:49:28 GMT
COPY file:b5fc4f9d62c474e25c56f62242c0cbb4f21e732408978c639846820bd9b440a3 in /nats-server 
# Wed, 01 Apr 2020 06:49:28 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 01 Apr 2020 06:49:28 GMT
EXPOSE 4222 6222 8222
# Wed, 01 Apr 2020 06:49:29 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 01 Apr 2020 06:49:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9bafc186f2720cd817d9a0dca0d2d85b62db3667b346e18ad3cedee711853463`  
		Last Modified: Wed, 01 Apr 2020 06:49:48 GMT  
		Size: 4.1 MB (4068300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc99d87cfb673f46f50d4862e4486d00a26509752daa87beb60702054d53a2f8`  
		Last Modified: Wed, 01 Apr 2020 06:49:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:eff9f3146f76a2f78e896166707efdecae7f4aa7510d78cb4e986a578119bfb5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3781960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f158c883c70044a613a0b0a5bb6096487ac305e3f6f1b3e57a17a9f98bdaf09e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 31 Mar 2020 20:53:55 GMT
COPY file:5131c35b89e2bccdb55c8f10be46601f1fb947279308495595024bc0e2b29d5b in /nats-server 
# Tue, 31 Mar 2020 20:53:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 31 Mar 2020 20:53:57 GMT
EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 20:53:58 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 31 Mar 2020 20:53:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:705a3cd49f0567c17013b0eddbe53e6cffedd428744250d7076a8396babbe655`  
		Last Modified: Tue, 31 Mar 2020 20:54:42 GMT  
		Size: 3.8 MB (3781482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efabc067a958db0c40714b9365000273b61d5d19c9ce96c291b023d4ef2933f2`  
		Last Modified: Tue, 31 Mar 2020 20:54:41 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:bdda6b6ae6c62c1e78f902992214eca27cf00de2fc7d8d47235a663b3b35940a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3774917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7120ba5b06cdd64603f112b86a27c044b9e157fbfc6bdfad548f92351f75bbfe`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 01 Apr 2020 06:07:20 GMT
COPY file:846a74a5cdf1833ec24475ab97e1c375ea237825039dd6ad1d133be2c007faaf in /nats-server 
# Wed, 01 Apr 2020 06:07:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 01 Apr 2020 06:07:23 GMT
EXPOSE 4222 6222 8222
# Wed, 01 Apr 2020 06:07:24 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 01 Apr 2020 06:07:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3779a152c2262214f75fbef66a9ffa608a8a92efab5ce35515692282ae11c664`  
		Last Modified: Wed, 01 Apr 2020 06:08:10 GMT  
		Size: 3.8 MB (3774441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54270160df8d1b1d48a5e855464e3400a606022608035ba66e6914d03dd235f1`  
		Last Modified: Wed, 01 Apr 2020 06:08:08 GMT  
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

### `nats:latest` - windows version 10.0.17763.1217; amd64

```console
$ docker pull nats@sha256:87d7512bdc9d1226af1b312aa729660e09e95389183c3d488ce15b0f8bf09fe5
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105061846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8852e70f71f58a4bc75aed961cd7cc5ddec1fc483e7fd17f20bfe4e8e89b1e70`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 May 2020 12:39:06 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 14:50:51 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 May 2020 14:50:52 GMT
RUN cmd /S /C #(nop) COPY file:5493aca6ccb800df74d7e7b98176527689b02c807794603a1f7dde376217279b in C:\nats-server.exe 
# Wed, 13 May 2020 14:50:54 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 May 2020 14:50:55 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 May 2020 14:50:56 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 May 2020 14:50:57 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b9e6fec25718aef5ed18d499b27e43adb524f9ee4f2eb3f0fffaea018e7e86b0`  
		Size: 101.0 MB (101019852 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eafb3f3d63d93b402dfcc428e091787a4242326bc71283a6e3ad40046a60cba0`  
		Last Modified: Wed, 13 May 2020 14:55:00 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be222cbce7c5fdc837c8334dba94184d6668f565b5330de1d5979c73aeeee084`  
		Last Modified: Wed, 13 May 2020 14:54:59 GMT  
		Size: 4.0 MB (4036982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ec160b0022b6d17fb0f35f3c82d9a64610e13d8f82f37adb2d94a41ebc82d2`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 1.5 KB (1498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e6543f6d7c7f56c892ddae258ff87ccf91344dc58fd3781de1949aed35cb431`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a063fcb9d7392f7823b459c27227c671814eef764a3a30a824eb40e0acb5a9`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540bee75308cb6ecf746719faa19454db1d8eedc79dc5ee409528aae0e9a4c87`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:4dd85d386b2572917793b417e434162febf14a527e6d0fb9482d98ecdf72b4f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:03f7a9538ca823f3e342254f0e0bd62fce56410fd037d70f11e208a64b9be51b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4068777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61d7629fb1351a52582452f08d569ef8aa395377751df3706474cb5769e8400d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 01 Apr 2020 06:49:28 GMT
COPY file:b5fc4f9d62c474e25c56f62242c0cbb4f21e732408978c639846820bd9b440a3 in /nats-server 
# Wed, 01 Apr 2020 06:49:28 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 01 Apr 2020 06:49:28 GMT
EXPOSE 4222 6222 8222
# Wed, 01 Apr 2020 06:49:29 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 01 Apr 2020 06:49:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9bafc186f2720cd817d9a0dca0d2d85b62db3667b346e18ad3cedee711853463`  
		Last Modified: Wed, 01 Apr 2020 06:49:48 GMT  
		Size: 4.1 MB (4068300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc99d87cfb673f46f50d4862e4486d00a26509752daa87beb60702054d53a2f8`  
		Last Modified: Wed, 01 Apr 2020 06:49:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:eff9f3146f76a2f78e896166707efdecae7f4aa7510d78cb4e986a578119bfb5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3781960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f158c883c70044a613a0b0a5bb6096487ac305e3f6f1b3e57a17a9f98bdaf09e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 31 Mar 2020 20:53:55 GMT
COPY file:5131c35b89e2bccdb55c8f10be46601f1fb947279308495595024bc0e2b29d5b in /nats-server 
# Tue, 31 Mar 2020 20:53:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 31 Mar 2020 20:53:57 GMT
EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 20:53:58 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 31 Mar 2020 20:53:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:705a3cd49f0567c17013b0eddbe53e6cffedd428744250d7076a8396babbe655`  
		Last Modified: Tue, 31 Mar 2020 20:54:42 GMT  
		Size: 3.8 MB (3781482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efabc067a958db0c40714b9365000273b61d5d19c9ce96c291b023d4ef2933f2`  
		Last Modified: Tue, 31 Mar 2020 20:54:41 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:bdda6b6ae6c62c1e78f902992214eca27cf00de2fc7d8d47235a663b3b35940a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3774917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7120ba5b06cdd64603f112b86a27c044b9e157fbfc6bdfad548f92351f75bbfe`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 01 Apr 2020 06:07:20 GMT
COPY file:846a74a5cdf1833ec24475ab97e1c375ea237825039dd6ad1d133be2c007faaf in /nats-server 
# Wed, 01 Apr 2020 06:07:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 01 Apr 2020 06:07:23 GMT
EXPOSE 4222 6222 8222
# Wed, 01 Apr 2020 06:07:24 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 01 Apr 2020 06:07:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3779a152c2262214f75fbef66a9ffa608a8a92efab5ce35515692282ae11c664`  
		Last Modified: Wed, 01 Apr 2020 06:08:10 GMT  
		Size: 3.8 MB (3774441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54270160df8d1b1d48a5e855464e3400a606022608035ba66e6914d03dd235f1`  
		Last Modified: Wed, 01 Apr 2020 06:08:08 GMT  
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
$ docker pull nats@sha256:749649b3ae8a91032076aaa300a79c0fb4497ca8106c3952af344ab8474ceb94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64

### `nats:nanoserver` - windows version 10.0.17763.1217; amd64

```console
$ docker pull nats@sha256:87d7512bdc9d1226af1b312aa729660e09e95389183c3d488ce15b0f8bf09fe5
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105061846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8852e70f71f58a4bc75aed961cd7cc5ddec1fc483e7fd17f20bfe4e8e89b1e70`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 May 2020 12:39:06 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 14:50:51 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 May 2020 14:50:52 GMT
RUN cmd /S /C #(nop) COPY file:5493aca6ccb800df74d7e7b98176527689b02c807794603a1f7dde376217279b in C:\nats-server.exe 
# Wed, 13 May 2020 14:50:54 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 May 2020 14:50:55 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 May 2020 14:50:56 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 May 2020 14:50:57 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b9e6fec25718aef5ed18d499b27e43adb524f9ee4f2eb3f0fffaea018e7e86b0`  
		Size: 101.0 MB (101019852 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eafb3f3d63d93b402dfcc428e091787a4242326bc71283a6e3ad40046a60cba0`  
		Last Modified: Wed, 13 May 2020 14:55:00 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be222cbce7c5fdc837c8334dba94184d6668f565b5330de1d5979c73aeeee084`  
		Last Modified: Wed, 13 May 2020 14:54:59 GMT  
		Size: 4.0 MB (4036982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ec160b0022b6d17fb0f35f3c82d9a64610e13d8f82f37adb2d94a41ebc82d2`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 1.5 KB (1498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e6543f6d7c7f56c892ddae258ff87ccf91344dc58fd3781de1949aed35cb431`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a063fcb9d7392f7823b459c27227c671814eef764a3a30a824eb40e0acb5a9`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540bee75308cb6ecf746719faa19454db1d8eedc79dc5ee409528aae0e9a4c87`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:749649b3ae8a91032076aaa300a79c0fb4497ca8106c3952af344ab8474ceb94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.1217; amd64

```console
$ docker pull nats@sha256:87d7512bdc9d1226af1b312aa729660e09e95389183c3d488ce15b0f8bf09fe5
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105061846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8852e70f71f58a4bc75aed961cd7cc5ddec1fc483e7fd17f20bfe4e8e89b1e70`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 May 2020 12:39:06 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 14:50:51 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 May 2020 14:50:52 GMT
RUN cmd /S /C #(nop) COPY file:5493aca6ccb800df74d7e7b98176527689b02c807794603a1f7dde376217279b in C:\nats-server.exe 
# Wed, 13 May 2020 14:50:54 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 May 2020 14:50:55 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 May 2020 14:50:56 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 May 2020 14:50:57 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b9e6fec25718aef5ed18d499b27e43adb524f9ee4f2eb3f0fffaea018e7e86b0`  
		Size: 101.0 MB (101019852 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eafb3f3d63d93b402dfcc428e091787a4242326bc71283a6e3ad40046a60cba0`  
		Last Modified: Wed, 13 May 2020 14:55:00 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be222cbce7c5fdc837c8334dba94184d6668f565b5330de1d5979c73aeeee084`  
		Last Modified: Wed, 13 May 2020 14:54:59 GMT  
		Size: 4.0 MB (4036982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ec160b0022b6d17fb0f35f3c82d9a64610e13d8f82f37adb2d94a41ebc82d2`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 1.5 KB (1498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e6543f6d7c7f56c892ddae258ff87ccf91344dc58fd3781de1949aed35cb431`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a063fcb9d7392f7823b459c27227c671814eef764a3a30a824eb40e0acb5a9`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540bee75308cb6ecf746719faa19454db1d8eedc79dc5ee409528aae0e9a4c87`  
		Last Modified: Wed, 13 May 2020 14:54:58 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:4dd85d386b2572917793b417e434162febf14a527e6d0fb9482d98ecdf72b4f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:03f7a9538ca823f3e342254f0e0bd62fce56410fd037d70f11e208a64b9be51b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4068777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61d7629fb1351a52582452f08d569ef8aa395377751df3706474cb5769e8400d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 01 Apr 2020 06:49:28 GMT
COPY file:b5fc4f9d62c474e25c56f62242c0cbb4f21e732408978c639846820bd9b440a3 in /nats-server 
# Wed, 01 Apr 2020 06:49:28 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 01 Apr 2020 06:49:28 GMT
EXPOSE 4222 6222 8222
# Wed, 01 Apr 2020 06:49:29 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 01 Apr 2020 06:49:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9bafc186f2720cd817d9a0dca0d2d85b62db3667b346e18ad3cedee711853463`  
		Last Modified: Wed, 01 Apr 2020 06:49:48 GMT  
		Size: 4.1 MB (4068300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc99d87cfb673f46f50d4862e4486d00a26509752daa87beb60702054d53a2f8`  
		Last Modified: Wed, 01 Apr 2020 06:49:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:eff9f3146f76a2f78e896166707efdecae7f4aa7510d78cb4e986a578119bfb5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3781960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f158c883c70044a613a0b0a5bb6096487ac305e3f6f1b3e57a17a9f98bdaf09e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 31 Mar 2020 20:53:55 GMT
COPY file:5131c35b89e2bccdb55c8f10be46601f1fb947279308495595024bc0e2b29d5b in /nats-server 
# Tue, 31 Mar 2020 20:53:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 31 Mar 2020 20:53:57 GMT
EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 20:53:58 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 31 Mar 2020 20:53:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:705a3cd49f0567c17013b0eddbe53e6cffedd428744250d7076a8396babbe655`  
		Last Modified: Tue, 31 Mar 2020 20:54:42 GMT  
		Size: 3.8 MB (3781482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efabc067a958db0c40714b9365000273b61d5d19c9ce96c291b023d4ef2933f2`  
		Last Modified: Tue, 31 Mar 2020 20:54:41 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:bdda6b6ae6c62c1e78f902992214eca27cf00de2fc7d8d47235a663b3b35940a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3774917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7120ba5b06cdd64603f112b86a27c044b9e157fbfc6bdfad548f92351f75bbfe`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 01 Apr 2020 06:07:20 GMT
COPY file:846a74a5cdf1833ec24475ab97e1c375ea237825039dd6ad1d133be2c007faaf in /nats-server 
# Wed, 01 Apr 2020 06:07:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 01 Apr 2020 06:07:23 GMT
EXPOSE 4222 6222 8222
# Wed, 01 Apr 2020 06:07:24 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 01 Apr 2020 06:07:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3779a152c2262214f75fbef66a9ffa608a8a92efab5ce35515692282ae11c664`  
		Last Modified: Wed, 01 Apr 2020 06:08:10 GMT  
		Size: 3.8 MB (3774441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54270160df8d1b1d48a5e855464e3400a606022608035ba66e6914d03dd235f1`  
		Last Modified: Wed, 01 Apr 2020 06:08:08 GMT  
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
$ docker pull nats@sha256:49929c7e96cbd4d94b770c933fcdaa37523959b204770bcb8c6c64f39fd4d947
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64
	-	windows version 10.0.14393.3686; amd64

### `nats:windowsservercore` - windows version 10.0.17763.1217; amd64

```console
$ docker pull nats@sha256:38026bfd66cb1fe200a770ca74212b1855c9d6e853fb85ee00a3e18d58fee528
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1723030054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b410b6db1876f6835ba24bf47a165f529096991afa5e4d33092e7a9ea98682f6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 14:49:24 GMT
ENV NATS_DOCKERIZED=1
# Wed, 13 May 2020 14:49:25 GMT
ENV NATS_SERVER=2.1.6
# Wed, 13 May 2020 14:49:26 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Wed, 13 May 2020 14:49:46 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 May 2020 14:50:36 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 13 May 2020 14:50:37 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 May 2020 14:50:38 GMT
EXPOSE 4222 6222 8222
# Wed, 13 May 2020 14:50:39 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 May 2020 14:50:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6e220442d94ba050201e82fee90c58b5e714748e7906735032367404c473c91c`  
		Last Modified: Wed, 13 May 2020 14:27:38 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef78e6a0bb5c035fff387c2c5470bd8420babb53d74f1856b9e3ed900cd9af2`  
		Last Modified: Wed, 13 May 2020 14:54:40 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dcd0914a5c43759060ab8392ec986ac4a069accb2f9ce3fca4679b0a87d7c85`  
		Last Modified: Wed, 13 May 2020 14:54:40 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba2a9d9207a00a2aba1b3b0de0b4db3934394753808436964a988e33ee50f16`  
		Last Modified: Wed, 13 May 2020 14:54:40 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09721620d75a2711884513342bc0a1b80426f003a3fdd249f0449ae4e1d9ce5f`  
		Last Modified: Wed, 13 May 2020 14:54:40 GMT  
		Size: 340.9 KB (340876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfcdaddc68d3cecea8ab4b0121b52da7095d99088355df82ac59018d7dba025b`  
		Last Modified: Wed, 13 May 2020 14:54:43 GMT  
		Size: 4.3 MB (4346515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16f585abe2b7c6d8415117f4384304b4da7c7fa6bbde520ed7bc18e91d14d9e`  
		Last Modified: Wed, 13 May 2020 14:54:37 GMT  
		Size: 1.7 KB (1668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346112a5bf4cdc128a1a3469d52d43260ad562186d42e62b893e7850c660fa92`  
		Last Modified: Wed, 13 May 2020 14:54:37 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed443118936053d562d611d97fc3e38c75cd300f041dbd01171aa05ffd93bd10`  
		Last Modified: Wed, 13 May 2020 14:54:37 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9c7dfc60965547df88e7309ea367bb10050126f47110a7030f1ca563a9ce15`  
		Last Modified: Wed, 13 May 2020 14:54:37 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:windowsservercore` - windows version 10.0.14393.3686; amd64

```console
$ docker pull nats@sha256:9ac0a1a8b7c1d86e67b07c27da69c167bc06e4dd3d83235376b9441c2c7254dd
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5751199562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccc507bd9c022cd0ed7dbbd09cfa5913d866c520bcb826bfb6132ea62ea27549`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 14:51:03 GMT
ENV NATS_DOCKERIZED=1
# Wed, 13 May 2020 14:51:04 GMT
ENV NATS_SERVER=2.1.6
# Wed, 13 May 2020 14:51:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Wed, 13 May 2020 14:52:07 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 May 2020 14:54:02 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 13 May 2020 14:54:04 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 May 2020 14:54:06 GMT
EXPOSE 4222 6222 8222
# Wed, 13 May 2020 14:54:07 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 May 2020 14:54:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:78d9ecf24b3b7ef3e61c8b38d40e28e57a80552d6c97884f4cc142af2110ddff`  
		Last Modified: Wed, 13 May 2020 14:28:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5356fa8d07c48624dd3553b12cafae53b1e6818e2e77c7b4ad7c5e37a6edf5f5`  
		Last Modified: Wed, 13 May 2020 14:55:20 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:812d925d5330efdd0e3691f27be756f2d4bd21271b3d92a1fdbd7d0015ca751b`  
		Last Modified: Wed, 13 May 2020 14:55:21 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa02c160a78fb2c0432fda99964268c0d0be0c92dd4faad28abdc2aa3e9f2f3f`  
		Last Modified: Wed, 13 May 2020 14:55:20 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58a8e2f37803c472c8d10d3693e28446f643f41b20e716c97bb2cf561471f3c`  
		Last Modified: Wed, 13 May 2020 14:55:22 GMT  
		Size: 5.4 MB (5380611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a364666bd4bf347aa0241e06563fe518267439e92df88dd4c943475a6be316`  
		Last Modified: Wed, 13 May 2020 14:55:33 GMT  
		Size: 13.9 MB (13919327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07365ad87d191e5cdc05d203b8f0491d7c408b9cdbb94a131c53b05807f67f40`  
		Last Modified: Wed, 13 May 2020 14:55:17 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635bf5adfaf150aa00c8b9fe7bbfe96bfe97dbfee94544af1ad694e38cd7446c`  
		Last Modified: Wed, 13 May 2020 14:55:18 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84243df3097f51931f380c65fdf517d4a61a9a052a35d3fc8847695ca727781c`  
		Last Modified: Wed, 13 May 2020 14:55:17 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51aec177c2f2c1b498277b9130ad9ff47c26a7cb4057adf463705fc2fc671029`  
		Last Modified: Wed, 13 May 2020 14:55:18 GMT  
		Size: 1.1 KB (1104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:a122adcc06b520dba3748d187fe8cec27a8b4a57cd15624d669b616cbd0b53e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.1217; amd64

```console
$ docker pull nats@sha256:38026bfd66cb1fe200a770ca74212b1855c9d6e853fb85ee00a3e18d58fee528
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1723030054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b410b6db1876f6835ba24bf47a165f529096991afa5e4d33092e7a9ea98682f6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 14:49:24 GMT
ENV NATS_DOCKERIZED=1
# Wed, 13 May 2020 14:49:25 GMT
ENV NATS_SERVER=2.1.6
# Wed, 13 May 2020 14:49:26 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Wed, 13 May 2020 14:49:46 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 May 2020 14:50:36 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 13 May 2020 14:50:37 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 May 2020 14:50:38 GMT
EXPOSE 4222 6222 8222
# Wed, 13 May 2020 14:50:39 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 May 2020 14:50:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6e220442d94ba050201e82fee90c58b5e714748e7906735032367404c473c91c`  
		Last Modified: Wed, 13 May 2020 14:27:38 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef78e6a0bb5c035fff387c2c5470bd8420babb53d74f1856b9e3ed900cd9af2`  
		Last Modified: Wed, 13 May 2020 14:54:40 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dcd0914a5c43759060ab8392ec986ac4a069accb2f9ce3fca4679b0a87d7c85`  
		Last Modified: Wed, 13 May 2020 14:54:40 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba2a9d9207a00a2aba1b3b0de0b4db3934394753808436964a988e33ee50f16`  
		Last Modified: Wed, 13 May 2020 14:54:40 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09721620d75a2711884513342bc0a1b80426f003a3fdd249f0449ae4e1d9ce5f`  
		Last Modified: Wed, 13 May 2020 14:54:40 GMT  
		Size: 340.9 KB (340876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfcdaddc68d3cecea8ab4b0121b52da7095d99088355df82ac59018d7dba025b`  
		Last Modified: Wed, 13 May 2020 14:54:43 GMT  
		Size: 4.3 MB (4346515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16f585abe2b7c6d8415117f4384304b4da7c7fa6bbde520ed7bc18e91d14d9e`  
		Last Modified: Wed, 13 May 2020 14:54:37 GMT  
		Size: 1.7 KB (1668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346112a5bf4cdc128a1a3469d52d43260ad562186d42e62b893e7850c660fa92`  
		Last Modified: Wed, 13 May 2020 14:54:37 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed443118936053d562d611d97fc3e38c75cd300f041dbd01171aa05ffd93bd10`  
		Last Modified: Wed, 13 May 2020 14:54:37 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9c7dfc60965547df88e7309ea367bb10050126f47110a7030f1ca563a9ce15`  
		Last Modified: Wed, 13 May 2020 14:54:37 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:08c9781136f212ba6156cc3bb7d0371eb17053726b1ce2a851b01ba0fd721895
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3686; amd64

### `nats:windowsservercore-ltsc2016` - windows version 10.0.14393.3686; amd64

```console
$ docker pull nats@sha256:9ac0a1a8b7c1d86e67b07c27da69c167bc06e4dd3d83235376b9441c2c7254dd
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5751199562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccc507bd9c022cd0ed7dbbd09cfa5913d866c520bcb826bfb6132ea62ea27549`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 14:51:03 GMT
ENV NATS_DOCKERIZED=1
# Wed, 13 May 2020 14:51:04 GMT
ENV NATS_SERVER=2.1.6
# Wed, 13 May 2020 14:51:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Wed, 13 May 2020 14:52:07 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 May 2020 14:54:02 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 13 May 2020 14:54:04 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 May 2020 14:54:06 GMT
EXPOSE 4222 6222 8222
# Wed, 13 May 2020 14:54:07 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 May 2020 14:54:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:78d9ecf24b3b7ef3e61c8b38d40e28e57a80552d6c97884f4cc142af2110ddff`  
		Last Modified: Wed, 13 May 2020 14:28:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5356fa8d07c48624dd3553b12cafae53b1e6818e2e77c7b4ad7c5e37a6edf5f5`  
		Last Modified: Wed, 13 May 2020 14:55:20 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:812d925d5330efdd0e3691f27be756f2d4bd21271b3d92a1fdbd7d0015ca751b`  
		Last Modified: Wed, 13 May 2020 14:55:21 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa02c160a78fb2c0432fda99964268c0d0be0c92dd4faad28abdc2aa3e9f2f3f`  
		Last Modified: Wed, 13 May 2020 14:55:20 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58a8e2f37803c472c8d10d3693e28446f643f41b20e716c97bb2cf561471f3c`  
		Last Modified: Wed, 13 May 2020 14:55:22 GMT  
		Size: 5.4 MB (5380611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a364666bd4bf347aa0241e06563fe518267439e92df88dd4c943475a6be316`  
		Last Modified: Wed, 13 May 2020 14:55:33 GMT  
		Size: 13.9 MB (13919327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07365ad87d191e5cdc05d203b8f0491d7c408b9cdbb94a131c53b05807f67f40`  
		Last Modified: Wed, 13 May 2020 14:55:17 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635bf5adfaf150aa00c8b9fe7bbfe96bfe97dbfee94544af1ad694e38cd7446c`  
		Last Modified: Wed, 13 May 2020 14:55:18 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84243df3097f51931f380c65fdf517d4a61a9a052a35d3fc8847695ca727781c`  
		Last Modified: Wed, 13 May 2020 14:55:17 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51aec177c2f2c1b498277b9130ad9ff47c26a7cb4057adf463705fc2fc671029`  
		Last Modified: Wed, 13 May 2020 14:55:18 GMT  
		Size: 1.1 KB (1104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
