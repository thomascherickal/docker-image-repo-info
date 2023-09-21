<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats`

-	[`nats:2`](#nats2)
-	[`nats:2-alpine`](#nats2-alpine)
-	[`nats:2-alpine3.18`](#nats2-alpine318)
-	[`nats:2-linux`](#nats2-linux)
-	[`nats:2-nanoserver`](#nats2-nanoserver)
-	[`nats:2-nanoserver-1809`](#nats2-nanoserver-1809)
-	[`nats:2-scratch`](#nats2-scratch)
-	[`nats:2-windowsservercore`](#nats2-windowsservercore)
-	[`nats:2-windowsservercore-1809`](#nats2-windowsservercore-1809)
-	[`nats:2.10`](#nats210)
-	[`nats:2.10-alpine`](#nats210-alpine)
-	[`nats:2.10-alpine3.18`](#nats210-alpine318)
-	[`nats:2.10-linux`](#nats210-linux)
-	[`nats:2.10-nanoserver`](#nats210-nanoserver)
-	[`nats:2.10-nanoserver-1809`](#nats210-nanoserver-1809)
-	[`nats:2.10-scratch`](#nats210-scratch)
-	[`nats:2.10-windowsservercore`](#nats210-windowsservercore)
-	[`nats:2.10-windowsservercore-1809`](#nats210-windowsservercore-1809)
-	[`nats:2.10.1`](#nats2101)
-	[`nats:2.10.1-alpine`](#nats2101-alpine)
-	[`nats:2.10.1-alpine3.18`](#nats2101-alpine318)
-	[`nats:2.10.1-linux`](#nats2101-linux)
-	[`nats:2.10.1-nanoserver`](#nats2101-nanoserver)
-	[`nats:2.10.1-nanoserver-1809`](#nats2101-nanoserver-1809)
-	[`nats:2.10.1-scratch`](#nats2101-scratch)
-	[`nats:2.10.1-windowsservercore`](#nats2101-windowsservercore)
-	[`nats:2.10.1-windowsservercore-1809`](#nats2101-windowsservercore-1809)
-	[`nats:2.9`](#nats29)
-	[`nats:2.9-alpine`](#nats29-alpine)
-	[`nats:2.9-alpine3.18`](#nats29-alpine318)
-	[`nats:2.9-linux`](#nats29-linux)
-	[`nats:2.9-nanoserver`](#nats29-nanoserver)
-	[`nats:2.9-nanoserver-1809`](#nats29-nanoserver-1809)
-	[`nats:2.9-scratch`](#nats29-scratch)
-	[`nats:2.9-windowsservercore`](#nats29-windowsservercore)
-	[`nats:2.9-windowsservercore-1809`](#nats29-windowsservercore-1809)
-	[`nats:2.9.22`](#nats2922)
-	[`nats:2.9.22-alpine`](#nats2922-alpine)
-	[`nats:2.9.22-alpine3.18`](#nats2922-alpine318)
-	[`nats:2.9.22-linux`](#nats2922-linux)
-	[`nats:2.9.22-nanoserver`](#nats2922-nanoserver)
-	[`nats:2.9.22-nanoserver-1809`](#nats2922-nanoserver-1809)
-	[`nats:2.9.22-scratch`](#nats2922-scratch)
-	[`nats:2.9.22-windowsservercore`](#nats2922-windowsservercore)
-	[`nats:2.9.22-windowsservercore-1809`](#nats2922-windowsservercore-1809)
-	[`nats:alpine`](#natsalpine)
-	[`nats:alpine3.18`](#natsalpine318)
-	[`nats:latest`](#natslatest)
-	[`nats:linux`](#natslinux)
-	[`nats:nanoserver`](#natsnanoserver)
-	[`nats:nanoserver-1809`](#natsnanoserver-1809)
-	[`nats:scratch`](#natsscratch)
-	[`nats:windowsservercore`](#natswindowsservercore)
-	[`nats:windowsservercore-1809`](#natswindowsservercore-1809)

## `nats:2`

```console
$ docker pull nats@sha256:4c435644375188d384b184b05252331e4b7ba29a59eec81ba067e2ccab93a00d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4851; amd64

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:300b8159816cb200b0ddca347e2895e811131e89660b698819d6a04d017b51ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5457759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f5b65974bc0ab52f1a6bd8c018ff5fadadbc976f311db512c19acabce037b94`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 20 Sep 2023 00:49:23 GMT
COPY file:8e2a9a3f381167fcc1a95dc7718c10cb67f58a845a3197193a5273c57e28d08d in /nats-server 
# Wed, 20 Sep 2023 00:49:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 20 Sep 2023 00:49:23 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:49:23 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Sep 2023 00:49:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:949cbe9ff3fb07dc0fbd1c6fb6ba4a1c20304c28d574891f79f5d84e05439ec0`  
		Last Modified: Wed, 20 Sep 2023 00:50:22 GMT  
		Size: 5.5 MB (5457252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49c9fc5d845768deddd7c19342fd407ee4fdc4d110abf53e58444440c552181`  
		Last Modified: Wed, 20 Sep 2023 00:50:21 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:2a08a0c1d913294be585667f17f76f028053f5bf47b9d317e5bc0e409011ed1e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5245282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3517f7b93c37103553431effcb0b5a8262feb87c3649b04249d86012c34a9761`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 20 Sep 2023 00:49:17 GMT
COPY file:acdb0e47969d6e334bcadb9c85dfef3166c764ff4ac55254185a04b1a6e8bbee in /nats-server 
# Wed, 20 Sep 2023 00:49:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 20 Sep 2023 00:49:17 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:49:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Sep 2023 00:49:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aac801db9a2a97942dde4494f98ce2d08c529a3af03ecb92f0b93426bbfd6419`  
		Last Modified: Wed, 06 Sep 2023 23:20:56 GMT  
		Size: 5.2 MB (5244773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1646134cd3aac5e501d3658b95fcfd870fb902c4c9591a801a5b370a5aa574`  
		Last Modified: Wed, 20 Sep 2023 00:50:09 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:cce3ff90a32531db64bb74852140a156326d487dafbf812da2168f78c0e85388
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5178106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:111b8fef881498596233d1f7dda3dc1a4113c72bfe5e1088ded56d10a45d128f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 21 Sep 2023 00:07:58 GMT
COPY file:dbe6aeea160dba3a7bdcaf0c14808f7a7b31899bb87a50ed117996ead07014e6 in /nats-server 
# Thu, 21 Sep 2023 00:07:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 21 Sep 2023 00:07:58 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 00:07:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 21 Sep 2023 00:07:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6837114cbc023e4b8b17b6a951b2e91ab9668a1f3ffe65bec26f4ea44b812845`  
		Last Modified: Thu, 21 Sep 2023 00:08:53 GMT  
		Size: 5.2 MB (5177597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bde9589f631b3debf2ce00b1154c597464aeb530aac8a0016d7bee37f972958`  
		Last Modified: Thu, 21 Sep 2023 00:08:51 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:4f09dbc6c43267500545fe441ec8057908d1b6bab5333c432c5e3d4c7ea0fd58
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4980014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:898dfa8e8c4c3e0c69c7c3aec16c90f1f6db172f3af0e7ff763b3bf8db42ed3c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Sep 2023 23:49:29 GMT
COPY file:51aacaba9769a3f16e0467be1fc8eb86122f6f3496e89e41b61e0038083ae308 in /nats-server 
# Tue, 19 Sep 2023 23:49:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Sep 2023 23:49:29 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Sep 2023 23:49:29 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Sep 2023 23:49:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6a6e165fccf6da77ad3b09408162fc7daaafe266b71dd5da8679594aa110a3a5`  
		Last Modified: Wed, 06 Sep 2023 23:05:32 GMT  
		Size: 5.0 MB (4979506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07c6021b659fa78c25ff92ad1e74c46e34c95c5e691ca45f27ced97ea7ef9e2`  
		Last Modified: Tue, 19 Sep 2023 23:50:15 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:41b2a21a345689e5edc4cb8d24444c46df161e58ca89578e66a66e2e0aee2a47
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5171757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed343d1334d5c6f933acaae9f280c90acde044ea41eb6047dc9126ecd17dbd37`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 20 Sep 2023 00:39:39 GMT
COPY file:1ed1e6185c40930f2dc5e0e072cf3d42764ec8f3c10b2f65c3044c6aaf6d5ac5 in /nats-server 
# Wed, 20 Sep 2023 00:39:39 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 20 Sep 2023 00:39:39 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:39:40 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Sep 2023 00:39:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9af7ee06c60cdf35e2e953e1ad5700cf513329b5f88bb07096c8439fbdd7cfb4`  
		Last Modified: Wed, 20 Sep 2023 00:40:42 GMT  
		Size: 5.2 MB (5171248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5795401da82ad77eec35f59034d9f5ce5ff6af93cc82c2a00277bf954ef32c2`  
		Last Modified: Wed, 20 Sep 2023 00:40:41 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:64211266fe0d926796dae72e7484f5aebbdb77c7e7faa3fab3d01954fe03a82e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4970849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a40010bd31b571ac24ead3a8630fa80ce8609b0352d5dab096c6b72940be90a6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 20 Sep 2023 00:39:32 GMT
COPY file:aae670bb79c659968f632ae3be388af62614010873ced2a439475906dbb769c6 in /nats-server 
# Wed, 20 Sep 2023 00:39:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 20 Sep 2023 00:39:32 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:39:32 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Sep 2023 00:39:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:55b6dbad6639da13368cebb9688e8a5caaee29041e6b5e2e798201dfcf2b67ad`  
		Last Modified: Wed, 06 Sep 2023 22:58:23 GMT  
		Size: 5.0 MB (4970341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969097b6afede4aab7deed51f12918311993aadbe7075d4965c14497831f4a12`  
		Last Modified: Wed, 20 Sep 2023 00:40:29 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:e6aea49e5eb407c078286700c1402c6eda155ae11cdd40f8604194f6f70d0dd2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5029479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d109a8655a05cb22d5529db631b1a167bfae974cfc5d047c1ac261888ecd6e8`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 21 Sep 2023 05:05:18 GMT
COPY file:943544393eb61c235711dc43a87ec667d4491be8bcff70eee560d8276bd01b5b in /nats-server 
# Thu, 21 Sep 2023 05:05:18 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 21 Sep 2023 05:05:18 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 05:05:18 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 21 Sep 2023 05:05:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:85892a63e455fd1561bc50ef513a999a9a22152bbab4f029732ea77658da0b37`  
		Last Modified: Thu, 21 Sep 2023 05:06:05 GMT  
		Size: 5.0 MB (5028971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24d6a1649b69be08c681087d8f2f84e750824c24acb44b6d1be0a9a706bb112`  
		Last Modified: Thu, 21 Sep 2023 05:06:04 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:91e7a991da679db1020b25a760298f6944a9ea917e9ae90f10d1d7de9381fec4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4778849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb1745f4f81f20c728e9276ed07416c88490859cdbed438bdcb68aa051eb586c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Sep 2023 23:42:56 GMT
COPY file:d6eca5c67de65d1a8a30a51ea7318b044949c77108b2fdccc5aa0054c068c196 in /nats-server 
# Tue, 19 Sep 2023 23:42:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Sep 2023 23:42:56 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Sep 2023 23:42:56 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Sep 2023 23:42:56 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:88e5ff7f26ea25c6d2ab092989d9372cb32b3e60880124facfcefd7d3f0b7591`  
		Last Modified: Wed, 06 Sep 2023 22:40:49 GMT  
		Size: 4.8 MB (4778340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2424880e07e944598022ff8713b5897eb59c72af17978f7a3f1afa42dd022088`  
		Last Modified: Tue, 19 Sep 2023 23:43:51 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats@sha256:3ae7b24041d5c7f8bb775c1fd47da96b2891f8c6821bfe25f6bcf95a0eaf6064
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110068360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acf1d87f97e43bca95d8940d4aa3abf65c2c05adb6681005cb66f3f7d8001ffc`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Aug 2023 16:42:02 GMT
RUN Apply image 10.0.17763.4851
# Wed, 13 Sep 2023 05:08:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 21 Sep 2023 00:18:29 GMT
RUN cmd /S /C #(nop) COPY file:2b24d029bdf2310dcf6089c8f58986b6c70babf4fd4d433f329957862df58d77 in C:\nats-server.exe 
# Thu, 21 Sep 2023 00:18:29 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 21 Sep 2023 00:18:30 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 00:18:31 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 21 Sep 2023 00:18:31 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:17ba6b878467260559b72cb6f7e79c829eae67862a09efe87f6dc324f49fc086`  
		Last Modified: Tue, 12 Sep 2023 18:31:40 GMT  
		Size: 104.5 MB (104492504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9930674eb6676a1690e63a275d0da517ab8b8aeab7ccd20591f76f7c69a5`  
		Last Modified: Wed, 13 Sep 2023 05:08:48 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05405503d7afb6019521e5fa013d09e5c8636161e9408ba36c149f4853898e7`  
		Last Modified: Thu, 21 Sep 2023 00:19:36 GMT  
		Size: 5.6 MB (5569390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d1f97d2316001518d35eb0b75ac1888c2fe2da51ce49c16012d2fef9ccf5e0c`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.8 KB (1802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6a311706a8aadd91f05c001d3ffbd3a548f21286d0db22eed44fcd5999100f`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a3c2ef4f82e001ae8c4b096641708c8d404bd43dae8f46f843d21d8bb0fd69`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1a063be69428345c92d570f896ffe0326401a9b501ba554a0c4ebf8dc1f5dd`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:e9f41a4a8c1727e4a3ef9fdbff9cc963bfb88c7d77eaf946b2410e4f080e11c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:effbb639aba0db24ebaf3f42fe6e9201428fab869a9399897afeb797819e0a7d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9482934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7afe0964d1327c57759f61500b32db9d8337946f39bdc8264d0c0d8efef6921`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 20 Sep 2023 00:49:05 GMT
ENV NATS_SERVER=2.10.0
# Wed, 20 Sep 2023 00:49:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='59456ee8d222213c0f713e5b571156ec053db15288ee9035b3a7ad01e226c0bb' ;; 		armhf) natsArch='arm6'; sha256='c12c5cde86dba95fa4b433b58af3b9568893e3c7814fa22feae85eb47a9bb2bd' ;; 		armv7) natsArch='arm7'; sha256='748eb00c8d29c674bb4f98371a1afd8be9fba59336be9ef24d24fff148f1e7a4' ;; 		x86_64) natsArch='amd64'; sha256='76f5798ba3923dbc4f170bbae0055d3267d5c604179b2c644f6e7c79cc970d76' ;; 		x86) natsArch='386'; sha256='7f151267f76948293a5721e642b489e1135aecbeb2399dd23d00b04e6a609191' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 20 Sep 2023 00:49:08 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 20 Sep 2023 00:49:08 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 20 Sep 2023 00:49:08 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:49:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Sep 2023 00:49:08 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b04b7bc39016808990ede8996e6d82c3fd7375999baa7a075ce2b107276bd93`  
		Last Modified: Wed, 20 Sep 2023 00:49:47 GMT  
		Size: 6.1 MB (6080321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d9bfba1e3e94018e331b7feae544bb67022934ad7035d517856062cc8af6a2`  
		Last Modified: Wed, 20 Sep 2023 00:49:46 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a185a2d7152fec18042b0c2aaf92f7d8e6b4227691eb89b8cc180c1360a8cc`  
		Last Modified: Wed, 20 Sep 2023 00:49:46 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:84ff4ec4f07f6daee653039f475687b1fc9d518cfefd072fd7405c66708b2c52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8947432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ce27616fe886ff67930425f652c89bc5831f6566f233496b9f1269488d39bb9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Thu, 21 Sep 2023 00:07:43 GMT
ENV NATS_SERVER=2.10.1
# Thu, 21 Sep 2023 00:07:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='13ab69dd6b35b4e253e97f469b61c4038fb6c1d0de89df6dfc93f75af1728ace' ;; 		armhf) natsArch='arm6'; sha256='ad6da4b3289293624e1e60dd0c719d3f2c9cc768774b9f25e580c236915a906b' ;; 		armv7) natsArch='arm7'; sha256='9a706550622ce44f06e6cc44621c01aa27aa9f5da4347d4295e65e986b5cb907' ;; 		x86_64) natsArch='amd64'; sha256='f058d6195931f28cd14d2ac1b9b6a7ce1d760c66c76ccea72aa6b936f4b8d75c' ;; 		x86) natsArch='386'; sha256='1c1e82380139758a69b5040631890914a9db5234517ef9d82b0173e37b8ca96a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 21 Sep 2023 00:07:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 21 Sep 2023 00:07:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 21 Sep 2023 00:07:47 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 00:07:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Sep 2023 00:07:47 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f1a57b33f182668d91321a4367e03ea36a83b22cbb3512e7bf29a740166ac55`  
		Last Modified: Thu, 21 Sep 2023 00:08:27 GMT  
		Size: 5.8 MB (5801621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab09d7306f8d236dead5b1c5d7dfa7a6b386b8f86d77887da9405d0df4d4fd6`  
		Last Modified: Thu, 21 Sep 2023 00:08:25 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a037b525be2a5e8397e646ce00405c26939139fc529d945879cb727e772171`  
		Last Modified: Thu, 21 Sep 2023 00:08:25 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:793e82e82eb90127e5931e743d8b66fa93ce571aa7c3364b62fe1e8051397a0d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8694026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:029567069923892aa47d7aaf87e9018a5ad9406961686c368c467cef63fede5c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Wed, 20 Sep 2023 00:39:11 GMT
ENV NATS_SERVER=2.10.0
# Wed, 20 Sep 2023 00:39:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='59456ee8d222213c0f713e5b571156ec053db15288ee9035b3a7ad01e226c0bb' ;; 		armhf) natsArch='arm6'; sha256='c12c5cde86dba95fa4b433b58af3b9568893e3c7814fa22feae85eb47a9bb2bd' ;; 		armv7) natsArch='arm7'; sha256='748eb00c8d29c674bb4f98371a1afd8be9fba59336be9ef24d24fff148f1e7a4' ;; 		x86_64) natsArch='amd64'; sha256='76f5798ba3923dbc4f170bbae0055d3267d5c604179b2c644f6e7c79cc970d76' ;; 		x86) natsArch='386'; sha256='7f151267f76948293a5721e642b489e1135aecbeb2399dd23d00b04e6a609191' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 20 Sep 2023 00:39:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 20 Sep 2023 00:39:15 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 20 Sep 2023 00:39:15 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:39:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Sep 2023 00:39:15 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86cf505660fa5f57305b113eef333ce025a6d9136f88356db788061f3125927`  
		Last Modified: Wed, 20 Sep 2023 00:40:06 GMT  
		Size: 5.8 MB (5793543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7c97affb17c5049777a5f4c3748e8415a30d8e3fb1650078b3b33763877672`  
		Last Modified: Wed, 20 Sep 2023 00:40:05 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f28587da4e0140d1ee0d0f5fd63eb28e76cdbcc1cca375f6493d13f8fc404e`  
		Last Modified: Wed, 20 Sep 2023 00:40:05 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:2c90c42e3f08e748f4b37d4c85397f7434f2bc06f70f531348fd75f4981786a8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8984785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7d356a02623c8421e021ef35f15363a21ce68a6f855eeef311061f460fb4099`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Thu, 21 Sep 2023 05:04:42 GMT
ENV NATS_SERVER=2.10.1
# Thu, 21 Sep 2023 05:04:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='13ab69dd6b35b4e253e97f469b61c4038fb6c1d0de89df6dfc93f75af1728ace' ;; 		armhf) natsArch='arm6'; sha256='ad6da4b3289293624e1e60dd0c719d3f2c9cc768774b9f25e580c236915a906b' ;; 		armv7) natsArch='arm7'; sha256='9a706550622ce44f06e6cc44621c01aa27aa9f5da4347d4295e65e986b5cb907' ;; 		x86_64) natsArch='amd64'; sha256='f058d6195931f28cd14d2ac1b9b6a7ce1d760c66c76ccea72aa6b936f4b8d75c' ;; 		x86) natsArch='386'; sha256='1c1e82380139758a69b5040631890914a9db5234517ef9d82b0173e37b8ca96a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 21 Sep 2023 05:04:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 21 Sep 2023 05:04:44 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 21 Sep 2023 05:04:44 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 05:04:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Sep 2023 05:04:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36d636b74934d8449d366cac72e2a2f72e239d7a2b015bb861742b6954415a1`  
		Last Modified: Thu, 21 Sep 2023 05:05:42 GMT  
		Size: 5.7 MB (5653015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3918ce48c762d5088f364e86b7567e96b603661e7951055502a8186ffc9254`  
		Last Modified: Thu, 21 Sep 2023 05:05:41 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbe84c01f6bd1a347e498a6f38b3ca893236b40591ad8ae7eea2edfc50b9d99`  
		Last Modified: Thu, 21 Sep 2023 05:05:41 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.18`

```console
$ docker pull nats@sha256:e9f41a4a8c1727e4a3ef9fdbff9cc963bfb88c7d77eaf946b2410e4f080e11c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:effbb639aba0db24ebaf3f42fe6e9201428fab869a9399897afeb797819e0a7d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9482934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7afe0964d1327c57759f61500b32db9d8337946f39bdc8264d0c0d8efef6921`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 20 Sep 2023 00:49:05 GMT
ENV NATS_SERVER=2.10.0
# Wed, 20 Sep 2023 00:49:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='59456ee8d222213c0f713e5b571156ec053db15288ee9035b3a7ad01e226c0bb' ;; 		armhf) natsArch='arm6'; sha256='c12c5cde86dba95fa4b433b58af3b9568893e3c7814fa22feae85eb47a9bb2bd' ;; 		armv7) natsArch='arm7'; sha256='748eb00c8d29c674bb4f98371a1afd8be9fba59336be9ef24d24fff148f1e7a4' ;; 		x86_64) natsArch='amd64'; sha256='76f5798ba3923dbc4f170bbae0055d3267d5c604179b2c644f6e7c79cc970d76' ;; 		x86) natsArch='386'; sha256='7f151267f76948293a5721e642b489e1135aecbeb2399dd23d00b04e6a609191' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 20 Sep 2023 00:49:08 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 20 Sep 2023 00:49:08 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 20 Sep 2023 00:49:08 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:49:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Sep 2023 00:49:08 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b04b7bc39016808990ede8996e6d82c3fd7375999baa7a075ce2b107276bd93`  
		Last Modified: Wed, 20 Sep 2023 00:49:47 GMT  
		Size: 6.1 MB (6080321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d9bfba1e3e94018e331b7feae544bb67022934ad7035d517856062cc8af6a2`  
		Last Modified: Wed, 20 Sep 2023 00:49:46 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a185a2d7152fec18042b0c2aaf92f7d8e6b4227691eb89b8cc180c1360a8cc`  
		Last Modified: Wed, 20 Sep 2023 00:49:46 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:84ff4ec4f07f6daee653039f475687b1fc9d518cfefd072fd7405c66708b2c52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8947432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ce27616fe886ff67930425f652c89bc5831f6566f233496b9f1269488d39bb9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Thu, 21 Sep 2023 00:07:43 GMT
ENV NATS_SERVER=2.10.1
# Thu, 21 Sep 2023 00:07:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='13ab69dd6b35b4e253e97f469b61c4038fb6c1d0de89df6dfc93f75af1728ace' ;; 		armhf) natsArch='arm6'; sha256='ad6da4b3289293624e1e60dd0c719d3f2c9cc768774b9f25e580c236915a906b' ;; 		armv7) natsArch='arm7'; sha256='9a706550622ce44f06e6cc44621c01aa27aa9f5da4347d4295e65e986b5cb907' ;; 		x86_64) natsArch='amd64'; sha256='f058d6195931f28cd14d2ac1b9b6a7ce1d760c66c76ccea72aa6b936f4b8d75c' ;; 		x86) natsArch='386'; sha256='1c1e82380139758a69b5040631890914a9db5234517ef9d82b0173e37b8ca96a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 21 Sep 2023 00:07:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 21 Sep 2023 00:07:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 21 Sep 2023 00:07:47 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 00:07:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Sep 2023 00:07:47 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f1a57b33f182668d91321a4367e03ea36a83b22cbb3512e7bf29a740166ac55`  
		Last Modified: Thu, 21 Sep 2023 00:08:27 GMT  
		Size: 5.8 MB (5801621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab09d7306f8d236dead5b1c5d7dfa7a6b386b8f86d77887da9405d0df4d4fd6`  
		Last Modified: Thu, 21 Sep 2023 00:08:25 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a037b525be2a5e8397e646ce00405c26939139fc529d945879cb727e772171`  
		Last Modified: Thu, 21 Sep 2023 00:08:25 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:793e82e82eb90127e5931e743d8b66fa93ce571aa7c3364b62fe1e8051397a0d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8694026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:029567069923892aa47d7aaf87e9018a5ad9406961686c368c467cef63fede5c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Wed, 20 Sep 2023 00:39:11 GMT
ENV NATS_SERVER=2.10.0
# Wed, 20 Sep 2023 00:39:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='59456ee8d222213c0f713e5b571156ec053db15288ee9035b3a7ad01e226c0bb' ;; 		armhf) natsArch='arm6'; sha256='c12c5cde86dba95fa4b433b58af3b9568893e3c7814fa22feae85eb47a9bb2bd' ;; 		armv7) natsArch='arm7'; sha256='748eb00c8d29c674bb4f98371a1afd8be9fba59336be9ef24d24fff148f1e7a4' ;; 		x86_64) natsArch='amd64'; sha256='76f5798ba3923dbc4f170bbae0055d3267d5c604179b2c644f6e7c79cc970d76' ;; 		x86) natsArch='386'; sha256='7f151267f76948293a5721e642b489e1135aecbeb2399dd23d00b04e6a609191' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 20 Sep 2023 00:39:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 20 Sep 2023 00:39:15 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 20 Sep 2023 00:39:15 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:39:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Sep 2023 00:39:15 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86cf505660fa5f57305b113eef333ce025a6d9136f88356db788061f3125927`  
		Last Modified: Wed, 20 Sep 2023 00:40:06 GMT  
		Size: 5.8 MB (5793543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7c97affb17c5049777a5f4c3748e8415a30d8e3fb1650078b3b33763877672`  
		Last Modified: Wed, 20 Sep 2023 00:40:05 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f28587da4e0140d1ee0d0f5fd63eb28e76cdbcc1cca375f6493d13f8fc404e`  
		Last Modified: Wed, 20 Sep 2023 00:40:05 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:2c90c42e3f08e748f4b37d4c85397f7434f2bc06f70f531348fd75f4981786a8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8984785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7d356a02623c8421e021ef35f15363a21ce68a6f855eeef311061f460fb4099`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Thu, 21 Sep 2023 05:04:42 GMT
ENV NATS_SERVER=2.10.1
# Thu, 21 Sep 2023 05:04:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='13ab69dd6b35b4e253e97f469b61c4038fb6c1d0de89df6dfc93f75af1728ace' ;; 		armhf) natsArch='arm6'; sha256='ad6da4b3289293624e1e60dd0c719d3f2c9cc768774b9f25e580c236915a906b' ;; 		armv7) natsArch='arm7'; sha256='9a706550622ce44f06e6cc44621c01aa27aa9f5da4347d4295e65e986b5cb907' ;; 		x86_64) natsArch='amd64'; sha256='f058d6195931f28cd14d2ac1b9b6a7ce1d760c66c76ccea72aa6b936f4b8d75c' ;; 		x86) natsArch='386'; sha256='1c1e82380139758a69b5040631890914a9db5234517ef9d82b0173e37b8ca96a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 21 Sep 2023 05:04:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 21 Sep 2023 05:04:44 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 21 Sep 2023 05:04:44 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 05:04:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Sep 2023 05:04:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36d636b74934d8449d366cac72e2a2f72e239d7a2b015bb861742b6954415a1`  
		Last Modified: Thu, 21 Sep 2023 05:05:42 GMT  
		Size: 5.7 MB (5653015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3918ce48c762d5088f364e86b7567e96b603661e7951055502a8186ffc9254`  
		Last Modified: Thu, 21 Sep 2023 05:05:41 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbe84c01f6bd1a347e498a6f38b3ca893236b40591ad8ae7eea2edfc50b9d99`  
		Last Modified: Thu, 21 Sep 2023 05:05:41 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:279c3e1bc63c82126abafed2b06ae0c23cfe06d526db00f0cd2bf790595b1e53
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:300b8159816cb200b0ddca347e2895e811131e89660b698819d6a04d017b51ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5457759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f5b65974bc0ab52f1a6bd8c018ff5fadadbc976f311db512c19acabce037b94`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 20 Sep 2023 00:49:23 GMT
COPY file:8e2a9a3f381167fcc1a95dc7718c10cb67f58a845a3197193a5273c57e28d08d in /nats-server 
# Wed, 20 Sep 2023 00:49:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 20 Sep 2023 00:49:23 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:49:23 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Sep 2023 00:49:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:949cbe9ff3fb07dc0fbd1c6fb6ba4a1c20304c28d574891f79f5d84e05439ec0`  
		Last Modified: Wed, 20 Sep 2023 00:50:22 GMT  
		Size: 5.5 MB (5457252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49c9fc5d845768deddd7c19342fd407ee4fdc4d110abf53e58444440c552181`  
		Last Modified: Wed, 20 Sep 2023 00:50:21 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:cce3ff90a32531db64bb74852140a156326d487dafbf812da2168f78c0e85388
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5178106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:111b8fef881498596233d1f7dda3dc1a4113c72bfe5e1088ded56d10a45d128f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 21 Sep 2023 00:07:58 GMT
COPY file:dbe6aeea160dba3a7bdcaf0c14808f7a7b31899bb87a50ed117996ead07014e6 in /nats-server 
# Thu, 21 Sep 2023 00:07:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 21 Sep 2023 00:07:58 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 00:07:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 21 Sep 2023 00:07:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6837114cbc023e4b8b17b6a951b2e91ab9668a1f3ffe65bec26f4ea44b812845`  
		Last Modified: Thu, 21 Sep 2023 00:08:53 GMT  
		Size: 5.2 MB (5177597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bde9589f631b3debf2ce00b1154c597464aeb530aac8a0016d7bee37f972958`  
		Last Modified: Thu, 21 Sep 2023 00:08:51 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:41b2a21a345689e5edc4cb8d24444c46df161e58ca89578e66a66e2e0aee2a47
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5171757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed343d1334d5c6f933acaae9f280c90acde044ea41eb6047dc9126ecd17dbd37`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 20 Sep 2023 00:39:39 GMT
COPY file:1ed1e6185c40930f2dc5e0e072cf3d42764ec8f3c10b2f65c3044c6aaf6d5ac5 in /nats-server 
# Wed, 20 Sep 2023 00:39:39 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 20 Sep 2023 00:39:39 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:39:40 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Sep 2023 00:39:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9af7ee06c60cdf35e2e953e1ad5700cf513329b5f88bb07096c8439fbdd7cfb4`  
		Last Modified: Wed, 20 Sep 2023 00:40:42 GMT  
		Size: 5.2 MB (5171248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5795401da82ad77eec35f59034d9f5ce5ff6af93cc82c2a00277bf954ef32c2`  
		Last Modified: Wed, 20 Sep 2023 00:40:41 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:e6aea49e5eb407c078286700c1402c6eda155ae11cdd40f8604194f6f70d0dd2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5029479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d109a8655a05cb22d5529db631b1a167bfae974cfc5d047c1ac261888ecd6e8`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 21 Sep 2023 05:05:18 GMT
COPY file:943544393eb61c235711dc43a87ec667d4491be8bcff70eee560d8276bd01b5b in /nats-server 
# Thu, 21 Sep 2023 05:05:18 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 21 Sep 2023 05:05:18 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 05:05:18 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 21 Sep 2023 05:05:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:85892a63e455fd1561bc50ef513a999a9a22152bbab4f029732ea77658da0b37`  
		Last Modified: Thu, 21 Sep 2023 05:06:05 GMT  
		Size: 5.0 MB (5028971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24d6a1649b69be08c681087d8f2f84e750824c24acb44b6d1be0a9a706bb112`  
		Last Modified: Thu, 21 Sep 2023 05:06:04 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:6670fad4a4d64481de5425c7a8ee8e602faef2f05646051096bfa59d9126cbfb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats@sha256:3ae7b24041d5c7f8bb775c1fd47da96b2891f8c6821bfe25f6bcf95a0eaf6064
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110068360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acf1d87f97e43bca95d8940d4aa3abf65c2c05adb6681005cb66f3f7d8001ffc`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Aug 2023 16:42:02 GMT
RUN Apply image 10.0.17763.4851
# Wed, 13 Sep 2023 05:08:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 21 Sep 2023 00:18:29 GMT
RUN cmd /S /C #(nop) COPY file:2b24d029bdf2310dcf6089c8f58986b6c70babf4fd4d433f329957862df58d77 in C:\nats-server.exe 
# Thu, 21 Sep 2023 00:18:29 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 21 Sep 2023 00:18:30 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 00:18:31 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 21 Sep 2023 00:18:31 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:17ba6b878467260559b72cb6f7e79c829eae67862a09efe87f6dc324f49fc086`  
		Last Modified: Tue, 12 Sep 2023 18:31:40 GMT  
		Size: 104.5 MB (104492504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9930674eb6676a1690e63a275d0da517ab8b8aeab7ccd20591f76f7c69a5`  
		Last Modified: Wed, 13 Sep 2023 05:08:48 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05405503d7afb6019521e5fa013d09e5c8636161e9408ba36c149f4853898e7`  
		Last Modified: Thu, 21 Sep 2023 00:19:36 GMT  
		Size: 5.6 MB (5569390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d1f97d2316001518d35eb0b75ac1888c2fe2da51ce49c16012d2fef9ccf5e0c`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.8 KB (1802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6a311706a8aadd91f05c001d3ffbd3a548f21286d0db22eed44fcd5999100f`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a3c2ef4f82e001ae8c4b096641708c8d404bd43dae8f46f843d21d8bb0fd69`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1a063be69428345c92d570f896ffe0326401a9b501ba554a0c4ebf8dc1f5dd`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:6670fad4a4d64481de5425c7a8ee8e602faef2f05646051096bfa59d9126cbfb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats@sha256:3ae7b24041d5c7f8bb775c1fd47da96b2891f8c6821bfe25f6bcf95a0eaf6064
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110068360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acf1d87f97e43bca95d8940d4aa3abf65c2c05adb6681005cb66f3f7d8001ffc`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Aug 2023 16:42:02 GMT
RUN Apply image 10.0.17763.4851
# Wed, 13 Sep 2023 05:08:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 21 Sep 2023 00:18:29 GMT
RUN cmd /S /C #(nop) COPY file:2b24d029bdf2310dcf6089c8f58986b6c70babf4fd4d433f329957862df58d77 in C:\nats-server.exe 
# Thu, 21 Sep 2023 00:18:29 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 21 Sep 2023 00:18:30 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 00:18:31 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 21 Sep 2023 00:18:31 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:17ba6b878467260559b72cb6f7e79c829eae67862a09efe87f6dc324f49fc086`  
		Last Modified: Tue, 12 Sep 2023 18:31:40 GMT  
		Size: 104.5 MB (104492504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9930674eb6676a1690e63a275d0da517ab8b8aeab7ccd20591f76f7c69a5`  
		Last Modified: Wed, 13 Sep 2023 05:08:48 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05405503d7afb6019521e5fa013d09e5c8636161e9408ba36c149f4853898e7`  
		Last Modified: Thu, 21 Sep 2023 00:19:36 GMT  
		Size: 5.6 MB (5569390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d1f97d2316001518d35eb0b75ac1888c2fe2da51ce49c16012d2fef9ccf5e0c`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.8 KB (1802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6a311706a8aadd91f05c001d3ffbd3a548f21286d0db22eed44fcd5999100f`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a3c2ef4f82e001ae8c4b096641708c8d404bd43dae8f46f843d21d8bb0fd69`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1a063be69428345c92d570f896ffe0326401a9b501ba554a0c4ebf8dc1f5dd`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:279c3e1bc63c82126abafed2b06ae0c23cfe06d526db00f0cd2bf790595b1e53
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:300b8159816cb200b0ddca347e2895e811131e89660b698819d6a04d017b51ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5457759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f5b65974bc0ab52f1a6bd8c018ff5fadadbc976f311db512c19acabce037b94`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 20 Sep 2023 00:49:23 GMT
COPY file:8e2a9a3f381167fcc1a95dc7718c10cb67f58a845a3197193a5273c57e28d08d in /nats-server 
# Wed, 20 Sep 2023 00:49:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 20 Sep 2023 00:49:23 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:49:23 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Sep 2023 00:49:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:949cbe9ff3fb07dc0fbd1c6fb6ba4a1c20304c28d574891f79f5d84e05439ec0`  
		Last Modified: Wed, 20 Sep 2023 00:50:22 GMT  
		Size: 5.5 MB (5457252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49c9fc5d845768deddd7c19342fd407ee4fdc4d110abf53e58444440c552181`  
		Last Modified: Wed, 20 Sep 2023 00:50:21 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:cce3ff90a32531db64bb74852140a156326d487dafbf812da2168f78c0e85388
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5178106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:111b8fef881498596233d1f7dda3dc1a4113c72bfe5e1088ded56d10a45d128f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 21 Sep 2023 00:07:58 GMT
COPY file:dbe6aeea160dba3a7bdcaf0c14808f7a7b31899bb87a50ed117996ead07014e6 in /nats-server 
# Thu, 21 Sep 2023 00:07:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 21 Sep 2023 00:07:58 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 00:07:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 21 Sep 2023 00:07:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6837114cbc023e4b8b17b6a951b2e91ab9668a1f3ffe65bec26f4ea44b812845`  
		Last Modified: Thu, 21 Sep 2023 00:08:53 GMT  
		Size: 5.2 MB (5177597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bde9589f631b3debf2ce00b1154c597464aeb530aac8a0016d7bee37f972958`  
		Last Modified: Thu, 21 Sep 2023 00:08:51 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:41b2a21a345689e5edc4cb8d24444c46df161e58ca89578e66a66e2e0aee2a47
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5171757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed343d1334d5c6f933acaae9f280c90acde044ea41eb6047dc9126ecd17dbd37`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 20 Sep 2023 00:39:39 GMT
COPY file:1ed1e6185c40930f2dc5e0e072cf3d42764ec8f3c10b2f65c3044c6aaf6d5ac5 in /nats-server 
# Wed, 20 Sep 2023 00:39:39 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 20 Sep 2023 00:39:39 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:39:40 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Sep 2023 00:39:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9af7ee06c60cdf35e2e953e1ad5700cf513329b5f88bb07096c8439fbdd7cfb4`  
		Last Modified: Wed, 20 Sep 2023 00:40:42 GMT  
		Size: 5.2 MB (5171248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5795401da82ad77eec35f59034d9f5ce5ff6af93cc82c2a00277bf954ef32c2`  
		Last Modified: Wed, 20 Sep 2023 00:40:41 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:e6aea49e5eb407c078286700c1402c6eda155ae11cdd40f8604194f6f70d0dd2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5029479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d109a8655a05cb22d5529db631b1a167bfae974cfc5d047c1ac261888ecd6e8`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 21 Sep 2023 05:05:18 GMT
COPY file:943544393eb61c235711dc43a87ec667d4491be8bcff70eee560d8276bd01b5b in /nats-server 
# Thu, 21 Sep 2023 05:05:18 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 21 Sep 2023 05:05:18 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 05:05:18 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 21 Sep 2023 05:05:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:85892a63e455fd1561bc50ef513a999a9a22152bbab4f029732ea77658da0b37`  
		Last Modified: Thu, 21 Sep 2023 05:06:05 GMT  
		Size: 5.0 MB (5028971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24d6a1649b69be08c681087d8f2f84e750824c24acb44b6d1be0a9a706bb112`  
		Last Modified: Thu, 21 Sep 2023 05:06:04 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:caacdd68ac15825419bdd0d1ed333408d4c22b3a26035275e48d153c22268c1c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats@sha256:6a50e306cf3f0c7dbd1e2df340d2696b1622ad3232c7d83cb0d1f72195089ca5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2022614730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f82b912330f09e1d0a6d64e3034e0da94f54645b45b8713a83652480b2bea1b5`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 03:56:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Sep 2023 05:05:36 GMT
ENV NATS_DOCKERIZED=1
# Thu, 21 Sep 2023 00:15:15 GMT
ENV NATS_SERVER=2.10.1
# Thu, 21 Sep 2023 00:15:15 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.10.1/nats-server-v2.10.1-windows-amd64.zip
# Thu, 21 Sep 2023 00:15:16 GMT
ENV NATS_SERVER_SHASUM=88f2990dd6fea0bb2d8ba5cfde41ab5c96dd01bbaf4f9e9a3569815a0803cb1c
# Thu, 21 Sep 2023 00:16:19 GMT
RUN Set-PSDebug -Trace 2
# Thu, 21 Sep 2023 00:18:04 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 21 Sep 2023 00:18:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 21 Sep 2023 00:18:06 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 00:18:07 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 21 Sep 2023 00:18:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b21bbf840142288ae2bce3465085b591133cf10f78f7dda43277db4838332d8`  
		Last Modified: Wed, 13 Sep 2023 04:36:45 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54f616fe064e9d4e73bf2aec9a4fe9c58837ec84c2fc998a54ab7a77b52e109`  
		Last Modified: Wed, 13 Sep 2023 05:08:32 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905f26828615c039d9da3e9f52c8b61ad3b2183a7ec3940bb1985bfc9a64be81`  
		Last Modified: Thu, 21 Sep 2023 00:19:20 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a235c3fc87ed07702e70bb83fcbcb5ccaf81440d9ffd8d450d16bb7f273ce0`  
		Last Modified: Thu, 21 Sep 2023 00:19:20 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759a393cccf186a4709cd9d0c4da137cade59a534bc53125be57217f7b21ef61`  
		Last Modified: Thu, 21 Sep 2023 00:19:20 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1cc61521de3ff29def7a6479a78dc7165d144b87f68e455eedb1ed30775aeaa`  
		Last Modified: Thu, 21 Sep 2023 00:19:20 GMT  
		Size: 242.8 KB (242789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d014e00481cb1e60003ba14c0a143d5126a763b4d413032ddad39559313825d`  
		Last Modified: Thu, 21 Sep 2023 00:19:19 GMT  
		Size: 6.0 MB (6028853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ba83a190b4d5c219eab28b93cc94ab37e1a941e7270d4e60b5114f037589da`  
		Last Modified: Thu, 21 Sep 2023 00:19:18 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9ab4d57441cb1024559b87812361354ac635647bdb46a4ea450769c671d6f2`  
		Last Modified: Thu, 21 Sep 2023 00:19:18 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd0e1cd2f7b50ded5cab327e6c888492fb4c4e022a0062cc719b9b6f9bcd8f4`  
		Last Modified: Thu, 21 Sep 2023 00:19:18 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca70f3129ad44afad7b489a20cfd3a7bd2187694d47690907dab50fc4638c34`  
		Last Modified: Thu, 21 Sep 2023 00:19:18 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:caacdd68ac15825419bdd0d1ed333408d4c22b3a26035275e48d153c22268c1c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats@sha256:6a50e306cf3f0c7dbd1e2df340d2696b1622ad3232c7d83cb0d1f72195089ca5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2022614730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f82b912330f09e1d0a6d64e3034e0da94f54645b45b8713a83652480b2bea1b5`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 03:56:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Sep 2023 05:05:36 GMT
ENV NATS_DOCKERIZED=1
# Thu, 21 Sep 2023 00:15:15 GMT
ENV NATS_SERVER=2.10.1
# Thu, 21 Sep 2023 00:15:15 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.10.1/nats-server-v2.10.1-windows-amd64.zip
# Thu, 21 Sep 2023 00:15:16 GMT
ENV NATS_SERVER_SHASUM=88f2990dd6fea0bb2d8ba5cfde41ab5c96dd01bbaf4f9e9a3569815a0803cb1c
# Thu, 21 Sep 2023 00:16:19 GMT
RUN Set-PSDebug -Trace 2
# Thu, 21 Sep 2023 00:18:04 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 21 Sep 2023 00:18:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 21 Sep 2023 00:18:06 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 00:18:07 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 21 Sep 2023 00:18:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b21bbf840142288ae2bce3465085b591133cf10f78f7dda43277db4838332d8`  
		Last Modified: Wed, 13 Sep 2023 04:36:45 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54f616fe064e9d4e73bf2aec9a4fe9c58837ec84c2fc998a54ab7a77b52e109`  
		Last Modified: Wed, 13 Sep 2023 05:08:32 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905f26828615c039d9da3e9f52c8b61ad3b2183a7ec3940bb1985bfc9a64be81`  
		Last Modified: Thu, 21 Sep 2023 00:19:20 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a235c3fc87ed07702e70bb83fcbcb5ccaf81440d9ffd8d450d16bb7f273ce0`  
		Last Modified: Thu, 21 Sep 2023 00:19:20 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759a393cccf186a4709cd9d0c4da137cade59a534bc53125be57217f7b21ef61`  
		Last Modified: Thu, 21 Sep 2023 00:19:20 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1cc61521de3ff29def7a6479a78dc7165d144b87f68e455eedb1ed30775aeaa`  
		Last Modified: Thu, 21 Sep 2023 00:19:20 GMT  
		Size: 242.8 KB (242789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d014e00481cb1e60003ba14c0a143d5126a763b4d413032ddad39559313825d`  
		Last Modified: Thu, 21 Sep 2023 00:19:19 GMT  
		Size: 6.0 MB (6028853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ba83a190b4d5c219eab28b93cc94ab37e1a941e7270d4e60b5114f037589da`  
		Last Modified: Thu, 21 Sep 2023 00:19:18 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9ab4d57441cb1024559b87812361354ac635647bdb46a4ea450769c671d6f2`  
		Last Modified: Thu, 21 Sep 2023 00:19:18 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd0e1cd2f7b50ded5cab327e6c888492fb4c4e022a0062cc719b9b6f9bcd8f4`  
		Last Modified: Thu, 21 Sep 2023 00:19:18 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca70f3129ad44afad7b489a20cfd3a7bd2187694d47690907dab50fc4638c34`  
		Last Modified: Thu, 21 Sep 2023 00:19:18 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10`

```console
$ docker pull nats@sha256:d2bdc0afd157302d96e103fad188c56b754559ceceb9e134edf57334a0973425
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4851; amd64

### `nats:2.10` - linux; amd64

```console
$ docker pull nats@sha256:300b8159816cb200b0ddca347e2895e811131e89660b698819d6a04d017b51ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5457759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f5b65974bc0ab52f1a6bd8c018ff5fadadbc976f311db512c19acabce037b94`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 20 Sep 2023 00:49:23 GMT
COPY file:8e2a9a3f381167fcc1a95dc7718c10cb67f58a845a3197193a5273c57e28d08d in /nats-server 
# Wed, 20 Sep 2023 00:49:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 20 Sep 2023 00:49:23 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:49:23 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Sep 2023 00:49:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:949cbe9ff3fb07dc0fbd1c6fb6ba4a1c20304c28d574891f79f5d84e05439ec0`  
		Last Modified: Wed, 20 Sep 2023 00:50:22 GMT  
		Size: 5.5 MB (5457252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49c9fc5d845768deddd7c19342fd407ee4fdc4d110abf53e58444440c552181`  
		Last Modified: Wed, 20 Sep 2023 00:50:21 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10` - linux; arm variant v6

```console
$ docker pull nats@sha256:cce3ff90a32531db64bb74852140a156326d487dafbf812da2168f78c0e85388
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5178106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:111b8fef881498596233d1f7dda3dc1a4113c72bfe5e1088ded56d10a45d128f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 21 Sep 2023 00:07:58 GMT
COPY file:dbe6aeea160dba3a7bdcaf0c14808f7a7b31899bb87a50ed117996ead07014e6 in /nats-server 
# Thu, 21 Sep 2023 00:07:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 21 Sep 2023 00:07:58 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 00:07:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 21 Sep 2023 00:07:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6837114cbc023e4b8b17b6a951b2e91ab9668a1f3ffe65bec26f4ea44b812845`  
		Last Modified: Thu, 21 Sep 2023 00:08:53 GMT  
		Size: 5.2 MB (5177597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bde9589f631b3debf2ce00b1154c597464aeb530aac8a0016d7bee37f972958`  
		Last Modified: Thu, 21 Sep 2023 00:08:51 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10` - linux; arm variant v7

```console
$ docker pull nats@sha256:41b2a21a345689e5edc4cb8d24444c46df161e58ca89578e66a66e2e0aee2a47
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5171757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed343d1334d5c6f933acaae9f280c90acde044ea41eb6047dc9126ecd17dbd37`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 20 Sep 2023 00:39:39 GMT
COPY file:1ed1e6185c40930f2dc5e0e072cf3d42764ec8f3c10b2f65c3044c6aaf6d5ac5 in /nats-server 
# Wed, 20 Sep 2023 00:39:39 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 20 Sep 2023 00:39:39 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:39:40 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Sep 2023 00:39:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9af7ee06c60cdf35e2e953e1ad5700cf513329b5f88bb07096c8439fbdd7cfb4`  
		Last Modified: Wed, 20 Sep 2023 00:40:42 GMT  
		Size: 5.2 MB (5171248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5795401da82ad77eec35f59034d9f5ce5ff6af93cc82c2a00277bf954ef32c2`  
		Last Modified: Wed, 20 Sep 2023 00:40:41 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:e6aea49e5eb407c078286700c1402c6eda155ae11cdd40f8604194f6f70d0dd2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5029479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d109a8655a05cb22d5529db631b1a167bfae974cfc5d047c1ac261888ecd6e8`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 21 Sep 2023 05:05:18 GMT
COPY file:943544393eb61c235711dc43a87ec667d4491be8bcff70eee560d8276bd01b5b in /nats-server 
# Thu, 21 Sep 2023 05:05:18 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 21 Sep 2023 05:05:18 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 05:05:18 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 21 Sep 2023 05:05:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:85892a63e455fd1561bc50ef513a999a9a22152bbab4f029732ea77658da0b37`  
		Last Modified: Thu, 21 Sep 2023 05:06:05 GMT  
		Size: 5.0 MB (5028971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24d6a1649b69be08c681087d8f2f84e750824c24acb44b6d1be0a9a706bb112`  
		Last Modified: Thu, 21 Sep 2023 05:06:04 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats@sha256:3ae7b24041d5c7f8bb775c1fd47da96b2891f8c6821bfe25f6bcf95a0eaf6064
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110068360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acf1d87f97e43bca95d8940d4aa3abf65c2c05adb6681005cb66f3f7d8001ffc`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Aug 2023 16:42:02 GMT
RUN Apply image 10.0.17763.4851
# Wed, 13 Sep 2023 05:08:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 21 Sep 2023 00:18:29 GMT
RUN cmd /S /C #(nop) COPY file:2b24d029bdf2310dcf6089c8f58986b6c70babf4fd4d433f329957862df58d77 in C:\nats-server.exe 
# Thu, 21 Sep 2023 00:18:29 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 21 Sep 2023 00:18:30 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 00:18:31 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 21 Sep 2023 00:18:31 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:17ba6b878467260559b72cb6f7e79c829eae67862a09efe87f6dc324f49fc086`  
		Last Modified: Tue, 12 Sep 2023 18:31:40 GMT  
		Size: 104.5 MB (104492504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9930674eb6676a1690e63a275d0da517ab8b8aeab7ccd20591f76f7c69a5`  
		Last Modified: Wed, 13 Sep 2023 05:08:48 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05405503d7afb6019521e5fa013d09e5c8636161e9408ba36c149f4853898e7`  
		Last Modified: Thu, 21 Sep 2023 00:19:36 GMT  
		Size: 5.6 MB (5569390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d1f97d2316001518d35eb0b75ac1888c2fe2da51ce49c16012d2fef9ccf5e0c`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.8 KB (1802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6a311706a8aadd91f05c001d3ffbd3a548f21286d0db22eed44fcd5999100f`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a3c2ef4f82e001ae8c4b096641708c8d404bd43dae8f46f843d21d8bb0fd69`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1a063be69428345c92d570f896ffe0326401a9b501ba554a0c4ebf8dc1f5dd`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10-alpine`

```console
$ docker pull nats@sha256:e9f41a4a8c1727e4a3ef9fdbff9cc963bfb88c7d77eaf946b2410e4f080e11c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.10-alpine` - linux; amd64

```console
$ docker pull nats@sha256:effbb639aba0db24ebaf3f42fe6e9201428fab869a9399897afeb797819e0a7d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9482934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7afe0964d1327c57759f61500b32db9d8337946f39bdc8264d0c0d8efef6921`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 20 Sep 2023 00:49:05 GMT
ENV NATS_SERVER=2.10.0
# Wed, 20 Sep 2023 00:49:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='59456ee8d222213c0f713e5b571156ec053db15288ee9035b3a7ad01e226c0bb' ;; 		armhf) natsArch='arm6'; sha256='c12c5cde86dba95fa4b433b58af3b9568893e3c7814fa22feae85eb47a9bb2bd' ;; 		armv7) natsArch='arm7'; sha256='748eb00c8d29c674bb4f98371a1afd8be9fba59336be9ef24d24fff148f1e7a4' ;; 		x86_64) natsArch='amd64'; sha256='76f5798ba3923dbc4f170bbae0055d3267d5c604179b2c644f6e7c79cc970d76' ;; 		x86) natsArch='386'; sha256='7f151267f76948293a5721e642b489e1135aecbeb2399dd23d00b04e6a609191' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 20 Sep 2023 00:49:08 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 20 Sep 2023 00:49:08 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 20 Sep 2023 00:49:08 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:49:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Sep 2023 00:49:08 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b04b7bc39016808990ede8996e6d82c3fd7375999baa7a075ce2b107276bd93`  
		Last Modified: Wed, 20 Sep 2023 00:49:47 GMT  
		Size: 6.1 MB (6080321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d9bfba1e3e94018e331b7feae544bb67022934ad7035d517856062cc8af6a2`  
		Last Modified: Wed, 20 Sep 2023 00:49:46 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a185a2d7152fec18042b0c2aaf92f7d8e6b4227691eb89b8cc180c1360a8cc`  
		Last Modified: Wed, 20 Sep 2023 00:49:46 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:84ff4ec4f07f6daee653039f475687b1fc9d518cfefd072fd7405c66708b2c52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8947432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ce27616fe886ff67930425f652c89bc5831f6566f233496b9f1269488d39bb9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Thu, 21 Sep 2023 00:07:43 GMT
ENV NATS_SERVER=2.10.1
# Thu, 21 Sep 2023 00:07:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='13ab69dd6b35b4e253e97f469b61c4038fb6c1d0de89df6dfc93f75af1728ace' ;; 		armhf) natsArch='arm6'; sha256='ad6da4b3289293624e1e60dd0c719d3f2c9cc768774b9f25e580c236915a906b' ;; 		armv7) natsArch='arm7'; sha256='9a706550622ce44f06e6cc44621c01aa27aa9f5da4347d4295e65e986b5cb907' ;; 		x86_64) natsArch='amd64'; sha256='f058d6195931f28cd14d2ac1b9b6a7ce1d760c66c76ccea72aa6b936f4b8d75c' ;; 		x86) natsArch='386'; sha256='1c1e82380139758a69b5040631890914a9db5234517ef9d82b0173e37b8ca96a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 21 Sep 2023 00:07:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 21 Sep 2023 00:07:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 21 Sep 2023 00:07:47 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 00:07:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Sep 2023 00:07:47 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f1a57b33f182668d91321a4367e03ea36a83b22cbb3512e7bf29a740166ac55`  
		Last Modified: Thu, 21 Sep 2023 00:08:27 GMT  
		Size: 5.8 MB (5801621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab09d7306f8d236dead5b1c5d7dfa7a6b386b8f86d77887da9405d0df4d4fd6`  
		Last Modified: Thu, 21 Sep 2023 00:08:25 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a037b525be2a5e8397e646ce00405c26939139fc529d945879cb727e772171`  
		Last Modified: Thu, 21 Sep 2023 00:08:25 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:793e82e82eb90127e5931e743d8b66fa93ce571aa7c3364b62fe1e8051397a0d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8694026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:029567069923892aa47d7aaf87e9018a5ad9406961686c368c467cef63fede5c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Wed, 20 Sep 2023 00:39:11 GMT
ENV NATS_SERVER=2.10.0
# Wed, 20 Sep 2023 00:39:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='59456ee8d222213c0f713e5b571156ec053db15288ee9035b3a7ad01e226c0bb' ;; 		armhf) natsArch='arm6'; sha256='c12c5cde86dba95fa4b433b58af3b9568893e3c7814fa22feae85eb47a9bb2bd' ;; 		armv7) natsArch='arm7'; sha256='748eb00c8d29c674bb4f98371a1afd8be9fba59336be9ef24d24fff148f1e7a4' ;; 		x86_64) natsArch='amd64'; sha256='76f5798ba3923dbc4f170bbae0055d3267d5c604179b2c644f6e7c79cc970d76' ;; 		x86) natsArch='386'; sha256='7f151267f76948293a5721e642b489e1135aecbeb2399dd23d00b04e6a609191' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 20 Sep 2023 00:39:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 20 Sep 2023 00:39:15 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 20 Sep 2023 00:39:15 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:39:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Sep 2023 00:39:15 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86cf505660fa5f57305b113eef333ce025a6d9136f88356db788061f3125927`  
		Last Modified: Wed, 20 Sep 2023 00:40:06 GMT  
		Size: 5.8 MB (5793543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7c97affb17c5049777a5f4c3748e8415a30d8e3fb1650078b3b33763877672`  
		Last Modified: Wed, 20 Sep 2023 00:40:05 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f28587da4e0140d1ee0d0f5fd63eb28e76cdbcc1cca375f6493d13f8fc404e`  
		Last Modified: Wed, 20 Sep 2023 00:40:05 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:2c90c42e3f08e748f4b37d4c85397f7434f2bc06f70f531348fd75f4981786a8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8984785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7d356a02623c8421e021ef35f15363a21ce68a6f855eeef311061f460fb4099`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Thu, 21 Sep 2023 05:04:42 GMT
ENV NATS_SERVER=2.10.1
# Thu, 21 Sep 2023 05:04:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='13ab69dd6b35b4e253e97f469b61c4038fb6c1d0de89df6dfc93f75af1728ace' ;; 		armhf) natsArch='arm6'; sha256='ad6da4b3289293624e1e60dd0c719d3f2c9cc768774b9f25e580c236915a906b' ;; 		armv7) natsArch='arm7'; sha256='9a706550622ce44f06e6cc44621c01aa27aa9f5da4347d4295e65e986b5cb907' ;; 		x86_64) natsArch='amd64'; sha256='f058d6195931f28cd14d2ac1b9b6a7ce1d760c66c76ccea72aa6b936f4b8d75c' ;; 		x86) natsArch='386'; sha256='1c1e82380139758a69b5040631890914a9db5234517ef9d82b0173e37b8ca96a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 21 Sep 2023 05:04:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 21 Sep 2023 05:04:44 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 21 Sep 2023 05:04:44 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 05:04:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Sep 2023 05:04:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36d636b74934d8449d366cac72e2a2f72e239d7a2b015bb861742b6954415a1`  
		Last Modified: Thu, 21 Sep 2023 05:05:42 GMT  
		Size: 5.7 MB (5653015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3918ce48c762d5088f364e86b7567e96b603661e7951055502a8186ffc9254`  
		Last Modified: Thu, 21 Sep 2023 05:05:41 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbe84c01f6bd1a347e498a6f38b3ca893236b40591ad8ae7eea2edfc50b9d99`  
		Last Modified: Thu, 21 Sep 2023 05:05:41 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10-alpine3.18`

```console
$ docker pull nats@sha256:e9f41a4a8c1727e4a3ef9fdbff9cc963bfb88c7d77eaf946b2410e4f080e11c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.10-alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:effbb639aba0db24ebaf3f42fe6e9201428fab869a9399897afeb797819e0a7d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9482934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7afe0964d1327c57759f61500b32db9d8337946f39bdc8264d0c0d8efef6921`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 20 Sep 2023 00:49:05 GMT
ENV NATS_SERVER=2.10.0
# Wed, 20 Sep 2023 00:49:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='59456ee8d222213c0f713e5b571156ec053db15288ee9035b3a7ad01e226c0bb' ;; 		armhf) natsArch='arm6'; sha256='c12c5cde86dba95fa4b433b58af3b9568893e3c7814fa22feae85eb47a9bb2bd' ;; 		armv7) natsArch='arm7'; sha256='748eb00c8d29c674bb4f98371a1afd8be9fba59336be9ef24d24fff148f1e7a4' ;; 		x86_64) natsArch='amd64'; sha256='76f5798ba3923dbc4f170bbae0055d3267d5c604179b2c644f6e7c79cc970d76' ;; 		x86) natsArch='386'; sha256='7f151267f76948293a5721e642b489e1135aecbeb2399dd23d00b04e6a609191' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 20 Sep 2023 00:49:08 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 20 Sep 2023 00:49:08 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 20 Sep 2023 00:49:08 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:49:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Sep 2023 00:49:08 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b04b7bc39016808990ede8996e6d82c3fd7375999baa7a075ce2b107276bd93`  
		Last Modified: Wed, 20 Sep 2023 00:49:47 GMT  
		Size: 6.1 MB (6080321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d9bfba1e3e94018e331b7feae544bb67022934ad7035d517856062cc8af6a2`  
		Last Modified: Wed, 20 Sep 2023 00:49:46 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a185a2d7152fec18042b0c2aaf92f7d8e6b4227691eb89b8cc180c1360a8cc`  
		Last Modified: Wed, 20 Sep 2023 00:49:46 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:84ff4ec4f07f6daee653039f475687b1fc9d518cfefd072fd7405c66708b2c52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8947432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ce27616fe886ff67930425f652c89bc5831f6566f233496b9f1269488d39bb9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Thu, 21 Sep 2023 00:07:43 GMT
ENV NATS_SERVER=2.10.1
# Thu, 21 Sep 2023 00:07:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='13ab69dd6b35b4e253e97f469b61c4038fb6c1d0de89df6dfc93f75af1728ace' ;; 		armhf) natsArch='arm6'; sha256='ad6da4b3289293624e1e60dd0c719d3f2c9cc768774b9f25e580c236915a906b' ;; 		armv7) natsArch='arm7'; sha256='9a706550622ce44f06e6cc44621c01aa27aa9f5da4347d4295e65e986b5cb907' ;; 		x86_64) natsArch='amd64'; sha256='f058d6195931f28cd14d2ac1b9b6a7ce1d760c66c76ccea72aa6b936f4b8d75c' ;; 		x86) natsArch='386'; sha256='1c1e82380139758a69b5040631890914a9db5234517ef9d82b0173e37b8ca96a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 21 Sep 2023 00:07:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 21 Sep 2023 00:07:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 21 Sep 2023 00:07:47 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 00:07:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Sep 2023 00:07:47 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f1a57b33f182668d91321a4367e03ea36a83b22cbb3512e7bf29a740166ac55`  
		Last Modified: Thu, 21 Sep 2023 00:08:27 GMT  
		Size: 5.8 MB (5801621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab09d7306f8d236dead5b1c5d7dfa7a6b386b8f86d77887da9405d0df4d4fd6`  
		Last Modified: Thu, 21 Sep 2023 00:08:25 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a037b525be2a5e8397e646ce00405c26939139fc529d945879cb727e772171`  
		Last Modified: Thu, 21 Sep 2023 00:08:25 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:793e82e82eb90127e5931e743d8b66fa93ce571aa7c3364b62fe1e8051397a0d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8694026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:029567069923892aa47d7aaf87e9018a5ad9406961686c368c467cef63fede5c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Wed, 20 Sep 2023 00:39:11 GMT
ENV NATS_SERVER=2.10.0
# Wed, 20 Sep 2023 00:39:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='59456ee8d222213c0f713e5b571156ec053db15288ee9035b3a7ad01e226c0bb' ;; 		armhf) natsArch='arm6'; sha256='c12c5cde86dba95fa4b433b58af3b9568893e3c7814fa22feae85eb47a9bb2bd' ;; 		armv7) natsArch='arm7'; sha256='748eb00c8d29c674bb4f98371a1afd8be9fba59336be9ef24d24fff148f1e7a4' ;; 		x86_64) natsArch='amd64'; sha256='76f5798ba3923dbc4f170bbae0055d3267d5c604179b2c644f6e7c79cc970d76' ;; 		x86) natsArch='386'; sha256='7f151267f76948293a5721e642b489e1135aecbeb2399dd23d00b04e6a609191' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 20 Sep 2023 00:39:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 20 Sep 2023 00:39:15 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 20 Sep 2023 00:39:15 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:39:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Sep 2023 00:39:15 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86cf505660fa5f57305b113eef333ce025a6d9136f88356db788061f3125927`  
		Last Modified: Wed, 20 Sep 2023 00:40:06 GMT  
		Size: 5.8 MB (5793543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7c97affb17c5049777a5f4c3748e8415a30d8e3fb1650078b3b33763877672`  
		Last Modified: Wed, 20 Sep 2023 00:40:05 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f28587da4e0140d1ee0d0f5fd63eb28e76cdbcc1cca375f6493d13f8fc404e`  
		Last Modified: Wed, 20 Sep 2023 00:40:05 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:2c90c42e3f08e748f4b37d4c85397f7434f2bc06f70f531348fd75f4981786a8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8984785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7d356a02623c8421e021ef35f15363a21ce68a6f855eeef311061f460fb4099`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Thu, 21 Sep 2023 05:04:42 GMT
ENV NATS_SERVER=2.10.1
# Thu, 21 Sep 2023 05:04:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='13ab69dd6b35b4e253e97f469b61c4038fb6c1d0de89df6dfc93f75af1728ace' ;; 		armhf) natsArch='arm6'; sha256='ad6da4b3289293624e1e60dd0c719d3f2c9cc768774b9f25e580c236915a906b' ;; 		armv7) natsArch='arm7'; sha256='9a706550622ce44f06e6cc44621c01aa27aa9f5da4347d4295e65e986b5cb907' ;; 		x86_64) natsArch='amd64'; sha256='f058d6195931f28cd14d2ac1b9b6a7ce1d760c66c76ccea72aa6b936f4b8d75c' ;; 		x86) natsArch='386'; sha256='1c1e82380139758a69b5040631890914a9db5234517ef9d82b0173e37b8ca96a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 21 Sep 2023 05:04:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 21 Sep 2023 05:04:44 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 21 Sep 2023 05:04:44 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 05:04:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Sep 2023 05:04:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36d636b74934d8449d366cac72e2a2f72e239d7a2b015bb861742b6954415a1`  
		Last Modified: Thu, 21 Sep 2023 05:05:42 GMT  
		Size: 5.7 MB (5653015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3918ce48c762d5088f364e86b7567e96b603661e7951055502a8186ffc9254`  
		Last Modified: Thu, 21 Sep 2023 05:05:41 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbe84c01f6bd1a347e498a6f38b3ca893236b40591ad8ae7eea2edfc50b9d99`  
		Last Modified: Thu, 21 Sep 2023 05:05:41 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10-linux`

```console
$ docker pull nats@sha256:279c3e1bc63c82126abafed2b06ae0c23cfe06d526db00f0cd2bf790595b1e53
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.10-linux` - linux; amd64

```console
$ docker pull nats@sha256:300b8159816cb200b0ddca347e2895e811131e89660b698819d6a04d017b51ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5457759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f5b65974bc0ab52f1a6bd8c018ff5fadadbc976f311db512c19acabce037b94`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 20 Sep 2023 00:49:23 GMT
COPY file:8e2a9a3f381167fcc1a95dc7718c10cb67f58a845a3197193a5273c57e28d08d in /nats-server 
# Wed, 20 Sep 2023 00:49:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 20 Sep 2023 00:49:23 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:49:23 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Sep 2023 00:49:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:949cbe9ff3fb07dc0fbd1c6fb6ba4a1c20304c28d574891f79f5d84e05439ec0`  
		Last Modified: Wed, 20 Sep 2023 00:50:22 GMT  
		Size: 5.5 MB (5457252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49c9fc5d845768deddd7c19342fd407ee4fdc4d110abf53e58444440c552181`  
		Last Modified: Wed, 20 Sep 2023 00:50:21 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:cce3ff90a32531db64bb74852140a156326d487dafbf812da2168f78c0e85388
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5178106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:111b8fef881498596233d1f7dda3dc1a4113c72bfe5e1088ded56d10a45d128f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 21 Sep 2023 00:07:58 GMT
COPY file:dbe6aeea160dba3a7bdcaf0c14808f7a7b31899bb87a50ed117996ead07014e6 in /nats-server 
# Thu, 21 Sep 2023 00:07:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 21 Sep 2023 00:07:58 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 00:07:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 21 Sep 2023 00:07:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6837114cbc023e4b8b17b6a951b2e91ab9668a1f3ffe65bec26f4ea44b812845`  
		Last Modified: Thu, 21 Sep 2023 00:08:53 GMT  
		Size: 5.2 MB (5177597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bde9589f631b3debf2ce00b1154c597464aeb530aac8a0016d7bee37f972958`  
		Last Modified: Thu, 21 Sep 2023 00:08:51 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:41b2a21a345689e5edc4cb8d24444c46df161e58ca89578e66a66e2e0aee2a47
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5171757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed343d1334d5c6f933acaae9f280c90acde044ea41eb6047dc9126ecd17dbd37`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 20 Sep 2023 00:39:39 GMT
COPY file:1ed1e6185c40930f2dc5e0e072cf3d42764ec8f3c10b2f65c3044c6aaf6d5ac5 in /nats-server 
# Wed, 20 Sep 2023 00:39:39 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 20 Sep 2023 00:39:39 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:39:40 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Sep 2023 00:39:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9af7ee06c60cdf35e2e953e1ad5700cf513329b5f88bb07096c8439fbdd7cfb4`  
		Last Modified: Wed, 20 Sep 2023 00:40:42 GMT  
		Size: 5.2 MB (5171248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5795401da82ad77eec35f59034d9f5ce5ff6af93cc82c2a00277bf954ef32c2`  
		Last Modified: Wed, 20 Sep 2023 00:40:41 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:e6aea49e5eb407c078286700c1402c6eda155ae11cdd40f8604194f6f70d0dd2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5029479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d109a8655a05cb22d5529db631b1a167bfae974cfc5d047c1ac261888ecd6e8`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 21 Sep 2023 05:05:18 GMT
COPY file:943544393eb61c235711dc43a87ec667d4491be8bcff70eee560d8276bd01b5b in /nats-server 
# Thu, 21 Sep 2023 05:05:18 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 21 Sep 2023 05:05:18 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 05:05:18 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 21 Sep 2023 05:05:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:85892a63e455fd1561bc50ef513a999a9a22152bbab4f029732ea77658da0b37`  
		Last Modified: Thu, 21 Sep 2023 05:06:05 GMT  
		Size: 5.0 MB (5028971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24d6a1649b69be08c681087d8f2f84e750824c24acb44b6d1be0a9a706bb112`  
		Last Modified: Thu, 21 Sep 2023 05:06:04 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10-nanoserver`

```console
$ docker pull nats@sha256:6670fad4a4d64481de5425c7a8ee8e602faef2f05646051096bfa59d9126cbfb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `nats:2.10-nanoserver` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats@sha256:3ae7b24041d5c7f8bb775c1fd47da96b2891f8c6821bfe25f6bcf95a0eaf6064
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110068360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acf1d87f97e43bca95d8940d4aa3abf65c2c05adb6681005cb66f3f7d8001ffc`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Aug 2023 16:42:02 GMT
RUN Apply image 10.0.17763.4851
# Wed, 13 Sep 2023 05:08:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 21 Sep 2023 00:18:29 GMT
RUN cmd /S /C #(nop) COPY file:2b24d029bdf2310dcf6089c8f58986b6c70babf4fd4d433f329957862df58d77 in C:\nats-server.exe 
# Thu, 21 Sep 2023 00:18:29 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 21 Sep 2023 00:18:30 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 00:18:31 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 21 Sep 2023 00:18:31 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:17ba6b878467260559b72cb6f7e79c829eae67862a09efe87f6dc324f49fc086`  
		Last Modified: Tue, 12 Sep 2023 18:31:40 GMT  
		Size: 104.5 MB (104492504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9930674eb6676a1690e63a275d0da517ab8b8aeab7ccd20591f76f7c69a5`  
		Last Modified: Wed, 13 Sep 2023 05:08:48 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05405503d7afb6019521e5fa013d09e5c8636161e9408ba36c149f4853898e7`  
		Last Modified: Thu, 21 Sep 2023 00:19:36 GMT  
		Size: 5.6 MB (5569390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d1f97d2316001518d35eb0b75ac1888c2fe2da51ce49c16012d2fef9ccf5e0c`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.8 KB (1802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6a311706a8aadd91f05c001d3ffbd3a548f21286d0db22eed44fcd5999100f`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a3c2ef4f82e001ae8c4b096641708c8d404bd43dae8f46f843d21d8bb0fd69`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1a063be69428345c92d570f896ffe0326401a9b501ba554a0c4ebf8dc1f5dd`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10-nanoserver-1809`

```console
$ docker pull nats@sha256:6670fad4a4d64481de5425c7a8ee8e602faef2f05646051096bfa59d9126cbfb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `nats:2.10-nanoserver-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats@sha256:3ae7b24041d5c7f8bb775c1fd47da96b2891f8c6821bfe25f6bcf95a0eaf6064
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110068360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acf1d87f97e43bca95d8940d4aa3abf65c2c05adb6681005cb66f3f7d8001ffc`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Aug 2023 16:42:02 GMT
RUN Apply image 10.0.17763.4851
# Wed, 13 Sep 2023 05:08:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 21 Sep 2023 00:18:29 GMT
RUN cmd /S /C #(nop) COPY file:2b24d029bdf2310dcf6089c8f58986b6c70babf4fd4d433f329957862df58d77 in C:\nats-server.exe 
# Thu, 21 Sep 2023 00:18:29 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 21 Sep 2023 00:18:30 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 00:18:31 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 21 Sep 2023 00:18:31 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:17ba6b878467260559b72cb6f7e79c829eae67862a09efe87f6dc324f49fc086`  
		Last Modified: Tue, 12 Sep 2023 18:31:40 GMT  
		Size: 104.5 MB (104492504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9930674eb6676a1690e63a275d0da517ab8b8aeab7ccd20591f76f7c69a5`  
		Last Modified: Wed, 13 Sep 2023 05:08:48 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05405503d7afb6019521e5fa013d09e5c8636161e9408ba36c149f4853898e7`  
		Last Modified: Thu, 21 Sep 2023 00:19:36 GMT  
		Size: 5.6 MB (5569390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d1f97d2316001518d35eb0b75ac1888c2fe2da51ce49c16012d2fef9ccf5e0c`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.8 KB (1802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6a311706a8aadd91f05c001d3ffbd3a548f21286d0db22eed44fcd5999100f`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a3c2ef4f82e001ae8c4b096641708c8d404bd43dae8f46f843d21d8bb0fd69`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1a063be69428345c92d570f896ffe0326401a9b501ba554a0c4ebf8dc1f5dd`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10-scratch`

```console
$ docker pull nats@sha256:279c3e1bc63c82126abafed2b06ae0c23cfe06d526db00f0cd2bf790595b1e53
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.10-scratch` - linux; amd64

```console
$ docker pull nats@sha256:300b8159816cb200b0ddca347e2895e811131e89660b698819d6a04d017b51ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5457759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f5b65974bc0ab52f1a6bd8c018ff5fadadbc976f311db512c19acabce037b94`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 20 Sep 2023 00:49:23 GMT
COPY file:8e2a9a3f381167fcc1a95dc7718c10cb67f58a845a3197193a5273c57e28d08d in /nats-server 
# Wed, 20 Sep 2023 00:49:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 20 Sep 2023 00:49:23 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:49:23 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Sep 2023 00:49:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:949cbe9ff3fb07dc0fbd1c6fb6ba4a1c20304c28d574891f79f5d84e05439ec0`  
		Last Modified: Wed, 20 Sep 2023 00:50:22 GMT  
		Size: 5.5 MB (5457252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49c9fc5d845768deddd7c19342fd407ee4fdc4d110abf53e58444440c552181`  
		Last Modified: Wed, 20 Sep 2023 00:50:21 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:cce3ff90a32531db64bb74852140a156326d487dafbf812da2168f78c0e85388
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5178106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:111b8fef881498596233d1f7dda3dc1a4113c72bfe5e1088ded56d10a45d128f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 21 Sep 2023 00:07:58 GMT
COPY file:dbe6aeea160dba3a7bdcaf0c14808f7a7b31899bb87a50ed117996ead07014e6 in /nats-server 
# Thu, 21 Sep 2023 00:07:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 21 Sep 2023 00:07:58 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 00:07:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 21 Sep 2023 00:07:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6837114cbc023e4b8b17b6a951b2e91ab9668a1f3ffe65bec26f4ea44b812845`  
		Last Modified: Thu, 21 Sep 2023 00:08:53 GMT  
		Size: 5.2 MB (5177597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bde9589f631b3debf2ce00b1154c597464aeb530aac8a0016d7bee37f972958`  
		Last Modified: Thu, 21 Sep 2023 00:08:51 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:41b2a21a345689e5edc4cb8d24444c46df161e58ca89578e66a66e2e0aee2a47
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5171757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed343d1334d5c6f933acaae9f280c90acde044ea41eb6047dc9126ecd17dbd37`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 20 Sep 2023 00:39:39 GMT
COPY file:1ed1e6185c40930f2dc5e0e072cf3d42764ec8f3c10b2f65c3044c6aaf6d5ac5 in /nats-server 
# Wed, 20 Sep 2023 00:39:39 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 20 Sep 2023 00:39:39 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:39:40 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Sep 2023 00:39:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9af7ee06c60cdf35e2e953e1ad5700cf513329b5f88bb07096c8439fbdd7cfb4`  
		Last Modified: Wed, 20 Sep 2023 00:40:42 GMT  
		Size: 5.2 MB (5171248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5795401da82ad77eec35f59034d9f5ce5ff6af93cc82c2a00277bf954ef32c2`  
		Last Modified: Wed, 20 Sep 2023 00:40:41 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:e6aea49e5eb407c078286700c1402c6eda155ae11cdd40f8604194f6f70d0dd2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5029479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d109a8655a05cb22d5529db631b1a167bfae974cfc5d047c1ac261888ecd6e8`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 21 Sep 2023 05:05:18 GMT
COPY file:943544393eb61c235711dc43a87ec667d4491be8bcff70eee560d8276bd01b5b in /nats-server 
# Thu, 21 Sep 2023 05:05:18 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 21 Sep 2023 05:05:18 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 05:05:18 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 21 Sep 2023 05:05:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:85892a63e455fd1561bc50ef513a999a9a22152bbab4f029732ea77658da0b37`  
		Last Modified: Thu, 21 Sep 2023 05:06:05 GMT  
		Size: 5.0 MB (5028971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24d6a1649b69be08c681087d8f2f84e750824c24acb44b6d1be0a9a706bb112`  
		Last Modified: Thu, 21 Sep 2023 05:06:04 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10-windowsservercore`

```console
$ docker pull nats@sha256:caacdd68ac15825419bdd0d1ed333408d4c22b3a26035275e48d153c22268c1c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `nats:2.10-windowsservercore` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats@sha256:6a50e306cf3f0c7dbd1e2df340d2696b1622ad3232c7d83cb0d1f72195089ca5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2022614730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f82b912330f09e1d0a6d64e3034e0da94f54645b45b8713a83652480b2bea1b5`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 03:56:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Sep 2023 05:05:36 GMT
ENV NATS_DOCKERIZED=1
# Thu, 21 Sep 2023 00:15:15 GMT
ENV NATS_SERVER=2.10.1
# Thu, 21 Sep 2023 00:15:15 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.10.1/nats-server-v2.10.1-windows-amd64.zip
# Thu, 21 Sep 2023 00:15:16 GMT
ENV NATS_SERVER_SHASUM=88f2990dd6fea0bb2d8ba5cfde41ab5c96dd01bbaf4f9e9a3569815a0803cb1c
# Thu, 21 Sep 2023 00:16:19 GMT
RUN Set-PSDebug -Trace 2
# Thu, 21 Sep 2023 00:18:04 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 21 Sep 2023 00:18:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 21 Sep 2023 00:18:06 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 00:18:07 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 21 Sep 2023 00:18:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b21bbf840142288ae2bce3465085b591133cf10f78f7dda43277db4838332d8`  
		Last Modified: Wed, 13 Sep 2023 04:36:45 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54f616fe064e9d4e73bf2aec9a4fe9c58837ec84c2fc998a54ab7a77b52e109`  
		Last Modified: Wed, 13 Sep 2023 05:08:32 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905f26828615c039d9da3e9f52c8b61ad3b2183a7ec3940bb1985bfc9a64be81`  
		Last Modified: Thu, 21 Sep 2023 00:19:20 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a235c3fc87ed07702e70bb83fcbcb5ccaf81440d9ffd8d450d16bb7f273ce0`  
		Last Modified: Thu, 21 Sep 2023 00:19:20 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759a393cccf186a4709cd9d0c4da137cade59a534bc53125be57217f7b21ef61`  
		Last Modified: Thu, 21 Sep 2023 00:19:20 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1cc61521de3ff29def7a6479a78dc7165d144b87f68e455eedb1ed30775aeaa`  
		Last Modified: Thu, 21 Sep 2023 00:19:20 GMT  
		Size: 242.8 KB (242789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d014e00481cb1e60003ba14c0a143d5126a763b4d413032ddad39559313825d`  
		Last Modified: Thu, 21 Sep 2023 00:19:19 GMT  
		Size: 6.0 MB (6028853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ba83a190b4d5c219eab28b93cc94ab37e1a941e7270d4e60b5114f037589da`  
		Last Modified: Thu, 21 Sep 2023 00:19:18 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9ab4d57441cb1024559b87812361354ac635647bdb46a4ea450769c671d6f2`  
		Last Modified: Thu, 21 Sep 2023 00:19:18 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd0e1cd2f7b50ded5cab327e6c888492fb4c4e022a0062cc719b9b6f9bcd8f4`  
		Last Modified: Thu, 21 Sep 2023 00:19:18 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca70f3129ad44afad7b489a20cfd3a7bd2187694d47690907dab50fc4638c34`  
		Last Modified: Thu, 21 Sep 2023 00:19:18 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10-windowsservercore-1809`

```console
$ docker pull nats@sha256:caacdd68ac15825419bdd0d1ed333408d4c22b3a26035275e48d153c22268c1c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `nats:2.10-windowsservercore-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats@sha256:6a50e306cf3f0c7dbd1e2df340d2696b1622ad3232c7d83cb0d1f72195089ca5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2022614730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f82b912330f09e1d0a6d64e3034e0da94f54645b45b8713a83652480b2bea1b5`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 03:56:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Sep 2023 05:05:36 GMT
ENV NATS_DOCKERIZED=1
# Thu, 21 Sep 2023 00:15:15 GMT
ENV NATS_SERVER=2.10.1
# Thu, 21 Sep 2023 00:15:15 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.10.1/nats-server-v2.10.1-windows-amd64.zip
# Thu, 21 Sep 2023 00:15:16 GMT
ENV NATS_SERVER_SHASUM=88f2990dd6fea0bb2d8ba5cfde41ab5c96dd01bbaf4f9e9a3569815a0803cb1c
# Thu, 21 Sep 2023 00:16:19 GMT
RUN Set-PSDebug -Trace 2
# Thu, 21 Sep 2023 00:18:04 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 21 Sep 2023 00:18:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 21 Sep 2023 00:18:06 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 00:18:07 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 21 Sep 2023 00:18:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b21bbf840142288ae2bce3465085b591133cf10f78f7dda43277db4838332d8`  
		Last Modified: Wed, 13 Sep 2023 04:36:45 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54f616fe064e9d4e73bf2aec9a4fe9c58837ec84c2fc998a54ab7a77b52e109`  
		Last Modified: Wed, 13 Sep 2023 05:08:32 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905f26828615c039d9da3e9f52c8b61ad3b2183a7ec3940bb1985bfc9a64be81`  
		Last Modified: Thu, 21 Sep 2023 00:19:20 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a235c3fc87ed07702e70bb83fcbcb5ccaf81440d9ffd8d450d16bb7f273ce0`  
		Last Modified: Thu, 21 Sep 2023 00:19:20 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759a393cccf186a4709cd9d0c4da137cade59a534bc53125be57217f7b21ef61`  
		Last Modified: Thu, 21 Sep 2023 00:19:20 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1cc61521de3ff29def7a6479a78dc7165d144b87f68e455eedb1ed30775aeaa`  
		Last Modified: Thu, 21 Sep 2023 00:19:20 GMT  
		Size: 242.8 KB (242789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d014e00481cb1e60003ba14c0a143d5126a763b4d413032ddad39559313825d`  
		Last Modified: Thu, 21 Sep 2023 00:19:19 GMT  
		Size: 6.0 MB (6028853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ba83a190b4d5c219eab28b93cc94ab37e1a941e7270d4e60b5114f037589da`  
		Last Modified: Thu, 21 Sep 2023 00:19:18 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9ab4d57441cb1024559b87812361354ac635647bdb46a4ea450769c671d6f2`  
		Last Modified: Thu, 21 Sep 2023 00:19:18 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd0e1cd2f7b50ded5cab327e6c888492fb4c4e022a0062cc719b9b6f9bcd8f4`  
		Last Modified: Thu, 21 Sep 2023 00:19:18 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca70f3129ad44afad7b489a20cfd3a7bd2187694d47690907dab50fc4638c34`  
		Last Modified: Thu, 21 Sep 2023 00:19:18 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.1`

```console
$ docker pull nats@sha256:0a32bcf62a4763af6e2614c25ad79fa3d1d14106d127a67a7c1646300de2ae89
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4851; amd64

### `nats:2.10.1` - linux; arm variant v6

```console
$ docker pull nats@sha256:cce3ff90a32531db64bb74852140a156326d487dafbf812da2168f78c0e85388
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5178106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:111b8fef881498596233d1f7dda3dc1a4113c72bfe5e1088ded56d10a45d128f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 21 Sep 2023 00:07:58 GMT
COPY file:dbe6aeea160dba3a7bdcaf0c14808f7a7b31899bb87a50ed117996ead07014e6 in /nats-server 
# Thu, 21 Sep 2023 00:07:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 21 Sep 2023 00:07:58 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 00:07:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 21 Sep 2023 00:07:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6837114cbc023e4b8b17b6a951b2e91ab9668a1f3ffe65bec26f4ea44b812845`  
		Last Modified: Thu, 21 Sep 2023 00:08:53 GMT  
		Size: 5.2 MB (5177597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bde9589f631b3debf2ce00b1154c597464aeb530aac8a0016d7bee37f972958`  
		Last Modified: Thu, 21 Sep 2023 00:08:51 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.1` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:e6aea49e5eb407c078286700c1402c6eda155ae11cdd40f8604194f6f70d0dd2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5029479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d109a8655a05cb22d5529db631b1a167bfae974cfc5d047c1ac261888ecd6e8`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 21 Sep 2023 05:05:18 GMT
COPY file:943544393eb61c235711dc43a87ec667d4491be8bcff70eee560d8276bd01b5b in /nats-server 
# Thu, 21 Sep 2023 05:05:18 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 21 Sep 2023 05:05:18 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 05:05:18 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 21 Sep 2023 05:05:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:85892a63e455fd1561bc50ef513a999a9a22152bbab4f029732ea77658da0b37`  
		Last Modified: Thu, 21 Sep 2023 05:06:05 GMT  
		Size: 5.0 MB (5028971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24d6a1649b69be08c681087d8f2f84e750824c24acb44b6d1be0a9a706bb112`  
		Last Modified: Thu, 21 Sep 2023 05:06:04 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.1` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats@sha256:3ae7b24041d5c7f8bb775c1fd47da96b2891f8c6821bfe25f6bcf95a0eaf6064
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110068360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acf1d87f97e43bca95d8940d4aa3abf65c2c05adb6681005cb66f3f7d8001ffc`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Aug 2023 16:42:02 GMT
RUN Apply image 10.0.17763.4851
# Wed, 13 Sep 2023 05:08:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 21 Sep 2023 00:18:29 GMT
RUN cmd /S /C #(nop) COPY file:2b24d029bdf2310dcf6089c8f58986b6c70babf4fd4d433f329957862df58d77 in C:\nats-server.exe 
# Thu, 21 Sep 2023 00:18:29 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 21 Sep 2023 00:18:30 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 00:18:31 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 21 Sep 2023 00:18:31 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:17ba6b878467260559b72cb6f7e79c829eae67862a09efe87f6dc324f49fc086`  
		Last Modified: Tue, 12 Sep 2023 18:31:40 GMT  
		Size: 104.5 MB (104492504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9930674eb6676a1690e63a275d0da517ab8b8aeab7ccd20591f76f7c69a5`  
		Last Modified: Wed, 13 Sep 2023 05:08:48 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05405503d7afb6019521e5fa013d09e5c8636161e9408ba36c149f4853898e7`  
		Last Modified: Thu, 21 Sep 2023 00:19:36 GMT  
		Size: 5.6 MB (5569390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d1f97d2316001518d35eb0b75ac1888c2fe2da51ce49c16012d2fef9ccf5e0c`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.8 KB (1802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6a311706a8aadd91f05c001d3ffbd3a548f21286d0db22eed44fcd5999100f`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a3c2ef4f82e001ae8c4b096641708c8d404bd43dae8f46f843d21d8bb0fd69`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1a063be69428345c92d570f896ffe0326401a9b501ba554a0c4ebf8dc1f5dd`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.1-alpine`

```console
$ docker pull nats@sha256:1ea66a35583be784ef1210872c0980b94d3359850efda8e22b12d63b18d1baf4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `nats:2.10.1-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:84ff4ec4f07f6daee653039f475687b1fc9d518cfefd072fd7405c66708b2c52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8947432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ce27616fe886ff67930425f652c89bc5831f6566f233496b9f1269488d39bb9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Thu, 21 Sep 2023 00:07:43 GMT
ENV NATS_SERVER=2.10.1
# Thu, 21 Sep 2023 00:07:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='13ab69dd6b35b4e253e97f469b61c4038fb6c1d0de89df6dfc93f75af1728ace' ;; 		armhf) natsArch='arm6'; sha256='ad6da4b3289293624e1e60dd0c719d3f2c9cc768774b9f25e580c236915a906b' ;; 		armv7) natsArch='arm7'; sha256='9a706550622ce44f06e6cc44621c01aa27aa9f5da4347d4295e65e986b5cb907' ;; 		x86_64) natsArch='amd64'; sha256='f058d6195931f28cd14d2ac1b9b6a7ce1d760c66c76ccea72aa6b936f4b8d75c' ;; 		x86) natsArch='386'; sha256='1c1e82380139758a69b5040631890914a9db5234517ef9d82b0173e37b8ca96a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 21 Sep 2023 00:07:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 21 Sep 2023 00:07:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 21 Sep 2023 00:07:47 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 00:07:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Sep 2023 00:07:47 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f1a57b33f182668d91321a4367e03ea36a83b22cbb3512e7bf29a740166ac55`  
		Last Modified: Thu, 21 Sep 2023 00:08:27 GMT  
		Size: 5.8 MB (5801621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab09d7306f8d236dead5b1c5d7dfa7a6b386b8f86d77887da9405d0df4d4fd6`  
		Last Modified: Thu, 21 Sep 2023 00:08:25 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a037b525be2a5e8397e646ce00405c26939139fc529d945879cb727e772171`  
		Last Modified: Thu, 21 Sep 2023 00:08:25 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.1-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:2c90c42e3f08e748f4b37d4c85397f7434f2bc06f70f531348fd75f4981786a8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8984785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7d356a02623c8421e021ef35f15363a21ce68a6f855eeef311061f460fb4099`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Thu, 21 Sep 2023 05:04:42 GMT
ENV NATS_SERVER=2.10.1
# Thu, 21 Sep 2023 05:04:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='13ab69dd6b35b4e253e97f469b61c4038fb6c1d0de89df6dfc93f75af1728ace' ;; 		armhf) natsArch='arm6'; sha256='ad6da4b3289293624e1e60dd0c719d3f2c9cc768774b9f25e580c236915a906b' ;; 		armv7) natsArch='arm7'; sha256='9a706550622ce44f06e6cc44621c01aa27aa9f5da4347d4295e65e986b5cb907' ;; 		x86_64) natsArch='amd64'; sha256='f058d6195931f28cd14d2ac1b9b6a7ce1d760c66c76ccea72aa6b936f4b8d75c' ;; 		x86) natsArch='386'; sha256='1c1e82380139758a69b5040631890914a9db5234517ef9d82b0173e37b8ca96a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 21 Sep 2023 05:04:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 21 Sep 2023 05:04:44 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 21 Sep 2023 05:04:44 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 05:04:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Sep 2023 05:04:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36d636b74934d8449d366cac72e2a2f72e239d7a2b015bb861742b6954415a1`  
		Last Modified: Thu, 21 Sep 2023 05:05:42 GMT  
		Size: 5.7 MB (5653015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3918ce48c762d5088f364e86b7567e96b603661e7951055502a8186ffc9254`  
		Last Modified: Thu, 21 Sep 2023 05:05:41 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbe84c01f6bd1a347e498a6f38b3ca893236b40591ad8ae7eea2edfc50b9d99`  
		Last Modified: Thu, 21 Sep 2023 05:05:41 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.1-alpine3.18`

```console
$ docker pull nats@sha256:1ea66a35583be784ef1210872c0980b94d3359850efda8e22b12d63b18d1baf4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `nats:2.10.1-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:84ff4ec4f07f6daee653039f475687b1fc9d518cfefd072fd7405c66708b2c52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8947432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ce27616fe886ff67930425f652c89bc5831f6566f233496b9f1269488d39bb9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Thu, 21 Sep 2023 00:07:43 GMT
ENV NATS_SERVER=2.10.1
# Thu, 21 Sep 2023 00:07:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='13ab69dd6b35b4e253e97f469b61c4038fb6c1d0de89df6dfc93f75af1728ace' ;; 		armhf) natsArch='arm6'; sha256='ad6da4b3289293624e1e60dd0c719d3f2c9cc768774b9f25e580c236915a906b' ;; 		armv7) natsArch='arm7'; sha256='9a706550622ce44f06e6cc44621c01aa27aa9f5da4347d4295e65e986b5cb907' ;; 		x86_64) natsArch='amd64'; sha256='f058d6195931f28cd14d2ac1b9b6a7ce1d760c66c76ccea72aa6b936f4b8d75c' ;; 		x86) natsArch='386'; sha256='1c1e82380139758a69b5040631890914a9db5234517ef9d82b0173e37b8ca96a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 21 Sep 2023 00:07:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 21 Sep 2023 00:07:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 21 Sep 2023 00:07:47 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 00:07:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Sep 2023 00:07:47 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f1a57b33f182668d91321a4367e03ea36a83b22cbb3512e7bf29a740166ac55`  
		Last Modified: Thu, 21 Sep 2023 00:08:27 GMT  
		Size: 5.8 MB (5801621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab09d7306f8d236dead5b1c5d7dfa7a6b386b8f86d77887da9405d0df4d4fd6`  
		Last Modified: Thu, 21 Sep 2023 00:08:25 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a037b525be2a5e8397e646ce00405c26939139fc529d945879cb727e772171`  
		Last Modified: Thu, 21 Sep 2023 00:08:25 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.1-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:2c90c42e3f08e748f4b37d4c85397f7434f2bc06f70f531348fd75f4981786a8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8984785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7d356a02623c8421e021ef35f15363a21ce68a6f855eeef311061f460fb4099`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Thu, 21 Sep 2023 05:04:42 GMT
ENV NATS_SERVER=2.10.1
# Thu, 21 Sep 2023 05:04:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='13ab69dd6b35b4e253e97f469b61c4038fb6c1d0de89df6dfc93f75af1728ace' ;; 		armhf) natsArch='arm6'; sha256='ad6da4b3289293624e1e60dd0c719d3f2c9cc768774b9f25e580c236915a906b' ;; 		armv7) natsArch='arm7'; sha256='9a706550622ce44f06e6cc44621c01aa27aa9f5da4347d4295e65e986b5cb907' ;; 		x86_64) natsArch='amd64'; sha256='f058d6195931f28cd14d2ac1b9b6a7ce1d760c66c76ccea72aa6b936f4b8d75c' ;; 		x86) natsArch='386'; sha256='1c1e82380139758a69b5040631890914a9db5234517ef9d82b0173e37b8ca96a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 21 Sep 2023 05:04:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 21 Sep 2023 05:04:44 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 21 Sep 2023 05:04:44 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 05:04:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Sep 2023 05:04:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36d636b74934d8449d366cac72e2a2f72e239d7a2b015bb861742b6954415a1`  
		Last Modified: Thu, 21 Sep 2023 05:05:42 GMT  
		Size: 5.7 MB (5653015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3918ce48c762d5088f364e86b7567e96b603661e7951055502a8186ffc9254`  
		Last Modified: Thu, 21 Sep 2023 05:05:41 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbe84c01f6bd1a347e498a6f38b3ca893236b40591ad8ae7eea2edfc50b9d99`  
		Last Modified: Thu, 21 Sep 2023 05:05:41 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.1-linux`

```console
$ docker pull nats@sha256:9f01f9f8b3861c084ecb451539c4e9a9c4de11b47e5c6c1d3701a1603658d124
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `nats:2.10.1-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:cce3ff90a32531db64bb74852140a156326d487dafbf812da2168f78c0e85388
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5178106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:111b8fef881498596233d1f7dda3dc1a4113c72bfe5e1088ded56d10a45d128f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 21 Sep 2023 00:07:58 GMT
COPY file:dbe6aeea160dba3a7bdcaf0c14808f7a7b31899bb87a50ed117996ead07014e6 in /nats-server 
# Thu, 21 Sep 2023 00:07:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 21 Sep 2023 00:07:58 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 00:07:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 21 Sep 2023 00:07:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6837114cbc023e4b8b17b6a951b2e91ab9668a1f3ffe65bec26f4ea44b812845`  
		Last Modified: Thu, 21 Sep 2023 00:08:53 GMT  
		Size: 5.2 MB (5177597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bde9589f631b3debf2ce00b1154c597464aeb530aac8a0016d7bee37f972958`  
		Last Modified: Thu, 21 Sep 2023 00:08:51 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.1-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:e6aea49e5eb407c078286700c1402c6eda155ae11cdd40f8604194f6f70d0dd2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5029479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d109a8655a05cb22d5529db631b1a167bfae974cfc5d047c1ac261888ecd6e8`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 21 Sep 2023 05:05:18 GMT
COPY file:943544393eb61c235711dc43a87ec667d4491be8bcff70eee560d8276bd01b5b in /nats-server 
# Thu, 21 Sep 2023 05:05:18 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 21 Sep 2023 05:05:18 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 05:05:18 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 21 Sep 2023 05:05:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:85892a63e455fd1561bc50ef513a999a9a22152bbab4f029732ea77658da0b37`  
		Last Modified: Thu, 21 Sep 2023 05:06:05 GMT  
		Size: 5.0 MB (5028971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24d6a1649b69be08c681087d8f2f84e750824c24acb44b6d1be0a9a706bb112`  
		Last Modified: Thu, 21 Sep 2023 05:06:04 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.1-nanoserver`

```console
$ docker pull nats@sha256:6670fad4a4d64481de5425c7a8ee8e602faef2f05646051096bfa59d9126cbfb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `nats:2.10.1-nanoserver` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats@sha256:3ae7b24041d5c7f8bb775c1fd47da96b2891f8c6821bfe25f6bcf95a0eaf6064
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110068360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acf1d87f97e43bca95d8940d4aa3abf65c2c05adb6681005cb66f3f7d8001ffc`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Aug 2023 16:42:02 GMT
RUN Apply image 10.0.17763.4851
# Wed, 13 Sep 2023 05:08:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 21 Sep 2023 00:18:29 GMT
RUN cmd /S /C #(nop) COPY file:2b24d029bdf2310dcf6089c8f58986b6c70babf4fd4d433f329957862df58d77 in C:\nats-server.exe 
# Thu, 21 Sep 2023 00:18:29 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 21 Sep 2023 00:18:30 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 00:18:31 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 21 Sep 2023 00:18:31 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:17ba6b878467260559b72cb6f7e79c829eae67862a09efe87f6dc324f49fc086`  
		Last Modified: Tue, 12 Sep 2023 18:31:40 GMT  
		Size: 104.5 MB (104492504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9930674eb6676a1690e63a275d0da517ab8b8aeab7ccd20591f76f7c69a5`  
		Last Modified: Wed, 13 Sep 2023 05:08:48 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05405503d7afb6019521e5fa013d09e5c8636161e9408ba36c149f4853898e7`  
		Last Modified: Thu, 21 Sep 2023 00:19:36 GMT  
		Size: 5.6 MB (5569390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d1f97d2316001518d35eb0b75ac1888c2fe2da51ce49c16012d2fef9ccf5e0c`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.8 KB (1802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6a311706a8aadd91f05c001d3ffbd3a548f21286d0db22eed44fcd5999100f`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a3c2ef4f82e001ae8c4b096641708c8d404bd43dae8f46f843d21d8bb0fd69`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1a063be69428345c92d570f896ffe0326401a9b501ba554a0c4ebf8dc1f5dd`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.1-nanoserver-1809`

```console
$ docker pull nats@sha256:6670fad4a4d64481de5425c7a8ee8e602faef2f05646051096bfa59d9126cbfb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `nats:2.10.1-nanoserver-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats@sha256:3ae7b24041d5c7f8bb775c1fd47da96b2891f8c6821bfe25f6bcf95a0eaf6064
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110068360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acf1d87f97e43bca95d8940d4aa3abf65c2c05adb6681005cb66f3f7d8001ffc`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Aug 2023 16:42:02 GMT
RUN Apply image 10.0.17763.4851
# Wed, 13 Sep 2023 05:08:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 21 Sep 2023 00:18:29 GMT
RUN cmd /S /C #(nop) COPY file:2b24d029bdf2310dcf6089c8f58986b6c70babf4fd4d433f329957862df58d77 in C:\nats-server.exe 
# Thu, 21 Sep 2023 00:18:29 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 21 Sep 2023 00:18:30 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 00:18:31 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 21 Sep 2023 00:18:31 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:17ba6b878467260559b72cb6f7e79c829eae67862a09efe87f6dc324f49fc086`  
		Last Modified: Tue, 12 Sep 2023 18:31:40 GMT  
		Size: 104.5 MB (104492504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9930674eb6676a1690e63a275d0da517ab8b8aeab7ccd20591f76f7c69a5`  
		Last Modified: Wed, 13 Sep 2023 05:08:48 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05405503d7afb6019521e5fa013d09e5c8636161e9408ba36c149f4853898e7`  
		Last Modified: Thu, 21 Sep 2023 00:19:36 GMT  
		Size: 5.6 MB (5569390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d1f97d2316001518d35eb0b75ac1888c2fe2da51ce49c16012d2fef9ccf5e0c`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.8 KB (1802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6a311706a8aadd91f05c001d3ffbd3a548f21286d0db22eed44fcd5999100f`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a3c2ef4f82e001ae8c4b096641708c8d404bd43dae8f46f843d21d8bb0fd69`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1a063be69428345c92d570f896ffe0326401a9b501ba554a0c4ebf8dc1f5dd`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.1-scratch`

```console
$ docker pull nats@sha256:9f01f9f8b3861c084ecb451539c4e9a9c4de11b47e5c6c1d3701a1603658d124
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `nats:2.10.1-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:cce3ff90a32531db64bb74852140a156326d487dafbf812da2168f78c0e85388
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5178106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:111b8fef881498596233d1f7dda3dc1a4113c72bfe5e1088ded56d10a45d128f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 21 Sep 2023 00:07:58 GMT
COPY file:dbe6aeea160dba3a7bdcaf0c14808f7a7b31899bb87a50ed117996ead07014e6 in /nats-server 
# Thu, 21 Sep 2023 00:07:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 21 Sep 2023 00:07:58 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 00:07:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 21 Sep 2023 00:07:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6837114cbc023e4b8b17b6a951b2e91ab9668a1f3ffe65bec26f4ea44b812845`  
		Last Modified: Thu, 21 Sep 2023 00:08:53 GMT  
		Size: 5.2 MB (5177597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bde9589f631b3debf2ce00b1154c597464aeb530aac8a0016d7bee37f972958`  
		Last Modified: Thu, 21 Sep 2023 00:08:51 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.1-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:e6aea49e5eb407c078286700c1402c6eda155ae11cdd40f8604194f6f70d0dd2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5029479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d109a8655a05cb22d5529db631b1a167bfae974cfc5d047c1ac261888ecd6e8`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 21 Sep 2023 05:05:18 GMT
COPY file:943544393eb61c235711dc43a87ec667d4491be8bcff70eee560d8276bd01b5b in /nats-server 
# Thu, 21 Sep 2023 05:05:18 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 21 Sep 2023 05:05:18 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 05:05:18 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 21 Sep 2023 05:05:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:85892a63e455fd1561bc50ef513a999a9a22152bbab4f029732ea77658da0b37`  
		Last Modified: Thu, 21 Sep 2023 05:06:05 GMT  
		Size: 5.0 MB (5028971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24d6a1649b69be08c681087d8f2f84e750824c24acb44b6d1be0a9a706bb112`  
		Last Modified: Thu, 21 Sep 2023 05:06:04 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.1-windowsservercore`

```console
$ docker pull nats@sha256:caacdd68ac15825419bdd0d1ed333408d4c22b3a26035275e48d153c22268c1c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `nats:2.10.1-windowsservercore` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats@sha256:6a50e306cf3f0c7dbd1e2df340d2696b1622ad3232c7d83cb0d1f72195089ca5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2022614730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f82b912330f09e1d0a6d64e3034e0da94f54645b45b8713a83652480b2bea1b5`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 03:56:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Sep 2023 05:05:36 GMT
ENV NATS_DOCKERIZED=1
# Thu, 21 Sep 2023 00:15:15 GMT
ENV NATS_SERVER=2.10.1
# Thu, 21 Sep 2023 00:15:15 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.10.1/nats-server-v2.10.1-windows-amd64.zip
# Thu, 21 Sep 2023 00:15:16 GMT
ENV NATS_SERVER_SHASUM=88f2990dd6fea0bb2d8ba5cfde41ab5c96dd01bbaf4f9e9a3569815a0803cb1c
# Thu, 21 Sep 2023 00:16:19 GMT
RUN Set-PSDebug -Trace 2
# Thu, 21 Sep 2023 00:18:04 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 21 Sep 2023 00:18:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 21 Sep 2023 00:18:06 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 00:18:07 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 21 Sep 2023 00:18:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b21bbf840142288ae2bce3465085b591133cf10f78f7dda43277db4838332d8`  
		Last Modified: Wed, 13 Sep 2023 04:36:45 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54f616fe064e9d4e73bf2aec9a4fe9c58837ec84c2fc998a54ab7a77b52e109`  
		Last Modified: Wed, 13 Sep 2023 05:08:32 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905f26828615c039d9da3e9f52c8b61ad3b2183a7ec3940bb1985bfc9a64be81`  
		Last Modified: Thu, 21 Sep 2023 00:19:20 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a235c3fc87ed07702e70bb83fcbcb5ccaf81440d9ffd8d450d16bb7f273ce0`  
		Last Modified: Thu, 21 Sep 2023 00:19:20 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759a393cccf186a4709cd9d0c4da137cade59a534bc53125be57217f7b21ef61`  
		Last Modified: Thu, 21 Sep 2023 00:19:20 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1cc61521de3ff29def7a6479a78dc7165d144b87f68e455eedb1ed30775aeaa`  
		Last Modified: Thu, 21 Sep 2023 00:19:20 GMT  
		Size: 242.8 KB (242789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d014e00481cb1e60003ba14c0a143d5126a763b4d413032ddad39559313825d`  
		Last Modified: Thu, 21 Sep 2023 00:19:19 GMT  
		Size: 6.0 MB (6028853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ba83a190b4d5c219eab28b93cc94ab37e1a941e7270d4e60b5114f037589da`  
		Last Modified: Thu, 21 Sep 2023 00:19:18 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9ab4d57441cb1024559b87812361354ac635647bdb46a4ea450769c671d6f2`  
		Last Modified: Thu, 21 Sep 2023 00:19:18 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd0e1cd2f7b50ded5cab327e6c888492fb4c4e022a0062cc719b9b6f9bcd8f4`  
		Last Modified: Thu, 21 Sep 2023 00:19:18 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca70f3129ad44afad7b489a20cfd3a7bd2187694d47690907dab50fc4638c34`  
		Last Modified: Thu, 21 Sep 2023 00:19:18 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.1-windowsservercore-1809`

```console
$ docker pull nats@sha256:caacdd68ac15825419bdd0d1ed333408d4c22b3a26035275e48d153c22268c1c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `nats:2.10.1-windowsservercore-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats@sha256:6a50e306cf3f0c7dbd1e2df340d2696b1622ad3232c7d83cb0d1f72195089ca5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2022614730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f82b912330f09e1d0a6d64e3034e0da94f54645b45b8713a83652480b2bea1b5`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 03:56:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Sep 2023 05:05:36 GMT
ENV NATS_DOCKERIZED=1
# Thu, 21 Sep 2023 00:15:15 GMT
ENV NATS_SERVER=2.10.1
# Thu, 21 Sep 2023 00:15:15 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.10.1/nats-server-v2.10.1-windows-amd64.zip
# Thu, 21 Sep 2023 00:15:16 GMT
ENV NATS_SERVER_SHASUM=88f2990dd6fea0bb2d8ba5cfde41ab5c96dd01bbaf4f9e9a3569815a0803cb1c
# Thu, 21 Sep 2023 00:16:19 GMT
RUN Set-PSDebug -Trace 2
# Thu, 21 Sep 2023 00:18:04 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 21 Sep 2023 00:18:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 21 Sep 2023 00:18:06 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 00:18:07 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 21 Sep 2023 00:18:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b21bbf840142288ae2bce3465085b591133cf10f78f7dda43277db4838332d8`  
		Last Modified: Wed, 13 Sep 2023 04:36:45 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54f616fe064e9d4e73bf2aec9a4fe9c58837ec84c2fc998a54ab7a77b52e109`  
		Last Modified: Wed, 13 Sep 2023 05:08:32 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905f26828615c039d9da3e9f52c8b61ad3b2183a7ec3940bb1985bfc9a64be81`  
		Last Modified: Thu, 21 Sep 2023 00:19:20 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a235c3fc87ed07702e70bb83fcbcb5ccaf81440d9ffd8d450d16bb7f273ce0`  
		Last Modified: Thu, 21 Sep 2023 00:19:20 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759a393cccf186a4709cd9d0c4da137cade59a534bc53125be57217f7b21ef61`  
		Last Modified: Thu, 21 Sep 2023 00:19:20 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1cc61521de3ff29def7a6479a78dc7165d144b87f68e455eedb1ed30775aeaa`  
		Last Modified: Thu, 21 Sep 2023 00:19:20 GMT  
		Size: 242.8 KB (242789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d014e00481cb1e60003ba14c0a143d5126a763b4d413032ddad39559313825d`  
		Last Modified: Thu, 21 Sep 2023 00:19:19 GMT  
		Size: 6.0 MB (6028853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ba83a190b4d5c219eab28b93cc94ab37e1a941e7270d4e60b5114f037589da`  
		Last Modified: Thu, 21 Sep 2023 00:19:18 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9ab4d57441cb1024559b87812361354ac635647bdb46a4ea450769c671d6f2`  
		Last Modified: Thu, 21 Sep 2023 00:19:18 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd0e1cd2f7b50ded5cab327e6c888492fb4c4e022a0062cc719b9b6f9bcd8f4`  
		Last Modified: Thu, 21 Sep 2023 00:19:18 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca70f3129ad44afad7b489a20cfd3a7bd2187694d47690907dab50fc4638c34`  
		Last Modified: Thu, 21 Sep 2023 00:19:18 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9`

```console
$ docker pull nats@sha256:488386bec6ea7b0822f48795e51ed1dd0b367e6e2fffe466d4f304e2fa628918
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9` - linux; amd64

```console
$ docker pull nats@sha256:2a08a0c1d913294be585667f17f76f028053f5bf47b9d317e5bc0e409011ed1e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5245282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3517f7b93c37103553431effcb0b5a8262feb87c3649b04249d86012c34a9761`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 20 Sep 2023 00:49:17 GMT
COPY file:acdb0e47969d6e334bcadb9c85dfef3166c764ff4ac55254185a04b1a6e8bbee in /nats-server 
# Wed, 20 Sep 2023 00:49:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 20 Sep 2023 00:49:17 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:49:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Sep 2023 00:49:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aac801db9a2a97942dde4494f98ce2d08c529a3af03ecb92f0b93426bbfd6419`  
		Last Modified: Wed, 06 Sep 2023 23:20:56 GMT  
		Size: 5.2 MB (5244773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1646134cd3aac5e501d3658b95fcfd870fb902c4c9591a801a5b370a5aa574`  
		Last Modified: Wed, 20 Sep 2023 00:50:09 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm variant v6

```console
$ docker pull nats@sha256:4f09dbc6c43267500545fe441ec8057908d1b6bab5333c432c5e3d4c7ea0fd58
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4980014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:898dfa8e8c4c3e0c69c7c3aec16c90f1f6db172f3af0e7ff763b3bf8db42ed3c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Sep 2023 23:49:29 GMT
COPY file:51aacaba9769a3f16e0467be1fc8eb86122f6f3496e89e41b61e0038083ae308 in /nats-server 
# Tue, 19 Sep 2023 23:49:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Sep 2023 23:49:29 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Sep 2023 23:49:29 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Sep 2023 23:49:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6a6e165fccf6da77ad3b09408162fc7daaafe266b71dd5da8679594aa110a3a5`  
		Last Modified: Wed, 06 Sep 2023 23:05:32 GMT  
		Size: 5.0 MB (4979506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07c6021b659fa78c25ff92ad1e74c46e34c95c5e691ca45f27ced97ea7ef9e2`  
		Last Modified: Tue, 19 Sep 2023 23:50:15 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm variant v7

```console
$ docker pull nats@sha256:64211266fe0d926796dae72e7484f5aebbdb77c7e7faa3fab3d01954fe03a82e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4970849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a40010bd31b571ac24ead3a8630fa80ce8609b0352d5dab096c6b72940be90a6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 20 Sep 2023 00:39:32 GMT
COPY file:aae670bb79c659968f632ae3be388af62614010873ced2a439475906dbb769c6 in /nats-server 
# Wed, 20 Sep 2023 00:39:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 20 Sep 2023 00:39:32 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:39:32 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Sep 2023 00:39:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:55b6dbad6639da13368cebb9688e8a5caaee29041e6b5e2e798201dfcf2b67ad`  
		Last Modified: Wed, 06 Sep 2023 22:58:23 GMT  
		Size: 5.0 MB (4970341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969097b6afede4aab7deed51f12918311993aadbe7075d4965c14497831f4a12`  
		Last Modified: Wed, 20 Sep 2023 00:40:29 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:91e7a991da679db1020b25a760298f6944a9ea917e9ae90f10d1d7de9381fec4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4778849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb1745f4f81f20c728e9276ed07416c88490859cdbed438bdcb68aa051eb586c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Sep 2023 23:42:56 GMT
COPY file:d6eca5c67de65d1a8a30a51ea7318b044949c77108b2fdccc5aa0054c068c196 in /nats-server 
# Tue, 19 Sep 2023 23:42:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Sep 2023 23:42:56 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Sep 2023 23:42:56 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Sep 2023 23:42:56 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:88e5ff7f26ea25c6d2ab092989d9372cb32b3e60880124facfcefd7d3f0b7591`  
		Last Modified: Wed, 06 Sep 2023 22:40:49 GMT  
		Size: 4.8 MB (4778340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2424880e07e944598022ff8713b5897eb59c72af17978f7a3f1afa42dd022088`  
		Last Modified: Tue, 19 Sep 2023 23:43:51 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine`

```console
$ docker pull nats@sha256:36d34c59ed76472d9b3caafc5e3764b7a587498808efdd5178468f4efe8b4887
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine` - linux; amd64

```console
$ docker pull nats@sha256:756a55661288407f688c52224ac8b12d008f0fec9343c68281b04bb59cbcc427
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9270382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbb9252d07acfbe3ac9083449c0fef74561021019d85c2993f5bce02c7a16201`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 23:19:53 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 23:19:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 23:19:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 23:19:55 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 23:19:55 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:19:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 23:19:55 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75fdd304ec17c2cf1f7629eefc922e04fae260b6d902e4fd42c81a5e5ce9d5dc`  
		Last Modified: Wed, 06 Sep 2023 23:20:32 GMT  
		Size: 5.9 MB (5867770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2863800c65f086f618bf3df0e7855997aea26ba27f4c759cf8bfae94da866bb`  
		Last Modified: Wed, 06 Sep 2023 23:20:31 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e32a641538132ed9885ca87c473fe9ff71415289c1f5276ba1157bb0760bd04`  
		Last Modified: Wed, 06 Sep 2023 23:20:31 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:e66fcde15a5b8028aed7cdd2e03392aa10c4a51c224e964f014eddc1c821433d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8749092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6e3524e57732f8e26091d551f1b5ce64405e4217d19f047345dc28a29a1b847`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 23:04:40 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 23:04:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 23:04:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 23:04:43 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 23:04:43 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:04:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 23:04:43 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a6e71bd2ab60e313e659b569f8c33e5e9dcfdb580c25af0f9c5e7eca59f92f`  
		Last Modified: Wed, 06 Sep 2023 23:05:08 GMT  
		Size: 5.6 MB (5603285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b94c778bbad17cc9be59c68102602e2e77462672d2e045f4713e80ce1cbb1c`  
		Last Modified: Wed, 06 Sep 2023 23:05:07 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b258e6095309f7819e72dd444d848fe600fb2e73b5bd12bd1e9a556a17bf56`  
		Last Modified: Wed, 06 Sep 2023 23:05:07 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:9ca6685d1ad99fa588f9d4dc05ffe27569ed660b735218fd38795568fe508c73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8492829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0271598ef211f3df61073ff64c769275b4bb72b68b984931c8a7af1706fe80c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 22:57:29 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 22:57:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 22:57:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 22:57:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 22:57:32 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:57:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 22:57:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1962026ec365b08ba406dd0e38e57c06dcd04f2225faffcc17883ed87716cdc8`  
		Last Modified: Wed, 06 Sep 2023 22:58:03 GMT  
		Size: 5.6 MB (5592351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578cf75378460664df525d3b5d1412e778f7b8cdc5f3c31207b3bbc2f6c074f5`  
		Last Modified: Wed, 06 Sep 2023 22:58:01 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64bf3e24d68a6cadd0880ce3163738934bf8e5b267923da68dd6922cd6b98a31`  
		Last Modified: Wed, 06 Sep 2023 22:58:01 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:51e884da4e764cc784998e4bc69bbbefa4f39420be30021b4a1074dc40604423
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8734219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c8cdff0ce493eb27f871f27f7ec452d1c36de63801fda0b331cd41067f858b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 22:39:45 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 22:39:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 22:39:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 22:39:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 22:39:47 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 22:39:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64353667b2ee68f04c527f8dcef72789d979435b90c5b8073485e6c2fcc5c3f7`  
		Last Modified: Wed, 06 Sep 2023 22:40:28 GMT  
		Size: 5.4 MB (5402455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540b41e481b61500ce8ed1c72cc5c0f937cabb489d0ba9de2dc2dad279696a28`  
		Last Modified: Wed, 06 Sep 2023 22:40:27 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb56160de8c01873d42326860132a0b877e470be0ff76c774c04b542515c9e4a`  
		Last Modified: Wed, 06 Sep 2023 22:40:27 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine3.18`

```console
$ docker pull nats@sha256:36d34c59ed76472d9b3caafc5e3764b7a587498808efdd5178468f4efe8b4887
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:756a55661288407f688c52224ac8b12d008f0fec9343c68281b04bb59cbcc427
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9270382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbb9252d07acfbe3ac9083449c0fef74561021019d85c2993f5bce02c7a16201`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 23:19:53 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 23:19:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 23:19:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 23:19:55 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 23:19:55 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:19:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 23:19:55 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75fdd304ec17c2cf1f7629eefc922e04fae260b6d902e4fd42c81a5e5ce9d5dc`  
		Last Modified: Wed, 06 Sep 2023 23:20:32 GMT  
		Size: 5.9 MB (5867770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2863800c65f086f618bf3df0e7855997aea26ba27f4c759cf8bfae94da866bb`  
		Last Modified: Wed, 06 Sep 2023 23:20:31 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e32a641538132ed9885ca87c473fe9ff71415289c1f5276ba1157bb0760bd04`  
		Last Modified: Wed, 06 Sep 2023 23:20:31 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:e66fcde15a5b8028aed7cdd2e03392aa10c4a51c224e964f014eddc1c821433d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8749092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6e3524e57732f8e26091d551f1b5ce64405e4217d19f047345dc28a29a1b847`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 23:04:40 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 23:04:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 23:04:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 23:04:43 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 23:04:43 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:04:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 23:04:43 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a6e71bd2ab60e313e659b569f8c33e5e9dcfdb580c25af0f9c5e7eca59f92f`  
		Last Modified: Wed, 06 Sep 2023 23:05:08 GMT  
		Size: 5.6 MB (5603285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b94c778bbad17cc9be59c68102602e2e77462672d2e045f4713e80ce1cbb1c`  
		Last Modified: Wed, 06 Sep 2023 23:05:07 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b258e6095309f7819e72dd444d848fe600fb2e73b5bd12bd1e9a556a17bf56`  
		Last Modified: Wed, 06 Sep 2023 23:05:07 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:9ca6685d1ad99fa588f9d4dc05ffe27569ed660b735218fd38795568fe508c73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8492829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0271598ef211f3df61073ff64c769275b4bb72b68b984931c8a7af1706fe80c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 22:57:29 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 22:57:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 22:57:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 22:57:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 22:57:32 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:57:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 22:57:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1962026ec365b08ba406dd0e38e57c06dcd04f2225faffcc17883ed87716cdc8`  
		Last Modified: Wed, 06 Sep 2023 22:58:03 GMT  
		Size: 5.6 MB (5592351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578cf75378460664df525d3b5d1412e778f7b8cdc5f3c31207b3bbc2f6c074f5`  
		Last Modified: Wed, 06 Sep 2023 22:58:01 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64bf3e24d68a6cadd0880ce3163738934bf8e5b267923da68dd6922cd6b98a31`  
		Last Modified: Wed, 06 Sep 2023 22:58:01 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:51e884da4e764cc784998e4bc69bbbefa4f39420be30021b4a1074dc40604423
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8734219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c8cdff0ce493eb27f871f27f7ec452d1c36de63801fda0b331cd41067f858b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 22:39:45 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 22:39:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 22:39:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 22:39:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 22:39:47 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 22:39:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64353667b2ee68f04c527f8dcef72789d979435b90c5b8073485e6c2fcc5c3f7`  
		Last Modified: Wed, 06 Sep 2023 22:40:28 GMT  
		Size: 5.4 MB (5402455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540b41e481b61500ce8ed1c72cc5c0f937cabb489d0ba9de2dc2dad279696a28`  
		Last Modified: Wed, 06 Sep 2023 22:40:27 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb56160de8c01873d42326860132a0b877e470be0ff76c774c04b542515c9e4a`  
		Last Modified: Wed, 06 Sep 2023 22:40:27 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-linux`

```console
$ docker pull nats@sha256:488386bec6ea7b0822f48795e51ed1dd0b367e6e2fffe466d4f304e2fa628918
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-linux` - linux; amd64

```console
$ docker pull nats@sha256:2a08a0c1d913294be585667f17f76f028053f5bf47b9d317e5bc0e409011ed1e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5245282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3517f7b93c37103553431effcb0b5a8262feb87c3649b04249d86012c34a9761`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 20 Sep 2023 00:49:17 GMT
COPY file:acdb0e47969d6e334bcadb9c85dfef3166c764ff4ac55254185a04b1a6e8bbee in /nats-server 
# Wed, 20 Sep 2023 00:49:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 20 Sep 2023 00:49:17 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:49:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Sep 2023 00:49:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aac801db9a2a97942dde4494f98ce2d08c529a3af03ecb92f0b93426bbfd6419`  
		Last Modified: Wed, 06 Sep 2023 23:20:56 GMT  
		Size: 5.2 MB (5244773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1646134cd3aac5e501d3658b95fcfd870fb902c4c9591a801a5b370a5aa574`  
		Last Modified: Wed, 20 Sep 2023 00:50:09 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:4f09dbc6c43267500545fe441ec8057908d1b6bab5333c432c5e3d4c7ea0fd58
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4980014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:898dfa8e8c4c3e0c69c7c3aec16c90f1f6db172f3af0e7ff763b3bf8db42ed3c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Sep 2023 23:49:29 GMT
COPY file:51aacaba9769a3f16e0467be1fc8eb86122f6f3496e89e41b61e0038083ae308 in /nats-server 
# Tue, 19 Sep 2023 23:49:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Sep 2023 23:49:29 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Sep 2023 23:49:29 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Sep 2023 23:49:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6a6e165fccf6da77ad3b09408162fc7daaafe266b71dd5da8679594aa110a3a5`  
		Last Modified: Wed, 06 Sep 2023 23:05:32 GMT  
		Size: 5.0 MB (4979506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07c6021b659fa78c25ff92ad1e74c46e34c95c5e691ca45f27ced97ea7ef9e2`  
		Last Modified: Tue, 19 Sep 2023 23:50:15 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:64211266fe0d926796dae72e7484f5aebbdb77c7e7faa3fab3d01954fe03a82e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4970849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a40010bd31b571ac24ead3a8630fa80ce8609b0352d5dab096c6b72940be90a6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 20 Sep 2023 00:39:32 GMT
COPY file:aae670bb79c659968f632ae3be388af62614010873ced2a439475906dbb769c6 in /nats-server 
# Wed, 20 Sep 2023 00:39:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 20 Sep 2023 00:39:32 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:39:32 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Sep 2023 00:39:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:55b6dbad6639da13368cebb9688e8a5caaee29041e6b5e2e798201dfcf2b67ad`  
		Last Modified: Wed, 06 Sep 2023 22:58:23 GMT  
		Size: 5.0 MB (4970341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969097b6afede4aab7deed51f12918311993aadbe7075d4965c14497831f4a12`  
		Last Modified: Wed, 20 Sep 2023 00:40:29 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:91e7a991da679db1020b25a760298f6944a9ea917e9ae90f10d1d7de9381fec4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4778849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb1745f4f81f20c728e9276ed07416c88490859cdbed438bdcb68aa051eb586c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Sep 2023 23:42:56 GMT
COPY file:d6eca5c67de65d1a8a30a51ea7318b044949c77108b2fdccc5aa0054c068c196 in /nats-server 
# Tue, 19 Sep 2023 23:42:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Sep 2023 23:42:56 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Sep 2023 23:42:56 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Sep 2023 23:42:56 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:88e5ff7f26ea25c6d2ab092989d9372cb32b3e60880124facfcefd7d3f0b7591`  
		Last Modified: Wed, 06 Sep 2023 22:40:49 GMT  
		Size: 4.8 MB (4778340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2424880e07e944598022ff8713b5897eb59c72af17978f7a3f1afa42dd022088`  
		Last Modified: Tue, 19 Sep 2023 23:43:51 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver`

```console
$ docker pull nats@sha256:a040fc4874378f2c73b2d333916a89e39936f9fb0bef541e4bdf241c9eea6343
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `nats:2.9-nanoserver` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats@sha256:ef369c5330e436aca92b7521434dcad6019b82114a6095132bc5e4e582a93861
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109819053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0053513aeb5883341d4904ae9f696d46f6f79373919c304dc1199f0cde262ef4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Aug 2023 16:42:02 GMT
RUN Apply image 10.0.17763.4851
# Wed, 13 Sep 2023 05:08:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Sep 2023 05:08:05 GMT
RUN cmd /S /C #(nop) COPY file:393d7e944d1b6697a14f19f6cb9673d95da4e1a0fc9508b238325e94beebc857 in C:\nats-server.exe 
# Wed, 13 Sep 2023 05:08:05 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 13 Sep 2023 05:08:06 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 Sep 2023 05:08:07 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Sep 2023 05:08:07 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:17ba6b878467260559b72cb6f7e79c829eae67862a09efe87f6dc324f49fc086`  
		Last Modified: Tue, 12 Sep 2023 18:31:40 GMT  
		Size: 104.5 MB (104492504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9930674eb6676a1690e63a275d0da517ab8b8aeab7ccd20591f76f7c69a5`  
		Last Modified: Wed, 13 Sep 2023 05:08:48 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cf628408f2a1164bcd400567aa3cd56db3926c391837397914b8cd6c337369f`  
		Last Modified: Wed, 13 Sep 2023 05:08:47 GMT  
		Size: 5.3 MB (5320086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e6195a95c838cacd22627e342b84f22112007d2f4e70079c6de80beb6e7c45`  
		Last Modified: Wed, 13 Sep 2023 05:08:45 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c249fb3d5e5f1f8e0ef37e85a0cfaed40a4bb8df20e92e8937d686c2ec18fed`  
		Last Modified: Wed, 13 Sep 2023 05:08:45 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01b907719f9c8b285c36f7971a978e09c143bfa695bfcc5f46a9d56fd55458d`  
		Last Modified: Wed, 13 Sep 2023 05:08:45 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af083ba70a28322391995a59e841ea4478fe0d88eabbb83b4cfcbf20fab0cc4`  
		Last Modified: Wed, 13 Sep 2023 05:08:45 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver-1809`

```console
$ docker pull nats@sha256:a040fc4874378f2c73b2d333916a89e39936f9fb0bef541e4bdf241c9eea6343
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `nats:2.9-nanoserver-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats@sha256:ef369c5330e436aca92b7521434dcad6019b82114a6095132bc5e4e582a93861
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109819053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0053513aeb5883341d4904ae9f696d46f6f79373919c304dc1199f0cde262ef4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Aug 2023 16:42:02 GMT
RUN Apply image 10.0.17763.4851
# Wed, 13 Sep 2023 05:08:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Sep 2023 05:08:05 GMT
RUN cmd /S /C #(nop) COPY file:393d7e944d1b6697a14f19f6cb9673d95da4e1a0fc9508b238325e94beebc857 in C:\nats-server.exe 
# Wed, 13 Sep 2023 05:08:05 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 13 Sep 2023 05:08:06 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 Sep 2023 05:08:07 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Sep 2023 05:08:07 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:17ba6b878467260559b72cb6f7e79c829eae67862a09efe87f6dc324f49fc086`  
		Last Modified: Tue, 12 Sep 2023 18:31:40 GMT  
		Size: 104.5 MB (104492504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9930674eb6676a1690e63a275d0da517ab8b8aeab7ccd20591f76f7c69a5`  
		Last Modified: Wed, 13 Sep 2023 05:08:48 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cf628408f2a1164bcd400567aa3cd56db3926c391837397914b8cd6c337369f`  
		Last Modified: Wed, 13 Sep 2023 05:08:47 GMT  
		Size: 5.3 MB (5320086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e6195a95c838cacd22627e342b84f22112007d2f4e70079c6de80beb6e7c45`  
		Last Modified: Wed, 13 Sep 2023 05:08:45 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c249fb3d5e5f1f8e0ef37e85a0cfaed40a4bb8df20e92e8937d686c2ec18fed`  
		Last Modified: Wed, 13 Sep 2023 05:08:45 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01b907719f9c8b285c36f7971a978e09c143bfa695bfcc5f46a9d56fd55458d`  
		Last Modified: Wed, 13 Sep 2023 05:08:45 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af083ba70a28322391995a59e841ea4478fe0d88eabbb83b4cfcbf20fab0cc4`  
		Last Modified: Wed, 13 Sep 2023 05:08:45 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-scratch`

```console
$ docker pull nats@sha256:488386bec6ea7b0822f48795e51ed1dd0b367e6e2fffe466d4f304e2fa628918
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-scratch` - linux; amd64

```console
$ docker pull nats@sha256:2a08a0c1d913294be585667f17f76f028053f5bf47b9d317e5bc0e409011ed1e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5245282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3517f7b93c37103553431effcb0b5a8262feb87c3649b04249d86012c34a9761`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 20 Sep 2023 00:49:17 GMT
COPY file:acdb0e47969d6e334bcadb9c85dfef3166c764ff4ac55254185a04b1a6e8bbee in /nats-server 
# Wed, 20 Sep 2023 00:49:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 20 Sep 2023 00:49:17 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:49:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Sep 2023 00:49:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aac801db9a2a97942dde4494f98ce2d08c529a3af03ecb92f0b93426bbfd6419`  
		Last Modified: Wed, 06 Sep 2023 23:20:56 GMT  
		Size: 5.2 MB (5244773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1646134cd3aac5e501d3658b95fcfd870fb902c4c9591a801a5b370a5aa574`  
		Last Modified: Wed, 20 Sep 2023 00:50:09 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:4f09dbc6c43267500545fe441ec8057908d1b6bab5333c432c5e3d4c7ea0fd58
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4980014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:898dfa8e8c4c3e0c69c7c3aec16c90f1f6db172f3af0e7ff763b3bf8db42ed3c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Sep 2023 23:49:29 GMT
COPY file:51aacaba9769a3f16e0467be1fc8eb86122f6f3496e89e41b61e0038083ae308 in /nats-server 
# Tue, 19 Sep 2023 23:49:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Sep 2023 23:49:29 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Sep 2023 23:49:29 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Sep 2023 23:49:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6a6e165fccf6da77ad3b09408162fc7daaafe266b71dd5da8679594aa110a3a5`  
		Last Modified: Wed, 06 Sep 2023 23:05:32 GMT  
		Size: 5.0 MB (4979506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07c6021b659fa78c25ff92ad1e74c46e34c95c5e691ca45f27ced97ea7ef9e2`  
		Last Modified: Tue, 19 Sep 2023 23:50:15 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:64211266fe0d926796dae72e7484f5aebbdb77c7e7faa3fab3d01954fe03a82e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4970849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a40010bd31b571ac24ead3a8630fa80ce8609b0352d5dab096c6b72940be90a6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 20 Sep 2023 00:39:32 GMT
COPY file:aae670bb79c659968f632ae3be388af62614010873ced2a439475906dbb769c6 in /nats-server 
# Wed, 20 Sep 2023 00:39:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 20 Sep 2023 00:39:32 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:39:32 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Sep 2023 00:39:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:55b6dbad6639da13368cebb9688e8a5caaee29041e6b5e2e798201dfcf2b67ad`  
		Last Modified: Wed, 06 Sep 2023 22:58:23 GMT  
		Size: 5.0 MB (4970341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969097b6afede4aab7deed51f12918311993aadbe7075d4965c14497831f4a12`  
		Last Modified: Wed, 20 Sep 2023 00:40:29 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:91e7a991da679db1020b25a760298f6944a9ea917e9ae90f10d1d7de9381fec4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4778849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb1745f4f81f20c728e9276ed07416c88490859cdbed438bdcb68aa051eb586c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Sep 2023 23:42:56 GMT
COPY file:d6eca5c67de65d1a8a30a51ea7318b044949c77108b2fdccc5aa0054c068c196 in /nats-server 
# Tue, 19 Sep 2023 23:42:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Sep 2023 23:42:56 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Sep 2023 23:42:56 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Sep 2023 23:42:56 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:88e5ff7f26ea25c6d2ab092989d9372cb32b3e60880124facfcefd7d3f0b7591`  
		Last Modified: Wed, 06 Sep 2023 22:40:49 GMT  
		Size: 4.8 MB (4778340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2424880e07e944598022ff8713b5897eb59c72af17978f7a3f1afa42dd022088`  
		Last Modified: Tue, 19 Sep 2023 23:43:51 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore`

```console
$ docker pull nats@sha256:0d1237c42b0bf510367a68f73790bafd41d3e4dba95502ecf7d630eb6dcf0694
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `nats:2.9-windowsservercore` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats@sha256:4bc9d7dc99d75f7813148b82653c884ac51975085d49de22b68ac981bf1b3c40
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2022365856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5f7856c543b220cf294996bece7566b5515805212fc38127b1450f60b3e3ba5`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 03:56:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Sep 2023 05:05:36 GMT
ENV NATS_DOCKERIZED=1
# Wed, 13 Sep 2023 05:05:36 GMT
ENV NATS_SERVER=2.9.22
# Wed, 13 Sep 2023 05:05:37 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.22/nats-server-v2.9.22-windows-amd64.zip
# Wed, 13 Sep 2023 05:05:38 GMT
ENV NATS_SERVER_SHASUM=e91db73b02bd4dca3eb7a4bf32e29763450b08d593f73e87d0a6b70102dea0d4
# Wed, 13 Sep 2023 05:06:28 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 Sep 2023 05:07:52 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 13 Sep 2023 05:07:52 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 13 Sep 2023 05:07:53 GMT
EXPOSE 4222 6222 8222
# Wed, 13 Sep 2023 05:07:54 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Sep 2023 05:07:55 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b21bbf840142288ae2bce3465085b591133cf10f78f7dda43277db4838332d8`  
		Last Modified: Wed, 13 Sep 2023 04:36:45 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54f616fe064e9d4e73bf2aec9a4fe9c58837ec84c2fc998a54ab7a77b52e109`  
		Last Modified: Wed, 13 Sep 2023 05:08:32 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e138a75d8a68c57acda5ac3d2a5ea38cfcd91aeeac6e996187886cdc4fe512b`  
		Last Modified: Wed, 13 Sep 2023 05:08:31 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ba6b3e055f188fc0c938c464d3df287b87b4ebd990c6d3023e4043e9475882b`  
		Last Modified: Wed, 13 Sep 2023 05:08:30 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733d1091bb5b201027155aa6154441b33e21f06c80c98e5502f0ea97d3e6ac36`  
		Last Modified: Wed, 13 Sep 2023 05:08:30 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98cf75715be616bda4fd455e8842d5c47e6361520831c79994aac63897f074a6`  
		Last Modified: Wed, 13 Sep 2023 05:08:30 GMT  
		Size: 242.8 KB (242766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3267078f67f5f3fb7955bda584f1a858622791ed81e9c2e45ac79383c6c3795`  
		Last Modified: Wed, 13 Sep 2023 05:08:30 GMT  
		Size: 5.8 MB (5779913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd81aab1223d4ac5fade6bcbff4e433f5a038988f73089bb43aff8b974c715a2`  
		Last Modified: Wed, 13 Sep 2023 05:08:28 GMT  
		Size: 2.0 KB (1985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a790db19f2a0d625636fa4d186b3b076500c592809d8b95c7a725e0c46a094`  
		Last Modified: Wed, 13 Sep 2023 05:08:28 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4edbf9880281abc4bccc4d818ad299ce3cd5ad235e1cb033fbc49b3096f3a7`  
		Last Modified: Wed, 13 Sep 2023 05:08:28 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c05fad63f054ab864e4484c552a76f82c3bf9e322da181d03f63a597755912`  
		Last Modified: Wed, 13 Sep 2023 05:08:28 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore-1809`

```console
$ docker pull nats@sha256:0d1237c42b0bf510367a68f73790bafd41d3e4dba95502ecf7d630eb6dcf0694
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `nats:2.9-windowsservercore-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats@sha256:4bc9d7dc99d75f7813148b82653c884ac51975085d49de22b68ac981bf1b3c40
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2022365856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5f7856c543b220cf294996bece7566b5515805212fc38127b1450f60b3e3ba5`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 03:56:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Sep 2023 05:05:36 GMT
ENV NATS_DOCKERIZED=1
# Wed, 13 Sep 2023 05:05:36 GMT
ENV NATS_SERVER=2.9.22
# Wed, 13 Sep 2023 05:05:37 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.22/nats-server-v2.9.22-windows-amd64.zip
# Wed, 13 Sep 2023 05:05:38 GMT
ENV NATS_SERVER_SHASUM=e91db73b02bd4dca3eb7a4bf32e29763450b08d593f73e87d0a6b70102dea0d4
# Wed, 13 Sep 2023 05:06:28 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 Sep 2023 05:07:52 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 13 Sep 2023 05:07:52 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 13 Sep 2023 05:07:53 GMT
EXPOSE 4222 6222 8222
# Wed, 13 Sep 2023 05:07:54 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Sep 2023 05:07:55 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b21bbf840142288ae2bce3465085b591133cf10f78f7dda43277db4838332d8`  
		Last Modified: Wed, 13 Sep 2023 04:36:45 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54f616fe064e9d4e73bf2aec9a4fe9c58837ec84c2fc998a54ab7a77b52e109`  
		Last Modified: Wed, 13 Sep 2023 05:08:32 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e138a75d8a68c57acda5ac3d2a5ea38cfcd91aeeac6e996187886cdc4fe512b`  
		Last Modified: Wed, 13 Sep 2023 05:08:31 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ba6b3e055f188fc0c938c464d3df287b87b4ebd990c6d3023e4043e9475882b`  
		Last Modified: Wed, 13 Sep 2023 05:08:30 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733d1091bb5b201027155aa6154441b33e21f06c80c98e5502f0ea97d3e6ac36`  
		Last Modified: Wed, 13 Sep 2023 05:08:30 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98cf75715be616bda4fd455e8842d5c47e6361520831c79994aac63897f074a6`  
		Last Modified: Wed, 13 Sep 2023 05:08:30 GMT  
		Size: 242.8 KB (242766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3267078f67f5f3fb7955bda584f1a858622791ed81e9c2e45ac79383c6c3795`  
		Last Modified: Wed, 13 Sep 2023 05:08:30 GMT  
		Size: 5.8 MB (5779913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd81aab1223d4ac5fade6bcbff4e433f5a038988f73089bb43aff8b974c715a2`  
		Last Modified: Wed, 13 Sep 2023 05:08:28 GMT  
		Size: 2.0 KB (1985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a790db19f2a0d625636fa4d186b3b076500c592809d8b95c7a725e0c46a094`  
		Last Modified: Wed, 13 Sep 2023 05:08:28 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4edbf9880281abc4bccc4d818ad299ce3cd5ad235e1cb033fbc49b3096f3a7`  
		Last Modified: Wed, 13 Sep 2023 05:08:28 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c05fad63f054ab864e4484c552a76f82c3bf9e322da181d03f63a597755912`  
		Last Modified: Wed, 13 Sep 2023 05:08:28 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.22`

```console
$ docker pull nats@sha256:488386bec6ea7b0822f48795e51ed1dd0b367e6e2fffe466d4f304e2fa628918
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.22` - linux; amd64

```console
$ docker pull nats@sha256:2a08a0c1d913294be585667f17f76f028053f5bf47b9d317e5bc0e409011ed1e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5245282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3517f7b93c37103553431effcb0b5a8262feb87c3649b04249d86012c34a9761`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 20 Sep 2023 00:49:17 GMT
COPY file:acdb0e47969d6e334bcadb9c85dfef3166c764ff4ac55254185a04b1a6e8bbee in /nats-server 
# Wed, 20 Sep 2023 00:49:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 20 Sep 2023 00:49:17 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:49:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Sep 2023 00:49:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aac801db9a2a97942dde4494f98ce2d08c529a3af03ecb92f0b93426bbfd6419`  
		Last Modified: Wed, 06 Sep 2023 23:20:56 GMT  
		Size: 5.2 MB (5244773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1646134cd3aac5e501d3658b95fcfd870fb902c4c9591a801a5b370a5aa574`  
		Last Modified: Wed, 20 Sep 2023 00:50:09 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.22` - linux; arm variant v6

```console
$ docker pull nats@sha256:4f09dbc6c43267500545fe441ec8057908d1b6bab5333c432c5e3d4c7ea0fd58
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4980014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:898dfa8e8c4c3e0c69c7c3aec16c90f1f6db172f3af0e7ff763b3bf8db42ed3c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Sep 2023 23:49:29 GMT
COPY file:51aacaba9769a3f16e0467be1fc8eb86122f6f3496e89e41b61e0038083ae308 in /nats-server 
# Tue, 19 Sep 2023 23:49:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Sep 2023 23:49:29 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Sep 2023 23:49:29 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Sep 2023 23:49:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6a6e165fccf6da77ad3b09408162fc7daaafe266b71dd5da8679594aa110a3a5`  
		Last Modified: Wed, 06 Sep 2023 23:05:32 GMT  
		Size: 5.0 MB (4979506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07c6021b659fa78c25ff92ad1e74c46e34c95c5e691ca45f27ced97ea7ef9e2`  
		Last Modified: Tue, 19 Sep 2023 23:50:15 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.22` - linux; arm variant v7

```console
$ docker pull nats@sha256:64211266fe0d926796dae72e7484f5aebbdb77c7e7faa3fab3d01954fe03a82e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4970849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a40010bd31b571ac24ead3a8630fa80ce8609b0352d5dab096c6b72940be90a6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 20 Sep 2023 00:39:32 GMT
COPY file:aae670bb79c659968f632ae3be388af62614010873ced2a439475906dbb769c6 in /nats-server 
# Wed, 20 Sep 2023 00:39:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 20 Sep 2023 00:39:32 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:39:32 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Sep 2023 00:39:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:55b6dbad6639da13368cebb9688e8a5caaee29041e6b5e2e798201dfcf2b67ad`  
		Last Modified: Wed, 06 Sep 2023 22:58:23 GMT  
		Size: 5.0 MB (4970341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969097b6afede4aab7deed51f12918311993aadbe7075d4965c14497831f4a12`  
		Last Modified: Wed, 20 Sep 2023 00:40:29 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.22` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:91e7a991da679db1020b25a760298f6944a9ea917e9ae90f10d1d7de9381fec4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4778849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb1745f4f81f20c728e9276ed07416c88490859cdbed438bdcb68aa051eb586c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Sep 2023 23:42:56 GMT
COPY file:d6eca5c67de65d1a8a30a51ea7318b044949c77108b2fdccc5aa0054c068c196 in /nats-server 
# Tue, 19 Sep 2023 23:42:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Sep 2023 23:42:56 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Sep 2023 23:42:56 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Sep 2023 23:42:56 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:88e5ff7f26ea25c6d2ab092989d9372cb32b3e60880124facfcefd7d3f0b7591`  
		Last Modified: Wed, 06 Sep 2023 22:40:49 GMT  
		Size: 4.8 MB (4778340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2424880e07e944598022ff8713b5897eb59c72af17978f7a3f1afa42dd022088`  
		Last Modified: Tue, 19 Sep 2023 23:43:51 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.22-alpine`

```console
$ docker pull nats@sha256:36d34c59ed76472d9b3caafc5e3764b7a587498808efdd5178468f4efe8b4887
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.22-alpine` - linux; amd64

```console
$ docker pull nats@sha256:756a55661288407f688c52224ac8b12d008f0fec9343c68281b04bb59cbcc427
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9270382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbb9252d07acfbe3ac9083449c0fef74561021019d85c2993f5bce02c7a16201`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 23:19:53 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 23:19:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 23:19:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 23:19:55 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 23:19:55 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:19:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 23:19:55 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75fdd304ec17c2cf1f7629eefc922e04fae260b6d902e4fd42c81a5e5ce9d5dc`  
		Last Modified: Wed, 06 Sep 2023 23:20:32 GMT  
		Size: 5.9 MB (5867770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2863800c65f086f618bf3df0e7855997aea26ba27f4c759cf8bfae94da866bb`  
		Last Modified: Wed, 06 Sep 2023 23:20:31 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e32a641538132ed9885ca87c473fe9ff71415289c1f5276ba1157bb0760bd04`  
		Last Modified: Wed, 06 Sep 2023 23:20:31 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.22-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:e66fcde15a5b8028aed7cdd2e03392aa10c4a51c224e964f014eddc1c821433d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8749092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6e3524e57732f8e26091d551f1b5ce64405e4217d19f047345dc28a29a1b847`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 23:04:40 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 23:04:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 23:04:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 23:04:43 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 23:04:43 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:04:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 23:04:43 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a6e71bd2ab60e313e659b569f8c33e5e9dcfdb580c25af0f9c5e7eca59f92f`  
		Last Modified: Wed, 06 Sep 2023 23:05:08 GMT  
		Size: 5.6 MB (5603285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b94c778bbad17cc9be59c68102602e2e77462672d2e045f4713e80ce1cbb1c`  
		Last Modified: Wed, 06 Sep 2023 23:05:07 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b258e6095309f7819e72dd444d848fe600fb2e73b5bd12bd1e9a556a17bf56`  
		Last Modified: Wed, 06 Sep 2023 23:05:07 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.22-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:9ca6685d1ad99fa588f9d4dc05ffe27569ed660b735218fd38795568fe508c73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8492829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0271598ef211f3df61073ff64c769275b4bb72b68b984931c8a7af1706fe80c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 22:57:29 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 22:57:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 22:57:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 22:57:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 22:57:32 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:57:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 22:57:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1962026ec365b08ba406dd0e38e57c06dcd04f2225faffcc17883ed87716cdc8`  
		Last Modified: Wed, 06 Sep 2023 22:58:03 GMT  
		Size: 5.6 MB (5592351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578cf75378460664df525d3b5d1412e778f7b8cdc5f3c31207b3bbc2f6c074f5`  
		Last Modified: Wed, 06 Sep 2023 22:58:01 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64bf3e24d68a6cadd0880ce3163738934bf8e5b267923da68dd6922cd6b98a31`  
		Last Modified: Wed, 06 Sep 2023 22:58:01 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.22-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:51e884da4e764cc784998e4bc69bbbefa4f39420be30021b4a1074dc40604423
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8734219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c8cdff0ce493eb27f871f27f7ec452d1c36de63801fda0b331cd41067f858b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 22:39:45 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 22:39:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 22:39:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 22:39:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 22:39:47 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 22:39:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64353667b2ee68f04c527f8dcef72789d979435b90c5b8073485e6c2fcc5c3f7`  
		Last Modified: Wed, 06 Sep 2023 22:40:28 GMT  
		Size: 5.4 MB (5402455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540b41e481b61500ce8ed1c72cc5c0f937cabb489d0ba9de2dc2dad279696a28`  
		Last Modified: Wed, 06 Sep 2023 22:40:27 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb56160de8c01873d42326860132a0b877e470be0ff76c774c04b542515c9e4a`  
		Last Modified: Wed, 06 Sep 2023 22:40:27 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.22-alpine3.18`

```console
$ docker pull nats@sha256:36d34c59ed76472d9b3caafc5e3764b7a587498808efdd5178468f4efe8b4887
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.22-alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:756a55661288407f688c52224ac8b12d008f0fec9343c68281b04bb59cbcc427
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9270382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbb9252d07acfbe3ac9083449c0fef74561021019d85c2993f5bce02c7a16201`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 23:19:53 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 23:19:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 23:19:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 23:19:55 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 23:19:55 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:19:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 23:19:55 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75fdd304ec17c2cf1f7629eefc922e04fae260b6d902e4fd42c81a5e5ce9d5dc`  
		Last Modified: Wed, 06 Sep 2023 23:20:32 GMT  
		Size: 5.9 MB (5867770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2863800c65f086f618bf3df0e7855997aea26ba27f4c759cf8bfae94da866bb`  
		Last Modified: Wed, 06 Sep 2023 23:20:31 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e32a641538132ed9885ca87c473fe9ff71415289c1f5276ba1157bb0760bd04`  
		Last Modified: Wed, 06 Sep 2023 23:20:31 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.22-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:e66fcde15a5b8028aed7cdd2e03392aa10c4a51c224e964f014eddc1c821433d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8749092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6e3524e57732f8e26091d551f1b5ce64405e4217d19f047345dc28a29a1b847`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 23:04:40 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 23:04:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 23:04:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 23:04:43 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 23:04:43 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:04:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 23:04:43 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a6e71bd2ab60e313e659b569f8c33e5e9dcfdb580c25af0f9c5e7eca59f92f`  
		Last Modified: Wed, 06 Sep 2023 23:05:08 GMT  
		Size: 5.6 MB (5603285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b94c778bbad17cc9be59c68102602e2e77462672d2e045f4713e80ce1cbb1c`  
		Last Modified: Wed, 06 Sep 2023 23:05:07 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b258e6095309f7819e72dd444d848fe600fb2e73b5bd12bd1e9a556a17bf56`  
		Last Modified: Wed, 06 Sep 2023 23:05:07 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.22-alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:9ca6685d1ad99fa588f9d4dc05ffe27569ed660b735218fd38795568fe508c73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8492829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0271598ef211f3df61073ff64c769275b4bb72b68b984931c8a7af1706fe80c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 22:57:29 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 22:57:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 22:57:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 22:57:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 22:57:32 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:57:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 22:57:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1962026ec365b08ba406dd0e38e57c06dcd04f2225faffcc17883ed87716cdc8`  
		Last Modified: Wed, 06 Sep 2023 22:58:03 GMT  
		Size: 5.6 MB (5592351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578cf75378460664df525d3b5d1412e778f7b8cdc5f3c31207b3bbc2f6c074f5`  
		Last Modified: Wed, 06 Sep 2023 22:58:01 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64bf3e24d68a6cadd0880ce3163738934bf8e5b267923da68dd6922cd6b98a31`  
		Last Modified: Wed, 06 Sep 2023 22:58:01 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.22-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:51e884da4e764cc784998e4bc69bbbefa4f39420be30021b4a1074dc40604423
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8734219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c8cdff0ce493eb27f871f27f7ec452d1c36de63801fda0b331cd41067f858b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 22:39:45 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 22:39:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 22:39:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 22:39:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 22:39:47 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 22:39:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64353667b2ee68f04c527f8dcef72789d979435b90c5b8073485e6c2fcc5c3f7`  
		Last Modified: Wed, 06 Sep 2023 22:40:28 GMT  
		Size: 5.4 MB (5402455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540b41e481b61500ce8ed1c72cc5c0f937cabb489d0ba9de2dc2dad279696a28`  
		Last Modified: Wed, 06 Sep 2023 22:40:27 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb56160de8c01873d42326860132a0b877e470be0ff76c774c04b542515c9e4a`  
		Last Modified: Wed, 06 Sep 2023 22:40:27 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.22-linux`

```console
$ docker pull nats@sha256:488386bec6ea7b0822f48795e51ed1dd0b367e6e2fffe466d4f304e2fa628918
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.22-linux` - linux; amd64

```console
$ docker pull nats@sha256:2a08a0c1d913294be585667f17f76f028053f5bf47b9d317e5bc0e409011ed1e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5245282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3517f7b93c37103553431effcb0b5a8262feb87c3649b04249d86012c34a9761`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 20 Sep 2023 00:49:17 GMT
COPY file:acdb0e47969d6e334bcadb9c85dfef3166c764ff4ac55254185a04b1a6e8bbee in /nats-server 
# Wed, 20 Sep 2023 00:49:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 20 Sep 2023 00:49:17 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:49:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Sep 2023 00:49:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aac801db9a2a97942dde4494f98ce2d08c529a3af03ecb92f0b93426bbfd6419`  
		Last Modified: Wed, 06 Sep 2023 23:20:56 GMT  
		Size: 5.2 MB (5244773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1646134cd3aac5e501d3658b95fcfd870fb902c4c9591a801a5b370a5aa574`  
		Last Modified: Wed, 20 Sep 2023 00:50:09 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.22-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:4f09dbc6c43267500545fe441ec8057908d1b6bab5333c432c5e3d4c7ea0fd58
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4980014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:898dfa8e8c4c3e0c69c7c3aec16c90f1f6db172f3af0e7ff763b3bf8db42ed3c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Sep 2023 23:49:29 GMT
COPY file:51aacaba9769a3f16e0467be1fc8eb86122f6f3496e89e41b61e0038083ae308 in /nats-server 
# Tue, 19 Sep 2023 23:49:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Sep 2023 23:49:29 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Sep 2023 23:49:29 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Sep 2023 23:49:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6a6e165fccf6da77ad3b09408162fc7daaafe266b71dd5da8679594aa110a3a5`  
		Last Modified: Wed, 06 Sep 2023 23:05:32 GMT  
		Size: 5.0 MB (4979506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07c6021b659fa78c25ff92ad1e74c46e34c95c5e691ca45f27ced97ea7ef9e2`  
		Last Modified: Tue, 19 Sep 2023 23:50:15 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.22-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:64211266fe0d926796dae72e7484f5aebbdb77c7e7faa3fab3d01954fe03a82e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4970849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a40010bd31b571ac24ead3a8630fa80ce8609b0352d5dab096c6b72940be90a6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 20 Sep 2023 00:39:32 GMT
COPY file:aae670bb79c659968f632ae3be388af62614010873ced2a439475906dbb769c6 in /nats-server 
# Wed, 20 Sep 2023 00:39:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 20 Sep 2023 00:39:32 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:39:32 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Sep 2023 00:39:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:55b6dbad6639da13368cebb9688e8a5caaee29041e6b5e2e798201dfcf2b67ad`  
		Last Modified: Wed, 06 Sep 2023 22:58:23 GMT  
		Size: 5.0 MB (4970341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969097b6afede4aab7deed51f12918311993aadbe7075d4965c14497831f4a12`  
		Last Modified: Wed, 20 Sep 2023 00:40:29 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.22-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:91e7a991da679db1020b25a760298f6944a9ea917e9ae90f10d1d7de9381fec4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4778849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb1745f4f81f20c728e9276ed07416c88490859cdbed438bdcb68aa051eb586c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Sep 2023 23:42:56 GMT
COPY file:d6eca5c67de65d1a8a30a51ea7318b044949c77108b2fdccc5aa0054c068c196 in /nats-server 
# Tue, 19 Sep 2023 23:42:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Sep 2023 23:42:56 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Sep 2023 23:42:56 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Sep 2023 23:42:56 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:88e5ff7f26ea25c6d2ab092989d9372cb32b3e60880124facfcefd7d3f0b7591`  
		Last Modified: Wed, 06 Sep 2023 22:40:49 GMT  
		Size: 4.8 MB (4778340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2424880e07e944598022ff8713b5897eb59c72af17978f7a3f1afa42dd022088`  
		Last Modified: Tue, 19 Sep 2023 23:43:51 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.22-nanoserver`

```console
$ docker pull nats@sha256:a040fc4874378f2c73b2d333916a89e39936f9fb0bef541e4bdf241c9eea6343
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `nats:2.9.22-nanoserver` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats@sha256:ef369c5330e436aca92b7521434dcad6019b82114a6095132bc5e4e582a93861
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109819053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0053513aeb5883341d4904ae9f696d46f6f79373919c304dc1199f0cde262ef4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Aug 2023 16:42:02 GMT
RUN Apply image 10.0.17763.4851
# Wed, 13 Sep 2023 05:08:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Sep 2023 05:08:05 GMT
RUN cmd /S /C #(nop) COPY file:393d7e944d1b6697a14f19f6cb9673d95da4e1a0fc9508b238325e94beebc857 in C:\nats-server.exe 
# Wed, 13 Sep 2023 05:08:05 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 13 Sep 2023 05:08:06 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 Sep 2023 05:08:07 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Sep 2023 05:08:07 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:17ba6b878467260559b72cb6f7e79c829eae67862a09efe87f6dc324f49fc086`  
		Last Modified: Tue, 12 Sep 2023 18:31:40 GMT  
		Size: 104.5 MB (104492504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9930674eb6676a1690e63a275d0da517ab8b8aeab7ccd20591f76f7c69a5`  
		Last Modified: Wed, 13 Sep 2023 05:08:48 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cf628408f2a1164bcd400567aa3cd56db3926c391837397914b8cd6c337369f`  
		Last Modified: Wed, 13 Sep 2023 05:08:47 GMT  
		Size: 5.3 MB (5320086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e6195a95c838cacd22627e342b84f22112007d2f4e70079c6de80beb6e7c45`  
		Last Modified: Wed, 13 Sep 2023 05:08:45 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c249fb3d5e5f1f8e0ef37e85a0cfaed40a4bb8df20e92e8937d686c2ec18fed`  
		Last Modified: Wed, 13 Sep 2023 05:08:45 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01b907719f9c8b285c36f7971a978e09c143bfa695bfcc5f46a9d56fd55458d`  
		Last Modified: Wed, 13 Sep 2023 05:08:45 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af083ba70a28322391995a59e841ea4478fe0d88eabbb83b4cfcbf20fab0cc4`  
		Last Modified: Wed, 13 Sep 2023 05:08:45 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.22-nanoserver-1809`

```console
$ docker pull nats@sha256:a040fc4874378f2c73b2d333916a89e39936f9fb0bef541e4bdf241c9eea6343
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `nats:2.9.22-nanoserver-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats@sha256:ef369c5330e436aca92b7521434dcad6019b82114a6095132bc5e4e582a93861
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109819053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0053513aeb5883341d4904ae9f696d46f6f79373919c304dc1199f0cde262ef4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Aug 2023 16:42:02 GMT
RUN Apply image 10.0.17763.4851
# Wed, 13 Sep 2023 05:08:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Sep 2023 05:08:05 GMT
RUN cmd /S /C #(nop) COPY file:393d7e944d1b6697a14f19f6cb9673d95da4e1a0fc9508b238325e94beebc857 in C:\nats-server.exe 
# Wed, 13 Sep 2023 05:08:05 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 13 Sep 2023 05:08:06 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 Sep 2023 05:08:07 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Sep 2023 05:08:07 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:17ba6b878467260559b72cb6f7e79c829eae67862a09efe87f6dc324f49fc086`  
		Last Modified: Tue, 12 Sep 2023 18:31:40 GMT  
		Size: 104.5 MB (104492504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9930674eb6676a1690e63a275d0da517ab8b8aeab7ccd20591f76f7c69a5`  
		Last Modified: Wed, 13 Sep 2023 05:08:48 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cf628408f2a1164bcd400567aa3cd56db3926c391837397914b8cd6c337369f`  
		Last Modified: Wed, 13 Sep 2023 05:08:47 GMT  
		Size: 5.3 MB (5320086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e6195a95c838cacd22627e342b84f22112007d2f4e70079c6de80beb6e7c45`  
		Last Modified: Wed, 13 Sep 2023 05:08:45 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c249fb3d5e5f1f8e0ef37e85a0cfaed40a4bb8df20e92e8937d686c2ec18fed`  
		Last Modified: Wed, 13 Sep 2023 05:08:45 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01b907719f9c8b285c36f7971a978e09c143bfa695bfcc5f46a9d56fd55458d`  
		Last Modified: Wed, 13 Sep 2023 05:08:45 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af083ba70a28322391995a59e841ea4478fe0d88eabbb83b4cfcbf20fab0cc4`  
		Last Modified: Wed, 13 Sep 2023 05:08:45 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.22-scratch`

```console
$ docker pull nats@sha256:488386bec6ea7b0822f48795e51ed1dd0b367e6e2fffe466d4f304e2fa628918
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.22-scratch` - linux; amd64

```console
$ docker pull nats@sha256:2a08a0c1d913294be585667f17f76f028053f5bf47b9d317e5bc0e409011ed1e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5245282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3517f7b93c37103553431effcb0b5a8262feb87c3649b04249d86012c34a9761`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 20 Sep 2023 00:49:17 GMT
COPY file:acdb0e47969d6e334bcadb9c85dfef3166c764ff4ac55254185a04b1a6e8bbee in /nats-server 
# Wed, 20 Sep 2023 00:49:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 20 Sep 2023 00:49:17 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:49:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Sep 2023 00:49:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aac801db9a2a97942dde4494f98ce2d08c529a3af03ecb92f0b93426bbfd6419`  
		Last Modified: Wed, 06 Sep 2023 23:20:56 GMT  
		Size: 5.2 MB (5244773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1646134cd3aac5e501d3658b95fcfd870fb902c4c9591a801a5b370a5aa574`  
		Last Modified: Wed, 20 Sep 2023 00:50:09 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.22-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:4f09dbc6c43267500545fe441ec8057908d1b6bab5333c432c5e3d4c7ea0fd58
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4980014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:898dfa8e8c4c3e0c69c7c3aec16c90f1f6db172f3af0e7ff763b3bf8db42ed3c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Sep 2023 23:49:29 GMT
COPY file:51aacaba9769a3f16e0467be1fc8eb86122f6f3496e89e41b61e0038083ae308 in /nats-server 
# Tue, 19 Sep 2023 23:49:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Sep 2023 23:49:29 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Sep 2023 23:49:29 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Sep 2023 23:49:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6a6e165fccf6da77ad3b09408162fc7daaafe266b71dd5da8679594aa110a3a5`  
		Last Modified: Wed, 06 Sep 2023 23:05:32 GMT  
		Size: 5.0 MB (4979506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07c6021b659fa78c25ff92ad1e74c46e34c95c5e691ca45f27ced97ea7ef9e2`  
		Last Modified: Tue, 19 Sep 2023 23:50:15 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.22-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:64211266fe0d926796dae72e7484f5aebbdb77c7e7faa3fab3d01954fe03a82e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4970849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a40010bd31b571ac24ead3a8630fa80ce8609b0352d5dab096c6b72940be90a6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 20 Sep 2023 00:39:32 GMT
COPY file:aae670bb79c659968f632ae3be388af62614010873ced2a439475906dbb769c6 in /nats-server 
# Wed, 20 Sep 2023 00:39:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 20 Sep 2023 00:39:32 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:39:32 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Sep 2023 00:39:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:55b6dbad6639da13368cebb9688e8a5caaee29041e6b5e2e798201dfcf2b67ad`  
		Last Modified: Wed, 06 Sep 2023 22:58:23 GMT  
		Size: 5.0 MB (4970341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969097b6afede4aab7deed51f12918311993aadbe7075d4965c14497831f4a12`  
		Last Modified: Wed, 20 Sep 2023 00:40:29 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.22-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:91e7a991da679db1020b25a760298f6944a9ea917e9ae90f10d1d7de9381fec4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4778849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb1745f4f81f20c728e9276ed07416c88490859cdbed438bdcb68aa051eb586c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Sep 2023 23:42:56 GMT
COPY file:d6eca5c67de65d1a8a30a51ea7318b044949c77108b2fdccc5aa0054c068c196 in /nats-server 
# Tue, 19 Sep 2023 23:42:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Sep 2023 23:42:56 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Sep 2023 23:42:56 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Sep 2023 23:42:56 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:88e5ff7f26ea25c6d2ab092989d9372cb32b3e60880124facfcefd7d3f0b7591`  
		Last Modified: Wed, 06 Sep 2023 22:40:49 GMT  
		Size: 4.8 MB (4778340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2424880e07e944598022ff8713b5897eb59c72af17978f7a3f1afa42dd022088`  
		Last Modified: Tue, 19 Sep 2023 23:43:51 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.22-windowsservercore`

```console
$ docker pull nats@sha256:0d1237c42b0bf510367a68f73790bafd41d3e4dba95502ecf7d630eb6dcf0694
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `nats:2.9.22-windowsservercore` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats@sha256:4bc9d7dc99d75f7813148b82653c884ac51975085d49de22b68ac981bf1b3c40
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2022365856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5f7856c543b220cf294996bece7566b5515805212fc38127b1450f60b3e3ba5`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 03:56:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Sep 2023 05:05:36 GMT
ENV NATS_DOCKERIZED=1
# Wed, 13 Sep 2023 05:05:36 GMT
ENV NATS_SERVER=2.9.22
# Wed, 13 Sep 2023 05:05:37 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.22/nats-server-v2.9.22-windows-amd64.zip
# Wed, 13 Sep 2023 05:05:38 GMT
ENV NATS_SERVER_SHASUM=e91db73b02bd4dca3eb7a4bf32e29763450b08d593f73e87d0a6b70102dea0d4
# Wed, 13 Sep 2023 05:06:28 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 Sep 2023 05:07:52 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 13 Sep 2023 05:07:52 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 13 Sep 2023 05:07:53 GMT
EXPOSE 4222 6222 8222
# Wed, 13 Sep 2023 05:07:54 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Sep 2023 05:07:55 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b21bbf840142288ae2bce3465085b591133cf10f78f7dda43277db4838332d8`  
		Last Modified: Wed, 13 Sep 2023 04:36:45 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54f616fe064e9d4e73bf2aec9a4fe9c58837ec84c2fc998a54ab7a77b52e109`  
		Last Modified: Wed, 13 Sep 2023 05:08:32 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e138a75d8a68c57acda5ac3d2a5ea38cfcd91aeeac6e996187886cdc4fe512b`  
		Last Modified: Wed, 13 Sep 2023 05:08:31 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ba6b3e055f188fc0c938c464d3df287b87b4ebd990c6d3023e4043e9475882b`  
		Last Modified: Wed, 13 Sep 2023 05:08:30 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733d1091bb5b201027155aa6154441b33e21f06c80c98e5502f0ea97d3e6ac36`  
		Last Modified: Wed, 13 Sep 2023 05:08:30 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98cf75715be616bda4fd455e8842d5c47e6361520831c79994aac63897f074a6`  
		Last Modified: Wed, 13 Sep 2023 05:08:30 GMT  
		Size: 242.8 KB (242766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3267078f67f5f3fb7955bda584f1a858622791ed81e9c2e45ac79383c6c3795`  
		Last Modified: Wed, 13 Sep 2023 05:08:30 GMT  
		Size: 5.8 MB (5779913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd81aab1223d4ac5fade6bcbff4e433f5a038988f73089bb43aff8b974c715a2`  
		Last Modified: Wed, 13 Sep 2023 05:08:28 GMT  
		Size: 2.0 KB (1985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a790db19f2a0d625636fa4d186b3b076500c592809d8b95c7a725e0c46a094`  
		Last Modified: Wed, 13 Sep 2023 05:08:28 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4edbf9880281abc4bccc4d818ad299ce3cd5ad235e1cb033fbc49b3096f3a7`  
		Last Modified: Wed, 13 Sep 2023 05:08:28 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c05fad63f054ab864e4484c552a76f82c3bf9e322da181d03f63a597755912`  
		Last Modified: Wed, 13 Sep 2023 05:08:28 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.22-windowsservercore-1809`

```console
$ docker pull nats@sha256:0d1237c42b0bf510367a68f73790bafd41d3e4dba95502ecf7d630eb6dcf0694
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `nats:2.9.22-windowsservercore-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats@sha256:4bc9d7dc99d75f7813148b82653c884ac51975085d49de22b68ac981bf1b3c40
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2022365856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5f7856c543b220cf294996bece7566b5515805212fc38127b1450f60b3e3ba5`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 03:56:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Sep 2023 05:05:36 GMT
ENV NATS_DOCKERIZED=1
# Wed, 13 Sep 2023 05:05:36 GMT
ENV NATS_SERVER=2.9.22
# Wed, 13 Sep 2023 05:05:37 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.22/nats-server-v2.9.22-windows-amd64.zip
# Wed, 13 Sep 2023 05:05:38 GMT
ENV NATS_SERVER_SHASUM=e91db73b02bd4dca3eb7a4bf32e29763450b08d593f73e87d0a6b70102dea0d4
# Wed, 13 Sep 2023 05:06:28 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 Sep 2023 05:07:52 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 13 Sep 2023 05:07:52 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 13 Sep 2023 05:07:53 GMT
EXPOSE 4222 6222 8222
# Wed, 13 Sep 2023 05:07:54 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Sep 2023 05:07:55 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b21bbf840142288ae2bce3465085b591133cf10f78f7dda43277db4838332d8`  
		Last Modified: Wed, 13 Sep 2023 04:36:45 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54f616fe064e9d4e73bf2aec9a4fe9c58837ec84c2fc998a54ab7a77b52e109`  
		Last Modified: Wed, 13 Sep 2023 05:08:32 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e138a75d8a68c57acda5ac3d2a5ea38cfcd91aeeac6e996187886cdc4fe512b`  
		Last Modified: Wed, 13 Sep 2023 05:08:31 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ba6b3e055f188fc0c938c464d3df287b87b4ebd990c6d3023e4043e9475882b`  
		Last Modified: Wed, 13 Sep 2023 05:08:30 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733d1091bb5b201027155aa6154441b33e21f06c80c98e5502f0ea97d3e6ac36`  
		Last Modified: Wed, 13 Sep 2023 05:08:30 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98cf75715be616bda4fd455e8842d5c47e6361520831c79994aac63897f074a6`  
		Last Modified: Wed, 13 Sep 2023 05:08:30 GMT  
		Size: 242.8 KB (242766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3267078f67f5f3fb7955bda584f1a858622791ed81e9c2e45ac79383c6c3795`  
		Last Modified: Wed, 13 Sep 2023 05:08:30 GMT  
		Size: 5.8 MB (5779913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd81aab1223d4ac5fade6bcbff4e433f5a038988f73089bb43aff8b974c715a2`  
		Last Modified: Wed, 13 Sep 2023 05:08:28 GMT  
		Size: 2.0 KB (1985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a790db19f2a0d625636fa4d186b3b076500c592809d8b95c7a725e0c46a094`  
		Last Modified: Wed, 13 Sep 2023 05:08:28 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4edbf9880281abc4bccc4d818ad299ce3cd5ad235e1cb033fbc49b3096f3a7`  
		Last Modified: Wed, 13 Sep 2023 05:08:28 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c05fad63f054ab864e4484c552a76f82c3bf9e322da181d03f63a597755912`  
		Last Modified: Wed, 13 Sep 2023 05:08:28 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:e9f41a4a8c1727e4a3ef9fdbff9cc963bfb88c7d77eaf946b2410e4f080e11c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:effbb639aba0db24ebaf3f42fe6e9201428fab869a9399897afeb797819e0a7d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9482934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7afe0964d1327c57759f61500b32db9d8337946f39bdc8264d0c0d8efef6921`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 20 Sep 2023 00:49:05 GMT
ENV NATS_SERVER=2.10.0
# Wed, 20 Sep 2023 00:49:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='59456ee8d222213c0f713e5b571156ec053db15288ee9035b3a7ad01e226c0bb' ;; 		armhf) natsArch='arm6'; sha256='c12c5cde86dba95fa4b433b58af3b9568893e3c7814fa22feae85eb47a9bb2bd' ;; 		armv7) natsArch='arm7'; sha256='748eb00c8d29c674bb4f98371a1afd8be9fba59336be9ef24d24fff148f1e7a4' ;; 		x86_64) natsArch='amd64'; sha256='76f5798ba3923dbc4f170bbae0055d3267d5c604179b2c644f6e7c79cc970d76' ;; 		x86) natsArch='386'; sha256='7f151267f76948293a5721e642b489e1135aecbeb2399dd23d00b04e6a609191' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 20 Sep 2023 00:49:08 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 20 Sep 2023 00:49:08 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 20 Sep 2023 00:49:08 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:49:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Sep 2023 00:49:08 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b04b7bc39016808990ede8996e6d82c3fd7375999baa7a075ce2b107276bd93`  
		Last Modified: Wed, 20 Sep 2023 00:49:47 GMT  
		Size: 6.1 MB (6080321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d9bfba1e3e94018e331b7feae544bb67022934ad7035d517856062cc8af6a2`  
		Last Modified: Wed, 20 Sep 2023 00:49:46 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a185a2d7152fec18042b0c2aaf92f7d8e6b4227691eb89b8cc180c1360a8cc`  
		Last Modified: Wed, 20 Sep 2023 00:49:46 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:84ff4ec4f07f6daee653039f475687b1fc9d518cfefd072fd7405c66708b2c52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8947432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ce27616fe886ff67930425f652c89bc5831f6566f233496b9f1269488d39bb9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Thu, 21 Sep 2023 00:07:43 GMT
ENV NATS_SERVER=2.10.1
# Thu, 21 Sep 2023 00:07:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='13ab69dd6b35b4e253e97f469b61c4038fb6c1d0de89df6dfc93f75af1728ace' ;; 		armhf) natsArch='arm6'; sha256='ad6da4b3289293624e1e60dd0c719d3f2c9cc768774b9f25e580c236915a906b' ;; 		armv7) natsArch='arm7'; sha256='9a706550622ce44f06e6cc44621c01aa27aa9f5da4347d4295e65e986b5cb907' ;; 		x86_64) natsArch='amd64'; sha256='f058d6195931f28cd14d2ac1b9b6a7ce1d760c66c76ccea72aa6b936f4b8d75c' ;; 		x86) natsArch='386'; sha256='1c1e82380139758a69b5040631890914a9db5234517ef9d82b0173e37b8ca96a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 21 Sep 2023 00:07:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 21 Sep 2023 00:07:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 21 Sep 2023 00:07:47 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 00:07:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Sep 2023 00:07:47 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f1a57b33f182668d91321a4367e03ea36a83b22cbb3512e7bf29a740166ac55`  
		Last Modified: Thu, 21 Sep 2023 00:08:27 GMT  
		Size: 5.8 MB (5801621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab09d7306f8d236dead5b1c5d7dfa7a6b386b8f86d77887da9405d0df4d4fd6`  
		Last Modified: Thu, 21 Sep 2023 00:08:25 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a037b525be2a5e8397e646ce00405c26939139fc529d945879cb727e772171`  
		Last Modified: Thu, 21 Sep 2023 00:08:25 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:793e82e82eb90127e5931e743d8b66fa93ce571aa7c3364b62fe1e8051397a0d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8694026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:029567069923892aa47d7aaf87e9018a5ad9406961686c368c467cef63fede5c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Wed, 20 Sep 2023 00:39:11 GMT
ENV NATS_SERVER=2.10.0
# Wed, 20 Sep 2023 00:39:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='59456ee8d222213c0f713e5b571156ec053db15288ee9035b3a7ad01e226c0bb' ;; 		armhf) natsArch='arm6'; sha256='c12c5cde86dba95fa4b433b58af3b9568893e3c7814fa22feae85eb47a9bb2bd' ;; 		armv7) natsArch='arm7'; sha256='748eb00c8d29c674bb4f98371a1afd8be9fba59336be9ef24d24fff148f1e7a4' ;; 		x86_64) natsArch='amd64'; sha256='76f5798ba3923dbc4f170bbae0055d3267d5c604179b2c644f6e7c79cc970d76' ;; 		x86) natsArch='386'; sha256='7f151267f76948293a5721e642b489e1135aecbeb2399dd23d00b04e6a609191' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 20 Sep 2023 00:39:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 20 Sep 2023 00:39:15 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 20 Sep 2023 00:39:15 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:39:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Sep 2023 00:39:15 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86cf505660fa5f57305b113eef333ce025a6d9136f88356db788061f3125927`  
		Last Modified: Wed, 20 Sep 2023 00:40:06 GMT  
		Size: 5.8 MB (5793543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7c97affb17c5049777a5f4c3748e8415a30d8e3fb1650078b3b33763877672`  
		Last Modified: Wed, 20 Sep 2023 00:40:05 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f28587da4e0140d1ee0d0f5fd63eb28e76cdbcc1cca375f6493d13f8fc404e`  
		Last Modified: Wed, 20 Sep 2023 00:40:05 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:2c90c42e3f08e748f4b37d4c85397f7434f2bc06f70f531348fd75f4981786a8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8984785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7d356a02623c8421e021ef35f15363a21ce68a6f855eeef311061f460fb4099`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Thu, 21 Sep 2023 05:04:42 GMT
ENV NATS_SERVER=2.10.1
# Thu, 21 Sep 2023 05:04:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='13ab69dd6b35b4e253e97f469b61c4038fb6c1d0de89df6dfc93f75af1728ace' ;; 		armhf) natsArch='arm6'; sha256='ad6da4b3289293624e1e60dd0c719d3f2c9cc768774b9f25e580c236915a906b' ;; 		armv7) natsArch='arm7'; sha256='9a706550622ce44f06e6cc44621c01aa27aa9f5da4347d4295e65e986b5cb907' ;; 		x86_64) natsArch='amd64'; sha256='f058d6195931f28cd14d2ac1b9b6a7ce1d760c66c76ccea72aa6b936f4b8d75c' ;; 		x86) natsArch='386'; sha256='1c1e82380139758a69b5040631890914a9db5234517ef9d82b0173e37b8ca96a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 21 Sep 2023 05:04:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 21 Sep 2023 05:04:44 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 21 Sep 2023 05:04:44 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 05:04:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Sep 2023 05:04:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36d636b74934d8449d366cac72e2a2f72e239d7a2b015bb861742b6954415a1`  
		Last Modified: Thu, 21 Sep 2023 05:05:42 GMT  
		Size: 5.7 MB (5653015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3918ce48c762d5088f364e86b7567e96b603661e7951055502a8186ffc9254`  
		Last Modified: Thu, 21 Sep 2023 05:05:41 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbe84c01f6bd1a347e498a6f38b3ca893236b40591ad8ae7eea2edfc50b9d99`  
		Last Modified: Thu, 21 Sep 2023 05:05:41 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.18`

```console
$ docker pull nats@sha256:e9f41a4a8c1727e4a3ef9fdbff9cc963bfb88c7d77eaf946b2410e4f080e11c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:effbb639aba0db24ebaf3f42fe6e9201428fab869a9399897afeb797819e0a7d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9482934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7afe0964d1327c57759f61500b32db9d8337946f39bdc8264d0c0d8efef6921`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 20 Sep 2023 00:49:05 GMT
ENV NATS_SERVER=2.10.0
# Wed, 20 Sep 2023 00:49:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='59456ee8d222213c0f713e5b571156ec053db15288ee9035b3a7ad01e226c0bb' ;; 		armhf) natsArch='arm6'; sha256='c12c5cde86dba95fa4b433b58af3b9568893e3c7814fa22feae85eb47a9bb2bd' ;; 		armv7) natsArch='arm7'; sha256='748eb00c8d29c674bb4f98371a1afd8be9fba59336be9ef24d24fff148f1e7a4' ;; 		x86_64) natsArch='amd64'; sha256='76f5798ba3923dbc4f170bbae0055d3267d5c604179b2c644f6e7c79cc970d76' ;; 		x86) natsArch='386'; sha256='7f151267f76948293a5721e642b489e1135aecbeb2399dd23d00b04e6a609191' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 20 Sep 2023 00:49:08 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 20 Sep 2023 00:49:08 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 20 Sep 2023 00:49:08 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:49:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Sep 2023 00:49:08 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b04b7bc39016808990ede8996e6d82c3fd7375999baa7a075ce2b107276bd93`  
		Last Modified: Wed, 20 Sep 2023 00:49:47 GMT  
		Size: 6.1 MB (6080321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d9bfba1e3e94018e331b7feae544bb67022934ad7035d517856062cc8af6a2`  
		Last Modified: Wed, 20 Sep 2023 00:49:46 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a185a2d7152fec18042b0c2aaf92f7d8e6b4227691eb89b8cc180c1360a8cc`  
		Last Modified: Wed, 20 Sep 2023 00:49:46 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:84ff4ec4f07f6daee653039f475687b1fc9d518cfefd072fd7405c66708b2c52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8947432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ce27616fe886ff67930425f652c89bc5831f6566f233496b9f1269488d39bb9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Thu, 21 Sep 2023 00:07:43 GMT
ENV NATS_SERVER=2.10.1
# Thu, 21 Sep 2023 00:07:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='13ab69dd6b35b4e253e97f469b61c4038fb6c1d0de89df6dfc93f75af1728ace' ;; 		armhf) natsArch='arm6'; sha256='ad6da4b3289293624e1e60dd0c719d3f2c9cc768774b9f25e580c236915a906b' ;; 		armv7) natsArch='arm7'; sha256='9a706550622ce44f06e6cc44621c01aa27aa9f5da4347d4295e65e986b5cb907' ;; 		x86_64) natsArch='amd64'; sha256='f058d6195931f28cd14d2ac1b9b6a7ce1d760c66c76ccea72aa6b936f4b8d75c' ;; 		x86) natsArch='386'; sha256='1c1e82380139758a69b5040631890914a9db5234517ef9d82b0173e37b8ca96a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 21 Sep 2023 00:07:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 21 Sep 2023 00:07:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 21 Sep 2023 00:07:47 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 00:07:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Sep 2023 00:07:47 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f1a57b33f182668d91321a4367e03ea36a83b22cbb3512e7bf29a740166ac55`  
		Last Modified: Thu, 21 Sep 2023 00:08:27 GMT  
		Size: 5.8 MB (5801621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab09d7306f8d236dead5b1c5d7dfa7a6b386b8f86d77887da9405d0df4d4fd6`  
		Last Modified: Thu, 21 Sep 2023 00:08:25 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a037b525be2a5e8397e646ce00405c26939139fc529d945879cb727e772171`  
		Last Modified: Thu, 21 Sep 2023 00:08:25 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:793e82e82eb90127e5931e743d8b66fa93ce571aa7c3364b62fe1e8051397a0d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8694026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:029567069923892aa47d7aaf87e9018a5ad9406961686c368c467cef63fede5c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Wed, 20 Sep 2023 00:39:11 GMT
ENV NATS_SERVER=2.10.0
# Wed, 20 Sep 2023 00:39:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='59456ee8d222213c0f713e5b571156ec053db15288ee9035b3a7ad01e226c0bb' ;; 		armhf) natsArch='arm6'; sha256='c12c5cde86dba95fa4b433b58af3b9568893e3c7814fa22feae85eb47a9bb2bd' ;; 		armv7) natsArch='arm7'; sha256='748eb00c8d29c674bb4f98371a1afd8be9fba59336be9ef24d24fff148f1e7a4' ;; 		x86_64) natsArch='amd64'; sha256='76f5798ba3923dbc4f170bbae0055d3267d5c604179b2c644f6e7c79cc970d76' ;; 		x86) natsArch='386'; sha256='7f151267f76948293a5721e642b489e1135aecbeb2399dd23d00b04e6a609191' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 20 Sep 2023 00:39:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 20 Sep 2023 00:39:15 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 20 Sep 2023 00:39:15 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:39:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Sep 2023 00:39:15 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86cf505660fa5f57305b113eef333ce025a6d9136f88356db788061f3125927`  
		Last Modified: Wed, 20 Sep 2023 00:40:06 GMT  
		Size: 5.8 MB (5793543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7c97affb17c5049777a5f4c3748e8415a30d8e3fb1650078b3b33763877672`  
		Last Modified: Wed, 20 Sep 2023 00:40:05 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f28587da4e0140d1ee0d0f5fd63eb28e76cdbcc1cca375f6493d13f8fc404e`  
		Last Modified: Wed, 20 Sep 2023 00:40:05 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:2c90c42e3f08e748f4b37d4c85397f7434f2bc06f70f531348fd75f4981786a8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8984785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7d356a02623c8421e021ef35f15363a21ce68a6f855eeef311061f460fb4099`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Thu, 21 Sep 2023 05:04:42 GMT
ENV NATS_SERVER=2.10.1
# Thu, 21 Sep 2023 05:04:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='13ab69dd6b35b4e253e97f469b61c4038fb6c1d0de89df6dfc93f75af1728ace' ;; 		armhf) natsArch='arm6'; sha256='ad6da4b3289293624e1e60dd0c719d3f2c9cc768774b9f25e580c236915a906b' ;; 		armv7) natsArch='arm7'; sha256='9a706550622ce44f06e6cc44621c01aa27aa9f5da4347d4295e65e986b5cb907' ;; 		x86_64) natsArch='amd64'; sha256='f058d6195931f28cd14d2ac1b9b6a7ce1d760c66c76ccea72aa6b936f4b8d75c' ;; 		x86) natsArch='386'; sha256='1c1e82380139758a69b5040631890914a9db5234517ef9d82b0173e37b8ca96a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 21 Sep 2023 05:04:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 21 Sep 2023 05:04:44 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 21 Sep 2023 05:04:44 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 05:04:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Sep 2023 05:04:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36d636b74934d8449d366cac72e2a2f72e239d7a2b015bb861742b6954415a1`  
		Last Modified: Thu, 21 Sep 2023 05:05:42 GMT  
		Size: 5.7 MB (5653015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3918ce48c762d5088f364e86b7567e96b603661e7951055502a8186ffc9254`  
		Last Modified: Thu, 21 Sep 2023 05:05:41 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbe84c01f6bd1a347e498a6f38b3ca893236b40591ad8ae7eea2edfc50b9d99`  
		Last Modified: Thu, 21 Sep 2023 05:05:41 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:4c435644375188d384b184b05252331e4b7ba29a59eec81ba067e2ccab93a00d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4851; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:300b8159816cb200b0ddca347e2895e811131e89660b698819d6a04d017b51ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5457759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f5b65974bc0ab52f1a6bd8c018ff5fadadbc976f311db512c19acabce037b94`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 20 Sep 2023 00:49:23 GMT
COPY file:8e2a9a3f381167fcc1a95dc7718c10cb67f58a845a3197193a5273c57e28d08d in /nats-server 
# Wed, 20 Sep 2023 00:49:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 20 Sep 2023 00:49:23 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:49:23 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Sep 2023 00:49:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:949cbe9ff3fb07dc0fbd1c6fb6ba4a1c20304c28d574891f79f5d84e05439ec0`  
		Last Modified: Wed, 20 Sep 2023 00:50:22 GMT  
		Size: 5.5 MB (5457252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49c9fc5d845768deddd7c19342fd407ee4fdc4d110abf53e58444440c552181`  
		Last Modified: Wed, 20 Sep 2023 00:50:21 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:2a08a0c1d913294be585667f17f76f028053f5bf47b9d317e5bc0e409011ed1e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5245282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3517f7b93c37103553431effcb0b5a8262feb87c3649b04249d86012c34a9761`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 20 Sep 2023 00:49:17 GMT
COPY file:acdb0e47969d6e334bcadb9c85dfef3166c764ff4ac55254185a04b1a6e8bbee in /nats-server 
# Wed, 20 Sep 2023 00:49:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 20 Sep 2023 00:49:17 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:49:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Sep 2023 00:49:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aac801db9a2a97942dde4494f98ce2d08c529a3af03ecb92f0b93426bbfd6419`  
		Last Modified: Wed, 06 Sep 2023 23:20:56 GMT  
		Size: 5.2 MB (5244773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1646134cd3aac5e501d3658b95fcfd870fb902c4c9591a801a5b370a5aa574`  
		Last Modified: Wed, 20 Sep 2023 00:50:09 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:cce3ff90a32531db64bb74852140a156326d487dafbf812da2168f78c0e85388
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5178106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:111b8fef881498596233d1f7dda3dc1a4113c72bfe5e1088ded56d10a45d128f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 21 Sep 2023 00:07:58 GMT
COPY file:dbe6aeea160dba3a7bdcaf0c14808f7a7b31899bb87a50ed117996ead07014e6 in /nats-server 
# Thu, 21 Sep 2023 00:07:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 21 Sep 2023 00:07:58 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 00:07:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 21 Sep 2023 00:07:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6837114cbc023e4b8b17b6a951b2e91ab9668a1f3ffe65bec26f4ea44b812845`  
		Last Modified: Thu, 21 Sep 2023 00:08:53 GMT  
		Size: 5.2 MB (5177597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bde9589f631b3debf2ce00b1154c597464aeb530aac8a0016d7bee37f972958`  
		Last Modified: Thu, 21 Sep 2023 00:08:51 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:4f09dbc6c43267500545fe441ec8057908d1b6bab5333c432c5e3d4c7ea0fd58
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4980014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:898dfa8e8c4c3e0c69c7c3aec16c90f1f6db172f3af0e7ff763b3bf8db42ed3c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Sep 2023 23:49:29 GMT
COPY file:51aacaba9769a3f16e0467be1fc8eb86122f6f3496e89e41b61e0038083ae308 in /nats-server 
# Tue, 19 Sep 2023 23:49:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Sep 2023 23:49:29 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Sep 2023 23:49:29 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Sep 2023 23:49:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6a6e165fccf6da77ad3b09408162fc7daaafe266b71dd5da8679594aa110a3a5`  
		Last Modified: Wed, 06 Sep 2023 23:05:32 GMT  
		Size: 5.0 MB (4979506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07c6021b659fa78c25ff92ad1e74c46e34c95c5e691ca45f27ced97ea7ef9e2`  
		Last Modified: Tue, 19 Sep 2023 23:50:15 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:41b2a21a345689e5edc4cb8d24444c46df161e58ca89578e66a66e2e0aee2a47
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5171757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed343d1334d5c6f933acaae9f280c90acde044ea41eb6047dc9126ecd17dbd37`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 20 Sep 2023 00:39:39 GMT
COPY file:1ed1e6185c40930f2dc5e0e072cf3d42764ec8f3c10b2f65c3044c6aaf6d5ac5 in /nats-server 
# Wed, 20 Sep 2023 00:39:39 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 20 Sep 2023 00:39:39 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:39:40 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Sep 2023 00:39:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9af7ee06c60cdf35e2e953e1ad5700cf513329b5f88bb07096c8439fbdd7cfb4`  
		Last Modified: Wed, 20 Sep 2023 00:40:42 GMT  
		Size: 5.2 MB (5171248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5795401da82ad77eec35f59034d9f5ce5ff6af93cc82c2a00277bf954ef32c2`  
		Last Modified: Wed, 20 Sep 2023 00:40:41 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:64211266fe0d926796dae72e7484f5aebbdb77c7e7faa3fab3d01954fe03a82e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4970849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a40010bd31b571ac24ead3a8630fa80ce8609b0352d5dab096c6b72940be90a6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 20 Sep 2023 00:39:32 GMT
COPY file:aae670bb79c659968f632ae3be388af62614010873ced2a439475906dbb769c6 in /nats-server 
# Wed, 20 Sep 2023 00:39:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 20 Sep 2023 00:39:32 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:39:32 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Sep 2023 00:39:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:55b6dbad6639da13368cebb9688e8a5caaee29041e6b5e2e798201dfcf2b67ad`  
		Last Modified: Wed, 06 Sep 2023 22:58:23 GMT  
		Size: 5.0 MB (4970341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969097b6afede4aab7deed51f12918311993aadbe7075d4965c14497831f4a12`  
		Last Modified: Wed, 20 Sep 2023 00:40:29 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:e6aea49e5eb407c078286700c1402c6eda155ae11cdd40f8604194f6f70d0dd2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5029479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d109a8655a05cb22d5529db631b1a167bfae974cfc5d047c1ac261888ecd6e8`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 21 Sep 2023 05:05:18 GMT
COPY file:943544393eb61c235711dc43a87ec667d4491be8bcff70eee560d8276bd01b5b in /nats-server 
# Thu, 21 Sep 2023 05:05:18 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 21 Sep 2023 05:05:18 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 05:05:18 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 21 Sep 2023 05:05:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:85892a63e455fd1561bc50ef513a999a9a22152bbab4f029732ea77658da0b37`  
		Last Modified: Thu, 21 Sep 2023 05:06:05 GMT  
		Size: 5.0 MB (5028971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24d6a1649b69be08c681087d8f2f84e750824c24acb44b6d1be0a9a706bb112`  
		Last Modified: Thu, 21 Sep 2023 05:06:04 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:91e7a991da679db1020b25a760298f6944a9ea917e9ae90f10d1d7de9381fec4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4778849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb1745f4f81f20c728e9276ed07416c88490859cdbed438bdcb68aa051eb586c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Sep 2023 23:42:56 GMT
COPY file:d6eca5c67de65d1a8a30a51ea7318b044949c77108b2fdccc5aa0054c068c196 in /nats-server 
# Tue, 19 Sep 2023 23:42:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Sep 2023 23:42:56 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Sep 2023 23:42:56 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Sep 2023 23:42:56 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:88e5ff7f26ea25c6d2ab092989d9372cb32b3e60880124facfcefd7d3f0b7591`  
		Last Modified: Wed, 06 Sep 2023 22:40:49 GMT  
		Size: 4.8 MB (4778340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2424880e07e944598022ff8713b5897eb59c72af17978f7a3f1afa42dd022088`  
		Last Modified: Tue, 19 Sep 2023 23:43:51 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats@sha256:3ae7b24041d5c7f8bb775c1fd47da96b2891f8c6821bfe25f6bcf95a0eaf6064
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110068360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acf1d87f97e43bca95d8940d4aa3abf65c2c05adb6681005cb66f3f7d8001ffc`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Aug 2023 16:42:02 GMT
RUN Apply image 10.0.17763.4851
# Wed, 13 Sep 2023 05:08:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 21 Sep 2023 00:18:29 GMT
RUN cmd /S /C #(nop) COPY file:2b24d029bdf2310dcf6089c8f58986b6c70babf4fd4d433f329957862df58d77 in C:\nats-server.exe 
# Thu, 21 Sep 2023 00:18:29 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 21 Sep 2023 00:18:30 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 00:18:31 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 21 Sep 2023 00:18:31 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:17ba6b878467260559b72cb6f7e79c829eae67862a09efe87f6dc324f49fc086`  
		Last Modified: Tue, 12 Sep 2023 18:31:40 GMT  
		Size: 104.5 MB (104492504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9930674eb6676a1690e63a275d0da517ab8b8aeab7ccd20591f76f7c69a5`  
		Last Modified: Wed, 13 Sep 2023 05:08:48 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05405503d7afb6019521e5fa013d09e5c8636161e9408ba36c149f4853898e7`  
		Last Modified: Thu, 21 Sep 2023 00:19:36 GMT  
		Size: 5.6 MB (5569390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d1f97d2316001518d35eb0b75ac1888c2fe2da51ce49c16012d2fef9ccf5e0c`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.8 KB (1802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6a311706a8aadd91f05c001d3ffbd3a548f21286d0db22eed44fcd5999100f`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a3c2ef4f82e001ae8c4b096641708c8d404bd43dae8f46f843d21d8bb0fd69`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1a063be69428345c92d570f896ffe0326401a9b501ba554a0c4ebf8dc1f5dd`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:279c3e1bc63c82126abafed2b06ae0c23cfe06d526db00f0cd2bf790595b1e53
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:300b8159816cb200b0ddca347e2895e811131e89660b698819d6a04d017b51ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5457759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f5b65974bc0ab52f1a6bd8c018ff5fadadbc976f311db512c19acabce037b94`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 20 Sep 2023 00:49:23 GMT
COPY file:8e2a9a3f381167fcc1a95dc7718c10cb67f58a845a3197193a5273c57e28d08d in /nats-server 
# Wed, 20 Sep 2023 00:49:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 20 Sep 2023 00:49:23 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:49:23 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Sep 2023 00:49:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:949cbe9ff3fb07dc0fbd1c6fb6ba4a1c20304c28d574891f79f5d84e05439ec0`  
		Last Modified: Wed, 20 Sep 2023 00:50:22 GMT  
		Size: 5.5 MB (5457252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49c9fc5d845768deddd7c19342fd407ee4fdc4d110abf53e58444440c552181`  
		Last Modified: Wed, 20 Sep 2023 00:50:21 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:cce3ff90a32531db64bb74852140a156326d487dafbf812da2168f78c0e85388
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5178106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:111b8fef881498596233d1f7dda3dc1a4113c72bfe5e1088ded56d10a45d128f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 21 Sep 2023 00:07:58 GMT
COPY file:dbe6aeea160dba3a7bdcaf0c14808f7a7b31899bb87a50ed117996ead07014e6 in /nats-server 
# Thu, 21 Sep 2023 00:07:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 21 Sep 2023 00:07:58 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 00:07:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 21 Sep 2023 00:07:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6837114cbc023e4b8b17b6a951b2e91ab9668a1f3ffe65bec26f4ea44b812845`  
		Last Modified: Thu, 21 Sep 2023 00:08:53 GMT  
		Size: 5.2 MB (5177597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bde9589f631b3debf2ce00b1154c597464aeb530aac8a0016d7bee37f972958`  
		Last Modified: Thu, 21 Sep 2023 00:08:51 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:41b2a21a345689e5edc4cb8d24444c46df161e58ca89578e66a66e2e0aee2a47
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5171757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed343d1334d5c6f933acaae9f280c90acde044ea41eb6047dc9126ecd17dbd37`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 20 Sep 2023 00:39:39 GMT
COPY file:1ed1e6185c40930f2dc5e0e072cf3d42764ec8f3c10b2f65c3044c6aaf6d5ac5 in /nats-server 
# Wed, 20 Sep 2023 00:39:39 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 20 Sep 2023 00:39:39 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:39:40 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Sep 2023 00:39:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9af7ee06c60cdf35e2e953e1ad5700cf513329b5f88bb07096c8439fbdd7cfb4`  
		Last Modified: Wed, 20 Sep 2023 00:40:42 GMT  
		Size: 5.2 MB (5171248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5795401da82ad77eec35f59034d9f5ce5ff6af93cc82c2a00277bf954ef32c2`  
		Last Modified: Wed, 20 Sep 2023 00:40:41 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:e6aea49e5eb407c078286700c1402c6eda155ae11cdd40f8604194f6f70d0dd2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5029479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d109a8655a05cb22d5529db631b1a167bfae974cfc5d047c1ac261888ecd6e8`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 21 Sep 2023 05:05:18 GMT
COPY file:943544393eb61c235711dc43a87ec667d4491be8bcff70eee560d8276bd01b5b in /nats-server 
# Thu, 21 Sep 2023 05:05:18 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 21 Sep 2023 05:05:18 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 05:05:18 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 21 Sep 2023 05:05:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:85892a63e455fd1561bc50ef513a999a9a22152bbab4f029732ea77658da0b37`  
		Last Modified: Thu, 21 Sep 2023 05:06:05 GMT  
		Size: 5.0 MB (5028971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24d6a1649b69be08c681087d8f2f84e750824c24acb44b6d1be0a9a706bb112`  
		Last Modified: Thu, 21 Sep 2023 05:06:04 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:6670fad4a4d64481de5425c7a8ee8e602faef2f05646051096bfa59d9126cbfb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `nats:nanoserver` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats@sha256:3ae7b24041d5c7f8bb775c1fd47da96b2891f8c6821bfe25f6bcf95a0eaf6064
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110068360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acf1d87f97e43bca95d8940d4aa3abf65c2c05adb6681005cb66f3f7d8001ffc`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Aug 2023 16:42:02 GMT
RUN Apply image 10.0.17763.4851
# Wed, 13 Sep 2023 05:08:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 21 Sep 2023 00:18:29 GMT
RUN cmd /S /C #(nop) COPY file:2b24d029bdf2310dcf6089c8f58986b6c70babf4fd4d433f329957862df58d77 in C:\nats-server.exe 
# Thu, 21 Sep 2023 00:18:29 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 21 Sep 2023 00:18:30 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 00:18:31 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 21 Sep 2023 00:18:31 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:17ba6b878467260559b72cb6f7e79c829eae67862a09efe87f6dc324f49fc086`  
		Last Modified: Tue, 12 Sep 2023 18:31:40 GMT  
		Size: 104.5 MB (104492504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9930674eb6676a1690e63a275d0da517ab8b8aeab7ccd20591f76f7c69a5`  
		Last Modified: Wed, 13 Sep 2023 05:08:48 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05405503d7afb6019521e5fa013d09e5c8636161e9408ba36c149f4853898e7`  
		Last Modified: Thu, 21 Sep 2023 00:19:36 GMT  
		Size: 5.6 MB (5569390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d1f97d2316001518d35eb0b75ac1888c2fe2da51ce49c16012d2fef9ccf5e0c`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.8 KB (1802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6a311706a8aadd91f05c001d3ffbd3a548f21286d0db22eed44fcd5999100f`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a3c2ef4f82e001ae8c4b096641708c8d404bd43dae8f46f843d21d8bb0fd69`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1a063be69428345c92d570f896ffe0326401a9b501ba554a0c4ebf8dc1f5dd`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:6670fad4a4d64481de5425c7a8ee8e602faef2f05646051096bfa59d9126cbfb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats@sha256:3ae7b24041d5c7f8bb775c1fd47da96b2891f8c6821bfe25f6bcf95a0eaf6064
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110068360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acf1d87f97e43bca95d8940d4aa3abf65c2c05adb6681005cb66f3f7d8001ffc`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Aug 2023 16:42:02 GMT
RUN Apply image 10.0.17763.4851
# Wed, 13 Sep 2023 05:08:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 21 Sep 2023 00:18:29 GMT
RUN cmd /S /C #(nop) COPY file:2b24d029bdf2310dcf6089c8f58986b6c70babf4fd4d433f329957862df58d77 in C:\nats-server.exe 
# Thu, 21 Sep 2023 00:18:29 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 21 Sep 2023 00:18:30 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 00:18:31 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 21 Sep 2023 00:18:31 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:17ba6b878467260559b72cb6f7e79c829eae67862a09efe87f6dc324f49fc086`  
		Last Modified: Tue, 12 Sep 2023 18:31:40 GMT  
		Size: 104.5 MB (104492504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9930674eb6676a1690e63a275d0da517ab8b8aeab7ccd20591f76f7c69a5`  
		Last Modified: Wed, 13 Sep 2023 05:08:48 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05405503d7afb6019521e5fa013d09e5c8636161e9408ba36c149f4853898e7`  
		Last Modified: Thu, 21 Sep 2023 00:19:36 GMT  
		Size: 5.6 MB (5569390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d1f97d2316001518d35eb0b75ac1888c2fe2da51ce49c16012d2fef9ccf5e0c`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.8 KB (1802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6a311706a8aadd91f05c001d3ffbd3a548f21286d0db22eed44fcd5999100f`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a3c2ef4f82e001ae8c4b096641708c8d404bd43dae8f46f843d21d8bb0fd69`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1a063be69428345c92d570f896ffe0326401a9b501ba554a0c4ebf8dc1f5dd`  
		Last Modified: Thu, 21 Sep 2023 00:19:35 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:279c3e1bc63c82126abafed2b06ae0c23cfe06d526db00f0cd2bf790595b1e53
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:300b8159816cb200b0ddca347e2895e811131e89660b698819d6a04d017b51ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5457759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f5b65974bc0ab52f1a6bd8c018ff5fadadbc976f311db512c19acabce037b94`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 20 Sep 2023 00:49:23 GMT
COPY file:8e2a9a3f381167fcc1a95dc7718c10cb67f58a845a3197193a5273c57e28d08d in /nats-server 
# Wed, 20 Sep 2023 00:49:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 20 Sep 2023 00:49:23 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:49:23 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Sep 2023 00:49:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:949cbe9ff3fb07dc0fbd1c6fb6ba4a1c20304c28d574891f79f5d84e05439ec0`  
		Last Modified: Wed, 20 Sep 2023 00:50:22 GMT  
		Size: 5.5 MB (5457252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49c9fc5d845768deddd7c19342fd407ee4fdc4d110abf53e58444440c552181`  
		Last Modified: Wed, 20 Sep 2023 00:50:21 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:cce3ff90a32531db64bb74852140a156326d487dafbf812da2168f78c0e85388
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5178106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:111b8fef881498596233d1f7dda3dc1a4113c72bfe5e1088ded56d10a45d128f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 21 Sep 2023 00:07:58 GMT
COPY file:dbe6aeea160dba3a7bdcaf0c14808f7a7b31899bb87a50ed117996ead07014e6 in /nats-server 
# Thu, 21 Sep 2023 00:07:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 21 Sep 2023 00:07:58 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 00:07:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 21 Sep 2023 00:07:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6837114cbc023e4b8b17b6a951b2e91ab9668a1f3ffe65bec26f4ea44b812845`  
		Last Modified: Thu, 21 Sep 2023 00:08:53 GMT  
		Size: 5.2 MB (5177597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bde9589f631b3debf2ce00b1154c597464aeb530aac8a0016d7bee37f972958`  
		Last Modified: Thu, 21 Sep 2023 00:08:51 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:41b2a21a345689e5edc4cb8d24444c46df161e58ca89578e66a66e2e0aee2a47
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5171757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed343d1334d5c6f933acaae9f280c90acde044ea41eb6047dc9126ecd17dbd37`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 20 Sep 2023 00:39:39 GMT
COPY file:1ed1e6185c40930f2dc5e0e072cf3d42764ec8f3c10b2f65c3044c6aaf6d5ac5 in /nats-server 
# Wed, 20 Sep 2023 00:39:39 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 20 Sep 2023 00:39:39 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:39:40 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Sep 2023 00:39:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9af7ee06c60cdf35e2e953e1ad5700cf513329b5f88bb07096c8439fbdd7cfb4`  
		Last Modified: Wed, 20 Sep 2023 00:40:42 GMT  
		Size: 5.2 MB (5171248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5795401da82ad77eec35f59034d9f5ce5ff6af93cc82c2a00277bf954ef32c2`  
		Last Modified: Wed, 20 Sep 2023 00:40:41 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:e6aea49e5eb407c078286700c1402c6eda155ae11cdd40f8604194f6f70d0dd2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5029479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d109a8655a05cb22d5529db631b1a167bfae974cfc5d047c1ac261888ecd6e8`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 21 Sep 2023 05:05:18 GMT
COPY file:943544393eb61c235711dc43a87ec667d4491be8bcff70eee560d8276bd01b5b in /nats-server 
# Thu, 21 Sep 2023 05:05:18 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 21 Sep 2023 05:05:18 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 05:05:18 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 21 Sep 2023 05:05:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:85892a63e455fd1561bc50ef513a999a9a22152bbab4f029732ea77658da0b37`  
		Last Modified: Thu, 21 Sep 2023 05:06:05 GMT  
		Size: 5.0 MB (5028971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24d6a1649b69be08c681087d8f2f84e750824c24acb44b6d1be0a9a706bb112`  
		Last Modified: Thu, 21 Sep 2023 05:06:04 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:caacdd68ac15825419bdd0d1ed333408d4c22b3a26035275e48d153c22268c1c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `nats:windowsservercore` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats@sha256:6a50e306cf3f0c7dbd1e2df340d2696b1622ad3232c7d83cb0d1f72195089ca5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2022614730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f82b912330f09e1d0a6d64e3034e0da94f54645b45b8713a83652480b2bea1b5`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 03:56:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Sep 2023 05:05:36 GMT
ENV NATS_DOCKERIZED=1
# Thu, 21 Sep 2023 00:15:15 GMT
ENV NATS_SERVER=2.10.1
# Thu, 21 Sep 2023 00:15:15 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.10.1/nats-server-v2.10.1-windows-amd64.zip
# Thu, 21 Sep 2023 00:15:16 GMT
ENV NATS_SERVER_SHASUM=88f2990dd6fea0bb2d8ba5cfde41ab5c96dd01bbaf4f9e9a3569815a0803cb1c
# Thu, 21 Sep 2023 00:16:19 GMT
RUN Set-PSDebug -Trace 2
# Thu, 21 Sep 2023 00:18:04 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 21 Sep 2023 00:18:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 21 Sep 2023 00:18:06 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 00:18:07 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 21 Sep 2023 00:18:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b21bbf840142288ae2bce3465085b591133cf10f78f7dda43277db4838332d8`  
		Last Modified: Wed, 13 Sep 2023 04:36:45 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54f616fe064e9d4e73bf2aec9a4fe9c58837ec84c2fc998a54ab7a77b52e109`  
		Last Modified: Wed, 13 Sep 2023 05:08:32 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905f26828615c039d9da3e9f52c8b61ad3b2183a7ec3940bb1985bfc9a64be81`  
		Last Modified: Thu, 21 Sep 2023 00:19:20 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a235c3fc87ed07702e70bb83fcbcb5ccaf81440d9ffd8d450d16bb7f273ce0`  
		Last Modified: Thu, 21 Sep 2023 00:19:20 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759a393cccf186a4709cd9d0c4da137cade59a534bc53125be57217f7b21ef61`  
		Last Modified: Thu, 21 Sep 2023 00:19:20 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1cc61521de3ff29def7a6479a78dc7165d144b87f68e455eedb1ed30775aeaa`  
		Last Modified: Thu, 21 Sep 2023 00:19:20 GMT  
		Size: 242.8 KB (242789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d014e00481cb1e60003ba14c0a143d5126a763b4d413032ddad39559313825d`  
		Last Modified: Thu, 21 Sep 2023 00:19:19 GMT  
		Size: 6.0 MB (6028853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ba83a190b4d5c219eab28b93cc94ab37e1a941e7270d4e60b5114f037589da`  
		Last Modified: Thu, 21 Sep 2023 00:19:18 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9ab4d57441cb1024559b87812361354ac635647bdb46a4ea450769c671d6f2`  
		Last Modified: Thu, 21 Sep 2023 00:19:18 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd0e1cd2f7b50ded5cab327e6c888492fb4c4e022a0062cc719b9b6f9bcd8f4`  
		Last Modified: Thu, 21 Sep 2023 00:19:18 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca70f3129ad44afad7b489a20cfd3a7bd2187694d47690907dab50fc4638c34`  
		Last Modified: Thu, 21 Sep 2023 00:19:18 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:caacdd68ac15825419bdd0d1ed333408d4c22b3a26035275e48d153c22268c1c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats@sha256:6a50e306cf3f0c7dbd1e2df340d2696b1622ad3232c7d83cb0d1f72195089ca5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2022614730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f82b912330f09e1d0a6d64e3034e0da94f54645b45b8713a83652480b2bea1b5`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 03:56:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Sep 2023 05:05:36 GMT
ENV NATS_DOCKERIZED=1
# Thu, 21 Sep 2023 00:15:15 GMT
ENV NATS_SERVER=2.10.1
# Thu, 21 Sep 2023 00:15:15 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.10.1/nats-server-v2.10.1-windows-amd64.zip
# Thu, 21 Sep 2023 00:15:16 GMT
ENV NATS_SERVER_SHASUM=88f2990dd6fea0bb2d8ba5cfde41ab5c96dd01bbaf4f9e9a3569815a0803cb1c
# Thu, 21 Sep 2023 00:16:19 GMT
RUN Set-PSDebug -Trace 2
# Thu, 21 Sep 2023 00:18:04 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 21 Sep 2023 00:18:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 21 Sep 2023 00:18:06 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 00:18:07 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 21 Sep 2023 00:18:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b21bbf840142288ae2bce3465085b591133cf10f78f7dda43277db4838332d8`  
		Last Modified: Wed, 13 Sep 2023 04:36:45 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54f616fe064e9d4e73bf2aec9a4fe9c58837ec84c2fc998a54ab7a77b52e109`  
		Last Modified: Wed, 13 Sep 2023 05:08:32 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905f26828615c039d9da3e9f52c8b61ad3b2183a7ec3940bb1985bfc9a64be81`  
		Last Modified: Thu, 21 Sep 2023 00:19:20 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a235c3fc87ed07702e70bb83fcbcb5ccaf81440d9ffd8d450d16bb7f273ce0`  
		Last Modified: Thu, 21 Sep 2023 00:19:20 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759a393cccf186a4709cd9d0c4da137cade59a534bc53125be57217f7b21ef61`  
		Last Modified: Thu, 21 Sep 2023 00:19:20 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1cc61521de3ff29def7a6479a78dc7165d144b87f68e455eedb1ed30775aeaa`  
		Last Modified: Thu, 21 Sep 2023 00:19:20 GMT  
		Size: 242.8 KB (242789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d014e00481cb1e60003ba14c0a143d5126a763b4d413032ddad39559313825d`  
		Last Modified: Thu, 21 Sep 2023 00:19:19 GMT  
		Size: 6.0 MB (6028853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ba83a190b4d5c219eab28b93cc94ab37e1a941e7270d4e60b5114f037589da`  
		Last Modified: Thu, 21 Sep 2023 00:19:18 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9ab4d57441cb1024559b87812361354ac635647bdb46a4ea450769c671d6f2`  
		Last Modified: Thu, 21 Sep 2023 00:19:18 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd0e1cd2f7b50ded5cab327e6c888492fb4c4e022a0062cc719b9b6f9bcd8f4`  
		Last Modified: Thu, 21 Sep 2023 00:19:18 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca70f3129ad44afad7b489a20cfd3a7bd2187694d47690907dab50fc4638c34`  
		Last Modified: Thu, 21 Sep 2023 00:19:18 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
