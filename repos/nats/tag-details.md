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
$ docker pull nats@sha256:022bb370083b17b579e53e2c30dc5573208279f5c03e088b42b7a2772274b158
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1158; amd64

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

### `nats:2` - windows version 10.0.17763.1158; amd64

```console
$ docker pull nats@sha256:7dca5cee5eb32035a486918a236b30e3bea310bd7342581b617341b9212d2509
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105160447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99847c9a35be50764de72371edfa89a333d08801404be076e5d3fa4f3c7aac45`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 12 Apr 2020 11:41:03 GMT
RUN Apply image 1809-amd64
# Wed, 15 Apr 2020 16:23:57 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Apr 2020 16:23:59 GMT
RUN cmd /S /C #(nop) COPY file:5493aca6ccb800df74d7e7b98176527689b02c807794603a1f7dde376217279b in C:\nats-server.exe 
# Wed, 15 Apr 2020 16:24:01 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Apr 2020 16:24:02 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Apr 2020 16:24:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Apr 2020 16:24:03 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0fe89239909ba300aeb9b977458b61ae3fbbcd2d9591086ed05ca023209d3122`  
		Size: 101.1 MB (101118377 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6151866e219b3e5eea36985660425a906885c867a80977ddaac7bfff310fdb2e`  
		Last Modified: Wed, 15 Apr 2020 16:27:45 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a4afadbc1daaf8812d1f4c3aef50b4e6315fc4aa26df76cca496aa4aeeca59`  
		Last Modified: Wed, 15 Apr 2020 16:27:44 GMT  
		Size: 4.0 MB (4037000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf1b6e541934a816c00f17e8dcf11813554106fd318c355e343b3a3f9e9c5ee`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 1.5 KB (1515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645f0e18a2213f9a2b28caa8c3df00f96e84a5509da51525aff66a98c50e5b73`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353939b19b775f0e0e00c2f2e0f9267aa85d487ddaf4885b9f10ce8bceb072d6`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09828d7c8cf14db261b17ae29f0cb492b08bd98fe36a2b5fc50341e1e56bf14`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1`

```console
$ docker pull nats@sha256:022bb370083b17b579e53e2c30dc5573208279f5c03e088b42b7a2772274b158
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1158; amd64

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

### `nats:2.1` - windows version 10.0.17763.1158; amd64

```console
$ docker pull nats@sha256:7dca5cee5eb32035a486918a236b30e3bea310bd7342581b617341b9212d2509
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105160447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99847c9a35be50764de72371edfa89a333d08801404be076e5d3fa4f3c7aac45`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 12 Apr 2020 11:41:03 GMT
RUN Apply image 1809-amd64
# Wed, 15 Apr 2020 16:23:57 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Apr 2020 16:23:59 GMT
RUN cmd /S /C #(nop) COPY file:5493aca6ccb800df74d7e7b98176527689b02c807794603a1f7dde376217279b in C:\nats-server.exe 
# Wed, 15 Apr 2020 16:24:01 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Apr 2020 16:24:02 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Apr 2020 16:24:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Apr 2020 16:24:03 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0fe89239909ba300aeb9b977458b61ae3fbbcd2d9591086ed05ca023209d3122`  
		Size: 101.1 MB (101118377 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6151866e219b3e5eea36985660425a906885c867a80977ddaac7bfff310fdb2e`  
		Last Modified: Wed, 15 Apr 2020 16:27:45 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a4afadbc1daaf8812d1f4c3aef50b4e6315fc4aa26df76cca496aa4aeeca59`  
		Last Modified: Wed, 15 Apr 2020 16:27:44 GMT  
		Size: 4.0 MB (4037000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf1b6e541934a816c00f17e8dcf11813554106fd318c355e343b3a3f9e9c5ee`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 1.5 KB (1515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645f0e18a2213f9a2b28caa8c3df00f96e84a5509da51525aff66a98c50e5b73`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353939b19b775f0e0e00c2f2e0f9267aa85d487ddaf4885b9f10ce8bceb072d6`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09828d7c8cf14db261b17ae29f0cb492b08bd98fe36a2b5fc50341e1e56bf14`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.6`

```console
$ docker pull nats@sha256:a3b7e6015154a2fa44e72f42dcf88492c10eed5aab0680bc7da89d3c73ff2af3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	windows version 10.0.17763.1158; amd64

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

### `nats:2.1.6` - windows version 10.0.17763.1158; amd64

```console
$ docker pull nats@sha256:7dca5cee5eb32035a486918a236b30e3bea310bd7342581b617341b9212d2509
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105160447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99847c9a35be50764de72371edfa89a333d08801404be076e5d3fa4f3c7aac45`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 12 Apr 2020 11:41:03 GMT
RUN Apply image 1809-amd64
# Wed, 15 Apr 2020 16:23:57 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Apr 2020 16:23:59 GMT
RUN cmd /S /C #(nop) COPY file:5493aca6ccb800df74d7e7b98176527689b02c807794603a1f7dde376217279b in C:\nats-server.exe 
# Wed, 15 Apr 2020 16:24:01 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Apr 2020 16:24:02 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Apr 2020 16:24:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Apr 2020 16:24:03 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0fe89239909ba300aeb9b977458b61ae3fbbcd2d9591086ed05ca023209d3122`  
		Size: 101.1 MB (101118377 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6151866e219b3e5eea36985660425a906885c867a80977ddaac7bfff310fdb2e`  
		Last Modified: Wed, 15 Apr 2020 16:27:45 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a4afadbc1daaf8812d1f4c3aef50b4e6315fc4aa26df76cca496aa4aeeca59`  
		Last Modified: Wed, 15 Apr 2020 16:27:44 GMT  
		Size: 4.0 MB (4037000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf1b6e541934a816c00f17e8dcf11813554106fd318c355e343b3a3f9e9c5ee`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 1.5 KB (1515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645f0e18a2213f9a2b28caa8c3df00f96e84a5509da51525aff66a98c50e5b73`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353939b19b775f0e0e00c2f2e0f9267aa85d487ddaf4885b9f10ce8bceb072d6`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09828d7c8cf14db261b17ae29f0cb492b08bd98fe36a2b5fc50341e1e56bf14`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.6-alpine`

```console
$ docker pull nats@sha256:7190a29a2c038aa156f230a198c2e6d0b025216d9581565ae0712b8ae8c70e47
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
$ docker pull nats@sha256:7190a29a2c038aa156f230a198c2e6d0b025216d9581565ae0712b8ae8c70e47
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
$ docker pull nats@sha256:008984a4d60bddf37f4028fce5f0fc1d4d3daf22ff1cde1fc9e023d3496806d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64

### `nats:2.1.6-nanoserver` - windows version 10.0.17763.1158; amd64

```console
$ docker pull nats@sha256:7dca5cee5eb32035a486918a236b30e3bea310bd7342581b617341b9212d2509
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105160447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99847c9a35be50764de72371edfa89a333d08801404be076e5d3fa4f3c7aac45`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 12 Apr 2020 11:41:03 GMT
RUN Apply image 1809-amd64
# Wed, 15 Apr 2020 16:23:57 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Apr 2020 16:23:59 GMT
RUN cmd /S /C #(nop) COPY file:5493aca6ccb800df74d7e7b98176527689b02c807794603a1f7dde376217279b in C:\nats-server.exe 
# Wed, 15 Apr 2020 16:24:01 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Apr 2020 16:24:02 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Apr 2020 16:24:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Apr 2020 16:24:03 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0fe89239909ba300aeb9b977458b61ae3fbbcd2d9591086ed05ca023209d3122`  
		Size: 101.1 MB (101118377 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6151866e219b3e5eea36985660425a906885c867a80977ddaac7bfff310fdb2e`  
		Last Modified: Wed, 15 Apr 2020 16:27:45 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a4afadbc1daaf8812d1f4c3aef50b4e6315fc4aa26df76cca496aa4aeeca59`  
		Last Modified: Wed, 15 Apr 2020 16:27:44 GMT  
		Size: 4.0 MB (4037000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf1b6e541934a816c00f17e8dcf11813554106fd318c355e343b3a3f9e9c5ee`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 1.5 KB (1515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645f0e18a2213f9a2b28caa8c3df00f96e84a5509da51525aff66a98c50e5b73`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353939b19b775f0e0e00c2f2e0f9267aa85d487ddaf4885b9f10ce8bceb072d6`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09828d7c8cf14db261b17ae29f0cb492b08bd98fe36a2b5fc50341e1e56bf14`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.6-nanoserver-1809`

```console
$ docker pull nats@sha256:008984a4d60bddf37f4028fce5f0fc1d4d3daf22ff1cde1fc9e023d3496806d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64

### `nats:2.1.6-nanoserver-1809` - windows version 10.0.17763.1158; amd64

```console
$ docker pull nats@sha256:7dca5cee5eb32035a486918a236b30e3bea310bd7342581b617341b9212d2509
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105160447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99847c9a35be50764de72371edfa89a333d08801404be076e5d3fa4f3c7aac45`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 12 Apr 2020 11:41:03 GMT
RUN Apply image 1809-amd64
# Wed, 15 Apr 2020 16:23:57 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Apr 2020 16:23:59 GMT
RUN cmd /S /C #(nop) COPY file:5493aca6ccb800df74d7e7b98176527689b02c807794603a1f7dde376217279b in C:\nats-server.exe 
# Wed, 15 Apr 2020 16:24:01 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Apr 2020 16:24:02 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Apr 2020 16:24:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Apr 2020 16:24:03 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0fe89239909ba300aeb9b977458b61ae3fbbcd2d9591086ed05ca023209d3122`  
		Size: 101.1 MB (101118377 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6151866e219b3e5eea36985660425a906885c867a80977ddaac7bfff310fdb2e`  
		Last Modified: Wed, 15 Apr 2020 16:27:45 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a4afadbc1daaf8812d1f4c3aef50b4e6315fc4aa26df76cca496aa4aeeca59`  
		Last Modified: Wed, 15 Apr 2020 16:27:44 GMT  
		Size: 4.0 MB (4037000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf1b6e541934a816c00f17e8dcf11813554106fd318c355e343b3a3f9e9c5ee`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 1.5 KB (1515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645f0e18a2213f9a2b28caa8c3df00f96e84a5509da51525aff66a98c50e5b73`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353939b19b775f0e0e00c2f2e0f9267aa85d487ddaf4885b9f10ce8bceb072d6`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09828d7c8cf14db261b17ae29f0cb492b08bd98fe36a2b5fc50341e1e56bf14`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 884.0 B  
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
$ docker pull nats@sha256:709794fd754e2c5baad0d8b6a200da48fa8139654f73038b74a3c115ebd9a169
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64
	-	windows version 10.0.14393.3630; amd64

### `nats:2.1.6-windowsservercore` - windows version 10.0.17763.1158; amd64

```console
$ docker pull nats@sha256:da6bdbb3e4b18381c6c8bd65e77e65362cb7093aaee4e8e75847d8a99d0408b9
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2284059992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53f78b59d77e6829d438329fa647c002d8909b0c67092c0301d26dfb40b7baea`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Wed, 15 Apr 2020 12:44:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 16:22:01 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Apr 2020 16:22:02 GMT
ENV NATS_SERVER=2.1.6
# Wed, 15 Apr 2020 16:22:02 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Wed, 15 Apr 2020 16:22:34 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Apr 2020 16:23:36 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Apr 2020 16:23:37 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Apr 2020 16:23:38 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Apr 2020 16:23:39 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Apr 2020 16:23:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:442da5a04696895ce6580924a45188bbec9a9db9f81cb7dcef41fc1d4b119130`  
		Last Modified: Wed, 15 Apr 2020 15:29:13 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eabc35632c4e9dfdc3df34c8c1768de1a8aabc637c634f666a062e04e7a01ee`  
		Last Modified: Wed, 15 Apr 2020 16:27:28 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5288564da248aa7179bae08b69418aad39d084799753bb07bfdd1661ad2333`  
		Last Modified: Wed, 15 Apr 2020 16:27:27 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27973c84fc7465c3ceeb48281ce8135848a6dcb336f1273b0137b360f9a131d`  
		Last Modified: Wed, 15 Apr 2020 16:27:28 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950a95d662fcdfc3a25fa648ab13266ba927dfeffbc98d3a1e66834762115c5a`  
		Last Modified: Wed, 15 Apr 2020 16:27:28 GMT  
		Size: 4.7 MB (4669475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4555dfda5583c4fd9be24b85380650589476c60b894b59d99ec6a382713b58`  
		Last Modified: Wed, 15 Apr 2020 16:27:27 GMT  
		Size: 8.7 MB (8673637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3b82a014997f818a346ad784acea3202845bff46f62107b2e463570cecbd50`  
		Last Modified: Wed, 15 Apr 2020 16:27:25 GMT  
		Size: 1.7 KB (1696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe13eafcd76e84ce1b4f08336aaf2c43f14f11b4b8f8a49990f09f577d368d7f`  
		Last Modified: Wed, 15 Apr 2020 16:27:25 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29bc2054912b5068f6e12959261449f157019effdffae5a62f112770ad472350`  
		Last Modified: Wed, 15 Apr 2020 16:27:25 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:983c805853aba21f8626b5cf6797e20a38a6905e59d4302c96116689b260adae`  
		Last Modified: Wed, 15 Apr 2020 16:27:25 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.6-windowsservercore` - windows version 10.0.14393.3630; amd64

```console
$ docker pull nats@sha256:66d7ae5a3047d921cdd982db951c43132b2b9f955f9c94f969a526f379644046
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 GB (5742882659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:362ac08032a58455577b6f347ac3cd8a762b2d2bb2f56014d6b0b017d15d62f6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Apr 2020 12:52:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 16:24:09 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Apr 2020 16:24:10 GMT
ENV NATS_SERVER=2.1.6
# Wed, 15 Apr 2020 16:24:10 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Wed, 15 Apr 2020 16:25:07 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Apr 2020 16:26:48 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Apr 2020 16:26:49 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Apr 2020 16:26:50 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Apr 2020 16:26:51 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Apr 2020 16:26:52 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5171ed01a0687a59b2bdf59e2df29a8932abe0ee22a4a6ff6368f8a8295a97d1`  
		Last Modified: Wed, 15 Apr 2020 15:29:42 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc6613d0d14b27f603772f6d2e32bc83e9cae7a2c5405bb55e04dd2afcc7965`  
		Last Modified: Wed, 15 Apr 2020 16:28:02 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9b2a9b009b5d32772c3e5a1b4266c0345d79830d28510e291416655fb32705`  
		Last Modified: Wed, 15 Apr 2020 16:28:03 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98891503dff691a3d836c03239d6c6855b25d57938484a3a5a25ead310bebaf7`  
		Last Modified: Wed, 15 Apr 2020 16:28:03 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a31b768b5812d2bb57739d75ffd7bc8dad60ce71628ea3af3e9a31f905dacea`  
		Last Modified: Wed, 15 Apr 2020 16:28:08 GMT  
		Size: 5.4 MB (5381044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc99fc11ca890a479faed2238fb44758549834a92a6d69bd4f73fa248fb82f96`  
		Last Modified: Wed, 15 Apr 2020 16:28:02 GMT  
		Size: 9.4 MB (9424463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d664d8f00459b6469eaf80e2b19d667e689b496b0fbd878c5e6b8d61cde564e`  
		Last Modified: Wed, 15 Apr 2020 16:28:00 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c4814c2ae0130e15bab2fa7897d662cc2b737e3171a6e9cdead5280315e51b`  
		Last Modified: Wed, 15 Apr 2020 16:28:00 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:312de9f796b94fcf03a3bb931cbc289d5232b2fa3182ce5a4a3ced2d6833ddb1`  
		Last Modified: Wed, 15 Apr 2020 16:28:00 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827eed70b785fb9807bdc599571dc408e1638b24badf64bb049a0f6a6a963151`  
		Last Modified: Wed, 15 Apr 2020 16:28:00 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.6-windowsservercore-1809`

```console
$ docker pull nats@sha256:3fdcc345a5b762095572d10973239e818bce5fc3fc97dfaab3a206bd9a41f834
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64

### `nats:2.1.6-windowsservercore-1809` - windows version 10.0.17763.1158; amd64

```console
$ docker pull nats@sha256:da6bdbb3e4b18381c6c8bd65e77e65362cb7093aaee4e8e75847d8a99d0408b9
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2284059992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53f78b59d77e6829d438329fa647c002d8909b0c67092c0301d26dfb40b7baea`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Wed, 15 Apr 2020 12:44:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 16:22:01 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Apr 2020 16:22:02 GMT
ENV NATS_SERVER=2.1.6
# Wed, 15 Apr 2020 16:22:02 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Wed, 15 Apr 2020 16:22:34 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Apr 2020 16:23:36 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Apr 2020 16:23:37 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Apr 2020 16:23:38 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Apr 2020 16:23:39 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Apr 2020 16:23:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:442da5a04696895ce6580924a45188bbec9a9db9f81cb7dcef41fc1d4b119130`  
		Last Modified: Wed, 15 Apr 2020 15:29:13 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eabc35632c4e9dfdc3df34c8c1768de1a8aabc637c634f666a062e04e7a01ee`  
		Last Modified: Wed, 15 Apr 2020 16:27:28 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5288564da248aa7179bae08b69418aad39d084799753bb07bfdd1661ad2333`  
		Last Modified: Wed, 15 Apr 2020 16:27:27 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27973c84fc7465c3ceeb48281ce8135848a6dcb336f1273b0137b360f9a131d`  
		Last Modified: Wed, 15 Apr 2020 16:27:28 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950a95d662fcdfc3a25fa648ab13266ba927dfeffbc98d3a1e66834762115c5a`  
		Last Modified: Wed, 15 Apr 2020 16:27:28 GMT  
		Size: 4.7 MB (4669475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4555dfda5583c4fd9be24b85380650589476c60b894b59d99ec6a382713b58`  
		Last Modified: Wed, 15 Apr 2020 16:27:27 GMT  
		Size: 8.7 MB (8673637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3b82a014997f818a346ad784acea3202845bff46f62107b2e463570cecbd50`  
		Last Modified: Wed, 15 Apr 2020 16:27:25 GMT  
		Size: 1.7 KB (1696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe13eafcd76e84ce1b4f08336aaf2c43f14f11b4b8f8a49990f09f577d368d7f`  
		Last Modified: Wed, 15 Apr 2020 16:27:25 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29bc2054912b5068f6e12959261449f157019effdffae5a62f112770ad472350`  
		Last Modified: Wed, 15 Apr 2020 16:27:25 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:983c805853aba21f8626b5cf6797e20a38a6905e59d4302c96116689b260adae`  
		Last Modified: Wed, 15 Apr 2020 16:27:25 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.6-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:2e138f118527bb3eba369cb7e1bd18bc51658a3a0fab001b9955bff4d3e7a482
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3630; amd64

### `nats:2.1.6-windowsservercore-ltsc2016` - windows version 10.0.14393.3630; amd64

```console
$ docker pull nats@sha256:66d7ae5a3047d921cdd982db951c43132b2b9f955f9c94f969a526f379644046
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 GB (5742882659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:362ac08032a58455577b6f347ac3cd8a762b2d2bb2f56014d6b0b017d15d62f6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Apr 2020 12:52:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 16:24:09 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Apr 2020 16:24:10 GMT
ENV NATS_SERVER=2.1.6
# Wed, 15 Apr 2020 16:24:10 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Wed, 15 Apr 2020 16:25:07 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Apr 2020 16:26:48 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Apr 2020 16:26:49 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Apr 2020 16:26:50 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Apr 2020 16:26:51 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Apr 2020 16:26:52 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5171ed01a0687a59b2bdf59e2df29a8932abe0ee22a4a6ff6368f8a8295a97d1`  
		Last Modified: Wed, 15 Apr 2020 15:29:42 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc6613d0d14b27f603772f6d2e32bc83e9cae7a2c5405bb55e04dd2afcc7965`  
		Last Modified: Wed, 15 Apr 2020 16:28:02 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9b2a9b009b5d32772c3e5a1b4266c0345d79830d28510e291416655fb32705`  
		Last Modified: Wed, 15 Apr 2020 16:28:03 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98891503dff691a3d836c03239d6c6855b25d57938484a3a5a25ead310bebaf7`  
		Last Modified: Wed, 15 Apr 2020 16:28:03 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a31b768b5812d2bb57739d75ffd7bc8dad60ce71628ea3af3e9a31f905dacea`  
		Last Modified: Wed, 15 Apr 2020 16:28:08 GMT  
		Size: 5.4 MB (5381044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc99fc11ca890a479faed2238fb44758549834a92a6d69bd4f73fa248fb82f96`  
		Last Modified: Wed, 15 Apr 2020 16:28:02 GMT  
		Size: 9.4 MB (9424463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d664d8f00459b6469eaf80e2b19d667e689b496b0fbd878c5e6b8d61cde564e`  
		Last Modified: Wed, 15 Apr 2020 16:28:00 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c4814c2ae0130e15bab2fa7897d662cc2b737e3171a6e9cdead5280315e51b`  
		Last Modified: Wed, 15 Apr 2020 16:28:00 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:312de9f796b94fcf03a3bb931cbc289d5232b2fa3182ce5a4a3ced2d6833ddb1`  
		Last Modified: Wed, 15 Apr 2020 16:28:00 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827eed70b785fb9807bdc599571dc408e1638b24badf64bb049a0f6a6a963151`  
		Last Modified: Wed, 15 Apr 2020 16:28:00 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-alpine`

```console
$ docker pull nats@sha256:7190a29a2c038aa156f230a198c2e6d0b025216d9581565ae0712b8ae8c70e47
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
$ docker pull nats@sha256:7190a29a2c038aa156f230a198c2e6d0b025216d9581565ae0712b8ae8c70e47
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
$ docker pull nats@sha256:008984a4d60bddf37f4028fce5f0fc1d4d3daf22ff1cde1fc9e023d3496806d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64

### `nats:2.1-nanoserver` - windows version 10.0.17763.1158; amd64

```console
$ docker pull nats@sha256:7dca5cee5eb32035a486918a236b30e3bea310bd7342581b617341b9212d2509
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105160447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99847c9a35be50764de72371edfa89a333d08801404be076e5d3fa4f3c7aac45`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 12 Apr 2020 11:41:03 GMT
RUN Apply image 1809-amd64
# Wed, 15 Apr 2020 16:23:57 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Apr 2020 16:23:59 GMT
RUN cmd /S /C #(nop) COPY file:5493aca6ccb800df74d7e7b98176527689b02c807794603a1f7dde376217279b in C:\nats-server.exe 
# Wed, 15 Apr 2020 16:24:01 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Apr 2020 16:24:02 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Apr 2020 16:24:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Apr 2020 16:24:03 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0fe89239909ba300aeb9b977458b61ae3fbbcd2d9591086ed05ca023209d3122`  
		Size: 101.1 MB (101118377 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6151866e219b3e5eea36985660425a906885c867a80977ddaac7bfff310fdb2e`  
		Last Modified: Wed, 15 Apr 2020 16:27:45 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a4afadbc1daaf8812d1f4c3aef50b4e6315fc4aa26df76cca496aa4aeeca59`  
		Last Modified: Wed, 15 Apr 2020 16:27:44 GMT  
		Size: 4.0 MB (4037000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf1b6e541934a816c00f17e8dcf11813554106fd318c355e343b3a3f9e9c5ee`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 1.5 KB (1515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645f0e18a2213f9a2b28caa8c3df00f96e84a5509da51525aff66a98c50e5b73`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353939b19b775f0e0e00c2f2e0f9267aa85d487ddaf4885b9f10ce8bceb072d6`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09828d7c8cf14db261b17ae29f0cb492b08bd98fe36a2b5fc50341e1e56bf14`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-nanoserver-1809`

```console
$ docker pull nats@sha256:008984a4d60bddf37f4028fce5f0fc1d4d3daf22ff1cde1fc9e023d3496806d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64

### `nats:2.1-nanoserver-1809` - windows version 10.0.17763.1158; amd64

```console
$ docker pull nats@sha256:7dca5cee5eb32035a486918a236b30e3bea310bd7342581b617341b9212d2509
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105160447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99847c9a35be50764de72371edfa89a333d08801404be076e5d3fa4f3c7aac45`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 12 Apr 2020 11:41:03 GMT
RUN Apply image 1809-amd64
# Wed, 15 Apr 2020 16:23:57 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Apr 2020 16:23:59 GMT
RUN cmd /S /C #(nop) COPY file:5493aca6ccb800df74d7e7b98176527689b02c807794603a1f7dde376217279b in C:\nats-server.exe 
# Wed, 15 Apr 2020 16:24:01 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Apr 2020 16:24:02 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Apr 2020 16:24:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Apr 2020 16:24:03 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0fe89239909ba300aeb9b977458b61ae3fbbcd2d9591086ed05ca023209d3122`  
		Size: 101.1 MB (101118377 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6151866e219b3e5eea36985660425a906885c867a80977ddaac7bfff310fdb2e`  
		Last Modified: Wed, 15 Apr 2020 16:27:45 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a4afadbc1daaf8812d1f4c3aef50b4e6315fc4aa26df76cca496aa4aeeca59`  
		Last Modified: Wed, 15 Apr 2020 16:27:44 GMT  
		Size: 4.0 MB (4037000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf1b6e541934a816c00f17e8dcf11813554106fd318c355e343b3a3f9e9c5ee`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 1.5 KB (1515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645f0e18a2213f9a2b28caa8c3df00f96e84a5509da51525aff66a98c50e5b73`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353939b19b775f0e0e00c2f2e0f9267aa85d487ddaf4885b9f10ce8bceb072d6`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09828d7c8cf14db261b17ae29f0cb492b08bd98fe36a2b5fc50341e1e56bf14`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 884.0 B  
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
$ docker pull nats@sha256:709794fd754e2c5baad0d8b6a200da48fa8139654f73038b74a3c115ebd9a169
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64
	-	windows version 10.0.14393.3630; amd64

### `nats:2.1-windowsservercore` - windows version 10.0.17763.1158; amd64

```console
$ docker pull nats@sha256:da6bdbb3e4b18381c6c8bd65e77e65362cb7093aaee4e8e75847d8a99d0408b9
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2284059992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53f78b59d77e6829d438329fa647c002d8909b0c67092c0301d26dfb40b7baea`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Wed, 15 Apr 2020 12:44:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 16:22:01 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Apr 2020 16:22:02 GMT
ENV NATS_SERVER=2.1.6
# Wed, 15 Apr 2020 16:22:02 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Wed, 15 Apr 2020 16:22:34 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Apr 2020 16:23:36 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Apr 2020 16:23:37 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Apr 2020 16:23:38 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Apr 2020 16:23:39 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Apr 2020 16:23:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:442da5a04696895ce6580924a45188bbec9a9db9f81cb7dcef41fc1d4b119130`  
		Last Modified: Wed, 15 Apr 2020 15:29:13 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eabc35632c4e9dfdc3df34c8c1768de1a8aabc637c634f666a062e04e7a01ee`  
		Last Modified: Wed, 15 Apr 2020 16:27:28 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5288564da248aa7179bae08b69418aad39d084799753bb07bfdd1661ad2333`  
		Last Modified: Wed, 15 Apr 2020 16:27:27 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27973c84fc7465c3ceeb48281ce8135848a6dcb336f1273b0137b360f9a131d`  
		Last Modified: Wed, 15 Apr 2020 16:27:28 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950a95d662fcdfc3a25fa648ab13266ba927dfeffbc98d3a1e66834762115c5a`  
		Last Modified: Wed, 15 Apr 2020 16:27:28 GMT  
		Size: 4.7 MB (4669475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4555dfda5583c4fd9be24b85380650589476c60b894b59d99ec6a382713b58`  
		Last Modified: Wed, 15 Apr 2020 16:27:27 GMT  
		Size: 8.7 MB (8673637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3b82a014997f818a346ad784acea3202845bff46f62107b2e463570cecbd50`  
		Last Modified: Wed, 15 Apr 2020 16:27:25 GMT  
		Size: 1.7 KB (1696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe13eafcd76e84ce1b4f08336aaf2c43f14f11b4b8f8a49990f09f577d368d7f`  
		Last Modified: Wed, 15 Apr 2020 16:27:25 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29bc2054912b5068f6e12959261449f157019effdffae5a62f112770ad472350`  
		Last Modified: Wed, 15 Apr 2020 16:27:25 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:983c805853aba21f8626b5cf6797e20a38a6905e59d4302c96116689b260adae`  
		Last Modified: Wed, 15 Apr 2020 16:27:25 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-windowsservercore` - windows version 10.0.14393.3630; amd64

```console
$ docker pull nats@sha256:66d7ae5a3047d921cdd982db951c43132b2b9f955f9c94f969a526f379644046
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 GB (5742882659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:362ac08032a58455577b6f347ac3cd8a762b2d2bb2f56014d6b0b017d15d62f6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Apr 2020 12:52:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 16:24:09 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Apr 2020 16:24:10 GMT
ENV NATS_SERVER=2.1.6
# Wed, 15 Apr 2020 16:24:10 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Wed, 15 Apr 2020 16:25:07 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Apr 2020 16:26:48 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Apr 2020 16:26:49 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Apr 2020 16:26:50 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Apr 2020 16:26:51 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Apr 2020 16:26:52 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5171ed01a0687a59b2bdf59e2df29a8932abe0ee22a4a6ff6368f8a8295a97d1`  
		Last Modified: Wed, 15 Apr 2020 15:29:42 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc6613d0d14b27f603772f6d2e32bc83e9cae7a2c5405bb55e04dd2afcc7965`  
		Last Modified: Wed, 15 Apr 2020 16:28:02 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9b2a9b009b5d32772c3e5a1b4266c0345d79830d28510e291416655fb32705`  
		Last Modified: Wed, 15 Apr 2020 16:28:03 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98891503dff691a3d836c03239d6c6855b25d57938484a3a5a25ead310bebaf7`  
		Last Modified: Wed, 15 Apr 2020 16:28:03 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a31b768b5812d2bb57739d75ffd7bc8dad60ce71628ea3af3e9a31f905dacea`  
		Last Modified: Wed, 15 Apr 2020 16:28:08 GMT  
		Size: 5.4 MB (5381044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc99fc11ca890a479faed2238fb44758549834a92a6d69bd4f73fa248fb82f96`  
		Last Modified: Wed, 15 Apr 2020 16:28:02 GMT  
		Size: 9.4 MB (9424463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d664d8f00459b6469eaf80e2b19d667e689b496b0fbd878c5e6b8d61cde564e`  
		Last Modified: Wed, 15 Apr 2020 16:28:00 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c4814c2ae0130e15bab2fa7897d662cc2b737e3171a6e9cdead5280315e51b`  
		Last Modified: Wed, 15 Apr 2020 16:28:00 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:312de9f796b94fcf03a3bb931cbc289d5232b2fa3182ce5a4a3ced2d6833ddb1`  
		Last Modified: Wed, 15 Apr 2020 16:28:00 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827eed70b785fb9807bdc599571dc408e1638b24badf64bb049a0f6a6a963151`  
		Last Modified: Wed, 15 Apr 2020 16:28:00 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-windowsservercore-1809`

```console
$ docker pull nats@sha256:3fdcc345a5b762095572d10973239e818bce5fc3fc97dfaab3a206bd9a41f834
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64

### `nats:2.1-windowsservercore-1809` - windows version 10.0.17763.1158; amd64

```console
$ docker pull nats@sha256:da6bdbb3e4b18381c6c8bd65e77e65362cb7093aaee4e8e75847d8a99d0408b9
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2284059992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53f78b59d77e6829d438329fa647c002d8909b0c67092c0301d26dfb40b7baea`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Wed, 15 Apr 2020 12:44:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 16:22:01 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Apr 2020 16:22:02 GMT
ENV NATS_SERVER=2.1.6
# Wed, 15 Apr 2020 16:22:02 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Wed, 15 Apr 2020 16:22:34 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Apr 2020 16:23:36 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Apr 2020 16:23:37 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Apr 2020 16:23:38 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Apr 2020 16:23:39 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Apr 2020 16:23:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:442da5a04696895ce6580924a45188bbec9a9db9f81cb7dcef41fc1d4b119130`  
		Last Modified: Wed, 15 Apr 2020 15:29:13 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eabc35632c4e9dfdc3df34c8c1768de1a8aabc637c634f666a062e04e7a01ee`  
		Last Modified: Wed, 15 Apr 2020 16:27:28 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5288564da248aa7179bae08b69418aad39d084799753bb07bfdd1661ad2333`  
		Last Modified: Wed, 15 Apr 2020 16:27:27 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27973c84fc7465c3ceeb48281ce8135848a6dcb336f1273b0137b360f9a131d`  
		Last Modified: Wed, 15 Apr 2020 16:27:28 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950a95d662fcdfc3a25fa648ab13266ba927dfeffbc98d3a1e66834762115c5a`  
		Last Modified: Wed, 15 Apr 2020 16:27:28 GMT  
		Size: 4.7 MB (4669475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4555dfda5583c4fd9be24b85380650589476c60b894b59d99ec6a382713b58`  
		Last Modified: Wed, 15 Apr 2020 16:27:27 GMT  
		Size: 8.7 MB (8673637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3b82a014997f818a346ad784acea3202845bff46f62107b2e463570cecbd50`  
		Last Modified: Wed, 15 Apr 2020 16:27:25 GMT  
		Size: 1.7 KB (1696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe13eafcd76e84ce1b4f08336aaf2c43f14f11b4b8f8a49990f09f577d368d7f`  
		Last Modified: Wed, 15 Apr 2020 16:27:25 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29bc2054912b5068f6e12959261449f157019effdffae5a62f112770ad472350`  
		Last Modified: Wed, 15 Apr 2020 16:27:25 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:983c805853aba21f8626b5cf6797e20a38a6905e59d4302c96116689b260adae`  
		Last Modified: Wed, 15 Apr 2020 16:27:25 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:2e138f118527bb3eba369cb7e1bd18bc51658a3a0fab001b9955bff4d3e7a482
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3630; amd64

### `nats:2.1-windowsservercore-ltsc2016` - windows version 10.0.14393.3630; amd64

```console
$ docker pull nats@sha256:66d7ae5a3047d921cdd982db951c43132b2b9f955f9c94f969a526f379644046
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 GB (5742882659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:362ac08032a58455577b6f347ac3cd8a762b2d2bb2f56014d6b0b017d15d62f6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Apr 2020 12:52:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 16:24:09 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Apr 2020 16:24:10 GMT
ENV NATS_SERVER=2.1.6
# Wed, 15 Apr 2020 16:24:10 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Wed, 15 Apr 2020 16:25:07 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Apr 2020 16:26:48 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Apr 2020 16:26:49 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Apr 2020 16:26:50 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Apr 2020 16:26:51 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Apr 2020 16:26:52 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5171ed01a0687a59b2bdf59e2df29a8932abe0ee22a4a6ff6368f8a8295a97d1`  
		Last Modified: Wed, 15 Apr 2020 15:29:42 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc6613d0d14b27f603772f6d2e32bc83e9cae7a2c5405bb55e04dd2afcc7965`  
		Last Modified: Wed, 15 Apr 2020 16:28:02 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9b2a9b009b5d32772c3e5a1b4266c0345d79830d28510e291416655fb32705`  
		Last Modified: Wed, 15 Apr 2020 16:28:03 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98891503dff691a3d836c03239d6c6855b25d57938484a3a5a25ead310bebaf7`  
		Last Modified: Wed, 15 Apr 2020 16:28:03 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a31b768b5812d2bb57739d75ffd7bc8dad60ce71628ea3af3e9a31f905dacea`  
		Last Modified: Wed, 15 Apr 2020 16:28:08 GMT  
		Size: 5.4 MB (5381044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc99fc11ca890a479faed2238fb44758549834a92a6d69bd4f73fa248fb82f96`  
		Last Modified: Wed, 15 Apr 2020 16:28:02 GMT  
		Size: 9.4 MB (9424463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d664d8f00459b6469eaf80e2b19d667e689b496b0fbd878c5e6b8d61cde564e`  
		Last Modified: Wed, 15 Apr 2020 16:28:00 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c4814c2ae0130e15bab2fa7897d662cc2b737e3171a6e9cdead5280315e51b`  
		Last Modified: Wed, 15 Apr 2020 16:28:00 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:312de9f796b94fcf03a3bb931cbc289d5232b2fa3182ce5a4a3ced2d6833ddb1`  
		Last Modified: Wed, 15 Apr 2020 16:28:00 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827eed70b785fb9807bdc599571dc408e1638b24badf64bb049a0f6a6a963151`  
		Last Modified: Wed, 15 Apr 2020 16:28:00 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:7190a29a2c038aa156f230a198c2e6d0b025216d9581565ae0712b8ae8c70e47
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
$ docker pull nats@sha256:7190a29a2c038aa156f230a198c2e6d0b025216d9581565ae0712b8ae8c70e47
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
$ docker pull nats@sha256:008984a4d60bddf37f4028fce5f0fc1d4d3daf22ff1cde1fc9e023d3496806d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.1158; amd64

```console
$ docker pull nats@sha256:7dca5cee5eb32035a486918a236b30e3bea310bd7342581b617341b9212d2509
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105160447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99847c9a35be50764de72371edfa89a333d08801404be076e5d3fa4f3c7aac45`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 12 Apr 2020 11:41:03 GMT
RUN Apply image 1809-amd64
# Wed, 15 Apr 2020 16:23:57 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Apr 2020 16:23:59 GMT
RUN cmd /S /C #(nop) COPY file:5493aca6ccb800df74d7e7b98176527689b02c807794603a1f7dde376217279b in C:\nats-server.exe 
# Wed, 15 Apr 2020 16:24:01 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Apr 2020 16:24:02 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Apr 2020 16:24:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Apr 2020 16:24:03 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0fe89239909ba300aeb9b977458b61ae3fbbcd2d9591086ed05ca023209d3122`  
		Size: 101.1 MB (101118377 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6151866e219b3e5eea36985660425a906885c867a80977ddaac7bfff310fdb2e`  
		Last Modified: Wed, 15 Apr 2020 16:27:45 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a4afadbc1daaf8812d1f4c3aef50b4e6315fc4aa26df76cca496aa4aeeca59`  
		Last Modified: Wed, 15 Apr 2020 16:27:44 GMT  
		Size: 4.0 MB (4037000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf1b6e541934a816c00f17e8dcf11813554106fd318c355e343b3a3f9e9c5ee`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 1.5 KB (1515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645f0e18a2213f9a2b28caa8c3df00f96e84a5509da51525aff66a98c50e5b73`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353939b19b775f0e0e00c2f2e0f9267aa85d487ddaf4885b9f10ce8bceb072d6`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09828d7c8cf14db261b17ae29f0cb492b08bd98fe36a2b5fc50341e1e56bf14`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:008984a4d60bddf37f4028fce5f0fc1d4d3daf22ff1cde1fc9e023d3496806d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.1158; amd64

```console
$ docker pull nats@sha256:7dca5cee5eb32035a486918a236b30e3bea310bd7342581b617341b9212d2509
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105160447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99847c9a35be50764de72371edfa89a333d08801404be076e5d3fa4f3c7aac45`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 12 Apr 2020 11:41:03 GMT
RUN Apply image 1809-amd64
# Wed, 15 Apr 2020 16:23:57 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Apr 2020 16:23:59 GMT
RUN cmd /S /C #(nop) COPY file:5493aca6ccb800df74d7e7b98176527689b02c807794603a1f7dde376217279b in C:\nats-server.exe 
# Wed, 15 Apr 2020 16:24:01 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Apr 2020 16:24:02 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Apr 2020 16:24:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Apr 2020 16:24:03 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0fe89239909ba300aeb9b977458b61ae3fbbcd2d9591086ed05ca023209d3122`  
		Size: 101.1 MB (101118377 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6151866e219b3e5eea36985660425a906885c867a80977ddaac7bfff310fdb2e`  
		Last Modified: Wed, 15 Apr 2020 16:27:45 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a4afadbc1daaf8812d1f4c3aef50b4e6315fc4aa26df76cca496aa4aeeca59`  
		Last Modified: Wed, 15 Apr 2020 16:27:44 GMT  
		Size: 4.0 MB (4037000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf1b6e541934a816c00f17e8dcf11813554106fd318c355e343b3a3f9e9c5ee`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 1.5 KB (1515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645f0e18a2213f9a2b28caa8c3df00f96e84a5509da51525aff66a98c50e5b73`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353939b19b775f0e0e00c2f2e0f9267aa85d487ddaf4885b9f10ce8bceb072d6`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09828d7c8cf14db261b17ae29f0cb492b08bd98fe36a2b5fc50341e1e56bf14`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 884.0 B  
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
$ docker pull nats@sha256:709794fd754e2c5baad0d8b6a200da48fa8139654f73038b74a3c115ebd9a169
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64
	-	windows version 10.0.14393.3630; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.1158; amd64

```console
$ docker pull nats@sha256:da6bdbb3e4b18381c6c8bd65e77e65362cb7093aaee4e8e75847d8a99d0408b9
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2284059992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53f78b59d77e6829d438329fa647c002d8909b0c67092c0301d26dfb40b7baea`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Wed, 15 Apr 2020 12:44:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 16:22:01 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Apr 2020 16:22:02 GMT
ENV NATS_SERVER=2.1.6
# Wed, 15 Apr 2020 16:22:02 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Wed, 15 Apr 2020 16:22:34 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Apr 2020 16:23:36 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Apr 2020 16:23:37 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Apr 2020 16:23:38 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Apr 2020 16:23:39 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Apr 2020 16:23:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:442da5a04696895ce6580924a45188bbec9a9db9f81cb7dcef41fc1d4b119130`  
		Last Modified: Wed, 15 Apr 2020 15:29:13 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eabc35632c4e9dfdc3df34c8c1768de1a8aabc637c634f666a062e04e7a01ee`  
		Last Modified: Wed, 15 Apr 2020 16:27:28 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5288564da248aa7179bae08b69418aad39d084799753bb07bfdd1661ad2333`  
		Last Modified: Wed, 15 Apr 2020 16:27:27 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27973c84fc7465c3ceeb48281ce8135848a6dcb336f1273b0137b360f9a131d`  
		Last Modified: Wed, 15 Apr 2020 16:27:28 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950a95d662fcdfc3a25fa648ab13266ba927dfeffbc98d3a1e66834762115c5a`  
		Last Modified: Wed, 15 Apr 2020 16:27:28 GMT  
		Size: 4.7 MB (4669475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4555dfda5583c4fd9be24b85380650589476c60b894b59d99ec6a382713b58`  
		Last Modified: Wed, 15 Apr 2020 16:27:27 GMT  
		Size: 8.7 MB (8673637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3b82a014997f818a346ad784acea3202845bff46f62107b2e463570cecbd50`  
		Last Modified: Wed, 15 Apr 2020 16:27:25 GMT  
		Size: 1.7 KB (1696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe13eafcd76e84ce1b4f08336aaf2c43f14f11b4b8f8a49990f09f577d368d7f`  
		Last Modified: Wed, 15 Apr 2020 16:27:25 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29bc2054912b5068f6e12959261449f157019effdffae5a62f112770ad472350`  
		Last Modified: Wed, 15 Apr 2020 16:27:25 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:983c805853aba21f8626b5cf6797e20a38a6905e59d4302c96116689b260adae`  
		Last Modified: Wed, 15 Apr 2020 16:27:25 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-windowsservercore` - windows version 10.0.14393.3630; amd64

```console
$ docker pull nats@sha256:66d7ae5a3047d921cdd982db951c43132b2b9f955f9c94f969a526f379644046
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 GB (5742882659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:362ac08032a58455577b6f347ac3cd8a762b2d2bb2f56014d6b0b017d15d62f6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Apr 2020 12:52:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 16:24:09 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Apr 2020 16:24:10 GMT
ENV NATS_SERVER=2.1.6
# Wed, 15 Apr 2020 16:24:10 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Wed, 15 Apr 2020 16:25:07 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Apr 2020 16:26:48 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Apr 2020 16:26:49 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Apr 2020 16:26:50 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Apr 2020 16:26:51 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Apr 2020 16:26:52 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5171ed01a0687a59b2bdf59e2df29a8932abe0ee22a4a6ff6368f8a8295a97d1`  
		Last Modified: Wed, 15 Apr 2020 15:29:42 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc6613d0d14b27f603772f6d2e32bc83e9cae7a2c5405bb55e04dd2afcc7965`  
		Last Modified: Wed, 15 Apr 2020 16:28:02 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9b2a9b009b5d32772c3e5a1b4266c0345d79830d28510e291416655fb32705`  
		Last Modified: Wed, 15 Apr 2020 16:28:03 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98891503dff691a3d836c03239d6c6855b25d57938484a3a5a25ead310bebaf7`  
		Last Modified: Wed, 15 Apr 2020 16:28:03 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a31b768b5812d2bb57739d75ffd7bc8dad60ce71628ea3af3e9a31f905dacea`  
		Last Modified: Wed, 15 Apr 2020 16:28:08 GMT  
		Size: 5.4 MB (5381044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc99fc11ca890a479faed2238fb44758549834a92a6d69bd4f73fa248fb82f96`  
		Last Modified: Wed, 15 Apr 2020 16:28:02 GMT  
		Size: 9.4 MB (9424463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d664d8f00459b6469eaf80e2b19d667e689b496b0fbd878c5e6b8d61cde564e`  
		Last Modified: Wed, 15 Apr 2020 16:28:00 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c4814c2ae0130e15bab2fa7897d662cc2b737e3171a6e9cdead5280315e51b`  
		Last Modified: Wed, 15 Apr 2020 16:28:00 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:312de9f796b94fcf03a3bb931cbc289d5232b2fa3182ce5a4a3ced2d6833ddb1`  
		Last Modified: Wed, 15 Apr 2020 16:28:00 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827eed70b785fb9807bdc599571dc408e1638b24badf64bb049a0f6a6a963151`  
		Last Modified: Wed, 15 Apr 2020 16:28:00 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:3fdcc345a5b762095572d10973239e818bce5fc3fc97dfaab3a206bd9a41f834
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.1158; amd64

```console
$ docker pull nats@sha256:da6bdbb3e4b18381c6c8bd65e77e65362cb7093aaee4e8e75847d8a99d0408b9
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2284059992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53f78b59d77e6829d438329fa647c002d8909b0c67092c0301d26dfb40b7baea`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Wed, 15 Apr 2020 12:44:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 16:22:01 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Apr 2020 16:22:02 GMT
ENV NATS_SERVER=2.1.6
# Wed, 15 Apr 2020 16:22:02 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Wed, 15 Apr 2020 16:22:34 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Apr 2020 16:23:36 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Apr 2020 16:23:37 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Apr 2020 16:23:38 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Apr 2020 16:23:39 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Apr 2020 16:23:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:442da5a04696895ce6580924a45188bbec9a9db9f81cb7dcef41fc1d4b119130`  
		Last Modified: Wed, 15 Apr 2020 15:29:13 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eabc35632c4e9dfdc3df34c8c1768de1a8aabc637c634f666a062e04e7a01ee`  
		Last Modified: Wed, 15 Apr 2020 16:27:28 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5288564da248aa7179bae08b69418aad39d084799753bb07bfdd1661ad2333`  
		Last Modified: Wed, 15 Apr 2020 16:27:27 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27973c84fc7465c3ceeb48281ce8135848a6dcb336f1273b0137b360f9a131d`  
		Last Modified: Wed, 15 Apr 2020 16:27:28 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950a95d662fcdfc3a25fa648ab13266ba927dfeffbc98d3a1e66834762115c5a`  
		Last Modified: Wed, 15 Apr 2020 16:27:28 GMT  
		Size: 4.7 MB (4669475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4555dfda5583c4fd9be24b85380650589476c60b894b59d99ec6a382713b58`  
		Last Modified: Wed, 15 Apr 2020 16:27:27 GMT  
		Size: 8.7 MB (8673637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3b82a014997f818a346ad784acea3202845bff46f62107b2e463570cecbd50`  
		Last Modified: Wed, 15 Apr 2020 16:27:25 GMT  
		Size: 1.7 KB (1696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe13eafcd76e84ce1b4f08336aaf2c43f14f11b4b8f8a49990f09f577d368d7f`  
		Last Modified: Wed, 15 Apr 2020 16:27:25 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29bc2054912b5068f6e12959261449f157019effdffae5a62f112770ad472350`  
		Last Modified: Wed, 15 Apr 2020 16:27:25 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:983c805853aba21f8626b5cf6797e20a38a6905e59d4302c96116689b260adae`  
		Last Modified: Wed, 15 Apr 2020 16:27:25 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:2e138f118527bb3eba369cb7e1bd18bc51658a3a0fab001b9955bff4d3e7a482
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3630; amd64

### `nats:2-windowsservercore-ltsc2016` - windows version 10.0.14393.3630; amd64

```console
$ docker pull nats@sha256:66d7ae5a3047d921cdd982db951c43132b2b9f955f9c94f969a526f379644046
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 GB (5742882659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:362ac08032a58455577b6f347ac3cd8a762b2d2bb2f56014d6b0b017d15d62f6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Apr 2020 12:52:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 16:24:09 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Apr 2020 16:24:10 GMT
ENV NATS_SERVER=2.1.6
# Wed, 15 Apr 2020 16:24:10 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Wed, 15 Apr 2020 16:25:07 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Apr 2020 16:26:48 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Apr 2020 16:26:49 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Apr 2020 16:26:50 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Apr 2020 16:26:51 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Apr 2020 16:26:52 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5171ed01a0687a59b2bdf59e2df29a8932abe0ee22a4a6ff6368f8a8295a97d1`  
		Last Modified: Wed, 15 Apr 2020 15:29:42 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc6613d0d14b27f603772f6d2e32bc83e9cae7a2c5405bb55e04dd2afcc7965`  
		Last Modified: Wed, 15 Apr 2020 16:28:02 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9b2a9b009b5d32772c3e5a1b4266c0345d79830d28510e291416655fb32705`  
		Last Modified: Wed, 15 Apr 2020 16:28:03 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98891503dff691a3d836c03239d6c6855b25d57938484a3a5a25ead310bebaf7`  
		Last Modified: Wed, 15 Apr 2020 16:28:03 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a31b768b5812d2bb57739d75ffd7bc8dad60ce71628ea3af3e9a31f905dacea`  
		Last Modified: Wed, 15 Apr 2020 16:28:08 GMT  
		Size: 5.4 MB (5381044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc99fc11ca890a479faed2238fb44758549834a92a6d69bd4f73fa248fb82f96`  
		Last Modified: Wed, 15 Apr 2020 16:28:02 GMT  
		Size: 9.4 MB (9424463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d664d8f00459b6469eaf80e2b19d667e689b496b0fbd878c5e6b8d61cde564e`  
		Last Modified: Wed, 15 Apr 2020 16:28:00 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c4814c2ae0130e15bab2fa7897d662cc2b737e3171a6e9cdead5280315e51b`  
		Last Modified: Wed, 15 Apr 2020 16:28:00 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:312de9f796b94fcf03a3bb931cbc289d5232b2fa3182ce5a4a3ced2d6833ddb1`  
		Last Modified: Wed, 15 Apr 2020 16:28:00 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827eed70b785fb9807bdc599571dc408e1638b24badf64bb049a0f6a6a963151`  
		Last Modified: Wed, 15 Apr 2020 16:28:00 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:7190a29a2c038aa156f230a198c2e6d0b025216d9581565ae0712b8ae8c70e47
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
$ docker pull nats@sha256:7190a29a2c038aa156f230a198c2e6d0b025216d9581565ae0712b8ae8c70e47
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
$ docker pull nats@sha256:022bb370083b17b579e53e2c30dc5573208279f5c03e088b42b7a2772274b158
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1158; amd64

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

### `nats:latest` - windows version 10.0.17763.1158; amd64

```console
$ docker pull nats@sha256:7dca5cee5eb32035a486918a236b30e3bea310bd7342581b617341b9212d2509
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105160447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99847c9a35be50764de72371edfa89a333d08801404be076e5d3fa4f3c7aac45`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 12 Apr 2020 11:41:03 GMT
RUN Apply image 1809-amd64
# Wed, 15 Apr 2020 16:23:57 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Apr 2020 16:23:59 GMT
RUN cmd /S /C #(nop) COPY file:5493aca6ccb800df74d7e7b98176527689b02c807794603a1f7dde376217279b in C:\nats-server.exe 
# Wed, 15 Apr 2020 16:24:01 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Apr 2020 16:24:02 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Apr 2020 16:24:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Apr 2020 16:24:03 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0fe89239909ba300aeb9b977458b61ae3fbbcd2d9591086ed05ca023209d3122`  
		Size: 101.1 MB (101118377 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6151866e219b3e5eea36985660425a906885c867a80977ddaac7bfff310fdb2e`  
		Last Modified: Wed, 15 Apr 2020 16:27:45 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a4afadbc1daaf8812d1f4c3aef50b4e6315fc4aa26df76cca496aa4aeeca59`  
		Last Modified: Wed, 15 Apr 2020 16:27:44 GMT  
		Size: 4.0 MB (4037000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf1b6e541934a816c00f17e8dcf11813554106fd318c355e343b3a3f9e9c5ee`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 1.5 KB (1515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645f0e18a2213f9a2b28caa8c3df00f96e84a5509da51525aff66a98c50e5b73`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353939b19b775f0e0e00c2f2e0f9267aa85d487ddaf4885b9f10ce8bceb072d6`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09828d7c8cf14db261b17ae29f0cb492b08bd98fe36a2b5fc50341e1e56bf14`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 884.0 B  
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
$ docker pull nats@sha256:008984a4d60bddf37f4028fce5f0fc1d4d3daf22ff1cde1fc9e023d3496806d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64

### `nats:nanoserver` - windows version 10.0.17763.1158; amd64

```console
$ docker pull nats@sha256:7dca5cee5eb32035a486918a236b30e3bea310bd7342581b617341b9212d2509
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105160447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99847c9a35be50764de72371edfa89a333d08801404be076e5d3fa4f3c7aac45`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 12 Apr 2020 11:41:03 GMT
RUN Apply image 1809-amd64
# Wed, 15 Apr 2020 16:23:57 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Apr 2020 16:23:59 GMT
RUN cmd /S /C #(nop) COPY file:5493aca6ccb800df74d7e7b98176527689b02c807794603a1f7dde376217279b in C:\nats-server.exe 
# Wed, 15 Apr 2020 16:24:01 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Apr 2020 16:24:02 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Apr 2020 16:24:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Apr 2020 16:24:03 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0fe89239909ba300aeb9b977458b61ae3fbbcd2d9591086ed05ca023209d3122`  
		Size: 101.1 MB (101118377 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6151866e219b3e5eea36985660425a906885c867a80977ddaac7bfff310fdb2e`  
		Last Modified: Wed, 15 Apr 2020 16:27:45 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a4afadbc1daaf8812d1f4c3aef50b4e6315fc4aa26df76cca496aa4aeeca59`  
		Last Modified: Wed, 15 Apr 2020 16:27:44 GMT  
		Size: 4.0 MB (4037000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf1b6e541934a816c00f17e8dcf11813554106fd318c355e343b3a3f9e9c5ee`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 1.5 KB (1515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645f0e18a2213f9a2b28caa8c3df00f96e84a5509da51525aff66a98c50e5b73`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353939b19b775f0e0e00c2f2e0f9267aa85d487ddaf4885b9f10ce8bceb072d6`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09828d7c8cf14db261b17ae29f0cb492b08bd98fe36a2b5fc50341e1e56bf14`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:008984a4d60bddf37f4028fce5f0fc1d4d3daf22ff1cde1fc9e023d3496806d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.1158; amd64

```console
$ docker pull nats@sha256:7dca5cee5eb32035a486918a236b30e3bea310bd7342581b617341b9212d2509
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105160447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99847c9a35be50764de72371edfa89a333d08801404be076e5d3fa4f3c7aac45`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 12 Apr 2020 11:41:03 GMT
RUN Apply image 1809-amd64
# Wed, 15 Apr 2020 16:23:57 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Apr 2020 16:23:59 GMT
RUN cmd /S /C #(nop) COPY file:5493aca6ccb800df74d7e7b98176527689b02c807794603a1f7dde376217279b in C:\nats-server.exe 
# Wed, 15 Apr 2020 16:24:01 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Apr 2020 16:24:02 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Apr 2020 16:24:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Apr 2020 16:24:03 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0fe89239909ba300aeb9b977458b61ae3fbbcd2d9591086ed05ca023209d3122`  
		Size: 101.1 MB (101118377 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6151866e219b3e5eea36985660425a906885c867a80977ddaac7bfff310fdb2e`  
		Last Modified: Wed, 15 Apr 2020 16:27:45 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a4afadbc1daaf8812d1f4c3aef50b4e6315fc4aa26df76cca496aa4aeeca59`  
		Last Modified: Wed, 15 Apr 2020 16:27:44 GMT  
		Size: 4.0 MB (4037000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf1b6e541934a816c00f17e8dcf11813554106fd318c355e343b3a3f9e9c5ee`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 1.5 KB (1515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645f0e18a2213f9a2b28caa8c3df00f96e84a5509da51525aff66a98c50e5b73`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353939b19b775f0e0e00c2f2e0f9267aa85d487ddaf4885b9f10ce8bceb072d6`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09828d7c8cf14db261b17ae29f0cb492b08bd98fe36a2b5fc50341e1e56bf14`  
		Last Modified: Wed, 15 Apr 2020 16:27:43 GMT  
		Size: 884.0 B  
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
$ docker pull nats@sha256:709794fd754e2c5baad0d8b6a200da48fa8139654f73038b74a3c115ebd9a169
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64
	-	windows version 10.0.14393.3630; amd64

### `nats:windowsservercore` - windows version 10.0.17763.1158; amd64

```console
$ docker pull nats@sha256:da6bdbb3e4b18381c6c8bd65e77e65362cb7093aaee4e8e75847d8a99d0408b9
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2284059992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53f78b59d77e6829d438329fa647c002d8909b0c67092c0301d26dfb40b7baea`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Wed, 15 Apr 2020 12:44:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 16:22:01 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Apr 2020 16:22:02 GMT
ENV NATS_SERVER=2.1.6
# Wed, 15 Apr 2020 16:22:02 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Wed, 15 Apr 2020 16:22:34 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Apr 2020 16:23:36 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Apr 2020 16:23:37 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Apr 2020 16:23:38 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Apr 2020 16:23:39 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Apr 2020 16:23:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:442da5a04696895ce6580924a45188bbec9a9db9f81cb7dcef41fc1d4b119130`  
		Last Modified: Wed, 15 Apr 2020 15:29:13 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eabc35632c4e9dfdc3df34c8c1768de1a8aabc637c634f666a062e04e7a01ee`  
		Last Modified: Wed, 15 Apr 2020 16:27:28 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5288564da248aa7179bae08b69418aad39d084799753bb07bfdd1661ad2333`  
		Last Modified: Wed, 15 Apr 2020 16:27:27 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27973c84fc7465c3ceeb48281ce8135848a6dcb336f1273b0137b360f9a131d`  
		Last Modified: Wed, 15 Apr 2020 16:27:28 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950a95d662fcdfc3a25fa648ab13266ba927dfeffbc98d3a1e66834762115c5a`  
		Last Modified: Wed, 15 Apr 2020 16:27:28 GMT  
		Size: 4.7 MB (4669475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4555dfda5583c4fd9be24b85380650589476c60b894b59d99ec6a382713b58`  
		Last Modified: Wed, 15 Apr 2020 16:27:27 GMT  
		Size: 8.7 MB (8673637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3b82a014997f818a346ad784acea3202845bff46f62107b2e463570cecbd50`  
		Last Modified: Wed, 15 Apr 2020 16:27:25 GMT  
		Size: 1.7 KB (1696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe13eafcd76e84ce1b4f08336aaf2c43f14f11b4b8f8a49990f09f577d368d7f`  
		Last Modified: Wed, 15 Apr 2020 16:27:25 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29bc2054912b5068f6e12959261449f157019effdffae5a62f112770ad472350`  
		Last Modified: Wed, 15 Apr 2020 16:27:25 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:983c805853aba21f8626b5cf6797e20a38a6905e59d4302c96116689b260adae`  
		Last Modified: Wed, 15 Apr 2020 16:27:25 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:windowsservercore` - windows version 10.0.14393.3630; amd64

```console
$ docker pull nats@sha256:66d7ae5a3047d921cdd982db951c43132b2b9f955f9c94f969a526f379644046
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 GB (5742882659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:362ac08032a58455577b6f347ac3cd8a762b2d2bb2f56014d6b0b017d15d62f6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Apr 2020 12:52:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 16:24:09 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Apr 2020 16:24:10 GMT
ENV NATS_SERVER=2.1.6
# Wed, 15 Apr 2020 16:24:10 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Wed, 15 Apr 2020 16:25:07 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Apr 2020 16:26:48 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Apr 2020 16:26:49 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Apr 2020 16:26:50 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Apr 2020 16:26:51 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Apr 2020 16:26:52 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5171ed01a0687a59b2bdf59e2df29a8932abe0ee22a4a6ff6368f8a8295a97d1`  
		Last Modified: Wed, 15 Apr 2020 15:29:42 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc6613d0d14b27f603772f6d2e32bc83e9cae7a2c5405bb55e04dd2afcc7965`  
		Last Modified: Wed, 15 Apr 2020 16:28:02 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9b2a9b009b5d32772c3e5a1b4266c0345d79830d28510e291416655fb32705`  
		Last Modified: Wed, 15 Apr 2020 16:28:03 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98891503dff691a3d836c03239d6c6855b25d57938484a3a5a25ead310bebaf7`  
		Last Modified: Wed, 15 Apr 2020 16:28:03 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a31b768b5812d2bb57739d75ffd7bc8dad60ce71628ea3af3e9a31f905dacea`  
		Last Modified: Wed, 15 Apr 2020 16:28:08 GMT  
		Size: 5.4 MB (5381044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc99fc11ca890a479faed2238fb44758549834a92a6d69bd4f73fa248fb82f96`  
		Last Modified: Wed, 15 Apr 2020 16:28:02 GMT  
		Size: 9.4 MB (9424463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d664d8f00459b6469eaf80e2b19d667e689b496b0fbd878c5e6b8d61cde564e`  
		Last Modified: Wed, 15 Apr 2020 16:28:00 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c4814c2ae0130e15bab2fa7897d662cc2b737e3171a6e9cdead5280315e51b`  
		Last Modified: Wed, 15 Apr 2020 16:28:00 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:312de9f796b94fcf03a3bb931cbc289d5232b2fa3182ce5a4a3ced2d6833ddb1`  
		Last Modified: Wed, 15 Apr 2020 16:28:00 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827eed70b785fb9807bdc599571dc408e1638b24badf64bb049a0f6a6a963151`  
		Last Modified: Wed, 15 Apr 2020 16:28:00 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:3fdcc345a5b762095572d10973239e818bce5fc3fc97dfaab3a206bd9a41f834
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.1158; amd64

```console
$ docker pull nats@sha256:da6bdbb3e4b18381c6c8bd65e77e65362cb7093aaee4e8e75847d8a99d0408b9
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2284059992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53f78b59d77e6829d438329fa647c002d8909b0c67092c0301d26dfb40b7baea`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Wed, 15 Apr 2020 12:44:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 16:22:01 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Apr 2020 16:22:02 GMT
ENV NATS_SERVER=2.1.6
# Wed, 15 Apr 2020 16:22:02 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Wed, 15 Apr 2020 16:22:34 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Apr 2020 16:23:36 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Apr 2020 16:23:37 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Apr 2020 16:23:38 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Apr 2020 16:23:39 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Apr 2020 16:23:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:442da5a04696895ce6580924a45188bbec9a9db9f81cb7dcef41fc1d4b119130`  
		Last Modified: Wed, 15 Apr 2020 15:29:13 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eabc35632c4e9dfdc3df34c8c1768de1a8aabc637c634f666a062e04e7a01ee`  
		Last Modified: Wed, 15 Apr 2020 16:27:28 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5288564da248aa7179bae08b69418aad39d084799753bb07bfdd1661ad2333`  
		Last Modified: Wed, 15 Apr 2020 16:27:27 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27973c84fc7465c3ceeb48281ce8135848a6dcb336f1273b0137b360f9a131d`  
		Last Modified: Wed, 15 Apr 2020 16:27:28 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950a95d662fcdfc3a25fa648ab13266ba927dfeffbc98d3a1e66834762115c5a`  
		Last Modified: Wed, 15 Apr 2020 16:27:28 GMT  
		Size: 4.7 MB (4669475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4555dfda5583c4fd9be24b85380650589476c60b894b59d99ec6a382713b58`  
		Last Modified: Wed, 15 Apr 2020 16:27:27 GMT  
		Size: 8.7 MB (8673637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3b82a014997f818a346ad784acea3202845bff46f62107b2e463570cecbd50`  
		Last Modified: Wed, 15 Apr 2020 16:27:25 GMT  
		Size: 1.7 KB (1696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe13eafcd76e84ce1b4f08336aaf2c43f14f11b4b8f8a49990f09f577d368d7f`  
		Last Modified: Wed, 15 Apr 2020 16:27:25 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29bc2054912b5068f6e12959261449f157019effdffae5a62f112770ad472350`  
		Last Modified: Wed, 15 Apr 2020 16:27:25 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:983c805853aba21f8626b5cf6797e20a38a6905e59d4302c96116689b260adae`  
		Last Modified: Wed, 15 Apr 2020 16:27:25 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:2e138f118527bb3eba369cb7e1bd18bc51658a3a0fab001b9955bff4d3e7a482
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3630; amd64

### `nats:windowsservercore-ltsc2016` - windows version 10.0.14393.3630; amd64

```console
$ docker pull nats@sha256:66d7ae5a3047d921cdd982db951c43132b2b9f955f9c94f969a526f379644046
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 GB (5742882659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:362ac08032a58455577b6f347ac3cd8a762b2d2bb2f56014d6b0b017d15d62f6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Apr 2020 12:52:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 16:24:09 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Apr 2020 16:24:10 GMT
ENV NATS_SERVER=2.1.6
# Wed, 15 Apr 2020 16:24:10 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.6/nats-server-v2.1.6-windows-amd64.zip
# Wed, 15 Apr 2020 16:25:07 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Apr 2020 16:26:48 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 15 Apr 2020 16:26:49 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 15 Apr 2020 16:26:50 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Apr 2020 16:26:51 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Apr 2020 16:26:52 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5171ed01a0687a59b2bdf59e2df29a8932abe0ee22a4a6ff6368f8a8295a97d1`  
		Last Modified: Wed, 15 Apr 2020 15:29:42 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc6613d0d14b27f603772f6d2e32bc83e9cae7a2c5405bb55e04dd2afcc7965`  
		Last Modified: Wed, 15 Apr 2020 16:28:02 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9b2a9b009b5d32772c3e5a1b4266c0345d79830d28510e291416655fb32705`  
		Last Modified: Wed, 15 Apr 2020 16:28:03 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98891503dff691a3d836c03239d6c6855b25d57938484a3a5a25ead310bebaf7`  
		Last Modified: Wed, 15 Apr 2020 16:28:03 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a31b768b5812d2bb57739d75ffd7bc8dad60ce71628ea3af3e9a31f905dacea`  
		Last Modified: Wed, 15 Apr 2020 16:28:08 GMT  
		Size: 5.4 MB (5381044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc99fc11ca890a479faed2238fb44758549834a92a6d69bd4f73fa248fb82f96`  
		Last Modified: Wed, 15 Apr 2020 16:28:02 GMT  
		Size: 9.4 MB (9424463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d664d8f00459b6469eaf80e2b19d667e689b496b0fbd878c5e6b8d61cde564e`  
		Last Modified: Wed, 15 Apr 2020 16:28:00 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c4814c2ae0130e15bab2fa7897d662cc2b737e3171a6e9cdead5280315e51b`  
		Last Modified: Wed, 15 Apr 2020 16:28:00 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:312de9f796b94fcf03a3bb931cbc289d5232b2fa3182ce5a4a3ced2d6833ddb1`  
		Last Modified: Wed, 15 Apr 2020 16:28:00 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827eed70b785fb9807bdc599571dc408e1638b24badf64bb049a0f6a6a963151`  
		Last Modified: Wed, 15 Apr 2020 16:28:00 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
