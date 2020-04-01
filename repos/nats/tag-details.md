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
$ docker pull nats@sha256:5f1b3d8c699cdaf8fa11f0a65bb431f5138cb2c56958cace2fd8a7f242367a25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1098; amd64

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

### `nats:2` - windows version 10.0.17763.1098; amd64

```console
$ docker pull nats@sha256:4ec9c8b5fc9c9f5ea875830d8355ac6e9f93d0e3fe5d374d24a5eb6bdf2608fa
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105092070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7678424b503caf1f5241062780f3e6969a8867e91fa257eff465274911c9568`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 Mar 2020 13:28:48 GMT
RUN Apply image 1809-amd64
# Wed, 11 Mar 2020 14:47:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 31 Mar 2020 21:16:16 GMT
RUN cmd /S /C #(nop) COPY file:5493aca6ccb800df74d7e7b98176527689b02c807794603a1f7dde376217279b in C:\nats-server.exe 
# Tue, 31 Mar 2020 21:16:18 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 31 Mar 2020 21:16:19 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 21:16:20 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 31 Mar 2020 21:16:20 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8e709836e4dce2fa52689be79fedc1e3d040ba47ec2da2fc3b23f33fc6944b50`  
		Size: 101.1 MB (101050245 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:11472ae705112ae5e29e58c937ca3e026bd8eb756b2fcbe538bba856f7d80ff9`  
		Last Modified: Wed, 11 Mar 2020 14:48:32 GMT  
		Size: 938.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e455632008f14f11f8b72d69a1da128950a141735926961bcf2baf8c2ae12c2`  
		Last Modified: Tue, 31 Mar 2020 21:20:05 GMT  
		Size: 4.0 MB (4036943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f44539e2ede61bafd54f622e8042099620ea0dafd8c87cf6043d295f17932f6`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030bd5a2e51cc12afa370bd2ec9b2ba2c6ad83cb09ce43555d0ba3b3eb497b49`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 835.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670e0425975dec676f07849687918818aa9a711883c2e2b6d39f40c1d922b71b`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 862.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ec1ea0b29e208f3799b3561fef99ab4b126884eeea9301d6c55f699847d80d`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 825.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1`

```console
$ docker pull nats@sha256:5f1b3d8c699cdaf8fa11f0a65bb431f5138cb2c56958cace2fd8a7f242367a25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1098; amd64

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

### `nats:2.1` - windows version 10.0.17763.1098; amd64

```console
$ docker pull nats@sha256:4ec9c8b5fc9c9f5ea875830d8355ac6e9f93d0e3fe5d374d24a5eb6bdf2608fa
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105092070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7678424b503caf1f5241062780f3e6969a8867e91fa257eff465274911c9568`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 Mar 2020 13:28:48 GMT
RUN Apply image 1809-amd64
# Wed, 11 Mar 2020 14:47:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 31 Mar 2020 21:16:16 GMT
RUN cmd /S /C #(nop) COPY file:5493aca6ccb800df74d7e7b98176527689b02c807794603a1f7dde376217279b in C:\nats-server.exe 
# Tue, 31 Mar 2020 21:16:18 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 31 Mar 2020 21:16:19 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 21:16:20 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 31 Mar 2020 21:16:20 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8e709836e4dce2fa52689be79fedc1e3d040ba47ec2da2fc3b23f33fc6944b50`  
		Size: 101.1 MB (101050245 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:11472ae705112ae5e29e58c937ca3e026bd8eb756b2fcbe538bba856f7d80ff9`  
		Last Modified: Wed, 11 Mar 2020 14:48:32 GMT  
		Size: 938.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e455632008f14f11f8b72d69a1da128950a141735926961bcf2baf8c2ae12c2`  
		Last Modified: Tue, 31 Mar 2020 21:20:05 GMT  
		Size: 4.0 MB (4036943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f44539e2ede61bafd54f622e8042099620ea0dafd8c87cf6043d295f17932f6`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030bd5a2e51cc12afa370bd2ec9b2ba2c6ad83cb09ce43555d0ba3b3eb497b49`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 835.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670e0425975dec676f07849687918818aa9a711883c2e2b6d39f40c1d922b71b`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 862.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ec1ea0b29e208f3799b3561fef99ab4b126884eeea9301d6c55f699847d80d`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 825.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.6`

```console
$ docker pull nats@sha256:c1c4706eb89551e889b729742b3cbff9d84d6077fca45064d3fa0d9813442937
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	windows version 10.0.17763.1098; amd64

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

### `nats:2.1.6` - windows version 10.0.17763.1098; amd64

```console
$ docker pull nats@sha256:4ec9c8b5fc9c9f5ea875830d8355ac6e9f93d0e3fe5d374d24a5eb6bdf2608fa
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105092070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7678424b503caf1f5241062780f3e6969a8867e91fa257eff465274911c9568`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 Mar 2020 13:28:48 GMT
RUN Apply image 1809-amd64
# Wed, 11 Mar 2020 14:47:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 31 Mar 2020 21:16:16 GMT
RUN cmd /S /C #(nop) COPY file:5493aca6ccb800df74d7e7b98176527689b02c807794603a1f7dde376217279b in C:\nats-server.exe 
# Tue, 31 Mar 2020 21:16:18 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 31 Mar 2020 21:16:19 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 21:16:20 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 31 Mar 2020 21:16:20 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8e709836e4dce2fa52689be79fedc1e3d040ba47ec2da2fc3b23f33fc6944b50`  
		Size: 101.1 MB (101050245 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:11472ae705112ae5e29e58c937ca3e026bd8eb756b2fcbe538bba856f7d80ff9`  
		Last Modified: Wed, 11 Mar 2020 14:48:32 GMT  
		Size: 938.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e455632008f14f11f8b72d69a1da128950a141735926961bcf2baf8c2ae12c2`  
		Last Modified: Tue, 31 Mar 2020 21:20:05 GMT  
		Size: 4.0 MB (4036943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f44539e2ede61bafd54f622e8042099620ea0dafd8c87cf6043d295f17932f6`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030bd5a2e51cc12afa370bd2ec9b2ba2c6ad83cb09ce43555d0ba3b3eb497b49`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 835.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670e0425975dec676f07849687918818aa9a711883c2e2b6d39f40c1d922b71b`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 862.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ec1ea0b29e208f3799b3561fef99ab4b126884eeea9301d6c55f699847d80d`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 825.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.6-alpine`

```console
$ docker pull nats@sha256:2187a6653c7c4e78db59e22bd5fbbe25b43b8f3253df398d61751bdb80cb0aa7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats:2.1.6-alpine` - linux; amd64

```console
$ docker pull nats@sha256:306471c8b6440327201e8078fe735e4e703cfda47e00980a018adfe41a801fb6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7175368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d816644c99a5174a9ac5e95b93b977eed6723785fa06810f538ee1bd625d4239`
-	Default Command: `["nats-server"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Wed, 01 Apr 2020 06:49:16 GMT
ENV NATS_SERVER=2.1.6
# Wed, 01 Apr 2020 06:49:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 01 Apr 2020 06:49:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 01 Apr 2020 06:49:18 GMT
EXPOSE 4222 6222 8222
# Wed, 01 Apr 2020 06:49:18 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ec7c5cccacb89b8af24413a53fdb893b60bc947b226d2c7e2735016efd0e8f`  
		Last Modified: Wed, 01 Apr 2020 06:49:41 GMT  
		Size: 4.4 MB (4371583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80c118a8e6ccf42f7aa4e34428dc07dcbd2d8d7cff7eb910e0067bfd7f38ada`  
		Last Modified: Wed, 01 Apr 2020 06:49:40 GMT  
		Size: 530.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.6-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:bce00d9d88bc4c6fba21488335026e3102f66ee55daa353311345e5c807b2458
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6702865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b23480fa7be718a41b7727b4ddc07dde9ddd114da9d7d54e8072b2c408844458`
-	Default Command: `["nats-server"]`

```dockerfile
# Mon, 23 Mar 2020 21:49:26 GMT
ADD file:e2fdfc637b534345942caf4097883508a5ed23be97d85ccc3357b8277aaa5430 in / 
# Mon, 23 Mar 2020 21:49:27 GMT
CMD ["/bin/sh"]
# Tue, 31 Mar 2020 20:49:36 GMT
ENV NATS_SERVER=2.1.6
# Tue, 31 Mar 2020 20:49:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 31 Mar 2020 20:49:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 31 Mar 2020 20:49:52 GMT
EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 20:49:53 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:0776aeec3430c5a5ba3f43937f0ee6a7770a1fe81a318c9d94cc76512e5375e9`  
		Last Modified: Mon, 23 Mar 2020 21:49:50 GMT  
		Size: 2.6 MB (2618579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1de55532fc814c4a862e789c611472b72868c4fd20d806e8062eaafe58dd641`  
		Last Modified: Tue, 31 Mar 2020 20:54:29 GMT  
		Size: 4.1 MB (4083724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f6c7842c241e086a908b5ff2159b1add2ffd4d10e4ba2b7519709c326d53b3c`  
		Last Modified: Tue, 31 Mar 2020 20:54:28 GMT  
		Size: 562.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.6-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:9914b699049a64964fdcea31b1777b01b03a195466f4d26f6cb9b21c3f608be1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6497861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05e93c4064d5ecafbd500bc7252d1ecbc4785fc5162e2b6d5c1a1ef29ce76aab`
-	Default Command: `["nats-server"]`

```dockerfile
# Mon, 23 Mar 2020 21:57:55 GMT
ADD file:3bde6b6fd06efbf24e66446c6d32f72294fc749ae9ee6191776242e92b2f8ab4 in / 
# Mon, 23 Mar 2020 21:57:56 GMT
CMD ["/bin/sh"]
# Wed, 01 Apr 2020 06:01:54 GMT
ENV NATS_SERVER=2.1.6
# Wed, 01 Apr 2020 06:01:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 01 Apr 2020 06:01:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 01 Apr 2020 06:02:00 GMT
EXPOSE 4222 6222 8222
# Wed, 01 Apr 2020 06:02:01 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:d9bf605ce3d4449f4b90035c3e21d691806324781d43a5287b1da25a01779d6b`  
		Last Modified: Mon, 23 Mar 2020 21:58:16 GMT  
		Size: 2.4 MB (2420493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23dfc407cfb62fcc989fc550e01b071587084a28b301a1716e2c71112a2b51e`  
		Last Modified: Wed, 01 Apr 2020 06:07:55 GMT  
		Size: 4.1 MB (4076812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75090e66199501633c177682c4bef49fc00b0f80abb29a8abe7e1af6f3cdec8c`  
		Last Modified: Wed, 01 Apr 2020 06:07:54 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.6-alpine3.11`

```console
$ docker pull nats@sha256:2187a6653c7c4e78db59e22bd5fbbe25b43b8f3253df398d61751bdb80cb0aa7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats:2.1.6-alpine3.11` - linux; amd64

```console
$ docker pull nats@sha256:306471c8b6440327201e8078fe735e4e703cfda47e00980a018adfe41a801fb6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7175368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d816644c99a5174a9ac5e95b93b977eed6723785fa06810f538ee1bd625d4239`
-	Default Command: `["nats-server"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Wed, 01 Apr 2020 06:49:16 GMT
ENV NATS_SERVER=2.1.6
# Wed, 01 Apr 2020 06:49:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 01 Apr 2020 06:49:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 01 Apr 2020 06:49:18 GMT
EXPOSE 4222 6222 8222
# Wed, 01 Apr 2020 06:49:18 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ec7c5cccacb89b8af24413a53fdb893b60bc947b226d2c7e2735016efd0e8f`  
		Last Modified: Wed, 01 Apr 2020 06:49:41 GMT  
		Size: 4.4 MB (4371583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80c118a8e6ccf42f7aa4e34428dc07dcbd2d8d7cff7eb910e0067bfd7f38ada`  
		Last Modified: Wed, 01 Apr 2020 06:49:40 GMT  
		Size: 530.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.6-alpine3.11` - linux; arm variant v6

```console
$ docker pull nats@sha256:bce00d9d88bc4c6fba21488335026e3102f66ee55daa353311345e5c807b2458
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6702865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b23480fa7be718a41b7727b4ddc07dde9ddd114da9d7d54e8072b2c408844458`
-	Default Command: `["nats-server"]`

```dockerfile
# Mon, 23 Mar 2020 21:49:26 GMT
ADD file:e2fdfc637b534345942caf4097883508a5ed23be97d85ccc3357b8277aaa5430 in / 
# Mon, 23 Mar 2020 21:49:27 GMT
CMD ["/bin/sh"]
# Tue, 31 Mar 2020 20:49:36 GMT
ENV NATS_SERVER=2.1.6
# Tue, 31 Mar 2020 20:49:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 31 Mar 2020 20:49:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 31 Mar 2020 20:49:52 GMT
EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 20:49:53 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:0776aeec3430c5a5ba3f43937f0ee6a7770a1fe81a318c9d94cc76512e5375e9`  
		Last Modified: Mon, 23 Mar 2020 21:49:50 GMT  
		Size: 2.6 MB (2618579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1de55532fc814c4a862e789c611472b72868c4fd20d806e8062eaafe58dd641`  
		Last Modified: Tue, 31 Mar 2020 20:54:29 GMT  
		Size: 4.1 MB (4083724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f6c7842c241e086a908b5ff2159b1add2ffd4d10e4ba2b7519709c326d53b3c`  
		Last Modified: Tue, 31 Mar 2020 20:54:28 GMT  
		Size: 562.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.6-alpine3.11` - linux; arm variant v7

```console
$ docker pull nats@sha256:9914b699049a64964fdcea31b1777b01b03a195466f4d26f6cb9b21c3f608be1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6497861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05e93c4064d5ecafbd500bc7252d1ecbc4785fc5162e2b6d5c1a1ef29ce76aab`
-	Default Command: `["nats-server"]`

```dockerfile
# Mon, 23 Mar 2020 21:57:55 GMT
ADD file:3bde6b6fd06efbf24e66446c6d32f72294fc749ae9ee6191776242e92b2f8ab4 in / 
# Mon, 23 Mar 2020 21:57:56 GMT
CMD ["/bin/sh"]
# Wed, 01 Apr 2020 06:01:54 GMT
ENV NATS_SERVER=2.1.6
# Wed, 01 Apr 2020 06:01:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 01 Apr 2020 06:01:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 01 Apr 2020 06:02:00 GMT
EXPOSE 4222 6222 8222
# Wed, 01 Apr 2020 06:02:01 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:d9bf605ce3d4449f4b90035c3e21d691806324781d43a5287b1da25a01779d6b`  
		Last Modified: Mon, 23 Mar 2020 21:58:16 GMT  
		Size: 2.4 MB (2420493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23dfc407cfb62fcc989fc550e01b071587084a28b301a1716e2c71112a2b51e`  
		Last Modified: Wed, 01 Apr 2020 06:07:55 GMT  
		Size: 4.1 MB (4076812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75090e66199501633c177682c4bef49fc00b0f80abb29a8abe7e1af6f3cdec8c`  
		Last Modified: Wed, 01 Apr 2020 06:07:54 GMT  
		Size: 556.0 B  
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
$ docker pull nats@sha256:aea7cc2831f9abd383f4174e38b17849df3606beea6648d63b824eb2a8b88dbd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `nats:2.1.6-nanoserver` - windows version 10.0.17763.1098; amd64

```console
$ docker pull nats@sha256:4ec9c8b5fc9c9f5ea875830d8355ac6e9f93d0e3fe5d374d24a5eb6bdf2608fa
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105092070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7678424b503caf1f5241062780f3e6969a8867e91fa257eff465274911c9568`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 Mar 2020 13:28:48 GMT
RUN Apply image 1809-amd64
# Wed, 11 Mar 2020 14:47:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 31 Mar 2020 21:16:16 GMT
RUN cmd /S /C #(nop) COPY file:5493aca6ccb800df74d7e7b98176527689b02c807794603a1f7dde376217279b in C:\nats-server.exe 
# Tue, 31 Mar 2020 21:16:18 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 31 Mar 2020 21:16:19 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 21:16:20 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 31 Mar 2020 21:16:20 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8e709836e4dce2fa52689be79fedc1e3d040ba47ec2da2fc3b23f33fc6944b50`  
		Size: 101.1 MB (101050245 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:11472ae705112ae5e29e58c937ca3e026bd8eb756b2fcbe538bba856f7d80ff9`  
		Last Modified: Wed, 11 Mar 2020 14:48:32 GMT  
		Size: 938.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e455632008f14f11f8b72d69a1da128950a141735926961bcf2baf8c2ae12c2`  
		Last Modified: Tue, 31 Mar 2020 21:20:05 GMT  
		Size: 4.0 MB (4036943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f44539e2ede61bafd54f622e8042099620ea0dafd8c87cf6043d295f17932f6`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030bd5a2e51cc12afa370bd2ec9b2ba2c6ad83cb09ce43555d0ba3b3eb497b49`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 835.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670e0425975dec676f07849687918818aa9a711883c2e2b6d39f40c1d922b71b`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 862.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ec1ea0b29e208f3799b3561fef99ab4b126884eeea9301d6c55f699847d80d`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 825.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.6-nanoserver-1809`

```console
$ docker pull nats@sha256:aea7cc2831f9abd383f4174e38b17849df3606beea6648d63b824eb2a8b88dbd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `nats:2.1.6-nanoserver-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull nats@sha256:4ec9c8b5fc9c9f5ea875830d8355ac6e9f93d0e3fe5d374d24a5eb6bdf2608fa
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105092070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7678424b503caf1f5241062780f3e6969a8867e91fa257eff465274911c9568`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 Mar 2020 13:28:48 GMT
RUN Apply image 1809-amd64
# Wed, 11 Mar 2020 14:47:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 31 Mar 2020 21:16:16 GMT
RUN cmd /S /C #(nop) COPY file:5493aca6ccb800df74d7e7b98176527689b02c807794603a1f7dde376217279b in C:\nats-server.exe 
# Tue, 31 Mar 2020 21:16:18 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 31 Mar 2020 21:16:19 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 21:16:20 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 31 Mar 2020 21:16:20 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8e709836e4dce2fa52689be79fedc1e3d040ba47ec2da2fc3b23f33fc6944b50`  
		Size: 101.1 MB (101050245 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:11472ae705112ae5e29e58c937ca3e026bd8eb756b2fcbe538bba856f7d80ff9`  
		Last Modified: Wed, 11 Mar 2020 14:48:32 GMT  
		Size: 938.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e455632008f14f11f8b72d69a1da128950a141735926961bcf2baf8c2ae12c2`  
		Last Modified: Tue, 31 Mar 2020 21:20:05 GMT  
		Size: 4.0 MB (4036943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f44539e2ede61bafd54f622e8042099620ea0dafd8c87cf6043d295f17932f6`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030bd5a2e51cc12afa370bd2ec9b2ba2c6ad83cb09ce43555d0ba3b3eb497b49`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 835.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670e0425975dec676f07849687918818aa9a711883c2e2b6d39f40c1d922b71b`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 862.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ec1ea0b29e208f3799b3561fef99ab4b126884eeea9301d6c55f699847d80d`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 825.0 B  
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
$ docker pull nats@sha256:0a0363aee1ab915ca6823f0cb8f5064cb561b8bd779b34b2167960a6d8d935d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64
	-	windows version 10.0.14393.3568; amd64

### `nats:2.1.6-windowsservercore` - windows version 10.0.17763.1098; amd64

```console
$ docker pull nats@sha256:e3a5d10d77bb9a35c8167bc655529206d03c0e7dac2c44f3b9da230c165781b7
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2278709759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:128cc6d6411b3c714e63facea2b4da51b0a7c042c7decc5d5634624f90d3f250`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Tue, 10 Mar 2020 23:23:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Mar 2020 14:45:12 GMT
ENV NATS_DOCKERIZED=1
# Tue, 31 Mar 2020 21:14:33 GMT
ENV NATS_SERVER=2.1.6
# Tue, 31 Mar 2020 21:14:34 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Tue, 31 Mar 2020 21:15:02 GMT
RUN Set-PSDebug -Trace 2
# Tue, 31 Mar 2020 21:16:01 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Tue, 31 Mar 2020 21:16:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 31 Mar 2020 21:16:03 GMT
EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 21:16:04 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 31 Mar 2020 21:16:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb49f89affc2d69b541463d095fdfbe61fa62e02b0aa5fa6d26bc134fb66bf35`  
		Last Modified: Wed, 11 Mar 2020 00:30:48 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ed96bfcc8cc17c8c1192c9f852f19ab1a2bcea7fa094f5e3f417f29b731f1e`  
		Last Modified: Wed, 11 Mar 2020 14:48:09 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18957d3bf61a5f19ebc5847b6ca77f7a7863643e54b7101511766974bad6b69`  
		Last Modified: Tue, 31 Mar 2020 21:19:48 GMT  
		Size: 1.1 KB (1096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b302c84191e1df029de15f2967d9a7b53246786fb26544da226b8c607925ff`  
		Last Modified: Tue, 31 Mar 2020 21:19:47 GMT  
		Size: 1.1 KB (1088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93836f3c0cffa6b0a37b955c3dce4dafe0642ab66960be80b1d74d406edf25c`  
		Last Modified: Tue, 31 Mar 2020 21:19:48 GMT  
		Size: 4.7 MB (4681616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ffbfa8e12b45b0c4d7bff5269d1ff7699720245d9e2037149c0477cd7c1a0e6`  
		Last Modified: Tue, 31 Mar 2020 21:19:46 GMT  
		Size: 8.7 MB (8682323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bea1418e16fcf97cee4031be619e7e26ef941739136dd28cd3f04451f9f132a`  
		Last Modified: Tue, 31 Mar 2020 21:19:44 GMT  
		Size: 1.6 KB (1628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941e7ca764c534845927416d06df263615a01f5f7e2a9aee1385322b761f6fc7`  
		Last Modified: Tue, 31 Mar 2020 21:19:45 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014dd1ff508af5046533914bacdc75ddaa7efdd00cc1327c448272dc08014353`  
		Last Modified: Tue, 31 Mar 2020 21:19:45 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e25f9b92198997df236a1495f0fc7bf389f99880eb61de4877d2e67ca58431a`  
		Last Modified: Tue, 31 Mar 2020 21:19:44 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.6-windowsservercore` - windows version 10.0.14393.3568; amd64

```console
$ docker pull nats@sha256:93e77d94d5181b2e8ca9efbacd8c6ef9401b54c6c318b9dd23b7e5751e1653d1
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 GB (5743587455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28335910c356ede194b2dcd9233b435a9cf6f610dd9c49e62c6bab814e302781`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 10 Mar 2020 08:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 18 Mar 2020 12:27:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 18 Mar 2020 13:38:31 GMT
ENV NATS_DOCKERIZED=1
# Tue, 31 Mar 2020 21:16:26 GMT
ENV NATS_SERVER=2.1.6
# Tue, 31 Mar 2020 21:16:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Tue, 31 Mar 2020 21:17:26 GMT
RUN Set-PSDebug -Trace 2
# Tue, 31 Mar 2020 21:19:04 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Tue, 31 Mar 2020 21:19:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 31 Mar 2020 21:19:07 GMT
EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 21:19:08 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 31 Mar 2020 21:19:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a5d20b7a2294a0d2631f74f49fc34574484a692913559546ef0bceae789fd7a8`  
		Size: 1.7 GB (1658775203 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8cd5aa189dca96a2d4bcc0e2516d85f8a69d277957f44aca08575ecf42e5bc2f`  
		Last Modified: Wed, 18 Mar 2020 13:22:17 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ddde0325982310255792cba68184203cd656b044bf4f46ab5c1ebf779122527`  
		Last Modified: Wed, 18 Mar 2020 13:42:12 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122d2e783014460190d162f128fa5710a117cd9136ff0582c542e645c5f0b10f`  
		Last Modified: Tue, 31 Mar 2020 21:20:23 GMT  
		Size: 1.1 KB (1080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0a23ecd71b35608af4c4e06f1857aab4211c34048dde0a2072401bc8421176`  
		Last Modified: Tue, 31 Mar 2020 21:20:23 GMT  
		Size: 1.1 KB (1088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9948d714ad0c8a48c12fe7b9becc3fabe09f61d4d66bd75cf77d91316713000e`  
		Last Modified: Tue, 31 Mar 2020 21:20:24 GMT  
		Size: 5.4 MB (5384998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f47e480e660c2de16210e4a70aaf550bd0dd240bf43f1766a7049cfe020cf25`  
		Last Modified: Tue, 31 Mar 2020 21:20:30 GMT  
		Size: 9.4 MB (9431821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d276126def9ffa1ac85e80e3ce86f78dc9f815bf1241f060c953972b16fe8459`  
		Last Modified: Tue, 31 Mar 2020 21:20:20 GMT  
		Size: 1.7 KB (1673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6342f41571faf0fe60bbb2d11b642f0a8499c91ee7b7b48806b4851a5ebd95b8`  
		Last Modified: Tue, 31 Mar 2020 21:20:20 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662962efab83cc3a58e4d9c59b9e23abc78f4f8634c5ea2d5b87034063037ec9`  
		Last Modified: Tue, 31 Mar 2020 21:20:20 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a4c33960d69a58662fa5a7dac06bd5ceaa709df8079062bf9f684318c0c1b0`  
		Last Modified: Tue, 31 Mar 2020 21:20:20 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.6-windowsservercore-1809`

```console
$ docker pull nats@sha256:186133a96780f6a775e4055406f8770a684424433af78e6189512064438e47c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `nats:2.1.6-windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull nats@sha256:e3a5d10d77bb9a35c8167bc655529206d03c0e7dac2c44f3b9da230c165781b7
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2278709759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:128cc6d6411b3c714e63facea2b4da51b0a7c042c7decc5d5634624f90d3f250`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Tue, 10 Mar 2020 23:23:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Mar 2020 14:45:12 GMT
ENV NATS_DOCKERIZED=1
# Tue, 31 Mar 2020 21:14:33 GMT
ENV NATS_SERVER=2.1.6
# Tue, 31 Mar 2020 21:14:34 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Tue, 31 Mar 2020 21:15:02 GMT
RUN Set-PSDebug -Trace 2
# Tue, 31 Mar 2020 21:16:01 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Tue, 31 Mar 2020 21:16:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 31 Mar 2020 21:16:03 GMT
EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 21:16:04 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 31 Mar 2020 21:16:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb49f89affc2d69b541463d095fdfbe61fa62e02b0aa5fa6d26bc134fb66bf35`  
		Last Modified: Wed, 11 Mar 2020 00:30:48 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ed96bfcc8cc17c8c1192c9f852f19ab1a2bcea7fa094f5e3f417f29b731f1e`  
		Last Modified: Wed, 11 Mar 2020 14:48:09 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18957d3bf61a5f19ebc5847b6ca77f7a7863643e54b7101511766974bad6b69`  
		Last Modified: Tue, 31 Mar 2020 21:19:48 GMT  
		Size: 1.1 KB (1096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b302c84191e1df029de15f2967d9a7b53246786fb26544da226b8c607925ff`  
		Last Modified: Tue, 31 Mar 2020 21:19:47 GMT  
		Size: 1.1 KB (1088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93836f3c0cffa6b0a37b955c3dce4dafe0642ab66960be80b1d74d406edf25c`  
		Last Modified: Tue, 31 Mar 2020 21:19:48 GMT  
		Size: 4.7 MB (4681616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ffbfa8e12b45b0c4d7bff5269d1ff7699720245d9e2037149c0477cd7c1a0e6`  
		Last Modified: Tue, 31 Mar 2020 21:19:46 GMT  
		Size: 8.7 MB (8682323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bea1418e16fcf97cee4031be619e7e26ef941739136dd28cd3f04451f9f132a`  
		Last Modified: Tue, 31 Mar 2020 21:19:44 GMT  
		Size: 1.6 KB (1628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941e7ca764c534845927416d06df263615a01f5f7e2a9aee1385322b761f6fc7`  
		Last Modified: Tue, 31 Mar 2020 21:19:45 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014dd1ff508af5046533914bacdc75ddaa7efdd00cc1327c448272dc08014353`  
		Last Modified: Tue, 31 Mar 2020 21:19:45 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e25f9b92198997df236a1495f0fc7bf389f99880eb61de4877d2e67ca58431a`  
		Last Modified: Tue, 31 Mar 2020 21:19:44 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.6-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:d35b6c4a3418f8ef1ba66c3bcc1a8b938fa440fd3718b2a63b4f66d4d9e2ad1b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3568; amd64

### `nats:2.1.6-windowsservercore-ltsc2016` - windows version 10.0.14393.3568; amd64

```console
$ docker pull nats@sha256:93e77d94d5181b2e8ca9efbacd8c6ef9401b54c6c318b9dd23b7e5751e1653d1
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 GB (5743587455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28335910c356ede194b2dcd9233b435a9cf6f610dd9c49e62c6bab814e302781`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 10 Mar 2020 08:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 18 Mar 2020 12:27:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 18 Mar 2020 13:38:31 GMT
ENV NATS_DOCKERIZED=1
# Tue, 31 Mar 2020 21:16:26 GMT
ENV NATS_SERVER=2.1.6
# Tue, 31 Mar 2020 21:16:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Tue, 31 Mar 2020 21:17:26 GMT
RUN Set-PSDebug -Trace 2
# Tue, 31 Mar 2020 21:19:04 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Tue, 31 Mar 2020 21:19:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 31 Mar 2020 21:19:07 GMT
EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 21:19:08 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 31 Mar 2020 21:19:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a5d20b7a2294a0d2631f74f49fc34574484a692913559546ef0bceae789fd7a8`  
		Size: 1.7 GB (1658775203 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8cd5aa189dca96a2d4bcc0e2516d85f8a69d277957f44aca08575ecf42e5bc2f`  
		Last Modified: Wed, 18 Mar 2020 13:22:17 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ddde0325982310255792cba68184203cd656b044bf4f46ab5c1ebf779122527`  
		Last Modified: Wed, 18 Mar 2020 13:42:12 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122d2e783014460190d162f128fa5710a117cd9136ff0582c542e645c5f0b10f`  
		Last Modified: Tue, 31 Mar 2020 21:20:23 GMT  
		Size: 1.1 KB (1080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0a23ecd71b35608af4c4e06f1857aab4211c34048dde0a2072401bc8421176`  
		Last Modified: Tue, 31 Mar 2020 21:20:23 GMT  
		Size: 1.1 KB (1088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9948d714ad0c8a48c12fe7b9becc3fabe09f61d4d66bd75cf77d91316713000e`  
		Last Modified: Tue, 31 Mar 2020 21:20:24 GMT  
		Size: 5.4 MB (5384998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f47e480e660c2de16210e4a70aaf550bd0dd240bf43f1766a7049cfe020cf25`  
		Last Modified: Tue, 31 Mar 2020 21:20:30 GMT  
		Size: 9.4 MB (9431821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d276126def9ffa1ac85e80e3ce86f78dc9f815bf1241f060c953972b16fe8459`  
		Last Modified: Tue, 31 Mar 2020 21:20:20 GMT  
		Size: 1.7 KB (1673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6342f41571faf0fe60bbb2d11b642f0a8499c91ee7b7b48806b4851a5ebd95b8`  
		Last Modified: Tue, 31 Mar 2020 21:20:20 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662962efab83cc3a58e4d9c59b9e23abc78f4f8634c5ea2d5b87034063037ec9`  
		Last Modified: Tue, 31 Mar 2020 21:20:20 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a4c33960d69a58662fa5a7dac06bd5ceaa709df8079062bf9f684318c0c1b0`  
		Last Modified: Tue, 31 Mar 2020 21:20:20 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-alpine`

```console
$ docker pull nats@sha256:2187a6653c7c4e78db59e22bd5fbbe25b43b8f3253df398d61751bdb80cb0aa7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats:2.1-alpine` - linux; amd64

```console
$ docker pull nats@sha256:306471c8b6440327201e8078fe735e4e703cfda47e00980a018adfe41a801fb6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7175368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d816644c99a5174a9ac5e95b93b977eed6723785fa06810f538ee1bd625d4239`
-	Default Command: `["nats-server"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Wed, 01 Apr 2020 06:49:16 GMT
ENV NATS_SERVER=2.1.6
# Wed, 01 Apr 2020 06:49:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 01 Apr 2020 06:49:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 01 Apr 2020 06:49:18 GMT
EXPOSE 4222 6222 8222
# Wed, 01 Apr 2020 06:49:18 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ec7c5cccacb89b8af24413a53fdb893b60bc947b226d2c7e2735016efd0e8f`  
		Last Modified: Wed, 01 Apr 2020 06:49:41 GMT  
		Size: 4.4 MB (4371583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80c118a8e6ccf42f7aa4e34428dc07dcbd2d8d7cff7eb910e0067bfd7f38ada`  
		Last Modified: Wed, 01 Apr 2020 06:49:40 GMT  
		Size: 530.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:bce00d9d88bc4c6fba21488335026e3102f66ee55daa353311345e5c807b2458
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6702865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b23480fa7be718a41b7727b4ddc07dde9ddd114da9d7d54e8072b2c408844458`
-	Default Command: `["nats-server"]`

```dockerfile
# Mon, 23 Mar 2020 21:49:26 GMT
ADD file:e2fdfc637b534345942caf4097883508a5ed23be97d85ccc3357b8277aaa5430 in / 
# Mon, 23 Mar 2020 21:49:27 GMT
CMD ["/bin/sh"]
# Tue, 31 Mar 2020 20:49:36 GMT
ENV NATS_SERVER=2.1.6
# Tue, 31 Mar 2020 20:49:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 31 Mar 2020 20:49:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 31 Mar 2020 20:49:52 GMT
EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 20:49:53 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:0776aeec3430c5a5ba3f43937f0ee6a7770a1fe81a318c9d94cc76512e5375e9`  
		Last Modified: Mon, 23 Mar 2020 21:49:50 GMT  
		Size: 2.6 MB (2618579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1de55532fc814c4a862e789c611472b72868c4fd20d806e8062eaafe58dd641`  
		Last Modified: Tue, 31 Mar 2020 20:54:29 GMT  
		Size: 4.1 MB (4083724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f6c7842c241e086a908b5ff2159b1add2ffd4d10e4ba2b7519709c326d53b3c`  
		Last Modified: Tue, 31 Mar 2020 20:54:28 GMT  
		Size: 562.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:9914b699049a64964fdcea31b1777b01b03a195466f4d26f6cb9b21c3f608be1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6497861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05e93c4064d5ecafbd500bc7252d1ecbc4785fc5162e2b6d5c1a1ef29ce76aab`
-	Default Command: `["nats-server"]`

```dockerfile
# Mon, 23 Mar 2020 21:57:55 GMT
ADD file:3bde6b6fd06efbf24e66446c6d32f72294fc749ae9ee6191776242e92b2f8ab4 in / 
# Mon, 23 Mar 2020 21:57:56 GMT
CMD ["/bin/sh"]
# Wed, 01 Apr 2020 06:01:54 GMT
ENV NATS_SERVER=2.1.6
# Wed, 01 Apr 2020 06:01:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 01 Apr 2020 06:01:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 01 Apr 2020 06:02:00 GMT
EXPOSE 4222 6222 8222
# Wed, 01 Apr 2020 06:02:01 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:d9bf605ce3d4449f4b90035c3e21d691806324781d43a5287b1da25a01779d6b`  
		Last Modified: Mon, 23 Mar 2020 21:58:16 GMT  
		Size: 2.4 MB (2420493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23dfc407cfb62fcc989fc550e01b071587084a28b301a1716e2c71112a2b51e`  
		Last Modified: Wed, 01 Apr 2020 06:07:55 GMT  
		Size: 4.1 MB (4076812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75090e66199501633c177682c4bef49fc00b0f80abb29a8abe7e1af6f3cdec8c`  
		Last Modified: Wed, 01 Apr 2020 06:07:54 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-alpine3.11`

```console
$ docker pull nats@sha256:2187a6653c7c4e78db59e22bd5fbbe25b43b8f3253df398d61751bdb80cb0aa7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats:2.1-alpine3.11` - linux; amd64

```console
$ docker pull nats@sha256:306471c8b6440327201e8078fe735e4e703cfda47e00980a018adfe41a801fb6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7175368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d816644c99a5174a9ac5e95b93b977eed6723785fa06810f538ee1bd625d4239`
-	Default Command: `["nats-server"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Wed, 01 Apr 2020 06:49:16 GMT
ENV NATS_SERVER=2.1.6
# Wed, 01 Apr 2020 06:49:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 01 Apr 2020 06:49:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 01 Apr 2020 06:49:18 GMT
EXPOSE 4222 6222 8222
# Wed, 01 Apr 2020 06:49:18 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ec7c5cccacb89b8af24413a53fdb893b60bc947b226d2c7e2735016efd0e8f`  
		Last Modified: Wed, 01 Apr 2020 06:49:41 GMT  
		Size: 4.4 MB (4371583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80c118a8e6ccf42f7aa4e34428dc07dcbd2d8d7cff7eb910e0067bfd7f38ada`  
		Last Modified: Wed, 01 Apr 2020 06:49:40 GMT  
		Size: 530.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-alpine3.11` - linux; arm variant v6

```console
$ docker pull nats@sha256:bce00d9d88bc4c6fba21488335026e3102f66ee55daa353311345e5c807b2458
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6702865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b23480fa7be718a41b7727b4ddc07dde9ddd114da9d7d54e8072b2c408844458`
-	Default Command: `["nats-server"]`

```dockerfile
# Mon, 23 Mar 2020 21:49:26 GMT
ADD file:e2fdfc637b534345942caf4097883508a5ed23be97d85ccc3357b8277aaa5430 in / 
# Mon, 23 Mar 2020 21:49:27 GMT
CMD ["/bin/sh"]
# Tue, 31 Mar 2020 20:49:36 GMT
ENV NATS_SERVER=2.1.6
# Tue, 31 Mar 2020 20:49:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 31 Mar 2020 20:49:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 31 Mar 2020 20:49:52 GMT
EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 20:49:53 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:0776aeec3430c5a5ba3f43937f0ee6a7770a1fe81a318c9d94cc76512e5375e9`  
		Last Modified: Mon, 23 Mar 2020 21:49:50 GMT  
		Size: 2.6 MB (2618579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1de55532fc814c4a862e789c611472b72868c4fd20d806e8062eaafe58dd641`  
		Last Modified: Tue, 31 Mar 2020 20:54:29 GMT  
		Size: 4.1 MB (4083724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f6c7842c241e086a908b5ff2159b1add2ffd4d10e4ba2b7519709c326d53b3c`  
		Last Modified: Tue, 31 Mar 2020 20:54:28 GMT  
		Size: 562.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-alpine3.11` - linux; arm variant v7

```console
$ docker pull nats@sha256:9914b699049a64964fdcea31b1777b01b03a195466f4d26f6cb9b21c3f608be1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6497861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05e93c4064d5ecafbd500bc7252d1ecbc4785fc5162e2b6d5c1a1ef29ce76aab`
-	Default Command: `["nats-server"]`

```dockerfile
# Mon, 23 Mar 2020 21:57:55 GMT
ADD file:3bde6b6fd06efbf24e66446c6d32f72294fc749ae9ee6191776242e92b2f8ab4 in / 
# Mon, 23 Mar 2020 21:57:56 GMT
CMD ["/bin/sh"]
# Wed, 01 Apr 2020 06:01:54 GMT
ENV NATS_SERVER=2.1.6
# Wed, 01 Apr 2020 06:01:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 01 Apr 2020 06:01:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 01 Apr 2020 06:02:00 GMT
EXPOSE 4222 6222 8222
# Wed, 01 Apr 2020 06:02:01 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:d9bf605ce3d4449f4b90035c3e21d691806324781d43a5287b1da25a01779d6b`  
		Last Modified: Mon, 23 Mar 2020 21:58:16 GMT  
		Size: 2.4 MB (2420493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23dfc407cfb62fcc989fc550e01b071587084a28b301a1716e2c71112a2b51e`  
		Last Modified: Wed, 01 Apr 2020 06:07:55 GMT  
		Size: 4.1 MB (4076812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75090e66199501633c177682c4bef49fc00b0f80abb29a8abe7e1af6f3cdec8c`  
		Last Modified: Wed, 01 Apr 2020 06:07:54 GMT  
		Size: 556.0 B  
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
$ docker pull nats@sha256:aea7cc2831f9abd383f4174e38b17849df3606beea6648d63b824eb2a8b88dbd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `nats:2.1-nanoserver` - windows version 10.0.17763.1098; amd64

```console
$ docker pull nats@sha256:4ec9c8b5fc9c9f5ea875830d8355ac6e9f93d0e3fe5d374d24a5eb6bdf2608fa
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105092070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7678424b503caf1f5241062780f3e6969a8867e91fa257eff465274911c9568`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 Mar 2020 13:28:48 GMT
RUN Apply image 1809-amd64
# Wed, 11 Mar 2020 14:47:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 31 Mar 2020 21:16:16 GMT
RUN cmd /S /C #(nop) COPY file:5493aca6ccb800df74d7e7b98176527689b02c807794603a1f7dde376217279b in C:\nats-server.exe 
# Tue, 31 Mar 2020 21:16:18 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 31 Mar 2020 21:16:19 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 21:16:20 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 31 Mar 2020 21:16:20 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8e709836e4dce2fa52689be79fedc1e3d040ba47ec2da2fc3b23f33fc6944b50`  
		Size: 101.1 MB (101050245 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:11472ae705112ae5e29e58c937ca3e026bd8eb756b2fcbe538bba856f7d80ff9`  
		Last Modified: Wed, 11 Mar 2020 14:48:32 GMT  
		Size: 938.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e455632008f14f11f8b72d69a1da128950a141735926961bcf2baf8c2ae12c2`  
		Last Modified: Tue, 31 Mar 2020 21:20:05 GMT  
		Size: 4.0 MB (4036943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f44539e2ede61bafd54f622e8042099620ea0dafd8c87cf6043d295f17932f6`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030bd5a2e51cc12afa370bd2ec9b2ba2c6ad83cb09ce43555d0ba3b3eb497b49`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 835.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670e0425975dec676f07849687918818aa9a711883c2e2b6d39f40c1d922b71b`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 862.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ec1ea0b29e208f3799b3561fef99ab4b126884eeea9301d6c55f699847d80d`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 825.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-nanoserver-1809`

```console
$ docker pull nats@sha256:aea7cc2831f9abd383f4174e38b17849df3606beea6648d63b824eb2a8b88dbd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `nats:2.1-nanoserver-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull nats@sha256:4ec9c8b5fc9c9f5ea875830d8355ac6e9f93d0e3fe5d374d24a5eb6bdf2608fa
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105092070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7678424b503caf1f5241062780f3e6969a8867e91fa257eff465274911c9568`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 Mar 2020 13:28:48 GMT
RUN Apply image 1809-amd64
# Wed, 11 Mar 2020 14:47:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 31 Mar 2020 21:16:16 GMT
RUN cmd /S /C #(nop) COPY file:5493aca6ccb800df74d7e7b98176527689b02c807794603a1f7dde376217279b in C:\nats-server.exe 
# Tue, 31 Mar 2020 21:16:18 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 31 Mar 2020 21:16:19 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 21:16:20 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 31 Mar 2020 21:16:20 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8e709836e4dce2fa52689be79fedc1e3d040ba47ec2da2fc3b23f33fc6944b50`  
		Size: 101.1 MB (101050245 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:11472ae705112ae5e29e58c937ca3e026bd8eb756b2fcbe538bba856f7d80ff9`  
		Last Modified: Wed, 11 Mar 2020 14:48:32 GMT  
		Size: 938.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e455632008f14f11f8b72d69a1da128950a141735926961bcf2baf8c2ae12c2`  
		Last Modified: Tue, 31 Mar 2020 21:20:05 GMT  
		Size: 4.0 MB (4036943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f44539e2ede61bafd54f622e8042099620ea0dafd8c87cf6043d295f17932f6`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030bd5a2e51cc12afa370bd2ec9b2ba2c6ad83cb09ce43555d0ba3b3eb497b49`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 835.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670e0425975dec676f07849687918818aa9a711883c2e2b6d39f40c1d922b71b`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 862.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ec1ea0b29e208f3799b3561fef99ab4b126884eeea9301d6c55f699847d80d`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 825.0 B  
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
$ docker pull nats@sha256:0a0363aee1ab915ca6823f0cb8f5064cb561b8bd779b34b2167960a6d8d935d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64
	-	windows version 10.0.14393.3568; amd64

### `nats:2.1-windowsservercore` - windows version 10.0.17763.1098; amd64

```console
$ docker pull nats@sha256:e3a5d10d77bb9a35c8167bc655529206d03c0e7dac2c44f3b9da230c165781b7
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2278709759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:128cc6d6411b3c714e63facea2b4da51b0a7c042c7decc5d5634624f90d3f250`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Tue, 10 Mar 2020 23:23:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Mar 2020 14:45:12 GMT
ENV NATS_DOCKERIZED=1
# Tue, 31 Mar 2020 21:14:33 GMT
ENV NATS_SERVER=2.1.6
# Tue, 31 Mar 2020 21:14:34 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Tue, 31 Mar 2020 21:15:02 GMT
RUN Set-PSDebug -Trace 2
# Tue, 31 Mar 2020 21:16:01 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Tue, 31 Mar 2020 21:16:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 31 Mar 2020 21:16:03 GMT
EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 21:16:04 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 31 Mar 2020 21:16:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb49f89affc2d69b541463d095fdfbe61fa62e02b0aa5fa6d26bc134fb66bf35`  
		Last Modified: Wed, 11 Mar 2020 00:30:48 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ed96bfcc8cc17c8c1192c9f852f19ab1a2bcea7fa094f5e3f417f29b731f1e`  
		Last Modified: Wed, 11 Mar 2020 14:48:09 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18957d3bf61a5f19ebc5847b6ca77f7a7863643e54b7101511766974bad6b69`  
		Last Modified: Tue, 31 Mar 2020 21:19:48 GMT  
		Size: 1.1 KB (1096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b302c84191e1df029de15f2967d9a7b53246786fb26544da226b8c607925ff`  
		Last Modified: Tue, 31 Mar 2020 21:19:47 GMT  
		Size: 1.1 KB (1088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93836f3c0cffa6b0a37b955c3dce4dafe0642ab66960be80b1d74d406edf25c`  
		Last Modified: Tue, 31 Mar 2020 21:19:48 GMT  
		Size: 4.7 MB (4681616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ffbfa8e12b45b0c4d7bff5269d1ff7699720245d9e2037149c0477cd7c1a0e6`  
		Last Modified: Tue, 31 Mar 2020 21:19:46 GMT  
		Size: 8.7 MB (8682323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bea1418e16fcf97cee4031be619e7e26ef941739136dd28cd3f04451f9f132a`  
		Last Modified: Tue, 31 Mar 2020 21:19:44 GMT  
		Size: 1.6 KB (1628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941e7ca764c534845927416d06df263615a01f5f7e2a9aee1385322b761f6fc7`  
		Last Modified: Tue, 31 Mar 2020 21:19:45 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014dd1ff508af5046533914bacdc75ddaa7efdd00cc1327c448272dc08014353`  
		Last Modified: Tue, 31 Mar 2020 21:19:45 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e25f9b92198997df236a1495f0fc7bf389f99880eb61de4877d2e67ca58431a`  
		Last Modified: Tue, 31 Mar 2020 21:19:44 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-windowsservercore` - windows version 10.0.14393.3568; amd64

```console
$ docker pull nats@sha256:93e77d94d5181b2e8ca9efbacd8c6ef9401b54c6c318b9dd23b7e5751e1653d1
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 GB (5743587455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28335910c356ede194b2dcd9233b435a9cf6f610dd9c49e62c6bab814e302781`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 10 Mar 2020 08:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 18 Mar 2020 12:27:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 18 Mar 2020 13:38:31 GMT
ENV NATS_DOCKERIZED=1
# Tue, 31 Mar 2020 21:16:26 GMT
ENV NATS_SERVER=2.1.6
# Tue, 31 Mar 2020 21:16:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Tue, 31 Mar 2020 21:17:26 GMT
RUN Set-PSDebug -Trace 2
# Tue, 31 Mar 2020 21:19:04 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Tue, 31 Mar 2020 21:19:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 31 Mar 2020 21:19:07 GMT
EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 21:19:08 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 31 Mar 2020 21:19:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a5d20b7a2294a0d2631f74f49fc34574484a692913559546ef0bceae789fd7a8`  
		Size: 1.7 GB (1658775203 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8cd5aa189dca96a2d4bcc0e2516d85f8a69d277957f44aca08575ecf42e5bc2f`  
		Last Modified: Wed, 18 Mar 2020 13:22:17 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ddde0325982310255792cba68184203cd656b044bf4f46ab5c1ebf779122527`  
		Last Modified: Wed, 18 Mar 2020 13:42:12 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122d2e783014460190d162f128fa5710a117cd9136ff0582c542e645c5f0b10f`  
		Last Modified: Tue, 31 Mar 2020 21:20:23 GMT  
		Size: 1.1 KB (1080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0a23ecd71b35608af4c4e06f1857aab4211c34048dde0a2072401bc8421176`  
		Last Modified: Tue, 31 Mar 2020 21:20:23 GMT  
		Size: 1.1 KB (1088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9948d714ad0c8a48c12fe7b9becc3fabe09f61d4d66bd75cf77d91316713000e`  
		Last Modified: Tue, 31 Mar 2020 21:20:24 GMT  
		Size: 5.4 MB (5384998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f47e480e660c2de16210e4a70aaf550bd0dd240bf43f1766a7049cfe020cf25`  
		Last Modified: Tue, 31 Mar 2020 21:20:30 GMT  
		Size: 9.4 MB (9431821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d276126def9ffa1ac85e80e3ce86f78dc9f815bf1241f060c953972b16fe8459`  
		Last Modified: Tue, 31 Mar 2020 21:20:20 GMT  
		Size: 1.7 KB (1673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6342f41571faf0fe60bbb2d11b642f0a8499c91ee7b7b48806b4851a5ebd95b8`  
		Last Modified: Tue, 31 Mar 2020 21:20:20 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662962efab83cc3a58e4d9c59b9e23abc78f4f8634c5ea2d5b87034063037ec9`  
		Last Modified: Tue, 31 Mar 2020 21:20:20 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a4c33960d69a58662fa5a7dac06bd5ceaa709df8079062bf9f684318c0c1b0`  
		Last Modified: Tue, 31 Mar 2020 21:20:20 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-windowsservercore-1809`

```console
$ docker pull nats@sha256:186133a96780f6a775e4055406f8770a684424433af78e6189512064438e47c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `nats:2.1-windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull nats@sha256:e3a5d10d77bb9a35c8167bc655529206d03c0e7dac2c44f3b9da230c165781b7
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2278709759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:128cc6d6411b3c714e63facea2b4da51b0a7c042c7decc5d5634624f90d3f250`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Tue, 10 Mar 2020 23:23:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Mar 2020 14:45:12 GMT
ENV NATS_DOCKERIZED=1
# Tue, 31 Mar 2020 21:14:33 GMT
ENV NATS_SERVER=2.1.6
# Tue, 31 Mar 2020 21:14:34 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Tue, 31 Mar 2020 21:15:02 GMT
RUN Set-PSDebug -Trace 2
# Tue, 31 Mar 2020 21:16:01 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Tue, 31 Mar 2020 21:16:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 31 Mar 2020 21:16:03 GMT
EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 21:16:04 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 31 Mar 2020 21:16:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb49f89affc2d69b541463d095fdfbe61fa62e02b0aa5fa6d26bc134fb66bf35`  
		Last Modified: Wed, 11 Mar 2020 00:30:48 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ed96bfcc8cc17c8c1192c9f852f19ab1a2bcea7fa094f5e3f417f29b731f1e`  
		Last Modified: Wed, 11 Mar 2020 14:48:09 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18957d3bf61a5f19ebc5847b6ca77f7a7863643e54b7101511766974bad6b69`  
		Last Modified: Tue, 31 Mar 2020 21:19:48 GMT  
		Size: 1.1 KB (1096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b302c84191e1df029de15f2967d9a7b53246786fb26544da226b8c607925ff`  
		Last Modified: Tue, 31 Mar 2020 21:19:47 GMT  
		Size: 1.1 KB (1088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93836f3c0cffa6b0a37b955c3dce4dafe0642ab66960be80b1d74d406edf25c`  
		Last Modified: Tue, 31 Mar 2020 21:19:48 GMT  
		Size: 4.7 MB (4681616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ffbfa8e12b45b0c4d7bff5269d1ff7699720245d9e2037149c0477cd7c1a0e6`  
		Last Modified: Tue, 31 Mar 2020 21:19:46 GMT  
		Size: 8.7 MB (8682323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bea1418e16fcf97cee4031be619e7e26ef941739136dd28cd3f04451f9f132a`  
		Last Modified: Tue, 31 Mar 2020 21:19:44 GMT  
		Size: 1.6 KB (1628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941e7ca764c534845927416d06df263615a01f5f7e2a9aee1385322b761f6fc7`  
		Last Modified: Tue, 31 Mar 2020 21:19:45 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014dd1ff508af5046533914bacdc75ddaa7efdd00cc1327c448272dc08014353`  
		Last Modified: Tue, 31 Mar 2020 21:19:45 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e25f9b92198997df236a1495f0fc7bf389f99880eb61de4877d2e67ca58431a`  
		Last Modified: Tue, 31 Mar 2020 21:19:44 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:d35b6c4a3418f8ef1ba66c3bcc1a8b938fa440fd3718b2a63b4f66d4d9e2ad1b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3568; amd64

### `nats:2.1-windowsservercore-ltsc2016` - windows version 10.0.14393.3568; amd64

```console
$ docker pull nats@sha256:93e77d94d5181b2e8ca9efbacd8c6ef9401b54c6c318b9dd23b7e5751e1653d1
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 GB (5743587455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28335910c356ede194b2dcd9233b435a9cf6f610dd9c49e62c6bab814e302781`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 10 Mar 2020 08:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 18 Mar 2020 12:27:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 18 Mar 2020 13:38:31 GMT
ENV NATS_DOCKERIZED=1
# Tue, 31 Mar 2020 21:16:26 GMT
ENV NATS_SERVER=2.1.6
# Tue, 31 Mar 2020 21:16:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Tue, 31 Mar 2020 21:17:26 GMT
RUN Set-PSDebug -Trace 2
# Tue, 31 Mar 2020 21:19:04 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Tue, 31 Mar 2020 21:19:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 31 Mar 2020 21:19:07 GMT
EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 21:19:08 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 31 Mar 2020 21:19:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a5d20b7a2294a0d2631f74f49fc34574484a692913559546ef0bceae789fd7a8`  
		Size: 1.7 GB (1658775203 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8cd5aa189dca96a2d4bcc0e2516d85f8a69d277957f44aca08575ecf42e5bc2f`  
		Last Modified: Wed, 18 Mar 2020 13:22:17 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ddde0325982310255792cba68184203cd656b044bf4f46ab5c1ebf779122527`  
		Last Modified: Wed, 18 Mar 2020 13:42:12 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122d2e783014460190d162f128fa5710a117cd9136ff0582c542e645c5f0b10f`  
		Last Modified: Tue, 31 Mar 2020 21:20:23 GMT  
		Size: 1.1 KB (1080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0a23ecd71b35608af4c4e06f1857aab4211c34048dde0a2072401bc8421176`  
		Last Modified: Tue, 31 Mar 2020 21:20:23 GMT  
		Size: 1.1 KB (1088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9948d714ad0c8a48c12fe7b9becc3fabe09f61d4d66bd75cf77d91316713000e`  
		Last Modified: Tue, 31 Mar 2020 21:20:24 GMT  
		Size: 5.4 MB (5384998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f47e480e660c2de16210e4a70aaf550bd0dd240bf43f1766a7049cfe020cf25`  
		Last Modified: Tue, 31 Mar 2020 21:20:30 GMT  
		Size: 9.4 MB (9431821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d276126def9ffa1ac85e80e3ce86f78dc9f815bf1241f060c953972b16fe8459`  
		Last Modified: Tue, 31 Mar 2020 21:20:20 GMT  
		Size: 1.7 KB (1673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6342f41571faf0fe60bbb2d11b642f0a8499c91ee7b7b48806b4851a5ebd95b8`  
		Last Modified: Tue, 31 Mar 2020 21:20:20 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662962efab83cc3a58e4d9c59b9e23abc78f4f8634c5ea2d5b87034063037ec9`  
		Last Modified: Tue, 31 Mar 2020 21:20:20 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a4c33960d69a58662fa5a7dac06bd5ceaa709df8079062bf9f684318c0c1b0`  
		Last Modified: Tue, 31 Mar 2020 21:20:20 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:2187a6653c7c4e78db59e22bd5fbbe25b43b8f3253df398d61751bdb80cb0aa7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:306471c8b6440327201e8078fe735e4e703cfda47e00980a018adfe41a801fb6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7175368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d816644c99a5174a9ac5e95b93b977eed6723785fa06810f538ee1bd625d4239`
-	Default Command: `["nats-server"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Wed, 01 Apr 2020 06:49:16 GMT
ENV NATS_SERVER=2.1.6
# Wed, 01 Apr 2020 06:49:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 01 Apr 2020 06:49:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 01 Apr 2020 06:49:18 GMT
EXPOSE 4222 6222 8222
# Wed, 01 Apr 2020 06:49:18 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ec7c5cccacb89b8af24413a53fdb893b60bc947b226d2c7e2735016efd0e8f`  
		Last Modified: Wed, 01 Apr 2020 06:49:41 GMT  
		Size: 4.4 MB (4371583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80c118a8e6ccf42f7aa4e34428dc07dcbd2d8d7cff7eb910e0067bfd7f38ada`  
		Last Modified: Wed, 01 Apr 2020 06:49:40 GMT  
		Size: 530.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:bce00d9d88bc4c6fba21488335026e3102f66ee55daa353311345e5c807b2458
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6702865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b23480fa7be718a41b7727b4ddc07dde9ddd114da9d7d54e8072b2c408844458`
-	Default Command: `["nats-server"]`

```dockerfile
# Mon, 23 Mar 2020 21:49:26 GMT
ADD file:e2fdfc637b534345942caf4097883508a5ed23be97d85ccc3357b8277aaa5430 in / 
# Mon, 23 Mar 2020 21:49:27 GMT
CMD ["/bin/sh"]
# Tue, 31 Mar 2020 20:49:36 GMT
ENV NATS_SERVER=2.1.6
# Tue, 31 Mar 2020 20:49:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 31 Mar 2020 20:49:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 31 Mar 2020 20:49:52 GMT
EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 20:49:53 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:0776aeec3430c5a5ba3f43937f0ee6a7770a1fe81a318c9d94cc76512e5375e9`  
		Last Modified: Mon, 23 Mar 2020 21:49:50 GMT  
		Size: 2.6 MB (2618579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1de55532fc814c4a862e789c611472b72868c4fd20d806e8062eaafe58dd641`  
		Last Modified: Tue, 31 Mar 2020 20:54:29 GMT  
		Size: 4.1 MB (4083724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f6c7842c241e086a908b5ff2159b1add2ffd4d10e4ba2b7519709c326d53b3c`  
		Last Modified: Tue, 31 Mar 2020 20:54:28 GMT  
		Size: 562.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:9914b699049a64964fdcea31b1777b01b03a195466f4d26f6cb9b21c3f608be1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6497861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05e93c4064d5ecafbd500bc7252d1ecbc4785fc5162e2b6d5c1a1ef29ce76aab`
-	Default Command: `["nats-server"]`

```dockerfile
# Mon, 23 Mar 2020 21:57:55 GMT
ADD file:3bde6b6fd06efbf24e66446c6d32f72294fc749ae9ee6191776242e92b2f8ab4 in / 
# Mon, 23 Mar 2020 21:57:56 GMT
CMD ["/bin/sh"]
# Wed, 01 Apr 2020 06:01:54 GMT
ENV NATS_SERVER=2.1.6
# Wed, 01 Apr 2020 06:01:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 01 Apr 2020 06:01:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 01 Apr 2020 06:02:00 GMT
EXPOSE 4222 6222 8222
# Wed, 01 Apr 2020 06:02:01 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:d9bf605ce3d4449f4b90035c3e21d691806324781d43a5287b1da25a01779d6b`  
		Last Modified: Mon, 23 Mar 2020 21:58:16 GMT  
		Size: 2.4 MB (2420493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23dfc407cfb62fcc989fc550e01b071587084a28b301a1716e2c71112a2b51e`  
		Last Modified: Wed, 01 Apr 2020 06:07:55 GMT  
		Size: 4.1 MB (4076812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75090e66199501633c177682c4bef49fc00b0f80abb29a8abe7e1af6f3cdec8c`  
		Last Modified: Wed, 01 Apr 2020 06:07:54 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.11`

```console
$ docker pull nats@sha256:2187a6653c7c4e78db59e22bd5fbbe25b43b8f3253df398d61751bdb80cb0aa7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats:2-alpine3.11` - linux; amd64

```console
$ docker pull nats@sha256:306471c8b6440327201e8078fe735e4e703cfda47e00980a018adfe41a801fb6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7175368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d816644c99a5174a9ac5e95b93b977eed6723785fa06810f538ee1bd625d4239`
-	Default Command: `["nats-server"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Wed, 01 Apr 2020 06:49:16 GMT
ENV NATS_SERVER=2.1.6
# Wed, 01 Apr 2020 06:49:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 01 Apr 2020 06:49:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 01 Apr 2020 06:49:18 GMT
EXPOSE 4222 6222 8222
# Wed, 01 Apr 2020 06:49:18 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ec7c5cccacb89b8af24413a53fdb893b60bc947b226d2c7e2735016efd0e8f`  
		Last Modified: Wed, 01 Apr 2020 06:49:41 GMT  
		Size: 4.4 MB (4371583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80c118a8e6ccf42f7aa4e34428dc07dcbd2d8d7cff7eb910e0067bfd7f38ada`  
		Last Modified: Wed, 01 Apr 2020 06:49:40 GMT  
		Size: 530.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.11` - linux; arm variant v6

```console
$ docker pull nats@sha256:bce00d9d88bc4c6fba21488335026e3102f66ee55daa353311345e5c807b2458
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6702865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b23480fa7be718a41b7727b4ddc07dde9ddd114da9d7d54e8072b2c408844458`
-	Default Command: `["nats-server"]`

```dockerfile
# Mon, 23 Mar 2020 21:49:26 GMT
ADD file:e2fdfc637b534345942caf4097883508a5ed23be97d85ccc3357b8277aaa5430 in / 
# Mon, 23 Mar 2020 21:49:27 GMT
CMD ["/bin/sh"]
# Tue, 31 Mar 2020 20:49:36 GMT
ENV NATS_SERVER=2.1.6
# Tue, 31 Mar 2020 20:49:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 31 Mar 2020 20:49:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 31 Mar 2020 20:49:52 GMT
EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 20:49:53 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:0776aeec3430c5a5ba3f43937f0ee6a7770a1fe81a318c9d94cc76512e5375e9`  
		Last Modified: Mon, 23 Mar 2020 21:49:50 GMT  
		Size: 2.6 MB (2618579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1de55532fc814c4a862e789c611472b72868c4fd20d806e8062eaafe58dd641`  
		Last Modified: Tue, 31 Mar 2020 20:54:29 GMT  
		Size: 4.1 MB (4083724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f6c7842c241e086a908b5ff2159b1add2ffd4d10e4ba2b7519709c326d53b3c`  
		Last Modified: Tue, 31 Mar 2020 20:54:28 GMT  
		Size: 562.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.11` - linux; arm variant v7

```console
$ docker pull nats@sha256:9914b699049a64964fdcea31b1777b01b03a195466f4d26f6cb9b21c3f608be1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6497861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05e93c4064d5ecafbd500bc7252d1ecbc4785fc5162e2b6d5c1a1ef29ce76aab`
-	Default Command: `["nats-server"]`

```dockerfile
# Mon, 23 Mar 2020 21:57:55 GMT
ADD file:3bde6b6fd06efbf24e66446c6d32f72294fc749ae9ee6191776242e92b2f8ab4 in / 
# Mon, 23 Mar 2020 21:57:56 GMT
CMD ["/bin/sh"]
# Wed, 01 Apr 2020 06:01:54 GMT
ENV NATS_SERVER=2.1.6
# Wed, 01 Apr 2020 06:01:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 01 Apr 2020 06:01:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 01 Apr 2020 06:02:00 GMT
EXPOSE 4222 6222 8222
# Wed, 01 Apr 2020 06:02:01 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:d9bf605ce3d4449f4b90035c3e21d691806324781d43a5287b1da25a01779d6b`  
		Last Modified: Mon, 23 Mar 2020 21:58:16 GMT  
		Size: 2.4 MB (2420493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23dfc407cfb62fcc989fc550e01b071587084a28b301a1716e2c71112a2b51e`  
		Last Modified: Wed, 01 Apr 2020 06:07:55 GMT  
		Size: 4.1 MB (4076812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75090e66199501633c177682c4bef49fc00b0f80abb29a8abe7e1af6f3cdec8c`  
		Last Modified: Wed, 01 Apr 2020 06:07:54 GMT  
		Size: 556.0 B  
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
$ docker pull nats@sha256:aea7cc2831f9abd383f4174e38b17849df3606beea6648d63b824eb2a8b88dbd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.1098; amd64

```console
$ docker pull nats@sha256:4ec9c8b5fc9c9f5ea875830d8355ac6e9f93d0e3fe5d374d24a5eb6bdf2608fa
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105092070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7678424b503caf1f5241062780f3e6969a8867e91fa257eff465274911c9568`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 Mar 2020 13:28:48 GMT
RUN Apply image 1809-amd64
# Wed, 11 Mar 2020 14:47:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 31 Mar 2020 21:16:16 GMT
RUN cmd /S /C #(nop) COPY file:5493aca6ccb800df74d7e7b98176527689b02c807794603a1f7dde376217279b in C:\nats-server.exe 
# Tue, 31 Mar 2020 21:16:18 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 31 Mar 2020 21:16:19 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 21:16:20 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 31 Mar 2020 21:16:20 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8e709836e4dce2fa52689be79fedc1e3d040ba47ec2da2fc3b23f33fc6944b50`  
		Size: 101.1 MB (101050245 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:11472ae705112ae5e29e58c937ca3e026bd8eb756b2fcbe538bba856f7d80ff9`  
		Last Modified: Wed, 11 Mar 2020 14:48:32 GMT  
		Size: 938.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e455632008f14f11f8b72d69a1da128950a141735926961bcf2baf8c2ae12c2`  
		Last Modified: Tue, 31 Mar 2020 21:20:05 GMT  
		Size: 4.0 MB (4036943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f44539e2ede61bafd54f622e8042099620ea0dafd8c87cf6043d295f17932f6`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030bd5a2e51cc12afa370bd2ec9b2ba2c6ad83cb09ce43555d0ba3b3eb497b49`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 835.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670e0425975dec676f07849687918818aa9a711883c2e2b6d39f40c1d922b71b`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 862.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ec1ea0b29e208f3799b3561fef99ab4b126884eeea9301d6c55f699847d80d`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 825.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:aea7cc2831f9abd383f4174e38b17849df3606beea6648d63b824eb2a8b88dbd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull nats@sha256:4ec9c8b5fc9c9f5ea875830d8355ac6e9f93d0e3fe5d374d24a5eb6bdf2608fa
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105092070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7678424b503caf1f5241062780f3e6969a8867e91fa257eff465274911c9568`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 Mar 2020 13:28:48 GMT
RUN Apply image 1809-amd64
# Wed, 11 Mar 2020 14:47:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 31 Mar 2020 21:16:16 GMT
RUN cmd /S /C #(nop) COPY file:5493aca6ccb800df74d7e7b98176527689b02c807794603a1f7dde376217279b in C:\nats-server.exe 
# Tue, 31 Mar 2020 21:16:18 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 31 Mar 2020 21:16:19 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 21:16:20 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 31 Mar 2020 21:16:20 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8e709836e4dce2fa52689be79fedc1e3d040ba47ec2da2fc3b23f33fc6944b50`  
		Size: 101.1 MB (101050245 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:11472ae705112ae5e29e58c937ca3e026bd8eb756b2fcbe538bba856f7d80ff9`  
		Last Modified: Wed, 11 Mar 2020 14:48:32 GMT  
		Size: 938.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e455632008f14f11f8b72d69a1da128950a141735926961bcf2baf8c2ae12c2`  
		Last Modified: Tue, 31 Mar 2020 21:20:05 GMT  
		Size: 4.0 MB (4036943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f44539e2ede61bafd54f622e8042099620ea0dafd8c87cf6043d295f17932f6`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030bd5a2e51cc12afa370bd2ec9b2ba2c6ad83cb09ce43555d0ba3b3eb497b49`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 835.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670e0425975dec676f07849687918818aa9a711883c2e2b6d39f40c1d922b71b`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 862.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ec1ea0b29e208f3799b3561fef99ab4b126884eeea9301d6c55f699847d80d`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 825.0 B  
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
$ docker pull nats@sha256:0a0363aee1ab915ca6823f0cb8f5064cb561b8bd779b34b2167960a6d8d935d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64
	-	windows version 10.0.14393.3568; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.1098; amd64

```console
$ docker pull nats@sha256:e3a5d10d77bb9a35c8167bc655529206d03c0e7dac2c44f3b9da230c165781b7
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2278709759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:128cc6d6411b3c714e63facea2b4da51b0a7c042c7decc5d5634624f90d3f250`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Tue, 10 Mar 2020 23:23:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Mar 2020 14:45:12 GMT
ENV NATS_DOCKERIZED=1
# Tue, 31 Mar 2020 21:14:33 GMT
ENV NATS_SERVER=2.1.6
# Tue, 31 Mar 2020 21:14:34 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Tue, 31 Mar 2020 21:15:02 GMT
RUN Set-PSDebug -Trace 2
# Tue, 31 Mar 2020 21:16:01 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Tue, 31 Mar 2020 21:16:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 31 Mar 2020 21:16:03 GMT
EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 21:16:04 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 31 Mar 2020 21:16:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb49f89affc2d69b541463d095fdfbe61fa62e02b0aa5fa6d26bc134fb66bf35`  
		Last Modified: Wed, 11 Mar 2020 00:30:48 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ed96bfcc8cc17c8c1192c9f852f19ab1a2bcea7fa094f5e3f417f29b731f1e`  
		Last Modified: Wed, 11 Mar 2020 14:48:09 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18957d3bf61a5f19ebc5847b6ca77f7a7863643e54b7101511766974bad6b69`  
		Last Modified: Tue, 31 Mar 2020 21:19:48 GMT  
		Size: 1.1 KB (1096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b302c84191e1df029de15f2967d9a7b53246786fb26544da226b8c607925ff`  
		Last Modified: Tue, 31 Mar 2020 21:19:47 GMT  
		Size: 1.1 KB (1088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93836f3c0cffa6b0a37b955c3dce4dafe0642ab66960be80b1d74d406edf25c`  
		Last Modified: Tue, 31 Mar 2020 21:19:48 GMT  
		Size: 4.7 MB (4681616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ffbfa8e12b45b0c4d7bff5269d1ff7699720245d9e2037149c0477cd7c1a0e6`  
		Last Modified: Tue, 31 Mar 2020 21:19:46 GMT  
		Size: 8.7 MB (8682323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bea1418e16fcf97cee4031be619e7e26ef941739136dd28cd3f04451f9f132a`  
		Last Modified: Tue, 31 Mar 2020 21:19:44 GMT  
		Size: 1.6 KB (1628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941e7ca764c534845927416d06df263615a01f5f7e2a9aee1385322b761f6fc7`  
		Last Modified: Tue, 31 Mar 2020 21:19:45 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014dd1ff508af5046533914bacdc75ddaa7efdd00cc1327c448272dc08014353`  
		Last Modified: Tue, 31 Mar 2020 21:19:45 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e25f9b92198997df236a1495f0fc7bf389f99880eb61de4877d2e67ca58431a`  
		Last Modified: Tue, 31 Mar 2020 21:19:44 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-windowsservercore` - windows version 10.0.14393.3568; amd64

```console
$ docker pull nats@sha256:93e77d94d5181b2e8ca9efbacd8c6ef9401b54c6c318b9dd23b7e5751e1653d1
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 GB (5743587455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28335910c356ede194b2dcd9233b435a9cf6f610dd9c49e62c6bab814e302781`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 10 Mar 2020 08:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 18 Mar 2020 12:27:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 18 Mar 2020 13:38:31 GMT
ENV NATS_DOCKERIZED=1
# Tue, 31 Mar 2020 21:16:26 GMT
ENV NATS_SERVER=2.1.6
# Tue, 31 Mar 2020 21:16:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Tue, 31 Mar 2020 21:17:26 GMT
RUN Set-PSDebug -Trace 2
# Tue, 31 Mar 2020 21:19:04 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Tue, 31 Mar 2020 21:19:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 31 Mar 2020 21:19:07 GMT
EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 21:19:08 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 31 Mar 2020 21:19:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a5d20b7a2294a0d2631f74f49fc34574484a692913559546ef0bceae789fd7a8`  
		Size: 1.7 GB (1658775203 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8cd5aa189dca96a2d4bcc0e2516d85f8a69d277957f44aca08575ecf42e5bc2f`  
		Last Modified: Wed, 18 Mar 2020 13:22:17 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ddde0325982310255792cba68184203cd656b044bf4f46ab5c1ebf779122527`  
		Last Modified: Wed, 18 Mar 2020 13:42:12 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122d2e783014460190d162f128fa5710a117cd9136ff0582c542e645c5f0b10f`  
		Last Modified: Tue, 31 Mar 2020 21:20:23 GMT  
		Size: 1.1 KB (1080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0a23ecd71b35608af4c4e06f1857aab4211c34048dde0a2072401bc8421176`  
		Last Modified: Tue, 31 Mar 2020 21:20:23 GMT  
		Size: 1.1 KB (1088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9948d714ad0c8a48c12fe7b9becc3fabe09f61d4d66bd75cf77d91316713000e`  
		Last Modified: Tue, 31 Mar 2020 21:20:24 GMT  
		Size: 5.4 MB (5384998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f47e480e660c2de16210e4a70aaf550bd0dd240bf43f1766a7049cfe020cf25`  
		Last Modified: Tue, 31 Mar 2020 21:20:30 GMT  
		Size: 9.4 MB (9431821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d276126def9ffa1ac85e80e3ce86f78dc9f815bf1241f060c953972b16fe8459`  
		Last Modified: Tue, 31 Mar 2020 21:20:20 GMT  
		Size: 1.7 KB (1673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6342f41571faf0fe60bbb2d11b642f0a8499c91ee7b7b48806b4851a5ebd95b8`  
		Last Modified: Tue, 31 Mar 2020 21:20:20 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662962efab83cc3a58e4d9c59b9e23abc78f4f8634c5ea2d5b87034063037ec9`  
		Last Modified: Tue, 31 Mar 2020 21:20:20 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a4c33960d69a58662fa5a7dac06bd5ceaa709df8079062bf9f684318c0c1b0`  
		Last Modified: Tue, 31 Mar 2020 21:20:20 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:186133a96780f6a775e4055406f8770a684424433af78e6189512064438e47c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull nats@sha256:e3a5d10d77bb9a35c8167bc655529206d03c0e7dac2c44f3b9da230c165781b7
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2278709759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:128cc6d6411b3c714e63facea2b4da51b0a7c042c7decc5d5634624f90d3f250`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Tue, 10 Mar 2020 23:23:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Mar 2020 14:45:12 GMT
ENV NATS_DOCKERIZED=1
# Tue, 31 Mar 2020 21:14:33 GMT
ENV NATS_SERVER=2.1.6
# Tue, 31 Mar 2020 21:14:34 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Tue, 31 Mar 2020 21:15:02 GMT
RUN Set-PSDebug -Trace 2
# Tue, 31 Mar 2020 21:16:01 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Tue, 31 Mar 2020 21:16:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 31 Mar 2020 21:16:03 GMT
EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 21:16:04 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 31 Mar 2020 21:16:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb49f89affc2d69b541463d095fdfbe61fa62e02b0aa5fa6d26bc134fb66bf35`  
		Last Modified: Wed, 11 Mar 2020 00:30:48 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ed96bfcc8cc17c8c1192c9f852f19ab1a2bcea7fa094f5e3f417f29b731f1e`  
		Last Modified: Wed, 11 Mar 2020 14:48:09 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18957d3bf61a5f19ebc5847b6ca77f7a7863643e54b7101511766974bad6b69`  
		Last Modified: Tue, 31 Mar 2020 21:19:48 GMT  
		Size: 1.1 KB (1096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b302c84191e1df029de15f2967d9a7b53246786fb26544da226b8c607925ff`  
		Last Modified: Tue, 31 Mar 2020 21:19:47 GMT  
		Size: 1.1 KB (1088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93836f3c0cffa6b0a37b955c3dce4dafe0642ab66960be80b1d74d406edf25c`  
		Last Modified: Tue, 31 Mar 2020 21:19:48 GMT  
		Size: 4.7 MB (4681616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ffbfa8e12b45b0c4d7bff5269d1ff7699720245d9e2037149c0477cd7c1a0e6`  
		Last Modified: Tue, 31 Mar 2020 21:19:46 GMT  
		Size: 8.7 MB (8682323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bea1418e16fcf97cee4031be619e7e26ef941739136dd28cd3f04451f9f132a`  
		Last Modified: Tue, 31 Mar 2020 21:19:44 GMT  
		Size: 1.6 KB (1628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941e7ca764c534845927416d06df263615a01f5f7e2a9aee1385322b761f6fc7`  
		Last Modified: Tue, 31 Mar 2020 21:19:45 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014dd1ff508af5046533914bacdc75ddaa7efdd00cc1327c448272dc08014353`  
		Last Modified: Tue, 31 Mar 2020 21:19:45 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e25f9b92198997df236a1495f0fc7bf389f99880eb61de4877d2e67ca58431a`  
		Last Modified: Tue, 31 Mar 2020 21:19:44 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:d35b6c4a3418f8ef1ba66c3bcc1a8b938fa440fd3718b2a63b4f66d4d9e2ad1b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3568; amd64

### `nats:2-windowsservercore-ltsc2016` - windows version 10.0.14393.3568; amd64

```console
$ docker pull nats@sha256:93e77d94d5181b2e8ca9efbacd8c6ef9401b54c6c318b9dd23b7e5751e1653d1
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 GB (5743587455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28335910c356ede194b2dcd9233b435a9cf6f610dd9c49e62c6bab814e302781`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 10 Mar 2020 08:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 18 Mar 2020 12:27:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 18 Mar 2020 13:38:31 GMT
ENV NATS_DOCKERIZED=1
# Tue, 31 Mar 2020 21:16:26 GMT
ENV NATS_SERVER=2.1.6
# Tue, 31 Mar 2020 21:16:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Tue, 31 Mar 2020 21:17:26 GMT
RUN Set-PSDebug -Trace 2
# Tue, 31 Mar 2020 21:19:04 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Tue, 31 Mar 2020 21:19:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 31 Mar 2020 21:19:07 GMT
EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 21:19:08 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 31 Mar 2020 21:19:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a5d20b7a2294a0d2631f74f49fc34574484a692913559546ef0bceae789fd7a8`  
		Size: 1.7 GB (1658775203 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8cd5aa189dca96a2d4bcc0e2516d85f8a69d277957f44aca08575ecf42e5bc2f`  
		Last Modified: Wed, 18 Mar 2020 13:22:17 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ddde0325982310255792cba68184203cd656b044bf4f46ab5c1ebf779122527`  
		Last Modified: Wed, 18 Mar 2020 13:42:12 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122d2e783014460190d162f128fa5710a117cd9136ff0582c542e645c5f0b10f`  
		Last Modified: Tue, 31 Mar 2020 21:20:23 GMT  
		Size: 1.1 KB (1080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0a23ecd71b35608af4c4e06f1857aab4211c34048dde0a2072401bc8421176`  
		Last Modified: Tue, 31 Mar 2020 21:20:23 GMT  
		Size: 1.1 KB (1088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9948d714ad0c8a48c12fe7b9becc3fabe09f61d4d66bd75cf77d91316713000e`  
		Last Modified: Tue, 31 Mar 2020 21:20:24 GMT  
		Size: 5.4 MB (5384998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f47e480e660c2de16210e4a70aaf550bd0dd240bf43f1766a7049cfe020cf25`  
		Last Modified: Tue, 31 Mar 2020 21:20:30 GMT  
		Size: 9.4 MB (9431821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d276126def9ffa1ac85e80e3ce86f78dc9f815bf1241f060c953972b16fe8459`  
		Last Modified: Tue, 31 Mar 2020 21:20:20 GMT  
		Size: 1.7 KB (1673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6342f41571faf0fe60bbb2d11b642f0a8499c91ee7b7b48806b4851a5ebd95b8`  
		Last Modified: Tue, 31 Mar 2020 21:20:20 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662962efab83cc3a58e4d9c59b9e23abc78f4f8634c5ea2d5b87034063037ec9`  
		Last Modified: Tue, 31 Mar 2020 21:20:20 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a4c33960d69a58662fa5a7dac06bd5ceaa709df8079062bf9f684318c0c1b0`  
		Last Modified: Tue, 31 Mar 2020 21:20:20 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:2187a6653c7c4e78db59e22bd5fbbe25b43b8f3253df398d61751bdb80cb0aa7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:306471c8b6440327201e8078fe735e4e703cfda47e00980a018adfe41a801fb6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7175368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d816644c99a5174a9ac5e95b93b977eed6723785fa06810f538ee1bd625d4239`
-	Default Command: `["nats-server"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Wed, 01 Apr 2020 06:49:16 GMT
ENV NATS_SERVER=2.1.6
# Wed, 01 Apr 2020 06:49:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 01 Apr 2020 06:49:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 01 Apr 2020 06:49:18 GMT
EXPOSE 4222 6222 8222
# Wed, 01 Apr 2020 06:49:18 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ec7c5cccacb89b8af24413a53fdb893b60bc947b226d2c7e2735016efd0e8f`  
		Last Modified: Wed, 01 Apr 2020 06:49:41 GMT  
		Size: 4.4 MB (4371583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80c118a8e6ccf42f7aa4e34428dc07dcbd2d8d7cff7eb910e0067bfd7f38ada`  
		Last Modified: Wed, 01 Apr 2020 06:49:40 GMT  
		Size: 530.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:bce00d9d88bc4c6fba21488335026e3102f66ee55daa353311345e5c807b2458
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6702865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b23480fa7be718a41b7727b4ddc07dde9ddd114da9d7d54e8072b2c408844458`
-	Default Command: `["nats-server"]`

```dockerfile
# Mon, 23 Mar 2020 21:49:26 GMT
ADD file:e2fdfc637b534345942caf4097883508a5ed23be97d85ccc3357b8277aaa5430 in / 
# Mon, 23 Mar 2020 21:49:27 GMT
CMD ["/bin/sh"]
# Tue, 31 Mar 2020 20:49:36 GMT
ENV NATS_SERVER=2.1.6
# Tue, 31 Mar 2020 20:49:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 31 Mar 2020 20:49:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 31 Mar 2020 20:49:52 GMT
EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 20:49:53 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:0776aeec3430c5a5ba3f43937f0ee6a7770a1fe81a318c9d94cc76512e5375e9`  
		Last Modified: Mon, 23 Mar 2020 21:49:50 GMT  
		Size: 2.6 MB (2618579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1de55532fc814c4a862e789c611472b72868c4fd20d806e8062eaafe58dd641`  
		Last Modified: Tue, 31 Mar 2020 20:54:29 GMT  
		Size: 4.1 MB (4083724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f6c7842c241e086a908b5ff2159b1add2ffd4d10e4ba2b7519709c326d53b3c`  
		Last Modified: Tue, 31 Mar 2020 20:54:28 GMT  
		Size: 562.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:9914b699049a64964fdcea31b1777b01b03a195466f4d26f6cb9b21c3f608be1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6497861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05e93c4064d5ecafbd500bc7252d1ecbc4785fc5162e2b6d5c1a1ef29ce76aab`
-	Default Command: `["nats-server"]`

```dockerfile
# Mon, 23 Mar 2020 21:57:55 GMT
ADD file:3bde6b6fd06efbf24e66446c6d32f72294fc749ae9ee6191776242e92b2f8ab4 in / 
# Mon, 23 Mar 2020 21:57:56 GMT
CMD ["/bin/sh"]
# Wed, 01 Apr 2020 06:01:54 GMT
ENV NATS_SERVER=2.1.6
# Wed, 01 Apr 2020 06:01:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 01 Apr 2020 06:01:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 01 Apr 2020 06:02:00 GMT
EXPOSE 4222 6222 8222
# Wed, 01 Apr 2020 06:02:01 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:d9bf605ce3d4449f4b90035c3e21d691806324781d43a5287b1da25a01779d6b`  
		Last Modified: Mon, 23 Mar 2020 21:58:16 GMT  
		Size: 2.4 MB (2420493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23dfc407cfb62fcc989fc550e01b071587084a28b301a1716e2c71112a2b51e`  
		Last Modified: Wed, 01 Apr 2020 06:07:55 GMT  
		Size: 4.1 MB (4076812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75090e66199501633c177682c4bef49fc00b0f80abb29a8abe7e1af6f3cdec8c`  
		Last Modified: Wed, 01 Apr 2020 06:07:54 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.11`

```console
$ docker pull nats@sha256:2187a6653c7c4e78db59e22bd5fbbe25b43b8f3253df398d61751bdb80cb0aa7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats:alpine3.11` - linux; amd64

```console
$ docker pull nats@sha256:306471c8b6440327201e8078fe735e4e703cfda47e00980a018adfe41a801fb6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7175368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d816644c99a5174a9ac5e95b93b977eed6723785fa06810f538ee1bd625d4239`
-	Default Command: `["nats-server"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Wed, 01 Apr 2020 06:49:16 GMT
ENV NATS_SERVER=2.1.6
# Wed, 01 Apr 2020 06:49:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 01 Apr 2020 06:49:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 01 Apr 2020 06:49:18 GMT
EXPOSE 4222 6222 8222
# Wed, 01 Apr 2020 06:49:18 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ec7c5cccacb89b8af24413a53fdb893b60bc947b226d2c7e2735016efd0e8f`  
		Last Modified: Wed, 01 Apr 2020 06:49:41 GMT  
		Size: 4.4 MB (4371583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80c118a8e6ccf42f7aa4e34428dc07dcbd2d8d7cff7eb910e0067bfd7f38ada`  
		Last Modified: Wed, 01 Apr 2020 06:49:40 GMT  
		Size: 530.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.11` - linux; arm variant v6

```console
$ docker pull nats@sha256:bce00d9d88bc4c6fba21488335026e3102f66ee55daa353311345e5c807b2458
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6702865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b23480fa7be718a41b7727b4ddc07dde9ddd114da9d7d54e8072b2c408844458`
-	Default Command: `["nats-server"]`

```dockerfile
# Mon, 23 Mar 2020 21:49:26 GMT
ADD file:e2fdfc637b534345942caf4097883508a5ed23be97d85ccc3357b8277aaa5430 in / 
# Mon, 23 Mar 2020 21:49:27 GMT
CMD ["/bin/sh"]
# Tue, 31 Mar 2020 20:49:36 GMT
ENV NATS_SERVER=2.1.6
# Tue, 31 Mar 2020 20:49:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 31 Mar 2020 20:49:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 31 Mar 2020 20:49:52 GMT
EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 20:49:53 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:0776aeec3430c5a5ba3f43937f0ee6a7770a1fe81a318c9d94cc76512e5375e9`  
		Last Modified: Mon, 23 Mar 2020 21:49:50 GMT  
		Size: 2.6 MB (2618579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1de55532fc814c4a862e789c611472b72868c4fd20d806e8062eaafe58dd641`  
		Last Modified: Tue, 31 Mar 2020 20:54:29 GMT  
		Size: 4.1 MB (4083724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f6c7842c241e086a908b5ff2159b1add2ffd4d10e4ba2b7519709c326d53b3c`  
		Last Modified: Tue, 31 Mar 2020 20:54:28 GMT  
		Size: 562.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.11` - linux; arm variant v7

```console
$ docker pull nats@sha256:9914b699049a64964fdcea31b1777b01b03a195466f4d26f6cb9b21c3f608be1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6497861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05e93c4064d5ecafbd500bc7252d1ecbc4785fc5162e2b6d5c1a1ef29ce76aab`
-	Default Command: `["nats-server"]`

```dockerfile
# Mon, 23 Mar 2020 21:57:55 GMT
ADD file:3bde6b6fd06efbf24e66446c6d32f72294fc749ae9ee6191776242e92b2f8ab4 in / 
# Mon, 23 Mar 2020 21:57:56 GMT
CMD ["/bin/sh"]
# Wed, 01 Apr 2020 06:01:54 GMT
ENV NATS_SERVER=2.1.6
# Wed, 01 Apr 2020 06:01:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64' ;; 		armhf) natsArch='arm6' ;; 		armv7) natsArch='arm7' ;; 		x86_64) natsArch='amd64' ;; 		x86) natsArch='386' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 01 Apr 2020 06:01:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 01 Apr 2020 06:02:00 GMT
EXPOSE 4222 6222 8222
# Wed, 01 Apr 2020 06:02:01 GMT
CMD ["nats-server"]
```

-	Layers:
	-	`sha256:d9bf605ce3d4449f4b90035c3e21d691806324781d43a5287b1da25a01779d6b`  
		Last Modified: Mon, 23 Mar 2020 21:58:16 GMT  
		Size: 2.4 MB (2420493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23dfc407cfb62fcc989fc550e01b071587084a28b301a1716e2c71112a2b51e`  
		Last Modified: Wed, 01 Apr 2020 06:07:55 GMT  
		Size: 4.1 MB (4076812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75090e66199501633c177682c4bef49fc00b0f80abb29a8abe7e1af6f3cdec8c`  
		Last Modified: Wed, 01 Apr 2020 06:07:54 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:5f1b3d8c699cdaf8fa11f0a65bb431f5138cb2c56958cace2fd8a7f242367a25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1098; amd64

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

### `nats:latest` - windows version 10.0.17763.1098; amd64

```console
$ docker pull nats@sha256:4ec9c8b5fc9c9f5ea875830d8355ac6e9f93d0e3fe5d374d24a5eb6bdf2608fa
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105092070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7678424b503caf1f5241062780f3e6969a8867e91fa257eff465274911c9568`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 Mar 2020 13:28:48 GMT
RUN Apply image 1809-amd64
# Wed, 11 Mar 2020 14:47:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 31 Mar 2020 21:16:16 GMT
RUN cmd /S /C #(nop) COPY file:5493aca6ccb800df74d7e7b98176527689b02c807794603a1f7dde376217279b in C:\nats-server.exe 
# Tue, 31 Mar 2020 21:16:18 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 31 Mar 2020 21:16:19 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 21:16:20 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 31 Mar 2020 21:16:20 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8e709836e4dce2fa52689be79fedc1e3d040ba47ec2da2fc3b23f33fc6944b50`  
		Size: 101.1 MB (101050245 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:11472ae705112ae5e29e58c937ca3e026bd8eb756b2fcbe538bba856f7d80ff9`  
		Last Modified: Wed, 11 Mar 2020 14:48:32 GMT  
		Size: 938.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e455632008f14f11f8b72d69a1da128950a141735926961bcf2baf8c2ae12c2`  
		Last Modified: Tue, 31 Mar 2020 21:20:05 GMT  
		Size: 4.0 MB (4036943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f44539e2ede61bafd54f622e8042099620ea0dafd8c87cf6043d295f17932f6`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030bd5a2e51cc12afa370bd2ec9b2ba2c6ad83cb09ce43555d0ba3b3eb497b49`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 835.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670e0425975dec676f07849687918818aa9a711883c2e2b6d39f40c1d922b71b`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 862.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ec1ea0b29e208f3799b3561fef99ab4b126884eeea9301d6c55f699847d80d`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 825.0 B  
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
$ docker pull nats@sha256:aea7cc2831f9abd383f4174e38b17849df3606beea6648d63b824eb2a8b88dbd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `nats:nanoserver` - windows version 10.0.17763.1098; amd64

```console
$ docker pull nats@sha256:4ec9c8b5fc9c9f5ea875830d8355ac6e9f93d0e3fe5d374d24a5eb6bdf2608fa
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105092070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7678424b503caf1f5241062780f3e6969a8867e91fa257eff465274911c9568`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 Mar 2020 13:28:48 GMT
RUN Apply image 1809-amd64
# Wed, 11 Mar 2020 14:47:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 31 Mar 2020 21:16:16 GMT
RUN cmd /S /C #(nop) COPY file:5493aca6ccb800df74d7e7b98176527689b02c807794603a1f7dde376217279b in C:\nats-server.exe 
# Tue, 31 Mar 2020 21:16:18 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 31 Mar 2020 21:16:19 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 21:16:20 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 31 Mar 2020 21:16:20 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8e709836e4dce2fa52689be79fedc1e3d040ba47ec2da2fc3b23f33fc6944b50`  
		Size: 101.1 MB (101050245 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:11472ae705112ae5e29e58c937ca3e026bd8eb756b2fcbe538bba856f7d80ff9`  
		Last Modified: Wed, 11 Mar 2020 14:48:32 GMT  
		Size: 938.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e455632008f14f11f8b72d69a1da128950a141735926961bcf2baf8c2ae12c2`  
		Last Modified: Tue, 31 Mar 2020 21:20:05 GMT  
		Size: 4.0 MB (4036943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f44539e2ede61bafd54f622e8042099620ea0dafd8c87cf6043d295f17932f6`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030bd5a2e51cc12afa370bd2ec9b2ba2c6ad83cb09ce43555d0ba3b3eb497b49`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 835.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670e0425975dec676f07849687918818aa9a711883c2e2b6d39f40c1d922b71b`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 862.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ec1ea0b29e208f3799b3561fef99ab4b126884eeea9301d6c55f699847d80d`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 825.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:aea7cc2831f9abd383f4174e38b17849df3606beea6648d63b824eb2a8b88dbd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull nats@sha256:4ec9c8b5fc9c9f5ea875830d8355ac6e9f93d0e3fe5d374d24a5eb6bdf2608fa
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105092070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7678424b503caf1f5241062780f3e6969a8867e91fa257eff465274911c9568`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 Mar 2020 13:28:48 GMT
RUN Apply image 1809-amd64
# Wed, 11 Mar 2020 14:47:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 31 Mar 2020 21:16:16 GMT
RUN cmd /S /C #(nop) COPY file:5493aca6ccb800df74d7e7b98176527689b02c807794603a1f7dde376217279b in C:\nats-server.exe 
# Tue, 31 Mar 2020 21:16:18 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 31 Mar 2020 21:16:19 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 21:16:20 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 31 Mar 2020 21:16:20 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8e709836e4dce2fa52689be79fedc1e3d040ba47ec2da2fc3b23f33fc6944b50`  
		Size: 101.1 MB (101050245 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:11472ae705112ae5e29e58c937ca3e026bd8eb756b2fcbe538bba856f7d80ff9`  
		Last Modified: Wed, 11 Mar 2020 14:48:32 GMT  
		Size: 938.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e455632008f14f11f8b72d69a1da128950a141735926961bcf2baf8c2ae12c2`  
		Last Modified: Tue, 31 Mar 2020 21:20:05 GMT  
		Size: 4.0 MB (4036943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f44539e2ede61bafd54f622e8042099620ea0dafd8c87cf6043d295f17932f6`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030bd5a2e51cc12afa370bd2ec9b2ba2c6ad83cb09ce43555d0ba3b3eb497b49`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 835.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670e0425975dec676f07849687918818aa9a711883c2e2b6d39f40c1d922b71b`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 862.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ec1ea0b29e208f3799b3561fef99ab4b126884eeea9301d6c55f699847d80d`  
		Last Modified: Tue, 31 Mar 2020 21:20:04 GMT  
		Size: 825.0 B  
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
$ docker pull nats@sha256:0a0363aee1ab915ca6823f0cb8f5064cb561b8bd779b34b2167960a6d8d935d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64
	-	windows version 10.0.14393.3568; amd64

### `nats:windowsservercore` - windows version 10.0.17763.1098; amd64

```console
$ docker pull nats@sha256:e3a5d10d77bb9a35c8167bc655529206d03c0e7dac2c44f3b9da230c165781b7
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2278709759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:128cc6d6411b3c714e63facea2b4da51b0a7c042c7decc5d5634624f90d3f250`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Tue, 10 Mar 2020 23:23:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Mar 2020 14:45:12 GMT
ENV NATS_DOCKERIZED=1
# Tue, 31 Mar 2020 21:14:33 GMT
ENV NATS_SERVER=2.1.6
# Tue, 31 Mar 2020 21:14:34 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Tue, 31 Mar 2020 21:15:02 GMT
RUN Set-PSDebug -Trace 2
# Tue, 31 Mar 2020 21:16:01 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Tue, 31 Mar 2020 21:16:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 31 Mar 2020 21:16:03 GMT
EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 21:16:04 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 31 Mar 2020 21:16:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb49f89affc2d69b541463d095fdfbe61fa62e02b0aa5fa6d26bc134fb66bf35`  
		Last Modified: Wed, 11 Mar 2020 00:30:48 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ed96bfcc8cc17c8c1192c9f852f19ab1a2bcea7fa094f5e3f417f29b731f1e`  
		Last Modified: Wed, 11 Mar 2020 14:48:09 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18957d3bf61a5f19ebc5847b6ca77f7a7863643e54b7101511766974bad6b69`  
		Last Modified: Tue, 31 Mar 2020 21:19:48 GMT  
		Size: 1.1 KB (1096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b302c84191e1df029de15f2967d9a7b53246786fb26544da226b8c607925ff`  
		Last Modified: Tue, 31 Mar 2020 21:19:47 GMT  
		Size: 1.1 KB (1088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93836f3c0cffa6b0a37b955c3dce4dafe0642ab66960be80b1d74d406edf25c`  
		Last Modified: Tue, 31 Mar 2020 21:19:48 GMT  
		Size: 4.7 MB (4681616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ffbfa8e12b45b0c4d7bff5269d1ff7699720245d9e2037149c0477cd7c1a0e6`  
		Last Modified: Tue, 31 Mar 2020 21:19:46 GMT  
		Size: 8.7 MB (8682323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bea1418e16fcf97cee4031be619e7e26ef941739136dd28cd3f04451f9f132a`  
		Last Modified: Tue, 31 Mar 2020 21:19:44 GMT  
		Size: 1.6 KB (1628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941e7ca764c534845927416d06df263615a01f5f7e2a9aee1385322b761f6fc7`  
		Last Modified: Tue, 31 Mar 2020 21:19:45 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014dd1ff508af5046533914bacdc75ddaa7efdd00cc1327c448272dc08014353`  
		Last Modified: Tue, 31 Mar 2020 21:19:45 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e25f9b92198997df236a1495f0fc7bf389f99880eb61de4877d2e67ca58431a`  
		Last Modified: Tue, 31 Mar 2020 21:19:44 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:windowsservercore` - windows version 10.0.14393.3568; amd64

```console
$ docker pull nats@sha256:93e77d94d5181b2e8ca9efbacd8c6ef9401b54c6c318b9dd23b7e5751e1653d1
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 GB (5743587455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28335910c356ede194b2dcd9233b435a9cf6f610dd9c49e62c6bab814e302781`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 10 Mar 2020 08:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 18 Mar 2020 12:27:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 18 Mar 2020 13:38:31 GMT
ENV NATS_DOCKERIZED=1
# Tue, 31 Mar 2020 21:16:26 GMT
ENV NATS_SERVER=2.1.6
# Tue, 31 Mar 2020 21:16:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Tue, 31 Mar 2020 21:17:26 GMT
RUN Set-PSDebug -Trace 2
# Tue, 31 Mar 2020 21:19:04 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Tue, 31 Mar 2020 21:19:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 31 Mar 2020 21:19:07 GMT
EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 21:19:08 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 31 Mar 2020 21:19:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a5d20b7a2294a0d2631f74f49fc34574484a692913559546ef0bceae789fd7a8`  
		Size: 1.7 GB (1658775203 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8cd5aa189dca96a2d4bcc0e2516d85f8a69d277957f44aca08575ecf42e5bc2f`  
		Last Modified: Wed, 18 Mar 2020 13:22:17 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ddde0325982310255792cba68184203cd656b044bf4f46ab5c1ebf779122527`  
		Last Modified: Wed, 18 Mar 2020 13:42:12 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122d2e783014460190d162f128fa5710a117cd9136ff0582c542e645c5f0b10f`  
		Last Modified: Tue, 31 Mar 2020 21:20:23 GMT  
		Size: 1.1 KB (1080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0a23ecd71b35608af4c4e06f1857aab4211c34048dde0a2072401bc8421176`  
		Last Modified: Tue, 31 Mar 2020 21:20:23 GMT  
		Size: 1.1 KB (1088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9948d714ad0c8a48c12fe7b9becc3fabe09f61d4d66bd75cf77d91316713000e`  
		Last Modified: Tue, 31 Mar 2020 21:20:24 GMT  
		Size: 5.4 MB (5384998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f47e480e660c2de16210e4a70aaf550bd0dd240bf43f1766a7049cfe020cf25`  
		Last Modified: Tue, 31 Mar 2020 21:20:30 GMT  
		Size: 9.4 MB (9431821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d276126def9ffa1ac85e80e3ce86f78dc9f815bf1241f060c953972b16fe8459`  
		Last Modified: Tue, 31 Mar 2020 21:20:20 GMT  
		Size: 1.7 KB (1673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6342f41571faf0fe60bbb2d11b642f0a8499c91ee7b7b48806b4851a5ebd95b8`  
		Last Modified: Tue, 31 Mar 2020 21:20:20 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662962efab83cc3a58e4d9c59b9e23abc78f4f8634c5ea2d5b87034063037ec9`  
		Last Modified: Tue, 31 Mar 2020 21:20:20 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a4c33960d69a58662fa5a7dac06bd5ceaa709df8079062bf9f684318c0c1b0`  
		Last Modified: Tue, 31 Mar 2020 21:20:20 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:186133a96780f6a775e4055406f8770a684424433af78e6189512064438e47c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull nats@sha256:e3a5d10d77bb9a35c8167bc655529206d03c0e7dac2c44f3b9da230c165781b7
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2278709759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:128cc6d6411b3c714e63facea2b4da51b0a7c042c7decc5d5634624f90d3f250`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Tue, 10 Mar 2020 23:23:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Mar 2020 14:45:12 GMT
ENV NATS_DOCKERIZED=1
# Tue, 31 Mar 2020 21:14:33 GMT
ENV NATS_SERVER=2.1.6
# Tue, 31 Mar 2020 21:14:34 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Tue, 31 Mar 2020 21:15:02 GMT
RUN Set-PSDebug -Trace 2
# Tue, 31 Mar 2020 21:16:01 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Tue, 31 Mar 2020 21:16:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 31 Mar 2020 21:16:03 GMT
EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 21:16:04 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 31 Mar 2020 21:16:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb49f89affc2d69b541463d095fdfbe61fa62e02b0aa5fa6d26bc134fb66bf35`  
		Last Modified: Wed, 11 Mar 2020 00:30:48 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ed96bfcc8cc17c8c1192c9f852f19ab1a2bcea7fa094f5e3f417f29b731f1e`  
		Last Modified: Wed, 11 Mar 2020 14:48:09 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18957d3bf61a5f19ebc5847b6ca77f7a7863643e54b7101511766974bad6b69`  
		Last Modified: Tue, 31 Mar 2020 21:19:48 GMT  
		Size: 1.1 KB (1096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b302c84191e1df029de15f2967d9a7b53246786fb26544da226b8c607925ff`  
		Last Modified: Tue, 31 Mar 2020 21:19:47 GMT  
		Size: 1.1 KB (1088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93836f3c0cffa6b0a37b955c3dce4dafe0642ab66960be80b1d74d406edf25c`  
		Last Modified: Tue, 31 Mar 2020 21:19:48 GMT  
		Size: 4.7 MB (4681616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ffbfa8e12b45b0c4d7bff5269d1ff7699720245d9e2037149c0477cd7c1a0e6`  
		Last Modified: Tue, 31 Mar 2020 21:19:46 GMT  
		Size: 8.7 MB (8682323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bea1418e16fcf97cee4031be619e7e26ef941739136dd28cd3f04451f9f132a`  
		Last Modified: Tue, 31 Mar 2020 21:19:44 GMT  
		Size: 1.6 KB (1628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941e7ca764c534845927416d06df263615a01f5f7e2a9aee1385322b761f6fc7`  
		Last Modified: Tue, 31 Mar 2020 21:19:45 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014dd1ff508af5046533914bacdc75ddaa7efdd00cc1327c448272dc08014353`  
		Last Modified: Tue, 31 Mar 2020 21:19:45 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e25f9b92198997df236a1495f0fc7bf389f99880eb61de4877d2e67ca58431a`  
		Last Modified: Tue, 31 Mar 2020 21:19:44 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:d35b6c4a3418f8ef1ba66c3bcc1a8b938fa440fd3718b2a63b4f66d4d9e2ad1b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3568; amd64

### `nats:windowsservercore-ltsc2016` - windows version 10.0.14393.3568; amd64

```console
$ docker pull nats@sha256:93e77d94d5181b2e8ca9efbacd8c6ef9401b54c6c318b9dd23b7e5751e1653d1
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 GB (5743587455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28335910c356ede194b2dcd9233b435a9cf6f610dd9c49e62c6bab814e302781`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 10 Mar 2020 08:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 18 Mar 2020 12:27:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 18 Mar 2020 13:38:31 GMT
ENV NATS_DOCKERIZED=1
# Tue, 31 Mar 2020 21:16:26 GMT
ENV NATS_SERVER=2.1.6
# Tue, 31 Mar 2020 21:16:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Tue, 31 Mar 2020 21:17:26 GMT
RUN Set-PSDebug -Trace 2
# Tue, 31 Mar 2020 21:19:04 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Tue, 31 Mar 2020 21:19:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 31 Mar 2020 21:19:07 GMT
EXPOSE 4222 6222 8222
# Tue, 31 Mar 2020 21:19:08 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 31 Mar 2020 21:19:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a5d20b7a2294a0d2631f74f49fc34574484a692913559546ef0bceae789fd7a8`  
		Size: 1.7 GB (1658775203 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8cd5aa189dca96a2d4bcc0e2516d85f8a69d277957f44aca08575ecf42e5bc2f`  
		Last Modified: Wed, 18 Mar 2020 13:22:17 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ddde0325982310255792cba68184203cd656b044bf4f46ab5c1ebf779122527`  
		Last Modified: Wed, 18 Mar 2020 13:42:12 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122d2e783014460190d162f128fa5710a117cd9136ff0582c542e645c5f0b10f`  
		Last Modified: Tue, 31 Mar 2020 21:20:23 GMT  
		Size: 1.1 KB (1080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0a23ecd71b35608af4c4e06f1857aab4211c34048dde0a2072401bc8421176`  
		Last Modified: Tue, 31 Mar 2020 21:20:23 GMT  
		Size: 1.1 KB (1088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9948d714ad0c8a48c12fe7b9becc3fabe09f61d4d66bd75cf77d91316713000e`  
		Last Modified: Tue, 31 Mar 2020 21:20:24 GMT  
		Size: 5.4 MB (5384998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f47e480e660c2de16210e4a70aaf550bd0dd240bf43f1766a7049cfe020cf25`  
		Last Modified: Tue, 31 Mar 2020 21:20:30 GMT  
		Size: 9.4 MB (9431821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d276126def9ffa1ac85e80e3ce86f78dc9f815bf1241f060c953972b16fe8459`  
		Last Modified: Tue, 31 Mar 2020 21:20:20 GMT  
		Size: 1.7 KB (1673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6342f41571faf0fe60bbb2d11b642f0a8499c91ee7b7b48806b4851a5ebd95b8`  
		Last Modified: Tue, 31 Mar 2020 21:20:20 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662962efab83cc3a58e4d9c59b9e23abc78f4f8634c5ea2d5b87034063037ec9`  
		Last Modified: Tue, 31 Mar 2020 21:20:20 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a4c33960d69a58662fa5a7dac06bd5ceaa709df8079062bf9f684318c0c1b0`  
		Last Modified: Tue, 31 Mar 2020 21:20:20 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
